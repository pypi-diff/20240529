# Comparing `tmp/web-ui-helper-1.0.6.tar.gz` & `tmp/web-ui-helper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-1.0.6.tar", last modified: Tue May 28 17:24:43 2024, max compression
+gzip compressed data, was "web-ui-helper-1.0.7.tar", last modified: Tue May 28 17:31:22 2024, max compression
```

## Comparing `web-ui-helper-1.0.6.tar` & `web-ui-helper-1.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.975410 web-ui-helper-1.0.6/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      747 2024-05-28 17:24:43.974412 web-ui-helper-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 17:24:43.975410 web-ui-helper-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1325 2024-05-28 17:24:37.000000 web-ui-helper-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.931526 web-ui-helper-1.0.6/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.6/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.953468 web-ui-helper-1.0.6/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.6/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.6/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.6/web_ui_helper/common/http_proxy.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.958454 web-ui-helper-1.0.6/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.6/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.959466 web-ui-helper-1.0.6/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.6/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.962444 web-ui-helper-1.0.6/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.6/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    38704 2024-05-28 17:24:18.000000 web-ui-helper-1.0.6/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.965463 web-ui-helper-1.0.6/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.6/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.6/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.968428 web-ui-helper-1.0.6/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.6/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.971420 web-ui-helper-1.0.6/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.6/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-28 17:24:43.973415 web-ui-helper-1.0.6/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      747 2024-05-28 17:24:43.000000 web-ui-helper-1.0.6/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2024-05-28 17:24:43.000000 web-ui-helper-1.0.6/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 17:24:43.000000 web-ui-helper-1.0.6/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2024-05-28 17:24:43.000000 web-ui-helper-1.0.6/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-28 17:24:43.000000 web-ui-helper-1.0.6/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.203703 web-ui-helper-1.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      747 2024-05-28 17:31:22.202705 web-ui-helper-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 17:31:22.203703 web-ui-helper-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2024-05-28 17:31:14.000000 web-ui-helper-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.160818 web-ui-helper-1.0.7/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.7/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.179767 web-ui-helper-1.0.7/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.7/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.7/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.7/web_ui_helper/common/http_proxy.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.184753 web-ui-helper-1.0.7/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.7/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.185751 web-ui-helper-1.0.7/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.7/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.189740 web-ui-helper-1.0.7/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.7/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    38716 2024-05-28 17:31:10.000000 web-ui-helper-1.0.7/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.192732 web-ui-helper-1.0.7/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.7/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.7/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.195724 web-ui-helper-1.0.7/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.7/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.199713 web-ui-helper-1.0.7/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.7/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:31:22.201708 web-ui-helper-1.0.7/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      747 2024-05-28 17:31:22.000000 web-ui-helper-1.0.7/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2024-05-28 17:31:22.000000 web-ui-helper-1.0.7/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 17:31:22.000000 web-ui-helper-1.0.7/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2024-05-28 17:31:22.000000 web-ui-helper-1.0.7/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 17:31:22.000000 web-ui-helper-1.0.7/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-1.0.6/LICENSE` & `web-ui-helper-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/PKG-INFO` & `web-ui-helper-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.6
+Version: 1.0.7
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.6/setup.py` & `web-ui-helper-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='1.0.6',
+    version='1.0.7',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-1.0.6/web_ui_helper/common/date_extend.py` & `web-ui-helper-1.0.7/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/common/dir.py` & `web-ui-helper-1.0.7/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/common/http_proxy.py` & `web-ui-helper-1.0.7/web_ui_helper/common/http_proxy.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/common/log.py` & `web-ui-helper-1.0.7/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/common/metaclass.py` & `web-ui-helper-1.0.7/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/common/platforms.py` & `web-ui-helper-1.0.7/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/common/webdriver.py` & `web-ui-helper-1.0.7/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-1.0.7/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-1.0.7/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-1.0.7/web_ui_helper/selenium/frame/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             log_output=log_file
         )
         return service
 
     def get_browser(self) -> tuple:
         service = self.get_service()
         options = self.get_options()
-        browser = Chrome(service=service, options=options)
+        browser = driver_wire.Chrome(service=service, options=options)
         logger.warning("Selenium 版本: {}".format(selenium.__version__))
         logger.warning("浏览器版本: {}".format(browser.capabilities['browserVersion']))
         # 设置隐式等待时间为3秒
         # browser.implicitly_wait(3)
         # 反屏蔽
         browser.execute_cdp_cmd('Page.addScriptToEvaluateOnNewDocument', {
             'source': 'Object.defineProperty(navigator, "webdriver", {get: () => undefined})',
```

### Comparing `web-ui-helper-1.0.6/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-1.0.7/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-1.0.7/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper/terminal/device.py` & `web-ui-helper-1.0.7/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.6/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-1.0.7/web_ui_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.6
+Version: 1.0.7
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.6/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-1.0.7/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

