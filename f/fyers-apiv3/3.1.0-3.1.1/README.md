# Comparing `tmp/fyers_apiv3-3.1.0.tar.gz` & `tmp/fyers_apiv3-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_apiv3-3.1.0.tar", last modified: Tue Mar 26 11:43:51 2024, max compression
+gzip compressed data, was "fyers_apiv3-3.1.1.tar", last modified: Wed May 29 12:46:23 2024, max compression
```

## Comparing `fyers_apiv3-3.1.0.tar` & `fyers_apiv3-3.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2024-03-26 11:43:51.206861 fyers_apiv3-3.1.0/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-12-01 13:30:20.000000 fyers_apiv3-3.1.0/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15071 2024-03-26 11:43:51.206861 fyers_apiv3-3.1.0/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    14672 2023-12-01 13:30:49.000000 fyers_apiv3-3.1.0/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2024-03-26 11:43:51.182861 fyers_apiv3-3.1.0/fyers_apiv3/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2024-03-26 11:43:51.202861 fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-12-01 13:30:49.000000 fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    68171 2024-03-14 12:10:48.000000 fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1143 2024-03-14 12:35:08.000000 fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10026 2023-12-29 07:35:45.000000 fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    16953 2024-03-14 12:12:08.000000 fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-12-01 13:30:49.000000 fyers_apiv3-3.1.0/fyers_apiv3/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    38810 2024-03-14 12:48:01.000000 fyers_apiv3-3.1.0/fyers_apiv3/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2024-02-20 07:13:38.000000 fyers_apiv3-3.1.0/fyers_apiv3/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2024-03-26 11:43:51.202861 fyers_apiv3-3.1.0/fyers_apiv3.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15071 2024-03-26 11:43:51.000000 fyers_apiv3-3.1.0/fyers_apiv3.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      472 2024-03-26 11:43:51.000000 fyers_apiv3-3.1.0/fyers_apiv3.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2024-03-26 11:43:51.000000 fyers_apiv3-3.1.0/fyers_apiv3.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2024-03-26 11:43:51.000000 fyers_apiv3-3.1.0/fyers_apiv3.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       12 2024-03-26 11:43:51.000000 fyers_apiv3-3.1.0/fyers_apiv3.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2024-03-26 11:43:51.206861 fyers_apiv3-3.1.0/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1020 2024-03-26 10:35:02.000000 fyers_apiv3-3.1.0/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2024-05-29 12:46:23.909519 fyers_apiv3-3.1.1/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-12-01 13:30:20.000000 fyers_apiv3-3.1.1/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15071 2024-05-29 12:46:23.909519 fyers_apiv3-3.1.1/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    14672 2023-12-01 13:30:49.000000 fyers_apiv3-3.1.1/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2024-05-29 12:46:23.881520 fyers_apiv3-3.1.1/fyers_apiv3/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2024-05-29 12:46:23.909519 fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-12-01 13:30:49.000000 fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    68105 2024-05-29 12:42:43.000000 fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1143 2024-03-14 12:35:08.000000 fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10026 2023-12-29 07:35:45.000000 fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    16998 2024-05-29 12:35:37.000000 fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-12-01 13:30:49.000000 fyers_apiv3-3.1.1/fyers_apiv3/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    38810 2024-03-14 12:48:01.000000 fyers_apiv3-3.1.1/fyers_apiv3/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2024-02-20 07:13:38.000000 fyers_apiv3-3.1.1/fyers_apiv3/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2024-05-29 12:46:23.905520 fyers_apiv3-3.1.1/fyers_apiv3.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15071 2024-05-29 12:46:23.000000 fyers_apiv3-3.1.1/fyers_apiv3.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      472 2024-05-29 12:46:23.000000 fyers_apiv3-3.1.1/fyers_apiv3.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2024-05-29 12:46:23.000000 fyers_apiv3-3.1.1/fyers_apiv3.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2024-05-29 12:46:23.000000 fyers_apiv3-3.1.1/fyers_apiv3.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       12 2024-05-29 12:46:23.000000 fyers_apiv3-3.1.1/fyers_apiv3.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2024-05-29 12:46:23.909519 fyers_apiv3-3.1.1/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1020 2024-05-29 12:45:55.000000 fyers_apiv3-3.1.1/setup.py
```

### Comparing `fyers_apiv3-3.1.0/LICENSE.txt` & `fyers_apiv3-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_apiv3-3.1.0/PKG-INFO` & `fyers_apiv3-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_apiv3
-Version: 3.1.0
+Version: 3.1.1
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_apiv3-3.1.0/README.md` & `fyers_apiv3-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/data_ws.py` & `fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/data_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
                         update_dict = False
                         dp_index_flag =True
 
                     if update_dict:
                         datadict[hsm_symbol] = symbol
                 if response_data["invalidSymbol"]:
                     wrong_symbol = response_data["invalidSymbol"]
-                # print("datadict",datadict)
                 return (datadict, wrong_symbol, dp_index_flag,"")
 
             elif response_data['s'] == "error":
                 
                 return ({}, [],dp_index_flag, response_data["message"])
 
 
@@ -1495,14 +1494,15 @@
         Handles the error message.
 
         Args:
             message (str): The error message.
         """
         if self.OnError is not None:
             self.OnError(message)
+            self.data_logger.error(message)
         else:
             if self.write_to_file:
                 self.data_logger.debug(f"ERROR Response:{message}")
             else:
                 print(f"Error: {message}")
 
 
@@ -1572,15 +1572,14 @@
             self.message_thread.start()
             self.ping_thread.start()
             message = self.__access_token_msg()
             # self.message.append(message)
             self.add_message(message)
             self.reconnect_attempts = 0
             self.reconnect_delay = 0
-            print(self.reconnect_attempts,self.reconnect_delay )
             if self.lite:
                 message = self.__lite_mode_msg()
                 # self.message.append(message)
                 self.add_message(message)
             else:
                 message = self.__full_mode_msg()
                 # self.message.append(message)
```

### Comparing `fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/defines.py` & `fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/map.json` & `fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/map.json`

 * *Files identical despite different names*

### Comparing `fyers_apiv3-3.1.0/fyers_apiv3/FyersWebsocket/order_ws.py` & `fyers_apiv3-3.1.1/fyers_apiv3/FyersWebsocket/order_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 
         Args:
             message (str): The error message.
 
         """
         if self.onerror is not None:
             self.onerror(message)
+            self.order_logger.error(message)
         else:
             if self.write_to_file:
                 self.order_logger.debug(f"Response:{message}")
             else:
                 print(f"Error Response : {message}")
 
     def __on_open(self, ws):
```

### Comparing `fyers_apiv3-3.1.0/fyers_apiv3/fyersModel.py` & `fyers_apiv3-3.1.1/fyers_apiv3/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv3-3.1.0/fyers_apiv3/fyers_logger.py` & `fyers_apiv3-3.1.1/fyers_apiv3/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv3-3.1.0/fyers_apiv3.egg-info/PKG-INFO` & `fyers_apiv3-3.1.1/fyers_apiv3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-apiv3
-Version: 3.1.0
+Version: 3.1.1
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_apiv3-3.1.0/setup.py` & `fyers_apiv3-3.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_apiv3',  
-     version='3.1.0',
+     version='3.1.1',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

