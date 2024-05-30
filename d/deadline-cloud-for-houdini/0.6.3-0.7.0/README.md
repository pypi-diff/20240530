# Comparing `tmp/deadline_cloud_for_houdini-0.6.3.tar.gz` & `tmp/deadline_cloud_for_houdini-0.7.0.tar.gz`

## Comparing `deadline_cloud_for_houdini-0.6.3.tar` & `deadline_cloud_for_houdini-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/_version.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/HoudiniAdaptor.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/__init__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py
--rw-r--r--   0        0        0    20824 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/_version.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/INDEX__SECTION
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Sections.list
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/houdini.hdalibrary
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/CreateScript
--rw-r--r--   0        0        0    23586 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Help
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/PythonModule
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Sections.list
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/TypePropertiesOptions
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/__init__.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_assets.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_version.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml
--rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py
--rw-r--r--   0        0        0    25079 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/NOTICE
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/hatch.toml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/_version.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniAdaptor/HoudiniAdaptor.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniAdaptor/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py
+-rw-r--r--   0        0        0    20163 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniClient/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/_version.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/INDEX__SECTION
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Sections.list
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/houdini.hdalibrary
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/CreateScript
+-rw-r--r--   0        0        0    27021 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Help
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/PythonModule
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Sections.list
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/TypePropertiesOptions
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/__init__.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_assets.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_version.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py
+-rw-r--r--   0        0        0    27493 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/NOTICE
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/README.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/hatch.toml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.7.0/PKG-INFO
```

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,14 @@
 ]
 _OPTIONAL_HOUDINI_INIT_KEYS = {
     "ignore_input_nodes",
     "wedgenum",
     "wedge_node",
 }
 
-_HOUDINI_RUN_KEYS = {
-    "frame",
-}
-
 
 def _check_for_exception(func: Callable) -> Callable:
     """
     Decorator that checks if an exception has been caught before calling the
     decorated function
     """
 
@@ -87,15 +83,15 @@
     # Variables used for keeping track of produced outputs for progress reporting.
     # Will be optionally changed after the scene is set.
     _expected_outputs: int = 1  # Total number of renders to perform.
     _produced_outputs: int = 0  # Counter for tracking number of complete renders.
 
     @property
     def integration_data_interface_version(self) -> SemanticVersion:
-        return SemanticVersion(major=0, minor=1)
+        return SemanticVersion(major=0, minor=2)
 
     @staticmethod
     def _get_timer(timeout: int | float) -> Callable[[], bool]:
         """
         Given a timeout length, returns a lambda which returns False until the timeout occurs.
 
         Args:
@@ -426,34 +422,19 @@
         This starts a render in Houdini for the given frame, scene and layer(s) and
         performs a busy wait until the render completes.
         """
 
         if not self._houdini_is_running:
             raise HoudiniNotRunningError("Cannot render because Houdini is not running.")
 
-        # frame argument is string type and will fail validation unless we
-        # recast to int
-        # TODO: morgan - Fix this bug
-        run_data["frame"] = int(run_data["frame"])
         self.validators.run_data.validate(run_data)
-        # ERROR: Entrypoint failed:
-        # ERROR: openjd_fail: Error encountered while running adaptor: '1' is not of type 'number'
-        #
-        # Failed validating 'type' in schema['properties']['frame']:
-        #     {'type': 'number'}
-        #
-        # On instance['frame']:
-        #     '1'
         self._is_rendering = True
-
-        for name in _HOUDINI_RUN_KEYS:
-            if name in run_data:
-                self._action_queue.enqueue_action(Action(name, {name: run_data[name]}))
-
-        self._action_queue.enqueue_action(Action("start_render", {"frame": run_data["frame"]}))
+        self._action_queue.enqueue_action(
+            Action("start_render", {"frame_range": run_data["frame_range"]})
+        )
 
         while self._houdini_is_rendering and not self._has_exception:
             time.sleep(0.1)  # busy wait so that on_cleanup is not called
 
         if not self._houdini_is_running and self._houdini_client:  # Client will always exist here.
             #  This is always an error case because the Houdini Client should still be running and
             #  waiting for the next command. If the thread finished, then we cannot continue
```

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     def __init__(self) -> None:
         """
         Constructor for the houdini handler. Initializes action_dict and render variables
         """
         self.action_dict = {
             "scene_file": self.set_scene_file,
             "render_node": self.set_render_node,
-            "frame": self.set_frame,
             "ignore_input_nodes": self.set_ignore_input_nodes,
             "wedge_node": self.set_wedge_node,
             "wedgenum": self.set_wedge_num,
             "start_render": self.start_render,
         }
         self.render_kwargs = {"ignore_input_nodes": True}
         self.node = None
