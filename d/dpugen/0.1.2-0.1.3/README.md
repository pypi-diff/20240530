# Comparing `tmp/dpugen-0.1.2.tar.gz` & `tmp/dpugen-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpugen-0.1.2.tar", last modified: Tue Oct 10 20:34:56 2023, max compression
+gzip compressed data, was "dpugen-0.1.3.tar", last modified: Thu May 30 15:54:24 2024, max compression
```

## Comparing `dpugen-0.1.2.tar` & `dpugen-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 20:34:56.650777 dpugen-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-10-10 20:34:42.000000 dpugen-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2023-10-10 20:34:56.650777 dpugen-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2023-10-10 20:34:42.000000 dpugen-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 20:34:56.642777 dpugen-0.1.2/dpugen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 20:34:56.646777 dpugen-0.1.2/dpugen/dashgen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/acl_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/dash_appliance_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/dash_eni_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/dash_route_rule_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/dash_route_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/dash_vnet_mapping_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/dash_vnet_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/prefix_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/vpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/dashgen/vpcmappingtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 20:34:56.646777 dpugen-0.1.2/dpugen/dpugen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2023-10-10 20:34:56.000000 dpugen-0.1.2/dpugen/dpugen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-10-10 20:34:56.000000 dpugen-0.1.2/dpugen/dpugen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 20:34:56.000000 dpugen-0.1.2/dpugen/dpugen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-10 20:34:56.000000 dpugen-0.1.2/dpugen/dpugen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-10 20:34:56.000000 dpugen-0.1.2/dpugen/dpugen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 20:34:56.650777 dpugen-0.1.2/dpugen/saigen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/acl_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/address_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/direction_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/enis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/inbound_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/outbound_ca_to_pa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/outbound_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/pa_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/vips.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-10-10 20:34:42.000000 dpugen-0.1.2/dpugen/saigen/vnets.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-10 20:34:42.000000 dpugen-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-10-10 20:34:56.650777 dpugen-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:54:24.032064 dpugen-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 15:54:19.000000 dpugen-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-30 15:54:24.032064 dpugen-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-30 15:54:19.000000 dpugen-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:54:24.028064 dpugen-0.1.3/dpugen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:54:24.032064 dpugen-0.1.3/dpugen/dashgen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/acl_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/dash_appliance_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/dash_eni_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/dash_route_rule_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/dash_route_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/dash_vnet_mapping_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/dash_vnet_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/prefix_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/dashgen/vpcmappingtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:54:24.032064 dpugen-0.1.3/dpugen/dpugen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-30 15:54:24.000000 dpugen-0.1.3/dpugen/dpugen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-30 15:54:24.000000 dpugen-0.1.3/dpugen/dpugen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:54:24.000000 dpugen-0.1.3/dpugen/dpugen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:54:24.000000 dpugen-0.1.3/dpugen/dpugen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 15:54:24.000000 dpugen-0.1.3/dpugen/dpugen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:54:24.032064 dpugen-0.1.3/dpugen/saigen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/acl_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/address_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/direction_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/enis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/inbound_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/outbound_ca_to_pa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/outbound_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/pa_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/vips.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-30 15:54:19.000000 dpugen-0.1.3/dpugen/saigen/vnets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 15:54:19.000000 dpugen-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 15:54:24.036064 dpugen-0.1.3/setup.cfg
```

### Comparing `dpugen-0.1.2/LICENSE` & `dpugen-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/PKG-INFO` & `dpugen-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpugen
-Version: 0.1.2
+Version: 0.1.3
 Summary: Multi-vendor DPU library to generate its configuration
 Home-page: https://github.com/mgheorghe/dpugen
 Author: Mircea Dan Gheorghe
 Author-email: mircea-dan.gheorghe@keysight.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dpugen-0.1.2/README.md` & `dpugen-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/dpugen/dashgen/acl_group.py` & `dpugen-0.1.3/dpugen/dashgen/acl_group.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python3
+"""DASH generator for Acl Groups"""
 
 import os
 import sys
 
 from dpugen.confbase import ConfBase
 from dpugen.confutils import common_main
 
@@ -14,14 +15,15 @@
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):  # Per ENI
+            print(f'    acl_group:eni:{eni}', file=sys.stderr)
             for stage_in_index in range(p.ACL_NSG_COUNT):  # Per inbound stage
                 table_id = eni * 1000 + stage_in_index
 
                 self.num_yields += 1
                 yield {
                     'DASH_ACL_GROUP_TABLE:%d' % table_id: {
                         'ip_version': 'ipv4',
```

### Comparing `dpugen-0.1.2/dpugen/dashgen/acl_rule.py` & `dpugen-0.1.3/dpugen/dashgen/acl_rule.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,125 +1,146 @@
 #!/usr/bin/python3
 
 import os
 import sys
 from copy import deepcopy
 
-from dpugen.confbase import ConfBase
+from dpugen.confbase import (
+    ConfBase,
+    socket_inet_ntoa,
+    struct_pack
+)
 from dpugen.confutils import common_main
 
 
 class AclRules(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
-        cp = self.cooked_params
+        ip_int = self.cooked_params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):  # Per ENI (64)
-            local_ip = cp.IP_L_START + eni_index * cp.IP_STEP_ENI
-            l_ip_ac = deepcopy(str(local_ip) + '/32')
+            print(f'    acl:{eni}', file=sys.stderr)
+            local_ip = socket_inet_ntoa(struct_pack('>L', ip_int.IP_L_START + eni_index * ip_int.IP_STEP_ENI))
+            l_ip_ac = deepcopy(local_ip + '/32')
+
             for stage_in_index in range(p.ACL_NSG_COUNT):  # Per inbound group
                 table_id = eni * 1000 + stage_in_index
+                IP_R_START_stage = ip_int.IP_R_START + eni_index * ip_int.IP_STEP_ENI + stage_in_index * ip_int.IP_STEP_NSG
                 for ip_index in range(0, p.ACL_RULES_NSG, 2):  # Per even ACL rule
-                    remote_ip_a = cp.IP_R_START + (eni_index * cp.IP_STEP_ENI) + (stage_in_index * cp.IP_STEP_NSG) + ((ip_index // 2) * cp.IP_STEP_ACL)
-                    ip_list_a = [str(remote_ip_a + expanded_index * cp.IP_STEPE) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+                    remote_ip_a = IP_R_START_stage + ip_index * p.IP_PER_ACL_RULE
+                    ip_list_a = [socket_inet_ntoa(struct_pack('>L', remote_ip_a + expanded_index * ip_int.IP_STEPE)) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+
                     ip_list_all = []
                     if ((stage_in_index % p.ACL_NSG_COUNT) == (p.ACL_NSG_COUNT - 1)) and (ip_index == (p.ACL_RULES_NSG - 2)):
-                        all_ips_stage1 = cp.IP_R_START + eni_index * cp.IP_STEP_ENI + (stage_in_index + 1) * cp.IP_STEP_NSG
-                        all_ips_stage2 = all_ips_stage1 + 1 * cp.IP_STEP_NSG
-                        all_ips_stage3 = all_ips_stage1 + 2 * cp.IP_STEP_NSG
-                        all_ips_stage4 = all_ips_stage1 + 3 * cp.IP_STEP_NSG
-                        all_ips_stage5 = all_ips_stage1 + 4 * cp.IP_STEP_NSG
+                        all_ips_stage1 = ip_int.IP_R_START + eni_index * ip_int.IP_STEP_ENI + (stage_in_index + 1) * ip_int.IP_STEP_NSG - 1
+                        all_ips_stage2 = all_ips_stage1 + 1 * ip_int.IP_STEP_NSG
+                        all_ips_stage3 = all_ips_stage1 + 2 * ip_int.IP_STEP_NSG
+                        all_ips_stage4 = all_ips_stage1 + 3 * ip_int.IP_STEP_NSG
+                        all_ips_stage5 = all_ips_stage1 + 4 * ip_int.IP_STEP_NSG
                         ip_list_all = [
-                            str(all_ips_stage1) + '/15',
-                            str(all_ips_stage2) + '/15',
-                            str(all_ips_stage3) + '/15',
-                            str(all_ips_stage4) + '/15',
-                            str(all_ips_stage5) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage1)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage2)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage3)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage4)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage5)) + '/15',
                         ]
 
                     # Allow
