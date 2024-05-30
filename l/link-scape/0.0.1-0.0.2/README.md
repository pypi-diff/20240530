# Comparing `tmp/link_scape-0.0.1.tar.gz` & `tmp/link_scape-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "link_scape-0.0.1.tar", last modified: Thu May 30 10:43:32 2024, max compression
+gzip compressed data, was "link_scape-0.0.2.tar", last modified: Thu May 30 11:14:55 2024, max compression
```

## Comparing `link_scape-0.0.1.tar` & `link_scape-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:32.605659 link_scape-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 10:43:25.000000 link_scape-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 10:43:25.000000 link_scape-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 10:43:32.605659 link_scape-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:32.605659 link_scape-0.0.1/link_scape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 10:43:32.000000 link_scape-0.0.1/link_scape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-30 10:43:32.000000 link_scape-0.0.1/link_scape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:43:32.000000 link_scape-0.0.1/link_scape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 10:43:32.000000 link_scape-0.0.1/link_scape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:32.605659 link_scape-0.0.1/linkscape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:25.000000 link_scape-0.0.1/linkscape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-30 10:43:25.000000 link_scape-0.0.1/linkscape/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-30 10:43:25.000000 link_scape-0.0.1/linkscape/template.html
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:43:32.605659 link_scape-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 10:43:25.000000 link_scape-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:14:55.554955 link_scape-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 11:14:43.000000 link_scape-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 11:14:43.000000 link_scape-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-30 11:14:55.554955 link_scape-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:14:55.554955 link_scape-0.0.2/link_scape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-30 11:14:55.000000 link_scape-0.0.2/link_scape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-30 11:14:55.000000 link_scape-0.0.2/link_scape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:14:55.000000 link_scape-0.0.2/link_scape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 11:14:55.000000 link_scape-0.0.2/link_scape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:14:55.554955 link_scape-0.0.2/linkscape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:14:43.000000 link_scape-0.0.2/linkscape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-30 11:14:43.000000 link_scape-0.0.2/linkscape/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8903 2024-05-30 11:14:43.000000 link_scape-0.0.2/linkscape/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:14:55.554955 link_scape-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 11:14:43.000000 link_scape-0.0.2/setup.py
```

### Comparing `link_scape-0.0.1/LICENSE` & `link_scape-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `link_scape-0.0.1/PKG-INFO` & `link_scape-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: link-scape
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to plot force-directed graphs.
 Home-page: https://github.com/aloneguid/linkscape
 Author: Ivan Gavryliuk
 Author-email: ifs5vh19k@mozmail.com
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LinkScape
 
+[![PyPI - Version](https://img.shields.io/pypi/v/link-scape?style=flat-square&label=pypi%20%7C%20link-scape)](https://pypi.org/project/link-scape/)
+
+
 <img src="logo.jpg" width="150px" alt="ai-generated logo">
 
 Python network visualisation library I have created for visualising data when performing reverse engineering tasks.
 
 ## Features
 - Network parameters:
   - Collision radius.
@@ -30,9 +33,19 @@
 - Edge customization
   - Color.
   - Opacity.
   - Width.
   - Label.
   - Custom force.
 
+## Installation
+
+To install the library,
+
+```bash
+pip install link-scape
+```
+
+## Documentation
+
 You can browse documentation and examples in [this Jupyter notebook](https://nbviewer.jupyter.org/github/aloneguid/linkscape/tree/master/examples/).
```

### Comparing `link_scape-0.0.1/link_scape.egg-info/PKG-INFO` & `link_scape-0.0.2/link_scape.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: link-scape
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to plot force-directed graphs.
 Home-page: https://github.com/aloneguid/linkscape
 Author: Ivan Gavryliuk
 Author-email: ifs5vh19k@mozmail.com
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LinkScape
 
