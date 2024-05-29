# Comparing `tmp/AmazonTicoTool-0.1-py3-none-any.whl.zip` & `tmp/AmazonTicoTool-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5831 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    12977 b- defN 24-May-28 13:50 AmazonTicoTool/__init__.py
--rw-rw-rw-  2.0 fat     1069 b- defN 24-May-28 14:01 AmazonTicoTool-0.1.dist-info/LICENCE.txt
--rw-rw-rw-  2.0 fat      461 b- defN 24-May-28 14:01 AmazonTicoTool-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 14:01 AmazonTicoTool-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-May-28 14:01 AmazonTicoTool-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      498 b- defN 24-May-28 14:01 AmazonTicoTool-0.1.dist-info/RECORD
-6 files, 15112 bytes uncompressed, 4925 bytes compressed:  67.4%
+Zip file size: 6598 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    12925 b- defN 24-May-29 06:08 AmazonTicoTool/__init__.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 24-May-29 06:08 AmazonTicoTool-0.3.dist-info/LICENCE.txt
+-rw-rw-rw-  2.0 fat     2074 b- defN 24-May-29 06:08 AmazonTicoTool-0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-29 06:08 AmazonTicoTool-0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-29 06:08 AmazonTicoTool-0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      499 b- defN 24-May-29 06:08 AmazonTicoTool-0.3.dist-info/RECORD
+6 files, 16674 bytes uncompressed, 5692 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: AmazonTicoTool/__init__.py
 Comment: 
 
-Filename: AmazonTicoTool-0.1.dist-info/LICENCE.txt
+Filename: AmazonTicoTool-0.3.dist-info/LICENCE.txt
 Comment: 
 
-Filename: AmazonTicoTool-0.1.dist-info/METADATA
+Filename: AmazonTicoTool-0.3.dist-info/METADATA
 Comment: 
 
-Filename: AmazonTicoTool-0.1.dist-info/WHEEL
+Filename: AmazonTicoTool-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: AmazonTicoTool-0.1.dist-info/top_level.txt
+Filename: AmazonTicoTool-0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: AmazonTicoTool-0.1.dist-info/RECORD
+Filename: AmazonTicoTool-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## AmazonTicoTool/__init__.py

```diff
@@ -1,17 +1,15 @@
 import pandas as pd
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.chrome.service import Service
 import browser_cookie3
-
-import warnings
 from time import sleep
-warnings.filterwarnings("ignore")
+
 
 def mid_way_Authentication():
         
         options = webdriver.ChromeOptions()
         options.add_argument("--ignore-certificate-errors")
         options.add_argument("--acceptInsecureCerts")
         options.add_argument("--disable-notifications")
```

## Comparing `AmazonTicoTool-0.1.dist-info/LICENCE.txt` & `AmazonTicoTool-0.3.dist-info/LICENCE.txt`

 * *Files identical despite different names*