@@ -86,15 +85,15 @@
                         # logging that it was increased
                         # https://www.sidefx.com/docs/houdini/network/parms.html#color
                         print("Increased verbosity to '3' to include basic logging")
                 print(f"Logging verbosity is set to '{verbosity.eval()}'")
 
     def start_render(self, data: dict) -> None:
         """
-        Uses active node and calls hou's render, currently hardcoded to rendering a single frame
+        Uses active node and calls hou's render
 
         Args:
             data (dict):
 
         Raises:
             RuntimeError: .
         """
@@ -118,22 +117,25 @@
                 wl = allwedge[wedgenum]
                 setenvvariable("WEDGENUM", str(wedgenum))
                 print(f"Applying wedge: {wedgenum}")
                 hm.applyspecificwedge(self.wedge, wl)
             else:
                 raise ValueError(f"WEDGENUM out of range: {wedgenum}")
 
-        increment = 1
         self.node.parm("trange").set(1)
-        frame = self.render_kwargs["frame"]
-        frame_range = (frame, frame, increment)
+
         interleave = hou.renderMethod.RopByRop
+
+        start = data["frame_range"]["start"]
+        end = data["frame_range"]["end"]
+        step = data["frame_range"]["step"]
+
         self.node.render(
             verbose=True,
-            frame_range=frame_range,
+            frame_range=(start, end, step),
             ignore_inputs=self.render_kwargs["ignore_input_nodes"],
             method=interleave,
         )
 
         setenvvariable("WEDGENUM", "")
 
         print("Finished Rendering")
@@ -181,24 +183,14 @@
             data (dict):
         """
         wedgenum = data.get("wedgenum", None)
         if wedgenum is not None:
             print(f"wedgenum {wedgenum}")
             self.wedgenum = wedgenum
 
-    def set_frame(self, data: dict) -> None:
-        """
-        Sets the frame to render
-
-        Args:
-            data (dict):
-
-        """
-        self.render_kwargs["frame"] = int(data.get("frame", ""))
-
     def set_scene_file(self, data: dict) -> None:
         """
         Opens the scene file in Houdini.
 
         Args:
             data (dict): The data given from the Adaptor. Keys expected: ['scene_file']
```

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript`

 * *Files 24% similar despite different names*

