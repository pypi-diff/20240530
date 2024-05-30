# Comparing `tmp/vns_explorer-1.0.4.tar.gz` & `tmp/vns_explorer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vns_explorer-1.0.4.tar", last modified: Wed May 29 08:08:12 2024, max compression
+gzip compressed data, was "vns_explorer-1.0.5.tar", last modified: Thu May 30 06:07:42 2024, max compression
```

## Comparing `vns_explorer-1.0.4.tar` & `vns_explorer-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:08:12.983883 vns_explorer-1.0.4/
--rw-rw-rw-   0        0        0      601 2024-05-29 08:08:12.983883 vns_explorer-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-05-29 04:11:37.000000 vns_explorer-1.0.4/README.md
--rw-rw-rw-   0        0        0      796 2024-05-29 08:07:43.000000 vns_explorer-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      468 2024-05-29 08:08:12.990093 vns_explorer-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 08:08:12.936631 vns_explorer-1.0.4/vns_explorer/
--rw-rw-rw-   0        0        0       64 2024-05-29 06:10:09.000000 vns_explorer-1.0.4/vns_explorer/__init__.py
--rw-rw-rw-   0        0        0     1446 2024-05-29 04:00:43.000000 vns_explorer-1.0.4/vns_explorer/agent.py
--rw-rw-rw-   0        0        0    10485 2024-05-29 08:07:29.000000 vns_explorer-1.0.4/vns_explorer/browser.py
--rw-rw-rw-   0        0        0     2232 2024-05-29 08:05:39.000000 vns_explorer-1.0.4/vns_explorer/env.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:08:12.980749 vns_explorer-1.0.4/vns_explorer.egg-info/
--rw-rw-rw-   0        0        0      601 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 08:08:12.000000 vns_explorer-1.0.4/vns_explorer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 06:07:42.068092 vns_explorer-1.0.5/
+-rw-rw-rw-   0        0        0      601 2024-05-30 06:07:42.067091 vns_explorer-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-29 04:11:37.000000 vns_explorer-1.0.5/README.md
+-rw-rw-rw-   0        0        0      796 2024-05-29 08:15:21.000000 vns_explorer-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      468 2024-05-30 06:07:42.075277 vns_explorer-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 06:07:42.018577 vns_explorer-1.0.5/vns_explorer/
+-rw-rw-rw-   0        0        0       64 2024-05-29 06:10:09.000000 vns_explorer-1.0.5/vns_explorer/__init__.py
+-rw-rw-rw-   0        0        0     1446 2024-05-29 04:00:43.000000 vns_explorer-1.0.5/vns_explorer/agent.py
+-rw-rw-rw-   0        0        0    12135 2024-05-29 09:56:35.000000 vns_explorer-1.0.5/vns_explorer/browser.py
+-rw-rw-rw-   0        0        0     2232 2024-05-29 08:05:39.000000 vns_explorer-1.0.5/vns_explorer/env.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:07:42.064092 vns_explorer-1.0.5/vns_explorer.egg-info/
+-rw-rw-rw-   0        0        0      601 2024-05-30 06:07:41.000000 vns_explorer-1.0.5/vns_explorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-30 06:07:41.000000 vns_explorer-1.0.5/vns_explorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:07:41.000000 vns_explorer-1.0.5/vns_explorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-30 06:07:41.000000 vns_explorer-1.0.5/vns_explorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 06:07:41.000000 vns_explorer-1.0.5/vns_explorer.egg-info/top_level.txt
```

### Comparing `vns_explorer-1.0.4/PKG-INFO` & `vns_explorer-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vns_explorer
-Version: 1.0.4
+Version: 1.0.5
 Summary: Discover the Unseen
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `vns_explorer-1.0.4/pyproject.toml` & `vns_explorer-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 # Metadata Information
 [project]
 name = "vns_explorer"
-version = "1.0.4"
+version = "1.0.5"
 description = "Discover the Unseen"
 authors = [
     { name = "Thinh Vu", email = "mrthinh@live.com" },
     ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
```

### Comparing `vns_explorer-1.0.4/vns_explorer/agent.py` & `vns_explorer-1.0.5/vns_explorer/agent.py`

 * *Files identical despite different names*

### Comparing `vns_explorer-1.0.4/vns_explorer/browser.py` & `vns_explorer-1.0.5/vns_explorer/browser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 import time
 import os
+import sys
 from importlib.util import find_spec
