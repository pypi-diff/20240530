# Comparing `tmp/pulumi_proxmoxve-6.8.0.tar.gz` & `tmp/pulumi_proxmoxve-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-6.8.0.tar", last modified: Tue May 28 09:20:39 2024, max compression
+gzip compressed data, was "pulumi_proxmoxve-6.8.1.tar", last modified: Thu May 30 07:12:03 2024, max compression
```

## Comparing `pulumi_proxmoxve-6.8.0.tar` & `pulumi_proxmoxve-6.8.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33026 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37116 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64491 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    32310 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.659774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/download/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38006 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/download/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/get_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/get_vm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.659774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/ha_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.659774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/get_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.659774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/get_pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/get_usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.663775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    32979 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24800 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/network_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/network_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25525 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/user/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16708 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/user/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90275 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    77594 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   123851 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    25922 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.267578 pulumi_proxmoxve-6.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-30 07:12:03.267578 pulumi_proxmoxve-6.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.255578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33026 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.255578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.255578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.255578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37116 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64491 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32310 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.255578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38006 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/get_vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.259578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/get_ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/get_ha_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/get_ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/get_ha_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/ha_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.259578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/get_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.259578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/get_pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/get_usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.263578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32979 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24800 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/network_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/network_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.263578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25525 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.267578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.267578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16708 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/user/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.267578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90345 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77654 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123851 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25922 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:12:03.255578 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:12:03.267578 pulumi_proxmoxve-6.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-30 07:12:03.000000 pulumi_proxmoxve-6.8.1/setup.py
```

### Comparing `pulumi_proxmoxve-6.8.0/PKG-INFO` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_proxmoxve
-Version: 6.8.0
+Name: pulumi-proxmoxve
+Version: 6.8.1
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.8.0/README.md` & `pulumi_proxmoxve-6.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/acl.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/_inputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/options.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/cluster/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/download/file.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/download/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/get_node.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/get_vm2.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/get_vm2.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_group.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/get_ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_groups.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/get_ha_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_resource.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/get_ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_resources.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/get_ha_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/ha_group.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/ha_resource.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/ha/ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/__init__.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/get_mappings.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/get_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/_inputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/get_pci.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/get_pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/get_usb.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/get_usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/pci.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/usb.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/mapping/usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hardware/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/__init__.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_dns.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_hosts.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_time.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_version.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/network_bridge.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/network_bridge.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/network_vlan.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/network_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/user/token.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/user/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2289,40 +2289,41 @@
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
 @pulumi.input_type
 class VirtualMachineUsbArgs:
     def __init__(__self__, *,
-                 host: pulumi.Input[str],
+                 host: Optional[pulumi.Input[str]] = None,
                  mapping: Optional[pulumi.Input[str]] = None,
                  usb3: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] host: The USB device ID. Use either this or `mapping`.
         :param pulumi.Input[str] mapping: The resource mapping name of the device, for
                example usbdevice. Use either this or `id`.
         :param pulumi.Input[bool] usb3: Makes the USB device a USB3 device for the VM
                (defaults to `false`).
         """
-        pulumi.set(__self__, "host", host)
+        if host is not None:
+            pulumi.set(__self__, "host", host)
         if mapping is not None:
             pulumi.set(__self__, "mapping", mapping)
         if usb3 is not None:
             pulumi.set(__self__, "usb3", usb3)
 
     @property
     @pulumi.getter
-    def host(self) -> pulumi.Input[str]:
+    def host(self) -> Optional[pulumi.Input[str]]:
         """
         The USB device ID. Use either this or `mapping`.
         """
         return pulumi.get(self, "host")
 
     @host.setter
-    def host(self, value: pulumi.Input[str]):
+    def host(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host", value)
 
     @property
     @pulumi.getter
     def mapping(self) -> Optional[pulumi.Input[str]]:
         """
         The resource mapping name of the device, for
```

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2046,33 +2046,34 @@
         """
         return pulumi.get(self, "version")
 
 
 @pulumi.output_type
 class VirtualMachineUsb(dict):
     def __init__(__self__, *,
-                 host: str,
+                 host: Optional[str] = None,
                  mapping: Optional[str] = None,
                  usb3: Optional[bool] = None):
         """
         :param str host: The USB device ID. Use either this or `mapping`.
         :param str mapping: The resource mapping name of the device, for
                example usbdevice. Use either this or `id`.
         :param bool usb3: Makes the USB device a USB3 device for the VM
                (defaults to `false`).
         """
-        pulumi.set(__self__, "host", host)
+        if host is not None:
+            pulumi.set(__self__, "host", host)
         if mapping is not None:
             pulumi.set(__self__, "mapping", mapping)
         if usb3 is not None:
             pulumi.set(__self__, "usb3", usb3)
 
     @property
     @pulumi.getter
-    def host(self) -> str:
+    def host(self) -> Optional[str]:
         """
         The USB device ID. Use either this or `mapping`.
         """
         return pulumi.get(self, "host")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm2.py` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve/vm2.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-proxmoxve
-Version: 6.8.0
+Name: pulumi_proxmoxve
+Version: 6.8.1
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-6.8.1/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.8.0/setup.py` & `pulumi_proxmoxve-6.8.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.8.0"
+VERSION = "6.8.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
```

