# Comparing `tmp/scenebuilder-0.2.3.tar.gz` & `tmp/scenebuilder-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenebuilder-0.2.3.tar", max compression
+gzip compressed data, was "scenebuilder-0.2.4.tar", max compression
```

## Comparing `scenebuilder-0.2.3.tar` & `scenebuilder-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4205 2024-05-15 14:52:52.630508 scenebuilder-0.2.3/README.md
--rw-r--r--   0        0        0      486 2024-05-22 16:08:54.996188 scenebuilder-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       51 2024-05-22 15:35:02.149125 scenebuilder-0.2.3/scenebuilder/__init__.py
--rw-r--r--   0        0        0     1019 2024-05-22 13:02:21.441055 scenebuilder-0.2.3/scenebuilder/actions_stack.py
--rw-r--r--   0        0        0     5118 2024-05-22 13:02:22.513522 scenebuilder-0.2.3/scenebuilder/entities.py
--rw-r--r--   0        0        0      832 2024-05-22 13:02:23.030691 scenebuilder-0.2.3/scenebuilder/main.py
--rw-r--r--   0        0        0      454 2024-05-22 13:02:23.481805 scenebuilder-0.2.3/scenebuilder/mixins.py
--rw-r--r--   0        0        0     2196 2024-05-22 13:02:24.814981 scenebuilder-0.2.3/scenebuilder/observer_utils.py
--rw-r--r--   0        0        0     4231 2024-05-22 13:02:25.370139 scenebuilder-0.2.3/scenebuilder/patch_manager.py
--rw-r--r--   0        0        0     4345 2024-05-22 13:02:25.870949 scenebuilder-0.2.3/scenebuilder/patches.py
--rw-r--r--   0        0        0    26209 2024-05-22 15:58:44.899612 scenebuilder-0.2.3/scenebuilder/scenebuilder.py
--rw-r--r--   0        0        0     7164 2024-05-22 13:02:27.289875 scenebuilder-0.2.3/scenebuilder/ui_components.py
--rw-r--r--   0        0        0     7785 2024-05-22 13:02:27.792935 scenebuilder-0.2.3/scenebuilder/utils.py
--rw-r--r--   0        0        0     4785 1970-01-01 00:00:00.000000 scenebuilder-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     4205 2024-05-15 14:52:52.630508 scenebuilder-0.2.4/README.md
+-rw-r--r--   0        0        0      486 2024-05-30 13:33:51.845159 scenebuilder-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-22 16:18:34.788995 scenebuilder-0.2.4/scenebuilder/__init__.py
+-rw-r--r--   0        0        0     1019 2024-05-22 13:02:21.441055 scenebuilder-0.2.4/scenebuilder/actions_stack.py
+-rw-r--r--   0        0        0     5118 2024-05-22 13:02:22.513522 scenebuilder-0.2.4/scenebuilder/entities.py
+-rw-r--r--   0        0        0     1085 2024-05-30 13:48:51.824240 scenebuilder-0.2.4/scenebuilder/main.py
+-rw-r--r--   0        0        0      454 2024-05-22 13:02:23.481805 scenebuilder-0.2.4/scenebuilder/mixins.py
+-rw-r--r--   0        0        0     2196 2024-05-22 13:02:24.814981 scenebuilder-0.2.4/scenebuilder/observer_utils.py
+-rw-r--r--   0        0        0     4231 2024-05-22 13:02:25.370139 scenebuilder-0.2.4/scenebuilder/patch_manager.py
+-rw-r--r--   0        0        0     4345 2024-05-22 13:02:25.870949 scenebuilder-0.2.4/scenebuilder/patches.py
+-rw-r--r--   0        0        0    26266 2024-05-30 13:37:37.140539 scenebuilder-0.2.4/scenebuilder/scenebuilder.py
+-rw-r--r--   0        0        0     7164 2024-05-22 13:02:27.289875 scenebuilder-0.2.4/scenebuilder/ui_components.py
+-rw-r--r--   0        0        0     7785 2024-05-22 13:02:27.792935 scenebuilder-0.2.4/scenebuilder/utils.py
+-rw-r--r--   0        0        0     4785 1970-01-01 00:00:00.000000 scenebuilder-0.2.4/PKG-INFO
```

### Comparing `scenebuilder-0.2.3/README.md` & `scenebuilder-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.3/scenebuilder/actions_stack.py` & `scenebuilder-0.2.4/scenebuilder/actions_stack.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.3/scenebuilder/entities.py` & `scenebuilder-0.2.4/scenebuilder/entities.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.3/scenebuilder/main.py` & `scenebuilder-0.2.4/scenebuilder/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,32 @@
     parser.add_argument(
         "-l",
         "--load",
         type=str,
         help="Load a scene from a JSON file at the specified path",
     )
 
+    parser.add_argument(
+        "-s",
+        "--sidelength",
+        type=int,
+        help="Specify new arena sidelength in meters, eg: scenebuilder -s 10",
+    )
+
     args = parser.parse_args()
 
     app = SceneBuilder()
 
     loaded_file = None
     if args.load:
         app.load_scene(args.load)
         loaded_file = args.load
+    if args.sidelength:
+        l = args.sidelength
+        app.set_lims((-l/2, l/2))
 
     intro_message = (
         "Welcome to the SceneBuilder! \n"
         "This is a tool for creating and editing a 2D scene with drones and buildings."
     )
     if loaded_file:
         intro_message += f"\nLoaded scene from file: {loaded_file}"
```

### Comparing `scenebuilder-0.2.3/scenebuilder/observer_utils.py` & `scenebuilder-0.2.4/scenebuilder/observer_utils.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.3/scenebuilder/patch_manager.py` & `scenebuilder-0.2.4/scenebuilder/patch_manager.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.3/scenebuilder/patches.py` & `scenebuilder-0.2.4/scenebuilder/patches.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.3/scenebuilder/scenebuilder.py` & `scenebuilder-0.2.4/scenebuilder/scenebuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,18 @@
             self.patch_manager.add_drone_patch(drone)
         self._update()
 
     def draw_scene(self):
         """Draw the scene."""
         plt.show()
 
+    def set_lims(self, new_lims:tuple):
+        self.ax.set_xlim(new_lims)
+        self.ax.set_ylim(new_lims)
+
     def _plot_setup(self):
         fig = plt.figure(figsize=self.FIG_SIZE)
         ax = fig.add_subplot(111)
 
         fig.subplots_adjust(bottom=0.1, top=0.85)
 
         ax.set_xlim(self.AXIS_LIMITS)
@@ -357,16 +361,14 @@
         The event object contains information about the click, such as its position.
         You can use this information to add new elements to the plot, such as a new building or a new drone.
         #NOTE ORDER MATTERS, events will be handled in the order they are listed in this method"""
         # If clicked outside of the plot, do nothing
         # if not event.xdata or not event.ydata:
         #     return
         if event.inaxes != self.ax:
-            import sys
-            print(sys.version)
             return
 
         # handle moving building vertices
         if self._handle_vertex_movement(event):
             return
 
         # add a new vertex if near a building edge and allow moving it around with the mouse...
```

### Comparing `scenebuilder-0.2.3/scenebuilder/ui_components.py` & `scenebuilder-0.2.4/scenebuilder/ui_components.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.3/scenebuilder/utils.py` & `scenebuilder-0.2.4/scenebuilder/utils.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.3/PKG-INFO` & `scenebuilder-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenebuilder
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple GUI to create 2D scenes with obstacles and drone paths for multi-agent path planning algorithms
 Author: Adrian del Ser
 Author-email: adrian.delser@gmail.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

