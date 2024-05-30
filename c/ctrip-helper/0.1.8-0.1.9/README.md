# Comparing `tmp/ctrip-helper-0.1.8.tar.gz` & `tmp/ctrip-helper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.1.8.tar", last modified: Thu May 30 09:02:09 2024, max compression
+gzip compressed data, was "ctrip-helper-0.1.9.tar", last modified: Thu May 30 10:17:59 2024, max compression
```

## Comparing `ctrip-helper-0.1.8.tar` & `ctrip-helper-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 09:02:09.368098 ctrip-helper-0.1.8/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 09:02:09.366103 ctrip-helper-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 09:02:09.352141 ctrip-helper-0.1.8/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.8/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 09:02:09.363112 ctrip-helper-0.1.8/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.8/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30295 2024-05-30 09:01:40.000000 ctrip-helper-0.1.8/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.8/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.1.8/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.8/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4575 2024-05-30 08:55:03.000000 ctrip-helper-0.1.8/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.8/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 09:02:09.365116 ctrip-helper-0.1.8/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 09:02:09.000000 ctrip-helper-0.1.8/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 09:02:09.000000 ctrip-helper-0.1.8/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 09:02:09.000000 ctrip-helper-0.1.8/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 09:02:09.000000 ctrip-helper-0.1.8/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 09:02:09.000000 ctrip-helper-0.1.8/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 09:02:09.368098 ctrip-helper-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 09:01:58.000000 ctrip-helper-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:17:59.884139 ctrip-helper-0.1.9/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 10:17:59.883142 ctrip-helper-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 10:17:59.867185 ctrip-helper-0.1.9/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.9/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:17:59.880150 ctrip-helper-0.1.9/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.9/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30232 2024-05-30 10:16:18.000000 ctrip-helper-0.1.9/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.9/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.1.9/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.9/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4575 2024-05-30 10:17:44.000000 ctrip-helper-0.1.9/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.9/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:17:59.882145 ctrip-helper-0.1.9/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 10:17:59.000000 ctrip-helper-0.1.9/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 10:17:59.884139 ctrip-helper-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 10:17:53.000000 ctrip-helper-0.1.9/setup.py
```

### Comparing `ctrip-helper-0.1.8/LICENSE` & `ctrip-helper-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.8/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.1.9/ctrip_helper/api/desktop_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 # Author:       mfkifhss2023
 # CreateDate:   2024/05/29
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import re
 import time
+from enum import Enum
 from decimal import Decimal
 from selenium import webdriver
 from ctrip_helper.libs import logger
 from ctrip_helper.config import url_map
+from ctrip_helper.libs import get_element
 from selenium.webdriver.common.keys import Keys
-from ctrip_helper.libs import get_element, EnumMetaClass
 from ctrip_helper.utils import is_later_than_current_time
 
 
-class UILocatorRegx(EnumMetaClass):
+class UILocatorRegx(Enum):
     all_orders_select_box = {"locator": "xpath",
                              "regx": '//ul[@class="fix_myctrip_order_layer"]//div[@class="select-box"]'}
     order_id_input_box = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//input[@id="searchBookingNum"]'}
     order_query_button = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//button[@class="btn_sel"]'}
     order_status_with_list = {"locator": "xpath",
                               "regx": '//ul[@class="t_body"]//span[@class="order-price-status-title"]'}
     order_price = {"locator": "xpath", "regx": '//li[@class="item"]//div[@class="order-price-detail"]'}
