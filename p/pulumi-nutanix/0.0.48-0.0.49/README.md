# Comparing `tmp/pulumi_nutanix-0.0.48.tar.gz` & `tmp/pulumi_nutanix-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_nutanix-0.0.48.tar", last modified: Wed May 29 08:28:28 2024, max compression
+gzip compressed data, was "pulumi_nutanix-0.0.49.tar", last modified: Thu May 30 13:33:18 2024, max compression
```

## Comparing `pulumi_nutanix-0.0.48.tar` & `pulumi_nutanix-0.0.49.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:28.028052 pulumi_nutanix-0.0.48/pulumi_nutanix/
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1544197 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    28160 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/access_control_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/address_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/category_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/category_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/pulumi_nutanix/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    22943 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_central_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    43114 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_central_image_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    14716 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    82103 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_image_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_ipmi_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_access_control_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_access_control_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_address_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_address_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_assert_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_category_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_floating_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_cluster_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_clusters_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_node_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_nodes_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_list_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_discover_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_hypervisor_isos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_node_network_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_nos_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster_kube_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_private_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_private_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clones.py
--rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_dbserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_dbservers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_maintenance_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_network_available_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_sla.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_slas.py
--rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_time_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_time_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tms_capability.py
--rw-r--r--   0 runner    (1001) docker     (127)    38429 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_network_security_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_pbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_pbrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24933 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_protection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_protection_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_recovery_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_recovery_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_service_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_static_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_subnets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    33940 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_vpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42511 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    52706 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    19115 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_private_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18915 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_worker_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_authorize_dbserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    92262 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_clone_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    47795 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    98121 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    46080 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)    47875 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    57356 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    60370 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_dbserver_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_linked_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_log_catchups.py
--rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_maintenance_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    34180 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    28661 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    90606 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_register_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    56422 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_register_dbserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    47875 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_scale_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    29991 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_sla.py
--rw-r--r--   0 runner    (1001) docker     (127)    31118 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_software_version_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_stretched_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    22819 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_tms_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)   106914 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/network_security_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)  2714710 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30289 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/pbr.py
--rw-r--r--   0 runner    (1001) docker     (127)    67188 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    26646 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/protection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18624 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/recovery_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22461 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/service_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18834 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/static_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    60420 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    29328 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    21199 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)   128659 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    27270 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:33:18.087655 pulumi_nutanix-0.0.49/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-30 13:33:18.087655 pulumi_nutanix-0.0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:33:18.087655 pulumi_nutanix-0.0.49/pulumi_nutanix/
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1544197 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28160 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/access_control_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/address_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/category_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/category_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:33:18.087655 pulumi_nutanix-0.0.49/pulumi_nutanix/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22943 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_central_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43114 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_central_image_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14716 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82103 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_image_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_ipmi_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_access_control_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_access_control_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_address_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_address_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_assert_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_category_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_floating_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_cluster_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_imaged_clusters_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_imaged_node_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_imaged_nodes_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_list_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_discover_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_hypervisor_isos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_node_network_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_nos_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_cluster_kube_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_cluster_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_private_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_private_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_clones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_dbserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_dbservers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_maintenance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_network_available_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_sla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_slas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_time_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_time_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_tms_capability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38429 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_network_security_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_pbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_pbrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24933 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_protection_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_protection_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_recovery_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_recovery_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_service_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_static_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33940 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/get_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42511 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52706 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/karbon_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19115 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/karbon_private_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18915 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/karbon_worker_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_authorize_dbserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92262 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_clone_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47795 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98121 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46080 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_database_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47875 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_database_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57356 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_database_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60370 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_dbserver_vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_linked_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_log_catchups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_maintenance_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34180 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28661 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90606 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_register_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56422 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_register_dbserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47875 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_scale_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29991 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_sla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31118 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_software_version_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_stretched_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22819 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_tms_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106914 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/network_security_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2714710 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30289 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/pbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67188 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26646 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/protection_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18624 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/recovery_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22461 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/service_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18834 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/static_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60420 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29328 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21199 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128659 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27270 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/pulumi_nutanix/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:33:18.087655 pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-30 13:33:18.000000 pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-30 13:33:18.000000 pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:33:18.000000 pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:33:18.000000 pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 13:33:18.000000 pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 13:33:18.000000 pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:33:18.087655 pulumi_nutanix-0.0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-30 13:33:17.000000 pulumi_nutanix-0.0.49/setup.py
```

### Comparing `pulumi_nutanix-0.0.48/PKG-INFO` & `pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: pulumi_nutanix
-Version: 0.0.48
-Summary: A Pulumi package for creating and managing nutanix cloud resources.
+Name: pulumi-nutanix
+Version: 0.0.49
+Summary: A Pulumi package for creating and managing Nutanix cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-nutanix
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-nutanix
 Keywords: pulumi nutanix category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_nutanix-0.0.48/README.md` & `pulumi_nutanix-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/__init__.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/_inputs.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/_utilities.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/access_control_policy.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/access_control_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/address_group.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/address_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/category_key.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/category_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/category_value.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/category_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/config/vars.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/floating_ip.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_central_api_keys.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_central_api_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_central_image_cluster.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_central_image_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_image.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_image_nodes.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_image_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_ipmi_config.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/foundation_ipmi_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_access_control_policies.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_access_control_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_access_control_policy.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_access_control_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_address_group.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_address_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_address_groups.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_address_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_assert_helper.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_assert_helper.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_category_key.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_category_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_cluster.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_clusters.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_floating_ip.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_floating_ips.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_floating_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_api_keys.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_api_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_cluster_details.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_cluster_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_clusters_list.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_imaged_clusters_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_node_details.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_imaged_node_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_nodes_list.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_imaged_nodes_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_list_api_keys.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_central_list_api_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_discover_nodes.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_discover_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_hypervisor_isos.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_hypervisor_isos.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_node_network_details.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_node_network_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_nos_packages.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_foundation_nos_packages.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_host.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_hosts.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_image.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster_kube_config.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_cluster_kube_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster_ssh.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_cluster_ssh.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_clusters.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_private_registries.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_private_registries.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_private_registry.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_karbon_private_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clone.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_clone.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clones.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_clones.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_cluster.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clusters.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_database.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_databases.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_dbserver.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_dbserver.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_dbservers.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_dbservers.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_maintenance_window.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_maintenance_windows.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_maintenance_windows.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_network.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_network_available_ips.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_network_available_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_networks.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_profile.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_profiles.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_sla.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_sla.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_slas.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_slas.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_snapshot.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_snapshots.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_snapshots.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tag.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tags.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_time_machine.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_time_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_time_machines.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_time_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tms_capability.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_ndb_tms_capability.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_network_security_rule.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_network_security_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_pbr.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_pbr.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_pbrs.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_pbrs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_permission.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_permissions.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_project.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_projects.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_protection_rule.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_protection_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_protection_rules.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_protection_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_recovery_plan.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_recovery_plan.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_recovery_plans.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_recovery_plans.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_role.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_roles.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_service_group.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_service_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_service_groups.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_service_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_static_routes.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_static_routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_subnet.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_subnets.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_subnets.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_user.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_user_group.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_user_groups.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_users.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_virtual_machine.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_vpc.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/get_vpcs.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/get_vpcs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/image.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_cluster.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/karbon_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_private_registry.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/karbon_private_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_worker_nodepool.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/karbon_worker_nodepool.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_authorize_dbserver.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_authorize_dbserver.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_clone.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_clone.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_clone_refresh.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_clone_refresh.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_cluster.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_restore.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_database_restore.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_scale.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_database_scale.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_snapshot.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_database_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_dbserver_vm.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_dbserver_vm.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_linked_databases.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_linked_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_log_catchups.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_log_catchups.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_maintenance_task.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_maintenance_task.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_maintenance_window.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_network.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_profile.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_register_database.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_register_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_register_dbserver.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_register_dbserver.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_scale_database.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_scale_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_sla.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_sla.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_software_version_profile.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_software_version_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_stretched_vlan.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_stretched_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_tag.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_tms_cluster.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/ndb_tms_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/network_security_rule.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/network_security_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/outputs.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/pbr.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/pbr.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/project.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/protection_rule.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/protection_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/provider.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/recovery_plan.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/recovery_plan.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/role.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/service_group.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/service_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/static_routes.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/static_routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/subnet.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/user.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/user_groups.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/virtual_machine.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix/vpc.py` & `pulumi_nutanix-0.0.49/pulumi_nutanix/vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/PKG-INFO` & `pulumi_nutanix-0.0.49/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: pulumi-nutanix
-Version: 0.0.48
-Summary: A Pulumi package for creating and managing nutanix cloud resources.
+Name: pulumi_nutanix
+Version: 0.0.49
+Summary: A Pulumi package for creating and managing Nutanix cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-nutanix
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-nutanix
 Keywords: pulumi nutanix category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/SOURCES.txt` & `pulumi_nutanix-0.0.49/pulumi_nutanix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.48/setup.py` & `pulumi_nutanix-0.0.49/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.48"
+VERSION = "0.0.49"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "nutanix Pulumi Package - Development Version"
 
 
 setup(name='pulumi_nutanix',
       python_requires='>=3.8',
       version=VERSION,
-      description="A Pulumi package for creating and managing nutanix cloud resources.",
+      description="A Pulumi package for creating and managing Nutanix cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       keywords='pulumi nutanix category/cloud',
       url='https://github.com/pierskarsenbarg/pulumi-nutanix',
       project_urls={
           'Repository': 'https://github.com/pierskarsenbarg/pulumi-nutanix'
       },
```