+                    if len(ip_list_all) > 0:
+                        prefixes = ip_list_a[:] + ip_list_all[:]
+                    else:
+                        prefixes = ip_list_a
+                    
                     self.num_yields += 1
                     yield {
                         'DASH_ACL_RULE_TABLE:%d:rule%d' % (table_id, ip_index): {
                             'priority': ip_index,
                             'action': 'allow',
                             'terminating': 'true',
-                            'src_addr': ','.join(ip_list_a[:] + ip_list_all[:]),
+                            'src_addr': ','.join(prefixes),
                             'dst_addr': l_ip_ac
                         },
                         'OP': 'SET'
                     }
 
-                    remote_ip_d = remote_ip_a - cp.IP_STEP1
-                    ip_list_d = [str(remote_ip_d + expanded_index * cp.IP_STEPE) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+                    remote_ip_d = remote_ip_a - ip_int.IP_STEP1
+                    ip_list_d = [socket_inet_ntoa(struct_pack('>L', remote_ip_d + expanded_index * ip_int.IP_STEPE)) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
 
                     # Deny
+
                     self.num_yields += 1
                     yield {
                         'DASH_ACL_RULE_TABLE:%d:rule%d' % (table_id, ip_index + 1): {
                             'priority': ip_index + 1,
                             'action': 'deny',
                             'terminating': 'true',
-                            'src_addr': ','.join(ip_list_d[:]),
+                            'src_addr': ','.join(ip_list_d),
                             'dst_addr': l_ip_ac
                         },
                         'OP': 'SET'
                     }
 
             for stage_out_index in range(p.ACL_NSG_COUNT):
                 table_id = eni * 1000 + 500 + stage_out_index
+                IP_R_START_stage = ip_int.IP_R_START + (eni_index * ip_int.IP_STEP_ENI) + (p.ACL_NSG_COUNT + stage_out_index) * ip_int.IP_STEP_NSG
                 for ip_index in range(0, p.ACL_RULES_NSG, 2):
-                    remote_ip_a = cp.IP_R_START + (eni_index * cp.IP_STEP_ENI) + (p.ACL_NSG_COUNT + stage_out_index) * cp.IP_STEP_NSG + (ip_index // 2) * cp.IP_STEP_ACL
-                    ip_list_a = [str(remote_ip_a + expanded_index * cp.IP_STEPE) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+                    remote_ip_a = IP_R_START_stage + ip_index * p.IP_PER_ACL_RULE
+                    ip_list_a = [socket_inet_ntoa(struct_pack('>L', remote_ip_a + expanded_index * ip_int.IP_STEPE)) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
 
                     ip_list_all = []
                     if ((stage_out_index % p.ACL_NSG_COUNT)) == (p.ACL_NSG_COUNT - 1) and (ip_index == (p.ACL_RULES_NSG - 2)):
-                        all_ips_stage1 = cp.IP_R_START + eni_index * cp.IP_STEP_ENI
-                        all_ips_stage2 = all_ips_stage1 + 1 * cp.IP_STEP_NSG
-                        all_ips_stage3 = all_ips_stage1 + 2 * cp.IP_STEP_NSG
-                        all_ips_stage4 = all_ips_stage1 + 3 * cp.IP_STEP_NSG
-                        all_ips_stage5 = all_ips_stage1 + 4 * cp.IP_STEP_NSG
+                        all_ips_stage1 = ip_int.IP_R_START + eni_index * ip_int.IP_STEP_ENI - 1
+                        all_ips_stage2 = all_ips_stage1 + 1 * ip_int.IP_STEP_NSG
+                        all_ips_stage3 = all_ips_stage1 + 2 * ip_int.IP_STEP_NSG
+                        all_ips_stage4 = all_ips_stage1 + 3 * ip_int.IP_STEP_NSG
+                        all_ips_stage5 = all_ips_stage1 + 4 * ip_int.IP_STEP_NSG
                         ip_list_all = [
-                            str(all_ips_stage1) + '/15',
-                            str(all_ips_stage2) + '/15',
-                            str(all_ips_stage3) + '/15',
-                            str(all_ips_stage4) + '/15',
-                            str(all_ips_stage5) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage1)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage2)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage3)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage4)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage5)) + '/15',
                         ]
+
                     # allow
