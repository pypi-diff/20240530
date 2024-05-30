# Comparing `tmp/cam_manager-0.2.1.tar.gz` & `tmp/cam_manager-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cam_manager-0.2.1.tar", last modified: Mon May 27 07:45:56 2024, max compression
+gzip compressed data, was "cam_manager-0.2.2.tar", last modified: Thu May 30 12:49:24 2024, max compression
```

## Comparing `cam_manager-0.2.1.tar` & `cam_manager-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:45:56.019097 cam_manager-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-27 07:45:56.019097 cam_manager-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-27 07:45:48.000000 cam_manager-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:45:56.019097 cam_manager-0.2.1/cam_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 07:45:48.000000 cam_manager-0.2.1/cam_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-27 07:45:48.000000 cam_manager-0.2.1/cam_manager/cam_ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-27 07:45:48.000000 cam_manager-0.2.1/cam_manager/cam_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-27 07:45:48.000000 cam_manager-0.2.1/cam_manager/cam_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-27 07:45:48.000000 cam_manager-0.2.1/cam_manager/cam_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-27 07:45:48.000000 cam_manager-0.2.1/cam_manager/cam_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:45:56.019097 cam_manager-0.2.1/cam_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-27 07:45:56.000000 cam_manager-0.2.1/cam_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-27 07:45:56.000000 cam_manager-0.2.1/cam_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:45:56.000000 cam_manager-0.2.1/cam_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 07:45:56.000000 cam_manager-0.2.1/cam_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 07:45:56.000000 cam_manager-0.2.1/cam_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:45:56.019097 cam_manager-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-27 07:45:48.000000 cam_manager-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:49:24.182844 cam_manager-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-30 12:49:24.182844 cam_manager-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-30 12:49:12.000000 cam_manager-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:49:24.178845 cam_manager-0.2.2/cam_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-30 12:49:12.000000 cam_manager-0.2.2/cam_manager/cam_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:49:24.182844 cam_manager-0.2.2/cam_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 12:49:24.000000 cam_manager-0.2.2/cam_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:49:24.182844 cam_manager-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-30 12:49:12.000000 cam_manager-0.2.2/setup.py
```

### Comparing `cam_manager-0.2.1/PKG-INFO` & `cam_manager-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.2.1
+Version: 0.2.2
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pytorch==2.2.2
+Requires-Dist: mss==9.0.1
+Requires-Dist: torch==2.2.2
 Requires-Dist: torchaudio==2.2.2
 Requires-Dist: torchvision==0.17.2
+Requires-Dist: PyGetWindow==0.0.9
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: ultralytics==8.2.22
 Requires-Dist: opencv-python==4.9.0.80
 
 #MANAGER
 --------------------
 In the CamManager init, switch "is_ai" parameter to use the default AI process.
@@ -26,14 +28,19 @@
 --------------------
 get_available_cams
 =====
 Description: Get all available camera devices.
 Parameters: capture_method: The method used to capture the video stream (default is cv2.CAP_DSHOW).
 Returns: list: A list of indices of available camera devices.
 
+get_available_windows
+====
+Description: Get all available windows.
+Returns: list: A list of all available windows.
+
 get_active_cam
 =====
 Description: Get the currently active camera ID.
 Returns: int: The ID of the currently active camera. If no active camera, a message is printed.
 
 get_all_added_cams
 =====
@@ -79,40 +86,47 @@
 --------------------
 add_cam
 =====
 Description: Add a camera by its ID.
 Paramters:
     cam_id (int): The ID of the camera to be added.
     capture_method: The method used to capture the video stream (default is cv2.CAP_DSHOW).
+    tricky_window_title (str, optional): The title of the window to be used as a tricky cam.
 
 release_cam
 =====
 Description: Release a specific camera by its ID.
 Parameters: cam_id (int): The ID of the camera to be released.
+tricky_window_title (str, optional): The title of the tricky cam window to be released.
 
 release_all_cams
 =====
 Description: Release all cameras.
 
 switch_active_cam
 =====
 Description: Switch the active camera to the specified ID.
 Parameters: cam_id (int): The ID of the camera to be set as active.
+tricky_window_title (str, optional): The title of the tricky cam window to be set as active.
 
 get_frame
 =====
 Description: Get a frame from a specific camera or the active camera.
