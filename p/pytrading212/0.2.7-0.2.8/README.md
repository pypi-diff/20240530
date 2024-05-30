# Comparing `tmp/pytrading212-0.2.7.tar.gz` & `tmp/pytrading212-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrading212-0.2.7.tar", max compression
+gzip compressed data, was "pytrading212-0.2.8.tar", max compression
```

## Comparing `pytrading212-0.2.7.tar` & `pytrading212-0.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2024-04-03 11:11:26.032599 pytrading212-0.2.7/LICENSE
--rw-r--r--   0        0        0    11829 2024-04-03 11:11:26.032599 pytrading212-0.2.7/README.md
--rw-r--r--   0        0        0      410 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      377 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/__init__.py
--rw-r--r--   0        0        0      214 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/console.py
--rw-r--r--   0        0        0     5691 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/constants.py
--rw-r--r--   0        0        0     2473 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/instrument.py
--rw-r--r--   0        0        0     5487 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/order.py
--rw-r--r--   0        0        0      236 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/position.py
--rw-r--r--   0        0        0    14171 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/trading212.py
--rw-r--r--   0        0        0      520 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/utils.py
--rw-r--r--   0        0        0    12635 1970-01-01 00:00:00.000000 pytrading212-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-30 05:20:19.408819 pytrading212-0.2.8/LICENSE
+-rw-r--r--   0        0        0    11829 2024-05-30 05:20:19.408819 pytrading212-0.2.8/README.md
+-rw-r--r--   0        0        0      410 2024-05-30 05:20:19.408819 pytrading212-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      377 2024-05-30 05:20:19.412819 pytrading212-0.2.8/pytrading212/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-30 05:20:19.412819 pytrading212-0.2.8/pytrading212/console.py
+-rw-r--r--   0        0        0     4962 2024-05-30 05:20:19.412819 pytrading212-0.2.8/pytrading212/constants.py
+-rw-r--r--   0        0        0     2473 2024-05-30 05:20:19.412819 pytrading212-0.2.8/pytrading212/instrument.py
+-rw-r--r--   0        0        0     5487 2024-05-30 05:20:19.412819 pytrading212-0.2.8/pytrading212/order.py
+-rw-r--r--   0        0        0      236 2024-05-30 05:20:19.412819 pytrading212-0.2.8/pytrading212/position.py
+-rw-r--r--   0        0        0    13831 2024-05-30 05:20:19.412819 pytrading212-0.2.8/pytrading212/trading212.py
+-rw-r--r--   0        0        0      520 2024-05-30 05:20:19.412819 pytrading212-0.2.8/pytrading212/utils.py
+-rw-r--r--   0        0        0    12635 1970-01-01 00:00:00.000000 pytrading212-0.2.8/PKG-INFO
```

### Comparing `pytrading212-0.2.7/LICENSE` & `pytrading212-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrading212-0.2.7/README.md` & `pytrading212-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pytrading212-0.2.7/pytrading212/instrument.py` & `pytrading212-0.2.8/pytrading212/instrument.py`

 * *Files identical despite different names*

### Comparing `pytrading212-0.2.7/pytrading212/order.py` & `pytrading212-0.2.8/pytrading212/order.py`

 * *Files identical despite different names*

### Comparing `pytrading212-0.2.7/pytrading212/trading212.py` & `pytrading212-0.2.8/pytrading212/trading212.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,30 +45,22 @@
             console.log("Closing 'Cookies Popup'")
             self.driver.find_element(By.CLASS_NAME, constants.CLASS_COOKIES_NOTICE_BUTTON).click()
         except NoSuchElementException:
             pass  # ignore
 
         console.log("Authenticating")
 
-        WebDriverWait(self.driver, 120).until(expected_conditions.visibility_of_element_located((By.NAME, "email")))
+        WebDriverWait(self.driver, 120).until(expected_conditions.visibility_of_element_located((By.XPATH, constants.XPATH_EMAIL)))
 
         # Authenticate
-        self.driver.find_element(By.NAME, "email").send_keys(email)
-        self.driver.find_element(By.NAME, "password").send_keys(password)
+        self.driver.find_element(By.XPATH, constants.XPATH_EMAIL).send_keys(email)
+        self.driver.find_element(By.XPATH, constants.XPATH_PASSWORD).send_keys(password)
 
         # Click login button
-        self.driver.find_element(By.CLASS_NAME, constants.CLASS_LOGIN_BUTTON).click()
-
-        # Close new app button, should be removed later
-        try:
-            WebDriverWait(self.driver, 30).until(expected_conditions.visibility_of_element_located(
-                (By.CSS_SELECTOR, constants.SELECTOR_NEW_APP)))
-            self.driver.find_element(By.CSS_SELECTOR, constants.SELECTOR_NEW_APP).click()
-        except NoSuchElementException:
-            pass
+        self.driver.find_element(By.XPATH, constants.XPATH_LOGIN_BUTTON).click()
 
         self.user_agent = self.driver.execute_script("return navigator.userAgent;")
 
         # Switch to get also DEMO token
         self.switch()
         # Get session cookie
         cookies = self.driver.get_cookies()
```

### Comparing `pytrading212-0.2.7/pytrading212/utils.py` & `pytrading212-0.2.8/pytrading212/utils.py`

 * *Files identical despite different names*

### Comparing `pytrading212-0.2.7/PKG-INFO` & `pytrading212-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrading212
-Version: 0.2.7
+Version: 0.2.8
 Summary: Unofficial Trading212 API
 License: MIT
 Author: HellAmbro
 Author-email: frambrosini1998@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytrading212 Version: 0.2.7 Summary: Unofficial
+Metadata-Version: 2.1 Name: pytrading212 Version: 0.2.8 Summary: Unofficial
 Trading212 API License: MIT Author: HellAmbro Author-email:
 frambrosini1998@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

