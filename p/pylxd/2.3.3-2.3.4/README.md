# Comparing `tmp/pylxd-2.3.3.tar.gz` & `tmp/pylxd-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylxd-2.3.3.tar", last modified: Mon Apr 29 15:37:33 2024, max compression
+gzip compressed data, was "pylxd-2.3.4.tar", last modified: Thu May 30 14:56:27 2024, max compression
```

## Comparing `pylxd-2.3.3.tar` & `pylxd-2.3.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.527112 pylxd-2.3.3/
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1422 2023-05-05 08:25:21.000000 pylxd-2.3.3/CONTRIBUTORS.rst
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    10142 2021-09-29 19:03:03.000000 pylxd-2.3.3/LICENSE
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)       60 2021-09-29 19:03:03.000000 pylxd-2.3.3/MANIFEST.in
--rw-r--r--   0 sdeziel   (1000) sdeziel   (1000)     2940 2024-04-29 15:37:33.527112 pylxd-2.3.3/PKG-INFO
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1525 2023-10-18 17:36:47.000000 pylxd-2.3.3/README.rst
-drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.511112 pylxd-2.3.3/integration/
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.3/integration/__init__.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5370 2023-06-01 18:56:49.000000 pylxd-2.3.3/integration/busybox.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1469 2023-07-13 13:52:25.000000 pylxd-2.3.3/integration/test_client.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1492 2023-06-01 18:56:49.000000 pylxd-2.3.3/integration/test_cluster_members.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     9853 2024-02-27 18:44:48.000000 pylxd-2.3.3/integration/test_containers.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2994 2023-07-13 12:08:43.000000 pylxd-2.3.3/integration/test_images.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3981 2023-06-01 18:56:49.000000 pylxd-2.3.3/integration/test_networks.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2842 2024-01-11 18:53:51.000000 pylxd-2.3.3/integration/test_profiles.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3379 2022-04-08 22:48:50.000000 pylxd-2.3.3/integration/test_projects.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     6082 2023-07-13 16:12:42.000000 pylxd-2.3.3/integration/test_storage.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5769 2023-06-01 18:56:49.000000 pylxd-2.3.3/integration/testing.py
-drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.511112 pylxd-2.3.3/migration/
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.3/migration/__init__.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5370 2023-06-01 18:56:49.000000 pylxd-2.3.3/migration/busybox.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2839 2023-06-01 18:56:49.000000 pylxd-2.3.3/migration/test_containers.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5329 2023-06-01 18:56:49.000000 pylxd-2.3.3/migration/testing.py
-drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.515112 pylxd-2.3.3/pylxd/
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      696 2023-09-25 15:31:32.000000 pylxd-2.3.3/pylxd/__init__.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    19090 2023-08-08 15:38:43.000000 pylxd-2.3.3/pylxd/client.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2135 2024-04-22 20:24:10.000000 pylxd-2.3.3/pylxd/exceptions.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2456 2023-05-05 08:25:21.000000 pylxd-2.3.3/pylxd/managers.py
-drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.519112 pylxd-2.3.3/pylxd/models/
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      911 2022-10-31 15:18:30.000000 pylxd-2.3.3/pylxd/models/__init__.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    12772 2024-01-17 21:29:41.000000 pylxd-2.3.3/pylxd/models/_model.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3653 2022-06-06 22:07:26.000000 pylxd-2.3.3/pylxd/models/certificate.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     4058 2022-10-24 16:03:37.000000 pylxd-2.3.3/pylxd/models/cluster.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      802 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/container.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     8971 2024-04-26 16:18:04.000000 pylxd-2.3.3/pylxd/models/image.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    34058 2023-08-09 14:03:27.000000 pylxd-2.3.3/pylxd/models/instance.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     6223 2023-06-01 18:56:49.000000 pylxd-2.3.3/pylxd/models/network.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3431 2024-01-17 21:29:41.000000 pylxd-2.3.3/pylxd/models/operation.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2381 2024-01-11 18:53:51.000000 pylxd-2.3.3/pylxd/models/profile.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2367 2022-09-26 21:41:17.000000 pylxd-2.3.3/pylxd/models/project.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    23890 2023-10-18 17:36:47.000000 pylxd-2.3.3/pylxd/models/storage_pool.py
-drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.523112 pylxd-2.3.3/pylxd/models/tests/
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/__init__.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5113 2022-06-06 22:07:26.000000 pylxd-2.3.3/pylxd/models/tests/test_certificate.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1858 2022-10-24 16:03:37.000000 pylxd-2.3.3/pylxd/models/tests/test_cluster.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1376 2022-10-20 21:45:44.000000 pylxd-2.3.3/pylxd/models/tests/test_cluster_certificate.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1204 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_cluster_member.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    13387 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_image.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    30217 2023-05-05 08:25:21.000000 pylxd-2.3.3/pylxd/models/tests/test_instance.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    11372 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_model.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    14808 2023-01-11 16:17:27.000000 pylxd-2.3.3/pylxd/models/tests/test_network.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5198 2024-04-22 20:24:10.000000 pylxd-2.3.3/pylxd/models/tests/test_operation.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5198 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_profile.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     4864 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_project.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    11204 2022-10-20 15:23:34.000000 pylxd-2.3.3/pylxd/models/tests/test_storage.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      792 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/virtual_machine.py
-drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.523112 pylxd-2.3.3/pylxd/tests/
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/tests/__init__.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    36958 2022-10-31 15:18:30.000000 pylxd-2.3.3/pylxd/tests/mock_lxd.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    24040 2023-05-05 08:25:21.000000 pylxd-2.3.3/pylxd/tests/test_client.py
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1326 2022-10-20 15:23:34.000000 pylxd-2.3.3/pylxd/tests/testing.py
-drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.523112 pylxd-2.3.3/pylxd.egg-info/
--rw-r--r--   0 sdeziel   (1000) sdeziel   (1000)     2940 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/PKG-INFO
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1584 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/SOURCES.txt
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        1 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/dependency_links.txt
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      323 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/requires.txt
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)       28 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/top_level.txt
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2406 2024-04-29 15:37:33.527112 pylxd-2.3.3/setup.cfg
--rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      584 2023-10-17 18:41:38.000000 pylxd-2.3.3/setup.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-05-30 14:56:27.854832 pylxd-2.3.4/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1422 2023-05-05 08:25:21.000000 pylxd-2.3.4/CONTRIBUTORS.rst
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    10142 2021-09-29 19:03:03.000000 pylxd-2.3.4/LICENSE
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)       60 2021-09-29 19:03:03.000000 pylxd-2.3.4/MANIFEST.in
+-rw-r--r--   0 sdeziel   (1000) sdeziel   (1000)     2948 2024-05-30 14:56:27.850832 pylxd-2.3.4/PKG-INFO
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1525 2023-10-18 17:36:47.000000 pylxd-2.3.4/README.rst
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-05-30 14:56:27.838832 pylxd-2.3.4/integration/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.4/integration/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5370 2023-06-01 18:56:49.000000 pylxd-2.3.4/integration/busybox.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1469 2023-07-13 13:52:25.000000 pylxd-2.3.4/integration/test_client.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1492 2023-06-01 18:56:49.000000 pylxd-2.3.4/integration/test_cluster_members.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     9853 2024-02-27 18:44:48.000000 pylxd-2.3.4/integration/test_containers.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2994 2023-07-13 12:08:43.000000 pylxd-2.3.4/integration/test_images.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3981 2023-06-01 18:56:49.000000 pylxd-2.3.4/integration/test_networks.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2842 2024-01-11 18:53:51.000000 pylxd-2.3.4/integration/test_profiles.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3379 2022-04-08 22:48:50.000000 pylxd-2.3.4/integration/test_projects.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     6082 2023-07-13 16:12:42.000000 pylxd-2.3.4/integration/test_storage.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5769 2023-06-01 18:56:49.000000 pylxd-2.3.4/integration/testing.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-05-30 14:56:27.838832 pylxd-2.3.4/migration/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.4/migration/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5370 2023-06-01 18:56:49.000000 pylxd-2.3.4/migration/busybox.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2839 2023-06-01 18:56:49.000000 pylxd-2.3.4/migration/test_containers.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5329 2023-06-01 18:56:49.000000 pylxd-2.3.4/migration/testing.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-05-30 14:56:27.838832 pylxd-2.3.4/pylxd/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      696 2023-09-25 15:31:32.000000 pylxd-2.3.4/pylxd/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    19090 2023-08-08 15:38:43.000000 pylxd-2.3.4/pylxd/client.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2135 2024-04-22 20:24:10.000000 pylxd-2.3.4/pylxd/exceptions.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2456 2023-05-05 08:25:21.000000 pylxd-2.3.4/pylxd/managers.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-05-30 14:56:27.846832 pylxd-2.3.4/pylxd/models/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      911 2022-10-31 15:18:30.000000 pylxd-2.3.4/pylxd/models/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    12772 2024-01-17 21:29:41.000000 pylxd-2.3.4/pylxd/models/_model.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3653 2022-06-06 22:07:26.000000 pylxd-2.3.4/pylxd/models/certificate.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     4058 2022-10-24 16:03:37.000000 pylxd-2.3.4/pylxd/models/cluster.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      802 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/models/container.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     8971 2024-04-26 16:18:04.000000 pylxd-2.3.4/pylxd/models/image.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    34058 2023-08-09 14:03:27.000000 pylxd-2.3.4/pylxd/models/instance.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     6223 2023-06-01 18:56:49.000000 pylxd-2.3.4/pylxd/models/network.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3431 2024-01-17 21:29:41.000000 pylxd-2.3.4/pylxd/models/operation.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2381 2024-01-11 18:53:51.000000 pylxd-2.3.4/pylxd/models/profile.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2367 2022-09-26 21:41:17.000000 pylxd-2.3.4/pylxd/models/project.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    23890 2023-10-18 17:36:47.000000 pylxd-2.3.4/pylxd/models/storage_pool.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-05-30 14:56:27.846832 pylxd-2.3.4/pylxd/models/tests/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/models/tests/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5113 2022-06-06 22:07:26.000000 pylxd-2.3.4/pylxd/models/tests/test_certificate.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1858 2022-10-24 16:03:37.000000 pylxd-2.3.4/pylxd/models/tests/test_cluster.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1376 2022-10-20 21:45:44.000000 pylxd-2.3.4/pylxd/models/tests/test_cluster_certificate.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1204 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/models/tests/test_cluster_member.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    13387 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/models/tests/test_image.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    30217 2023-05-05 08:25:21.000000 pylxd-2.3.4/pylxd/models/tests/test_instance.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    11372 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/models/tests/test_model.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    14808 2023-01-11 16:17:27.000000 pylxd-2.3.4/pylxd/models/tests/test_network.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5198 2024-04-22 20:24:10.000000 pylxd-2.3.4/pylxd/models/tests/test_operation.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5198 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/models/tests/test_profile.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     4864 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/models/tests/test_project.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    11204 2022-10-20 15:23:34.000000 pylxd-2.3.4/pylxd/models/tests/test_storage.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      792 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/models/virtual_machine.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-05-30 14:56:27.850832 pylxd-2.3.4/pylxd/tests/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.4/pylxd/tests/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    36958 2022-10-31 15:18:30.000000 pylxd-2.3.4/pylxd/tests/mock_lxd.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    24040 2023-05-05 08:25:21.000000 pylxd-2.3.4/pylxd/tests/test_client.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1326 2022-10-20 15:23:34.000000 pylxd-2.3.4/pylxd/tests/testing.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-05-30 14:56:27.850832 pylxd-2.3.4/pylxd.egg-info/
+-rw-r--r--   0 sdeziel   (1000) sdeziel   (1000)     2948 2024-05-30 14:56:27.000000 pylxd-2.3.4/pylxd.egg-info/PKG-INFO
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1584 2024-05-30 14:56:27.000000 pylxd-2.3.4/pylxd.egg-info/SOURCES.txt
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        1 2024-05-30 14:56:27.000000 pylxd-2.3.4/pylxd.egg-info/dependency_links.txt
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      331 2024-05-30 14:56:27.000000 pylxd-2.3.4/pylxd.egg-info/requires.txt
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)       28 2024-05-30 14:56:27.000000 pylxd-2.3.4/pylxd.egg-info/top_level.txt
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2416 2024-05-30 14:56:27.854832 pylxd-2.3.4/setup.cfg
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      584 2023-10-17 18:41:38.000000 pylxd-2.3.4/setup.py
```

### Comparing `pylxd-2.3.3/CONTRIBUTORS.rst` & `pylxd-2.3.4/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/LICENSE` & `pylxd-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/PKG-INFO` & `pylxd-2.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pylxd
-Version: 2.3.3
+Version: 2.3.4
 Summary: python library for LXD
 Home-page: https://ubuntu.com/lxd
 Author: Paul Hummer and others (see CONTRIBUTORS.rst)
 Author-email: lxd@lists.canonical.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: cryptography>=3.2
 Requires-Dist: python-dateutil>=2.4.2
