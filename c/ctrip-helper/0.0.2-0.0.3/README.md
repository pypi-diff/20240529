# Comparing `tmp/ctrip-helper-0.0.2.tar.gz` & `tmp/ctrip-helper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.0.2.tar", last modified: Wed May 29 11:17:30 2024, max compression
+gzip compressed data, was "ctrip-helper-0.0.3.tar", last modified: Wed May 29 12:57:11 2024, max compression
```

## Comparing `ctrip-helper-0.0.2.tar` & `ctrip-helper-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:17:30.301581 ctrip-helper-0.0.2/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 11:17:30.299585 ctrip-helper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 11:17:30.285622 ctrip-helper-0.0.2/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.2/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:17:30.296592 ctrip-helper-0.0.2/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.2/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    14768 2024-05-29 11:17:00.000000 ctrip-helper-0.0.2/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10767 2024-05-29 02:48:04.000000 ctrip-helper-0.0.2/ctrip_helper/api/http.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.2/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.2/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.2/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     3007 2024-05-29 02:27:34.000000 ctrip-helper-0.0.2/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:17:30.298588 ctrip-helper-0.0.2/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 11:17:30.301581 ctrip-helper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 11:17:09.000000 ctrip-helper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:57:11.496893 ctrip-helper-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 12:57:11.495896 ctrip-helper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 12:57:11.480936 ctrip-helper-0.0.3/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.3/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:57:11.492905 ctrip-helper-0.0.3/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.3/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    20074 2024-05-29 12:56:13.000000 ctrip-helper-0.0.3/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10767 2024-05-29 02:48:04.000000 ctrip-helper-0.0.3/ctrip_helper/api/http.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.3/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.3/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.3/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.3/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:57:11.494899 ctrip-helper-0.0.3/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:57:11.497891 ctrip-helper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 12:57:06.000000 ctrip-helper-0.0.3/setup.py
```

### Comparing `ctrip-helper-0.0.2/LICENSE` & `ctrip-helper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.2/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.0.3/ctrip_helper/api/desktop_ui.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,33 +5,40 @@
 # FileName:     desktop_ui.py
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/05/29
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
+import re
 import time
 from decimal import Decimal
 from selenium import webdriver
 from ctrip_helper.libs import logger
 from ctrip_helper.config import url_map
 from selenium.webdriver.common.keys import Keys
 from ctrip_helper.libs import get_element, EnumMetaClass
+from ctrip_helper.utils import is_later_than_current_time
 
 
 class UILocatorRegx(EnumMetaClass):
     all_orders_select_box = {"locator": "xpath",
                              "regx": '//ul[@class="fix_myctrip_order_layer"]//div[@class="select-box"]'},
     order_id_input_box = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//input[@id="searchBookingNum"]'},
     order_query_button = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//button[@class="btn_sel"]'}
     order_status_with_list = {"locator": "xpath",
                               "regx": '//ul[@class="t_body"]//span[@class="order-price-status-title"]'}
     order_price = {"locator": "xpath", "regx": '//li[@class="item"]//div[@class="order-price-detail"]'}
+    order_status_sub_title = {"locator": "xpath",
+                              "regx": '//div[contains(@data-testid, "orderstatus_StatusSubTitleWrap")]'}
+    order_status_booking_amount = {"locator": "xpath",
+                                   "regx": '//div[@data-testid="fbu_PaymentWrapper"]//span[@data-testid="false"]'}
     order_to_payment = {"locator": "xpath", "regx": '//div[@id="button-group"]//a[@data-ubt-v="主订单支付"]'}
     order_payment_amount = {"locator": "xpath", "regx": '//div[@class="m-order-amount"]//div[@class="m-order-money"]'}
