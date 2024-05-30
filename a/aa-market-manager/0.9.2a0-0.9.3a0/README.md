# Comparing `tmp/aa-market-manager-0.9.2a0.tar.gz` & `tmp/aa-market-manager-0.9.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-market-manager-0.9.2a0.tar", last modified: Thu Aug  4 11:04:24 2022, max compression
+gzip compressed data, was "aa-market-manager-0.9.3a0.tar", last modified: Sat Aug  6 06:29:47 2022, max compression
```

## Comparing `aa-market-manager-0.9.2a0.tar` & `aa-market-manager-0.9.3a0.tar`

### file list

```diff
@@ -1,154 +1,155 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.776088 aa-market-manager-0.9.2a0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      177 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12883 2022-08-04 11:04:24.776088 aa-market-manager-0.9.2a0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11914 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.741085 aa-market-manager-0.9.2a0/aa_market_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12883 2022-08-04 11:04:24.000000 aa-market-manager-0.9.2a0/aa_market_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5947 2022-08-04 11:04:24.000000 aa-market-manager-0.9.2a0/aa_market_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-04 11:04:24.000000 aa-market-manager-0.9.2a0/aa_market_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2022-08-04 11:04:24.000000 aa-market-manager-0.9.2a0/aa_market_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-08-04 11:04:24.000000 aa-market-manager-0.9.2a0/aa_market_manager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.747086 aa-market-manager-0.9.2a0/marketmanager/
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.747086 aa-market-manager-0.9.2a0/marketmanager/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      284 2022-08-04 11:04:24.000000 aa-market-manager-0.9.2a0/marketmanager/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     5587 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/buybacks.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/fittings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.734084 aa-market-manager-0.9.2a0/marketmanager/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.731084 aa-market-manager-0.9.2a0/marketmanager/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.748086 aa-market-manager-0.9.2a0/marketmanager/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     3920 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.731084 aa-market-manager-0.9.2a0/marketmanager/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.749086 aa-market-manager-0.9.2a0/marketmanager/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     3919 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.732084 aa-market-manager-0.9.2a0/marketmanager/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.749086 aa-market-manager-0.9.2a0/marketmanager/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      385 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     3921 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.732084 aa-market-manager-0.9.2a0/marketmanager/locale/fr_FR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.750086 aa-market-manager-0.9.2a0/marketmanager/locale/fr_FR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      398 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/fr_FR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     3934 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.733084 aa-market-manager-0.9.2a0/marketmanager/locale/it_IT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.750086 aa-market-manager-0.9.2a0/marketmanager/locale/it_IT/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      399 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/it_IT/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     3935 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.733084 aa-market-manager-0.9.2a0/marketmanager/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.751086 aa-market-manager-0.9.2a0/marketmanager/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      379 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     3915 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.733084 aa-market-manager-0.9.2a0/marketmanager/locale/ko_KR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.752086 aa-market-manager-0.9.2a0/marketmanager/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      391 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/ko_KR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     3927 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.734084 aa-market-manager-0.9.2a0/marketmanager/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.752086 aa-market-manager-0.9.2a0/marketmanager/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      523 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     4059 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.734084 aa-market-manager-0.9.2a0/marketmanager/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.753086 aa-market-manager-0.9.2a0/marketmanager/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      399 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     3935 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.735085 aa-market-manager-0.9.2a0/marketmanager/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.753086 aa-market-manager-0.9.2a0/marketmanager/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     1522 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/management/commands/marketmanager_preload_common_eve_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.768088 aa-market-manager-0.9.2a0/marketmanager/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7797 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0001_squashed_0014_alter_privateconfig_valid_corporations_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0002_alter_structure_created_at_alter_watchconfig_type.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0002_auto_20211129_1339.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0003_alter_general_options.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0003_rename_type_watchconfig_eve_type.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0004_alter_order_wallet_division.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0004_alter_watchconfig_jita_compare_percent_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0005_alter_general_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1568 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0005_alter_watchconfig_constellation_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0006_auto_20211201_1343.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0006_watchconfig_config_type_alter_watchconfig_webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)      493 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0007_alter_order_is_buy_order.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0007_rename_webhook_webhook_url_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1042 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0008_alter_general_options.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0008_alter_order_state.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0009_remove_watchconfig_fail_webhooks_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     2226 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0009_rename_config_publicconfig_order_source_character_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0010_alter_watchconfig_debug_webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0010_order_source_private.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0011_alter_privateconfig_failed_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0011_rename_location_watchconfig_structure.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0012_remove_watchconfig_constellation.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0012_structure_created_at_structure_updated_at_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1042 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0013_alter_privateconfig_failure_reason_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0013_watchconfig_managed_app_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0014_alter_privateconfig_valid_corporations_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0014_alter_watchconfig_price_typestatistics.py
--rw-rw-rw-   0 root         (0) root         (0)     2424 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0015_typestatistics_eve_region_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0016_alter_typestatistics_eve_region.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0017_alter_watchconfig_managed_app_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0018_remove_typestatistics_buy_5_percent_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0019_remove_order_escrow_remove_order_source_character_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     3469 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0020_alter_order_duration_alter_order_price_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0021_typestatistics_new_eden.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0022_remove_typestatistics_evetypeeveregiontypestatistic.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0023_alter_typestatistics_eve_region.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0024_remove_typestatistics_new_eden.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0025_statisticsconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0026_alter_publicconfig_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0027_managedwatchconfig_remove_watchconfig_managed_app_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0028_rename_manged_app_reason_managedwatchconfig_managed_app_reason.py
--rw-rw-rw-   0 root         (0) root         (0)     3053 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0029_managedwatchconfig_managed_buy_order_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     2002 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0030_channel_managedwatchconfig_managed_channels_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/0031_alter_channel_name.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16172 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4238 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.736085 aa-market-manager-0.9.2a0/marketmanager/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.736085 aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.768088 aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/css/
--rw-rw-rw-   0 root         (0) root         (0)      964 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/css/marketmanager.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.768088 aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/icons/
--rw-rw-rw-   0 root         (0) root         (0)     1569 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/icons/Market.png
--rw-rw-rw-   0 root         (0) root         (0)     3124 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/icons/Searchmarket.png
--rw-rw-rw-   0 root         (0) root         (0)   852943 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     8143 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/task_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    26680 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.737085 aa-market-manager-0.9.2a0/marketmanager/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.769088 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.771088 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/buy_orders.html
--rw-rw-rw-   0 root         (0) root         (0)     3240 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/item_details.html
--rw-rw-rw-   0 root         (0) root         (0)      695 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/item_selector.html
--rw-rw-rw-   0 root         (0) root         (0)      905 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/region_selector.html
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/search.html
--rw-rw-rw-   0 root         (0) root         (0)     1032 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/sell_orders.html
--rw-rw-rw-   0 root         (0) root         (0)     6616 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.772088 aa-market-manager-0.9.2a0/marketmanager/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.772088 aa-market-manager-0.9.2a0/marketmanager/tests/esi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/esi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2248 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/esi/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/test_providers.py
--rw-rw-rw-   0 root         (0) root         (0)     3651 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/test_task_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/test_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.774088 aa-market-manager-0.9.2a0/marketmanager/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/testdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/testdata/create_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)    56804 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/testdata/eveuniverse.json
--rw-rw-rw-   0 root         (0) root         (0)      383 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/tests/testdata/load_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    11525 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/marketmanager/views.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-08-04 11:04:24.777088 aa-market-manager-0.9.2a0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1681 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 11:04:24.776088 aa-market-manager-0.9.2a0/testauth/
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/testauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/testauth/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    11114 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/testauth/settingsAA2.py
--rw-rw-rw-   0 root         (0) root         (0)    11125 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/testauth/settingsAA3.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/testauth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2022-08-04 11:04:16.000000 aa-market-manager-0.9.2a0/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.588244 aa-market-manager-0.9.3a0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      177 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12883 2022-08-06 06:29:47.588244 aa-market-manager-0.9.3a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11914 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.551240 aa-market-manager-0.9.3a0/aa_market_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12883 2022-08-06 06:29:47.000000 aa-market-manager-0.9.3a0/aa_market_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6019 2022-08-06 06:29:47.000000 aa-market-manager-0.9.3a0/aa_market_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-06 06:29:47.000000 aa-market-manager-0.9.3a0/aa_market_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2022-08-06 06:29:47.000000 aa-market-manager-0.9.3a0/aa_market_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2022-08-06 06:29:47.000000 aa-market-manager-0.9.3a0/aa_market_manager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.557241 aa-market-manager-0.9.3a0/marketmanager/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.557241 aa-market-manager-0.9.3a0/marketmanager/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      284 2022-08-06 06:29:47.000000 aa-market-manager-0.9.3a0/marketmanager/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     5592 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/buybacks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/fittings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.544240 aa-market-manager-0.9.3a0/marketmanager/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.540239 aa-market-manager-0.9.3a0/marketmanager/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.558241 aa-market-manager-0.9.3a0/marketmanager/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.540239 aa-market-manager-0.9.3a0/marketmanager/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.558241 aa-market-manager-0.9.3a0/marketmanager/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3919 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.541239 aa-market-manager-0.9.3a0/marketmanager/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.559241 aa-market-manager-0.9.3a0/marketmanager/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      385 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.541239 aa-market-manager-0.9.3a0/marketmanager/locale/fr_FR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.560241 aa-market-manager-0.9.3a0/marketmanager/locale/fr_FR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      398 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3934 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.542239 aa-market-manager-0.9.3a0/marketmanager/locale/it_IT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.560241 aa-market-manager-0.9.3a0/marketmanager/locale/it_IT/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      399 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/it_IT/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3935 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.542239 aa-market-manager-0.9.3a0/marketmanager/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.561241 aa-market-manager-0.9.3a0/marketmanager/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      379 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.543239 aa-market-manager-0.9.3a0/marketmanager/locale/ko_KR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.562241 aa-market-manager-0.9.3a0/marketmanager/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      391 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3927 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.543239 aa-market-manager-0.9.3a0/marketmanager/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.562241 aa-market-manager-0.9.3a0/marketmanager/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4059 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.544240 aa-market-manager-0.9.3a0/marketmanager/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.563241 aa-market-manager-0.9.3a0/marketmanager/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      399 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3935 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.544240 aa-market-manager-0.9.3a0/marketmanager/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.563241 aa-market-manager-0.9.3a0/marketmanager/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/management/commands/marketmanager_preload_common_eve_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.579243 aa-market-manager-0.9.3a0/marketmanager/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7797 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0001_squashed_0014_alter_privateconfig_valid_corporations_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0002_alter_structure_created_at_alter_watchconfig_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0002_auto_20211129_1339.py
+-rw-rw-rw-   0 root         (0) root         (0)      582 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0003_alter_general_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0003_rename_type_watchconfig_eve_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      525 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0004_alter_order_wallet_division.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0004_alter_watchconfig_jita_compare_percent_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0005_alter_general_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0005_alter_watchconfig_constellation_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0006_auto_20211201_1343.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0006_watchconfig_config_type_alter_watchconfig_webhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      493 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0007_alter_order_is_buy_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0007_rename_webhook_webhook_url_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0008_alter_general_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0008_alter_order_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0009_remove_watchconfig_fail_webhooks_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     2226 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0009_rename_config_publicconfig_order_source_character_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0010_alter_watchconfig_debug_webhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0010_order_source_private.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0011_alter_privateconfig_failed_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0011_rename_location_watchconfig_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0012_remove_watchconfig_constellation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0012_structure_created_at_structure_updated_at_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0013_alter_privateconfig_failure_reason_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0013_watchconfig_managed_app_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0014_alter_privateconfig_valid_corporations_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0014_alter_watchconfig_price_typestatistics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2424 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0015_typestatistics_eve_region_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0016_alter_typestatistics_eve_region.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0017_alter_watchconfig_managed_app_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0018_remove_typestatistics_buy_5_percent_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0019_remove_order_escrow_remove_order_source_character_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     3469 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0020_alter_order_duration_alter_order_price_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0021_typestatistics_new_eden.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0022_remove_typestatistics_evetypeeveregiontypestatistic.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0023_alter_typestatistics_eve_region.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0024_remove_typestatistics_new_eden.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0025_statisticsconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0026_alter_publicconfig_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0027_managedwatchconfig_remove_watchconfig_managed_app_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0028_rename_manged_app_reason_managedwatchconfig_managed_app_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0029_managedwatchconfig_managed_buy_order_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0030_channel_managedwatchconfig_managed_channels_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0031_alter_channel_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/0032_alter_watchconfig_managed_watch_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16193 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.545240 aa-market-manager-0.9.3a0/marketmanager/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.546240 aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.580243 aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/css/
+-rw-rw-rw-   0 root         (0) root         (0)      964 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/css/marketmanager.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.580243 aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/icons/Market.png
+-rw-rw-rw-   0 root         (0) root         (0)     3124 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/icons/Searchmarket.png
+-rw-rw-rw-   0 root         (0) root         (0)   852943 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/swagger.json
+-rw-rw-rw-   0 root         (0) root         (0)     8416 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/task_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    26697 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.546240 aa-market-manager-0.9.3a0/marketmanager/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.581243 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.583243 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/buy_orders.html
+-rw-rw-rw-   0 root         (0) root         (0)     3240 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/item_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      695 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/item_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)      905 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/region_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)      229 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/search.html
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/sell_orders.html
+-rw-rw-rw-   0 root         (0) root         (0)     6616 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.584243 aa-market-manager-0.9.3a0/marketmanager/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.585243 aa-market-manager-0.9.3a0/marketmanager/tests/esi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/esi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/esi/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      435 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/test_providers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/test_task_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/test_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.586243 aa-market-manager-0.9.3a0/marketmanager/tests/testdata/
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/testdata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/testdata/create_eveuniverse.py
+-rw-rw-rw-   0 root         (0) root         (0)    56804 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/testdata/eveuniverse.json
+-rw-rw-rw-   0 root         (0) root         (0)      383 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/tests/testdata/load_eveuniverse.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    11525 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/marketmanager/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2022-08-06 06:29:47.589244 aa-market-manager-0.9.3a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-06 06:29:47.588244 aa-market-manager-0.9.3a0/testauth/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/testauth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/testauth/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    11114 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/testauth/settingsAA2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11125 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/testauth/settingsAA3.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/testauth/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2022-08-06 06:29:38.000000 aa-market-manager-0.9.3a0/testauth/wsgi.py
```

### Comparing `aa-market-manager-0.9.2a0/LICENSE` & `aa-market-manager-0.9.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/PKG-INFO` & `aa-market-manager-0.9.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-market-manager
-Version: 0.9.2a0
+Version: 0.9.3a0
 Summary: AllianceAuth Market Management Tool
 Home-page: https://gitlab.com/tactical-supremacy/aa-market-manager
 Author: Joel Falknau
 Author-email: ozirascal@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-market-manager-0.9.2a0/README.md` & `aa-market-manager-0.9.3a0/README.md`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/aa_market_manager.egg-info/PKG-INFO` & `aa-market-manager-0.9.3a0/aa_market_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-market-manager
-Version: 0.9.2a0
+Version: 0.9.3a0
 Summary: AllianceAuth Market Management Tool
 Home-page: https://gitlab.com/tactical-supremacy/aa-market-manager
 Author: Joel Falknau
 Author-email: ozirascal@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-market-manager-0.9.2a0/aa_market_manager.egg-info/SOURCES.txt` & `aa-market-manager-0.9.3a0/aa_market_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 marketmanager/migrations/0025_statisticsconfig.py
 marketmanager/migrations/0026_alter_publicconfig_options_and_more.py
 marketmanager/migrations/0027_managedwatchconfig_remove_watchconfig_managed_app_and_more.py
 marketmanager/migrations/0028_rename_manged_app_reason_managedwatchconfig_managed_app_reason.py
 marketmanager/migrations/0029_managedwatchconfig_managed_buy_order_and_more.py
 marketmanager/migrations/0030_channel_managedwatchconfig_managed_channels_and_more.py
 marketmanager/migrations/0031_alter_channel_name.py
+marketmanager/migrations/0032_alter_watchconfig_managed_watch_config.py
 marketmanager/migrations/__init__.py
 marketmanager/static/marketmanager/css/marketmanager.css
 marketmanager/static/marketmanager/icons/Market.png
 marketmanager/static/marketmanager/icons/Searchmarket.png
 marketmanager/templates/marketmanager/marketbrowser.html
 marketmanager/templates/marketmanager/marketbrowser/buy_orders.html
 marketmanager/templates/marketmanager/marketbrowser/item_details.html
```