```diff
@@ -570,56 +570,62 @@
 
             parm {
                 name    "name"
                 label   "Name"
                 type    string
                 default { "$HIPNAME" }
                 parmtag { "script_callback_language" "python" }
+                help    "The job's name. Shown in the Deadline Monitor."
             }
             parm {
                 name    "description"
                 label   "Description"
                 type    string
                 default { "" }
                 parmtag { "script_callback_language" "python" }
+                help    "The job's description. Included in the job template."
             }
             parm {
                 name    "priority"
                 label   "Priority"
                 type    integer
                 default { "50" }
                 range   { 1 100 }
                 parmtag { "script_callback_language" "python" }
+                help    "The job's scheduling priority. The numerically largest priority is scheduled first. See the AWS Deadline Cloud job scheduling documentation for more details."
             }
             parm {
                 name    "initial_status"
                 label   "Initial State"
                 type    ordinal
                 default { "0" }
                 menu {
                     "READY"     "READY"
                     "SUSPENDED" "SUSPENDED"
                 }
                 parmtag { "script_callback_language" "python" }
+                help    "The initial status when the job is created. Jobs that are created with a SUSPENDED status will not run until manually requeued."
             }
             parm {
                 name    "failed_tasks_limit"
                 label   "Failed Tasks Limit"
                 type    integer
                 default { "20" }
                 range   { 0 200 }
                 parmtag { "script_callback_language" "python" }
+                help    "The number of task failures before the job stops running and is marked as FAILED."
             }
             parm {
                 name    "task_retry_limit"
                 label   "Task Retry Limit"
                 type    integer
                 default { "5" }
                 range   { 0 10 }
                 parmtag { "script_callback_language" "python" }
+                help    "The maximum number of retries for each task."
             }
         }
 
         groupsimple {
             name    "folder1"
             label   "Deadline Cloud Settings"
 
@@ -645,132 +651,186 @@
 
         parm {
             name    "separate_steps"
             label   "Submit Dependencies as Separate Steps"
             type    toggle
             default { "1" }
             parmtag { "script_callback_language" "python" }
+            help    "Split the ROP graph into separate rendering steps for easier monitoring and debugging."
         }
         parm {
             name    "include_adaptor_wheels"
             label   "Include Adaptor Wheels"
             type    toggle
             default { "0" }
             parmtag { "script_callback_language" "python" }
+            help    "Adaptor wheels are custom builds of the adaptor that change rendering behavior."
         }
         parm {
             name    "adaptor_wheels"
             label   "Adaptor Wheels"
             type    directory
             default { "" }
             disablewhen "{ include_adaptor_wheels == 0 }"
             parmtag { "script_callback_language" "python" }
+            help    "The directory for adaptor wheels."
         }
         parm {
              name    "auto_unlock_rops"
              label   "Automatically unlock ROPs"
              type    toggle
              default { "0" }
              parmtag { "script_callback_language" "python" }
+             help    "A locked ROP will use existing outputs and won't re-render. It will also block dependencies from re-rendering. Select this option to automatically unlock dependency ROPs."
          }
          parm {
              name    "auto_parse_hip"
-             label   "Automatically parse Hip references"
+             label   "Automatically parse scene (.hip) references"
              type    toggle
              default { "0" }
              parmtag { "script_callback_language" "python" }
+             help    "Automatically discover and attach the job's input and output file names and directories based on the ROP graph during job submission."
          }
          parm {
              name    "auto_save_hip"
-             label   "Automatically save Hip"
+             label   "Automatically save scene (.hip) file"
              type    toggle
              default { "0" }
              parmtag { "script_callback_language" "python" }
+             help    "Automatically save the scene (.hip) file to $HIP when submitting a job."
          }
     }
 
     group {
         name    "job_settings_2"
         label   "Job Attachments"
 
         parm {
             name    "parse_files"
             label   "Parse Files"
             type    button
             default { "0" }
             parmtag { "script_callback" "hou.phm().callback(kwargs)" }
             parmtag { "script_callback_language" "python" }
+            help    "Discover and attach the job's input and output file names and directories based on the current ROP graph."
         }
         multiscroll {
             name    "input_filenames"
             label    "Input Filenames"
 
             parm {
                 name    "input_filenames#"
                 label   "Input File"
                 type    file
                 default { "" }
                 parmtag { "script_callback_language" "python" }
+                help    "Files that will be uploaded as inputs during job submission."
             }
         }
 
         multiscroll {
             name    "input_directories"
             label    "Input Directories"
 
             parm {
                 name    "input_dir#"
                 label   "Input Directory"
                 type    directory
                 default { "" }
                 parmtag { "script_callback_language" "python" }
+                help    "Directories from which all files will be uploaded as inputs during job submission."
             }
         }
 
         multiscroll {
             name    "output_directories"
             label    "Output Directories"
 
             parm {
                 name    "output_dir#"
                 label   "Output Directory"
                 type    directory
                 default { "" }
                 parmtag { "script_callback_language" "python" }
+                help    "Directories that will contain output files when the job is run. This controls what the worker will upload after rendering."
             }
         }
 
+        multiparm {
+            name    "auto_input_filenames"
+            label   "Auto Detected Input Filenames"
+            invisible
+
+            parm {
+                name    "auto_input_filename#"
+                label   "Auto Detected Input Filename"
+                type    file
+                default { "" }
+                invisible
+            }
+        }
+
+        multiparm {
+            name    "auto_input_directories"
+            label   "Auto Detected Input Directories"
+            invisible
+
+            parm {
+                name    "auto_input_directory#"
+                label   "Auto Detected Input Directory"
+                type    directory
+                default { "" }
+                invisible
+            }
+        }
+
+        multiparm {
+            name    "auto_output_directories"
+            label   "Auto Detected Output Directories"
+            invisible
+
+            parm {
+                name    "auto_output_directory#"
+                label   "Auto Detected Output Directory"
+                type    directory
+                default { "" }
+                invisible
+            }
+        }
     }
 
     parm {
         name    "login"
         label   "Login"
         type    button
         joinnext
         default { "0" }
         parmtag { "script_callback" "hou.phm().callback(kwargs)" }
         parmtag { "script_callback_language" "python" }
+        help    "Log in to AWS Deadline Cloud and authenticate for job submission."
     }
     parm {
         name    "logout"
         label   "Logout"
         type    button
         joinnext
         default { "0" }
         parmtag { "script_callback" "hou.phm().callback(kwargs)" }
         parmtag { "script_callback_language" "python" }
+        help    "Log out of AWS Deadline Cloud."
     }
     parm {
         name    "settings"
         label   "Settings"
         type    button
         joinnext
         default { "0" }
         parmtag { "script_callback" "hou.phm().callback(kwargs)" }
         parmtag { "script_callback_language" "python" }
+        help    "Update the AWS Deadline Cloud workstation configuration shared by all tools."
     }
     parm {
         name    "labelparm"
         label   "Label"
         type    label
         nolabel
         joinnext
@@ -780,17 +840,19 @@
         name    "save_bundle"
         label   "Save Bundle"
         type    button
         joinnext
         default { "0" }
         parmtag { "script_callback" "hou.phm().callback(kwargs)" }
         parmtag { "script_callback_language" "python" }
+        help    "Save the current job bundle to disk. Useful for debugging generated jobs without submitting them to AWS Deadline Cloud."
     }
     parm {
         name    "submit"
         label   "Submit"
         type    button
         default { "0" }
         parmtag { "script_callback" "hou.phm().callback(kwargs)" }
         parmtag { "script_callback_language" "python" }
+        help    "Submit the job to AWS Deadline Cloud."
     }
 }
```

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py` & `deadline_cloud_for_houdini-0.7.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
+from enum import Enum
 import os
 import sys
 import yaml
 import json
