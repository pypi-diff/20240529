# Comparing `tmp/ctrip-helper-0.0.4.tar.gz` & `tmp/ctrip-helper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.0.4.tar", last modified: Wed May 29 15:57:05 2024, max compression
+gzip compressed data, was "ctrip-helper-0.0.5.tar", last modified: Wed May 29 16:54:32 2024, max compression
```

## Comparing `ctrip-helper-0.0.4.tar` & `ctrip-helper-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 15:57:05.861245 ctrip-helper-0.0.4/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 15:57:05.859250 ctrip-helper-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 15:57:05.845288 ctrip-helper-0.0.4/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.4/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 15:57:05.856257 ctrip-helper-0.0.4/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.4/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    20826 2024-05-29 15:53:31.000000 ctrip-helper-0.0.4/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10767 2024-05-29 02:48:04.000000 ctrip-helper-0.0.4/ctrip_helper/api/http.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.4/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.4/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.4/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.4/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 15:57:05.858252 ctrip-helper-0.0.4/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 15:57:05.861245 ctrip-helper-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 15:56:10.000000 ctrip-helper-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:54:32.918455 ctrip-helper-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 16:54:32.917458 ctrip-helper-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 16:54:32.904493 ctrip-helper-0.0.5/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.5/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:54:32.914466 ctrip-helper-0.0.5/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.5/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    23531 2024-05-29 16:53:50.000000 ctrip-helper-0.0.5/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.0.5/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.5/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.5/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.5/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.5/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:54:32.916461 ctrip-helper-0.0.5/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 16:54:32.918455 ctrip-helper-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 16:54:05.000000 ctrip-helper-0.0.5/setup.py
```

### Comparing `ctrip-helper-0.0.4/LICENSE` & `ctrip-helper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.4/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.0.5/ctrip_helper/api/desktop_ui.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,17 @@
                               "regx": '//ul[@class="t_body"]//span[@class="order-price-status-title"]'}
     order_price = {"locator": "xpath", "regx": '//li[@class="item"]//div[@class="order-price-detail"]'}
     order_status_sub_title = {"locator": "xpath",
                               "regx": '//div[contains(@data-testid, "orderstatus_StatusSubTitleWrap")]'}
     order_status_booking_amount = {"locator": "xpath",
                                    "regx": '//div[@data-testid="fbu_PaymentWrapper"]//span[@data-testid="false"]'}
     order_to_payment = {"locator": "xpath", "regx": '//div[@id="button-group"]//a[@data-ubt-v="主订单支付"]'}