### Comparing `aa-market-manager-0.9.2a0/marketmanager/admin.py` & `aa-market-manager-0.9.3a0/marketmanager/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 @admin.register(Channel)
 class ChannelAdmin(admin.ModelAdmin):
     list_display = ('name', )
 
 @admin.register(ManagedWatchConfig)
 class ManagedWatchConfigAdmin(admin.ModelAdmin):
-    list_display = ('managed_app', 'managed_app_identifier', 'managed_app_reason' )
+    list_display = ('managed_app_reason', 'managed_quantity', 'managed_app_identifier' )
     filter_horizontal = ["managed_structure", "managed_structure_type", "managed_webhooks", "managed_debug_webhooks", "managed_solar_system", "managed_region", "managed_channels", "managed_debug_channels"]
     list_filter = ('managed_buy_order', 'managed_webhooks', 'managed_debug_webhooks')
 
     def formfield_for_foreignkey(self, db_field, request, **kwargs):
         # Only items that have market groups?
         if db_field.name == "managed_eve_type":
             kwargs["queryset"] = EveType.objects.filter(eve_market_group__isnull=False)
```

### Comparing `aa-market-manager-0.9.2a0/marketmanager/app_settings.py` & `aa-market-manager-0.9.3a0/marketmanager/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/auth_hooks.py` & `aa-market-manager-0.9.3a0/marketmanager/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/fittings.py` & `aa-market-manager-0.9.3a0/marketmanager/fittings.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/de/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/en/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/es/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/fr_FR/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/it_IT/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/ja/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/ko_KR/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/ru/LC_MESSAGES/django.mo` & `aa-market-manager-0.9.3a0/marketmanager/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/ru/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/locale/zh_Hans/LC_MESSAGES/django.po` & `aa-market-manager-0.9.3a0/marketmanager/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/management/commands/marketmanager_preload_common_eve_types.py` & `aa-market-manager-0.9.3a0/marketmanager/management/commands/marketmanager_preload_common_eve_types.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0001_initial.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0001_squashed_0014_alter_privateconfig_valid_corporations_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0001_squashed_0014_alter_privateconfig_valid_corporations_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0002_alter_structure_created_at_alter_watchconfig_type.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0002_alter_structure_created_at_alter_watchconfig_type.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0002_auto_20211129_1339.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0002_auto_20211129_1339.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0003_alter_general_options.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0003_alter_general_options.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0004_alter_order_wallet_division.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0004_alter_order_wallet_division.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0004_alter_watchconfig_jita_compare_percent_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0004_alter_watchconfig_jita_compare_percent_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0005_alter_general_options.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0005_alter_general_options.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0005_alter_watchconfig_constellation_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0005_alter_watchconfig_constellation_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0006_auto_20211201_1343.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0006_auto_20211201_1343.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0006_watchconfig_config_type_alter_watchconfig_webhooks.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0006_watchconfig_config_type_alter_watchconfig_webhooks.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0007_rename_webhook_webhook_url_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0007_rename_webhook_webhook_url_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0008_alter_general_options.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0008_alter_general_options.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0008_alter_order_state.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0008_alter_order_state.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0009_remove_watchconfig_fail_webhooks_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0009_remove_watchconfig_fail_webhooks_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0009_rename_config_publicconfig_order_source_character_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0009_rename_config_publicconfig_order_source_character_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0010_alter_watchconfig_debug_webhooks.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0010_alter_watchconfig_debug_webhooks.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0011_alter_privateconfig_failed_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0011_alter_privateconfig_failed_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0012_structure_created_at_structure_updated_at_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0012_structure_created_at_structure_updated_at_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0013_alter_privateconfig_failure_reason_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0013_alter_privateconfig_failure_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0013_watchconfig_managed_app_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0013_watchconfig_managed_app_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0014_alter_privateconfig_valid_corporations_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0014_alter_privateconfig_valid_corporations_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0014_alter_watchconfig_price_typestatistics.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0014_alter_watchconfig_price_typestatistics.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0015_typestatistics_eve_region_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0015_typestatistics_eve_region_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0016_alter_typestatistics_eve_region.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0016_alter_typestatistics_eve_region.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0017_alter_watchconfig_managed_app_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0017_alter_watchconfig_managed_app_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0018_remove_typestatistics_buy_5_percent_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0018_remove_typestatistics_buy_5_percent_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0019_remove_order_escrow_remove_order_source_character_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0019_remove_order_escrow_remove_order_source_character_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0020_alter_order_duration_alter_order_price_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0020_alter_order_duration_alter_order_price_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0023_alter_typestatistics_eve_region.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0023_alter_typestatistics_eve_region.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0025_statisticsconfig.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0025_statisticsconfig.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0026_alter_publicconfig_options_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0026_alter_publicconfig_options_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0027_managedwatchconfig_remove_watchconfig_managed_app_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0027_managedwatchconfig_remove_watchconfig_managed_app_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0029_managedwatchconfig_managed_buy_order_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0029_managedwatchconfig_managed_buy_order_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/migrations/0030_channel_managedwatchconfig_managed_channels_and_more.py` & `aa-market-manager-0.9.3a0/marketmanager/migrations/0030_channel_managedwatchconfig_managed_channels_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/models.py` & `aa-market-manager-0.9.3a0/marketmanager/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
         Channel,
         verbose_name=_("Debug Channels"),
         related_name="debug_channels",
         blank=True,
         help_text="Primarily for Testing/Debugging Purposes. This webhook will receive updates on WatchConfigs that _dont_ notify. Because their Configs didnt Meet/Breach.")
     managed_watch_config = models.ForeignKey(
         ManagedWatchConfig,
-        verbose_name=_(""),
+        verbose_name=_("Managed Watch Configs"),
         on_delete=models.CASCADE,
         null=True)
     class Meta:
         """
         Meta definitions
         """
         default_permissions = ()
