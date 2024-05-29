# Comparing `tmp/ctrip-helper-0.0.1.tar.gz` & `tmp/ctrip-helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.0.1.tar", last modified: Wed May 29 09:00:13 2024, max compression
+gzip compressed data, was "ctrip-helper-0.0.2.tar", last modified: Wed May 29 11:17:30 2024, max compression
```

## Comparing `ctrip-helper-0.0.1.tar` & `ctrip-helper-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 09:00:13.304021 ctrip-helper-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 09:00:13.302026 ctrip-helper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 09:00:13.286067 ctrip-helper-0.0.1/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.1/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:00:13.299034 ctrip-helper-0.0.1/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.1/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    14766 2024-05-29 08:38:05.000000 ctrip-helper-0.0.1/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10767 2024-05-29 02:48:04.000000 ctrip-helper-0.0.1/ctrip_helper/api/http.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.1/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.1/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.1/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     3007 2024-05-29 02:27:34.000000 ctrip-helper-0.0.1/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:00:13.301028 ctrip-helper-0.0.1/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 09:00:13.000000 ctrip-helper-0.0.1/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-05-29 09:00:13.000000 ctrip-helper-0.0.1/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 09:00:13.000000 ctrip-helper-0.0.1/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 09:00:13.000000 ctrip-helper-0.0.1/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 09:00:13.000000 ctrip-helper-0.0.1/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 09:00:13.304021 ctrip-helper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 09:00:10.000000 ctrip-helper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:17:30.301581 ctrip-helper-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 11:17:30.299585 ctrip-helper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:17:30.285622 ctrip-helper-0.0.2/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.2/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:17:30.296592 ctrip-helper-0.0.2/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.2/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    14768 2024-05-29 11:17:00.000000 ctrip-helper-0.0.2/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10767 2024-05-29 02:48:04.000000 ctrip-helper-0.0.2/ctrip_helper/api/http.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.2/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.2/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.2/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     3007 2024-05-29 02:27:34.000000 ctrip-helper-0.0.2/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:17:30.298588 ctrip-helper-0.0.2/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 11:17:30.000000 ctrip-helper-0.0.2/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:17:30.301581 ctrip-helper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 11:17:09.000000 ctrip-helper-0.0.2/setup.py
```

### Comparing `ctrip-helper-0.0.1/LICENSE` & `ctrip-helper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.1/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.0.2/ctrip_helper/api/desktop_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     yeepay2b_payment_next_button = {"locator": "xpath",
                                     "regx": '//div[@class="account-pay-main"]//button[@id="passPayButton"]'}
 
 
 class SeleniumApi(object):
 
     @classmethod
-    def open_order_query_home_with_flight(cls, driver: webdriver, sleep: int = 0) -> None:
+    def open_order_query_home_with_flight(cls, driver: webdriver, sleep: float = 0) -> None:
         driver.get(url_map.get_url('order_query_home_with_flight'))
         if sleep > 0:
             time.sleep(sleep)
         logger.info("打开机票订单查询首页")
 
     @classmethod
     def click_more_filter_conditions(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
```

### Comparing `ctrip-helper-0.0.1/ctrip_helper/api/http.py` & `ctrip-helper-0.0.2/ctrip_helper/api/http.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.1/ctrip_helper/config.py` & `ctrip-helper-0.0.2/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.1/ctrip_helper/http_client.py` & `ctrip-helper-0.0.2/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.1/ctrip_helper/libs.py` & `ctrip-helper-0.0.2/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.1/ctrip_helper/utils.py` & `ctrip-helper-0.0.2/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.1/setup.py` & `ctrip-helper-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.0.1',
+    version='0.0.2',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

