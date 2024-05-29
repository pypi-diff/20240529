# Comparing `tmp/ctrip-helper-0.0.7.tar.gz` & `tmp/ctrip-helper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.0.7.tar", last modified: Wed May 29 17:53:19 2024, max compression
+gzip compressed data, was "ctrip-helper-0.0.8.tar", last modified: Wed May 29 17:56:54 2024, max compression
```

## Comparing `ctrip-helper-0.0.7.tar` & `ctrip-helper-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 17:53:19.119855 ctrip-helper-0.0.7/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 17:53:19.117863 ctrip-helper-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 17:53:19.102900 ctrip-helper-0.0.7/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.7/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:53:19.114868 ctrip-helper-0.0.7/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.7/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    23677 2024-05-29 17:53:01.000000 ctrip-helper-0.0.7/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.0.7/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.7/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.7/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.7/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.7/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:53:19.116864 ctrip-helper-0.0.7/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 17:53:18.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-29 17:53:19.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 17:53:18.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 17:53:18.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 17:53:18.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 17:53:19.119855 ctrip-helper-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 17:53:12.000000 ctrip-helper-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:56:54.651420 ctrip-helper-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 17:56:54.649425 ctrip-helper-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 17:56:54.634468 ctrip-helper-0.0.8/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.8/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:56:54.646434 ctrip-helper-0.0.8/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.8/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    23819 2024-05-29 17:56:43.000000 ctrip-helper-0.0.8/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.0.8/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.8/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.8/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.8/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.8/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:56:54.648429 ctrip-helper-0.0.8/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 17:56:54.000000 ctrip-helper-0.0.8/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-29 17:56:54.000000 ctrip-helper-0.0.8/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:56:54.000000 ctrip-helper-0.0.8/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 17:56:54.000000 ctrip-helper-0.0.8/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 17:56:54.000000 ctrip-helper-0.0.8/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:56:54.651420 ctrip-helper-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 17:56:49.000000 ctrip-helper-0.0.8/setup.py
```

### Comparing `ctrip-helper-0.0.7/LICENSE` & `ctrip-helper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.7/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.0.8/ctrip_helper/api/desktop_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,14 +404,18 @@
                 logger.warning("查找密码输入框的第一个框失败")
                 return False
         else:
             logger.warning("没有出现输入密码的弹框")
             return False
 
     @classmethod
+    def is_wallet_payment_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> bool:
+        return True
+
+    @classmethod
     def enter_yeepay2b_account(cls, driver: webdriver, account: str, loop: int = 1, sleep: float = 0) -> bool:
         current_url = driver.current_url
         if current_url.startswith(url_map.get("yeepay2b_cash_desk")) is True:
             input_box = get_element(
                 driver=driver, locator=UILocatorRegx.get("yeepay2b_accout_input_box").get("locator"),
                 regx=UILocatorRegx.get("yeepay2b_accout_input_box").get("regx"), loop=loop, sleep=sleep
             )
```

### Comparing `ctrip-helper-0.0.7/ctrip_helper/api/http_api.py` & `ctrip-helper-0.0.8/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.7/ctrip_helper/config.py` & `ctrip-helper-0.0.8/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.7/ctrip_helper/http_client.py` & `ctrip-helper-0.0.8/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.7/ctrip_helper/libs.py` & `ctrip-helper-0.0.8/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.7/ctrip_helper/utils.py` & `ctrip-helper-0.0.8/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.7/setup.py` & `ctrip-helper-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.0.7',
+    version='0.0.8',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