-# import random
-# import pyautogui
+import logging
+from typing import Optional
+
+# Set up logging
+logging.basicConfig(format='%(asctime)s - %(message)s', datefmt='%d-%b-%y %H:%M:%S')
+logger = logging.getLogger(__name__)
+# setup logging template
+
 
 # Detect if running on Google Colab
-is_colab = "COLAB_GPU" in os.environ
 
-# Import the setup function from setup_selenium if in Colab
+is_colab = 'google.colab' in sys.modules
+try:
+    is_hf = '.hf.space' in os.environ['SPACE_HOST']
+except:
+    is_hf = False
+
+Import the setup function from setup_selenium if in Colab
 if is_colab:
     from .env import setup_selenium
     setup_selenium()
 
 Imports = {
     "selenium": find_spec("selenium") is not None,
     "webdriver": find_spec("webdriver_manager") is not None,
-    # "pyautogui": find_spec("pyautogui") is not None and not is_colab
 }
 
 if not Imports["selenium"] or not Imports["webdriver"]:
     raise ImportError("selenium, webdriver_manager are required to run this script. Please install them using 'pip install selenium webdriver_manager and try again.")
 else:
     from selenium import webdriver
     from selenium.webdriver.chrome.service import Service as ChromeService
@@ -28,63 +39,111 @@
     from selenium.webdriver.support.ui import WebDriverWait
     from selenium.webdriver.support import expected_conditions as EC
     from webdriver_manager.chrome import ChromeDriverManager
     from selenium.common.exceptions import NoSuchElementException, TimeoutException
     import time  # Make sure to import time if using sleep
 
     class ChromeDriver():
-        def __init__(self, method='headless', duration=None, profile_path=None):
+        def __init__(self, method='headless', duration:Optional[int]=None, profile_path:Optional[str]=None, show_log:Optional[bool]=False):
             """
             Initialize the ChromeDriver instance.
             
             Parameters:
                 - method (str): The method to run the ChromeDriver. 'headless' for headless mode and None for normal mode.
                 - duration (int): The duration to wait after each action. Default is None.
             """
+            self.show_log = show_log
             if method not in ['headless', None]:
                 raise ValueError('Invalid method. Method must be either "headless" or None for normal mode.')
+            
+            if profile_path is None:
+                self.current_dir = os.getcwd()
+                self.profile_path = os.path.join(self.current_dir, "selenium_profile")
+                os.makedirs(self.profile_path, exist_ok=True)
+            else:
+                self.profile_path = profile_path
+
+            if method == 'headless':
+                self.method = 'headless'
+                self._common_driver_options(method='headless')
+
+            if is_colab:
+                self._colab_driver()
+                logger.info('Running mode is Google Colab')
+            elif is_hf:
+                self._hf_driver(profile_path=profile_path)
+                logger.info('Running mode is Huggingface Spaces')
+            else:
+                self._normal_driver(method=method)
+                logger.info('Running mode is local machine')
+
+            if method is None:
+                self.driver.maximize_window()
+            self.duration = duration
+
+        def _common_driver_options(self, method='headless'):
             chrome_options = Options()
             if method == 'headless':
                 chrome_options.add_argument("--headless")
                 chrome_options.add_argument("--no-sandbox")
                 chrome_options.add_argument("--disable-dev-shm-usage")
 
             # Set to disable the 'controlled by automated test software' notice
             chrome_options.add_experimental_option("excludeSwitches", ["enable-automation"])
             chrome_options.add_experimental_option('useAutomationExtension', False)
-
             # Add flag to ignore SSL certificate errors
             chrome_options.add_argument("--ignore-certificate-errors")
+            # Use the specified or default profile path
+            chrome_options.add_argument(f"user-data-dir={self.profile_path}")
+            self.chrome_options = chrome_options
+            if self.show_log:
+                logger.info('ChromeDriver options set up successfully!')
+
+        def _colab_driver(self):
+            options = Options()
+            options.add_argument("--headless")
+            options.add_argument("--no-sandbox")
+            self.driver = webdriver.Chrome(options=options)
+        
+        def _hf_driver(self, profile_path=None):
+            """
+            Set up the ChromeDriver instance for Huggingface Spaces which is specify for running in Docker Spaces.
+            """
+            self._common_driver_options(method='headless')
 
             if profile_path is None:
