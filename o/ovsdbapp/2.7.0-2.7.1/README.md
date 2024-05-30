# Comparing `tmp/ovsdbapp-2.7.0.tar.gz` & `tmp/ovsdbapp-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovsdbapp-2.7.0.tar", last modified: Thu May 16 13:07:06 2024, max compression
+gzip compressed data, was "ovsdbapp-2.7.1.tar", last modified: Mon May 20 18:55:28 2024, max compression
```

## Comparing `ovsdbapp-2.7.0.tar` & `ovsdbapp-2.7.1.tar`

### file list

```diff
@@ -1,198 +1,199 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4111 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3648 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18052 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2042 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/TESTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2670 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/user/overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4840 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/user/tutorial.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.164367 ovsdbapp-2.7.0/ovsdbapp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/CHANGES
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.168369 ovsdbapp-2.7.0/ovsdbapp/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9364 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14070 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/command.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8119 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16687 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/idlutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/rowview.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5256 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/transaction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3320 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/vlog.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6596 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7885 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9755 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.176374 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8593 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13455 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5614 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.176374 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2179 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.176374 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    60641 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    75757 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18489 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.176374 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4648 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15722 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6227 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   116548 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7393 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.188381 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12330 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2715 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.188381 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.188381 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3026 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11749 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/venv.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.168369 ovsdbapp-2.7.0/ovsdbapp.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5999 2024-05-16 13:07:06.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.156362 ovsdbapp-2.7.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.192383 ovsdbapp-2.7.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/configure-ovsdb-manager-a29a148b241a125e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/drop-py27-support-c426980520444bfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/drop-python-3-6-and-3-7-8ae8ccf16e422fc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/ovn-support-allow-stateless-01aed5acdcd1c0d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/ovn-support-discard-nexthop-cdb1d35aceaf4b63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/ovn-support-hw-vtep-ca8b3ee7a74df3fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/ovn-support-ic-northbound-df557a866a1f411f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-address-set-api-3cb387b9e571d4ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-lb-hc-api-8ff13ccaf75f1eee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-lrp-gateway-chassis-api-14e2948183f60cfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-lrp-get-method-a33a99a7f86b827e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-lrp-networks-modifying-1af13589064c12c6.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/2023.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/2024.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7768 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-05-16 13:07:06.200388 ovsdbapp-2.7.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1863 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1774 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/debug_venv
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1735 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/debug_venv.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      509 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/setup-ovs.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      278 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/zuul.d/ovsdbapp-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.470827 ovsdbapp-2.7.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4111 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3679 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18178 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2024-05-20 18:55:28.470827 ovsdbapp-2.7.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2042 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/TESTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.438819 ovsdbapp-2.7.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.438819 ovsdbapp-2.7.1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2670 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.438819 ovsdbapp-2.7.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.438819 ovsdbapp-2.7.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.438819 ovsdbapp-2.7.1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/doc/source/user/overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4840 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/doc/source/user/tutorial.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.438819 ovsdbapp-2.7.1/ovsdbapp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/CHANGES
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.442820 ovsdbapp-2.7.1/ovsdbapp/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.442820 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9364 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14252 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/command.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.446821 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8119 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16687 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/idlutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.446821 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/linux/connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/rowview.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5256 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/transaction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3320 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/vlog.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.446821 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/windows/connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/windows/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6596 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.446821 ovsdbapp-2.7.1/ovsdbapp/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.446821 ovsdbapp-2.7.1/ovsdbapp/schema/hardware_vtep/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/hardware_vtep/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7885 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/hardware_vtep/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9755 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/hardware_vtep/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/hardware_vtep/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.446821 ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8593 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13455 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5614 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.450822 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_ic_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_ic_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2179 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_ic_northbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_ic_northbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.450822 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60815 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_northbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    75757 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_northbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18517 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_northbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.450822 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_southbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_southbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_southbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4648 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_southbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/schema/ovn_southbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.450822 ovsdbapp-2.7.1/ovsdbapp/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.450822 ovsdbapp-2.7.1/ovsdbapp/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.454823 ovsdbapp-2.7.1/ovsdbapp/tests/functional/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.454823 ovsdbapp-2.7.1/ovsdbapp/tests/functional/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.454823 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.454823 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/hardware_vtep/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/hardware_vtep/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15722 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.454823 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6227 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.454823 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_ic_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_ic_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.458824 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   117082 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.458824 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_southbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_southbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_southbound/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7393 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.458824 ovsdbapp-2.7.1/ovsdbapp/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.458824 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.458824 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12330 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2715 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/test_ovs_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.462825 ovsdbapp-2.7.1/ovsdbapp/tests/unit/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/schema/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.462825 ovsdbapp-2.7.1/ovsdbapp/tests/unit/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3026 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/test_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11749 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/ovsdbapp/venv.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.442820 ovsdbapp-2.7.1/ovsdbapp.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/ovsdbapp.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6023 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/ovsdbapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/ovsdbapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/ovsdbapp.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/ovsdbapp.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/ovsdbapp.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-05-20 18:55:28.000000 ovsdbapp-2.7.1/ovsdbapp.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.434818 ovsdbapp-2.7.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.462825 ovsdbapp-2.7.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/configure-ovsdb-manager-a29a148b241a125e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/drop-py27-support-c426980520444bfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/drop-python-3-6-and-3-7-8ae8ccf16e422fc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/ovn-support-allow-stateless-01aed5acdcd1c0d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/ovn-support-discard-nexthop-cdb1d35aceaf4b63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/ovn-support-hw-vtep-ca8b3ee7a74df3fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/ovn-support-ic-northbound-df557a866a1f411f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/provide-address-set-api-3cb387b9e571d4ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/provide-lb-hc-api-8ff13ccaf75f1eee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/provide-lrp-gateway-chassis-api-14e2948183f60cfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/provide-lrp-get-method-a33a99a7f86b827e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/notes/provide-lrp-networks-modifying-1af13589064c12c6.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.466826 ovsdbapp-2.7.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.466826 ovsdbapp-2.7.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7768 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-05-20 18:55:28.470827 ovsdbapp-2.7.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.470827 ovsdbapp-2.7.1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1863 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1774 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/tools/debug_venv
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1735 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/tools/debug_venv.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      509 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/tools/setup-ovs.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      278 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-20 18:55:28.470827 ovsdbapp-2.7.1/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/zuul.d/ovsdbapp-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-05-20 18:55:01.000000 ovsdbapp-2.7.1/zuul.d/project.yaml
```

### Comparing `ovsdbapp-2.7.0/.pylintrc` & `ovsdbapp-2.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/AUTHORS` & `ovsdbapp-2.7.1/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -87,11 +87,12 @@
 pengyuesheng <pengyuesheng@gohighsec.com>
 qingszhao <zhao.daqing@99cloud.net>
 reedip <rbanerje@redhat.com>
 rossella <rsblendido@suse.com>
 shanyunfan33 <shanyunfan@inspur.com>
 wangzihao <wangzihao@yovole.com>
 yan.haifeng <yanheven@qq.com>