+                    if len(ip_list_all) > 0:
+                        prefixes = ip_list_a[:] + ip_list_all[:]
+                    else:
+                        prefixes = ip_list_a
+                        
                     self.num_yields += 1
                     yield {
                         'DASH_ACL_RULE_TABLE:%d:rule%d' % (table_id, ip_index): {
                             'priority': ip_index,
                             'action': 'allow',
                             'terminating': 'true',
                             'src_addr': l_ip_ac,
-                            'dst_addr': ','.join(ip_list_a[:] + ip_list_all[:])
+                            'dst_addr': ','.join(prefixes)
                         },
                         'OP': 'SET'
                     }
 
-                    remote_ip_d = remote_ip_a - cp.IP_STEP1
-                    ip_list_d = [str(remote_ip_d + expanded_index * cp.IP_STEPE) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
-
                     # Deny
+                    remote_ip_d = remote_ip_a - ip_int.IP_STEP1
+                    ip_list_d = [socket_inet_ntoa(struct_pack('>L', remote_ip_d + expanded_index * ip_int.IP_STEPE)) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+
                     self.num_yields += 1
                     yield {
                         'DASH_ACL_RULE_TABLE:%d:rule%d' % (table_id, ip_index + 1): {
                             'priority': ip_index + 1,
                             'action': 'deny',
                             'terminating': 'true',
                             'src_addr': l_ip_ac,
-                            'dst_addr': ','.join(ip_list_d[:])
+                            'dst_addr': ','.join(ip_list_d)
                         },
                         'OP': 'SET'
                     }
 
 
 if __name__ == '__main__':
     conf = AclRules()
```

### Comparing `dpugen-0.1.2/dpugen/dashgen/dash_appliance_table.py` & `dpugen-0.1.3/dpugen/dashgen/dash_appliance_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         #             "vm_vni": f'{eni}'
         #         },
         #         'OP': 'SET'
         #     }
         self.num_yields += 1
         yield {
             'DASH_APPLIANCE_TABLE:appliance-%d' % p.ENI_START: {
-                'sip': '221.0.0.1',
+                'sip': f'{p.LOOPBACK}',
                 'vm_vni': f'{p.ENI_START}'
             },
             'OP': 'SET'
         }
 
 
 if __name__ == '__main__':
```

### Comparing `dpugen-0.1.2/dpugen/dashgen/dash_eni_table.py` & `dpugen-0.1.3/dpugen/dashgen/dash_eni_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 #!/usr/bin/python3
+"""DASH generator for ENI"""
 
 import os
 import sys
 
 from dpugen.confbase import (
     ConfBase,
-    ipa,
-    maca
+    maca,
+    socket_inet_ntoa,
+    struct_pack
 )
 from dpugen.confutils import common_main
 
 
 class Enis(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
-        cp = self.cooked_params
+        ip_int = self.cooked_params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):  # Per ENI
-            local_mac = str(maca(int(cp.MAC_L_START) + eni_index * int(maca(p.ENI_MAC_STEP)))).replace('-', ':')
-            vm_underlay_dip = str(ipa(p.PAL) + eni_index * int(ipa(p.IP_STEP1)))
+            local_mac = str(maca(ip_int.MAC_L_START + eni_index * ip_int.MAC_STEP_ENI))
+            vm_underlay_dip = socket_inet_ntoa(struct_pack('>L', ip_int.PAL + eni_index * ip_int.IP_STEP1))
             r_vni_id = p.ENI_L2R_STEP + eni
             for nsg_index in range(p.ACL_NSG_COUNT * 2):
                 stage = nsg_index % p.ACL_NSG_COUNT + 1
                 if nsg_index < p.ACL_NSG_COUNT:
                     nsg_id = eni * 1000 + nsg_index
                     self.num_yields += 1
                     yield {
```

### Comparing `dpugen-0.1.2/dpugen/dashgen/dash_route_rule_table.py` & `dpugen-0.1.3/dpugen/dashgen/dash_route_rule_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 #!/usr/bin/python3
 
 import os
 import sys
 
-from dpugen.confbase import ConfBase
+from dpugen.confbase import (
+    ConfBase,
+    socket_inet_ntoa,
+    struct_pack
+)
 from dpugen.confutils import common_main
 
 
-class RouteRules(ConfBase):
+class InRouteRules(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
-        cp = self.cooked_params
+        ip_int = self.cooked_params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
             r_vni_id = eni + p.ENI_L2R_STEP
-            vtep_remote = cp.PAR + eni_index * cp.IP_STEP1
+            vtep_remote = socket_inet_ntoa(struct_pack('>L', ip_int.PAR + eni_index * ip_int.IP_STEP1))
             self.num_yields += 1
             yield {
                 'DASH_ROUTE_RULE_TABLE:eni-%d:%d:%s/32' % (eni, r_vni_id, vtep_remote): {
                     'action_type': 'decap',
                     'priority': '0',
                     # "protocol": "0",
                     'pa_validation': 'true',
                     'vnet':  'vnet-%d' % r_vni_id
                 },
                 'OP': 'SET'
             }
 
 
 if __name__ == '__main__':
-    conf = RouteRules()
+    conf = InRouteRules()
     common_main(conf)
```

### Comparing `dpugen-0.1.2/dpugen/dashgen/dash_vnet_mapping_table.py` & `dpugen-0.1.3/dpugen/dashgen/dash_vnet_mapping_table.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,107 @@
 #!/usr/bin/python3
+"""DASH generator for Outbound CA PA mapping table"""
 
 import os
 import sys
 
 from dpugen.confbase import (
     ConfBase,
-    ipa,
-    maca
+    maca,
+    socket_inet_ntoa,
+    struct_pack
 )
 from dpugen.confutils import common_main
 
 
 class Mappings(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
+        ip_int = self.cooked_params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):  # Per ENI
-            vtep_remote = str(ipa(p.PAR) + int(ipa(p.IP_STEP1)) * eni_index)
-            vtep_eni = str(ipa(p.PAL) + int(ipa(p.IP_STEP1)) * eni_index)
+            vtep_remote = socket_inet_ntoa(struct_pack('>L', ip_int.PAR + ip_int.IP_STEP1 * eni_index))
+            gateway_ip =  socket_inet_ntoa(struct_pack('>L', ip_int.GATEWAY + ip_int.IP_STEP1 * eni_index))
+            remote_ip_a_eni = ip_int.IP_R_START + eni_index * ip_int.IP_STEP_ENI
+            remote_mac_a_eni = ip_int.MAC_R_START + eni_index * ip_int.MAC_STEP_ENI
+            gateway_mac = str(maca(remote_mac_a_eni))
+
+            # add mapping for ENI itself SAI_OBJECT_TYPE_ENI_ETHER_ADDRESS_MAP_ENTRY
+            eni_ip = socket_inet_ntoa(struct_pack('>L', ip_int.IP_L_START + eni_index * ip_int.IP_STEP_ENI))
+            eni_mac = str(maca(ip_int.MAC_L_START + eni_index * ip_int.MAC_STEP_ENI))
             r_vni_id = eni + p.ENI_L2R_STEP
+            
+            self.num_yields += 1
+            yield {
+                'DASH_VNET_MAPPING_TABLE:vnet-%d:%s' % (r_vni_id, eni_ip): {
+                    'routing_type': 'vnet_encap',
+                    'underlay_ip': p.LOOPBACK,
+                    'mac_address': eni_mac,
+                    'use_dst_vni': 'true'
+                },
+                'OP': 'SET'
+            }
 
-            # 1 in 4 enis will have all its ips mapped
-            if (eni % 4) == 1:
-                # mapped IPs
+            # just some prefixes may have a mapping entry
+            if p.ACL_MAPPED_PER_NSG >= 1:
                 print(f'    mapped:eni:{eni}', file=sys.stderr)
-                for nsg_index in range(p.ACL_NSG_COUNT):  # Per outbound stage
+                for nsg_index in range(p.ACL_NSG_COUNT * 2):  # Per outbound stage
+                    remote_ip_a_nsg = remote_ip_a_eni + nsg_index * ip_int.IP_STEP_NSG
+                    remote_mac_a_nsg = remote_mac_a_eni + nsg_index * ip_int.MAC_STEP_NSG
+                    
                     # Per half of the rules
-                    for acl_index in range(p.ACL_RULES_NSG // 2):
-                        remote_ip_a = ipa(p.IP_R_START) + (eni_index * int(ipa(p.IP_STEP_ENI))) + \
-                            (nsg_index * int(ipa(p.IP_STEP_NSG))) + \
-                            (acl_index * int(ipa(p.IP_STEP_ACL)))
-                        remote_mac_a = str(
-                            maca(
-                                int(maca(p.MAC_R_START))
-                                + eni_index * int(maca(p.ENI_MAC_STEP))
-                                + nsg_index * int(maca(p.ACL_NSG_MAC_STEP))
-                                + acl_index * int(maca(p.ACL_POLICY_MAC_STEP))
-                            )
-                        ).replace('-', ':')
-
-                        # Allow
-                        for i in range(p.IP_MAPPED_PER_ACL_RULE):  # Per rule prefix
-                            remote_expanded_ip = str(remote_ip_a + i * 2)
-                            remote_expanded_mac = str(
-                                maca(
-                                    int(maca(remote_mac_a)) + i * 2
-                                )
-                            ).replace('-', ':')
-
-                            self.num_yields += 1
-                            yield {
-                                'DASH_VNET_MAPPING_TABLE:vnet-%d:%s' % (r_vni_id, remote_expanded_ip): {
-                                    'routing_type': 'vnet_encap',
-                                    'underlay_ip': str(vtep_remote),
-                                    'mac_address': remote_expanded_mac,
-                                    'use_dst_vni': 'true'
-                                },
-                                'OP': 'SET'
-                            }
+                    for acl_index in range(p.ACL_RULES_NSG):
+                        remote_ip_a = remote_ip_a_nsg + acl_index * p.IP_PER_ACL_RULE
+                        remote_mac_a = remote_mac_a_nsg + acl_index * p.IP_PER_ACL_RULE
+
+                        if (acl_index % 2) == 0:
+                            # Allow
+                            if acl_index <= p.ACL_MAPPED_PER_NSG:
+                                for i in range(p.IP_PER_ACL_RULE):  # Per rule prefix
+                                    remote_expanded_ip = socket_inet_ntoa(struct_pack('>L', remote_ip_a + i * 2))
+                                    remote_expanded_mac = str(maca(remote_mac_a + i * 2))
+
+                                    self.num_yields += 1
+                                    yield {
+                                        'DASH_VNET_MAPPING_TABLE:vnet-%d:%s' % (r_vni_id, remote_expanded_ip): {
+                                            'routing_type': 'vnet_encap',
+                                            'underlay_ip': vtep_remote,
+                                            'mac_address': remote_expanded_mac,
+                                            'use_dst_vni': 'true'
+                                        },
+                                        'OP': 'SET'
+                                    }
+                            else:
+                                pass
+
+                        else:
+                            # Deny
+                            pass
 
-            # 3 in 4 enis will have just mapping for gateway ip, for ip that are only routed and not mapped
-            else:
-                # routed IPs
+            # some prefixes will be routed through a gateway, need mapping for gateway
+            elif p.ACL_MAPPED_PER_NSG == 0:
                 print(f'    routed:eni:{eni}', file=sys.stderr)
 
-                remote_expanded_mac = str(
-                    maca(
-                        int(maca(p.MAC_R_START)) +
-                        eni_index * int(maca(p.ENI_MAC_STEP))
-                    )
-                ).replace('-', ':')
                 self.num_yields += 1
                 yield {
-                    'DASH_VNET_MAPPING_TABLE:vnet-%d:%s' % (r_vni_id, vtep_eni): {
+                    'DASH_VNET_MAPPING_TABLE:vnet-%d:%s' % (r_vni_id, gateway_ip): {
                         'routing_type': 'vnet_encap',
-                        'underlay_ip': str(vtep_remote),
-                        'mac_address': remote_expanded_mac,
+                        'underlay_ip': vtep_remote,
+                        'mac_address': gateway_mac,
                         'use_dst_vni': 'true'
                     },
                     'OP': 'SET'
                 }
+            
+            else:
+                raise Exception('ACL_MAPPED_PER_NSG <%d> cannot be < 0' % p.ACL_MAPPED_PER_NSG)
 
 
 if __name__ == '__main__':
     conf = Mappings()
     common_main(conf)
```

### Comparing `dpugen-0.1.2/dpugen/dashgen/dash_vnet_table.py` & `dpugen-0.1.3/dpugen/dashgen/dash_vnet_table.py`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/dpugen/dashgen/prefix_tag.py` & `dpugen-0.1.3/dpugen/dashgen/prefix_tag.py`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/dpugen/dashgen/vpc.py` & `dpugen-0.1.3/dpugen/dashgen/vpc.py`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/dpugen/dashgen/vpcmappingtypes.py` & `dpugen-0.1.3/dpugen/dashgen/vpcmappingtypes.py`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/dpugen/dpugen.egg-info/PKG-INFO` & `dpugen-0.1.3/dpugen/dpugen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpugen
-Version: 0.1.2
+Version: 0.1.3
 Summary: Multi-vendor DPU library to generate its configuration
 Home-page: https://github.com/mgheorghe/dpugen
 Author: Mircea Dan Gheorghe
 Author-email: mircea-dan.gheorghe@keysight.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dpugen-0.1.2/dpugen/dpugen.egg-info/SOURCES.txt` & `dpugen-0.1.3/dpugen/dpugen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/dpugen/saigen/acl_group.py` & `dpugen-0.1.3/dpugen/saigen/acl_group.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,30 +14,35 @@
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
 
-        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
-            for nsg_index in range(1, (p.ACL_NSG_COUNT + 1)):
+        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):  # Per ENI
+            print(f'    acl_group:eni:{eni}', file=sys.stderr)
+            for stage_in_index in range(p.ACL_NSG_COUNT):  # Per inbound stage
+                table_id = eni * 1000 + stage_in_index
 
                 self.num_yields += 1
                 yield {
-                    'name': f'in_acl_group_#eni{eni}nsg{nsg_index}',
+                    'name': f'in_acl_group_#{table_id}',
                     'op': 'create',
                     'type': 'SAI_OBJECT_TYPE_DASH_ACL_GROUP',
                     'attributes': [
                         'SAI_DASH_ACL_GROUP_ATTR_IP_ADDR_FAMILY', 'SAI_IP_ADDR_FAMILY_IPV4',
                     ]
                 }
 
+            for stage_out_index in range(p.ACL_NSG_COUNT):  # Per outbound stage
+                table_id = eni * 1000 + 500 + stage_out_index
+
                 self.num_yields += 1
                 yield {
-                    'name': f'out_acl_group_#eni{eni}nsg{nsg_index}',
+                    'name': f'out_acl_group_#{table_id}',
                     'op': 'create',
                     'type': 'SAI_OBJECT_TYPE_DASH_ACL_GROUP',
                     'attributes': [
                         'SAI_DASH_ACL_GROUP_ATTR_IP_ADDR_FAMILY', 'SAI_IP_ADDR_FAMILY_IPV4',
                     ]
                 }
```

### Comparing `dpugen-0.1.2/dpugen/saigen/acl_rule.py` & `dpugen-0.1.3/dpugen/saigen/acl_rule.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,194 +1,164 @@
 #!/usr/bin/python3
 
 import os
 import sys
 from copy import deepcopy
 
-from dpugen.confbase import ConfBase
+from dpugen.confbase import (
+    ConfBase,
+    socket_inet_ntoa,
+    struct_pack
+)
 from dpugen.confutils import common_main
 
 
 class AclRules(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
-        cp = self.cooked_params
+        ip_int = self.cooked_params
 
-        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT)):
-            local_ip = cp.IP_L_START + eni_index * cp.IP_STEP_ENI
-            l_ip_ac = deepcopy(str(local_ip) + '/32')
+        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):  # Per ENI (64)
+            print(f'    acl:{eni}', file=sys.stderr)
+            local_ip = socket_inet_ntoa(struct_pack('>L', ip_int.IP_L_START + eni_index * ip_int.IP_STEP_ENI))
+            l_ip_ac = deepcopy(local_ip + '/32')
 
-            for stage_in_index in range(p.ACL_NSG_COUNT):
-                nsg_index = stage_in_index + 1
+            for stage_in_index in range(p.ACL_NSG_COUNT):  # Per inbound group
                 table_id = eni * 1000 + stage_in_index
-
-                for ip_index in range(0, p.ACL_RULES_NSG, 2):
-                    # print("        %d" % ip_index)
-                    remote_ip_a = cp.IP_R_START + eni_index * cp.IP_STEP_ENI + stage_in_index * cp.IP_STEP_NSG + ip_index * cp.IP_STEP_ACL
-
-                    ip_list_a = [str(remote_ip_a + expanded_index * cp.IP_STEPE)
-                                 + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
-
-                    # allow
+                IP_R_START_stage = ip_int.IP_R_START + eni_index * ip_int.IP_STEP_ENI + stage_in_index * ip_int.IP_STEP_NSG
+                for ip_index in range(0, p.ACL_RULES_NSG, 2):  # Per even ACL rule
+                    remote_ip_a = IP_R_START_stage + ip_index * p.IP_PER_ACL_RULE
+                    ip_list_a = [socket_inet_ntoa(struct_pack('>L', remote_ip_a + expanded_index * ip_int.IP_STEPE)) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+
+                    ip_list_all = []
+                    if ((stage_in_index % p.ACL_NSG_COUNT) == (p.ACL_NSG_COUNT - 1)) and (ip_index == (p.ACL_RULES_NSG - 2)):
+                        all_ips_stage1 = ip_int.IP_R_START + eni_index * ip_int.IP_STEP_ENI + (stage_in_index + 1) * ip_int.IP_STEP_NSG - 1
+                        all_ips_stage2 = all_ips_stage1 + 1 * ip_int.IP_STEP_NSG
+                        all_ips_stage3 = all_ips_stage1 + 2 * ip_int.IP_STEP_NSG
+                        all_ips_stage4 = all_ips_stage1 + 3 * ip_int.IP_STEP_NSG
+                        all_ips_stage5 = all_ips_stage1 + 4 * ip_int.IP_STEP_NSG
+                        ip_list_all = [
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage1)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage2)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage3)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage4)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage5)) + '/15',
+                        ]
+
+                    # Allow
+                    if len(ip_list_all) > 0:
+                        prefixes = ip_list_a[:] + ip_list_all[:]
+                    else:
+                        prefixes = ip_list_a
+                    
                     self.num_yields += 1
                     yield {
                         'name': 'dash_acl_%d_rule_%d' % (table_id, ip_index),
                         'op': 'create',
                         'type': 'SAI_OBJECT_TYPE_DASH_ACL_RULE',
                         'attributes': [
-                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$in_acl_group_#eni{eni}nsg{nsg_index}',
-                            'SAI_DASH_ACL_RULE_ATTR_PRIORITY','%d' % ip_index,
-                            'SAI_DASH_ACL_RULE_ATTR_ACTION','SAI_DASH_ACL_RULE_ACTION_PERMIT',
-                            'SAI_DASH_ACL_RULE_ATTR_SIP',','.join(ip_list_a[:]),
-                            'SAI_DASH_ACL_RULE_ATTR_DIP',l_ip_ac,
+                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$in_acl_group_#{table_id}',
+                            'SAI_DASH_ACL_RULE_ATTR_PRIORITY', '%d' % ip_index,
+                            'SAI_DASH_ACL_RULE_ATTR_ACTION', 'SAI_DASH_ACL_RULE_ACTION_PERMIT',
+                            'SAI_DASH_ACL_RULE_ATTR_SIP', ','.join(prefixes),
+                            'SAI_DASH_ACL_RULE_ATTR_DIP', l_ip_ac,
                             # 'SAI_DASH_ACL_RULE_ATTR_PROTOCOL','sai_u8_list_t',
                             # 'SAI_DASH_ACL_RULE_ATTR_SRC_PORT','sai_u16_range_list_t',
                             # 'SAI_DASH_ACL_RULE_ATTR_DST_PORT','sai_u16_range_list_t',
                         ]
                     }
 
