# Comparing `tmp/nautobot_device_onboarding-3.0.1.tar.gz` & `tmp/nautobot_device_onboarding-4.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_device_onboarding-3.0.1.tar", max compression
+gzip compressed data, was "nautobot_device_onboarding-4.0.0b1.tar", max compression
```

## Comparing `nautobot_device_onboarding-3.0.1.tar` & `nautobot_device_onboarding-4.0.0b1.tar`

### file list

```diff
@@ -1,37 +1,171 @@
--rw-r--r--   0        0        0      591 2023-11-24 19:29:27.906775 nautobot_device_onboarding-3.0.1/LICENSE
--rw-r--r--   0        0        0     4191 2023-11-24 19:29:27.906775 nautobot_device_onboarding-3.0.1/README.md
--rw-r--r--   0        0        0     1772 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/__init__.py
--rw-r--r--   0        0        0      244 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/constants.py
--rw-r--r--   0        0        0      115 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/exceptions.py
--rw-r--r--   0        0        0     1419 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/helpers.py
--rw-r--r--   0        0        0     8119 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/jobs.py
--rw-r--r--   0        0        0     2947 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0001_initial.py
--rw-r--r--   0        0        0     3961 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0001_squash__0001_0004_0005_0006.py
--rw-r--r--   0        0        0      595 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0002_create_onboardingdevice.py
--rw-r--r--   0        0        0      780 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0003_onboardingtask_label.py
--rw-r--r--   0        0        0      571 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_1.py
--rw-r--r--   0        0        0      739 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_2.py
--rw-r--r--   0        0        0     1407 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_3.py
--rw-r--r--   0        0        0      564 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_1.py
--rw-r--r--   0        0        0      769 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_2.py
--rw-r--r--   0        0        0     1252 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_3.py
--rw-r--r--   0        0        0      576 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_1.py
--rw-r--r--   0        0        0      451 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_2.py
--rw-r--r--   0        0        0      639 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_3.py
--rw-r--r--   0        0        0      474 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0007_alter_onboardingtask_ip_address.py
--rw-r--r--   0        0        0      774 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0008_alter_onboardingtask_options.py
--rw-r--r--   0        0        0      986 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0009_remove_models.py
--rw-r--r--   0        0        0        0 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/__init__.py
--rw-r--r--   0        0        0    21661 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/nautobot_keeper.py
--rw-r--r--   0        0        0    11648 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/netdev_keeper.py
--rw-r--r--   0        0        0       18 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/onboarding/__init__.py
--rw-r--r--   0        0        0      771 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/onboarding/onboarding.py
--rw-r--r--   0        0        0       29 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/onboarding_extensions/__init__.py
--rw-r--r--   0        0        0      916 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/onboarding_extensions/ios.py
--rw-r--r--   0        0        0       56 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/tests/__init__.py
--rw-r--r--   0        0        0     1578 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/tests/test_basic.py
--rw-r--r--   0        0        0    23425 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/tests/test_nautobot_keeper.py
--rw-r--r--   0        0        0     5098 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/tests/test_onboarding.py
--rw-r--r--   0        0        0     1201 2023-11-24 19:29:27.910775 nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/utils/credentials.py
--rw-r--r--   0        0        0     3419 2023-11-24 19:29:35.214887 nautobot_device_onboarding-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 nautobot_device_onboarding-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-05-29 22:46:34.813099 nautobot_device_onboarding-4.0.0b1/LICENSE
+-rw-r--r--   0        0        0     4184 2024-05-29 22:46:34.813099 nautobot_device_onboarding-4.0.0b1/README.md
+-rw-r--r--   0        0        0     1863 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/__init__.py
+-rwxr-xr-x   0        0        0      180 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/choices.py
+-rwxr-xr-x   0        0        0     4386 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/command_mappers/arista_eos.yml
+-rwxr-xr-x   0        0        0     4247 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/command_mappers/cisco_ios.yml
+-rwxr-xr-x   0        0        0     4693 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/command_mappers/cisco_nxos.yml
+-rwxr-xr-x   0        0        0      755 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/command_mappers/cisco_wlc.yml
+-rwxr-xr-x   0        0        0     4325 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/command_mappers/cisco_xe.yml
+-rwxr-xr-x   0        0        0     6637 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/command_mappers/juniper_junos.yml
+-rw-r--r--   0        0        0     1505 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/constants.py
+-rwxr-xr-x   0        0        0      804 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/datasources.py
+-rw-r--r--   0        0        0       57 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/diffsync/__init__.py
+-rw-r--r--   0        0        0       87 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/diffsync/adapters/__init__.py
+-rw-r--r--   0        0        0    18488 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/diffsync/adapters/sync_devices_adapters.py
+-rw-r--r--   0        0        0    31301 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/diffsync/adapters/sync_network_data_adapters.py
+-rw-r--r--   0        0        0    16910 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/diffsync/models/sync_devices_models.py
+-rw-r--r--   0        0        0    22408 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/diffsync/models/sync_network_data_models.py
+-rw-r--r--   0        0        0      115 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/exceptions.py
+-rwxr-xr-x   0        0        0     3507 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/jinja_filters.py
+-rwxr-xr-x   0        0        0    33496 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/jobs.py
+-rw-r--r--   0        0        0     2948 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3961 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0001_squash__0001_0004_0005_0006.py
+-rw-r--r--   0        0        0      595 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0002_create_onboardingdevice.py
+-rw-r--r--   0        0        0      780 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0003_onboardingtask_label.py
+-rw-r--r--   0        0        0      570 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_1.py
+-rw-r--r--   0        0        0      739 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_2.py
+-rw-r--r--   0        0        0     1407 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_3.py
+-rw-r--r--   0        0        0      564 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_1.py
+-rw-r--r--   0        0        0      769 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_2.py
+-rw-r--r--   0        0        0     1252 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_3.py
+-rw-r--r--   0        0        0      576 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_1.py
+-rw-r--r--   0        0        0      451 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_2.py
+-rw-r--r--   0        0        0      639 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_3.py
+-rw-r--r--   0        0        0      474 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0007_alter_onboardingtask_ip_address.py
+-rw-r--r--   0        0        0      774 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0008_alter_onboardingtask_options.py
+-rw-r--r--   0        0        0      986 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0009_remove_models.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/__init__.py
+-rw-r--r--   0        0        0    22401 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nautobot_keeper.py
+-rw-r--r--   0        0        0    11609 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/netdev_keeper.py
+-rwxr-xr-x   0        0        0    14662 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nornir_plays/command_getter.py
+-rwxr-xr-x   0        0        0      798 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nornir_plays/empty_inventory.py
+-rwxr-xr-x   0        0        0    10623 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nornir_plays/formatter.py
+-rwxr-xr-x   0        0        0     1830 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nornir_plays/inventory_creator.py
+-rwxr-xr-x   0        0        0     1748 2024-05-29 22:46:34.817099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nornir_plays/logger.py
+-rwxr-xr-x   0        0        0     5389 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nornir_plays/processor.py
+-rwxr-xr-x   0        0        0     8783 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nornir_plays/schemas.py
+-rwxr-xr-x   0        0        0     1617 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nornir_plays/transform.py
+-rw-r--r--   0        0        0       18 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/onboarding/__init__.py
+-rw-r--r--   0        0        0      687 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/onboarding/onboarding.py
+-rw-r--r--   0        0        0       29 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/onboarding_extensions/__init__.py
+-rw-r--r--   0        0        0      916 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/onboarding_extensions/ios.py
+-rw-r--r--   0        0        0    33439 2024-05-29 22:47:03.681008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/404.html
+-rw-r--r--   0        0        0    35643 2024-05-29 22:47:03.701008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    51047 2024-05-29 22:47:03.709008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/install.html
+-rw-r--r--   0        0        0    35241 2024-05-29 22:47:03.717008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    37635 2024-05-29 22:47:03.717008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    45897 2024-05-29 22:47:03.721008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/release_notes/version_1.1.html
+-rw-r--r--   0        0        0    38461 2024-05-29 22:47:03.725008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/release_notes/version_1.2.html
+-rw-r--r--   0        0        0    39346 2024-05-29 22:47:03.729008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/release_notes/version_2.0.html
+-rw-r--r--   0        0        0    41089 2024-05-29 22:47:03.729008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/release_notes/version_3.0.html
+-rw-r--r--   0        0        0    38091 2024-05-29 22:47:03.713008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    36661 2024-05-29 22:47:03.713008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/admin/upgrade.html
+-rw-r--r--   0        0        0     1000 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     5135 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    17074 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2024-05-29 22:47:03.565009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2024-05-29 22:47:03.569009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2024-05-29 22:47:03.569009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2024-05-29 22:47:03.569009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0     9204 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   113505 2024-05-29 22:47:03.569009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/stylesheets/main.26e3688c.min.css
+-rw-r--r--   0        0        0    38975 2024-05-29 22:47:03.569009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/stylesheets/main.26e3688c.min.css.map
+-rw-r--r--   0        0        0    12245 2024-05-29 22:47:03.569009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/stylesheets/palette.ecc896b0.min.css
+-rw-r--r--   0        0        0     3639 2024-05-29 22:47:03.569009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/assets/stylesheets/palette.ecc896b0.min.css.map
+-rw-r--r--   0        0        0    35444 2024-05-29 22:47:03.733008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/dev/arch_decision.html
+-rw-r--r--   0        0        0    35253 2024-05-29 22:47:03.765008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/dev/code_reference/index.html
+-rw-r--r--   0        0        0    46557 2024-05-29 22:47:03.773008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/dev/code_reference/package.html
+-rw-r--r--   0        0        0    41025 2024-05-29 22:47:03.737008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/dev/contributing.html
+-rw-r--r--   0        0        0    97172 2024-05-29 22:47:03.757008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    39564 2024-05-29 22:47:03.757008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/dev/extending.html
+-rw-r--r--   0        0        0    42596 2024-05-29 22:47:03.761008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/dev/onboarding_extensions.html
+-rw-r--r--   0        0        0    80113 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/images/do_job_inputs.png
+-rw-r--r--   0        0        0     2937 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/images/icon-DeviceOnboarding.png
+-rw-r--r--   0        0        0    62560 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/images/platform_cisco_ios.png
+-rw-r--r--   0        0        0    62375 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/images/platform_juniper_junos.png
+-rw-r--r--   0        0        0    42287 2024-05-29 22:47:03.697008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/index.html
+-rw-r--r--   0        0        0      253 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/objects.inv
+-rw-r--r--   0        0        0      120 2024-05-29 22:47:03.561009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/requirements.txt
+-rw-r--r--   0        0        0    98477 2024-05-29 22:47:03.805008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/search/search_index.json
+-rw-r--r--   0        0        0     5582 2024-05-29 22:47:03.573009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/sitemap.xml
+-rw-r--r--   0        0        0      473 2024-05-29 22:47:03.573009 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    43755 2024-05-29 22:47:03.777008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/user/app_detailed_design.html
+-rw-r--r--   0        0        0    40160 2024-05-29 22:47:03.777008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    46343 2024-05-29 22:47:03.781008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/user/app_overview.html
+-rw-r--r--   0        0        0    47953 2024-05-29 22:47:03.789008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0    51332 2024-05-29 22:47:03.793008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/user/app_use_cases_original.html
+-rw-r--r--   0        0        0    45677 2024-05-29 22:47:03.801008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/user/app_yaml_overrides.html
+-rw-r--r--   0        0        0    37740 2024-05-29 22:47:03.801008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/user/external_interactions.html
+-rw-r--r--   0        0        0    51701 2024-05-29 22:47:03.805008 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/static/nautobot_device_onboarding/docs/user/faq.html
+-rw-r--r--   0        0        0       53 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/__init__.py
+-rw-r--r--   0        0        0     1346 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/fixtures/sync_devices_fixture.py
+-rw-r--r--   0        0        0     6557 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/fixtures/sync_network_data_fixture.py
+-rwxr-xr-x   0        0        0    16013 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/arista_eos/command_getter_result_1.json
+-rwxr-xr-x   0        0        0      155 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/arista_eos/sync_devices_expected_result_1.json
+-rwxr-xr-x   0        0        0    17126 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_ios/command_getter_result_1.json
+-rwxr-xr-x   0        0        0      146 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_ios/sync_devices_expected_result_1.json
+-rwxr-xr-x   0        0        0   155376 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_nxos/command_getter_result_1.json
+-rwxr-xr-x   0        0        0      142 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_nxos/sync_devices_expected_result_1.json
+-rwxr-xr-x   0        0        0     1609 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_wlc/command_getter_result_1.json
+-rwxr-xr-x   0        0        0      136 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_wlc/sync_devices_expected_result_1.json
+-rwxr-xr-x   0        0        0    17126 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_xe/command_getter_result_1.json
+-rwxr-xr-x   0        0        0   127360 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_xe/command_getter_result_2.json
+-rwxr-xr-x   0        0        0   411035 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_xe/command_getter_result_3.json
+-rwxr-xr-x   0        0        0      146 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_xe/sync_devices_expected_result_1.json
+-rwxr-xr-x   0        0        0      143 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_xe/sync_devices_expected_result_2.json
+-rwxr-xr-x   0        0        0      132 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/cisco_xe/sync_devices_expected_result_3.json
+-rwxr-xr-x   0        0        0     4727 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/command_mappers/mock_cisco_ios.yml
+-rwxr-xr-x   0        0        0   244149 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/juniper_junos/command_getter_result_1.json
+-rwxr-xr-x   0        0        0      127 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/mock/juniper_junos/sync_devices_expected_result_1.json
+-rw-r--r--   0        0        0     1043 2024-05-29 22:46:34.821099 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_basic.py
+-rwxr-xr-x   0        0        0     8919 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_command_getter.py
+-rwxr-xr-x   0        0        0      667 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_empty_inventory.py
+-rwxr-xr-x   0        0        0    27702 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_formatter.py
+-rwxr-xr-x   0        0        0     2205 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_inventory_creator.py
+-rw-r--r--   0        0        0    24461 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_nautobot_keeper.py
+-rw-r--r--   0        0        0     5015 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_onboarding.py
+-rw-r--r--   0        0        0     3558 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_sync_devices_network_adapter.py
+-rwxr-xr-x   0        0        0     4778 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_transform.py
+-rw-r--r--   0        0        0     6406 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/utils.py
+-rw-r--r--   0        0        0     1201 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/utils/credentials.py
+-rw-r--r--   0        0        0     3812 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/utils/diffsync_utils.py
+-rw-r--r--   0        0        0     3397 2024-05-29 22:46:34.825100 nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/utils/helper.py
+-rwxr-xr-x   0        0        0     5854 2024-05-29 22:46:43.593070 nautobot_device_onboarding-4.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 nautobot_device_onboarding-4.0.0b1/PKG-INFO
```

### Comparing `nautobot_device_onboarding-3.0.1/LICENSE` & `nautobot_device_onboarding-4.0.0b1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Apache Software License 2.0
 