```

### Comparing `aa-market-manager-0.9.2a0/marketmanager/providers.py` & `aa-market-manager-0.9.3a0/marketmanager/providers.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/css/marketmanager.css` & `aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/css/marketmanager.css`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/icons/Market.png` & `aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/icons/Market.png`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/static/marketmanager/icons/Searchmarket.png` & `aa-market-manager-0.9.3a0/marketmanager/static/marketmanager/icons/Searchmarket.png`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/swagger.json` & `aa-market-manager-0.9.3a0/marketmanager/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/task_helpers.py` & `aa-market-manager-0.9.3a0/marketmanager/task_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import random
 from typing import Union
 
 from discord import Embed
 from eveuniverse.models import EveRegion, EveType
 
 from django.core.exceptions import ObjectDoesNotExist
@@ -111,14 +112,15 @@
         title = f"{config.eve_type.name}",
         description = description,
         colour = colour,
         url = f"{get_site_url()}/marketmanager/marketbrowser?type_id={config.eve_type.id}",
     )
 
     embed.set_thumbnail(url = config.eve_type.icon_url())
+    embed.timestamp = datetime.datetime.now()
     embed.set_footer(
         icon_url = "",
         text = f"AA Market Manager v{__version__}"
     )
 
     if buy_order is True:
         buy_order_string = "BUY"
@@ -175,18 +177,22 @@
         embed.add_field(
             name = "Structure_Types",
             value = structure_type_string,
             inline = False
         )
 
     if config.managed_watch_config is not None:
+        if config.managed_watch_config.managed_app == 'fittings':
+            managed_app = "AA-Fittings"
+        else:
+            managed_app = config.managed_watch_config.managed_app
 
         embed.add_field(
-            name = config.managed_watch_config.managed_app,
-            value = config.managed_watch_config.managed_app_reason,
+            name = managed_app,
+            value = f"{config.managed_watch_config.managed_app_reason} x{config.managed_watch_config.managed_quantity}",
             inline = True
         )
 
 
     return embed
 
 def fifth_percentile(eve_type: EveType, eve_region: EveRegion = EveRegion(None), buy_order: bool = False):
```