-                    remote_ip_d = remote_ip_a - cp.IP_STEP1
+                    remote_ip_d = remote_ip_a - ip_int.IP_STEP1
+                    ip_list_d = [socket_inet_ntoa(struct_pack('>L', remote_ip_d + expanded_index * ip_int.IP_STEPE)) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
 
-                    ip_list_d = [str(remote_ip_d + expanded_index * cp.IP_STEPE) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+                    # Deny
 
-                    # denny
                     self.num_yields += 1
                     yield {
                         'name': 'dash_acl_%d_rule_%d' % (table_id, ip_index + 1),
                         'op': 'create',
                         'type': 'SAI_OBJECT_TYPE_DASH_ACL_RULE',
                         'attributes': [
-                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$in_acl_group_#eni{eni}nsg{nsg_index}',
+                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$in_acl_group_#{table_id}',
                             'SAI_DASH_ACL_RULE_ATTR_PRIORITY', f'{ip_index+1}',
                             'SAI_DASH_ACL_RULE_ATTR_ACTION', 'SAI_DASH_ACL_RULE_ACTION_DENY',
-                            'SAI_DASH_ACL_RULE_ATTR_SIP', ','.join(ip_list_d[:]),
-                            'SAI_DASH_ACL_RULE_ATTR_DIP', l_ip_ac,
-                            # 'SAI_DASH_ACL_RULE_ATTR_PROTOCOL', 'sai_u8_list_t',
-                            # 'SAI_DASH_ACL_RULE_ATTR_SRC_PORT', 'sai_u16_range_list_t',
-                            # 'SAI_DASH_ACL_RULE_ATTR_DST_PORT', 'sai_u16_range_list_t',
-                        ]
-                    }
-
-                # add as last rule in last table from ingress and egress an allow rule for all the ip's from egress and ingress
-                if (stage_in_index % p.ACL_NSG_COUNT) == 4:
-                    all_ips_stage1 = cp.IP_R_START + eni_index * cp.IP_STEP_ENI + stage_in_index * 4 * cp.IP_STEP_NSG
-                    all_ips_stage2 = all_ips_stage1 + 1 * 4 * cp.IP_STEP_NSG
-                    all_ips_stage3 = all_ips_stage1 + 2 * 4 * cp.IP_STEP_NSG
-                    all_ips_stage4 = all_ips_stage1 + 3 * 4 * cp.IP_STEP_NSG
-                    all_ips_stage5 = all_ips_stage1 + 4 * 4 * cp.IP_STEP_NSG
-                    ip_list_all = [
-                        str(all_ips_stage1) + '/14',
-                        str(all_ips_stage2) + '/14',
-                        str(all_ips_stage3) + '/14',
-                        str(all_ips_stage4) + '/14',
-                        str(all_ips_stage5) + '/14',
-                    ]
-
-                    # allow
-                    self.num_yields += 1
-                    yield {
-                        'name': 'dash_acl_%d_rule_%d' % (table_id, ip_index + 2),
-                        'op': 'create',
-                        'type': 'SAI_OBJECT_TYPE_DASH_ACL_RULE',
-                        'attributes': [
-                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$in_acl_group_#eni{eni}nsg{nsg_index}',
-                            'SAI_DASH_ACL_RULE_ATTR_PRIORITY', f'{ip_index + 2}',
-                            'SAI_DASH_ACL_RULE_ATTR_ACTION', 'SAI_DASH_ACL_RULE_ACTION_PERMIT',
-                            'SAI_DASH_ACL_RULE_ATTR_SIP', ','.join(ip_list_all[:]),
+                            'SAI_DASH_ACL_RULE_ATTR_SIP', ','.join(ip_list_d),
                             'SAI_DASH_ACL_RULE_ATTR_DIP', l_ip_ac,
                             # 'SAI_DASH_ACL_RULE_ATTR_PROTOCOL', 'sai_u8_list_t',
                             # 'SAI_DASH_ACL_RULE_ATTR_SRC_PORT', 'sai_u16_range_list_t',
                             # 'SAI_DASH_ACL_RULE_ATTR_DST_PORT', 'sai_u16_range_list_t',
                         ]
                     }
 
             for stage_out_index in range(p.ACL_NSG_COUNT):
                 table_id = eni * 1000 + 500 + stage_out_index
-
+                IP_R_START_stage = ip_int.IP_R_START + (eni_index * ip_int.IP_STEP_ENI) + (p.ACL_NSG_COUNT + stage_out_index) * ip_int.IP_STEP_NSG
                 for ip_index in range(0, p.ACL_RULES_NSG, 2):
-                    # print("        %d" % ip_index)
-                    remote_ip_a = cp.IP_R_START + eni_index * cp.IP_STEP_ENI + \
-                        (p.ACL_NSG_COUNT + stage_in_index) * cp.IP_STEP_NSG + ip_index * cp.IP_STEP_ACL
+                    remote_ip_a = IP_R_START_stage + ip_index * p.IP_PER_ACL_RULE
+                    ip_list_a = [socket_inet_ntoa(struct_pack('>L', remote_ip_a + expanded_index * ip_int.IP_STEPE)) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
 
-                    ip_list_a = [str(remote_ip_a + expanded_index * cp.IP_STEPE)
-                                 + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+                    ip_list_all = []
+                    if ((stage_out_index % p.ACL_NSG_COUNT)) == (p.ACL_NSG_COUNT - 1) and (ip_index == (p.ACL_RULES_NSG - 2)):
+                        all_ips_stage1 = ip_int.IP_R_START + eni_index * ip_int.IP_STEP_ENI - 1
+                        all_ips_stage2 = all_ips_stage1 + 1 * ip_int.IP_STEP_NSG
+                        all_ips_stage3 = all_ips_stage1 + 2 * ip_int.IP_STEP_NSG
+                        all_ips_stage4 = all_ips_stage1 + 3 * ip_int.IP_STEP_NSG
+                        all_ips_stage5 = all_ips_stage1 + 4 * ip_int.IP_STEP_NSG
+                        ip_list_all = [
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage1)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage2)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage3)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage4)) + '/15',
+                            socket_inet_ntoa(struct_pack('>L', all_ips_stage5)) + '/15',
+                        ]
 
                     # allow
