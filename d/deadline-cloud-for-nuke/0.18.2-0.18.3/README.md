# Comparing `tmp/deadline_cloud_for_nuke-0.18.2.tar.gz` & `tmp/deadline_cloud_for_nuke-0.18.3.tar.gz`

## Comparing `deadline_cloud_for_nuke-0.18.2.tar` & `deadline_cloud_for_nuke-0.18.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/_version.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/hatch_custom_hook.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/menu.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/_version.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/NukeAdaptor.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/__init__.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/__main__.py
--rw-r--r--   0        0        0    19258 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/adaptor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/py.typed
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/__init__.py
--rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/nuke_client.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/nuke_handler.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/py.typed
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/__init__.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/_logging.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/_version.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/adaptor_override_environment.yaml
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/assets.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/data_classes.py
--rw-r--r--   0        0        0    14467 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/deadline_submitter_for_nuke.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/default_nuke_job_template.yaml
--rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/job_bundle_output_test_runner.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/py.typed
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/ui/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_util/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_util/_version.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_util/ocio.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/NOTICE
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/README.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/hatch.toml
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/pyproject.toml
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/_version.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/hatch_custom_hook.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/menu.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/_version.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/NukeAdaptor.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/__init__.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/__main__.py
+-rw-r--r--   0        0        0    19258 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/adaptor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/py.typed
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeClient/__init__.py
+-rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeClient/nuke_client.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeClient/nuke_handler.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeClient/py.typed
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/__init__.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/_logging.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/_version.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/assets.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/data_classes.py
+-rw-r--r--   0        0        0    16082 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/deadline_submitter_for_nuke.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/default_nuke_job_template.yaml
+-rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/job_bundle_output_test_runner.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/py.typed
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_util/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_util/_version.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_util/ocio.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/NOTICE
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/README.md
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/hatch.toml
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/pyproject.toml
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.3/PKG-INFO
```

### Comparing `deadline_cloud_for_nuke-0.18.2/hatch_custom_hook.py` & `deadline_cloud_for_nuke-0.18.3/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/menu.py` & `deadline_cloud_for_nuke-0.18.3/src/menu.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/__main__.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/adaptor.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/schemas/init_data.schema.json` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeAdaptor/schemas/init_data.schema.json`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/nuke_client.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeClient/nuke_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/nuke_handler.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_adaptor/NukeClient/nuke_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/_logging.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/_logging.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/adaptor_override_environment.yaml` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/assets.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/assets.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/data_classes.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/data_classes.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     view_selection: str = field(default="", metadata={"sticky": True})
     is_proxy_mode: bool = field(default=False, metadata={"sticky": True})
 
     input_filenames: list[str] = field(default_factory=list, metadata={"sticky": True})
     input_directories: list[str] = field(default_factory=list, metadata={"sticky": True})
     output_directories: list[str] = field(default_factory=list, metadata={"sticky": True})
 
+    timeouts_enabled: bool = field(default=True, metadata={"sticky": True})
+    on_run_timeout_seconds: int = field(default=518400, metadata={"sticky": True})  # 6 days
+    on_enter_timeout_seconds: int = field(default=86400, metadata={"sticky": True})  # 1 day
+    on_exit_timeout_seconds: int = field(default=3600, metadata={"sticky": True})  # 1 hour
+
     # developer options
     include_adaptor_wheels: bool = field(default=False, metadata={"sticky": True})
 
     def load_sticky_settings(self, scene_filename: str):
         sticky_settings_filename = Path(scene_filename).with_suffix(
             RENDER_SUBMITTER_SETTINGS_FILE_EXT
         )
```

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/deadline_submitter_for_nuke.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/deadline_submitter_for_nuke.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,25 +47,55 @@
     if settings.write_node_selection:
         write_node = nuke.toNode(settings.write_node_selection)
     else:
         write_node = nuke.root()
     return write_node, settings.write_node_selection
 
 
+def _set_timeouts(template: dict[str, Any], settings: RenderSubmitterUISettings) -> None:
+    """
+    Timeouts are an OpenJD field applicable to actions but for specification 2023-09, timeouts must
+    be hard-coded in the job template. There are three types of actions: OnRun, onEnter, and onExit.
+    This function does an in-place modification of timeout values for each action in the template.
+    """
+
+    def _handle_environment(environment: dict):
+        if "script" in environment:
+            actions = environment["script"]["actions"]
+            actions["onEnter"]["timeout"] = settings.on_enter_timeout_seconds
+            if "onExit" in actions:
+                actions["onExit"]["timeout"] = settings.on_exit_timeout_seconds
+
+    def _handle_step(step: dict):
+        for environment in step.get("stepEnvironments", []):
+            _handle_environment(environment)
+
+        step["script"]["actions"]["onRun"]["timeout"] = settings.on_run_timeout_seconds
+
+    for environment in template.get("jobEnvironments", []):
+        _handle_environment(environment)
+
+    for step in template.get("steps", []):
+        _handle_step(step)
+
+
 def _get_job_template(settings: RenderSubmitterUISettings) -> dict[str, Any]:
     # Load the default Nuke job template, and then fill in scene-specific
     # values it needs.
     with open(Path(__file__).parent / "default_nuke_job_template.yaml") as f:
         job_template = yaml.safe_load(f)
 
     # Set the job's name and description
     job_template["name"] = settings.name
     if settings.description:
         job_template["description"] = settings.description
 
