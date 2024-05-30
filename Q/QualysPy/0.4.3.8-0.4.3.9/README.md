# Comparing `tmp/qualyspy-0.4.3.8.tar.gz` & `tmp/qualyspy-0.4.3.9.tar.gz`

## Comparing `qualyspy-0.4.3.8.tar` & `qualyspy-0.4.3.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/.qualyspy-example
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/.readthedocs.yaml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/.vscode/launch.json
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/.vscode/settings.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/.vscode/tasks.json
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/debug/build.sh
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/debug/knowledge_base_vuln_list_output.dtd
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/debug/remove_cookies.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/docs/Makefile
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/docs/conf.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/docs/make.bat
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/docs/modules.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/docs/qualyspy.models.rst
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/docs/qualyspy.models.vmdr.rst
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/docs/qualyspy.rst
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/URLS.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/__init__.py
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/asset_mgmt_tagging.py
--rw-r--r--   0        0        0    14502 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/base.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/exceptions.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/gav.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/qutils.py
--rw-r--r--   0        0        0    15179 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/vmdr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/__init__.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/sa_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/asset_output.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/asset_request.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/tag_output.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/tag_request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/gav/__init__.py
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/gav/asset_details_orm.py
--rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/gav/asset_details_output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/vmdr/__init__.py
--rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/vmdr/host_list_orm.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/vmdr/host_list_output.py
--rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/vmdr/host_list_vm_detection_orm.py
--rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/vmdr/host_list_vm_detection_output.py
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/qualyspy/models/vmdr/knowledgebase_output.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/requirements/dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/tests/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/tests/asset_mgmt_tagging_test.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/tests/gav_test.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/tests/vmdr_test.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/LICENSE
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/README.md
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 qualyspy-0.4.3.8/PKG-INFO
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/.qualyspy-example
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/.vscode/launch.json
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/.vscode/settings.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/debug/build.sh
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/debug/knowledge_base_vuln_list_output.dtd
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/debug/remove_cookies.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/docs/Makefile
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/docs/conf.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/docs/make.bat
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/docs/modules.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/docs/qualyspy.models.rst
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/docs/qualyspy.models.vmdr.rst
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/docs/qualyspy.rst
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/URLS.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/__init__.py
+-rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/asset_mgmt_tagging.py
+-rw-r--r--   0        0        0    14502 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/base.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/exceptions.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/gav.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/qutils.py
+-rw-r--r--   0        0        0    15179 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/vmdr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/__init__.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/sa_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/asset_output.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/asset_request.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/tag_output.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/tag_request.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/gav/__init__.py
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/gav/asset_details_orm.py
+-rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/gav/asset_details_output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/vmdr/__init__.py
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/vmdr/host_list_orm.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/vmdr/host_list_output.py
+-rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/vmdr/host_list_vm_detection_orm.py
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/vmdr/host_list_vm_detection_output.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/qualyspy/models/vmdr/knowledgebase_output.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/requirements/dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/tests/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/tests/asset_mgmt_tagging_test.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/tests/gav_test.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/tests/vmdr_test.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/LICENSE
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/README.md
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 qualyspy-0.4.3.9/PKG-INFO
```

### Comparing `qualyspy-0.4.3.8/.readthedocs.yaml` & `qualyspy-0.4.3.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/.vscode/launch.json` & `qualyspy-0.4.3.9/.vscode/launch.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9801587301587301%*

 * *Differences: {"'configurations'": "{0: {'type': 'debugpy'}, 1: {'type': 'debugpy'}, 2: {'type': 'debugpy'}}"}*

```diff
@@ -2,31 +2,31 @@
     "configurations": [
         {
             "console": "integratedTerminal",
             "justMyCode": true,
             "name": "Python: Current File",
             "program": "${file}",
             "request": "launch",
-            "type": "python"
+            "type": "debugpy"
         },
         {
             "console": "integratedTerminal",
             "justMyCode": true,
             "name": "QualysPy",
             "program": "${workspaceFolder}/debug/test.py",
             "request": "launch",
-            "type": "python"
+            "type": "debugpy"
         },
         {
             "console": "integratedTerminal",
             "justMyCode": false,
             "name": "Python: Debug Tests",
             "program": "${file}",
             "purpose": [
                 "debug-test"
             ],
             "request": "launch",
-            "type": "python"
+            "type": "debugpy"
         }
     ],
     "version": "0.2.0"
 }
```