-Parameters: cam_id (int, optional): The ID of the camera to get the frame from. If None, the frame is captured from the active camera (default is None).
+Parameters:
+    cam_id (int, optional): The ID of the camera to get the frame from. If None, the frame is captured from the active camera (default is None).
+    tricky_window_title (str, optional): The title of the tricky cam window to get the frame from. Default is None.
 Returns: The captured frame from the specified or active camera, or None if failed.
 
+
 capture_image
 =====
 Description: Capture an image from a specific camera or the active camera and save it to a file.
 Parameters:
     cam_id (int, optional): The ID of the camera to capture the image from. If None, the image is captured from the active camera (default is None).
+    tricky_window_title (str, optional): The title of the tricky cam window to capture the image from. Default is None.
     filename (str, optional): The name of the file to save the captured image (default is "capture.jpg").
 
 #AI
 --------------------
 add_ai_to_frame
 =====
 Description: Add AI-based object detection or segmentation to the frame.
```

### Comparing `cam_manager-0.2.1/README.md` & `cam_manager-0.2.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 --------------------
 get_available_cams
 =====
 Description: Get all available camera devices.
 Parameters: capture_method: The method used to capture the video stream (default is cv2.CAP_DSHOW).
 Returns: list: A list of indices of available camera devices.
 
+get_available_windows
+====
+Description: Get all available windows.
+Returns: list: A list of all available windows.
+
 get_active_cam
 =====
 Description: Get the currently active camera ID.
 Returns: int: The ID of the currently active camera. If no active camera, a message is printed.
 
 get_all_added_cams
 =====
@@ -60,40 +65,47 @@
 --------------------
 add_cam
 =====
 Description: Add a camera by its ID.
 Paramters:
     cam_id (int): The ID of the camera to be added.
     capture_method: The method used to capture the video stream (default is cv2.CAP_DSHOW).
+    tricky_window_title (str, optional): The title of the window to be used as a tricky cam.
 
 release_cam
 =====
 Description: Release a specific camera by its ID.
 Parameters: cam_id (int): The ID of the camera to be released.
+tricky_window_title (str, optional): The title of the tricky cam window to be released.
 
 release_all_cams
 =====
 Description: Release all cameras.
 
 switch_active_cam
 =====
 Description: Switch the active camera to the specified ID.
 Parameters: cam_id (int): The ID of the camera to be set as active.
+tricky_window_title (str, optional): The title of the tricky cam window to be set as active.
 
 get_frame
 =====
 Description: Get a frame from a specific camera or the active camera.
-Parameters: cam_id (int, optional): The ID of the camera to get the frame from. If None, the frame is captured from the active camera (default is None).
+Parameters:
+    cam_id (int, optional): The ID of the camera to get the frame from. If None, the frame is captured from the active camera (default is None).
+    tricky_window_title (str, optional): The title of the tricky cam window to get the frame from. Default is None.
 Returns: The captured frame from the specified or active camera, or None if failed.
 
+
 capture_image
 =====
 Description: Capture an image from a specific camera or the active camera and save it to a file.
 Parameters:
     cam_id (int, optional): The ID of the camera to capture the image from. If None, the image is captured from the active camera (default is None).
+    tricky_window_title (str, optional): The title of the tricky cam window to capture the image from. Default is None.
     filename (str, optional): The name of the file to save the captured image (default is "capture.jpg").
 
 #AI
 --------------------
 add_ai_to_frame
 =====
 Description: Add AI-based object detection or segmentation to the frame.
