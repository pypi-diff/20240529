# Comparing `tmp/vns_explorer-1.0.1.tar.gz` & `tmp/vns_explorer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vns_explorer-1.0.1.tar", last modified: Wed May 29 06:48:26 2024, max compression
+gzip compressed data, was "vns_explorer-1.0.2.tar", last modified: Wed May 29 07:00:40 2024, max compression
```

## Comparing `vns_explorer-1.0.1.tar` & `vns_explorer-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 06:48:26.371178 vns_explorer-1.0.1/
--rw-rw-rw-   0        0        0      601 2024-05-29 06:48:26.370131 vns_explorer-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-05-29 04:11:37.000000 vns_explorer-1.0.1/README.md
--rw-rw-rw-   0        0        0      796 2024-05-29 06:30:57.000000 vns_explorer-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      468 2024-05-29 06:48:26.377692 vns_explorer-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 06:48:26.329128 vns_explorer-1.0.1/vns_explorer/
--rw-rw-rw-   0        0        0       64 2024-05-29 06:10:09.000000 vns_explorer-1.0.1/vns_explorer/__init__.py
--rw-rw-rw-   0        0        0     1446 2024-05-29 04:00:43.000000 vns_explorer-1.0.1/vns_explorer/agent.py
--rw-rw-rw-   0        0        0    10517 2024-05-29 06:47:34.000000 vns_explorer-1.0.1/vns_explorer/browser.py
--rw-rw-rw-   0        0        0     2293 2024-05-29 06:09:48.000000 vns_explorer-1.0.1/vns_explorer/env.py
-drwxrwxrwx   0        0        0        0 2024-05-29 06:48:26.368166 vns_explorer-1.0.1/vns_explorer.egg-info/
--rw-rw-rw-   0        0        0      601 2024-05-29 06:48:26.000000 vns_explorer-1.0.1/vns_explorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-29 06:48:26.000000 vns_explorer-1.0.1/vns_explorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 06:48:26.000000 vns_explorer-1.0.1/vns_explorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-29 06:48:26.000000 vns_explorer-1.0.1/vns_explorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 06:48:26.000000 vns_explorer-1.0.1/vns_explorer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 07:00:40.425590 vns_explorer-1.0.2/
+-rw-rw-rw-   0        0        0      601 2024-05-29 07:00:40.424591 vns_explorer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-29 04:11:37.000000 vns_explorer-1.0.2/README.md
+-rw-rw-rw-   0        0        0      796 2024-05-29 06:58:20.000000 vns_explorer-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      468 2024-05-29 07:00:40.431594 vns_explorer-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 07:00:40.361199 vns_explorer-1.0.2/vns_explorer/
+-rw-rw-rw-   0        0        0       64 2024-05-29 06:10:09.000000 vns_explorer-1.0.2/vns_explorer/__init__.py
+-rw-rw-rw-   0        0        0     1446 2024-05-29 04:00:43.000000 vns_explorer-1.0.2/vns_explorer/agent.py
+-rw-rw-rw-   0        0        0    10481 2024-05-29 06:58:14.000000 vns_explorer-1.0.2/vns_explorer/browser.py
+-rw-rw-rw-   0        0        0     2293 2024-05-29 06:09:48.000000 vns_explorer-1.0.2/vns_explorer/env.py
+drwxrwxrwx   0        0        0        0 2024-05-29 07:00:40.420591 vns_explorer-1.0.2/vns_explorer.egg-info/
+-rw-rw-rw-   0        0        0      601 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/top_level.txt
```

### Comparing `vns_explorer-1.0.1/PKG-INFO` & `vns_explorer-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vns_explorer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Discover the Unseen
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `vns_explorer-1.0.1/pyproject.toml` & `vns_explorer-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 # Metadata Information
 [project]
 name = "vns_explorer"
-version = "1.0.1"
+version = "1.0.2"
 description = "Discover the Unseen"
 authors = [
     { name = "Thinh Vu", email = "mrthinh@live.com" },
     ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
```

