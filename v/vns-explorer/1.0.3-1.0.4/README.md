# Comparing `tmp/vns_explorer-1.0.3.tar.gz` & `tmp/vns_explorer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vns_explorer-1.0.3.tar", last modified: Wed May 29 07:32:17 2024, max compression
+gzip compressed data, was "vns_explorer-1.0.4.tar", last modified: Wed May 29 08:08:12 2024, max compression
```

## Comparing `vns_explorer-1.0.3.tar` & `vns_explorer-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 07:32:17.715870 vns_explorer-1.0.3/
--rw-rw-rw-   0        0        0      601 2024-05-29 07:32:17.715870 vns_explorer-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-05-29 04:11:37.000000 vns_explorer-1.0.3/README.md
--rw-rw-rw-   0        0        0      796 2024-05-29 07:31:15.000000 vns_explorer-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      468 2024-05-29 07:32:17.722368 vns_explorer-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 07:32:17.679380 vns_explorer-1.0.3/vns_explorer/
--rw-rw-rw-   0        0        0       64 2024-05-29 06:10:09.000000 vns_explorer-1.0.3/vns_explorer/__init__.py
--rw-rw-rw-   0        0        0     1446 2024-05-29 04:00:43.000000 vns_explorer-1.0.3/vns_explorer/agent.py
--rw-rw-rw-   0        0        0    10483 2024-05-29 07:31:02.000000 vns_explorer-1.0.3/vns_explorer/browser.py
--rw-rw-rw-   0        0        0     2293 2024-05-29 06:09:48.000000 vns_explorer-1.0.3/vns_explorer/env.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:32:17.713855 vns_explorer-1.0.3/vns_explorer.egg-info/
--rw-rw-rw-   0        0        0      601 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 08:08:12.983883 vns_explorer-1.0.4/
+-rw-rw-rw-   0        0        0      601 2024-05-29 08:08:12.983883 vns_explorer-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-29 04:11:37.000000 vns_explorer-1.0.4/README.md
+-rw-rw-rw-   0        0        0      796 2024-05-29 08:07:43.000000 vns_explorer-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      468 2024-05-29 08:08:12.990093 vns_explorer-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 08:08:12.936631 vns_explorer-1.0.4/vns_explorer/
+-rw-rw-rw-   0        0        0       64 2024-05-29 06:10:09.000000 vns_explorer-1.0.4/vns_explorer/__init__.py
+-rw-rw-rw-   0        0        0     1446 2024-05-29 04:00:43.000000 vns_explorer-1.0.4/vns_explorer/agent.py
+-rw-rw-rw-   0        0        0    10485 2024-05-29 08:07:29.000000 vns_explorer-1.0.4/vns_explorer/browser.py
+-rw-rw-rw-   0        0        0     2232 2024-05-29 08:05:39.000000 vns_explorer-1.0.4/vns_explorer/env.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:08:12.980749 vns_explorer-1.0.4/vns_explorer.egg-info/
+-rw-rw-rw-   0        0        0      601 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/top_level.txt
```

### Comparing `vns_explorer-1.0.3/PKG-INFO` & `vns_explorer-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vns_explorer
-Version: 1.0.3
+Version: 1.0.4
 Summary: Discover the Unseen
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `vns_explorer-1.0.3/pyproject.toml` & `vns_explorer-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 # Metadata Information
 [project]
 name = "vns_explorer"
-version = "1.0.3"
+version = "1.0.4"
 description = "Discover the Unseen"
 authors = [
     { name = "Thinh Vu", email = "mrthinh@live.com" },
     ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
```

### Comparing `vns_explorer-1.0.3/vns_explorer/agent.py` & `vns_explorer-1.0.4/vns_explorer/agent.py`

 * *Files identical despite different names*

### Comparing `vns_explorer-1.0.3/vns_explorer/browser.py` & `vns_explorer-1.0.4/vns_explorer/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
-import random
-# import pyautogui
 import os
 from importlib.util import find_spec
+# import random
+# import pyautogui
 
 # Detect if running on Google Colab
 is_colab = "COLAB_GPU" in os.environ
 
 # Import the setup function from setup_selenium if in Colab
 if is_colab:
     from .env import setup_selenium
@@ -78,33 +78,14 @@
             """
             Open a specific URL in the ChromeDriver instance.
             """
             print(f'Visiting {url}')
             self.driver.get(url)
             print(self.driver.title)
 
-        # def random_mouse(self, duration=2, frequency=0.5):
-        #     """
-        #     Simulate random mouse movements on the screen.
-
-        #     Parameters:
-        #         - duration (int): The total duration to simulate random mouse movements, in seconds.
-        #         - frequency (float): The frequency of mouse movements, in seconds.
-        #     """
-        #     if is_colab:
-        #         print("random_mouse() is not supported in Google Colab environment.")
-        #         return
-        #     end_time = time.time() + duration
-        #     while time.time() < end_time:
-        #         screen_width, screen_height = pyautogui.size()
-        #         x = random.randint(0, screen_width)
-        #         y = random.randint(0, screen_height)
-        #         pyautogui.moveTo(x, y, duration=frequency)
-        #         time.sleep(frequency)
-
         def scroll(self, direction='down', pct=0.2, duration=2):
             """
             Scroll the page up or down by a certain percentage.
 
             Parameters:
                 - direction (str): The direction to scroll. 'up' for scrolling up and 'down' for scrolling down. Default is 'down'.
                 - pct (float): The percentage of the page to scroll. Default is 0.2 (20%).
@@ -220,7 +201,26 @@
             """
             Take a screenshot of the current page.
 
             Parameters:
                 - path (str): The path to save the screenshot. Default is 'screenshot.png'.
             """
             self.driver.save_screenshot(path)
+
+        # def random_mouse(self, duration=2, frequency=0.5):
+        #     """
+        #     Simulate random mouse movements on the screen.
+
+        #     Parameters:
+        #         - duration (int): The total duration to simulate random mouse movements, in seconds.
+        #         - frequency (float): The frequency of mouse movements, in seconds.
+        #     """
+        #     if is_colab:
+        #         print("random_mouse() is not supported in Google Colab environment.")
+        #         return
+        #     end_time = time.time() + duration
+        #     while time.time() < end_time:
+        #         screen_width, screen_height = pyautogui.size()
+        #         x = random.randint(0, screen_width)
+        #         y = random.randint(0, screen_height)
+        #         pyautogui.moveTo(x, y, duration=frequency)
+        #         time.sleep(frequency)
```

### Comparing `vns_explorer-1.0.3/vns_explorer.egg-info/PKG-INFO` & `vns_explorer-1.0.4/vns_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vns_explorer
-Version: 1.0.3
+Version: 1.0.4
 Summary: Discover the Unseen
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