### Comparing `aa-market-manager-0.9.2a0/marketmanager/tasks.py` & `aa-market-manager-0.9.3a0/marketmanager/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,29 +432,30 @@
 
     if config.structure_type.count() > 0 :
         valid_structures = Structure.objects.filter(eve_type__in=config.structure_type.all())
         matching_orders_location = matching_orders_location.filter(location_id__in=valid_structures.all())
 
     # Comparators
     ## if price is not zero, filter out all orders that dont meet minimum
+    if config.price != 0:
+        comparator_price = config.price
+    else:
+        comparator_price = 0
+
     if config.jita_compare_percent != 0:
         try:
             type_statistics = TypeStatistics.objects.get(
                 eve_type = config.eve_type,
                 eve_region = EveRegion.objects.get(id=10000002))
+            if config.buy_order == True:
+                comparator_price = type_statistics.buy_weighted_average * config.jita_compare_percent
+            if config.buy_order == False:
+                comparator_price = type_statistics.sell_weighted_average * config.jita_compare_percent
         except ObjectDoesNotExist:
             comparator_price = 0
-        if config.buy_order == True:
-            comparator_price = type_statistics.buy_weighted_average * config.jita_compare_percent
-        if config.buy_order == False:
-            comparator_price = type_statistics.sell_weighted_average * config.jita_compare_percent
-    if config.price != 0:
-        comparator_price = config.price
-    else:
-        comparator_price = 0
 
     if comparator_price != 0 and config.buy_order == True:
         matching_orders_location_price = matching_orders_location.filter(price__gte=comparator_price)
     elif comparator_price != 0 and config.buy_order == False:
         matching_orders_location_price = matching_orders_location.filter(price__lte=comparator_price)
     else:
         matching_orders_location_price = matching_orders_location
