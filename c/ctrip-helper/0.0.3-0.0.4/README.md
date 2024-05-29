# Comparing `tmp/ctrip-helper-0.0.3.tar.gz` & `tmp/ctrip-helper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.0.3.tar", last modified: Wed May 29 12:57:11 2024, max compression
+gzip compressed data, was "ctrip-helper-0.0.4.tar", last modified: Wed May 29 15:57:05 2024, max compression
```

## Comparing `ctrip-helper-0.0.3.tar` & `ctrip-helper-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:57:11.496893 ctrip-helper-0.0.3/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 12:57:11.495896 ctrip-helper-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 12:57:11.480936 ctrip-helper-0.0.3/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.3/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:57:11.492905 ctrip-helper-0.0.3/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.3/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    20074 2024-05-29 12:56:13.000000 ctrip-helper-0.0.3/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10767 2024-05-29 02:48:04.000000 ctrip-helper-0.0.3/ctrip_helper/api/http.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.3/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.3/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.3/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.3/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:57:11.494899 ctrip-helper-0.0.3/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 12:57:11.000000 ctrip-helper-0.0.3/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 12:57:11.497891 ctrip-helper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 12:57:06.000000 ctrip-helper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:57:05.861245 ctrip-helper-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 15:57:05.859250 ctrip-helper-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 15:57:05.845288 ctrip-helper-0.0.4/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.4/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:57:05.856257 ctrip-helper-0.0.4/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.4/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    20826 2024-05-29 15:53:31.000000 ctrip-helper-0.0.4/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10767 2024-05-29 02:48:04.000000 ctrip-helper-0.0.4/ctrip_helper/api/http.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.4/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.4/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.4/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.4/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:57:05.858252 ctrip-helper-0.0.4/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 15:57:05.000000 ctrip-helper-0.0.4/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 15:57:05.861245 ctrip-helper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 15:56:10.000000 ctrip-helper-0.0.4/setup.py
```

### Comparing `ctrip-helper-0.0.3/LICENSE` & `ctrip-helper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.3/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.0.4/ctrip_helper/api/desktop_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,22 +114,36 @@
         )
         if order_status_element:
             order_status = order_status_element.text.strip()
             logger.info("获取订单的状态为：{}".format(order_status))
         return order_status
 
     @classmethod
-    def click_order_price(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
-        order_price_element = get_element(
+    def get_order_amonut_with_query_list(cls, driver: webdriver, order_id: str, loop: int = 1,
+                                         sleep: float = 0) -> Decimal:
+        order_amonut = "0.00"
+        order_amonut_element = get_element(
             driver=driver, locator=UILocatorRegx.order_price.get("locator"),
             regx=UILocatorRegx.order_price.get("regx"), loop=loop, sleep=sleep
         )
-        if order_price_element:
-            order_price_element.click()
-            logger.info("点击订单价格，进入订单详情界面")
+        if order_amonut_element:
+            text = order_amonut_element.text.strip()
+            logger.info("从查询列表中获取订单: {} 的金额：{}".format(order_id, text))
+            order_amonut = text.split("¥")[-1]
+        return Decimal(order_amonut)
+
+    @classmethod
+    def click_order_amonut_with_query_list(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+        order_amonut_element = get_element(
+            driver=driver, locator=UILocatorRegx.order_price.get("locator"),
+            regx=UILocatorRegx.order_price.get("regx"), loop=loop, sleep=sleep
+        )
+        if order_amonut_element:
+            order_amonut_element.click()
+            logger.info("点击订单金额，进入订单详情界面")
             return True
         else:
             return False
 
     @classmethod
     def click_to_payment(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0) -> bool:
         current_url = driver.current_url
@@ -146,15 +160,15 @@
             else:
                 return False
         else:
             logger.warn("当前订单详情页面: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
             return False
 
     @classmethod
-    def get_order_amount(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> Decimal:
+    def get_order_amount_with_safe_payment_home(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> Decimal:
         order_payment_amount = "0.00"
         current_url = driver.current_url
         if current_url.startswith(url_map.get("safe_payment_home")) is True:
             order_payment_amount_element = get_element(
                 driver=driver, locator=UILocatorRegx.order_payment_amount.get("locator"),
                 regx=UILocatorRegx.order_payment_amount.get("regx"), loop=loop, sleep=sleep
             )
```

### Comparing `ctrip-helper-0.0.3/ctrip_helper/api/http.py` & `ctrip-helper-0.0.4/ctrip_helper/api/http.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.3/ctrip_helper/config.py` & `ctrip-helper-0.0.4/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.3/ctrip_helper/http_client.py` & `ctrip-helper-0.0.4/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.3/ctrip_helper/libs.py` & `ctrip-helper-0.0.4/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.3/ctrip_helper/utils.py` & `ctrip-helper-0.0.4/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.3/setup.py` & `ctrip-helper-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.0.3',
+    version='0.0.4',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

