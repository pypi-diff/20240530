# Comparing `tmp/streamlit_pyvista-0.0.5.tar.gz` & `tmp/streamlit_pyvista-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_pyvista-0.0.5.tar", max compression
+gzip compressed data, was "streamlit_pyvista-0.0.6.tar", max compression
```

## Comparing `streamlit_pyvista-0.0.5.tar` & `streamlit_pyvista-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,16 @@
--rw-r--r--   0        0        0      104 2024-04-16 16:04:25.476831 streamlit_pyvista-0.0.5/README.md
--rw-r--r--   0        0        0      659 2024-04-16 16:04:31.117806 streamlit_pyvista-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6070 2024-04-16 16:04:25.478831 streamlit_pyvista-0.0.5/streamlit_pyvista/MeshViewerComponent.py
--rw-r--r--   0        0        0       89 2024-04-16 16:04:25.478831 streamlit_pyvista-0.0.5/streamlit_pyvista/__init__.py
--rw-r--r--   0        0        0    24891 2024-04-16 16:04:25.478831 streamlit_pyvista-0.0.5/streamlit_pyvista/trame_viewer.py
--rw-r--r--   0        0        0      208 2024-04-16 16:04:25.478831 streamlit_pyvista-0.0.5/streamlit_pyvista/utils.py
--rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 streamlit_pyvista-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-05-30 15:06:23.796502 streamlit_pyvista-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2392 2024-05-30 15:06:23.796502 streamlit_pyvista-0.0.6/README.md
+-rw-r--r--   0        0        0      955 2024-05-30 15:06:29.764482 streamlit_pyvista-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8725 2024-05-30 15:06:23.804502 streamlit_pyvista-0.0.6/streamlit_pyvista/MeshViewerComponent.py
+-rw-r--r--   0        0        0     5066 2024-05-30 15:06:23.805502 streamlit_pyvista-0.0.6/streamlit_pyvista/Proxy.py
+-rw-r--r--   0        0        0    16882 2024-05-30 15:06:23.805502 streamlit_pyvista-0.0.6/streamlit_pyvista/TrameAdvancedViewer.py
+-rw-r--r--   0        0        0    13352 2024-05-30 15:06:23.805502 streamlit_pyvista-0.0.6/streamlit_pyvista/TrameViewer.py
+-rw-r--r--   0        0        0       73 2024-05-30 15:06:23.805502 streamlit_pyvista-0.0.6/streamlit_pyvista/__init__.py
+-rw-r--r--   0        0        0     7431 2024-05-30 15:06:23.805502 streamlit_pyvista-0.0.6/streamlit_pyvista/server_managers/ServerManager.py
+-rw-r--r--   0        0        0     6304 2024-05-30 15:06:23.805502 streamlit_pyvista-0.0.6/streamlit_pyvista/server_managers/ServerManagerProxified.py
+-rw-r--r--   0        0        0     1483 2024-05-30 15:06:23.805502 streamlit_pyvista-0.0.6/streamlit_pyvista/server_managers/ServerMessageInterface.py
+-rw-r--r--   0        0        0      146 2024-05-30 15:06:23.805502 streamlit_pyvista-0.0.6/streamlit_pyvista/server_managers/__init__.py
+-rw-r--r--   0        0        0    28282 2024-05-30 15:06:23.806502 streamlit_pyvista-0.0.6/streamlit_pyvista/trame_viewer.py
+-rw-r--r--   0        0        0    11497 2024-05-30 15:06:23.806502 streamlit_pyvista-0.0.6/streamlit_pyvista/utils.py
+-rw-r--r--   0        0        0    13312 2024-05-30 15:06:23.806502 streamlit_pyvista-0.0.6/streamlit_pyvista/viewer.py
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 streamlit_pyvista-0.0.6/PKG-INFO
```

### Comparing `streamlit_pyvista-0.0.5/pyproject.toml` & `streamlit_pyvista-0.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 [tool.poetry]
 name = "streamlit-pyvista"