```

### Comparing `aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/buy_orders.html` & `aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/buy_orders.html`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/item_details.html` & `aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/item_details.html`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/item_selector.html` & `aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/item_selector.html`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/region_selector.html` & `aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/region_selector.html`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser/sell_orders.html` & `aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser/sell_orders.html`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/templates/marketmanager/marketbrowser.html` & `aa-market-manager-0.9.3a0/marketmanager/templates/marketmanager/marketbrowser.html`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/tests/esi/utils.py` & `aa-market-manager-0.9.3a0/marketmanager/tests/esi/utils.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/tests/test_task_helpers.py` & `aa-market-manager-0.9.3a0/marketmanager/tests/test_task_helpers.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/tests/test_tasks.py` & `aa-market-manager-0.9.3a0/marketmanager/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/tests/testdata/create_eveuniverse.py` & `aa-market-manager-0.9.3a0/marketmanager/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/tests/testdata/eveuniverse.json` & `aa-market-manager-0.9.3a0/marketmanager/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/urls.py` & `aa-market-manager-0.9.3a0/marketmanager/urls.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/marketmanager/views.py` & `aa-market-manager-0.9.3a0/marketmanager/views.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/setup.py` & `aa-market-manager-0.9.3a0/setup.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/testauth/celery.py` & `aa-market-manager-0.9.3a0/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/testauth/settingsAA2.py` & `aa-market-manager-0.9.3a0/testauth/settingsAA2.py`

 * *Files identical despite different names*

### Comparing `aa-market-manager-0.9.2a0/testauth/settingsAA3.py` & `aa-market-manager-0.9.3a0/testauth/settingsAA3.py`

 * *Files identical despite different names*