@@ -73,23 +74,23 @@
 class SeleniumApi(object):
 
     @classmethod
     def is_login(cls, driver: webdriver, username: str, platform: str, loop: int = 1, sleep: float = 0,
                  **kwargs) -> bool:
         """是否已登录"""
         is_login_button = get_element(
-            driver=driver, locator=UILocatorRegx.get("is_login_button").get("locator"),
-            regx=UILocatorRegx.get("is_login_button").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.is_login_button.value.get("locator"),
+            regx=UILocatorRegx.is_login_button.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if is_login_button:
             logger.info("{}平台用户<{}>已登录".format(platform, username))
             return True
         is_login_span = get_element(
-            driver=driver, locator=UILocatorRegx.get("is_login_span").get("locator"),
-            regx=UILocatorRegx.get("is_login_span").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.is_login_span.value.get("locator"),
+            regx=UILocatorRegx.is_login_span.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if is_login_span:
             logger.info("{}平台用户<{}>已登录".format(platform, username))
             return True
         else:
             return False
 
@@ -102,75 +103,75 @@
         if sleep > 0:
             time.sleep(sleep)
         logger.info("打开携程网页版登录页")
 
     @classmethod
     def enter_user_name(cls, driver: webdriver, username: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         input_box = get_element(
-            driver=driver, locator=UILocatorRegx.get("account_input").get("locator"),
-            regx=UILocatorRegx.get("account_input").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.account_input.value.get("locator"),
+            regx=UILocatorRegx.account_input.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if input_box:
             # 模拟键盘操作清空输入框内容
             input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
             input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
             input_box.send_keys('{}'.format(username))
             logger.info("输入登录账号：{}".format(username))
             return True
         else:
             return False
 
     @classmethod
     def enter_user_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         input_box = get_element(
-            driver=driver, locator=UILocatorRegx.get("password_input").get("locator"),
-            regx=UILocatorRegx.get("password_input").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.password_input.value.get("locator"),
+            regx=UILocatorRegx.password_input.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if input_box:
             # 模拟键盘操作清空输入框内容
             input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
             input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
             input_box.send_keys('{}'.format(password))
             logger.info("输入登录密码：{}".format(password))
             return True
         else:
             return False
 
     @classmethod
     def click_service_agreement(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         checkbox = get_element(
-            driver=driver, locator=UILocatorRegx.get("service_agreement").get("locator"),
-            regx=UILocatorRegx.get("service_agreement").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.service_agreement.value.get("locator"),
+            regx=UILocatorRegx.service_agreement.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if checkbox:
             checkbox.click()
             logger.info("选中【阅读并同意携程的服务协议和个人信息保护政策】")
             return True
         else:
             return False
 
     @classmethod
     def click_login(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         login_button = get_element(
-            driver=driver, locator=UILocatorRegx.get("login_button").get("locator"),
-            regx=UILocatorRegx.get("login_button").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.login_button.value.get("locator"),
+            regx=UILocatorRegx.login_button.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if login_button:
             login_button.click()
             logger.info("点击登录页面的【登录】按钮")
             return True
         else:
             return False
 
     @classmethod
     def is_exist_slider_verify(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         slider_verify = get_element(
-            driver=driver, locator=UILocatorRegx.get("slider_verify").get("locator"),
-            regx=UILocatorRegx.get("slider_verify").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.slider_verify.value.get("locator"),
+            regx=UILocatorRegx.slider_verify.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if slider_verify:
             logger.info("当前页面：{} 出现了滑块验证码".format(current_url))
             return True
         else:
             return False
 
@@ -180,100 +181,100 @@
         if sleep > 0:
             time.sleep(sleep)
         logger.info("打开机票订单查询首页")
 
     @classmethod
     def click_more_filter_conditions(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         more_filter_expand = get_element(
-            driver=driver, locator=UILocatorRegx.get("all_orders_select_box").get("locator"),
-            regx=UILocatorRegx.get("all_orders_select_box").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.all_orders_select_box.value.get("locator"),
+            regx=UILocatorRegx.all_orders_select_box.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if more_filter_expand:
             more_filter_expand.click()
             logger.info("选择【更多筛选条件】，展开条件列表")
             return True
         else:
             return False
 
     @classmethod
     def enter_order_id(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         input_box = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_id_input_box").get("locator"),
-            regx=UILocatorRegx.get("order_id_input_box").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.order_id_input_box.value.get("locator"),
+            regx=UILocatorRegx.order_id_input_box.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if input_box:
             # 模拟键盘操作清空输入框内容
             input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
             input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
             input_box.send_keys('{}'.format(order_id))
             logger.info("输入查询订单号：{}".format(order_id))
             return True
         else:
             return False
 
     @classmethod
     def click_order_query(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         order_query_button = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_query_button").get("locator"),
-            regx=UILocatorRegx.get("order_query_button").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.order_query_button.value.get("locator"),
+            regx=UILocatorRegx.order_query_button.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if order_query_button:
             order_query_button.click()
             logger.info("点击【查询】按钮")
             return True
         else:
             return False
 
     @classmethod
     def get_order_status(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> str:
         order_status = ""
         order_status_element = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_status_with_list").get("locator"),
-            regx=UILocatorRegx.get("order_status_with_list").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.order_status_with_list.value.get("locator"),
+            regx=UILocatorRegx.order_status_with_list.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if order_status_element:
             order_status = order_status_element.text.strip()
             logger.info("获取订单的状态为：{}".format(order_status))
         return order_status
 
     @classmethod
     def get_order_amonut_with_query_list(cls, driver: webdriver, order_id: str, loop: int = 1,
                                          sleep: float = 0, **kwargs) -> Decimal:
         order_amonut = "0.00"
         order_amonut_element = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
-            regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.order_price.value.get("locator"),
+            regx=UILocatorRegx.order_price.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if order_amonut_element:
             text = order_amonut_element.text.strip()
             logger.info("从查询列表中获取订单: {} 的金额：{}".format(order_id, text))
             order_amonut = text.split("¥")[-1]
         return Decimal(order_amonut)
 
     @classmethod
     def click_order_amonut_with_query_list(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         order_amonut_element = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
-            regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.order_price.value.get("locator"),
+            regx=UILocatorRegx.order_price.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if order_amonut_element:
             order_amonut_element.click()
             logger.info("点击订单金额，进入订单详情界面")
             return True
         else:
             return False
 
     @classmethod
     def click_to_payment(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
         if current_url.startswith(local_url) is True:
             to_payment_button = get_element(
-                driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
-                regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep, **kwargs
+                driver=driver, locator=UILocatorRegx.order_price.value.get("locator"),
+                regx=UILocatorRegx.order_price.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if to_payment_button:
                 to_payment_button.click()
                 logger.info("点击【去支付】，进入订单支付界面")
                 return True
             else:
                 return False
@@ -283,60 +284,60 @@
 
     @classmethod
     def click_order_cancel(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
         if current_url.startswith(local_url) is True:
             order_cancel_button = get_element(
-                driver=driver, locator=UILocatorRegx.get("order_to_cancel").get("locator"),
-                regx=UILocatorRegx.get("order_to_cancel").get("regx"), loop=loop, sleep=sleep, **kwargs
+                driver=driver, locator=UILocatorRegx.order_to_cancel.value.get("locator"),
+                regx=UILocatorRegx.order_to_cancel.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if order_cancel_button:
                 order_cancel_button.click()
                 logger.info("点击【取消订单】，接下来会出现【取消提示】小弹框")
                 return True
             else:
                 return False
         else:
             logger.warn("当前订单详情页面: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
             return False
 
     @classmethod
     def click_order_continue_cancel(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         continue_cance_button = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_continue_cancel").get("locator"),
-            regx=UILocatorRegx.get("order_continue_cancel").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.order_continue_cancel.value.get("locator"),
+            regx=UILocatorRegx.order_continue_cancel.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if continue_cance_button:
             continue_cance_button.click()
             logger.info("点击【继续取消】，接下来会出现【知道了】小弹框")
             return True
         else:
             return False
 
     @classmethod
     def is_order_cancel_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         got_it_button = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_cancel_got_it.value").get("locator"),
-            regx=UILocatorRegx.get("order_cancel_got_it").get("regx"), sleep=sleep, loop=loop, **kwargs
+            driver=driver, locator=UILocatorRegx.order_cancel_got_it.value.value.get("locator"),
+            regx=UILocatorRegx.order_cancel_got_it.value.get("regx"), sleep=sleep, loop=loop, **kwargs
         )
         if got_it_button:
             return True
         else:
             return False
 
     @classmethod
     def get_order_amount_with_safe_payment_home(cls, driver: webdriver, loop: int = 1, sleep: float = 0,
                                                 **kwargs) -> Decimal:
         order_payment_amount = "0.00"
         current_url = driver.current_url
         if current_url.startswith(url_map.get("safe_payment_home")) is True:
             order_payment_amount_element = get_element(
-                driver=driver, locator=UILocatorRegx.get("order_payment_amount").get("locator"),
-                regx=UILocatorRegx.get("order_payment_amount").get("regx"), loop=loop, sleep=sleep, **kwargs
+                driver=driver, locator=UILocatorRegx.order_payment_amount.value.get("locator"),
+                regx=UILocatorRegx.order_payment_amount.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if order_payment_amount_element:
                 order_payment_amount = order_payment_amount_element.text.strip()
                 logger.info("获取订单的支付金额为：{}".format(order_payment_amount))
         else:
             logger.warning("当前的界面：{} 不是订单安全支付界面".format(current_url))
         return Decimal(order_payment_amount)
@@ -344,21 +345,17 @@
     @classmethod
     def is_cancel_order(cls, driver: webdriver, out_total_amount: str, amount_loss_limit: str, profit_cap: str,
                         passenger_number: int, platform: str, loop: int = 1, sleep: float = 0,
                         discount_amount: str = None, **kwargs) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = ""
-        status_sub_title_element = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_status_sub_title").get("locator"),
-            regx=UILocatorRegx.get("order_status_sub_title").get("regx"), loop=loop, sleep=sleep, **kwargs
-        )
         booking_amount_element = get_element(
-            driver=driver, locator=UILocatorRegx.get("order_status_booking_amount").get("locator"),
-            regx=UILocatorRegx.get("order_status_booking_amount").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.order_status_booking_amount.value.get("locator"),
+            regx=UILocatorRegx.order_status_booking_amount.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if booking_amount_element:
             booking_amount_text = booking_amount_element.text.strip()
             # 使用 findall 获取所有匹配项
             amount_match = re.search(r"¥(\d+)", booking_amount_text)
             if amount_match:
                 amount_str = amount_match.group(1)
@@ -394,14 +391,18 @@
                         return flag, remark
             else:
                 remark = "从订单详情页面获取订单过期时间和订单金额有异常"
                 logger.warning(remark)
         else:
             remark = "订单详情页面中未找到订单金额元素"
             logger.warning(remark)
+        status_sub_title_element = get_element(
+            driver=driver, locator=UILocatorRegx.order_status_sub_title.value.get("locator"),
+            regx=UILocatorRegx.order_status_sub_title.value.get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
         if status_sub_title_element:
             sub_title_text = status_sub_title_element.text.strip()
             # 使用 findall 获取所有匹配项
             time_match = re.search(r"(\d{2}:\d{2})", sub_title_text)
             if time_match:
                 time_str = time_match.group(1)
                 logger.info("从订单获取到的过期时间为：{}".format(time_str))
@@ -418,99 +419,99 @@
             remark = "从订单详情页面中未找到订单过期时间元素"
         logger.warning(remark)
         return flag, remark
 
     @classmethod
     def is_wallet_disable(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         wallet_disable_element = get_element(
-            driver=driver, locator=UILocatorRegx.get("wallet_disable").get("locator"),
-            regx=UILocatorRegx.get("wallet_disable").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.wallet_disable.value.get("locator"),
+            regx=UILocatorRegx.wallet_disable.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if wallet_disable_element:
             logger.warning("当前订单: {} 钱包不可用，需要切换至其他支付方式".format(order_id))
             return True
         else:
             return False
 
     @classmethod
     def get_wallet_balance(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> Decimal:
         wallet_balance = "0.00"
         wallet_balance_element = get_element(
-            driver=driver, locator=UILocatorRegx.get("wallet_balance").get("locator"),
-            regx=UILocatorRegx.get("wallet_balance").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.wallet_balance.value.get("locator"),
+            regx=UILocatorRegx.wallet_balance.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if wallet_balance_element:
             text = wallet_balance_element.text.strip()
             logger.info("获取账号礼品卡{}".format(text))
             wallet_balance = text.split("¥")[-1]
         return Decimal(wallet_balance)
 
     @classmethod
     def click_use_wallet(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         use_wallet_switch = get_element(
-            driver=driver, locator=UILocatorRegx.get("use_wallet").get("locator"),
-            regx=UILocatorRegx.get("use_wallet").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.use_wallet.value.get("locator"),
+            regx=UILocatorRegx.use_wallet.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if use_wallet_switch:
             use_wallet_switch.click()
             logger.info("选择使用钱包支付")
             return True
         else:
             return False
 
     @classmethod
     def click_wallet_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         immediately_payment_button = get_element(
-            driver=driver, locator=UILocatorRegx.get("wallet_immediately_payment").get("locator"),
-            regx=UILocatorRegx.get("use_wallet").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.wallet_immediately_payment.value.get("locator"),
+            regx=UILocatorRegx.use_wallet.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if immediately_payment_button:
             immediately_payment_button.click()
             logger.info("点击钱包【立即支付】")
             return True
         else:
             return False
 
     @classmethod
     def click_use_yeepay2b(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         use_yeepay2b_switch = get_element(
-            driver=driver, locator=UILocatorRegx.get("use_yeepay2b_pyament").get("locator"),
-            regx=UILocatorRegx.get("use_yeepay2b_pyament").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.use_yeepay2b_pyament.value.get("locator"),
+            regx=UILocatorRegx.use_yeepay2b_pyament.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if use_yeepay2b_switch:
             use_yeepay2b_switch.click()
             logger.info("选择使用易宝会员支付")
             return True
         else:
             return False
 
     @classmethod
     def click_yeepay2b_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         immediately_payment_button = get_element(
-            driver=driver, locator=UILocatorRegx.get("yeepay2b_immediately_payment").get("locator"),
-            regx=UILocatorRegx.get("yeepay2b_immediately_payment").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.yeepay2b_immediately_payment.value.get("locator"),
+            regx=UILocatorRegx.yeepay2b_immediately_payment.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if immediately_payment_button:
             immediately_payment_button.click()
             logger.info("点击【易宝支付】按钮")
             return True
         else:
             return False
 
     @classmethod
     def enter_payment_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0,
                                **kwargs) -> bool:
         is_exist_pop_box = get_element(
-            driver=driver, locator=UILocatorRegx.get("password_pop_box").get("locator"),
-            regx=UILocatorRegx.get("password_pop_box").get("regx"), sleep=sleep, loop=loop, **kwargs
+            driver=driver, locator=UILocatorRegx.password_pop_box.value.get("locator"),
+            regx=UILocatorRegx.password_pop_box.value.get("regx"), sleep=sleep, loop=loop, **kwargs
         )
         if is_exist_pop_box:
             first_password_inout_box = get_element(
-                driver=driver, locator=UILocatorRegx.get("first_password_input_box").get("locator"),
-                regx=UILocatorRegx.get("first_password_input_box").get("regx"), sleep=sleep, loop=loop, **kwargs
+                driver=driver, locator=UILocatorRegx.first_password_input_box.value.get("locator"),
+                regx=UILocatorRegx.first_password_input_box.value.get("regx"), sleep=sleep, loop=loop, **kwargs
             )
             if first_password_inout_box:
                 if not isinstance(password, str):
                     password = str(password)
                 first_password_inout_box.click()
                 for i in password:
                     driver.send_keys(i)
@@ -529,16 +530,16 @@
         return True
 
     @classmethod
     def enter_yeepay2b_account(cls, driver: webdriver, account: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         if current_url.startswith(url_map.get("yeepay2b_cash_desk")) is True:
             input_box = get_element(
-                driver=driver, locator=UILocatorRegx.get("yeepay2b_accout_input_box").get("locator"),
-                regx=UILocatorRegx.get("yeepay2b_accout_input_box").get("regx"), loop=loop, sleep=sleep, **kwargs
+                driver=driver, locator=UILocatorRegx.yeepay2b_accout_input_box.value.get("locator"),
+                regx=UILocatorRegx.yeepay2b_accout_input_box.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if input_box:
                 # 模拟键盘操作清空输入框内容
                 input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
                 input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
                 input_box.send_keys('{}'.format(account))
                 logger.info("输入的易宝会员账号：{}".format(account))
@@ -548,32 +549,32 @@
         else:
             return False
 
     @classmethod
     def enter_yeepay2b_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0,
                                 **kwargs) -> bool:
         input_box = get_element(
-            driver=driver, locator=UILocatorRegx.get("yeepay2b_password_input_box").get("locator"),
-            regx=UILocatorRegx.get("yeepay2b_password_input_box").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.yeepay2b_password_input_box.value.get("locator"),
+            regx=UILocatorRegx.yeepay2b_password_input_box.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if input_box:
             # 模拟键盘操作清空输入框内容
             input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
             input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
             input_box.send_keys('{}'.format(password))
             logger.info("输入的易宝会员账号密码：{}".format(password))
             return True
         else:
             return False
 
     @classmethod
     def click_yeepay2b_payment_next(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         next_button = get_element(
-            driver=driver, locator=UILocatorRegx.get("yeepay2b_payment_next_button").get("locator"),
-            regx=UILocatorRegx.get("yeepay2b_payment_next_button").get("regx"), loop=loop, sleep=sleep, **kwargs
+            driver=driver, locator=UILocatorRegx.yeepay2b_payment_next_button.value.get("locator"),
+            regx=UILocatorRegx.yeepay2b_payment_next_button.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if next_button:
             next_button.click()
             logger.info("易宝支付收银台界面点击【下一步】")
             return True
         else:
             return False
```

### Comparing `ctrip-helper-0.1.8/ctrip_helper/api/http_api.py` & `ctrip-helper-0.1.9/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.8/ctrip_helper/config.py` & `ctrip-helper-0.1.9/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.8/ctrip_helper/http_client.py` & `ctrip-helper-0.1.9/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.8/ctrip_helper/libs.py` & `ctrip-helper-0.1.9/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.8/ctrip_helper/utils.py` & `ctrip-helper-0.1.9/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.8/setup.py` & `ctrip-helper-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.1.8',
+    version='0.1.9',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