-Requires-Dist: requests>=2.20.0
+Requires-Dist: requests<2.32.0,>=2.20.0
 Requires-Dist: requests-toolbelt>=0.8.0
 Requires-Dist: requests-unixsocket>=0.1.5
 Requires-Dist: urllib3<2
 Requires-Dist: ws4py!=0.3.5,>=0.3.4
 Provides-Extra: testing
 Requires-Dist: ddt>=0.7.0; extra == "testing"
 Requires-Dist: mock-services>=0.3; extra == "testing"
```

### Comparing `pylxd-2.3.3/README.rst` & `pylxd-2.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/busybox.py` & `pylxd-2.3.4/integration/busybox.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/test_client.py` & `pylxd-2.3.4/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/test_cluster_members.py` & `pylxd-2.3.4/integration/test_cluster_members.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/test_containers.py` & `pylxd-2.3.4/integration/test_containers.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/test_images.py` & `pylxd-2.3.4/integration/test_images.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/test_networks.py` & `pylxd-2.3.4/integration/test_networks.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/test_profiles.py` & `pylxd-2.3.4/integration/test_profiles.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/test_projects.py` & `pylxd-2.3.4/integration/test_projects.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/test_storage.py` & `pylxd-2.3.4/integration/test_storage.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/integration/testing.py` & `pylxd-2.3.4/integration/testing.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/migration/busybox.py` & `pylxd-2.3.4/migration/busybox.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/migration/test_containers.py` & `pylxd-2.3.4/migration/test_containers.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/migration/testing.py` & `pylxd-2.3.4/migration/testing.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/__init__.py` & `pylxd-2.3.4/pylxd/__init__.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/client.py` & `pylxd-2.3.4/pylxd/client.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/exceptions.py` & `pylxd-2.3.4/pylxd/exceptions.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/managers.py` & `pylxd-2.3.4/pylxd/managers.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/__init__.py` & `pylxd-2.3.4/pylxd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/_model.py` & `pylxd-2.3.4/pylxd/models/_model.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/certificate.py` & `pylxd-2.3.4/pylxd/models/certificate.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/cluster.py` & `pylxd-2.3.4/pylxd/models/cluster.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/container.py` & `pylxd-2.3.4/pylxd/models/container.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/image.py` & `pylxd-2.3.4/pylxd/models/image.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/instance.py` & `pylxd-2.3.4/pylxd/models/instance.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/network.py` & `pylxd-2.3.4/pylxd/models/network.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/operation.py` & `pylxd-2.3.4/pylxd/models/operation.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/profile.py` & `pylxd-2.3.4/pylxd/models/profile.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/project.py` & `pylxd-2.3.4/pylxd/models/project.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/storage_pool.py` & `pylxd-2.3.4/pylxd/models/storage_pool.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_certificate.py` & `pylxd-2.3.4/pylxd/models/tests/test_certificate.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_cluster.py` & `pylxd-2.3.4/pylxd/models/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_cluster_certificate.py` & `pylxd-2.3.4/pylxd/models/tests/test_cluster_certificate.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_cluster_member.py` & `pylxd-2.3.4/pylxd/models/tests/test_cluster_member.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_image.py` & `pylxd-2.3.4/pylxd/models/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_instance.py` & `pylxd-2.3.4/pylxd/models/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_model.py` & `pylxd-2.3.4/pylxd/models/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_network.py` & `pylxd-2.3.4/pylxd/models/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_operation.py` & `pylxd-2.3.4/pylxd/models/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_profile.py` & `pylxd-2.3.4/pylxd/models/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_project.py` & `pylxd-2.3.4/pylxd/models/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/tests/test_storage.py` & `pylxd-2.3.4/pylxd/models/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/models/virtual_machine.py` & `pylxd-2.3.4/pylxd/models/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/tests/mock_lxd.py` & `pylxd-2.3.4/pylxd/tests/mock_lxd.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/tests/test_client.py` & `pylxd-2.3.4/pylxd/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd/tests/testing.py` & `pylxd-2.3.4/pylxd/tests/testing.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/pylxd.egg-info/PKG-INFO` & `pylxd-2.3.4/pylxd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pylxd
-Version: 2.3.3
+Version: 2.3.4
 Summary: python library for LXD
 Home-page: https://ubuntu.com/lxd
 Author: Paul Hummer and others (see CONTRIBUTORS.rst)
 Author-email: lxd@lists.canonical.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: cryptography>=3.2
 Requires-Dist: python-dateutil>=2.4.2
