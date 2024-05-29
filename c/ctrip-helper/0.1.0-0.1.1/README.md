# Comparing `tmp/ctrip-helper-0.1.0.tar.gz` & `tmp/ctrip-helper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.1.0.tar", last modified: Wed May 29 18:18:09 2024, max compression
+gzip compressed data, was "ctrip-helper-0.1.1.tar", last modified: Wed May 29 18:23:36 2024, max compression
```

## Comparing `ctrip-helper-0.1.0.tar` & `ctrip-helper-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 18:18:09.907397 ctrip-helper-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 18:18:09.906394 ctrip-helper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 18:18:09.889438 ctrip-helper-0.1.0/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.0/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 18:18:09.903402 ctrip-helper-0.1.0/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.0/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    23858 2024-05-29 18:17:55.000000 ctrip-helper-0.1.0/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.0/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.1.0/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.0/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.1.0/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.0/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 18:18:09.905397 ctrip-helper-0.1.0/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 18:18:09.000000 ctrip-helper-0.1.0/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-29 18:18:09.000000 ctrip-helper-0.1.0/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 18:18:09.000000 ctrip-helper-0.1.0/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 18:18:09.000000 ctrip-helper-0.1.0/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 18:18:09.000000 ctrip-helper-0.1.0/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 18:18:09.907397 ctrip-helper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 18:18:05.000000 ctrip-helper-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:23:36.434348 ctrip-helper-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 18:23:36.433351 ctrip-helper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 18:23:36.420385 ctrip-helper-0.1.1/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.1.1/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:23:36.430359 ctrip-helper-0.1.1/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.1.1/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    23858 2024-05-29 18:23:28.000000 ctrip-helper-0.1.1/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.1.1/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.1.1/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.1.1/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.1.1/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.1.1/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:23:36.432353 ctrip-helper-0.1.1/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 18:23:36.000000 ctrip-helper-0.1.1/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:23:36.435345 ctrip-helper-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 18:23:32.000000 ctrip-helper-0.1.1/setup.py
```

### Comparing `ctrip-helper-0.1.0/LICENSE` & `ctrip-helper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.0/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.1.1/ctrip_helper/api/desktop_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
     def click_yeepay2b_immediately_payment(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
         immediately_payment_button = get_element(
             driver=driver, locator=UILocatorRegx.get("yeepay2b_immediately_payment").get("locator"),
             regx=UILocatorRegx.get("yeepay2b_immediately_payment").get("regx"), loop=loop, sleep=sleep
         )
         if immediately_payment_button:
             immediately_payment_button.click()
-            logger.info("点击钱包【易宝支付】")
+            logger.info("点击【易宝支付】按钮")
             return True
         else:
             return False
 
     @classmethod
     def enter_payment_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0) -> bool:
         is_exist_pop_box = get_element(
```

### Comparing `ctrip-helper-0.1.0/ctrip_helper/api/http_api.py` & `ctrip-helper-0.1.1/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.0/ctrip_helper/config.py` & `ctrip-helper-0.1.1/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.0/ctrip_helper/http_client.py` & `ctrip-helper-0.1.1/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.0/ctrip_helper/libs.py` & `ctrip-helper-0.1.1/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.0/ctrip_helper/utils.py` & `ctrip-helper-0.1.1/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.1.0/setup.py` & `ctrip-helper-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.1.0',
+    version='0.1.1',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