-                current_dir = os.getcwd()
-                profile_path = os.path.join(current_dir, "selenium_profile")
-                os.makedirs(profile_path, exist_ok=True)
+                os.makedirs(self.profile_path, exist_ok=True)
+
+            # ! Specify the path to the Google Chrome binary - this is tailored for this code running on Huggingface Docker Spaces
+            self.chrome_options.binary_location = '/usr/bin/google-chrome-stable'
             
             # Use the specified or default profile path
-            chrome_options.add_argument(f"user-data-dir={profile_path}")
+            self.chrome_options.add_argument(f"user-data-dir={self.profile_path}")
+            self.driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install()), options=self.chrome_options)          
 
-            self.driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install()), options=chrome_options)
-            if method is None:
-                self.driver.maximize_window()
-            self.duration = duration
+        def _normal_driver(self, method='headless'):
+            """
+            Normal ChromeDriver setup for machine with GUI (e.g. local machine).
+            """
+            self._common_driver_options(method=method)
+            self.driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install()), options=self.chrome_options)
 
         def quit(self):
             """
             Close the ChromeDriver instance.
             """
             self.driver.quit()
 
         def visit(self, url='https://huggingface.co/spaces/thinh-vu/vnstock'):
             """
             Open a specific URL in the ChromeDriver instance.
             """
-            print(f'Visiting {url}')
+            logger.info(f'Visiting {url}')
             self.driver.get(url)
-            print(self.driver.title)
+            logger.info(self.driver.title)
 
         def scroll(self, direction='down', pct=0.2, duration=2):
             """
             Scroll the page up or down by a certain percentage.
 
             Parameters:
                 - direction (str): The direction to scroll. 'up' for scrolling up and 'down' for scrolling down. Default is 'down'.
@@ -106,15 +165,15 @@
         def get_token (self):
             cookies = self.get_cookies()
             try:
                 for item in cookies:
                     if item['domain'] == '.ssi.com.vn' and item['name'] == 'token':
                         token = item['value']
                         assert isinstance(token, str)
-                        print('Token extracted successfully!')
+                        logger.info('Token extracted successfully!')
                 return token
             except Exception as e:
                 raise ValueError('Token extraction failed!') from e
         
         def wait_element(self, selector, duration=10, by=By.CSS_SELECTOR):
             """
             Wait for an element to appear on the page.
@@ -123,30 +182,30 @@
                 - selector (str): The identifier of the element to wait for. Determined using Google Chrome Inspector.
                 - duration (int): The maximum wait time for the element to appear on the page. Default is 10 seconds.
                 - by (By): The method to search for the element. Default is ID. Other methods include: NAME, XPATH, LINK_TEXT, PARTIAL_LINK_TEXT, TAG_NAME, CLASS_NAME.
             """
             try:
                 return WebDriverWait(self.driver, duration).until(EC.presence_of_element_located((by, selector)))
             except TimeoutException:
-                print(f'Element not found with {by} and selector: {selector}')
+                logger.info(f'Element not found with {by} and selector: {selector}')
                 return None
 
         def find_element(self, selector, by=By.CSS_SELECTOR):
             """
             Find a specific element on the page.
 
             Parameters:
                 - selector (str): The identifier of the element to find. Determined using Google Chrome Inspector.
                 - by (By): The method to search for the element. Default is ID. Other methods include: NAME, XPATH, LINK_TEXT, PARTIAL_LINK_TEXT, TAG_NAME, CLASS_NAME.
             """
             element = self.wait_element(selector, by=by)
             if element:
                 return element
             else:
-                print(f'Element not found with {by} and selector: {selector}')
+                logger.info(f'Element not found with {by} and selector: {selector}')
                 return None
 
         def click_element(self, selector, duration=10, by=By.CSS_SELECTOR):
             """
             Click on a specific element on the page.
 
             Parameters:
@@ -201,26 +260,7 @@
             """
             Take a screenshot of the current page.
 
             Parameters:
                 - path (str): The path to save the screenshot. Default is 'screenshot.png'.
             """
             self.driver.save_screenshot(path)
-
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
```

### Comparing `vns_explorer-1.0.4/vns_explorer/env.py` & `vns_explorer-1.0.5/vns_explorer/env.py`

 * *Files identical despite different names*

### Comparing `vns_explorer-1.0.4/vns_explorer.egg-info/PKG-INFO` & `vns_explorer-1.0.5/vns_explorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vns_explorer
-Version: 1.0.4
+Version: 1.0.5
 Summary: Discover the Unseen
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

