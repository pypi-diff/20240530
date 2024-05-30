# Comparing `tmp/ctrip-helper-0.1.1.tar.gz` & `tmp/ctrip-helper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.1.1.tar", last modified: Wed May 29 18:23:36 2024, max compression
+gzip compressed data, was "ctrip-helper-0.1.2.tar", last modified: Wed May 29 18:49:02 2024, max compression
```

## Comparing `ctrip-helper-0.1.1.tar` & `ctrip-helper-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 18:23:36.434348 ctrip-helper-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 18:23:36.433351 ctrip-helper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 18:23:36.420385 ctrip-helper-0.1.1/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.1/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 18:23:36.430359 ctrip-helper-0.1.1/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.1/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    23858 2024-05-29 18:23:28.000000 ctrip-helper-0.1.1/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.1/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.1.1/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.1/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.1.1/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.1/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 18:23:36.432353 ctrip-helper-0.1.1/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 18:23:36.435345 ctrip-helper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 18:23:32.000000 ctrip-helper-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:49:02.560474 ctrip-helper-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 18:49:02.559473 ctrip-helper-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 18:49:02.547505 ctrip-helper-0.1.2/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.2/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:49:02.556489 ctrip-helper-0.1.2/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.2/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    24596 2024-05-29 18:48:23.000000 ctrip-helper-0.1.2/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.2/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.1.2/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.2/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4575 2024-05-29 18:45:32.000000 ctrip-helper-0.1.2/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.2/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:49:02.557478 ctrip-helper-0.1.2/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 18:49:02.000000 ctrip-helper-0.1.2/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:49:02.560474 ctrip-helper-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 18:48:57.000000 ctrip-helper-0.1.2/setup.py
```

### Comparing `ctrip-helper-0.1.1/LICENSE` & `ctrip-helper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.1/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.1.2/ctrip_helper/api/desktop_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,186 +63,187 @@
     def open_order_query_home_with_flight(cls, driver: webdriver, sleep: float = 0) -> None:
         driver.get(url_map.get_url('order_query_home_with_flight'))
         if sleep > 0:
             time.sleep(sleep)
         logger.info("打开机票订单查询首页")
 
     @classmethod