```

### Comparing `cam_manager-0.2.1/cam_manager/cam_ai.py` & `cam_manager-0.2.2/cam_manager/cam_ai.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.2.1/cam_manager/cam_effects.py` & `cam_manager-0.2.2/cam_manager/cam_effects.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.2.1/cam_manager/cam_info.py` & `cam_manager-0.2.2/cam_manager/cam_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import cv2
+import pygetwindow as gw
 
 class CamInfoMixin:
     def get_available_cams(self, capture_method = cv2.CAP_DSHOW) -> list:
         """
         Get all available cam devices.
         Parameters: capture_method: The method used to capture the video stream.
         Returns: list: A list of indices of available cam devices.
@@ -18,14 +19,24 @@
             arr.append(index)
             cap.release()
             index += 1
 
         if not arr: print("No cams available.")
         return arr
 
+    def get_available_windows(self) -> list:
+            """
+            Get all available windows.
+            Returns: list: A list of all available windows.
+            """
+            windows = gw.getAllTitles()
+            if not windows:
+                print("No windows available.")
+            return windows
+
     def get_active_cam(self) -> int:
         """
         Get the currently active cam ID.
         Returns: int: The ID of the currently active cam.
         """
 
         if self.active_cam_id is None: print("No active cam.")
```

### Comparing `cam_manager-0.2.1/cam_manager/cam_manager.py` & `cam_manager-0.2.2/cam_manager/cam_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,13 +8,14 @@
         if ai_mode not in possible_ai_modes:
             ai_mode = "detection"
             print(f"Invalid AI mode. Possible values are {possible_ai_modes}")
 
         super().__init__()
 
         self.cams = {}
+        self.tricky_cams = {}
         self.active_cam_id = None
 
         if is_ai:
             from cam_manager.cam_ai import CamAIMixin
             self.ai = CamAIMixin(ai_mode)
         else: self.ai = None
```

### Comparing `cam_manager-0.2.1/cam_manager.egg-info/PKG-INFO` & `cam_manager-0.2.2/cam_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.2.1
+Version: 0.2.2
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pytorch==2.2.2
+Requires-Dist: mss==9.0.1
+Requires-Dist: torch==2.2.2
 Requires-Dist: torchaudio==2.2.2
 Requires-Dist: torchvision==0.17.2
+Requires-Dist: PyGetWindow==0.0.9
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: ultralytics==8.2.22
 Requires-Dist: opencv-python==4.9.0.80
 
 #MANAGER
 --------------------
 In the CamManager init, switch "is_ai" parameter to use the default AI process.
@@ -26,14 +28,19 @@
 --------------------
 get_available_cams
 =====
 Description: Get all available camera devices.
 Parameters: capture_method: The method used to capture the video stream (default is cv2.CAP_DSHOW).
 Returns: list: A list of indices of available camera devices.
 
+get_available_windows
+====
+Description: Get all available windows.
+Returns: list: A list of all available windows.
+
 get_active_cam
 =====
 Description: Get the currently active camera ID.
 Returns: int: The ID of the currently active camera. If no active camera, a message is printed.
 
 get_all_added_cams
 =====
@@ -79,40 +86,47 @@
 --------------------
 add_cam
 =====
 Description: Add a camera by its ID.
 Paramters:
     cam_id (int): The ID of the camera to be added.
     capture_method: The method used to capture the video stream (default is cv2.CAP_DSHOW).
+    tricky_window_title (str, optional): The title of the window to be used as a tricky cam.
 
 release_cam
 =====
 Description: Release a specific camera by its ID.
 Parameters: cam_id (int): The ID of the camera to be released.
+tricky_window_title (str, optional): The title of the tricky cam window to be released.
 
 release_all_cams
 =====
 Description: Release all cameras.
 
 switch_active_cam
 =====
 Description: Switch the active camera to the specified ID.
 Parameters: cam_id (int): The ID of the camera to be set as active.
+tricky_window_title (str, optional): The title of the tricky cam window to be set as active.
 
 get_frame
 =====
 Description: Get a frame from a specific camera or the active camera.
-Parameters: cam_id (int, optional): The ID of the camera to get the frame from. If None, the frame is captured from the active camera (default is None).
+Parameters:
+    cam_id (int, optional): The ID of the camera to get the frame from. If None, the frame is captured from the active camera (default is None).
+    tricky_window_title (str, optional): The title of the tricky cam window to get the frame from. Default is None.
 Returns: The captured frame from the specified or active camera, or None if failed.
 
+
 capture_image
 =====
 Description: Capture an image from a specific camera or the active camera and save it to a file.
 Parameters:
     cam_id (int, optional): The ID of the camera to capture the image from. If None, the image is captured from the active camera (default is None).
+    tricky_window_title (str, optional): The title of the tricky cam window to capture the image from. Default is None.
     filename (str, optional): The name of the file to save the captured image (default is "capture.jpg").
 
 #AI
 --------------------
 add_ai_to_frame
 =====
 Description: Add AI-based object detection or segmentation to the frame.
```

### Comparing `cam_manager-0.2.1/setup.py` & `cam_manager-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version = "0.2.1",
+    version = "0.2.2",
     name = "cam_manager",
     description = "A camera management library to easily handle cameras with OpenCV.",
 
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
 
     author = "snatev",
```