+    # Set the timeouts for each action:
+    _set_timeouts(job_template, settings)
+
     # Get a map of the parameter definitions for easier lookup
     parameter_def_map = {param["name"]: param for param in job_template["parameterDefinitions"]}
 
     # Set the WriteNode parameter allowed values
     parameter_def_map["WriteNode"]["allowedValues"].extend(
         sorted(node.fullName() for node in find_all_write_nodes())
     )
@@ -95,20 +125,14 @@
         }:
             raise RuntimeError(
                 "The Developer Option 'Include Adaptor Wheels' is enabled, but the wheels directory contains the wrong wheels:\n"
                 + "Expected: openjd_adaptor_runtime, deadline, and deadline_cloud_for_nuke\n"
                 + f"Actual: {wheels_path_package_names}"
             )
 
-        adaptor_wheels_param = [
-            param
-            for param in override_environment["parameterDefinitions"]
-            if param["name"] == "AdaptorWheels"
-        ][0]
-        adaptor_wheels_param["default"] = str(wheels_path)
         override_adaptor_name_param = [
             param
             for param in override_environment["parameterDefinitions"]
             if param["name"] == "OverrideAdaptorName"
         ][0]
         override_adaptor_name_param["default"] = "NukeAdaptor"
 
@@ -174,14 +198,17 @@
     if settings.view_selection:
         parameter_values.append({"name": "View", "value": settings.view_selection})
 
     # Set the ProxyMode parameter default
     parameter_values.append(
         {"name": "ProxyMode", "value": "true" if settings.is_proxy_mode else "false"}
     )
+    if settings.include_adaptor_wheels:
+        wheels_path = str(Path(__file__).parent.parent.parent.parent / "wheels")
+        parameter_values.append({"name": "AdaptorWheels", "value": wheels_path})
 
     # Check for any overlap between the job parameters we've defined and the
     # queue parameters. This is an error, as we weren't synchronizing the values
     # between the two different tabs where they came from.
     parameter_names = {param["name"] for param in parameter_values}
     queue_parameter_names = {param["name"] for param in queue_parameters}
     parameter_overlap = parameter_names.intersection(queue_parameter_names)
@@ -226,21 +253,14 @@
     # Initialize telemetry client, opt-out is respected
     get_deadline_cloud_library_telemetry_client().update_common_details(
         {
             "deadline-cloud-for-nuke-submitter-version": version,
             "nuke-version": nuke.env["NukeVersionString"],
         }
     )
-    render_settings = RenderSubmitterUISettings()
-
-    # Set the setting defaults that come from the scene
-    render_settings.name = Path(get_nuke_script_file()).name
-    render_settings.frame_list = str(nuke.root().frameRange())
-    render_settings.is_proxy_mode = nuke.root().proxy()
-
     script_path = get_nuke_script_file()
     if not script_path:
         raise DeadlineOperationError(
             "The Nuke Script is not saved to disk. Please save it before opening the submitter dialog."
         )
 
     if nuke.root().modified():
@@ -277,14 +297,28 @@
                 message,
                 QMessageBox.Yes | QMessageBox.No,
                 QMessageBox.No,
             )
             if result == QMessageBox.Yes:
                 nuke.scriptSave()
 
+        if settings.timeouts_enabled:
+            message = "The following timeout value(s) must be greater than 0: \n"
+            zero_timeouts = []
+            if not settings.on_run_timeout_seconds:
+                zero_timeouts.append("Render Timeout")
+            if not settings.on_enter_timeout_seconds:
+                zero_timeouts.append("Setup Timeout")
+            if not settings.on_exit_timeout_seconds:
+                zero_timeouts.append("Teardown Timeout")
+            if zero_timeouts:
+                message += ", ".join(zero_timeouts)
+                message += "\n\nPlease configure these value(s) in the 'Job-Specific Settings' tab."
+                raise DeadlineOperationError(message)
+
         job_bundle_path = Path(job_bundle_dir)
         job_template = _get_job_template(settings)
 
         # If "HostRequirements" is provided, inject it into each of the "Step"
         if host_requirements:
             # for each step in the template, append the same host requirements.
             for step in job_template["steps"]:
```

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/default_nuke_job_template.yaml` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/default_nuke_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/job_bundle_output_test_runner.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_submitter/job_bundle_output_test_runner.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_util/ocio.py` & `deadline_cloud_for_nuke-0.18.3/src/deadline/nuke_util/ocio.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/LICENSE` & `deadline_cloud_for_nuke-0.18.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/README.md` & `deadline_cloud_for_nuke-0.18.3/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/hatch.toml` & `deadline_cloud_for_nuke-0.18.3/hatch.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 lint = [
   "style",
   "typing",
 ]
 
 [[envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11"]
+python = ["3.9", "3.10", "3.11"]
 
 [envs.default.env-vars]
 SKIP_BOOTSTRAP_TEST_RESOURCES="True"
 
 [envs.codebuild.scripts]
 build = "hatch build"
```

### Comparing `deadline_cloud_for_nuke-0.18.2/pyproject.toml` & `deadline_cloud_for_nuke-0.18.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.2/PKG-INFO` & `deadline_cloud_for_nuke-0.18.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-nuke
-Version: 0.18.2
+Version: 0.18.3
 Summary: The submitter and adaptor to enable Nuke support for AWS Deadline Cloud
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-nuke
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-nuke
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