### Comparing `vns_explorer-1.0.1/vns_explorer/agent.py` & `vns_explorer-1.0.2/vns_explorer/agent.py`

 * *Files identical despite different names*

### Comparing `vns_explorer-1.0.1/vns_explorer/browser.py` & `vns_explorer-1.0.2/vns_explorer/browser.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 if is_colab:
     from .env import setup_selenium
     setup_selenium()
 
 Imports = {
     "selenium": find_spec("selenium") is not None,
     "webdriver": find_spec("webdriver_manager") is not None,
-    "pyautogui": find_spec("pyautogui") is not None and not is_colab
+    # "pyautogui": find_spec("pyautogui") is not None and not is_colab
 }
 
-if not Imports["selenium"] or not Imports["webdriver"] or (not Imports["pyautogui"] and not is_colab):
-    raise ImportError("selenium, webdriver_manager and pyautogui are required to run this script. Please install them using 'pip install selenium webdriver_manager pyautogui' and try again.")
+if not Imports["selenium"] or not Imports["webdriver"]:
+    raise ImportError("selenium, webdriver_manager are required to run this script. Please install them using 'pip install selenium webdriver_manager and try again.")
 else:
     from selenium import webdriver
     from selenium.webdriver.chrome.service import Service as ChromeService
     from selenium.webdriver.chrome.options import Options
     from selenium.webdriver.common.by import By
     from selenium.webdriver.support.ui import WebDriverWait
     from selenium.webdriver.support import expected_conditions as EC
@@ -78,32 +78,32 @@
             """
             Open a specific URL in the ChromeDriver instance.
             """
             print(f'Visiting {url}')
             self.driver.get(url)
             print(self.driver.title)
 
-        def random_mouse(self, duration=2, frequency=0.5):
-            """
-            Simulate random mouse movements on the screen.
-
-            Parameters:
-                - duration (int): The total duration to simulate random mouse movements, in seconds.
-                - frequency (float): The frequency of mouse movements, in seconds.
-            """
-            if is_colab:
-                print("random_mouse() is not supported in Google Colab environment.")
-                return
-            end_time = time.time() + duration
-            while time.time() < end_time:
-                screen_width, screen_height = pyautogui.size()
-                x = random.randint(0, screen_width)
-                y = random.randint(0, screen_height)
-                pyautogui.moveTo(x, y, duration=frequency)
-                time.sleep(frequency)
+        # def random_mouse(self, duration=2, frequency=0.5):
+        #     """
+        #     Simulate random mouse movements on the screen.
+
+        #     Parameters:
+        #         - duration (int): The total duration to simulate random mouse movements, in seconds.
+        #         - frequency (float): The frequency of mouse movements, in seconds.
+        #     """
+        #     if is_colab:
+        #         print("random_mouse() is not supported in Google Colab environment.")
+        #         return
+        #     end_time = time.time() + duration
+        #     while time.time() < end_time:
+        #         screen_width, screen_height = pyautogui.size()
+        #         x = random.randint(0, screen_width)
+        #         y = random.randint(0, screen_height)
+        #         pyautogui.moveTo(x, y, duration=frequency)
+        #         time.sleep(frequency)
 
         def scroll(self, direction='down', pct=0.2, duration=2):
             """
             Scroll the page up or down by a certain percentage.
 
             Parameters:
                 - direction (str): The direction to scroll. 'up' for scrolling up and 'down' for scrolling down. Default is 'down'.
```

### Comparing `vns_explorer-1.0.1/vns_explorer/env.py` & `vns_explorer-1.0.2/vns_explorer/env.py`

 * *Files identical despite different names*

### Comparing `vns_explorer-1.0.1/vns_explorer.egg-info/PKG-INFO` & `vns_explorer-1.0.2/vns_explorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vns_explorer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Discover the Unseen
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

