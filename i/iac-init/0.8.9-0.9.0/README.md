# Comparing `tmp/iac_init-0.8.9.tar.gz` & `tmp/iac_init-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.8.9.tar", max compression
+gzip compressed data, was "iac_init-0.9.0.tar", max compression
```

## Comparing `iac_init-0.8.9.tar` & `iac_init-0.9.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    16295 2024-05-30 04:19:20.863742 iac_init-0.8.9/LICENSE
--rw-r--r--   0        0        0        0 2024-05-30 04:19:20.863742 iac_init-0.8.9/README.md
--rw-r--r--   0        0        0      392 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/__main__.py
--rwxr-xr-x   0        0        0   740216 2024-05-30 04:19:42.679525 iac_init-0.8.9/iac_init/cli/main.so
--rwxr-xr-x   0        0        0    81232 2024-05-30 04:19:42.967523 iac_init-0.8.9/iac_init/cli/options.so
--rw-r--r--   0        0        0     1827 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/conf/__init__.py
--rwxr-xr-x   0        0        0   111224 2024-05-30 04:19:43.479518 iac_init-0.8.9/iac_init/conf/global_settings.so
--rwxr-xr-x   0        0        0   270296 2024-05-30 04:19:48.631463 iac_init-0.8.9/iac_init/scripts/ansible_tool.so
--rwxr-xr-x   0        0        0   327968 2024-05-30 04:19:51.315436 iac_init-0.8.9/iac_init/scripts/apic_connecton_tool.so
--rwxr-xr-x   0        0        0   696144 2024-05-30 04:19:46.747482 iac_init-0.8.9/iac_init/scripts/cimc_precheck_tool.so
--rwxr-xr-x   0        0        0   199472 2024-05-30 04:19:52.007430 iac_init-0.8.9/iac_init/scripts/ssh_tool.so
--rwxr-xr-x   0        0        0   297296 2024-05-30 04:19:49.887450 iac_init-0.8.9/iac_init/scripts/telnet_tool.so
--rwxr-xr-x   0        0        0   207112 2024-05-30 04:19:47.499474 iac_init-0.8.9/iac_init/scripts/thread_tool.so
--rw-r--r--   0        0        0     3778 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-30 04:19:20.863742 iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/02-apic_init/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-30 04:19:20.867742 iac_init-0.8.9/iac_init/templates/03-nac_tasks/inventory.yaml.j2
--rwxr-xr-x   0        0        0    76688 2024-05-30 04:19:32.151626 iac_init-0.8.9/iac_init/utils/exceptions.so
--rwxr-xr-x   0        0        0   390296 2024-05-30 04:19:31.867629 iac_init-0.8.9/iac_init/utils/functional.so
--rwxr-xr-x   0        0        0  1133136 2024-05-30 04:19:30.059650 iac_init-0.8.9/iac_init/validator.so
--rwxr-xr-x   0        0        0   526264 2024-05-30 04:19:34.815597 iac_init-0.8.9/iac_init/yaml_conf/iac_yaml.so
--rwxr-xr-x   0        0        0   627976 2024-05-30 04:19:37.943564 iac_init-0.8.9/iac_init/yaml_conf/yaml_writer.so
--rw-r--r--   0        0        0     1636 2024-05-30 04:19:20.867742 iac_init-0.8.9/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-30 05:48:09.408414 iac_init-0.9.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-30 05:48:09.408414 iac_init-0.9.0/README.md
+-rw-r--r--   0        0        0      392 2024-05-30 05:48:09.408414 iac_init-0.9.0/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-30 05:48:09.408414 iac_init-0.9.0/iac_init/__main__.py
+-rw-r--r--   0        0        0    13438 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1827 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1166 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1583 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2847 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7992 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      443 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1871 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      336 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    14664 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/validator.py
+-rw-r--r--   0        0        0     5269 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5542 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-05-30 05:48:09.416413 iac_init-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.9.0/PKG-INFO
```

### Comparing `iac_init-0.8.9/LICENSE` & `iac_init-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/conf/__init__.py` & `iac_init-0.9.0/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/tasks/main.yml` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/tasks/main.yml` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/01-fabric_bootstrap/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/tasks/main.yml` & `iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/iac_init/templates/02-apic_init/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.9/pyproject.toml` & `iac_init-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.8.9"
+version = "0.9.0"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.8.9/PKG-INFO` & `iac_init-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.8.9
+Version: 0.9.0
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