-Requires-Dist: requests>=2.20.0
+Requires-Dist: requests<2.32.0,>=2.20.0
 Requires-Dist: requests-toolbelt>=0.8.0
 Requires-Dist: requests-unixsocket>=0.1.5
 Requires-Dist: urllib3<2
 Requires-Dist: ws4py!=0.3.5,>=0.3.4
 Provides-Extra: testing
 Requires-Dist: ddt>=0.7.0; extra == "testing"
 Requires-Dist: mock-services>=0.3; extra == "testing"
```

### Comparing `pylxd-2.3.3/pylxd.egg-info/SOURCES.txt` & `pylxd-2.3.4/pylxd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.3/setup.cfg` & `pylxd-2.3.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylxd
-version = 2.3.3
+version = 2.3.4
 description = python library for LXD
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Paul Hummer and others (see CONTRIBUTORS.rst)
 author_email = lxd@lists.canonical.com
 home_page = https://ubuntu.com/lxd
 classifier = 
@@ -16,15 +16,15 @@
 
 [options]
 python_requires = >= 3.8
 packages = find:
 install_requires = 
 	cryptography >= 3.2
 	python-dateutil >= 2.4.2
-	requests >= 2.20.0
+	requests >= 2.20.0, < 2.32.0
 	requests-toolbelt >= 0.8.0
 	requests-unixsocket >= 0.1.5
 	urllib3 < 2
 	ws4py != 0.3.5, >= 0.3.4  # 0.3.5 is broken for websocket support
 
 [options.extras_require]
 testing =
```

### Comparing `pylxd-2.3.3/setup.py` & `pylxd-2.3.4/setup.py`

 * *Files identical despite different names*