+    order_to_cancel = {"locator": "xpath", "regx": '//div[@id="button-group"]//a[@data-ubt-v="取消订单"]'}
+    order_continue_cancel = {"locator": "xpath", "regx": '//div[@class="ant-modal"]//div[@data-testid="继续取消"]'}
+    order_cancel_got_it = {"locator": "xpath", "regx": '//div[@class="ant-modal"]//div[@data-testid="知道了"]'}
     order_payment_amount = {"locator": "xpath", "regx": '//div[@class="m-order-amount"]//div[@class="m-order-money"]'}
     wallet_disable = {"locator": "xpath", "regx": '//div[@class="walelt-card"]//div[@class="lin-crd-disabled"]'}
     wallet_balance = {"locator": "xpath", "regx": '//div[@class="walelt-card"]//div[contains(@class, "crdlast")]'}
     use_wallet = {"locator": "xpath", "regx": '//div[@class="walelt-card"]//input[@class="am-switch-checkbox"]'}
     wallet_immediately_payment = {"locator": "xpath",
                                   "regx": '//div[@class="wallet_pay_button"]//button[@type="gradient"]'}
     use_yeepay2b_pyament = {"locator": "xpath",
@@ -75,106 +78,149 @@
             return True
         else:
             return False
 
     @classmethod
     def enter_order_id(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
         input_box = get_element(
-            driver=driver, locator=UILocatorRegx.order_id_input_box.get("locator"),
-            regx=UILocatorRegx.order_id_input_box.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("order_id_input_box").get("locator"),
+            regx=UILocatorRegx.get("order_id_input_box").get("regx"), loop=loop, sleep=sleep
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
     def click_order_query(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
         order_query_button = get_element(
-            driver=driver, locator=UILocatorRegx.order_query_button.get("locator"),
-            regx=UILocatorRegx.order_query_button.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("order_query_button").get("locator"),
+            regx=UILocatorRegx.get("order_query_button").get("regx"), loop=loop, sleep=sleep
         )
         if order_query_button:
             order_query_button.click()
             logger.info("点击【查询】按钮")
             return True
         else:
             return False
 
     @classmethod
     def get_order_status(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> str:
         order_status = ""
         order_status_element = get_element(
-            driver=driver, locator=UILocatorRegx.order_status_with_list.get("locator"),
-            regx=UILocatorRegx.order_status_with_list.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("order_status_with_list").get("locator"),
+            regx=UILocatorRegx.get("order_status_with_list").get("regx"), loop=loop, sleep=sleep
         )
         if order_status_element:
             order_status = order_status_element.text.strip()
             logger.info("获取订单的状态为：{}".format(order_status))
         return order_status
 
     @classmethod
     def get_order_amonut_with_query_list(cls, driver: webdriver, order_id: str, loop: int = 1,
                                          sleep: float = 0) -> Decimal:
         order_amonut = "0.00"
         order_amonut_element = get_element(
-            driver=driver, locator=UILocatorRegx.order_price.get("locator"),
-            regx=UILocatorRegx.order_price.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
+            regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep
         )
         if order_amonut_element:
             text = order_amonut_element.text.strip()
             logger.info("从查询列表中获取订单: {} 的金额：{}".format(order_id, text))
             order_amonut = text.split("¥")[-1]
         return Decimal(order_amonut)
 
     @classmethod
     def click_order_amonut_with_query_list(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
         order_amonut_element = get_element(
-            driver=driver, locator=UILocatorRegx.order_price.get("locator"),
-            regx=UILocatorRegx.order_price.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
+            regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep
         )
         if order_amonut_element:
             order_amonut_element.click()
             logger.info("点击订单金额，进入订单详情界面")
             return True
         else:
             return False
 
     @classmethod
     def click_to_payment(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
         current_url = driver.current_url
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
         if current_url.startswith(local_url) is True:
             to_payment_button = get_element(
-                driver=driver, locator=UILocatorRegx.order_price.get("locator"),
-                regx=UILocatorRegx.order_price.get("regx"), loop=loop, sleep=sleep
+                driver=driver, locator=UILocatorRegx.get("order_price").get("locator"),
+                regx=UILocatorRegx.get("order_price").get("regx"), loop=loop, sleep=sleep
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
+    def click_order_cancel(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
+        current_url = driver.current_url
+        local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
+        if current_url.startswith(local_url) is True:
+            order_cancel_button = get_element(
+                driver=driver, locator=UILocatorRegx.get("order_to_cancel").get("locator"),
+                regx=UILocatorRegx.get("order_to_cancel").get("regx"), loop=loop, sleep=sleep
+            )
+            if order_cancel_button:
+                order_cancel_button.click()
+                logger.info("点击【取消订单】，接下来会出现【取消提示】小弹框")
+                return True
+            else:
+                return False
+        else:
+            logger.warn("当前订单详情页面: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
+            return False
+
+    @classmethod
+    def click_order_continue_cancel(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+        continue_cance_button = get_element(
+            driver=driver, locator=UILocatorRegx.get("order_continue_cancel").get("locator"),
+            regx=UILocatorRegx.get("order_continue_cancel").get("regx"), loop=loop, sleep=sleep
+        )
+        if continue_cance_button:
+            continue_cance_button.click()
+            logger.info("点击【继续取消】，接下来会出现【知道了】小弹框")
+            return True
+        else:
+            return False
+
+    @classmethod
+    def is_order_cancel_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+        got_it_button = get_element(
+            driver=driver, locator=UILocatorRegx.get("order_cancel_got_it.value").get("locator"),
+            regx=UILocatorRegx.get("order_cancel_got_it").get("regx"), sleep=sleep, loop=loop
+        )
+        if got_it_button:
+            return True
+        else:
+            return False
+
+    @classmethod
     def get_order_amount_with_safe_payment_home(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> Decimal:
         order_payment_amount = "0.00"
         current_url = driver.current_url
         if current_url.startswith(url_map.get("safe_payment_home")) is True:
             order_payment_amount_element = get_element(
-                driver=driver, locator=UILocatorRegx.order_payment_amount.get("locator"),
-                regx=UILocatorRegx.order_payment_amount.get("regx"), loop=loop, sleep=sleep
+                driver=driver, locator=UILocatorRegx.get("order_payment_amount").get("locator"),
+                regx=UILocatorRegx.get("order_payment_amount").get("regx"), loop=loop, sleep=sleep
             )
             if order_payment_amount_element:
                 order_payment_amount = order_payment_amount_element.text.strip()
                 logger.info("获取订单的支付金额为：{}".format(order_payment_amount))
         else:
             logger.warning("当前的界面：{} 不是订单安全支付界面".format(current_url))
         return Decimal(order_payment_amount)
@@ -183,20 +229,20 @@
     def is_cancel_order(cls, driver: webdriver, out_total_price: str, amount_loss_limit: str, profit_cap: str,
                         passenger_number: int, platform: str, loop: int = 1, sleep: float = 0,
                         discount_amount: str = None) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = ""
         status_sub_title_element = get_element(
-            driver=driver, locator=UILocatorRegx.order_status_sub_title.get("locator"),
-            regx=UILocatorRegx.order_status_sub_title.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("order_status_sub_title").get("locator"),
+            regx=UILocatorRegx.get("order_status_sub_title").get("regx"), loop=loop, sleep=sleep
         )
         booking_amount_element = get_element(
-            driver=driver, locator=UILocatorRegx.order_status_booking_amount.get("locator"),
-            regx=UILocatorRegx.order_status_booking_amount.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("order_status_booking_amount").get("locator"),
+            regx=UILocatorRegx.get("order_status_booking_amount").get("regx"), loop=loop, sleep=sleep
         )
         if booking_amount_element:
             booking_amount_text = booking_amount_element.text.strip()
             # 使用 findall 获取所有匹配项
             amount_match = re.search(r"¥(\d+)", booking_amount_text)
             if amount_match:
                 amount_str = amount_match.group(1)
@@ -256,98 +302,98 @@
             remark = "从订单详情页面中未找到订单过期时间元素"
         logger.warning(remark)
         return flag, remark
 
     @classmethod
     def is_wallet_disable(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
         wallet_disable_element = get_element(
-            driver=driver, locator=UILocatorRegx.wallet_disable.get("locator"),
-            regx=UILocatorRegx.wallet_disable.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("wallet_disable").get("locator"),
+            regx=UILocatorRegx.get("wallet_disable").get("regx"), loop=loop, sleep=sleep
         )
         if wallet_disable_element:
             logger.info("当前订单: {} 钱包不可用".format(order_id))
             return True
         else:
             return False
 
     @classmethod
     def get_wallet_balance(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> Decimal:
         wallet_balance = "0.00"
         wallet_balance_element = get_element(
-            driver=driver, locator=UILocatorRegx.wallet_balance.get("locator"),
-            regx=UILocatorRegx.wallet_balance.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("wallet_balance").get("locator"),
+            regx=UILocatorRegx.get("wallet_balance").get("regx"), loop=loop, sleep=sleep
         )
         if wallet_balance_element:
             text = wallet_balance_element.text.strip()
             logger.info("获取账号礼品卡{}".format(text))
             wallet_balance = text.split("¥")[-1]
         return Decimal(wallet_balance)
 
     @classmethod
     def click_use_wallet(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
         use_wallet_switch = get_element(
-            driver=driver, locator=UILocatorRegx.use_wallet.get("locator"),
-            regx=UILocatorRegx.use_wallet.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("use_wallet").get("locator"),
+            regx=UILocatorRegx.get("use_wallet").get("regx"), loop=loop, sleep=sleep
         )
         if use_wallet_switch:
             use_wallet_switch.click()
             logger.info("选择使用钱包支付")
             return True
         else:
             return False
 
     @classmethod
     def click_wallet_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
         immediately_payment_button = get_element(
-            driver=driver, locator=UILocatorRegx.wallet_immediately_payment.get("locator"),
-            regx=UILocatorRegx.use_wallet.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("wallet_immediately_payment").get("locator"),
+            regx=UILocatorRegx.get("use_wallet").get("regx"), loop=loop, sleep=sleep
         )
         if immediately_payment_button:
             immediately_payment_button.click()
             logger.info("点击钱包【立即支付】")
             return True
         else:
             return False
 
     @classmethod
     def click_use_yeepay2b(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
         use_yeepay2b_switch = get_element(
-            driver=driver, locator=UILocatorRegx.use_yeepay2b_pyament.get("locator"),
-            regx=UILocatorRegx.use_yeepay2b_pyament.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("use_yeepay2b_pyament").get("locator"),
+            regx=UILocatorRegx.get("use_yeepay2b_pyament").get("regx"), loop=loop, sleep=sleep
         )
         if use_yeepay2b_switch:
             use_yeepay2b_switch.click()
             logger.info("选择使用易宝会员支付")
             return True
         else:
             return False
 
     @classmethod
     def click_yeepay2b_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
         immediately_payment_button = get_element(
-            driver=driver, locator=UILocatorRegx.yeepay2b_immediately_payment.get("locator"),
-            regx=UILocatorRegx.yeepay2b_immediately_payment.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("yeepay2b_immediately_payment").get("locator"),
+            regx=UILocatorRegx.get("yeepay2b_immediately_payment").get("regx"), loop=loop, sleep=sleep
         )
         if immediately_payment_button:
             immediately_payment_button.click()
             logger.info("点击钱包【易宝支付】")
             return True
         else:
             return False
 
     @classmethod
     def enter_payment_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0) -> bool:
         is_exist_pop_box = get_element(
-            driver=driver, locator=UILocatorRegx.password_pop_box.get("locator"),
-            regx=UILocatorRegx.password_pop_box.get("regx"), sleep=sleep, loop=loop
+            driver=driver, locator=UILocatorRegx.get("password_pop_box").get("locator"),
+            regx=UILocatorRegx.get("password_pop_box").get("regx"), sleep=sleep, loop=loop
         )
         if is_exist_pop_box:
             first_password_inout_box = get_element(
-                driver=driver, locator=UILocatorRegx.first_password_input_box.get("locator"),
-                regx=UILocatorRegx.first_password_input_box.get("regx"), sleep=sleep, loop=loop
+                driver=driver, locator=UILocatorRegx.get("first_password_input_box").get("locator"),
+                regx=UILocatorRegx.get("first_password_input_box").get("regx"), sleep=sleep, loop=loop
             )
             if first_password_inout_box:
                 if not isinstance(password, str):
                     password = str(password)
                 first_password_inout_box.click()
                 for i in password:
                     driver.send_keys(i)
@@ -360,16 +406,16 @@
             return False
 
     @classmethod
     def enter_yeepay2b_account(cls, driver: webdriver, account: str, loop: int = 1, sleep: float = 0) -> bool:
         current_url = driver.current_url
         if current_url.startswith(url_map.get("yeepay2b_cash_desk")) is True:
             input_box = get_element(
-                driver=driver, locator=UILocatorRegx.yeepay2b_accout_input_box.get("locator"),
-                regx=UILocatorRegx.yeepay2b_accout_input_box.get("regx"), loop=loop, sleep=sleep
+                driver=driver, locator=UILocatorRegx.get("yeepay2b_accout_input_box").get("locator"),
+                regx=UILocatorRegx.get("yeepay2b_accout_input_box").get("regx"), loop=loop, sleep=sleep
             )
             if input_box:
                 # 模拟键盘操作清空输入框内容
                 input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
                 input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
                 input_box.send_keys('{}'.format(account))
                 logger.info("输入的易宝会员账号：{}".format(account))
@@ -378,32 +424,32 @@
                 return False
         else:
             return False
 
     @classmethod
     def enter_yeepay2b_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0) -> bool:
         input_box = get_element(
-            driver=driver, locator=UILocatorRegx.yeepay2b_password_input_box.get("locator"),
-            regx=UILocatorRegx.yeepay2b_password_input_box.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("yeepay2b_password_input_box").get("locator"),
+            regx=UILocatorRegx.get("yeepay2b_password_input_box").get("regx"), loop=loop, sleep=sleep
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
     def click_yeepay2b_payment_next(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
         next_button = get_element(
-            driver=driver, locator=UILocatorRegx.yeepay2b_payment_next_button.get("locator"),
-            regx=UILocatorRegx.yeepay2b_payment_next_button.get("regx"), loop=loop, sleep=sleep
+            driver=driver, locator=UILocatorRegx.get("yeepay2b_payment_next_button").get("locator"),
+            regx=UILocatorRegx.get("yeepay2b_payment_next_button").get("regx"), loop=loop, sleep=sleep
         )
         if next_button:
             next_button.click()
             logger.info("易宝支付收银台界面点击【下一步】")
             return True
         else:
             return False
```

### Comparing `ctrip-helper-0.0.4/ctrip_helper/api/http.py` & `ctrip-helper-0.0.5/ctrip_helper/api/http_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 # ---------------------------------------------------------------------------------------------------------
 # ProjectName:  ctrip-helper
-# FileName:     http.py
+# FileName:     http_api.py
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/05/26
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import json
```

### Comparing `ctrip-helper-0.0.4/ctrip_helper/config.py` & `ctrip-helper-0.0.5/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.4/ctrip_helper/http_client.py` & `ctrip-helper-0.0.5/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.4/ctrip_helper/libs.py` & `ctrip-helper-0.0.5/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.4/ctrip_helper/utils.py` & `ctrip-helper-0.0.5/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.4/setup.py` & `ctrip-helper-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.0.4',
+    version='0.0.5',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