+yatinkarel <ykarel@redhat.com>
 zhangboye <zhangboye@inspur.com>
 zhangzs <zhangzhaoshan@inspur.com>
 zhouguowei <zhouguowei@inspur.com>
 zhouxinyong <zhouxinyong@inspur.com>
```

### Comparing `ovsdbapp-2.7.0/CONTRIBUTING.rst` & `ovsdbapp-2.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ChangeLog` & `ovsdbapp-2.7.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 CHANGES
 =======
 
+2.7.1
+-----
+
+* Add if\_exists to lrp\_set\_options
+
 2.7.0
 -----
 
 * Backend: always operate on (class level) ovsdb\_connection
+* Add pre-commit configuration
 * Remove executable from python files which don't really needs it
+* reno: Update master for unmaintained/zed
 * Handle IPv6 addresses for LB IP port mappings
 * Fix BFD functional test, avoid comparing status column
 * ovn-sb: remove chassis from Chassis\_Private on ChassisDelCommand
 * Update master for stable/2024.1
 * reno: Update master for unmaintained/xena
 * reno: Update master for unmaintained/wallaby
 * reno: Update master for unmaintained/victoria
```

### Comparing `ovsdbapp-2.7.0/LICENSE` & `ovsdbapp-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/PKG-INFO` & `ovsdbapp-2.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovsdbapp
-Version: 2.7.0
+Version: 2.7.1
 Summary: A library for creating OVSDB applications
 Home-page: https://pypi.org/project/ovsdbapp/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========
         ovsdbapp