-Copyright (c) 2023, Network to Code, LLC
+Copyright (c) 2024, Network to Code, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nautobot_device_onboarding-3.0.1/README.md` & `nautobot_device_onboarding-4.0.0b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Nautobot Device Onboarding
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-onboarding/develop/docs/images/icon-DeviceOnboarding.png" class="logo" height="200px">
+  <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-device-onboarding/develop/docs/images/icon-DeviceOnboarding.png" class="logo" height="200px">
   <br>
-  <a href="https://github.com/nautobot/nautobot-plugin-device-onboarding/actions"><img src="https://github.com/nautobot/nautobot-plugin-device-onboarding/actions/workflows/ci.yml/badge.svg?branch=develop"></a>
-  <a href="https://docs.nautobot.com/projects/device-onboarding/"><img src="https://readthedocs.org/projects/nautobot-plugin-device-onboarding/badge/"></a>
+  <a href="https://github.com/nautobot/nautobot-app-device-onboarding/actions"><img src="https://github.com/nautobot/nautobot-app-device-onboarding/actions/workflows/ci.yml/badge.svg?branch=develop"></a>
+  <a href="https://docs.nautobot.com/projects/device-onboarding/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-device-onboarding/badge/"></a>
   <a href="https://pypi.org/project/nautobot-device-onboarding/"><img src="https://img.shields.io/pypi/v/nautobot-device-onboarding"></a>
   <a href="https://pypi.org/project/nautobot-device-onboarding/"><img src="https://img.shields.io/pypi/dm/nautobot-device-onboarding"></a>
   <br>
   A plugin for <a href="https://github.com/nautobot/nautobot">Nautobot</a> to easily onboard new devices.
 </p>
 
 ## Overview
 
 The `nautobot-device-onboarding` plugin is using the [netmiko](https://github.com/ktbyers/netmiko) and [NAPALM](https://napalm.readthedocs.io/en/latest/) libraries to simplify the onboarding process of a new device into Nautobot down to, in many cases, an *IP Address* and a *Location*. In some cases, the user may also have to specify a specific *Device Platform* and *Device Port*.
 
-Regardless, the Onboarding Plugin greatly simplifies the onboarding process by allowing the user to specify a small amount of info and having the app populate a much larger amount of device data in Nautobot.
+Regardless, the Onboarding App greatly simplifies the onboarding process by allowing the user to specify a small amount of info and having the app populate a much larger amount of device data in Nautobot.
 
 ### Screenshots
 
 Device Onboarding is a Job that allows you to provide a few required pieces of information and onboard the device.
 
-![job input](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-onboarding/develop/docs/images/do_job_inputs.png)
+![job input](https://raw.githubusercontent.com/nautobot/nautobot-app-device-onboarding/develop/docs/images/do_job_inputs.png)
 
 ## Try it out!
 
 This App is installed in the Nautobot Community Sandbox found over at [demo.nautobot.com](https://demo.nautobot.com/)!
 
 > For a full list of all the available always-on sandbox environments, head over to the main page on [networktocode.com](https://www.networktocode.com/nautobot/sandbox-environments/).
 
@@ -37,15 +37,15 @@
 - [Administrator Guide](https://docs.nautobot.com/projects/device-onboarding/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the App.
 - [Developer Guide](https://docs.nautobot.com/projects/device-onboarding/en/latest/dev/contributing/) - Extending the App, Code Reference, Contribution Guide.
 - [Release Notes / Changelog](https://docs.nautobot.com/projects/device-onboarding/en/latest/admin/release_notes/).
 - [Frequently Asked Questions](https://docs.nautobot.com/projects/device-onboarding/en/latest/user/faq/).
 
 ### Contributing to the Docs
 
-You can find all the Markdown source for the App documentation under the [docs](https://github.com/nautobot/nautobot-plugin-device-onboarding/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient - clone the repository and edit away.
+You can find all the Markdown source for the App documentation under the [`docs`](https://github.com/nautobot/nautobot-app-device-onboarding/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient: clone the repository and edit away.
 
 If you need to view the fully generated documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be started using the invoke commands (details in the [Development Environment Guide](https://docs.nautobot.com/projects/device-onboarding/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). As your changes are saved, the live docs will be automatically reloaded.
 
 Any PRs with fixes or improvements are very welcome!
 
 ## Questions
```

#### html2text {}

```diff
@@ -1,52 +1,50 @@
 # Nautobot Device Onboarding
-[https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-onboarding/
+  [https://raw.githubusercontent.com/nautobot/nautobot-app-device-onboarding/
                 develop/docs/images/icon-DeviceOnboarding.png]
-    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_/_a_c_t_i_o_n_s_/
- _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_e_l_o_p_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/
-   _n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
-  _n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-
-                                  _o_n_b_o_a_r_d_i_n_g_]
+_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/
+  _c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_e_l_o_p_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-
+_p_l_u_g_i_n_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-
+    _o_n_b_o_a_r_d_i_n_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_]
              A plugin for _N_a_u_t_o_b_o_t to easily onboard new devices.
 ## Overview The `nautobot-device-onboarding` plugin is using the [netmiko]
 (https://github.com/ktbyers/netmiko) and [NAPALM](https://
 napalm.readthedocs.io/en/latest/) libraries to simplify the onboarding process
 of a new device into Nautobot down to, in many cases, an *IP Address* and a
 *Location*. In some cases, the user may also have to specify a specific *Device
-Platform* and *Device Port*. Regardless, the Onboarding Plugin greatly
-simplifies the onboarding process by allowing the user to specify a small
-amount of info and having the app populate a much larger amount of device data
-in Nautobot. ### Screenshots Device Onboarding is a Job that allows you to
-provide a few required pieces of information and onboard the device. ![job
-input](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-
-onboarding/develop/docs/images/do_job_inputs.png) ## Try it out! This App is
-installed in the Nautobot Community Sandbox found over at [demo.nautobot.com]
-(https://demo.nautobot.com/)! > For a full list of all the available always-on
-sandbox environments, head over to the main page on [networktocode.com](https:/
-/www.networktocode.com/nautobot/sandbox-environments/). ## Documentation Full
-web-based HTML documentation for this app can be found over on the [Nautobot
-Docs](https://docs.nautobot.com/) website: - [User Guide](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/user/app_overview/) -
-Overview, Using the App, Getting Started. - [Administrator Guide](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/admin/install/) - How to
-Install, Configure, Upgrade, or Uninstall the App. - [Developer Guide](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/dev/contributing/) -
-Extending the App, Code Reference, Contribution Guide. - [Release Notes /
-Changelog](https://docs.nautobot.com/projects/device-onboarding/en/latest/
-admin/release_notes/). - [Frequently Asked Questions](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/user/faq/). ###
-Contributing to the Docs You can find all the Markdown source for the App
-documentation under the [docs](https://github.com/nautobot/nautobot-plugin-
-device-onboarding/tree/develop/docs) folder in this repository. For simple
-edits, a Markdown capable editor is sufficient - clone the repository and edit
-away. If you need to view the fully generated documentation site, you can build
-it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be
-started using the invoke commands (details in the [Development Environment
-Guide](https://docs.nautobot.com/projects/device-onboarding/en/latest/dev/
-dev_environment/#docker-development-environment)) on [http://localhost:8001]
-(http://localhost:8001). As your changes are saved, the live docs will be
-automatically reloaded. Any PRs with fixes or improvements are very welcome! ##
-Questions For any questions or comments, please check the [FAQ](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/user/faq/) first. Feel
-free to also swing by the [Network to Code Slack](https://
-networktocode.slack.com/) (channel `#nautobot`), sign up [here](http://
-slack.networktocode.com/) if you don't have an account.
+Platform* and *Device Port*. Regardless, the Onboarding App greatly simplifies
+the onboarding process by allowing the user to specify a small amount of info
+and having the app populate a much larger amount of device data in Nautobot.
+### Screenshots Device Onboarding is a Job that allows you to provide a few
+required pieces of information and onboard the device. ![job input](https://
+raw.githubusercontent.com/nautobot/nautobot-app-device-onboarding/develop/docs/
+images/do_job_inputs.png) ## Try it out! This App is installed in the Nautobot
+Community Sandbox found over at [demo.nautobot.com](https://demo.nautobot.com/
+)! > For a full list of all the available always-on sandbox environments, head
+over to the main page on [networktocode.com](https://www.networktocode.com/
+nautobot/sandbox-environments/). ## Documentation Full web-based HTML
+documentation for this app can be found over on the [Nautobot Docs](https://
+docs.nautobot.com/) website: - [User Guide](https://docs.nautobot.com/projects/
+device-onboarding/en/latest/user/app_overview/) - Overview, Using the App,
+Getting Started. - [Administrator Guide](https://docs.nautobot.com/projects/
+device-onboarding/en/latest/admin/install/) - How to Install, Configure,
+Upgrade, or Uninstall the App. - [Developer Guide](https://docs.nautobot.com/
+projects/device-onboarding/en/latest/dev/contributing/) - Extending the App,
+Code Reference, Contribution Guide. - [Release Notes / Changelog](https://
+docs.nautobot.com/projects/device-onboarding/en/latest/admin/release_notes/). -
+[Frequently Asked Questions](https://docs.nautobot.com/projects/device-
+onboarding/en/latest/user/faq/). ### Contributing to the Docs You can find all
+the Markdown source for the App documentation under the [`docs`](https://
+github.com/nautobot/nautobot-app-device-onboarding/tree/develop/docs) folder in
+this repository. For simple edits, a Markdown capable editor is sufficient:
+clone the repository and edit away. If you need to view the fully generated
+documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A
+container hosting the docs will be started using the invoke commands (details
+in the [Development Environment Guide](https://docs.nautobot.com/projects/
+device-onboarding/en/latest/dev/dev_environment/#docker-development-
+environment)) on [http://localhost:8001](http://localhost:8001). As your
+changes are saved, the live docs will be automatically reloaded. Any PRs with
+fixes or improvements are very welcome! ## Questions For any questions or
+comments, please check the [FAQ](https://docs.nautobot.com/projects/device-
+onboarding/en/latest/user/faq/) first. Feel free to also swing by the [Network
+to Code Slack](https://networktocode.slack.com/) (channel `#nautobot`), sign up
+[here](http://slack.networktocode.com/) if you don't have an account.
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/__init__.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-"""Plugin declaration for nautobot_device_onboarding."""
-# Metadata is inherited from Nautobot. If not including Nautobot in the environment, this should be added
+"""App declaration for nautobot_device_onboarding."""
+
+# Metadata is inherited from Nautobot
+# If not including Nautobot in the environment, this should be added
 from importlib import metadata
 
-__version__ = metadata.version(__name__)
+from nautobot.apps import NautobotAppConfig
 
-from nautobot.extras.plugins import NautobotAppConfig
+__version__ = metadata.version(__name__)
 
 
 class NautobotDeviceOnboardingConfig(NautobotAppConfig):
-    """Plugin configuration for the nautobot_device_onboarding plugin."""
+    """App configuration for the nautobot_device_onboarding app."""
 
     name = "nautobot_device_onboarding"
     verbose_name = "Device Onboarding"
     version = __version__
     author = "Network to Code, LLC"
-    description = "Nautobot App that simplifies device onboarding (and re-onboarding) by collecting and populating common device 'facts' into Nautobot."
+    description = "Nautobot App that simplifies device onboarding (and re-onboarding) by \
+                   collecting and populating common device 'facts' into Nautobot."
     base_url = "nautobot-device-onboarding"
     required_settings = []
-    min_version = "2.0.3"
+    min_version = "2.1.1"
     max_version = "2.9999"
     default_settings = {
         "create_platform_if_missing": True,
         "create_manufacturer_if_missing": True,
         "create_device_type_if_missing": True,
         "create_device_role_if_missing": True,
         "default_device_role": "network",
@@ -30,14 +33,16 @@
         "default_management_prefix_length": 0,
         "default_device_status": "Active",
         "default_ip_status": "Active",
         "create_management_interface_if_missing": True,
         "skip_device_type_on_update": False,
         "skip_manufacturer_on_update": False,
         "platform_map": {},
+        "assign_secrets_group": False,
+        "set_management_only_interface": False,
         "onboarding_extensions_map": {
             "ios": "nautobot_device_onboarding.onboarding_extensions.ios",
         },
         "object_match_strategy": "loose",
     }
     caching_config = {}
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0001_initial.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.1.3 on 2021-02-22 03:40
 
-from django.db import migrations, models
-import django.db.models.deletion
 import uuid
 
+import django.db.models.deletion
+from django.db import migrations, models
+
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
         ("dcim", "0004_initial_part_4"),
     ]
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0001_squash__0001_0004_0005_0006.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0001_squash__0001_0004_0005_0006.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 3.2.21 on 2023-10-13 16:17
 
 import uuid
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 from nautobot.extras.models import RoleField
 
 
 class Migration(migrations.Migration):
     initial = True
 
     replaces = [
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0002_create_onboardingdevice.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0002_create_onboardingdevice.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0003_onboardingtask_label.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0003_onboardingtask_label.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_1.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.db import migrations, models
-
 from nautobot.extras.models import RoleField
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("nautobot_device_onboarding", "0001_initial"),
         ("dcim", "0029_device_and_rack_roles_data_migrations"),
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_2.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_2.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_3.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0004_migrate_to_extras_role_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_1.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_1.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_2.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_2.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_3.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0005_migrate_site_to_location_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_1.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_1.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_3.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0006_update_model_fields_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0008_alter_onboardingtask_options.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0008_alter_onboardingtask_options.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/migrations/0009_remove_models.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/migrations/0009_remove_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/nautobot_keeper.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/nautobot_keeper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Nautobot Keeper."""
 
-import logging
 import ipaddress
+import logging
 
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from nautobot.apps.choices import PrefixTypeChoices
 from nautobot.dcim.choices import InterfaceTypeChoices
-from nautobot.dcim.models import Manufacturer, Device, Interface, DeviceType
-from nautobot.extras.models import Role
-from nautobot.dcim.models import Platform
-from nautobot.dcim.models import Location
-from nautobot.extras.models import Status
+from nautobot.dcim.models import Device, DeviceType, Interface, Location, Manufacturer, Platform
+from nautobot.extras.models import Role, Status
 from nautobot.extras.models.customfields import CustomField
-from nautobot.ipam.models import IPAddress, Prefix, Namespace
+from nautobot.ipam.models import IPAddress, Namespace, Prefix
 
 from nautobot_device_onboarding.constants import NETMIKO_TO_NAPALM_STATIC
 from nautobot_device_onboarding.exceptions import OnboardException
 
 logger = logging.getLogger("rq.worker")
 
 PLUGIN_SETTINGS = settings.PLUGINS_CONFIG["nautobot_device_onboarding"]
@@ -89,14 +86,15 @@
         netdev_nb_platform_name=None,
         netdev_serial_number=None,
         netdev_mgmt_ifname=None,
         netdev_mgmt_pflen=None,
         netdev_netmiko_device_type=None,
         onboarding_class=None,
         driver_addon_result=None,
+        netdev_nb_credentials=None,
     ):
         """Create an instance and initialize the managed attributes that are used throughout the onboard processing.
 
         Args:
             netdev_hostname (str): Nautobot's device name
             netdev_nb_role_name (str): Nautobot's device role name
             netdev_vendor (str): Device's vendor name
@@ -108,21 +106,23 @@
             netdev_nb_platform_name (str): Nautobot device's platform name
             netdev_serial_number (str): Device's serial number
             netdev_mgmt_ifname (str): Device's management interface name
             netdev_mgmt_pflen (str): Device's management IP prefix-len
             netdev_netmiko_device_type (str): Device's Netmiko device type
             onboarding_class (Object): Onboarding Class (future use)
             driver_addon_result (Any): Attached extended result (future use)
+            netdev_nb_credentials (Object): Device's secrets group object
         """
         self.netdev_mgmt_ip_address = netdev_mgmt_ip_address
         self.netdev_nb_location_name = netdev_nb_location_name
         self.netdev_nb_device_type_name = netdev_nb_device_type_name
         self.netdev_nb_role_name = netdev_nb_role_name
         self.netdev_nb_role_color = netdev_nb_role_color
         self.netdev_nb_platform_name = netdev_nb_platform_name
+        self.netdev_nb_credentials = netdev_nb_credentials
 
         self.netdev_hostname = netdev_hostname
         self.netdev_vendor = netdev_vendor
         self.netdev_model = netdev_model
         self.netdev_serial_number = netdev_serial_number
         self.netdev_mgmt_ifname = netdev_mgmt_ifname
         self.netdev_mgmt_pflen = netdev_mgmt_pflen
@@ -290,16 +290,15 @@
                     f"fail-config - ERROR device role not found: {self.netdev_nb_role_name}"
                 ) from err
 
     def ensure_device_platform(self, create_platform_if_missing=PLUGIN_SETTINGS["create_platform_if_missing"]):
         """Get platform object from Nautobot filtered by platform_slug.
 
         Args:
-            platform_slug (string): slug of a platform object present in Nautobot, object will be created if not present
-            and create_platform_if_missing is enabled
+            create_platform_if_missing (bool): Flag to indicate if we need to create the platform, if not already present
 
         Return:
             nautobot.dcim.models.Platform object
 
         Raises:
             OnboardException
 
@@ -408,20 +407,29 @@
             raise OnboardException(
                 f"fail-general - ERROR multiple devices using same name in Nautobot: {self.netdev_hostname}",
             ) from err
 
     def ensure_interface(self):
         """Ensures that the interface associated with the mgmt_ipaddr exists and is assigned to the device."""
         if self.netdev_mgmt_ifname:
+            mgmt_only_setting = PLUGIN_SETTINGS["set_management_only_interface"]
+
             # TODO: Add option for default interface status
             self.nb_mgmt_ifname, _ = Interface.objects.get_or_create(
                 name=self.netdev_mgmt_ifname,
                 device=self.device,
-                defaults={"type": InterfaceTypeChoices.TYPE_OTHER, "status": Status.objects.get(name="Active")},
+                defaults={
+                    "type": InterfaceTypeChoices.TYPE_OTHER,
+                    "status": Status.objects.get(name="Active"),
+                    "mgmt_only": mgmt_only_setting,
+                },
             )
+            if mgmt_only_setting:
+                self.nb_mgmt_ifname.mgmt_only = mgmt_only_setting
+                self.nb_mgmt_ifname.validated_save()
 
             ensure_default_cf(obj=self.nb_mgmt_ifname, model=Interface)
 
     def ensure_primary_ip(self):
         """Ensure mgmt_ipaddr exists in IPAM, has the device interface, and is assigned as the primary IP address."""
         # see if the primary IP address exists in IPAM
         if self.netdev_mgmt_ip_address and self.netdev_mgmt_pflen:
@@ -464,20 +472,29 @@
                 self.nb_mgmt_ifname.save()
 
             # Ensure the primary IP is assigned to the device
             self.device.primary_ip4 = self.nb_primary_ip
             self.device.full_clean()
             self.device.save()
 
+    def ensure_secret_group(self):
+        """Optionally assign secret group from onboarding to created/updated device."""
+        if PLUGIN_SETTINGS["assign_secrets_group"]:
+            self.device.secrets_group = self.netdev_nb_credentials
+            self.device.validated_save()
+
     def ensure_device(self):
         """Ensure that the device represented by the DevNetKeeper exists in the Nautobot system."""
         self.ensure_onboarded_device()
         self.ensure_device_site()
         self.ensure_device_manufacturer()
         self.ensure_device_type()
         self.ensure_device_role()
         self.ensure_device_platform()
         self.ensure_device_instance()
 
         if PLUGIN_SETTINGS["create_management_interface_if_missing"]:
             self.ensure_interface()
             self.ensure_primary_ip()
+
+        if PLUGIN_SETTINGS["assign_secrets_group"]:
+            self.ensure_secret_group()
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/netdev_keeper.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/netdev_keeper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,23 @@
 
 import importlib
 import logging
 import socket
 
 from django.conf import settings
 from napalm import get_network_driver
-from napalm.base.exceptions import ConnectionException, CommandErrorException
+from napalm.base.exceptions import CommandErrorException, ConnectionException
 from napalm.base.netmiko_helpers import netmiko_args
-from netmiko import SSHDetect
-from netmiko import NetMikoAuthenticationException
-from netmiko import NetMikoTimeoutException
-from paramiko.ssh_exception import SSHException
-
 from nautobot.dcim.models import Platform
+from netmiko import NetMikoAuthenticationException, NetMikoTimeoutException, SSHDetect
+from paramiko.ssh_exception import SSHException
 
-from nautobot_device_onboarding.onboarding.onboarding import StandaloneOnboarding
 from nautobot_device_onboarding.constants import NETMIKO_TO_NAPALM_STATIC
 from nautobot_device_onboarding.exceptions import OnboardException
+from nautobot_device_onboarding.onboarding.onboarding import StandaloneOnboarding
 
 logger = logging.getLogger("rq.worker")
 
 PLUGIN_SETTINGS = settings.PLUGINS_CONFIG["nautobot_device_onboarding"]
 
 
 def get_mgmt_info(
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/onboarding/onboarding.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/onboarding/onboarding.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Onboarding module."""
 
 from nautobot_device_onboarding.nautobot_keeper import NautobotKeeper
 
 
-class Onboarding:  # pylint: disable=too-few-public-methods
+class Onboarding:
     """Generic onboarding class."""
 
     def __init__(self):
         """Init the class."""
         self.created_device = None
         self.credentials = None
 
     def run(self, onboarding_kwargs):
         """Implement run method."""
         raise NotImplementedError
 
 
-class StandaloneOnboarding(Onboarding):  # pylint: disable=too-few-public-methods
+class StandaloneOnboarding(Onboarding):
     """Standalone onboarding class."""
 
     def run(self, onboarding_kwargs):
         """Ensure device is created with Nautobot Keeper."""
         nb_k = NautobotKeeper(**onboarding_kwargs)
         nb_k.ensure_device()
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/onboarding_extensions/ios.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/onboarding_extensions/ios.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/tests/test_nautobot_keeper.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_nautobot_keeper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Unit tests for nautobot_device_onboarding.onboard module and its classes."""
+
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.test import TestCase
 from nautobot.dcim.choices import InterfaceTypeChoices
-from nautobot.dcim.models import Location, LocationType, Manufacturer, DeviceType, Device, Interface, Platform
-from nautobot.extras.models import Role, Status, CustomField
-from nautobot.ipam.models import IPAddress
+from nautobot.dcim.models import Device, DeviceType, Interface, Location, LocationType, Manufacturer, Platform
 from nautobot.extras.choices import CustomFieldTypeChoices
+from nautobot.extras.models import CustomField, Role, Status
+from nautobot.extras.models.secrets import SecretsGroup
+from nautobot.ipam.models import IPAddress
 
 from nautobot_device_onboarding.exceptions import OnboardException
 from nautobot_device_onboarding.nautobot_keeper import NautobotKeeper
 
 PLUGIN_SETTINGS = settings.PLUGINS_CONFIG["nautobot_device_onboarding"]
 
 
@@ -559,7 +561,33 @@
         self.assertEqual("cf_device_null" in device.cf, False)
         self.assertEqual(device.platform.cf["cf_platform"], True)
         self.assertEqual(device.device_type.cf["cf_devicetype"], 5)
         self.assertEqual(device.role.cf["cf_devicerole"], 10)
         self.assertEqual(device.device_type.manufacturer.cf["cf_manufacturer"], "Foobar!")
         self.assertEqual(device.interfaces.get(name="Management0").cf["cf_interface"], "2016-06-23")
         self.assertEqual(device.primary_ip.cf["cf_ipaddress"], "http://example.com/")
+
+    def test_ensure_secret_group_exist(self):
+        "Verify secret group assignment to device when specified in plugin config."
+
+        PLUGIN_SETTINGS["assign_secrets_group"] = True
+        test_secret_group = SecretsGroup.objects.create(name="test_secret_group")
+
+        onboarding_kwargs = {
+            "netdev_hostname": "device1",
+            "netdev_nb_role_name": "switch",
+            "netdev_vendor": "Cisco",
+            "netdev_model": "c2960",
+            "netdev_nb_location_name": self.site1,
+            "netdev_netmiko_device_type": "cisco_ios",
+            "netdev_serial_number": "123456",
+            "netdev_mgmt_ip_address": "192.0.2.10",
+            "netdev_mgmt_ifname": "GigaEthernet0",
+            "netdev_nb_credentials": test_secret_group,
+        }
+
+        nbk = NautobotKeeper(**onboarding_kwargs)
+
+        nbk.ensure_device()
+
+        nbk.ensure_secret_group()
+        self.assertEqual(nbk.netdev_nb_credentials.name, test_secret_group.name)
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/tests/test_onboarding.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/tests/test_onboarding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for nautobot_device_onboarding.netdev_keeper module and its classes."""
+
 # from unittest import mock
 
 from django.conf import settings
 
 # from django.test import TestCase
 # from django.contrib.contenttypes.models import ContentType
 
@@ -10,15 +11,15 @@
 # from nautobot.dcim.models import Device, Location, LocationType, Platform
 # from nautobot.extras.models import Status
 
 
 PLUGIN_SETTINGS = settings.PLUGINS_CONFIG["nautobot_device_onboarding"]
 
 
-class NapalmMock:  # pylint: disable=too-few-public-methods
+class NapalmMock:
     """Base napalm mock class for tests."""
 
     def __init__(self, *args, **kwargs):
         pass
 
     def open(self):
         """Mock test open ssh connection."""
@@ -62,15 +63,15 @@
         }
 
     def get_interfaces_ip(self):
         """Mock test get napalm interfaces on eos."""
         return {"Vlan100": {"ipv4": {"2.2.2.2": {"prefix_length": 32}}}}
 
 
-class SSHDetectMock:  # pylint: disable=too-few-public-methods
+class SSHDetectMock:
     """SSHDetect mock class for tests."""
 
     def __init__(self, *args, **kwargs):
         self.driver = args[0]
 
     def autodetect(self):
         """Mock test SSH."""
```

### Comparing `nautobot_device_onboarding-3.0.1/nautobot_device_onboarding/utils/credentials.py` & `nautobot_device_onboarding-4.0.0b1/nautobot_device_onboarding/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_onboarding-3.0.1/PKG-INFO` & `nautobot_device_onboarding-4.0.0b1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 Metadata-Version: 2.1
 Name: nautobot-device-onboarding
-Version: 3.0.1
-Summary: A plugin for Nautobot to easily onboard new devices.
-Home-page: https://github.com/nautobot/nautobot-plugin-device-onboarding
+Version: 4.0.0b1
+Summary: A app for Nautobot to easily onboard new devices.
+Home-page: https://github.com/nautobot/nautobot-app-device-onboarding
 License: Apache-2.0
-Keywords: nautobot,nautobot-plugin
+Keywords: nautobot,nautobot-app,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Requires-Dist: jdiff (>=0.0.6,<0.0.7)
 Requires-Dist: napalm (>=2.5.0,<5)
-Requires-Dist: nautobot (>=2.0.3,<3.0.0)
+Requires-Dist: nautobot (>=2.2.3,<3.0.0)
+Requires-Dist: nautobot-plugin-nornir (>=2.0.0,<3.0.0)
+Requires-Dist: nautobot-secrets-providers (>=2.0.1,<3.0.0)
+Requires-Dist: nautobot-ssot (>=2.6.0,<3.0.0)
+Requires-Dist: ntc-templates (>=5.1.0,<6.0.0)
+Requires-Dist: python-tss-sdk
 Requires-Dist: zipp (>=3.4.0,<4.0.0)
-Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-device-onboarding
+Project-URL: Repository, https://github.com/nautobot/nautobot-app-device-onboarding
 Description-Content-Type: text/markdown
 
 # Nautobot Device Onboarding
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-onboarding/develop/docs/images/icon-DeviceOnboarding.png" class="logo" height="200px">
+  <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-device-onboarding/develop/docs/images/icon-DeviceOnboarding.png" class="logo" height="200px">
   <br>
-  <a href="https://github.com/nautobot/nautobot-plugin-device-onboarding/actions"><img src="https://github.com/nautobot/nautobot-plugin-device-onboarding/actions/workflows/ci.yml/badge.svg?branch=develop"></a>
-  <a href="https://docs.nautobot.com/projects/device-onboarding/"><img src="https://readthedocs.org/projects/nautobot-plugin-device-onboarding/badge/"></a>
+  <a href="https://github.com/nautobot/nautobot-app-device-onboarding/actions"><img src="https://github.com/nautobot/nautobot-app-device-onboarding/actions/workflows/ci.yml/badge.svg?branch=develop"></a>
+  <a href="https://docs.nautobot.com/projects/device-onboarding/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-device-onboarding/badge/"></a>
   <a href="https://pypi.org/project/nautobot-device-onboarding/"><img src="https://img.shields.io/pypi/v/nautobot-device-onboarding"></a>
   <a href="https://pypi.org/project/nautobot-device-onboarding/"><img src="https://img.shields.io/pypi/dm/nautobot-device-onboarding"></a>
   <br>
   A plugin for <a href="https://github.com/nautobot/nautobot">Nautobot</a> to easily onboard new devices.
 </p>
 
 ## Overview
 
 The `nautobot-device-onboarding` plugin is using the [netmiko](https://github.com/ktbyers/netmiko) and [NAPALM](https://napalm.readthedocs.io/en/latest/) libraries to simplify the onboarding process of a new device into Nautobot down to, in many cases, an *IP Address* and a *Location*. In some cases, the user may also have to specify a specific *Device Platform* and *Device Port*.
 
-Regardless, the Onboarding Plugin greatly simplifies the onboarding process by allowing the user to specify a small amount of info and having the app populate a much larger amount of device data in Nautobot.
+Regardless, the Onboarding App greatly simplifies the onboarding process by allowing the user to specify a small amount of info and having the app populate a much larger amount of device data in Nautobot.
 
 ### Screenshots
 
 Device Onboarding is a Job that allows you to provide a few required pieces of information and onboard the device.
 
-![job input](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-onboarding/develop/docs/images/do_job_inputs.png)
+![job input](https://raw.githubusercontent.com/nautobot/nautobot-app-device-onboarding/develop/docs/images/do_job_inputs.png)
 
 ## Try it out!
 
 This App is installed in the Nautobot Community Sandbox found over at [demo.nautobot.com](https://demo.nautobot.com/)!
 
 > For a full list of all the available always-on sandbox environments, head over to the main page on [networktocode.com](https://www.networktocode.com/nautobot/sandbox-environments/).
 
@@ -61,15 +68,15 @@
 - [Administrator Guide](https://docs.nautobot.com/projects/device-onboarding/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the App.
 - [Developer Guide](https://docs.nautobot.com/projects/device-onboarding/en/latest/dev/contributing/) - Extending the App, Code Reference, Contribution Guide.
 - [Release Notes / Changelog](https://docs.nautobot.com/projects/device-onboarding/en/latest/admin/release_notes/).
 - [Frequently Asked Questions](https://docs.nautobot.com/projects/device-onboarding/en/latest/user/faq/).
 
 ### Contributing to the Docs
 
-You can find all the Markdown source for the App documentation under the [docs](https://github.com/nautobot/nautobot-plugin-device-onboarding/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient - clone the repository and edit away.
+You can find all the Markdown source for the App documentation under the [`docs`](https://github.com/nautobot/nautobot-app-device-onboarding/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient: clone the repository and edit away.
 
 If you need to view the fully generated documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be started using the invoke commands (details in the [Development Environment Guide](https://docs.nautobot.com/projects/device-onboarding/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). As your changes are saved, the live docs will be automatically reloaded.
 
 Any PRs with fixes or improvements are very welcome!
 
 ## Questions
```

#### html2text {}

```diff
@@ -1,65 +1,67 @@
-Metadata-Version: 2.1 Name: nautobot-device-onboarding Version: 3.0.1 Summary:
-A plugin for Nautobot to easily onboard new devices. Home-page: https://
-github.com/nautobot/nautobot-plugin-device-onboarding License: Apache-2.0
-Keywords: nautobot,nautobot-plugin Author: Network to Code, LLC Author-email:
-info@networktocode.com Requires-Python: >=3.8,<3.12 Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: napalm (>=2.5.0,<5) Requires-Dist: nautobot
-(>=2.0.3,<3.0.0) Requires-Dist: zipp (>=3.4.0,<4.0.0) Project-URL: Repository,
-https://github.com/nautobot/nautobot-plugin-device-onboarding Description-
-Content-Type: text/markdown # Nautobot Device Onboarding
-[https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-onboarding/
+Metadata-Version: 2.1 Name: nautobot-device-onboarding Version: 4.0.0b1
+Summary: A app for Nautobot to easily onboard new devices. Home-page: https://
+github.com/nautobot/nautobot-app-device-onboarding License: Apache-2.0
+Keywords: nautobot,nautobot-app,nautobot-plugin Author: Network to Code, LLC
+Author-email: info@networktocode.com Requires-Python: >=3.8,<3.12 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Provides-Extra: all Requires-Dist: jdiff
+(>=0.0.6,<0.0.7) Requires-Dist: napalm (>=2.5.0,<5) Requires-Dist: nautobot
+(>=2.2.3,<3.0.0) Requires-Dist: nautobot-plugin-nornir (>=2.0.0,<3.0.0)
+Requires-Dist: nautobot-secrets-providers (>=2.0.1,<3.0.0) Requires-Dist:
+nautobot-ssot (>=2.6.0,<3.0.0) Requires-Dist: ntc-templates (>=5.1.0,<6.0.0)
+Requires-Dist: python-tss-sdk Requires-Dist: zipp (>=3.4.0,<4.0.0) Project-URL:
+Repository, https://github.com/nautobot/nautobot-app-device-onboarding
+Description-Content-Type: text/markdown # Nautobot Device Onboarding
+  [https://raw.githubusercontent.com/nautobot/nautobot-app-device-onboarding/
                 develop/docs/images/icon-DeviceOnboarding.png]
-    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_/_a_c_t_i_o_n_s_/
- _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_e_l_o_p_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/
-   _n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
-  _n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-
-                                  _o_n_b_o_a_r_d_i_n_g_]
+_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/
+  _c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_e_l_o_p_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-
+_p_l_u_g_i_n_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-
+    _o_n_b_o_a_r_d_i_n_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_o_n_b_o_a_r_d_i_n_g_]
              A plugin for _N_a_u_t_o_b_o_t to easily onboard new devices.
 ## Overview The `nautobot-device-onboarding` plugin is using the [netmiko]
 (https://github.com/ktbyers/netmiko) and [NAPALM](https://
 napalm.readthedocs.io/en/latest/) libraries to simplify the onboarding process
 of a new device into Nautobot down to, in many cases, an *IP Address* and a
 *Location*. In some cases, the user may also have to specify a specific *Device
-Platform* and *Device Port*. Regardless, the Onboarding Plugin greatly
-simplifies the onboarding process by allowing the user to specify a small
-amount of info and having the app populate a much larger amount of device data
-in Nautobot. ### Screenshots Device Onboarding is a Job that allows you to
-provide a few required pieces of information and onboard the device. ![job
-input](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-
-onboarding/develop/docs/images/do_job_inputs.png) ## Try it out! This App is
-installed in the Nautobot Community Sandbox found over at [demo.nautobot.com]
-(https://demo.nautobot.com/)! > For a full list of all the available always-on
-sandbox environments, head over to the main page on [networktocode.com](https:/
-/www.networktocode.com/nautobot/sandbox-environments/). ## Documentation Full
-web-based HTML documentation for this app can be found over on the [Nautobot
-Docs](https://docs.nautobot.com/) website: - [User Guide](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/user/app_overview/) -
-Overview, Using the App, Getting Started. - [Administrator Guide](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/admin/install/) - How to
-Install, Configure, Upgrade, or Uninstall the App. - [Developer Guide](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/dev/contributing/) -
-Extending the App, Code Reference, Contribution Guide. - [Release Notes /
-Changelog](https://docs.nautobot.com/projects/device-onboarding/en/latest/
-admin/release_notes/). - [Frequently Asked Questions](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/user/faq/). ###
-Contributing to the Docs You can find all the Markdown source for the App
-documentation under the [docs](https://github.com/nautobot/nautobot-plugin-
-device-onboarding/tree/develop/docs) folder in this repository. For simple
-edits, a Markdown capable editor is sufficient - clone the repository and edit
-away. If you need to view the fully generated documentation site, you can build
-it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be
-started using the invoke commands (details in the [Development Environment
-Guide](https://docs.nautobot.com/projects/device-onboarding/en/latest/dev/
-dev_environment/#docker-development-environment)) on [http://localhost:8001]
-(http://localhost:8001). As your changes are saved, the live docs will be
-automatically reloaded. Any PRs with fixes or improvements are very welcome! ##
-Questions For any questions or comments, please check the [FAQ](https://
-docs.nautobot.com/projects/device-onboarding/en/latest/user/faq/) first. Feel
-free to also swing by the [Network to Code Slack](https://
-networktocode.slack.com/) (channel `#nautobot`), sign up [here](http://
-slack.networktocode.com/) if you don't have an account.
+Platform* and *Device Port*. Regardless, the Onboarding App greatly simplifies
+the onboarding process by allowing the user to specify a small amount of info
+and having the app populate a much larger amount of device data in Nautobot.
+### Screenshots Device Onboarding is a Job that allows you to provide a few
+required pieces of information and onboard the device. ![job input](https://
+raw.githubusercontent.com/nautobot/nautobot-app-device-onboarding/develop/docs/
+images/do_job_inputs.png) ## Try it out! This App is installed in the Nautobot
+Community Sandbox found over at [demo.nautobot.com](https://demo.nautobot.com/
+)! > For a full list of all the available always-on sandbox environments, head
+over to the main page on [networktocode.com](https://www.networktocode.com/
+nautobot/sandbox-environments/). ## Documentation Full web-based HTML
+documentation for this app can be found over on the [Nautobot Docs](https://
+docs.nautobot.com/) website: - [User Guide](https://docs.nautobot.com/projects/
+device-onboarding/en/latest/user/app_overview/) - Overview, Using the App,
+Getting Started. - [Administrator Guide](https://docs.nautobot.com/projects/
+device-onboarding/en/latest/admin/install/) - How to Install, Configure,
+Upgrade, or Uninstall the App. - [Developer Guide](https://docs.nautobot.com/
+projects/device-onboarding/en/latest/dev/contributing/) - Extending the App,
+Code Reference, Contribution Guide. - [Release Notes / Changelog](https://
+docs.nautobot.com/projects/device-onboarding/en/latest/admin/release_notes/). -
+[Frequently Asked Questions](https://docs.nautobot.com/projects/device-
+onboarding/en/latest/user/faq/). ### Contributing to the Docs You can find all
+the Markdown source for the App documentation under the [`docs`](https://
+github.com/nautobot/nautobot-app-device-onboarding/tree/develop/docs) folder in
+this repository. For simple edits, a Markdown capable editor is sufficient:
+clone the repository and edit away. If you need to view the fully generated
+documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A
+container hosting the docs will be started using the invoke commands (details
+in the [Development Environment Guide](https://docs.nautobot.com/projects/
+device-onboarding/en/latest/dev/dev_environment/#docker-development-
+environment)) on [http://localhost:8001](http://localhost:8001). As your
+changes are saved, the live docs will be automatically reloaded. Any PRs with
+fixes or improvements are very welcome! ## Questions For any questions or
+comments, please check the [FAQ](https://docs.nautobot.com/projects/device-
+onboarding/en/latest/user/faq/) first. Feel free to also swing by the [Network
+to Code Slack](https://networktocode.slack.com/) (channel `#nautobot`), sign up
+[here](http://slack.networktocode.com/) if you don't have an account.
```

