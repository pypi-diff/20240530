# Comparing `tmp/ctrip-helper-0.1.3.tar.gz` & `tmp/ctrip-helper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.1.3.tar", last modified: Thu May 30 02:24:34 2024, max compression
+gzip compressed data, was "ctrip-helper-0.1.4.tar", last modified: Thu May 30 02:57:33 2024, max compression
```

## Comparing `ctrip-helper-0.1.3.tar` & `ctrip-helper-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 02:24:34.420196 ctrip-helper-0.1.3/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 02:24:34.419199 ctrip-helper-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 02:24:34.405238 ctrip-helper-0.1.3/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.3/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 02:24:34.416208 ctrip-helper-0.1.3/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.3/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    25870 2024-05-30 02:24:05.000000 ctrip-helper-0.1.3/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.3/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.1.3/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.3/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4575 2024-05-29 18:45:32.000000 ctrip-helper-0.1.3/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.3/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 02:24:34.418201 ctrip-helper-0.1.3/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 02:24:34.000000 ctrip-helper-0.1.3/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 02:24:34.421193 ctrip-helper-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 02:24:30.000000 ctrip-helper-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:57:33.224723 ctrip-helper-0.1.4/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 02:57:33.222726 ctrip-helper-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 02:57:33.206770 ctrip-helper-0.1.4/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.4/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:57:33.219734 ctrip-helper-0.1.4/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.4/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    29633 2024-05-30 02:56:58.000000 ctrip-helper-0.1.4/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.4/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.1.4/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.4/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4575 2024-05-29 18:45:32.000000 ctrip-helper-0.1.4/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.4/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:57:33.221728 ctrip-helper-0.1.4/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 02:57:33.000000 ctrip-helper-0.1.4/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 02:57:33.000000 ctrip-helper-0.1.4/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 02:57:33.000000 ctrip-helper-0.1.4/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 02:57:33.000000 ctrip-helper-0.1.4/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 02:57:33.000000 ctrip-helper-0.1.4/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 02:57:33.224723 ctrip-helper-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 02:57:28.000000 ctrip-helper-0.1.4/setup.py
```

### Comparing `ctrip-helper-0.1.3/LICENSE` & `ctrip-helper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.3/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.1.4/ctrip_helper/api/desktop_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,21 @@
     yeepay2b_payment_next_button = {"locator": "xpath",
                                     "regx": '//div[@class="account-pay-main"]//button[@id="passPayButton"]'}
     is_login_button = {
         "locator": "xpath",
         "regx": '//div[@class="tl_nfes_home_header_login_wrapper_siwkn"]//button[contains(@aria-label, "我的账户")]'
     }
     is_login_span = {"locator": "xpath", "regx": '//div[@class="loginbar"]//span[@class="ctrip-username"]'}
+    account_input = {"locator": "xpath",
+                     "regx": '//div[@data-testid="accountPanel"]//input[@data-testid="accountNameInput"]'}
+    password_input = {"locator": "xpath",
+                      "regx": '//div[@data-testid="accountPanel"]//input[@data-testid="passwordInput"]'}
+    service_agreement = {"locator": "xpath",
+                         "regx": '//div[@data-testid="agreementList"]//label[@for="checkboxAgreementInput"]'}
+    login_button = {"locator": "xpath", "regx": '//div[@data-testid="accountPanel"]//input[@data-testid="loginButton"]'}
 
 
 class SeleniumApi(object):
 
     @classmethod
     def is_login(cls, driver: webdriver, username: str, platform: str, loop: int = 1, sleep: float = 0,
                  **kwargs) -> bool:
@@ -82,14 +89,82 @@
         if is_login_span:
             logger.info("{}平台用户<{}>已登录".format(platform, username))
             return True
         else:
             return False
 
     @classmethod