```

### Comparing `ovsdbapp-2.7.0/README.rst` & `ovsdbapp-2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/TESTING.rst` & `ovsdbapp-2.7.1/TESTING.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/doc/source/conf.py` & `ovsdbapp-2.7.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/doc/source/user/overview.rst` & `ovsdbapp-2.7.1/doc/source/user/overview.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/doc/source/user/tutorial.rst` & `ovsdbapp-2.7.1/doc/source/user/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/__init__.py` & `ovsdbapp-2.7.1/ovsdbapp/__init__.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/api.py` & `ovsdbapp-2.7.1/ovsdbapp/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/__init__.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/__init__.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/command.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,22 +344,28 @@
     def run_idl(self, txn):
         self.result = self.api.lookup(self.table, self.record)
 
 
 class BaseSetOptionsCommand(BaseCommand):
     table = []
 
-    def __init__(self, api, entity, **options):
+    def __init__(self, api, entity, if_exists=False, **options):
         super().__init__(api)
         self.entity = entity
         self.options = options
+        self.if_exists = if_exists
 
     def run_idl(self, txn):
-        entity = self.api.lookup(self.table, self.entity)
-        entity.options = self.options
+        try:
+            entity = self.api.lookup(self.table, self.entity)
+            entity.options = self.options
+        except idlutils.RowNotFound:
+            if self.if_exists:
+                return
+            raise
 
 
 class BaseGetOptionsCommand(ReadOnlyCommand):
     table = []
 
     def __init__(self, api, entity, **options):
         super().__init__(api)
```

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/connection.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/event.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/fixtures.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/idlutils.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/idlutils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/linux/connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/rowview.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/rowview.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/transaction.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/transaction.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/vlog.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/vlog.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/windows/connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/utils.py` & `ovsdbapp-2.7.1/ovsdbapp/backend/ovs_idl/windows/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/constants.py` & `ovsdbapp-2.7.1/ovsdbapp/constants.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/event.py` & `ovsdbapp-2.7.1/ovsdbapp/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/exceptions.py` & `ovsdbapp-2.7.1/ovsdbapp/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/api.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/hardware_vtep/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/commands.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/hardware_vtep/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/hardware_vtep/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/api.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/commands.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/helpers.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/helpers.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/open_vswitch/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/api.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_ic_northbound/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/commands.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_ic_northbound/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/api.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_northbound/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,22 +646,25 @@
 
         :param port: The name or uuid of the port
         :type port:  string or uuid.UUID
         :returns:
         """
 
     @abc.abstractmethod
-    def lrp_set_options(self, port, **options):
+    def lrp_set_options(self, port, if_exists=False, **options):
         """Set options related to the type of 'port'
 
-        :param port:    The name or uuid of the port
-        :type port:     string or uuid.UUID
-        :param options: keys and values for the port 'options' dict
-        :type options:  key: string, value: string
-        :returns:       :class:`Command` with no result
+        :param port:      The name or uuid of the port
+        :type port:       string or uuid.UUID
+        :param options:   keys and values for the port 'options' dict
+        :param if_exists: If True, don't fail if the logical router port
+                          doesn't exist
+        :type if_exists:  boolean
+        :type options:    key: string, value: string
+        :returns:         :class:`Command` with no result
         """
 
     @abc.abstractmethod
     def lrp_get_options(self, port):
         """Get the type-specific options for 'port'
 
         :param port: The name or uuid of the port
```

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/commands.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_northbound/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_northbound/impl_idl.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,16 +208,16 @@
 
     def lrp_set_enabled(self, port, is_enabled):
         return cmd.LrpSetEnabledCommand(self, port, is_enabled)
 
     def lrp_get_enabled(self, port):
         return cmd.LrpGetEnabledCommand(self, port)
 