+                    if len(ip_list_all) > 0:
+                        prefixes = ip_list_a[:] + ip_list_all[:]
+                    else:
+                        prefixes = ip_list_a
+                        
                     self.num_yields += 1
                     yield {
                         'name': 'dash_acl_%d_rule_%d' % (table_id, ip_index),
                         'op': 'create',
                         'type': 'SAI_OBJECT_TYPE_DASH_ACL_RULE',
                         'attributes': [
-                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$out_acl_group_#eni{eni}nsg{nsg_index}',
+                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$out_acl_group_#{table_id}',
                             'SAI_DASH_ACL_RULE_ATTR_PRIORITY',          f'{ip_index}',
                             'SAI_DASH_ACL_RULE_ATTR_ACTION',            'SAI_DASH_ACL_RULE_ACTION_PERMIT',
                             'SAI_DASH_ACL_RULE_ATTR_SIP',               l_ip_ac,
-                            'SAI_DASH_ACL_RULE_ATTR_DIP',               ','.join(ip_list_a[:]),
+                            'SAI_DASH_ACL_RULE_ATTR_DIP',               ','.join(prefixes),
                             # 'SAI_DASH_ACL_RULE_ATTR_PROTOCOL',          'sai_u8_list_t',
                             # 'SAI_DASH_ACL_RULE_ATTR_SRC_PORT',          'sai_u16_range_list_t',
                             # 'SAI_DASH_ACL_RULE_ATTR_DST_PORT',          'sai_u16_range_list_t',
                         ]
                     }
 
