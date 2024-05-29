# Comparing `tmp/ctrip-helper-0.0.5.tar.gz` & `tmp/ctrip-helper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.0.5.tar", last modified: Wed May 29 16:54:32 2024, max compression
+gzip compressed data, was "ctrip-helper-0.0.6.tar", last modified: Wed May 29 17:22:08 2024, max compression
```

## Comparing `ctrip-helper-0.0.5.tar` & `ctrip-helper-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 16:54:32.918455 ctrip-helper-0.0.5/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 16:54:32.917458 ctrip-helper-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 16:54:32.904493 ctrip-helper-0.0.5/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.5/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:54:32.914466 ctrip-helper-0.0.5/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.5/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    23531 2024-05-29 16:53:50.000000 ctrip-helper-0.0.5/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.0.5/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.5/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.5/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.5/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.5/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:54:32.916461 ctrip-helper-0.0.5/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 16:54:32.000000 ctrip-helper-0.0.5/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 16:54:32.918455 ctrip-helper-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 16:54:05.000000 ctrip-helper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:22:08.995578 ctrip-helper-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 17:22:08.994567 ctrip-helper-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 17:22:08.980605 ctrip-helper-0.0.6/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.6/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:22:08.991576 ctrip-helper-0.0.6/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.6/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    23534 2024-05-29 17:21:49.000000 ctrip-helper-0.0.6/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.0.6/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.6/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.6/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.6/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.6/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:22:08.993570 ctrip-helper-0.0.6/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:22:08.995578 ctrip-helper-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 17:22:04.000000 ctrip-helper-0.0.6/setup.py
```

### Comparing `ctrip-helper-0.0.5/LICENSE` & `ctrip-helper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.5/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.0.6/ctrip_helper/api/desktop_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
                 order_payment_amount = order_payment_amount_element.text.strip()
                 logger.info("获取订单的支付金额为：{}".format(order_payment_amount))
         else:
             logger.warning("当前的界面：{} 不是订单安全支付界面".format(current_url))
         return Decimal(order_payment_amount)
 
     @classmethod
-    def is_cancel_order(cls, driver: webdriver, out_total_price: str, amount_loss_limit: str, profit_cap: str,
+    def is_cancel_order(cls, driver: webdriver, out_total_amount: str, amount_loss_limit: str, profit_cap: str,
                         passenger_number: int, platform: str, loop: int = 1, sleep: float = 0,
                         discount_amount: str = None) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = ""
         status_sub_title_element = get_element(
             driver=driver, locator=UILocatorRegx.get("order_status_sub_title").get("locator"),
@@ -243,18 +243,18 @@
         if booking_amount_element:
             booking_amount_text = booking_amount_element.text.strip()
             # 使用 findall 获取所有匹配项
             amount_match = re.search(r"¥(\d+)", booking_amount_text)
             if amount_match:
                 amount_str = amount_match.group(1)
                 logger.warning("从{}订单获取的支付金额：{}，劲旅订单总价：{}".format(
-                    platform, amount_str, out_total_price
+                    platform, amount_str, out_total_amount
                 ))
                 # 预期订单利润
-                ex_order_profit = Decimal(out_total_price) - Decimal(amount_str)
+                ex_order_profit = Decimal(out_total_amount) - Decimal(amount_str)
                 if discount_amount:
                     # 实际订单利润
                     ac_order_profit = ex_order_profit + Decimal(discount_amount)
                 else:
                     ac_order_profit = ex_order_profit
                 # 订单利润 < 0, 存在亏钱，与亏钱的下限进行比较
                 if ac_order_profit < 0:
```

### Comparing `ctrip-helper-0.0.5/ctrip_helper/api/http_api.py` & `ctrip-helper-0.0.6/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.5/ctrip_helper/config.py` & `ctrip-helper-0.0.6/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.5/ctrip_helper/http_client.py` & `ctrip-helper-0.0.6/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.5/ctrip_helper/libs.py` & `ctrip-helper-0.0.6/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.5/ctrip_helper/utils.py` & `ctrip-helper-0.0.6/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.5/setup.py` & `ctrip-helper-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.0.5',
+    version='0.0.6',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

