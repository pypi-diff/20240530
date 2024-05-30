# Comparing `tmp/upcloud_api-2.5.1.tar.gz` & `tmp/upcloud_api-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upcloud_api-2.5.1.tar", last modified: Tue Sep 19 08:15:29 2023, max compression
+gzip compressed data, was "upcloud_api-2.6.0.tar", last modified: Thu May 30 07:26:43 2024, max compression
```

## Comparing `upcloud_api-2.5.1.tar` & `upcloud_api-2.6.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:15:29.246591 upcloud_api-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-09-19 08:15:29.246591 upcloud_api-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:15:29.218591 upcloud_api-2.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/CloudManager.md
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/Firewall.md
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/IP-address-mixin.md
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/IP-address.md
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/Server.md
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/Storage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/host-mixin.md
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/network-mixin.md
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/object_storage-mixin.md
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/server-mixin.md
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/docs/storage-mixin.md
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-09-19 08:15:29.246591 upcloud_api-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      619 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:15:29.218591 upcloud_api-2.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:15:29.234591 upcloud_api-2.5.1/test/json_data/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/account.json
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/firewall_rule.json
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/firewall_rules.json
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/host.json
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/host_7653311107.json
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/https:__fi-hel1.img.upcloud.com_uploader_session_07a6c9a3-300e-4d0e-b935-624f3dbdff3f.json
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/ip_address.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/ip_address_10.1.0.101.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/ip_address_post.json
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/network.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/network_03000000-0000-4000-8001-000000000000.json
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/network_036df3d0-8629-4549-984e-dc86fc3fa1b0.json
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/network_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/object-storage.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/object-storage_0608edc4-d4a3-4b01-abe4-e147bd7ffe45.json
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/object-storage_06b0e4fc-d74b-455e-a373-60cd6ca84022.json
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/object-storage_06b0e4fc-d74b-455e-a373-60cd6ca84022_stats_network.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/object-storage_post.json
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/plan.json
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/price.json
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/router.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/router_03b34bc2-5adf-4fc4-8c44-83f869058f5a.json
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/router_04da7f97-dc03-4df0-868f-239f304ba72f.json
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/router_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server-group_0b5169fc-23aa-4ba7-aaab-f38868ce99cd.json
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server-group_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server.json
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531_cdrom_eject_post.json
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531_cdrom_load_post.json
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server_0082c083-9847-4f9f-ae04-811251309b35_networking.json
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server_0082c083-9847-4f9f-ae04-811251309b35_networking_interface_7.json
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server_0082c083-9847-4f9f-ae04-811251309b35_networking_interface_post.json
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server_009d64ef-31d1-4684-a26b-c86c955cbf46.json
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/server_create.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_01350eec-6ebf-4418-abe4-e8bb1d5c9643.json
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e.json
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_backup_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_clone_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_import.json
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_import_cancel_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_import_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_templatize_post.json
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_attach.json
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_detach.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_post.json
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_public.json
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/storage_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/tag.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/tag_TheTestTag.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/test_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/timezone.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/json_data/zone.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_cloud_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_ip_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_object_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_server_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_server_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8711 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/test/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:15:29.242591 upcloud_api-2.5.1/upcloud_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:15:29.246591 upcloud_api-2.5.1/upcloud_api/cloud_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/firewall_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/host_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/ip_address_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/lb_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/network_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/object_storage_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/server_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/storage_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/cloud_manager/tag_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/ip_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    22596 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/server_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/storage_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/upcloud_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-09-19 08:15:18.000000 upcloud_api-2.5.1/upcloud_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:15:29.242591 upcloud_api-2.5.1/upcloud_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-09-19 08:15:29.000000 upcloud_api-2.5.1/upcloud_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2023-09-19 08:15:29.000000 upcloud_api-2.5.1/upcloud_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 08:15:29.000000 upcloud_api-2.5.1/upcloud_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-19 08:15:29.000000 upcloud_api-2.5.1/upcloud_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-19 08:15:29.000000 upcloud_api-2.5.1/upcloud_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:26:43.031641 upcloud_api-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-30 07:26:43.031641 upcloud_api-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:26:43.015641 upcloud_api-2.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/CloudManager.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/Firewall.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/IP-address-mixin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/IP-address.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/Server.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/Storage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/host-mixin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/network-mixin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/object_storage-mixin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/server-mixin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/docs/storage-mixin.md
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-30 07:26:43.031641 upcloud_api-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:26:43.015641 upcloud_api-2.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:26:43.023641 upcloud_api-2.6.0/test/json_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/account.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/firewall_rule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/firewall_rules.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/host.json
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/host_7653311107.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/https:__fi-hel1.img.upcloud.com_uploader_session_07a6c9a3-300e-4d0e-b935-624f3dbdff3f.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/ip_address.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/ip_address_10.1.0.101.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/ip_address_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/network.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/network_03000000-0000-4000-8001-000000000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/network_036df3d0-8629-4549-984e-dc86fc3fa1b0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/network_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/object-storage.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/object-storage_0608edc4-d4a3-4b01-abe4-e147bd7ffe45.json
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/object-storage_06b0e4fc-d74b-455e-a373-60cd6ca84022.json
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/object-storage_06b0e4fc-d74b-455e-a373-60cd6ca84022_stats_network.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/object-storage_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/plan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/price.json
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/router.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/router_03b34bc2-5adf-4fc4-8c44-83f869058f5a.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/router_04da7f97-dc03-4df0-868f-239f304ba72f.json
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/router_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server-group_0b5169fc-23aa-4ba7-aaab-f38868ce99cd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server-group_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531_cdrom_eject_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531_cdrom_load_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server_0082c083-9847-4f9f-ae04-811251309b35_networking.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server_0082c083-9847-4f9f-ae04-811251309b35_networking_interface_7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server_0082c083-9847-4f9f-ae04-811251309b35_networking_interface_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server_009d64ef-31d1-4684-a26b-c86c955cbf46.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/server_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_01350eec-6ebf-4418-abe4-e8bb1d5c9643.json
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e.json
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_backup_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_clone_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_import.json
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_import_cancel_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_import_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_templatize_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_attach.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_detach.json
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_public.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/storage_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/tag.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/tag_TheTestTag.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/test_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/timezone.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/json_data/zone.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_cloud_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_ip_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_server_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_server_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/test/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:26:43.027641 upcloud_api-2.6.0/upcloud_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:26:43.031641 upcloud_api-2.6.0/upcloud_api/cloud_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/firewall_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/host_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/ip_address_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/lb_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/network_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/object_storage_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/server_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/storage_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/cloud_manager/tag_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/ip_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22596 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/server_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/storage_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/upcloud_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-30 07:26:34.000000 upcloud_api-2.6.0/upcloud_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:26:43.031641 upcloud_api-2.6.0/upcloud_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-30 07:26:42.000000 upcloud_api-2.6.0/upcloud_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-30 07:26:43.000000 upcloud_api-2.6.0/upcloud_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:26:42.000000 upcloud_api-2.6.0/upcloud_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 07:26:42.000000 upcloud_api-2.6.0/upcloud_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 07:26:42.000000 upcloud_api-2.6.0/upcloud_api.egg-info/top_level.txt
```

### Comparing `upcloud_api-2.5.1/LICENSE.txt` & `upcloud_api-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/PKG-INFO` & `upcloud_api-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: upcloud_api
-Version: 2.5.1
+Version: 2.6.0
 Summary: UpCloud API Client
 Home-page: https://github.com/UpCloudLtd/upcloud-python-api
 Maintainer: UpCloud
 Maintainer-email: hello@upcloud.com
 License: MIT
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 
 # UpCloud's Python API Client
 
 [![test](https://github.com/UpCloudLtd/upcloud-python-api/actions/workflows/main.yml/badge.svg)](https://github.com/UpCloudLtd/upcloud-python-api/actions/workflows/main.yml)
@@ -31,19 +31,21 @@
 
 Alternatively, if you want the newest (possibly not yet released) stuff, clone the project and run:
 
 ``` bash
 python setup.py install
 ```
 
-### Supported Python versions in API v2.5.1
+### Supported Python versions in API v2.6.0
 
-- Python 3.7
 - Python 3.8
 - Python 3.9
+- Python 3.10
+- Python 3.11
+- Python 3.12
 - PyPy3
 
 **Python 2 has been deprecated**
 
 - Python 2.7 is no longer supported, but available in older API versions (< v2.0.0).
 
 ## Changelog
```

### Comparing `upcloud_api-2.5.1/README.md` & `upcloud_api-2.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 
 Alternatively, if you want the newest (possibly not yet released) stuff, clone the project and run:
 
 ``` bash
 python setup.py install
 ```
 
-### Supported Python versions in API v2.5.1
+### Supported Python versions in API v2.6.0
 
-- Python 3.7
 - Python 3.8
 - Python 3.9
+- Python 3.10
+- Python 3.11
+- Python 3.12
 - PyPy3
 
 **Python 2 has been deprecated**
 
 - Python 2.7 is no longer supported, but available in older API versions (< v2.0.0).
 
 ## Changelog
```

### Comparing `upcloud_api-2.5.1/docs/CloudManager.md` & `upcloud_api-2.6.0/docs/CloudManager.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/Firewall.md` & `upcloud_api-2.6.0/docs/Firewall.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/IP-address-mixin.md` & `upcloud_api-2.6.0/docs/IP-address-mixin.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/IP-address.md` & `upcloud_api-2.6.0/docs/IP-address.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/Server.md` & `upcloud_api-2.6.0/docs/Server.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/Storage.md` & `upcloud_api-2.6.0/docs/Storage.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 
 ```python
 
 storage1 = manager.create_storage(
     zone='fi-hel1',
     size=10,
     tier="maxiops",
-    title="my storage disk"
+    title="my storage disk",
+    encrypted=False
 )
 
 storage2 = manager.create_storage(zone='de-fra1', size=100)
 
 ```
```

### Comparing `upcloud_api-2.5.1/docs/host-mixin.md` & `upcloud_api-2.6.0/docs/host-mixin.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/index.md` & `upcloud_api-2.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/network-mixin.md` & `upcloud_api-2.6.0/docs/network-mixin.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/object_storage-mixin.md` & `upcloud_api-2.6.0/docs/object_storage-mixin.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/server-mixin.md` & `upcloud_api-2.6.0/docs/server-mixin.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/docs/storage-mixin.md` & `upcloud_api-2.6.0/docs/storage-mixin.md`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/pyproject.toml` & `upcloud_api-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.black]
 line-length = 99
-target-version = ['py37']
+target-version = ['py38']
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 exclude = [
     ".git",
     "ENV",
     "__pycache__",
     "build",
 ]
 ignore = [
```

### Comparing `upcloud_api-2.5.1/requirements-dev.txt` & `upcloud_api-2.6.0/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     # via requests
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via pip-tools
 coverage[toml]==7.2.7
     # via pytest-cov
-exceptiongroup==1.1.2
+exceptiongroup==1.2.1
     # via pytest
-idna==3.4
+idna==3.7
     # via requests
 iniconfig==2.0.0
     # via pytest
 mock==5.1.0
     # via -r requirements-dev.in
 packaging==23.1
     # via
@@ -36,28 +36,28 @@
     # via
     #   -r requirements-dev.in
     #   pytest-cov
 pytest-cov==4.1.0
     # via -r requirements-dev.in
 pyyaml==6.0.1
     # via responses
-requests==2.31.0
+requests==2.32.2
     # via responses
 responses==0.23.2
     # via -r requirements-dev.in
 tomli==2.0.1
     # via
     #   build
     #   coverage
     #   pip-tools
     #   pyproject-hooks
     #   pytest
 types-pyyaml==6.0.12.11
     # via responses
-urllib3==2.0.4
+urllib3==2.0.7
     # via
     #   requests
     #   responses
 wheel==0.41.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `upcloud_api-2.5.1/setup.cfg` & `upcloud_api-2.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 maintainer = UpCloud
 maintainer_email = hello@upcloud.com
 url = https://github.com/UpCloudLtd/upcloud-python-api
 packages = ['upcloud_api', 'upcloud_api.cloud_manager']
 license = MIT
 
 [options]
-python_requires = >=3.7, <4
+python_requires = >=3.8, <4
 setup_requires = 
 	setuptools
 install_requires = 
 	requests
 packages = 
 	upcloud_api
 	upcloud_api.cloud_manager
```

### Comparing `upcloud_api-2.5.1/setup.py` & `upcloud_api-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/conftest.py` & `upcloud_api-2.6.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/firewall_rules.json` & `upcloud_api-2.6.0/test/json_data/firewall_rules.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/host.json` & `upcloud_api-2.6.0/test/json_data/host.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/ip_address.json` & `upcloud_api-2.6.0/test/json_data/ip_address.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/network.json` & `upcloud_api-2.6.0/test/json_data/network.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/network_036df3d0-8629-4549-984e-dc86fc3fa1b0.json` & `upcloud_api-2.6.0/test/json_data/network_036df3d0-8629-4549-984e-dc86fc3fa1b0.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/network_post.json` & `upcloud_api-2.6.0/test/json_data/network_post.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/object-storage.json` & `upcloud_api-2.6.0/test/json_data/object-storage.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/plan.json` & `upcloud_api-2.6.0/test/json_data/plan.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/price.json` & `upcloud_api-2.6.0/test/json_data/price.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/router.json` & `upcloud_api-2.6.0/test/json_data/router.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/server-group_0b5169fc-23aa-4ba7-aaab-f38868ce99cd.json` & `upcloud_api-2.6.0/test/json_data/server-group_0b5169fc-23aa-4ba7-aaab-f38868ce99cd.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/server.json` & `upcloud_api-2.6.0/test/json_data/server.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531.json` & `upcloud_api-2.6.0/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531_cdrom_eject_post.json` & `upcloud_api-2.6.0/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531_cdrom_eject_post.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531_cdrom_load_post.json` & `upcloud_api-2.6.0/test/json_data/server_00798b85-efdc-41ca-8021-f6ef457b8531_cdrom_load_post.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/server_0082c083-9847-4f9f-ae04-811251309b35_networking.json` & `upcloud_api-2.6.0/test/json_data/server_0082c083-9847-4f9f-ae04-811251309b35_networking.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/server_009d64ef-31d1-4684-a26b-c86c955cbf46.json` & `upcloud_api-2.6.0/test/json_data/server_009d64ef-31d1-4684-a26b-c86c955cbf46.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/server_create.json` & `upcloud_api-2.6.0/test/json_data/server_create.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/storage_01350eec-6ebf-4418-abe4-e8bb1d5c9643.json` & `upcloud_api-2.6.0/test/json_data/storage_01350eec-6ebf-4418-abe4-e8bb1d5c9643.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e.json` & `upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'storage'": "{'encrypted': 'yes'}"}*

```diff
@@ -1,14 +1,15 @@
 {
     "storage": {
         "access": "private",
         "backup_rule": "",
         "backups": {
             "backup": []
         },
+        "encrypted": "yes",
         "labels": [
             {
                 "key": "role",
                 "value": "primary"
             }
         ],
         "license": 0,
```

### Comparing `upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_backup_post.json` & `upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_backup_post.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_clone_post.json` & `upcloud_api-2.6.0/test/json_data/storage_01d4fcd4-e446-433b-8a9c-551a1284952e_clone_post.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/storage_attach.json` & `upcloud_api-2.6.0/test/json_data/storage_attach.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/storage_detach.json` & `upcloud_api-2.6.0/test/json_data/storage_detach.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/storage_post.json` & `upcloud_api-2.6.0/test/json_data/storage_post.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'storage'": "{'encrypted': 'yes'}"}*

```diff
@@ -1,14 +1,15 @@
 {
     "storage": {
         "access": "private",
         "backup_rule": {},
         "backups": {
             "backup": []
         },
+        "encrypted": "yes",
         "labels": [
             {
                 "key": "role",
                 "value": "primary"
             }
         ],
         "license": 0,
```

### Comparing `upcloud_api-2.5.1/test/json_data/storage_public.json` & `upcloud_api-2.6.0/test/json_data/storage_public.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/storage_template.json` & `upcloud_api-2.6.0/test/json_data/storage_template.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/tag.json` & `upcloud_api-2.6.0/test/json_data/tag.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/json_data/timezone.json` & `upcloud_api-2.6.0/test/json_data/timezone.json`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_cloud_manager.py` & `upcloud_api-2.6.0/test/test_cloud_manager.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_firewall.py` & `upcloud_api-2.6.0/test/test_firewall.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_host.py` & `upcloud_api-2.6.0/test/test_host.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_ip_manager.py` & `upcloud_api-2.6.0/test/test_ip_manager.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_network.py` & `upcloud_api-2.6.0/test/test_network.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_object_storage.py` & `upcloud_api-2.6.0/test/test_object_storage.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_server.py` & `upcloud_api-2.6.0/test/test_server.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_server_creation.py` & `upcloud_api-2.6.0/test/test_server_creation.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_server_group.py` & `upcloud_api-2.6.0/test/test_server_group.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/test/test_storage.py` & `upcloud_api-2.6.0/test/test_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,30 +27,32 @@
         for template in templates:
             assert type(template) is dict
 
     @responses.activate
     def test_storage_create(self, manager):
         Mock.mock_post("storage")
         storage = manager.create_storage(
-            zone="fi-hel1", size=666, tier="maxiops", title="My data collection"
+            zone="fi-hel1", encrypted=True, size=666, tier="maxiops", title="My data collection"
         )
         assert type(storage).__name__ == "Storage"
+        assert storage.encrypted
         assert storage.size == 666
         assert storage.tier == "maxiops"
         assert storage.title == "My data collection"
         assert storage.zone == "fi-hel1"
 
     @responses.activate
     def test_clone_storage(self, manager):
         data = Mock.mock_get("storage/01d4fcd4-e446-433b-8a9c-551a1284952e")
         storage = manager.get_storage("01d4fcd4-e446-433b-8a9c-551a1284952e")
 
         Mock.mock_post("storage/01d4fcd4-e446-433b-8a9c-551a1284952e/clone")
         cloned_storage = storage.clone('cloned-storage-test', 'fi-hel1')
         assert type(cloned_storage).__name__ == "Storage"
+        assert not cloned_storage.encrypted
         assert cloned_storage.size == 666
         assert cloned_storage.tier == "maxiops"
         assert cloned_storage.title == "cloned-storage-test"
         assert cloned_storage.zone == "fi-hel1"
 
     @responses.activate
     def test_cancel_clone_storage(self, manager):
```

### Comparing `upcloud_api-2.5.1/test/test_tags.py` & `upcloud_api-2.6.0/test/test_tags.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/tox.ini` & `upcloud_api-2.6.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = py37, py38, py39, py310, pypy3
+envlist = py38, py39, py310, py311, py312, pypy3
 skip_missing_interpreters = True
 
 [testenv]
 commands = py.test --cov=test --cov={envsitepackagesdir}/upcloud_api --cov-report term-missing test/
 deps = -rrequirements-dev.txt
 
 [testenv:integration]
```

### Comparing `upcloud_api-2.5.1/upcloud_api/__init__.py` & `upcloud_api-2.6.0/upcloud_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Python Interface to UpCloud's API.
 """
 
-__version__ = '2.5.1'
+__version__ = '2.6.0'
 __author__ = 'Developers from UpCloud & elsewhere'
 __author_email__ = 'hello@upcloud.com'
 __maintainer__ = 'UpCloud'
 __maintainer_email__ = 'hello@upcloud.com'
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) 2015- UpCloud'
```

### Comparing `upcloud_api-2.5.1/upcloud_api/api.py` & `upcloud_api-2.6.0/upcloud_api/api.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/__init__.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/firewall_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/firewall_mixin.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/host_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/host_mixin.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/ip_address_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/ip_address_mixin.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/lb_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/lb_mixin.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/network_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/network_mixin.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/object_storage_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/object_storage_mixin.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/server_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/server_mixin.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/storage_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/storage_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,29 +41,34 @@
 
     def create_storage(
         self,
         zone: str,
         size: int = 10,
         tier: str = 'maxiops',
         title: str = 'Storage disk',
+        encrypted: bool = False,
         *,
         backup_rule: Optional[dict] = None,
     ) -> Storage:
         """
         Create a Storage object. Returns an object based on the API's response.
         """
         if backup_rule is None:
             backup_rule = {}
+
+        encrypted_str = 'yes' if encrypted else 'no'
+
         body = {
             'storage': {
                 'size': size,
                 'tier': tier,
                 'title': title,
                 'zone': zone,
                 'backup_rule': backup_rule,
+                'encrypted': encrypted_str,
             }
         }
         res = self.api.post_request('/storage', body)
         return Storage(cloud_manager=self, **res['storage'])
 
     def _modify_storage(self, storage, size, title, backup_rule: Optional[dict] = None):
         body = {'storage': {}}
```

### Comparing `upcloud_api-2.5.1/upcloud_api/cloud_manager/tag_mixin.py` & `upcloud_api-2.6.0/upcloud_api/cloud_manager/tag_mixin.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/errors.py` & `upcloud_api-2.6.0/upcloud_api/errors.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/firewall.py` & `upcloud_api-2.6.0/upcloud_api/firewall.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/ip_address.py` & `upcloud_api-2.6.0/upcloud_api/ip_address.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/label.py` & `upcloud_api-2.6.0/upcloud_api/label.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/load_balancer.py` & `upcloud_api-2.6.0/upcloud_api/load_balancer.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/server.py` & `upcloud_api-2.6.0/upcloud_api/server.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/server_group.py` & `upcloud_api-2.6.0/upcloud_api/server_group.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/storage.py` & `upcloud_api-2.6.0/upcloud_api/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     """
     Class representation of UpCloud Storage instance.
     """
 
     ATTRIBUTES = {
         'access': None,
         'address': None,
+        'encrypted': None,
         'labels': None,
         'license': None,
         'state': None,
         'size': 10,
         'tier': 'maxiops',
         'title': '',
         'type': None,
@@ -51,20 +52,34 @@
             self.title = kwargs['storage_title']
 
         if 'size' in kwargs:
             self.size = kwargs['size']
         elif 'storage_size' in kwargs:
             self.size = kwargs['storage_size']
 
+        if kwargs.get('encrypted') == 'yes':
+            self.encrypted = True
+        else:
+            self.encrypted = False
+
         # send the rest to super._reset
 
         filtered_kwargs = {
             key: val
             for key, val in kwargs.items()
-            if key not in ['uuid', 'storage', 'title', 'storage_title', 'size', 'storage_size']
+            if key
+            not in [
+                'uuid',
+                'storage',
+                'title',
+                'storage_title',
+                'size',
+                'storage_size',
+                'encrypted',
+            ]
         }
         super()._reset(**filtered_kwargs)
 
     def destroy(self) -> None:
         """
         Destroy the storage via the API.
         """
@@ -149,14 +164,17 @@
 
         if hasattr(self, 'labels'):
             dict_labels = []
             for label in self.labels:
                 dict_labels.append(label.to_dict())
             body['labels'] = dict_labels
 
+        if hasattr(self, 'encrypted') and isinstance(self.encrypted, bool):
+            body['encrypted'] = "yes" if self.encrypted else "no"
+
         return body
 
     @staticmethod
     def _create_storage_objs(storages, cloud_manager):
         # storages might be provided as a flat array or as a following dict:
         # {'storage_devices': {'storage_device': [...]}} || {'storage_device': [...]}
```

### Comparing `upcloud_api-2.5.1/upcloud_api/storage_import.py` & `upcloud_api-2.6.0/upcloud_api/storage_import.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/tag.py` & `upcloud_api-2.6.0/upcloud_api/tag.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/upcloud_resource.py` & `upcloud_api-2.6.0/upcloud_api/upcloud_resource.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api/utils.py` & `upcloud_api-2.6.0/upcloud_api/utils.py`

 * *Files identical despite different names*

### Comparing `upcloud_api-2.5.1/upcloud_api.egg-info/PKG-INFO` & `upcloud_api-2.6.0/upcloud_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: upcloud-api
-Version: 2.5.1
+Name: upcloud_api
+Version: 2.6.0
 Summary: UpCloud API Client
 Home-page: https://github.com/UpCloudLtd/upcloud-python-api
 Maintainer: UpCloud
 Maintainer-email: hello@upcloud.com
 License: MIT
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 
 # UpCloud's Python API Client
 
 [![test](https://github.com/UpCloudLtd/upcloud-python-api/actions/workflows/main.yml/badge.svg)](https://github.com/UpCloudLtd/upcloud-python-api/actions/workflows/main.yml)
@@ -31,19 +31,21 @@
 
 Alternatively, if you want the newest (possibly not yet released) stuff, clone the project and run:
 
 ``` bash
 python setup.py install
 ```
 
-### Supported Python versions in API v2.5.1
+### Supported Python versions in API v2.6.0
 
-- Python 3.7
 - Python 3.8
 - Python 3.9
+- Python 3.10
+- Python 3.11
+- Python 3.12
 - PyPy3
 
 **Python 2 has been deprecated**
 
 - Python 2.7 is no longer supported, but available in older API versions (< v2.0.0).
 
 ## Changelog
```

### Comparing `upcloud_api-2.5.1/upcloud_api.egg-info/SOURCES.txt` & `upcloud_api-2.6.0/upcloud_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