### Comparing `qualyspy-0.4.3.8/.vscode/tasks.json` & `qualyspy-0.4.3.9/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/debug/knowledge_base_vuln_list_output.dtd` & `qualyspy-0.4.3.9/debug/knowledge_base_vuln_list_output.dtd`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/debug/remove_cookies.py` & `qualyspy-0.4.3.9/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/docs/Makefile` & `qualyspy-0.4.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/docs/conf.py` & `qualyspy-0.4.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/docs/make.bat` & `qualyspy-0.4.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/docs/qualyspy.models.vmdr.rst` & `qualyspy-0.4.3.9/docs/qualyspy.models.vmdr.rst`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/docs/qualyspy.rst` & `qualyspy-0.4.3.9/docs/qualyspy.rst`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/URLS.py` & `qualyspy-0.4.3.9/qualyspy/URLS.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/asset_mgmt_tagging.py` & `qualyspy-0.4.3.9/qualyspy/asset_mgmt_tagging.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/base.py` & `qualyspy-0.4.3.9/qualyspy/base.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/gav.py` & `qualyspy-0.4.3.9/qualyspy/gav.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/qutils.py` & `qualyspy-0.4.3.9/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/vmdr.py` & `qualyspy-0.4.3.9/qualyspy/vmdr.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/sa_types.py` & `qualyspy-0.4.3.9/qualyspy/models/sa_types.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/asset_output.py` & `qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/asset_output.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/asset_request.py` & `qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/asset_request.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/tag_output.py` & `qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/tag_output.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/asset_mgmt_tagging/tag_request.py` & `qualyspy-0.4.3.9/qualyspy/models/asset_mgmt_tagging/tag_request.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/gav/asset_details_orm.py` & `qualyspy-0.4.3.9/qualyspy/models/gav/asset_details_orm.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/gav/asset_details_output.py` & `qualyspy-0.4.3.9/qualyspy/models/gav/asset_details_output.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/vmdr/host_list_orm.py` & `qualyspy-0.4.3.9/qualyspy/models/vmdr/host_list_orm.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/vmdr/host_list_output.py` & `qualyspy-0.4.3.9/qualyspy/models/vmdr/host_list_output.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/vmdr/host_list_vm_detection_orm.py` & `qualyspy-0.4.3.9/qualyspy/models/vmdr/host_list_vm_detection_orm.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/vmdr/host_list_vm_detection_output.py` & `qualyspy-0.4.3.9/qualyspy/models/vmdr/host_list_vm_detection_output.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/qualyspy/models/vmdr/knowledgebase_output.py` & `qualyspy-0.4.3.9/qualyspy/models/vmdr/knowledgebase_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,17 @@
     last_customization: LastCustomization | None = element(
         tag="LAST_CUSTOMIZATION", default=None
     )
     last_service_modification_datetime: datetime.datetime | None = element(
         tag="LAST_SERVICE_MODIFICATION_DATETIME", default=None
     )
     published_datetime: datetime.datetime = element(tag="PUBLISHED_DATETIME")
+    code_modified_datetime: datetime.datetime | None = element(
+        tag="CODE_MODIFIED_DATETIME", default=None
+    )
     bugtraq_list: list[Bugtraq] | None = wrapped(
         "BUGTRAQ_LIST", element(tag="BUGTRAQ", default=None)
     )
     patchable: bool | None = element(tag="PATCHABLE", default=None)
     software_list: list[Software] | None = wrapped(
         "SOFTWARE_LIST", element(tag="SOFTWARE", default=None)
     )
```

### Comparing `qualyspy-0.4.3.8/tests/asset_mgmt_tagging_test.py` & `qualyspy-0.4.3.9/tests/asset_mgmt_tagging_test.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/tests/gav_test.py` & `qualyspy-0.4.3.9/tests/gav_test.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/tests/vmdr_test.py` & `qualyspy-0.4.3.9/tests/vmdr_test.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/.gitignore` & `qualyspy-0.4.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/LICENSE` & `qualyspy-0.4.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/README.md` & `qualyspy-0.4.3.9/README.md`

 * *Files identical despite different names*

### Comparing `qualyspy-0.4.3.8/pyproject.toml` & `qualyspy-0.4.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.4.3.8"
+version = "0.4.3.9"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.4.3.8/PKG-INFO` & `qualyspy-0.4.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: QualysPy
-Version: 0.4.3.8
+Version: 0.4.3.9
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