+[![PyPI - Version](https://img.shields.io/pypi/v/link-scape?style=flat-square&label=pypi%20%7C%20link-scape)](https://pypi.org/project/link-scape/)
+
+
 <img src="logo.jpg" width="150px" alt="ai-generated logo">
 
 Python network visualisation library I have created for visualising data when performing reverse engineering tasks.
 
 ## Features
 - Network parameters:
   - Collision radius.
@@ -30,9 +33,19 @@
 - Edge customization
   - Color.
   - Opacity.
   - Width.
   - Label.
   - Custom force.
 
+## Installation
+
+To install the library,
+
+```bash
+pip install link-scape
+```
+
+## Documentation
+
 You can browse documentation and examples in [this Jupyter notebook](https://nbviewer.jupyter.org/github/aloneguid/linkscape/tree/master/examples/).
```

### Comparing `link_scape-0.0.1/linkscape/network.py` & `link_scape-0.0.2/linkscape/network.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import json
 from typing import List
 import base64
 
 
 class Node:
     def __init__(self,
-                 id: str,
+                 node_id: str,
                  label: str = None,
                  tooltip: str = None,
                  color: str = "#57C7E3", level: int = None,
                  radius: int = 18,
                  stroke_color: str = "#23B3D7",
                  stroke_width: int = 2):
-        self.id = id
+        self.node_id = node_id
         self.label = label
         self.tooltip = tooltip or label
         self.color = color
         self.level = level
         self.radius = radius
         self.stroke_color = stroke_color
         self.stroke_width = stroke_width
@@ -26,15 +26,15 @@
 class Edge:
     def __init__(self, source: str, target: str,
                  label: str = None,
                  color: str = "#94B3CC",
                  opacity: float = 1.0,
                  width: float = 1,
                  force: float = None):
-        self.id = 0
+        self.edge_id = 0
         self.label = label
         self.source = source
         self.target = target
         self.color = color
         self.opacity = opacity
         self.width = width
         self.force = force
@@ -59,59 +59,89 @@
         self._html = (self._html
                       .replace("$width", str(width))
                       .replace("$height", str(height))
                       .replace("$x_levels", str(x_levels))
                       .replace("$collision_radius", str(collision_radius))
                       .replace("$linkType", link_type)
                       .replace("$showArrows", "true" if show_arrows else "false")
-                      .replace("$nodeFontFamily", node_label_font_family)
-                      .replace("$nodeFontSize", node_label_font_size)
-                      .replace("$nodeFontColor", node_label_color)
-                      .replace("$linkFontFamily", link_label_font_family)
-                      .replace("$linkFontSize", link_label_font_size)
-                      .replace("$linkFontColor", link_label_color)
-                      .replace("$linkForce", str(link_force))
-                      .replace("$backgroundColor", background_color))
+                      .replace("$linkForce", str(link_force)))
+        self._generate_styles(node_label_font_family, node_label_font_size, node_label_color,
+                              link_label_font_family, link_label_font_size, link_label_color,
+                              background_color)
         self._width = width
         self._height = height
         self.show_arrows = show_arrows
 
         self._nodes: List[Node] = []
         self._edges: List[Edge] = []
 
         self._edge_id_i = 0
 
-    def node(self, node_id: str) -> Node:
-        n = Node(node_id)
+    def _generate_styles(self,
+                         node_label_font_family: str,
+                         node_label_font_size: str,
+                         node_label_color: str,
+                         link_label_font_family: str,
+                         link_label_font_size: str,
+                         link_label_color: str,
+                         background_color: str) -> None:
+        self._html = self._html.replace("<head></head>", f"""<head>
+    <style>
+        .node-label {{
+            font-family: "{node_label_font_family}";
+                font-size: {node_label_font_size};
+                fill: {node_label_color}
+            }}
+
+        .link-label {{
+            font-family: "{link_label_font_family}";
+            font-size: {link_label_font_size};
+            fill: {link_label_color};
+        }}
+
+        svg {{
+            background-color: {background_color};
+        }}
+    </style>
+</head>""")
+
+    def node(self, node_id: str, label: str | None = None) -> Node:
+        """
+        Create a new node and add it to the network.
+        :param label:
+        :param node_id:
+        :return:
+        """
+        n = Node(node_id, label)
         self._nodes.append(n)
         return n
 
     def edge(self, source_id: str, target_id: str) -> Edge:
         edge = Edge(source_id, target_id)
-        edge.id = self._edge_id_i
+        edge.edge_id = self._edge_id_i
         self._edge_id_i += 1
         self._edges.append(edge)
         return edge
 
     def _render_data(self) -> str:
         r = self._html
 
         nodes = [{
-            "id": n.id,
+            "id": n.node_id,
             "label": n.label,
             "tooltip": n.tooltip,
             "color": n.color,
             "level": n.level,
             "radius": n.radius,
             "stroke": n.stroke_color,
             "stroke_width": n.stroke_width
         } for n in self._nodes]
 
         links = [{
-            "id": l.id,
+            "id": l.edge_id,
             "label": l.label,
             "source": l.source,
             "target": l.target,
             "color": l.color,
             "opacity": l.opacity,
             "width": l.width,
             "force": l.force
@@ -127,12 +157,10 @@
 
     def _repr_html_(self):
         data = self._render_data()
         b64data = base64.b64encode(data.encode("utf-8")).decode("utf-8")
         url = f"data:text/html;charset=utf-8;base64,{b64data}"
         return f"<iframe src=\"{url}\" width=\"{self._width}\" height=\"{self._height}\" scrolling=\"no\" style=\"border:none !important;\"></iframe>"
 
-
-
     def save(self, path: str) -> None:
         with open(path, "w") as writer:
             writer.write(self._render_data())
```

### Comparing `link_scape-0.0.1/linkscape/template.html` & `link_scape-0.0.2/linkscape/template.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,9 @@
 <!DOCTYPE html>
-<head>
-    <style>
-        .node-label {
-            font-family: "$nodeFontFamily";
-            font-size: $nodeFontSize;
-            fill: $nodeFontColor;
-        }
-
-        .link-label {
-            font-family: "$linkFontFamily";
-            font-size: $linkFontSize;
-            fill: $linkFontColor;
-        }
-
-        svg {
-            background-color: $backgroundColor;
-        }
-    </style>
-</head>
+<head></head>
 <body>
     <script type="module">
 
         import * as d3 from "https://cdn.jsdelivr.net/npm/d3@7/+esm";
 
         const data_nodes = $data_nodes;
         const data_links = $data_links;
@@ -261,12 +243,10 @@
             if(linkType === "arc") {
                 return "M" + sourceX + "," + sourceY + "A" + dr + "," + dr + " 0 0,1 " + targetX + "," + targetY;
             } else {
                 return `M ${sourceX} ${sourceY} L ${targetX} ${targetY}`
             }
 
         }
-
-
     </script>
 </body>
 </html>
```

### Comparing `link_scape-0.0.1/setup.py` & `link_scape-0.0.2/setup.py`

 * *Files identical despite different names*