-version = "0.0.5"
-description = ""
+version = "0.0.6"
+description = "A Streamlit component that allow support for new PyVista viewer backend: Trame."
+license = "GPL-3.0-or-later"
+homepage = "https://gitlab.com/groups/dcsm"
+repository = "https://gitlab.com/dcsm/streamlit-pyvista"
 authors = ["Maxime Rochat <rochat.max@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.12"
 aiohttp = "^3.9.3"
 pyvista = "^0.43.3"
@@ -15,14 +18,19 @@
 trame-plotly = "^3.0.2"
 trame-server = "^2.17.2"
 trame-vtk = "^2.8.5"
 trame-vuetify = "^2.4.2"
 protobuf="<=4.25.3"
 pytest = ">=7.2.1"
 requests = "^2.29.0"
+validators = "^0.28.0"
+Flask = "^3.0.3"
+APScheduler = "^3.10.4"
+flask-sock = "^0.7.0"
+
 
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `streamlit_pyvista-0.0.5/streamlit_pyvista/MeshViewerComponent.py` & `streamlit_pyvista-0.0.6/streamlit_pyvista/server_managers/ServerManagerProxified.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,153 +1,142 @@
-import os
-import time
+import threading
+import subprocess
 import logging
-
-import streamlit.components.v1 as components
-import requests
 import json
-import subprocess
-import threading
-
+import base64
+import hashlib
+import ipaddress
 
+import requests
+from flask import Flask, request, make_response
+from flask_sock import Sock
 
-from .utils import is_localhost
+import os
+from streamlit_pyvista import ROOT_URL
+from streamlit_pyvista.server_managers.ServerManager import ServerManagerBase
+from streamlit_pyvista.utils import (find_free_port, is_server_available, is_server_alive,
+                                                     wait_for_server_alive, ServerItem)
+from streamlit_pyvista.server_managers.ServerMessageInterface import ServerMessageInterface, EndpointsInterface
 
-root_logger = logging.getLogger("solidipes")
+root_logger = logging.getLogger("streamlit-server-manager")
 root_logger.propagate = True
-root_logger.setLevel(logging.DEBUG)
-if "FULL_SOLIDIPES_LOG" not in os.environ:
-    root_logger.setLevel(logging.INFO)
-
-
-class MeshViewerComponent:
-    """Streamlit component to display 3d mesh using pyvista and it's Trame backend"""
-
-    def __init__(self, mesh_path: str = None, sequence_size=1, server_url="http://127.0.0.1:8080",
-                 setup_endpoint="/init_connection"):
-
-        # Transform the path given as arg to a absolute path to be able to pass it to the server without trouble
-        if not os.path.isabs(mesh_path):
-            mesh_path = os.getcwd() + "/" + mesh_path
-
-        # Set class attributes and check that files given as input exist all
-        self.check_valid_input_files(mesh_path, sequence_size)
-
-        self.mesh_path = mesh_path
-        self.sequence_size = sequence_size
-
-        self.width = 1200
-        self.height = 900
-
-        self.server_url = server_url
-        self.server_timeout = 2
-        self.max_retries = 3
-
-        # Set all attribute related to the dynamic endpoints settings.
-        # Set the default required endpoints,
-        # select mesh is used to ask the server to show a specific mesh and host is the host of the data rendering
-        self.required_endpoints = ["select_mesh", "host"]
-        # Dict that will contained value received for our endpoints. Init connection is the default endpoint to
-        # request the server to give use all it's required endpoints
-        self.endpoints = {
-            "init_connection": setup_endpoint,
-            "host":self.server_url
-        }
-        # If the default server url is on localhost we launch the server locally
-        if is_localhost(self.server_url):
-            self.setup_server()
-
-        # Set up the endpoints
-        self.setup_endpoints()
-
-        self.set_mesh()
-        root_logger.info("MeshViewer Created")
-
-
-    def check_valid_input_files(self, path, sequence_size=1):
-        """ Take a path and a sequence_size and check that each file of the sequence exists.
-        If it does not it outputs an error message """
-        if sequence_size != 1:
-            for i in range(sequence_size):
-                tmp_path = path % i
-                if not os.path.exists(tmp_path):
-                    root_logger.error(f"The file '{tmp_path}' does not exist.")
-        elif not os.path.exists(path):
-            root_logger.error(f"The file '{path}' does not exist.")
+root_logger.setLevel(logging.INFO)
 
 
-    def is_server_alive(self, server):
-        """ Try to make a request to the server and see if it responds to determine if he is alive """
+def run_trame_viewer(server_port, file_path):
+    """ Launch a Trame server using python subprocess """
+    try:
+        print(os.listdir())
+        print(os.getcwd())
+        
+        print(f"Trying to start {file_path} on port {server_port}")
+        subprocess.run(["python", file_path,
+                        "--server", "--port", str(server_port)],
+                       # stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL,
+                       check=True)  # stdout=subprocess.DEVNULL,  stderr=subprocess.DEVNULL,
+    except subprocess.CalledProcessError as e:
+        print("An error occured")
+
+
+class ServerManagerProxyfied(ServerManagerBase):
+    """ Implementation of ServerManagerBase that make use of a proxy for remote connection """
+    def __init__(self, host="0.0.0.0", port=8080, proxy_host="127.0.0.1", proxy_port=5000):
+        super().__init__(host, port)
+
+        self.proxy_host = proxy_host
+        self.proxy_port = proxy_port
+        self.base_url = ROOT_URL
+
+    def init_connection(self):
+        print("REQUEST FOR INIT CO", request.url)
+    
+        self.proxy_host = request.headers.get("Host").split(":")
+        if len(self.proxy_host) > 1:
+            self.proxy_host[1] = str(self.proxy_port)
+            self.proxy_host = ":".join(self.proxy_host) 
+        else:
+            self.proxy_host = self.proxy_host[0]     
+        print("Pass Header", self.proxy_host)
+        if request.is_json:
+            req = json.loads(request.json)
+        else:
+            return make_response({"Invalid format": "init_connection expected a json with field 'Viewer' "})
+        print("Pass Json fecth")
+        file_content = req.get(ServerMessageInterface.ViewerField, None)
+        
+        if file_content is None:
+            return make_response({"Viewer missing": "You should include the content of your viewer "
+                                                    "class file in the init_connection request"}, 400)
+
+        print("Extract content")
+        file_content = base64.b64decode(file_content)
+        checksum = hashlib.sha256(file_content).hexdigest()
+        print("Get checksum")
+        # Check if any server already running is available and if one was found use it and response with its endpoints
+        available_server = self.find_available_server(checksum)
+        # Get the remote proxy host
+        print("CHECK I SERVER AV")
+        
+        if available_server is not None:
+            
+            self.servers_running.append(available_server)
+            res = requests.get(f"{available_server.host}/init_connection").json()
+            print("Host", self.proxy_host)
+            print("URL COMPUTED", f"http://{self.proxy_host}{self.base_url}/server/{available_server.host.split('/')[-1]}")
+            res["host"] = f"http://{self.proxy_host}{self.base_url}/server/{available_server.host.split('/')[-1]}"
+            return make_response(res, 200)
+
+        print("No server av")
+
+        port = find_free_port()
+        print("Found free port")
+        file_path = f"{self.viewer_dir}/viewer_{port}.py"
+        with open(file_path, "wb") as f:
+            f.write(file_content)
+        print("Written the trame file")
+        print(file_path)
+        # Run the trame server in a new thread
+        threading.Thread(target=run_trame_viewer, args=[port, file_path]).start()
+        # Wait for server to come alive
+        wait_for_server_alive(f"{EndpointsInterface.Localhost}:{port}", timeout=10)
+        print("Server launch")
+        res = requests.get(f"{EndpointsInterface.Localhost}:{port}/init_connection")
+        print(res.content)
+        res = res.json()
+        # Add the new server to the proxy server list
+        print("making request at ", f"{EndpointsInterface.Localhost}:{self.proxy_port}{self.base_url}/update_available_servers")
+        proxy_res = requests.get(f"{EndpointsInterface.Localhost}:{self.proxy_port}{self.base_url}/update_available_servers",
+                                 json={"action": "add", "server_url": res['host']})
+        server_id = proxy_res.json()["server_id"]
+        # Change the host's endpoint to use the proxy, check if the host is an ip or a domain to reply with the right host
         try:
-            requests.get(server)
-            return True
-        except Exception:
-            return False
-
-    def setup_server(self):
-        """ Launch a local server using python subprocess on another thread. If a Trame server isn't already running """
-        if self.is_server_alive(self.server_url):
-            return
-        trame_viewer_thread = threading.Thread(target=self.run_trame_viewer)
-        trame_viewer_thread.start()
-        root_logger.info("MeshViewer Created")
-
-    def setup_endpoints(self):
-        """ Fill the endpoints dictionary with the info received from the server """
-        # If the server was launched locally, we need to wait for it to be up
-        self.wait_for_server_alive()
-        res = requests.get(self.server_url + self.endpoints["init_connection"])
-        try:
-            json_res = res.json()
-        except json.JSONDecodeError as e:
-            root_logger.error("Invalid server response")
-            return
-
-        # Check that all necessary endpoints where given in the request and fill the endpoints Dict
-        for endpoint in self.required_endpoints:
-            if endpoint not in json_res:
-                root_logger.error(f"ERROR, the endpoint {endpoint} was not specified by the server")
-                continue
-            self.endpoints[endpoint] = json_res[endpoint]
+            ipaddress.ip_address(self.proxy_host)
+            res["host"] = f"http://{self.proxy_host}{self.base_url}/server/{server_id}"
 
-    def run_trame_viewer(self):
-        """ Launche a Trame server using python subprocess """
-        try:
-            subprocess.run(["python3", os.path.dirname(os.path.abspath(__file__)) + "/trame_viewer.py", "--server"],
-                           stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL,
-                           check=True)  # stdout=subprocess.DEVNULL,  stderr=subprocess.DEVNULL,
-        except subprocess.CalledProcessError as e:
-            root_logger.error("It seems like the server crashed")
-
-    def wait_for_server_alive(self):
-        """ Try to ping the server to see if it is up  """
-        init_time = time.time()
-        attempt = 0
-        while not self.is_server_alive(self.endpoints["host"]) and attempt <= self.max_retries:
-            if time.time() - init_time >= self.server_timeout:
-                init_time = time.time()
-                self.setup_server()
-                attempt += 1
-
-    def set_mesh(self):
-        """ Set the mesh viewed on the server by making a request """
-        url = self.endpoints["host"] + self.endpoints["select_mesh"]
-        data = {
-            "mesh_path": self.mesh_path,
-            "nbr_frames": self.sequence_size,
-            "width": self.width,
-            "height": self.height
-        }
-        headers = {"Content-Type": "application/json"}
+        except ValueError:
+            res["host"] = f"http://{self.proxy_host}{self.base_url}/server/{server_id}"
+           
+        print("Got the host", res["host"])
+        # Since communication with the server runing is local, no need to use the url, localhost + port is always working
+        self.servers_running.append(ServerItem(f"{EndpointsInterface.Localhost}:{self.proxy_port}{self.base_url}/server/{server_id}", checksum, file_path))
+        return make_response(res, 200)
+
+    @staticmethod
+    def get_launch_path():
+        return os.path.abspath(__file__)
+
+    def _lifecycle_task_kill_server(self, servers_running):
+        servers_killed = super()._lifecycle_task_kill_server(servers_running)
+        # Complete the routine by notifying the proxy of all the server that needs to be unreferenced
+        for server in servers_killed:
+            payload = {"action": "remove", "server_url": server.host}
+            requests.get(f"http://{self.proxy_host}:{self.proxy_port}/update_available_servers", json=payload)
 
-        # Check in the response if any action is necessary such as make the iframe bigger
-        response = requests.get(url, data=json.dumps(data), headers=headers, timeout=2000)
-        try:
-            resp_body = response.json()
-            if "request_space" in resp_body:
-                self.height = resp_body["request_space"]
-        except requests.exceptions.JSONDecodeError:
-            return
-
-    def show(self):
-        """ Render the streamlit component """
-        components.iframe("http://127.0.0.1:8080/index.html", height=self.height)  # , scrolling=True
+
+
+
+if __name__ == "__main__":
+    server_manager = ServerManagerProxyfied()
+    try:
+        server_manager.run_server()
+    except KeyboardInterrupt:
+        print("STOPPING")
```

### Comparing `streamlit_pyvista-0.0.5/streamlit_pyvista/trame_viewer.py` & `streamlit_pyvista-0.0.6/streamlit_pyvista/trame_viewer.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,88 +3,121 @@
 from pyvista.trame.ui import plotter_ui
 from trame.app import get_server
 from trame.ui.vuetify3 import VAppLayout
 from trame.widgets import vuetify3 as vuetify
 from trame.widgets import html
 from aiohttp import web
 from trame.decorators import TrameApp, change, controller
+import validators
+import base64
 
 import logging
 import os
 import numpy as np
 import time, threading
 import asyncio
 from abc import ABC, abstractmethod
-
 from typing import Dict
 
+from vtk import vtkTransform
+from vtkmodules.vtkFiltersCore import (vtkDecimatePro, vtkTriangleFilter)
+from vtkmodules.vtkCommonDataModel import vtkPolyData
+
+from streamlit_pyvista.utils import is_web_link, save_mesh_content_from_url, update_cache, save_mesh_content
+
 root_logger = logging.getLogger("solidipes")
 root_logger.propagate = True
 root_logger.setLevel(logging.INFO)
 if "FULL_SOLIDIPES_LOG" not in os.environ:
-    root_logger.setLevel(logging.INFO)
+    root_logger.setLevel(logging.DEBUG)
 
 
 @TrameApp()
 class MeshViewer:
     """ A Trame server class that manage the view of a 3d mesh and its controls """
 
-    def __init__(self, mesh=None, plotter=None, server=None, port=8080):
+    def __init__(self, mesh=None, plotter=None, server=None, port=8080, host="0.0.0.0"):
 
         root_logger.info("Server started")
         pv.OFF_SCREEN = True
+        self.host = host
+        self.exposed_host = "127.0.0.1"
 
-        self.scalar_bar_exist = None
         if server is None:
             self.server = get_server(port=port)
         else:
             self.server = server
+
         self.slider_playing = False
         self.path = None
-
         self.mesh = None
         self.clean_mesh = None
+        self.cache_path = ".streamlit-pyvista-cache"
 
         self.style = {
             "background-color": "black",
             "font-color": "white"
         }
 
         self.pl = self.setup_pl()
 
+        # Setup server lifecycle callback functions
         setattr(self, "on_server_bind", self.server.controller.add("on_server_bind")(self.on_server_bind))
+        setattr(self, "on_client_exited", self.server.controller.add("on_client_exited")(self.on_client_exited))
+        setattr(self, "on_client_connected",
+                self.server.controller.add("on_client_connected")(self.on_client_connected))
+        setattr(self, "on_server_exited", self.server.controller.add("on_server_exited")(self.on_server_exited))
+
+        self.client_counter = 1
+        threading.Timer(3, self.client_counter_cb).start()
+        threading.Timer(60 * 5, self.stop_server).start()
 
         # Setup api endpoints
         self.my_routes = [
             web.get("/select_mesh", self.change_mesh),
             web.get("/init_connection", self.init_connection),
+            web.get("/upload_mesh", self.upload_mesh),
+            web.get("/nbr_clients", lambda x: web.json_response({"nbr_clients": self.client_counter}, status=200)),
+            web.get("/kill_server", self.kill_server),
         ]
+        self.mesh_missing = None
 
         self.setup_state()
 
         self.setup_timer()
 
-        self.loop = asyncio.get_event_loop()
+        self.loop = None
 
         self.mesh_array = None
-
         self.actor = None
         self.width = 800
         self.height = 900
         self.ui = self.build_ui()
 
+    def client_counter_cb(self):
+        self.client_counter -= 1
+
+    async def kill_server(self, request):
+        await self.server.stop()
+        return web.json_response({"success": "Server killed"}, status=200)
+
+    async def stop_server(self):
+        if self.client_counter == 0:
+            await self.server.stop()
+        else:
+            threading.Timer(60 * 5, self.stop_server).start()
+
     def setup_pl(self) -> pv.Plotter:
         """ Setup all class attributes related to the pyvista Plotter """
         # Create the plotter and add its styles
         pl = pv.Plotter()
         pl.background_color = self.style["background-color"]
         pl.theme.font.color = self.style["font-color"]
         # Initialize attribute related to the plotter
         self.bounds_scalar = None
-        self.scalar_bar_exist = False
         self.scalar_bar_mapper = None
         return pl
 
     def setup_state(self):
         """ Set up all the state variables to initial values """
         self.state.is_full_screen = False
         self.state.mesh_representation = self.state.options[0] if self.state.options is not None else None
@@ -104,63 +137,60 @@
         self.prev_bar_repr = self.state.mesh_representation
         self.prev_wrap = "0"
 
     def setup_timer(self):
         """ Set up the timer callback and timeout """
         self.timer_timeout = 0.25
         self.timer = threading.Thread(target=self.timer_callback)
-        self.sequence_bounds = [0, 70]
+        self.sequence_bounds = [0, 0]
 
     @change("mesh_representation")
     def update_mesh_representation(self, mesh_representation, **kwargs):
         """ This function is automatically called when the state 'mesh_representation' is changed.
         This state is used to determine which vector field is shown """
         # Remove the scalar bar representing the last vector field shown
-        if self.mesh is not None and self.mesh.active_scalars is not None:
-            self.pl.remove_scalar_bar()
-        self.prev_bar_repr = mesh_representation
+        self.clear_scalar_bars()
 
         # Replace the string input "None" with None
         if mesh_representation == "None":
             self.state.mesh_representation = None
 
         # Set all element of the mesh sequence with the same field shown
         for i in range(self.sequence_bounds[1]):
             if self.mesh_array is not None:
                 self.mesh_array[i].set_active_scalars(self.state.mesh_representation)
 
         # Update ui elements
         self.update_mesh_from_index(self.state.slider_value)
-        self.update_warp_input(self.state.warp_input)
+        self.update_warp_input()
         self.ui = self.build_ui()
 
     @change("warp_input")
-    def update_warp_input(self, warp_input, **kwargs):
+    def update_warp_input(self, **kwargs):
         """ This function is automatically called when the state 'warp_input' is changed. """
         try:
 
-            new_warp = float(warp_input)
+            new_warp = float(self.state.warp_input)
+            if self.mesh is None:
+                return
             dim = self.mesh.point_data.get_array(self.state.mesh_representation).ndim  # 1 if scalar, 2 if vector
 
             # if the dimension of the field is 1 we can warp by a scalar, else we warp by a vector
             if dim == 1:
                 new_pyvista_mesh = self.clean_mesh.warp_by_scalar(self.state.warped_field,
                                                                   factor=new_warp)
             else:
                 new_pyvista_mesh = self.clean_mesh.warp_by_vector(self.state.warped_field,
                                                                   factor=new_warp)
             self.prev_wrap = self.state.warp_input
             # Show the mesh that was warped
             self.replace_mesh(new_pyvista_mesh)
-
-        except ValueError as e:
-            print(e)
-            pass
         except Exception as e:
-            print(e)
+            root_logger.error(f"An error occurred with the warp {self.state.warp_input}")
+            root_logger.debug(e)
 
     @change("warped_field")
     def update_warped_field(self, warped_field, **kwargs):
         """ This function is automatically called when the state 'warped_field' is changed.
          This state is used to describe which vector field of the mesh we want to warp. """
         if warped_field is None or warped_field == "None":
             return
@@ -184,15 +214,16 @@
         return self.server.state
 
     @property
     def ctrl(self):
         return self.server.controller
 
     def timer_callback(self):
-        """ This function is called on all timer tick and update the mesh viewed to animate a sequence of mesh playing """
+        """ This function is called on all timer tick and update the mesh viewed to animate a sequence of mesh
+        playing """
 
         # The animation needs to stop when the server stop or if the animation was paused by the user
         while self.slider_playing and self.server.running:
             # Increment the counter while keeping it within the bound of the mesh sequence
             self.state.slider_value = (self.state.slider_value + 1) % self.sequence_bounds[1]
             # Call function on the main thread using thread safe method to update the server states and ui
             self.loop.call_soon_threadsafe(self.update_mesh_from_index, self.state.slider_value)
@@ -217,28 +248,31 @@
         """
         This function handles the loading of new mesh in the server
         Args:
             mesh_path: the path of the mesh
             seq_len: if it's a sequence of mesh, give its length else its one
         """
         self.mesh_array = []
-        # If the seqence is of length 1, just load it
-        if seq_len == 1:
-            if not os.path.exists(mesh_path):
-                root_logger.error(f"Error, the file {mesh_path} does not exist")
-                return
-            self.mesh_array.append(pv.read(mesh_path))
-            return
+        missing_mesh = []
         # If the mesh is a sequence, then format its path and load all element in the mesh array
-        for i in range(self.sequence_bounds[1]):
-            path = self.path % i
-            if not os.path.exists(path):
-                root_logger.error(f"Error, the file {path} does not exist")
-                return
+        for i, path in enumerate(mesh_path):
+            if is_web_link(path):
+                if not validators.url(path):
+                    root_logger.error(f"The link {path} is not valid")
+                    self.mesh_array.append(None)
+                    continue
+                path = save_mesh_content_from_url(path, f"{self.cache_path}/{path.split('/')[-1]}")
+
+
+            elif not os.path.exists(path):
+                missing_mesh.append((path, i))
+                self.mesh_array.append(None)
+                continue
             self.mesh_array.append(pv.read(path))
+        return missing_mesh
 
     async def change_mesh(self, request):
         """
         This function is called when a request to '/select_mesh' is made
         Args:
             request: the request received
 
@@ -249,38 +283,62 @@
         # Retrieve information from the request
         self.path = request_body.get("mesh_path", None)
         self.width = request_body.get("width", self.width)
         self.height = request_body.get("height", self.height)
         self.sequence_bounds[1] = request_body.get("nbr_frames", self.sequence_bounds[1])
         if self.path is None:
             root_logger.error("No filepath found in the change mesh request")
-            return web.json_response({"error": "Error : No filepath found in the change mesh request"}, status=400)
+            return web.json_response({"error": "No filepath found in the change mesh request"}, status=400)
 
         # Reset the viewer to an empty state
         self.clear_viewer()
-
         # Get the mesh and prepare it to be displayed
-        self.handle_new_mesh(self.path, self.sequence_bounds[1])
+        self.mesh_missing = self.handle_new_mesh(self.path, self.sequence_bounds[1])
+        if len(self.mesh_missing) > 0:
+            root_logger.info(f"Missing mesh: {self.mesh_missing}, request made to client")
+            return web.json_response({"request_files": self.mesh_missing}, status=200)
+        if len(self.mesh_array) == 0:
+            root_logger.error("None of the mesh passed as argument seemed to be working properly")
+            return web.json_response({"error": "No valid path passed"}, status=400)
+
+        self.handle_new_mesh_request()
+
+        # If the height allocated by the streamlit component, ask for more space in the response of the request
+        response_body = {}
+        if self.height - self.estimate_controller_height()[1] < 700:
+            response_body["request_space"] = 1.65 * self.height
+        return web.json_response(response_body, status=200)
+
+    def handle_new_mesh_request(self):
+
         self.replace_mesh(self.mesh_array[0])
 
         # Prepare ui elements that depends on the mesh
         self.state.options = self.mesh_array[0].array_names.copy()
         self.state.options.insert(0, "None")
         self.state.options_warp = self.state.options.copy()
 
         # Show the new mesh in the viewers and its controls
         self.computes_bounds_scalar()
         self.update_ui()
         self.pl.reset_camera()
 
-        # If the height allocated by the streamlit component, ask for more space in the response of the request
-        response_body = {}
-        if self.height - self.estimate_controller_height()[1] < 700:
-            response_body["request_space"] = 1.65 * self.height
-        return web.json_response(response_body, status=200)
+    async def upload_mesh(self, request):
+
+        request_body: Dict[str, str] = await request.json()
+        for key, (encoded_content, index) in request_body.items():
+            content = base64.b64decode(encoded_content)
+            loc = save_mesh_content(content, f"{self.cache_path}/{key}")
+            self.mesh_array[index] = pv.read(loc)
+            self.mesh_missing.remove((key, index))
+
+        if self.mesh_missing is None or len(self.mesh_missing) == 0:
+            self.handle_new_mesh_request()
+
+        return web.json_response({"success": "Mesh uploaded successfully"}, status=200)
 
     def clear_scalar_bars(self):
         """ Remove all the scalar bars shown on the plotter """
         if self.pl is None:
             return
         bar_to_remove = [key for key in self.pl.scalar_bars.keys()]
         [self.pl.remove_scalar_bar(title=key) for key in bar_to_remove]
@@ -383,19 +441,16 @@
         # Replace actor with the new mesh (automatically update the actor because they have the same name)
         self.actor = self.pl.add_mesh(self.mesh, style="wireframe" if self.state.wireframe_on else None,
                                       name="displayed_mesh", show_scalar_bar=True,
                                       scalar_bar_args={"mapper": self.pl.mapper})
 
     def start_server(self):
         """ Start the server """
-        try:
-            self.server.start()
-        except KeyboardInterrupt:
-            # Stop the thread that manage the play of the mesh sequence
-            self.timer.join()  # Wait for the timer thread to finish
+
+        self.server.start(host=self.host)
 
     def update_ui(self):
         """ Force to redraw the ui """
         if self.mesh is not None and self.mesh.active_scalars is not None:
             self.pl.remove_scalar_bar()
         self.ui = self.build_ui()
 
@@ -443,14 +498,16 @@
             root_logger.error("Impossible to start the sequence since it's a unique mesh")
             return
 
         # Invert the state of the play button and if it's playing start the timer updating frame at a fixed interval
         self.slider_playing = not self.slider_playing
         if self.slider_playing and not self.timer.is_alive():
             self.state.play_pause_icon = "mdi-pause"
+
+            self.loop = asyncio.get_event_loop()
             self.timer.start()
         else:
             self.state.play_pause_icon = "mdi-play"
         self.update_ui()
 
     def build_warp_option(self):
         """
@@ -499,19 +556,19 @@
         with (layout):
             with vuetify.VRow(dense=True):
                 with vuetify.VCol(cols="6"):
                     # If there are options show the dropdown
                     if self.state.options[0] is not None and len(self.state.options) > 1:
                         self.option_dropdown()
                 # If there are options create the warper layout
-                # if len(self.state.options) > 1:
-                self.build_warper()
+                if self.state.options[0] is not None and len(self.state.options) > 1:
+                    self.build_warper()
             vuetify.VCheckbox(v_model=("wireframe_on",), label="Wireframe on", id="wireframe_checkbox")
             # If the viewer display a sequence of mesh show the slider
-            if self.sequence_bounds[1] != 1:
+            if self.sequence_bounds[1] > 1:
                 self.build_slider()
 
             with vuetify.VBtn(click=self.request_full, style="position: absolute; bottom:25px; right:25px;", icon=True):
                 vuetify.VIcon("mdi-fullscreen" if not self.state.is_full_screen else "mdi-fullscreen-exit")
         return layout
 
     def estimate_controller_height(self):
@@ -531,15 +588,15 @@
         Build all the ui frontend with all different components
         Returns:
             a VAppLayout for the server
         """
         control_height = self.estimate_controller_height()[0]
         # Define some styling variables
         if not self.state.is_full_screen:
-            plotter_height = self.height - control_height
+            plotter_height = self.height - 250
             plotter_height = f"{plotter_height}px"
             width = "100%"
         else:
             plotter_height = "100%"
             width = "100%"
 
         with VAppLayout(self.server) as layout:
@@ -556,37 +613,57 @@
                                            style="width: 100%; height:100%;background-color: black;")
                             else:
                                 plotter_ui(self.pl, default_server_rendering=True,
                                            style="width: 100%; height:100%;background-color: black;")
                     with vuetify.VCol(style=f"height:{control_height}px;padding: 0;width:100%;"):
                         # Create the whole control layout
                         self.build_mesh_control_layout()
-            return layout
+
+        return layout
 
     def on_server_bind(self, wslink_server):
         """
-        When the server is bind, add api endpoint to it
+        When the server is bind, add api endpoint to it and update the cache
         Args:
             wslink_server: the socket manager of the server
         """
+        # Update the cache
+        update_cache(self.cache_path)
+        root_logger.info("Server endpoints were bind")
         wslink_server.app.add_routes(self.my_routes)
 
+    def on_client_exited(self):
+        self.client_counter -= 1
+        root_logger.info(f"A client disconnected, there are {self.client_counter} clients connected")
+
+    def on_client_connected(self):
+        self.client_counter += 1
+        root_logger.info(f"A client connected, there are {self.client_counter} clients connected")
+
+    def on_server_exited(self, **kwargs):
+        root_logger.info("Server stopped")
+        if self.slider_playing:
+            self.timer.join()
+        update_cache(self.cache_path)
+
     async def init_connection(self, request):
         """
         Base api endpoint on '/init_connection' to inform the client of all the endpoints available and their locations
         Args:
             request: the request made to this endpoint
 
         Returns:
             a json with all information about endpoints required and a success status 200
         """
         response_body = {
             "select_mesh": "/select_mesh",
-            "host": f"http://127.0.0.1:{self.server.port}"
+            "upload_mesh": "/upload_mesh",
+            "host": f"http://{self.exposed_host}:{self.server.port}"
         }
+        root_logger.info("Connection was initiated")
         return web.json_response(response_body, status=200)
 
     def request_full(self):
         """ Make a js call to request full screen on the iframe """
         self.server.js_call("container", "requestFullscreen")
         self.state.is_full_screen = not self.state.is_full_screen
         self.update_ui()
@@ -605,14 +682,15 @@
 
     @abstractmethod
     def render(self):
         pass
 
 
 if __name__ == "__main__":
+    pv.start_xvfb()
     # Add command line argument and support
     parser = argparse.ArgumentParser(description='Launch a trame server instance')
     # Add the port argument that allow user to specify the port to use for the server from command line
     parser.add_argument('--port', type=int, help='Specify the port of the server')
     # Add --server flag that is used to specify whether to use the trame as only a server and block the
     # automatic open of a browser
     parser.add_argument('--server', action="store_true", help='Specify if the trame is opened as a server')
```