-                    remote_ip_d = remote_ip_a - cp.IP_STEP1
-
-                    ip_list_d = [str(remote_ip_d + expanded_index * cp.IP_STEPE) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
+                    # Deny
+                    remote_ip_d = remote_ip_a - ip_int.IP_STEP1
+                    ip_list_d = [socket_inet_ntoa(struct_pack('>L', remote_ip_d + expanded_index * ip_int.IP_STEPE)) + '/32' for expanded_index in range(0, p.IP_PER_ACL_RULE)]
 
-                    # denny
                     self.num_yields += 1
                     yield {
                         'name': 'dash_acl_%d_rule_%d' % (table_id, ip_index + 1),
                         'op': 'create',
                         'type': 'SAI_OBJECT_TYPE_DASH_ACL_RULE',
                         'attributes': [
-                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$out_acl_group_#eni{eni}nsg{nsg_index}',
+                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$out_acl_group_#{table_id}',
                             'SAI_DASH_ACL_RULE_ATTR_PRIORITY',          f'{ip_index+1}',
                             'SAI_DASH_ACL_RULE_ATTR_ACTION',            'SAI_DASH_ACL_RULE_ACTION_DENY',
                             'SAI_DASH_ACL_RULE_ATTR_SIP',               l_ip_ac,
-                            'SAI_DASH_ACL_RULE_ATTR_DIP',               ','.join(ip_list_d[:]),
-                            # 'SAI_DASH_ACL_RULE_ATTR_PROTOCOL',          'sai_u8_list_t',
-                            # 'SAI_DASH_ACL_RULE_ATTR_SRC_PORT',          'sai_u16_range_list_t',
-                            # 'SAI_DASH_ACL_RULE_ATTR_DST_PORT',          'sai_u16_range_list_t',
-                        ]
-                    }
-
-                # add as last rule in last table from ingress and egress an allow rule for all the ip's from egress and ingress
-                if (stage_out_index % p.ACL_NSG_COUNT) == 4:
-                    all_ips_stage1 = cp.IP_R_START + eni_index * cp.IP_STEP_ENI
-                    all_ips_stage2 = all_ips_stage1 + 1 * 4 * cp.IP_STEP_NSG
-                    all_ips_stage3 = all_ips_stage1 + 2 * 4 * cp.IP_STEP_NSG
-                    all_ips_stage4 = all_ips_stage1 + 3 * 4 * cp.IP_STEP_NSG
-                    all_ips_stage5 = all_ips_stage1 + 4 * 4 * cp.IP_STEP_NSG
-                    ip_list_all = [
-                        str(all_ips_stage1) + '/14',
-                        str(all_ips_stage2) + '/14',
-                        str(all_ips_stage3) + '/14',
-                        str(all_ips_stage4) + '/14',
-                        str(all_ips_stage5) + '/14',
-                    ]
-
-                    # allow
-                    self.num_yields += 1
-                    yield {
-                        'name': 'dash_acl_%d_rule_%d' % (table_id, ip_index + 2),
-                        'op': 'create',
-                        'type': 'SAI_OBJECT_TYPE_DASH_ACL_RULE',
-                        'attributes': [
-                            'SAI_DASH_ACL_RULE_ATTR_DASH_ACL_GROUP_ID', f'$out_acl_group_#eni{eni}nsg{nsg_index}',
-                            'SAI_DASH_ACL_RULE_ATTR_PRIORITY',          f'{ip_index+2}',
-                            'SAI_DASH_ACL_RULE_ATTR_ACTION',            'SAI_DASH_ACL_RULE_ACTION_PERMIT',
-                            'SAI_DASH_ACL_RULE_ATTR_SIP',               l_ip_ac,
-                            'SAI_DASH_ACL_RULE_ATTR_DIP',               ','.join(ip_list_all[:]),
+                            'SAI_DASH_ACL_RULE_ATTR_DIP',               ','.join(ip_list_d),
                             # 'SAI_DASH_ACL_RULE_ATTR_PROTOCOL',          'sai_u8_list_t',
                             # 'SAI_DASH_ACL_RULE_ATTR_SRC_PORT',          'sai_u16_range_list_t',
                             # 'SAI_DASH_ACL_RULE_ATTR_DST_PORT',          'sai_u16_range_list_t',
                         ]
                     }
```

### Comparing `dpugen-0.1.2/dpugen/saigen/address_maps.py` & `dpugen-0.1.3/dpugen/saigen/address_maps.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,18 @@
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
+        ip_int = self.cooked_params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
-
-            eni_mac = str(
-                maca(
-                    int(maca(p.MAC_L_START)) + eni_index * int(maca(p.ENI_MAC_STEP))
-                )
-            ).replace('-', ':')
+            eni_mac = str(maca(ip_int.MAC_L_START + eni_index * ip_int.MAC_STEP_ENI))
 
             self.num_yields += 1
             yield {
                 'name': f'eni_ether_address_map_#eni{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_ENI_ETHER_ADDRESS_MAP_ENTRY',
                 'key': {
```

### Comparing `dpugen-0.1.2/dpugen/saigen/direction_lookup.py` & `dpugen-0.1.3/dpugen/saigen/direction_lookup.py`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/dpugen/saigen/enis.py` & `dpugen-0.1.3/dpugen/saigen/enis.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 """SAI generator for ENI"""
 
 import os
 import sys
 
 from dpugen.confbase import (
     ConfBase,
-    ipa
+    maca,
+    socket_inet_ntoa,
+    struct_pack
 )
 from dpugen.confutils import common_main
 
 
 class Enis(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
+        ip_int = self.cooked_params
 
-        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
-            vm_underlay_dip = str(ipa(p.PAL) + eni_index * int(ipa(p.IP_STEP1)))
+        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):  # Per ENI
+            vm_underlay_dip = socket_inet_ntoa(struct_pack('>L', ip_int.PAL + eni_index * ip_int.IP_STEP1))
 
             eni_data = {
                 'name': f'eni_#{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_ENI',
                 'attributes': [
                     'SAI_ENI_ATTR_CPS', '10000',
@@ -54,21 +57,24 @@
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE1_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE2_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE3_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE4_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE5_DASH_ACL_GROUP_ID', '0',
                 ]
             }
-            for nsg_index in range(1, (p.ACL_NSG_COUNT + 1)):
-                stage_index = eni_data['attributes'].index(
-                    f'SAI_ENI_ATTR_INBOUND_V4_STAGE{nsg_index}_DASH_ACL_GROUP_ID')
-                eni_data['attributes'][stage_index + 1] = f'$in_acl_group_#eni{eni}nsg{nsg_index}'
-                stage_index = eni_data['attributes'].index(
-                    f'SAI_ENI_ATTR_OUTBOUND_V4_STAGE{nsg_index}_DASH_ACL_GROUP_ID')
-                eni_data['attributes'][stage_index + 1] = f'$out_acl_group_#eni{eni}nsg{nsg_index}'
+            for nsg_index in range(p.ACL_NSG_COUNT * 2):
+                stage = nsg_index % p.ACL_NSG_COUNT + 1
+                if nsg_index < p.ACL_NSG_COUNT:
+                    nsg_id = eni * 1000 + nsg_index
+                    stage_index = eni_data['attributes'].index(f'SAI_ENI_ATTR_INBOUND_V4_STAGE{stage}_DASH_ACL_GROUP_ID')
+                    eni_data['attributes'][stage_index + 1] = f'$in_acl_group_#{nsg_id}'
+                else:
+                    nsg_id = eni * 1000 + 500 + nsg_index - p.ACL_NSG_COUNT
+                    stage_index = eni_data['attributes'].index(f'SAI_ENI_ATTR_OUTBOUND_V4_STAGE{stage}_DASH_ACL_GROUP_ID')
+                    eni_data['attributes'][stage_index + 1] = f'$out_acl_group_#{nsg_id}'
 
             self.num_yields += 1
             yield eni_data
 
 
 if __name__ == '__main__':
     conf = Enis()
```

### Comparing `dpugen-0.1.2/dpugen/saigen/inbound_routing.py` & `dpugen-0.1.3/dpugen/saigen/inbound_routing.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 """SAI generator for Inbound Routing"""
 
 import os
 import sys
 
 from dpugen.confbase import (
     ConfBase,
-    ipa
+    socket_inet_ntoa,
+    struct_pack
 )
 from dpugen.confutils import common_main
 
 
 class InboundRouting(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
+        ip_int = self.cooked_params
 
-        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
-            remote_ip = str(ipa(p.IP_R_START) + eni_index * int(ipa(p.IP_STEP_ENI)))
+        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):  # Per ENI
+            remote_ip = socket_inet_ntoa(struct_pack('>L', ip_int.IP_R_START + ip_int.IP_STEP_ENI * eni_index))
 
             self.num_yields += 1
             yield {
                 'name': f'inbound_routing_#eni{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_INBOUND_ROUTING_ENTRY',
                 'key': {
```

### Comparing `dpugen-0.1.2/dpugen/saigen/pa_validation.py` & `dpugen-0.1.3/dpugen/saigen/pa_validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 """SAI generator for PA Validation"""
 
 import os
 import sys
 
 from dpugen.confbase import (
     ConfBase,
-    ipa
+    socket_inet_ntoa,
+    struct_pack
 )
 from dpugen.confutils import common_main
 
 
 class PaValidation(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
         self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
+        ip_int = self.cooked_params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
-            vtep_remote = str(ipa(p.PAR) + int(ipa(p.IP_STEP1)) * eni_index)
+            vtep_remote = socket_inet_ntoa(struct_pack('>L', ip_int.PAR + ip_int.IP_STEP1 * eni_index))
 
             self.num_yields += 1
             yield {
                 'name': f'pa_validation_#eni{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_PA_VALIDATION_ENTRY',
                 'key': {
```

### Comparing `dpugen-0.1.2/dpugen/saigen/vips.py` & `dpugen-0.1.3/dpugen/saigen/vips.py`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/dpugen/saigen/vnets.py` & `dpugen-0.1.3/dpugen/saigen/vnets.py`

 * *Files identical despite different names*

### Comparing `dpugen-0.1.2/setup.cfg` & `dpugen-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dpugen
-version = 0.1.2
+version = 0.1.3
 author = Mircea Dan Gheorghe
 author_email = mircea-dan.gheorghe@keysight.com
 description = Multi-vendor DPU library to generate its configuration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mgheorghe/dpugen
 classifiers =
```