+    def open_login_page(cls, driver: webdriver, sleep: float = 0) -> None:
+        ctrip_login_prefix = url_map.get_url('ctrip_login_prefix')
+        ctrip_login_suffix = url_map.get_url('ctrip_login_suffix')
+        login_url = "{}{}".format(ctrip_login_prefix, ctrip_login_suffix)
+        driver.get(login_url)
+        if sleep > 0:
+            time.sleep(sleep)
+        logger.info("打开携程网页版登录页")
+
+    @classmethod
+    def enter_user_name(cls, driver: webdriver, username: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
+        input_box = get_element(
+            driver=driver, locator=UILocatorRegx.get("account_input").get("locator"),
+            regx=UILocatorRegx.get("account_input").get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if input_box:
+            # 模拟键盘操作清空输入框内容
+            input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
+            input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
+            input_box.send_keys('{}'.format(username))
+            logger.info("输入登录账号：{}".format(username))
+            return True
+        else:
+            return False
+
+    @classmethod
+    def enter_user_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
+        input_box = get_element(
+            driver=driver, locator=UILocatorRegx.get("password_input").get("locator"),
+            regx=UILocatorRegx.get("password_input").get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if input_box:
+            # 模拟键盘操作清空输入框内容
+            input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
+            input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
+            input_box.send_keys('{}'.format(password))
+            logger.info("输入登录密码：{}".format(password))
+            return True
+        else:
+            return False
+
+    @classmethod
+    def click_service_agreement(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
+        checkbox = get_element(
+            driver=driver, locator=UILocatorRegx.get("service_agreement").get("locator"),
+            regx=UILocatorRegx.get("service_agreement").get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if checkbox:
+            checkbox.click()
+            logger.info("选中【阅读并同意携程的服务协议和个人信息保护政策】")
+            return True
+        else:
+            return False
+
+    @classmethod
+    def click_login(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
+        login_button = get_element(
+            driver=driver, locator=UILocatorRegx.get("login_button").get("locator"),
+            regx=UILocatorRegx.get("login_button").get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if login_button:
+            login_button.click()
+            logger.info("点击登录页面的【登录】按钮")
+            return True
+        else:
+            return False
+
+    @classmethod
     def open_order_query_home_with_flight(cls, driver: webdriver, sleep: float = 0) -> None:
         driver.get(url_map.get_url('order_query_home_with_flight'))
         if sleep > 0:
             time.sleep(sleep)
         logger.info("打开机票订单查询首页")
 
     @classmethod
```

### Comparing `ctrip-helper-0.1.3/ctrip_helper/api/http_api.py` & `ctrip-helper-0.1.4/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.3/ctrip_helper/config.py` & `ctrip-helper-0.1.4/ctrip_helper/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,14 +43,17 @@
     "order_query_home_with_flight": "https://my.ctrip.com/myinfo/flight",
     # 订单详情页，?oid=32665635142
     "flight_order_details": "https://flights.ctrip.com/online/orderdetail/index",
     # 携程机票安全支付界面，?tradeNo=20240529144727TP1193583667800373067821
     "safe_payment_home": "https://secure.ctrip.com/webapp/payment8/index",
     # 易宝会员支付账号输入界面
     "yeepay2b_cash_desk": "https://cashdesk.yeepay.com/bc-cashier/bcnewpc/request",
+    # 登录页
+    "ctrip_login_prefix": "https://passport.ctrip.com/user/login",
+    "ctrip_login_suffix": "{}?BackUrl=https%3A%2F%2Fwww.ctrip.com%2F#ctm_ref=c_ph_login_buttom",
 }
 
 airline_request_params_template = {
     "adultCount": 1,
     "childCount": 0,
     "infantCount": 0,
     "flightWay": "S",  # OW: 单程, S:
```

### Comparing `ctrip-helper-0.1.3/ctrip_helper/http_client.py` & `ctrip-helper-0.1.4/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.3/ctrip_helper/libs.py` & `ctrip-helper-0.1.4/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.3/ctrip_helper/utils.py` & `ctrip-helper-0.1.4/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.3/setup.py` & `ctrip-helper-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.1.3',
+    version='0.1.4',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