-    def lrp_set_options(self, port, **options):
-        return cmd.LrpSetOptionsCommand(self, port, **options)
+    def lrp_set_options(self, port, if_exists=False, **options):
+        return cmd.LrpSetOptionsCommand(self, port, if_exists, **options)
 
     def lrp_get_options(self, port):
         return cmd.LrpGetOptionsCommand(self, port)
 
     def lrp_set_gateway_chassis(self, port, gateway_chassis, priority=0):
         return cmd.LrpSetGatewayChassisCommand(self,
                                                port, gateway_chassis, priority)
```

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/api.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_southbound/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/commands.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_southbound/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/schema/ovn_southbound/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/base.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/base.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/base.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/fixtures.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1638,14 +1638,25 @@
         options = {'one': 'two', 'three': 'four'}
         lrp = self._lrp_add(None)
         self.api.lrp_set_options(lrp.uuid, **options).execute(
             check_error=True)
         self.assertEqual(options, self.api.lrp_get_options(lrp.uuid).execute(
             check_error=True))
 
+    def test_lrp_set_options_if_exists(self):
+        options = {'one': 'two', 'three': 'four'}
+        self.api.lrp_set_options(utils.get_rand_device_name(),
+                                 if_exists=True,
+                                 **options).execute(check_error=True)
+
+    def test_lrp_set_options_no_exist(self):
+        options = {'one': 'two', 'three': 'four'}
+        cmd = self.api.lrp_set_options(utils.get_rand_device_name(), **options)
+        self.assertRaises(idlutils.RowNotFound, cmd.execute, check_error=True)
+
     def test_lrp_get_set_gateway_chassis(self):
         lrp = self._lrp_add(None)
         c1_name = utils.get_rand_device_name()
         self.api.lrp_set_gateway_chassis(lrp.uuid, c1_name).execute(
             check_error=True)
         c1 = self.api.lookup('Gateway_Chassis', "%s_%s" % (lrp.name, c1_name))
         lrp_gwcs = self.api.lrp_get_gateway_chassis(lrp.uuid).execute(
```

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_southbound/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/backend/test_ovs_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_api.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_event.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/test_event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_utils.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/tests/utils.py` & `ovsdbapp-2.7.1/ovsdbapp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/utils.py` & `ovsdbapp-2.7.1/ovsdbapp/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp/venv.py` & `ovsdbapp-2.7.1/ovsdbapp/venv.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/ovsdbapp.egg-info/PKG-INFO` & `ovsdbapp-2.7.1/ovsdbapp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovsdbapp
-Version: 2.7.0
+Version: 2.7.1
 Summary: A library for creating OVSDB applications
 Home-page: https://pypi.org/project/ovsdbapp/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========
         ovsdbapp
```

### Comparing `ovsdbapp-2.7.0/ovsdbapp.egg-info/SOURCES.txt` & `ovsdbapp-2.7.1/ovsdbapp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.pre-commit-config.yaml
 .pylintrc
 .stestr.conf
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 HACKING.rst
 LICENSE
```

### Comparing `ovsdbapp-2.7.0/releasenotes/source/conf.py` & `ovsdbapp-2.7.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/setup.cfg` & `ovsdbapp-2.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/setup.py` & `ovsdbapp-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/tools/coding-checks.sh` & `ovsdbapp-2.7.1/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/tools/debug_venv` & `ovsdbapp-2.7.1/tools/debug_venv`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/tools/debug_venv.py` & `ovsdbapp-2.7.1/tools/debug_venv.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.7.0/tox.ini` & `ovsdbapp-2.7.1/tox.ini`

 * *Files identical despite different names*

