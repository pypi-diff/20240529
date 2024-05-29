# Comparing `tmp/ctrip-helper-0.0.6.tar.gz` & `tmp/ctrip-helper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.0.6.tar", last modified: Wed May 29 17:22:08 2024, max compression
+gzip compressed data, was "ctrip-helper-0.0.7.tar", last modified: Wed May 29 17:53:19 2024, max compression
```

## Comparing `ctrip-helper-0.0.6.tar` & `ctrip-helper-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 17:22:08.995578 ctrip-helper-0.0.6/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-29 17:22:08.994567 ctrip-helper-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 17:22:08.980605 ctrip-helper-0.0.6/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.6/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:22:08.991576 ctrip-helper-0.0.6/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.6/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    23534 2024-05-29 17:21:49.000000 ctrip-helper-0.0.6/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.0.6/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.6/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.6/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.6/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.6/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:22:08.993570 ctrip-helper-0.0.6/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 17:22:08.000000 ctrip-helper-0.0.6/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 17:22:08.995578 ctrip-helper-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-29 17:22:04.000000 ctrip-helper-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:53:19.119855 ctrip-helper-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-29 17:53:19.117863 ctrip-helper-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 17:53:19.102900 ctrip-helper-0.0.7/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.0.7/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:53:19.114868 ctrip-helper-0.0.7/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.0.7/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    23677 2024-05-29 17:53:01.000000 ctrip-helper-0.0.7/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.0.7/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3558 2024-05-29 08:21:09.000000 ctrip-helper-0.0.7/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.0.7/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     4532 2024-05-29 04:09:02.000000 ctrip-helper-0.0.7/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.0.7/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:53:19.116864 ctrip-helper-0.0.7/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-29 17:53:18.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-29 17:53:19.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:53:18.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 17:53:18.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 17:53:18.000000 ctrip-helper-0.0.7/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:53:19.119855 ctrip-helper-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-29 17:53:12.000000 ctrip-helper-0.0.7/setup.py
```

### Comparing `ctrip-helper-0.0.6/LICENSE` & `ctrip-helper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.6/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.0.7/ctrip_helper/api/desktop_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,16 +397,18 @@
                 first_password_inout_box.click()
                 for i in password:
                     driver.send_keys(i)
                     # 可选：添加一个短暂的延迟，模拟更接近人类的输入速度
                     time.sleep(0.5)
                 return True
             else:
+                logger.warning("查找密码输入框的第一个框失败")
                 return False
         else:
+            logger.warning("没有出现输入密码的弹框")
             return False
 
     @classmethod
     def enter_yeepay2b_account(cls, driver: webdriver, account: str, loop: int = 1, sleep: float = 0) -> bool:
         current_url = driver.current_url
         if current_url.startswith(url_map.get("yeepay2b_cash_desk")) is True:
             input_box = get_element(
```

### Comparing `ctrip-helper-0.0.6/ctrip_helper/api/http_api.py` & `ctrip-helper-0.0.7/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.6/ctrip_helper/config.py` & `ctrip-helper-0.0.7/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.6/ctrip_helper/http_client.py` & `ctrip-helper-0.0.7/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.6/ctrip_helper/libs.py` & `ctrip-helper-0.0.7/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.6/ctrip_helper/utils.py` & `ctrip-helper-0.0.7/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.0.6/setup.py` & `ctrip-helper-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.0.6',
+    version='0.0.7',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