-    def click_more_filter_conditions(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_more_filter_conditions(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         more_filter_expand = get_element(
             driver=driver, locator=UILocatorRegx.get("all_orders_select_box").get("locator"),
-            regx=UILocatorRegx.get("all_orders_select_box").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("all_orders_select_box").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if more_filter_expand:
             more_filter_expand.click()
             logger.info("选择【更多筛选条件】，展开条件列表")
             return True
         else:
             return False
 
     @classmethod
-    def enter_order_id(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
+    def enter_order_id(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         input_box = get_element(
             driver=driver, locator=UILocatorRegx.get("order_id_input_box").get("locator"),
-            regx=UILocatorRegx.get("order_id_input_box").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("order_id_input_box").get("regx"), loop=loop, sleep=sleep, **kwargs
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
-    def click_order_query(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_order_query(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         order_query_button = get_element(
             driver=driver, locator=UILocatorRegx.get("order_query_button").get("locator"),
-            regx=UILocatorRegx.get("order_query_button").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("order_query_button").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if order_query_button:
             order_query_button.click()
             logger.info("点击【查询】按钮")
             return True
         else:
             return False
 
     @classmethod
-    def get_order_status(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> str:
+    def get_order_status(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> str:
         order_status = ""
         order_status_element = get_element(
             driver=driver, locator=UILocatorRegx.get("order_status_with_list").get("locator"),
-            regx=UILocatorRegx.get("order_status_with_list").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("order_status_with_list").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if order_status_element:
             order_status = order_status_element.text.strip()
             logger.info("获取订单的状态为：{}".format(order_status))
         return order_status
 
     @classmethod
     def get_order_amonut_with_query_list(cls, driver: webdriver, order_id: str, loop: int = 1,
-                                         sleep: float = 0) -> Decimal:
+                                         sleep: float = 0, **kwargs) -> Decimal:
         order_amonut = "0.00"
         order_amonut_element = get_element(
             driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
-            regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if order_amonut_element:
             text = order_amonut_element.text.strip()
             logger.info("从查询列表中获取订单: {} 的金额：{}".format(order_id, text))
             order_amonut = text.split("¥")[-1]
         return Decimal(order_amonut)
 
     @classmethod
-    def click_order_amonut_with_query_list(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_order_amonut_with_query_list(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         order_amonut_element = get_element(
             driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
-            regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if order_amonut_element:
             order_amonut_element.click()
             logger.info("点击订单金额，进入订单详情界面")
             return True
         else:
             return False
 
     @classmethod
-    def click_to_payment(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
+    def click_to_payment(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
         if current_url.startswith(local_url) is True:
             to_payment_button = get_element(
                 driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
-                regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep
+                regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if to_payment_button:
                 to_payment_button.click()
                 logger.info("点击【去支付】，进入订单支付界面")
                 return True
             else:
                 return False
         else:
             logger.warn("当前订单详情页面: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
             return False
 
     @classmethod
-    def click_order_cancel(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
+    def click_order_cancel(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
         if current_url.startswith(local_url) is True:
             order_cancel_button = get_element(
                 driver=driver, locator=UILocatorRegx.get("order_to_cancel").get("locator"),
-                regx=UILocatorRegx.get("order_to_cancel").get("regx"), loop=loop, sleep=sleep
+                regx=UILocatorRegx.get("order_to_cancel").get("regx"), loop=loop, sleep=sleep, **kwargs
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
-    def click_order_continue_cancel(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_order_continue_cancel(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         continue_cance_button = get_element(
             driver=driver, locator=UILocatorRegx.get("order_continue_cancel").get("locator"),
-            regx=UILocatorRegx.get("order_continue_cancel").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("order_continue_cancel").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if continue_cance_button:
             continue_cance_button.click()
             logger.info("点击【继续取消】，接下来会出现【知道了】小弹框")
             return True
         else:
             return False
 
     @classmethod
-    def is_order_cancel_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def is_order_cancel_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         got_it_button = get_element(
             driver=driver, locator=UILocatorRegx.get("order_cancel_got_it.value").get("locator"),
-            regx=UILocatorRegx.get("order_cancel_got_it").get("regx"), sleep=sleep, loop=loop
+            regx=UILocatorRegx.get("order_cancel_got_it").get("regx"), sleep=sleep, loop=loop, **kwargs
         )
         if got_it_button:
             return True
         else:
             return False
 
     @classmethod
-    def get_order_amount_with_safe_payment_home(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> Decimal:
+    def get_order_amount_with_safe_payment_home(cls, driver: webdriver, loop: int = 1, sleep: float = 0,
+                                                **kwargs) -> Decimal:
         order_payment_amount = "0.00"
         current_url = driver.current_url
         if current_url.startswith(url_map.get("safe_payment_home")) is True:
             order_payment_amount_element = get_element(
                 driver=driver, locator=UILocatorRegx.get("order_payment_amount").get("locator"),
-                regx=UILocatorRegx.get("order_payment_amount").get("regx"), loop=loop, sleep=sleep
+                regx=UILocatorRegx.get("order_payment_amount").get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if order_payment_amount_element:
                 order_payment_amount = order_payment_amount_element.text.strip()
                 logger.info("获取订单的支付金额为：{}".format(order_payment_amount))
         else:
             logger.warning("当前的界面：{} 不是订单安全支付界面".format(current_url))
         return Decimal(order_payment_amount)
 
     @classmethod
     def is_cancel_order(cls, driver: webdriver, out_total_amount: str, amount_loss_limit: str, profit_cap: str,
                         passenger_number: int, platform: str, loop: int = 1, sleep: float = 0,
-                        discount_amount: str = None) -> tuple:
+                        discount_amount: str = None, **kwargs) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = ""
         status_sub_title_element = get_element(
             driver=driver, locator=UILocatorRegx.get("order_status_sub_title").get("locator"),
-            regx=UILocatorRegx.get("order_status_sub_title").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("order_status_sub_title").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         booking_amount_element = get_element(
             driver=driver, locator=UILocatorRegx.get("order_status_booking_amount").get("locator"),
-            regx=UILocatorRegx.get("order_status_booking_amount").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("order_status_booking_amount").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if booking_amount_element:
             booking_amount_text = booking_amount_element.text.strip()
             # 使用 findall 获取所有匹配项
             amount_match = re.search(r"¥(\d+)", booking_amount_text)
             if amount_match:
                 amount_str = amount_match.group(1)
@@ -300,100 +301,101 @@
                 remark = "从文案<{}>中没有获取订单过期时间".format(sub_title_text)
         else:
             remark = "从订单详情页面中未找到订单过期时间元素"
         logger.warning(remark)
         return flag, remark
 
     @classmethod
-    def is_wallet_disable(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
+    def is_wallet_disable(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         wallet_disable_element = get_element(
             driver=driver, locator=UILocatorRegx.get("wallet_disable").get("locator"),
-            regx=UILocatorRegx.get("wallet_disable").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("wallet_disable").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if wallet_disable_element:
             logger.warning("当前订单: {} 钱包不可用，需要切换至其他支付方式".format(order_id))
             return True
         else:
             return False
 
     @classmethod
-    def get_wallet_balance(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> Decimal:
+    def get_wallet_balance(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> Decimal:
         wallet_balance = "0.00"
         wallet_balance_element = get_element(
             driver=driver, locator=UILocatorRegx.get("wallet_balance").get("locator"),
-            regx=UILocatorRegx.get("wallet_balance").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("wallet_balance").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if wallet_balance_element:
             text = wallet_balance_element.text.strip()
             logger.info("获取账号礼品卡{}".format(text))
             wallet_balance = text.split("¥")[-1]
         return Decimal(wallet_balance)
 
     @classmethod
-    def click_use_wallet(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_use_wallet(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         use_wallet_switch = get_element(
             driver=driver, locator=UILocatorRegx.get("use_wallet").get("locator"),
-            regx=UILocatorRegx.get("use_wallet").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("use_wallet").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if use_wallet_switch:
             use_wallet_switch.click()
             logger.info("选择使用钱包支付")
             return True
         else:
             return False
 
     @classmethod
-    def click_wallet_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_wallet_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         immediately_payment_button = get_element(
             driver=driver, locator=UILocatorRegx.get("wallet_immediately_payment").get("locator"),
-            regx=UILocatorRegx.get("use_wallet").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("use_wallet").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if immediately_payment_button:
             immediately_payment_button.click()
             logger.info("点击钱包【立即支付】")
             return True
         else:
             return False
 
     @classmethod
-    def click_use_yeepay2b(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_use_yeepay2b(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         use_yeepay2b_switch = get_element(
             driver=driver, locator=UILocatorRegx.get("use_yeepay2b_pyament").get("locator"),
-            regx=UILocatorRegx.get("use_yeepay2b_pyament").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("use_yeepay2b_pyament").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if use_yeepay2b_switch:
             use_yeepay2b_switch.click()
             logger.info("选择使用易宝会员支付")
             return True
         else:
             return False
 
     @classmethod
-    def click_yeepay2b_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_yeepay2b_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         immediately_payment_button = get_element(
             driver=driver, locator=UILocatorRegx.get("yeepay2b_immediately_payment").get("locator"),
-            regx=UILocatorRegx.get("yeepay2b_immediately_payment").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("yeepay2b_immediately_payment").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if immediately_payment_button:
             immediately_payment_button.click()
             logger.info("点击【易宝支付】按钮")
             return True
         else:
             return False
 
     @classmethod
-    def enter_payment_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0) -> bool:
+    def enter_payment_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0,
+                               **kwargs) -> bool:
         is_exist_pop_box = get_element(
             driver=driver, locator=UILocatorRegx.get("password_pop_box").get("locator"),
-            regx=UILocatorRegx.get("password_pop_box").get("regx"), sleep=sleep, loop=loop
+            regx=UILocatorRegx.get("password_pop_box").get("regx"), sleep=sleep, loop=loop, **kwargs
         )
         if is_exist_pop_box:
             first_password_inout_box = get_element(
                 driver=driver, locator=UILocatorRegx.get("first_password_input_box").get("locator"),
-                regx=UILocatorRegx.get("first_password_input_box").get("regx"), sleep=sleep, loop=loop
+                regx=UILocatorRegx.get("first_password_input_box").get("regx"), sleep=sleep, loop=loop, **kwargs
             )
             if first_password_inout_box:
                 if not isinstance(password, str):
                     password = str(password)
                 first_password_inout_box.click()
                 for i in password:
                     driver.send_keys(i)
@@ -404,58 +406,63 @@
                 logger.warning("查找密码输入框的第一个框失败")
                 return False
         else:
             logger.warning("没有出现输入密码的弹框")
             return False
 
     @classmethod
-    def is_wallet_payment_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def is_wallet_payment_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         return True
 
     @classmethod
-    def enter_yeepay2b_account(cls, driver: webdriver, account: str, loop: int = 1, sleep: float = 0) -> bool:
+    def enter_yeepay2b_account(cls, driver: webdriver, account: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         if current_url.startswith(url_map.get("yeepay2b_cash_desk")) is True:
             input_box = get_element(
                 driver=driver, locator=UILocatorRegx.get("yeepay2b_accout_input_box").get("locator"),
-                regx=UILocatorRegx.get("yeepay2b_accout_input_box").get("regx"), loop=loop, sleep=sleep
+                regx=UILocatorRegx.get("yeepay2b_accout_input_box").get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if input_box:
                 # 模拟键盘操作清空输入框内容
                 input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
                 input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
                 input_box.send_keys('{}'.format(account))
                 logger.info("输入的易宝会员账号：{}".format(account))
                 return True
             else:
                 return False
         else:
             return False
 
     @classmethod
-    def enter_yeepay2b_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0) -> bool:
+    def enter_yeepay2b_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0,
+                                **kwargs) -> bool:
         input_box = get_element(
             driver=driver, locator=UILocatorRegx.get("yeepay2b_password_input_box").get("locator"),
-            regx=UILocatorRegx.get("yeepay2b_password_input_box").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("yeepay2b_password_input_box").get("regx"), loop=loop, sleep=sleep, **kwargs
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
-    def click_yeepay2b_payment_next(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+    def click_yeepay2b_payment_next(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         next_button = get_element(
             driver=driver, locator=UILocatorRegx.get("yeepay2b_payment_next_button").get("locator"),
-            regx=UILocatorRegx.get("yeepay2b_payment_next_button").get("regx"), loop=loop, sleep=sleep
+            regx=UILocatorRegx.get("yeepay2b_payment_next_button").get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if next_button:
             next_button.click()
             logger.info("易宝支付收银台界面点击【下一步】")
             return True
         else:
             return False
+
+    @classmethod
+    def is_yeepay2b_payment_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
+        return True
```

### Comparing `ctrip-helper-0.1.1/ctrip_helper/api/http_api.py` & `ctrip-helper-0.1.2/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.1/ctrip_helper/config.py` & `ctrip-helper-0.1.2/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.1/ctrip_helper/http_client.py` & `ctrip-helper-0.1.2/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.1/ctrip_helper/libs.py` & `ctrip-helper-0.1.2/ctrip_helper/libs.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,17 +87,18 @@
             if is_ignore is False:
                 raise OverflowError("Element found failed, reason: {}".format(err_str))
         if sleep > 0:
             time.sleep(sleep)
     return is_exist
 
 
-def get_element(driver: webdriver, locator: str, regx: str, loop: int, sleep: float,
-                is_ignore: bool = True, is_log_output: bool = True) -> WebElement:
+def get_element(driver: webdriver, locator: str, regx: str, loop: int, sleep: float, **kwargs) -> WebElement:
     element = None
+    is_ignore = kwargs.get("is_ignore", True)
+    is_log_output = kwargs.get("is_log_output", True)
     for i in range(loop):
         try:
             # 根据实际情况定位按钮元素
             element = driver.find_element(Locator.get(locator), regx)
             if element:
                 return element
         except (NoSuchElementException,):
```

### Comparing `ctrip-helper-0.1.1/ctrip_helper/utils.py` & `ctrip-helper-0.1.2/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.1/setup.py` & `ctrip-helper-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.1.1',
+    version='0.1.2',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