+    wallet_disable = {"locator": "xpath", "regx": '//div[@class="walelt-card"]//div[@class="lin-crd-disabled"]'}
     wallet_balance = {"locator": "xpath", "regx": '//div[@class="walelt-card"]//div[contains(@class, "crdlast")]'}
     use_wallet = {"locator": "xpath", "regx": '//div[@class="walelt-card"]//input[@class="am-switch-checkbox"]'}
     wallet_immediately_payment = {"locator": "xpath",
                                   "regx": '//div[@class="wallet_pay_button"]//button[@type="gradient"]'}
     use_yeepay2b_pyament = {"locator": "xpath",
                             "regx": '//div[@class="pay_way_container"]//div[contains(text(), "易宝会员支付")]'}
     yeepay2b_immediately_payment = {"locator": "xpath",
@@ -155,14 +162,104 @@
                 order_payment_amount = order_payment_amount_element.text.strip()
                 logger.info("获取订单的支付金额为：{}".format(order_payment_amount))
         else:
             logger.warning("当前的界面：{} 不是订单安全支付界面".format(current_url))
         return Decimal(order_payment_amount)
 
     @classmethod
+    def is_cancel_order(cls, driver: webdriver, out_total_price: str, amount_loss_limit: str, profit_cap: str,
+                        passenger_number: int, platform: str, loop: int = 1, sleep: float = 0,
+                        discount_amount: str = None) -> tuple:
+        """在订单详情页，判断是否需要取消订单"""
+        flag = False
+        remark = ""
+        status_sub_title_element = get_element(
+            driver=driver, locator=UILocatorRegx.order_status_sub_title.get("locator"),
+            regx=UILocatorRegx.order_status_sub_title.get("regx"), loop=loop, sleep=sleep
+        )
+        booking_amount_element = get_element(
+            driver=driver, locator=UILocatorRegx.order_status_booking_amount.get("locator"),
+            regx=UILocatorRegx.order_status_booking_amount.get("regx"), loop=loop, sleep=sleep
+        )
+        if booking_amount_element:
+            booking_amount_text = booking_amount_element.text.strip()
+            # 使用 findall 获取所有匹配项
+            amount_match = re.search(r"¥(\d+)", booking_amount_text)
+            if amount_match:
+                amount_str = amount_match.group(1)
+                logger.warning("从{}订单获取的支付金额：{}，劲旅订单总价：{}".format(
+                    platform, amount_str, out_total_price
+                ))
+                # 预期订单利润
+                ex_order_profit = Decimal(out_total_price) - Decimal(amount_str)
+                if discount_amount:
+                    # 实际订单利润
+                    ac_order_profit = ex_order_profit + Decimal(discount_amount)
+                else:
+                    ac_order_profit = ex_order_profit
+                # 订单利润 < 0, 存在亏钱，与亏钱的下限进行比较
+                if ac_order_profit < 0:
+                    total = Decimal(amount_loss_limit) * passenger_number
+                    if ac_order_profit + total < 0:
+                        flag = True
+                        remark = "订单亏钱{:.2f}太多，超过订单总下限值{}(单人下限{} * {}人)".format(
+                            abs(ac_order_profit), total, amount_loss_limit, passenger_number
+                        )
+                        logger.warning(remark)
+                        return flag, remark
+                # 订单利润 >= 0, 存在毛利，与利润的上限进行比较
+                else:
+                    total = Decimal(profit_cap) * passenger_number
+                    if ac_order_profit - total > 0:
+                        flag = True
+                        remark = "订单利润{:.2f}太高，超过订单总下限值{}(单人下限{} * {}人)".format(
+                            ac_order_profit, total, profit_cap, passenger_number
+                        )
+                        logger.warning(remark)
+                        return flag, remark
+            else:
+                remark = "从订单详情页面获取订单过期时间和订单金额有异常"
+                logger.warning(remark)
+        else:
+            remark = "订单详情页面中未找到订单金额元素"
+            logger.warning(remark)
+        if status_sub_title_element:
+            sub_title_text = status_sub_title_element.text.strip()
+            # 使用 findall 获取所有匹配项
+            time_match = re.search(r"(\d{2}:\d{2})", sub_title_text)
+            if time_match:
+                time_str = time_match.group(1)
+                logger.info("从订单获取到的过期时间为：{}".format(time_str))
+                minutes = 1
+                is_later = is_later_than_current_time(time_str=time_str, minutes=minutes)
+                if is_later is False:
+                    flag = True
+                    remark = "支付时间少于{}分钟".format(minutes)
+                    logger.warning(remark)
+                    return flag, remark
+            else:
+                remark = "从文案<{}>中没有获取订单过期时间".format(sub_title_text)
+        else:
+            remark = "从订单详情页面中未找到订单过期时间元素"
+        logger.warning(remark)
+        return flag, remark
+
+    @classmethod
+    def is_wallet_disable(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
+        wallet_disable_element = get_element(
+            driver=driver, locator=UILocatorRegx.wallet_disable.get("locator"),
+            regx=UILocatorRegx.wallet_disable.get("regx"), loop=loop, sleep=sleep
+        )
+        if wallet_disable_element:
+            logger.info("当前订单: {} 钱包不可用".format(order_id))
+            return True
+        else:
+            return False
+
+    @classmethod
     def get_wallet_balance(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> Decimal:
         wallet_balance = "0.00"
         wallet_balance_element = get_element(
             driver=driver, locator=UILocatorRegx.wallet_balance.get("locator"),
             regx=UILocatorRegx.wallet_balance.get("regx"), loop=loop, sleep=sleep
         )
         if wallet_balance_element:
```

### Comparing `ctrip-helper-0.0.2/ctrip_helper/api/http.py` & `ctrip-helper-0.0.3/ctrip_helper/api/http.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.2/ctrip_helper/config.py` & `ctrip-helper-0.0.3/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.2/ctrip_helper/http_client.py` & `ctrip-helper-0.0.3/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.2/ctrip_helper/libs.py` & `ctrip-helper-0.0.3/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.2/setup.py` & `ctrip-helper-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.0.2',
+    version='0.0.3',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