-from typing import Any
+from typing import Any, Dict
 from pathlib import Path
 
 from deadline.client.job_bundle._yaml import deadline_yaml_dump
 from deadline.client import api
 from deadline.client.job_bundle.submission import AssetReferences
 from deadline.client.job_bundle import create_job_history_bundle_dir
 from deadline.client.job_bundle.parameters import JobParameter
@@ -32,14 +33,19 @@
 import hou
 
 
 _NONE_SELECTED_TEXT = "<none selected>"
 _REFRESHING_TEXT = "<refreshing>"
 
 
+class RenderStrategy(Enum):
+    SEQUENTIAL = "SEQUENTIAL"
+    PARALLEL = "PARALLEL"
+
+
 def _get_houdini_version() -> str:
     return hou.applicationVersionString()
 
 
 def _get_wedge_render_node(node: hou.Node):
     """Return ROP set as input or parameter to a wedge node
 
@@ -53,27 +59,45 @@
             renderpath = rendernode.path()
     if rendernode is None:
         renderpath = node.parm("driver").eval()
         rendernode = node.node(renderpath)
     return rendernode
 
 
-def _get_steps(node: hou.Node):
+def _get_steps(node: hou.Node, separate_steps: int):
     """Convert a network of ROP nodes into a list of steps
 
     Return a list of wedged steps if all the inputs terminate in a valid wedge
     node.
     """
     wedged_steps = _get_wedge_steps(node)
     if wedged_steps is not None:
         # valid wedged network detected
-        return wedged_steps
+        rop_steps = wedged_steps
     else:
         # standard network
-        return _get_rop_steps(node)
+        rop_steps = _get_rop_steps(node)
+
+    if not separate_steps:
+        # render the node connected to the deadline cloud node
+        # and all its input nodes. The opposite of splitting it
+        # up each node by step
+
+        try:
+            connected_node = rop_steps[-1]
+        except IndexError:
+            return []
+
+        # remove deps, as only 1 step
+        connected_node.pop("dependency_names", None)
+        # remove dependency info from name
+        connected_node["name"] = connected_node["rop"]
+        rop_steps = [connected_node]
+
+    return rop_steps
 
 
 def _get_wedge_steps(rop: hou.Node):
     """Convert ancestors of a wedge node into a list of wedged steps"""
     wedge_nodes = []
     # all inputs nodes must be wedge type
     for input_node in rop.inputs():
@@ -160,38 +184,68 @@
         # section after id lists the dependencies between [ ]
         deps: list[str] = []
         for d in rop_parts[1:-2]:
             if d in ["[", "]"]:
                 continue
             # id this depends on
             deps.append(d)
+
+        node = hou.node(path)
+
         # skip deadline and deadline_cloud rops
-        if hou.node(path).type().name() in ("deadline", "deadline_cloud"):
+        if node.type().name() in ("deadline", "deadline_cloud"):
             continue
+
         step_dict = {
             "id": _id,
             "name": f"{path}-{_id}",
             "dependency_ids": deps,
             "rop": path,
             "wedgenum": "",
             "wedge_node": "",
             "start": range_ints[0],
-            "stop": range_ints[1],
+            "end": range_ints[1],
             "step": range_ints[2],
+            "render_strategy": _get_render_strategy_for_node(node),
         }
         rop_steps.append(step_dict)
     # expand full dependency names once the list is complete
     id_steps = {n["id"]: n for n in rop_steps}
     for rop in rop_steps:
         if rop["dependency_ids"]:
             names = [id_steps[n]["name"] for n in rop["dependency_ids"]]
             rop["dependency_names"] = names
     return rop_steps
 
 
+# .
+def _get_render_strategy_for_node(node: hou.Node) -> RenderStrategy:
+    """Any changes to this function should be reflected in the user guide: /docs/user-guide.md"""
+    render_strategy = RenderStrategy.PARALLEL
+
+    if (
+        node.type().nameWithCategory() == "Driver/geometry"
+        and node.parm("initsim")
+        and node.parm("initsim").eval()
+    ):
+        render_strategy = RenderStrategy.SEQUENTIAL
+
+    if node.parm("deadline_cloud_render_strategy"):
+        strategy_string = node.parm("deadline_cloud_render_strategy").evalAsString()
+        if strategy_string.upper() == RenderStrategy.SEQUENTIAL.value:
+            render_strategy = RenderStrategy.SEQUENTIAL
+        elif strategy_string.upper() == RenderStrategy.PARALLEL.value:
+            render_strategy = RenderStrategy.PARALLEL
+        else:
+            raise ValueError(
+                f'The node "{node.path()}" has an unexpected value "{strategy_string}" for its "deadline_cloud_render_strategy" parameter. Ensure the value is {RenderStrategy.PARALLEL.value} or {RenderStrategy.SEQUENTIAL.value}'
+            )
+    return render_strategy
+
+
 def _get_parameter_values(node: hou.Node) -> dict[str, Any]:
     priority = node.parm("priority").eval()
     initial_status = node.parm("initial_status").evalAsString()
     failed_tasks_limit = node.parm("failed_tasks_limit").eval()
     task_retry_limit = node.parm("task_retry_limit").eval()
     parameter_values = [
         {"name": "deadline:priority", "value": priority},
@@ -243,18 +297,17 @@
                 print(f"Failed to unlock: {node_path}")
                 print(str(exc))
                 return False
     return False
 
 
 def _get_job_template(rop: hou.Node) -> dict[str, Any]:
-    job_name = rop.parm("name").evalAsString()
-    job_description = rop.parm("description").evalAsString()
     separate_steps = rop.parm("separate_steps").eval()
-    rop_steps = _get_steps(rop)
+    rop_steps = _get_steps(rop, separate_steps)
+    ignore_input_nodes = bool(separate_steps)
     queue_parameter_definitions_json = rop.userData("queue_parameter_definitions")
     parameter_definitions: list[dict[str, Any]] = (
         json.loads(queue_parameter_definitions_json)
         if queue_parameter_definitions_json is not None
         else []
     )
     parameter_definitions.append(
@@ -263,95 +316,27 @@
             "type": "PATH",
             "objectType": "FILE",
             "dataFlow": "IN",
             "default": _get_hip_file(),
         }
     )
     steps: list[dict[str, Any]] = []
-    ignore_input_nodes = "true"
-    if not separate_steps:
-        # render the node connected to the deadline cloud node
-        # and all its input nodes. The opposite of splitting it
-        # up each node by step
-        connected_node = rop_steps[-1]
-        # remove deps, as only 1 step
-        connected_node.pop("dependency_names", None)
-        # remove dependency info from name
-        connected_node["name"] = connected_node["rop"]
-        rop_steps = [connected_node]
-        ignore_input_nodes = "false"
     for node in rop_steps:
-        # init data
-        init_data_contents = []
-        init_data_contents.append("scene_file: '{{Param.HipFile}}'\n")
-        init_data_contents.append(f"render_node: '{node['rop']}'\n")
-        init_data_contents.append(f"version: {_get_houdini_version()}\n")
-        init_data_contents.append(f"ignore_input_nodes: {ignore_input_nodes}\n")
-        init_data_contents.append(f"wedgenum: '{node['wedgenum']}'\n")
-        init_data_contents.append(f"wedge_node: '{node['wedge_node']}'\n")
-        init_data_attachment = {
-            "name": "initData",
-            "filename": "init-data.yaml",
-            "type": "TEXT",
-            "data": "".join(init_data_contents),
-        }
-        # environments
-        environments = get_houdini_environments(init_data_attachment)
-        # task run data
-        task_data_contents = []
-        task_data_contents.append(f"render_node: {node['rop']}\n")
-        task_data_contents.append("frame: {{Task.Param.Frame}}\n")
-        task_data_contents.append(f"ignore_input_nodes: {ignore_input_nodes}\n")
-        # step
-        frame_range = "{start}-{stop}:{step}".format(**node)
-        step = {
-            "name": node["name"],
-            "parameterSpace": {
-                "taskParameterDefinitions": [{"name": "Frame", "range": frame_range, "type": "INT"}]
-            },
-            "stepEnvironments": environments,
-            "script": {
-                "embeddedFiles": [
-                    {
-                        "name": "runData",
-                        "filename": "run-data.yaml",
-                        "type": "TEXT",
-                        "data": "".join(task_data_contents),
-                    },
-                ],
-                "actions": {
-                    "onRun": {
-                        "command": "houdini-openjd",
-                        "args": [
-                            "daemon",
-                            "run",
-                            "--connection-file",
-                            "{{ Session.WorkingDirectory }}/connection.json",
-                            "--run-data",
-                            "file://{{ Task.File.runData }}",
-                        ],
-                        "cancelation": {
-                            "mode": "NOTIFY_THEN_TERMINATE",
-                        },
-                    },
-                },
-            },
-        }
-        if "dependency_names" in node:
-            deps = [{"dependsOn": d} for d in node["dependency_names"]]
-            step["dependencies"] = deps
-        steps.append(step)
+        steps.append(_get_step_template(node, ignore_input_nodes))
     job_template = {
         "specificationVersion": "jobtemplate-2023-09",
-        "name": job_name,
+        "name": rop.parm("name").evalAsString(),
         "parameterDefinitions": parameter_definitions,
         "steps": steps,
     }
-    if job_description:
-        job_template["description"] = job_description
+
+    description = rop.parm("description").evalAsString()
+    if description:
+        job_template["description"] = description
+
     include_adaptor_wheels = rop.parm("include_adaptor_wheels").eval()
     if include_adaptor_wheels:
         adaptor_wheels = rop.parm("adaptor_wheels").evalAsString()
         if os.path.exists(adaptor_wheels):
             override_file = os.path.join(
                 os.path.dirname(__file__), "adaptor_override_environment.yaml"
             )
@@ -359,17 +344,105 @@
                 override_environment = yaml.safe_load(yaml_file)
                 job_template["parameterDefinitions"].extend(
                     override_environment["parameterDefinitions"]
                 )
                 if "jobEnvironments" not in job_template:
                     job_template["jobEnvironments"] = []
                 job_template["jobEnvironments"].append(override_environment["environment"])
+
     return job_template
 
 
+def _get_step_template(node: Dict, ignore_input_nodes: bool):
+    init_data = {
+        "scene_file": "{{Param.HipFile}}",
+        "render_node": node["rop"],
+        "version": _get_houdini_version(),
+        "ignore_input_nodes": ignore_input_nodes,
+        "wedgenum": node["wedgenum"],
+        "wedge_node": node["wedge_node"],
+    }
+    init_data_attachment = {
+        "name": "initData",
+        "filename": "init-data.yaml",
+        "type": "TEXT",
+        # Convert to dict to YAML string using the prettier nested object format
+        "data": yaml.safe_dump(init_data, default_flow_style=False),
+    }
+
+    environments = get_houdini_environments(init_data_attachment)
+
+    task_data_dict = {"render_node": node["rop"], "ignore_input_nodes": ignore_input_nodes}
+
+    if node["render_strategy"] == RenderStrategy.SEQUENTIAL:
+        # Generate a single task that renders the whole frame range
+        parameter_space = None
+        task_data_dict["frame_range"] = {
+            "start": node["start"],
+            "end": node["end"],
+            "step": node["step"],
+        }
+    else:
+        # Generate one task per frame using step parameters
+        range_expression = "{start}-{end}:{step}".format(**node)
+        parameter_space = {
+            "taskParameterDefinitions": [
+                {"name": "Frame", "range": range_expression, "type": "INT"}
+            ]
+        }
+        task_data_dict["frame_range"] = {
+            "start": "{{Task.Param.Frame}}",
+            "end": "{{Task.Param.Frame}}",
+            "step": 1,
+        }
+
+    task_data = yaml.safe_dump(task_data_dict, default_flow_style=False)
+    # Remove single quotes around the frame parameter so it gets interpreted as a int and not a string
+    task_data = task_data.replace("'{{Task.Param.Frame}}'", "{{Task.Param.Frame}}")
+
+    step = {
+        "name": node["name"],
+        "stepEnvironments": environments,
+        "script": {
+            "embeddedFiles": [
+                {
+                    "name": "runData",
+                    "filename": "run-data.yaml",
+                    "type": "TEXT",
+                    "data": task_data,
+                },
+            ],
+            "actions": {
+                "onRun": {
+                    "command": "houdini-openjd",
+                    "args": [
+                        "daemon",
+                        "run",
+                        "--connection-file",
+                        "{{ Session.WorkingDirectory }}/connection.json",
+                        "--run-data",
+                        "file://{{ Task.File.runData }}",
+                    ],
+                    "cancelation": {
+                        "mode": "NOTIFY_THEN_TERMINATE",
+                    },
+                },
+            },
+        },
+    }
+
+    if parameter_space:
+        step["parameterSpace"] = parameter_space
+
+    if "dependency_names" in node:
+        deps = [{"dependsOn": d} for d in node["dependency_names"]]
+        step["dependencies"] = deps
+    return step
+
+
 def _create_job_bundle(
     rop_node: hou.Node, job_bundle_dir: str, asset_references: AssetReferences
 ) -> None:
     job_bundle_path = Path(job_bundle_dir)
     job_template = _get_job_template(rop_node)
     parameter_values = _get_parameter_values(rop_node)
     with open(job_bundle_path / "template.yaml", "w", encoding="utf8") as f:
@@ -575,26 +648,39 @@
         asset_manager = S3AssetManager(
             farm_id=farm_id,
             queue_id=queue_id,
             job_attachment_settings=JobAttachmentS3Settings(**queue["jobAttachmentSettings"]),
             session=queue_role_session,
         )
 
+        api.get_deadline_cloud_library_telemetry_client().record_event(
+            event_type="com.amazon.rum.deadline.submission",
+            event_details={
+                "submitter_name": "Houdini",
+            },
+            from_gui=True,
+        )
+
         job_progress_dialog = SubmitJobProgressDialog(parent=hou.qt.mainWindow())
         job_progress_dialog.start_submission(
             farm_id,
             queue_id,
             storage_profile,
             job_bundle_dir,
             queue_parameters,
             asset_manager,
             deadline,
             auto_accept=str2bool(get_setting("settings.auto_accept")),
         )
     except Exception as exc:
+        api.get_deadline_cloud_library_telemetry_client().record_error(
+            event_details={"exception_scope": "submit_callback"},
+            exception_type=str(type(exc)),
+            from_gui=True,
+        )
         print(str(exc))
         hou.ui.displayMessage(
             str(exc), title="Houdini Job Submission", severity=hou.severityType.Warning
         )
 
 
 def settings_callback(kwargs):
```

### Comparing `deadline_cloud_for_houdini-0.6.3/LICENSE` & `deadline_cloud_for_houdini-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/README.md` & `deadline_cloud_for_houdini-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/hatch.toml` & `deadline_cloud_for_houdini-0.7.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/pyproject.toml` & `deadline_cloud_for_houdini-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.3/PKG-INFO` & `deadline_cloud_for_houdini-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-houdini
-Version: 0.6.3
+Version: 0.7.0
 Summary: AWS Deadline Cloud for Houdini
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-houdini
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-houdini
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

