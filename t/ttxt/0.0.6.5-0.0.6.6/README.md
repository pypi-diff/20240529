# Comparing `tmp/ttxt-0.0.6.5.tar.gz` & `tmp/ttxt-0.0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttxt-0.0.6.5.tar", last modified: Mon May 20 19:56:42 2024, max compression
+gzip compressed data, was "ttxt-0.0.6.6.tar", last modified: Wed May 29 09:23:01 2024, max compression
```

## Comparing `ttxt-0.0.6.5.tar` & `ttxt-0.0.6.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-20 19:56:42.233382 ttxt-0.0.6.5/
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.6.5/LICENSE
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-20 19:56:42.233265 ttxt-0.0.6.5/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.6.5/README.md
--rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-05-20 19:56:42.233427 ttxt-0.0.6.5/setup.cfg
--rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-05-20 19:56:21.000000 ttxt-0.0.6.5/setup.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-20 19:56:42.224327 ttxt-0.0.6.5/ttxt/
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1101 2024-05-03 15:38:46.000000 ttxt-0.0.6.5/ttxt/__init__.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-20 19:56:42.225360 ttxt-0.0.6.5/ttxt/base/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.6.5/ttxt/base/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.6.5/ttxt/base/baseFuturesExchange.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.6.5/ttxt/base/baseSpotExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-20 19:56:42.231387 ttxt-0.0.6.5/ttxt/exchanges/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.6.5/ttxt/exchanges/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11536 2024-05-20 19:55:58.000000 ttxt-0.0.6.5/ttxt/exchanges/ascendex.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.6.5/ttxt/exchanges/biconomy.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.6.5/ttxt/exchanges/binance.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.6.5/ttxt/exchanges/bingx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.6.5/ttxt/exchanges/bitget.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.6.5/ttxt/exchanges/bitgetFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.6.5/ttxt/exchanges/bitmart.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    21199 2024-05-02 08:57:55.000000 ttxt-0.0.6.5/ttxt/exchanges/bybit.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.6.5/ttxt/exchanges/bybitFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.6.5/ttxt/exchanges/cryptocom.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.6.5/ttxt/exchanges/gateFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    15293 2024-05-07 14:02:35.000000 ttxt-0.0.6.5/ttxt/exchanges/gateio.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.6.5/ttxt/exchanges/huobi.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.6.5/ttxt/exchanges/kucoin.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.6.5/ttxt/exchanges/mexc.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.6.5/ttxt/exchanges/okx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.6.5/ttxt/exchanges/xt.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-20 19:56:42.231564 ttxt-0.0.6.5/ttxt/tests/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.6.5/ttxt/tests/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10237 2024-05-14 15:17:38.000000 ttxt-0.0.6.5/ttxt/tests/testExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-20 19:56:42.232024 ttxt-0.0.6.5/ttxt/types/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.6.5/ttxt/types/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.6.5/ttxt/types/baseTypes.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-20 19:56:42.232656 ttxt-0.0.6.5/ttxt/utils/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.6.5/ttxt/utils/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.6.5/ttxt/utils/general.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.6.5/ttxt/utils/xtUtils.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-20 19:56:42.224902 ttxt-0.0.6.5/ttxt.egg-info/
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-20 19:56:42.000000 ttxt-0.0.6.5/ttxt.egg-info/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)      871 2024-05-20 19:56:42.000000 ttxt-0.0.6.5/ttxt.egg-info/SOURCES.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-05-20 19:56:42.000000 ttxt-0.0.6.5/ttxt.egg-info/dependency_links.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-05-20 19:56:42.000000 ttxt-0.0.6.5/ttxt.egg-info/top_level.txt
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-29 09:23:01.761738 ttxt-0.0.6.6/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.6.6/LICENSE
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-29 09:23:01.761586 ttxt-0.0.6.6/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.6.6/README.md
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-05-29 09:23:01.761813 ttxt-0.0.6.6/setup.cfg
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-05-29 09:22:42.000000 ttxt-0.0.6.6/setup.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-29 09:23:01.753145 ttxt-0.0.6.6/ttxt/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1101 2024-05-03 15:38:46.000000 ttxt-0.0.6.6/ttxt/__init__.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-29 09:23:01.754271 ttxt-0.0.6.6/ttxt/base/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.6.6/ttxt/base/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.6.6/ttxt/base/baseFuturesExchange.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.6.6/ttxt/base/baseSpotExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-29 09:23:01.759780 ttxt-0.0.6.6/ttxt/exchanges/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.6.6/ttxt/exchanges/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11536 2024-05-20 19:55:58.000000 ttxt-0.0.6.6/ttxt/exchanges/ascendex.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.6.6/ttxt/exchanges/biconomy.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.6.6/ttxt/exchanges/binance.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.6.6/ttxt/exchanges/bingx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.6.6/ttxt/exchanges/bitget.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.6.6/ttxt/exchanges/bitgetFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.6.6/ttxt/exchanges/bitmart.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    21219 2024-05-29 09:22:11.000000 ttxt-0.0.6.6/ttxt/exchanges/bybit.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.6.6/ttxt/exchanges/bybitFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.6.6/ttxt/exchanges/cryptocom.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.6.6/ttxt/exchanges/gateFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    15293 2024-05-07 14:02:35.000000 ttxt-0.0.6.6/ttxt/exchanges/gateio.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.6.6/ttxt/exchanges/huobi.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.6.6/ttxt/exchanges/kucoin.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.6.6/ttxt/exchanges/mexc.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.6.6/ttxt/exchanges/okx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.6.6/ttxt/exchanges/xt.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-29 09:23:01.759972 ttxt-0.0.6.6/ttxt/tests/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.6.6/ttxt/tests/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10237 2024-05-14 15:17:38.000000 ttxt-0.0.6.6/ttxt/tests/testExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-29 09:23:01.760343 ttxt-0.0.6.6/ttxt/types/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.6.6/ttxt/types/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.6.6/ttxt/types/baseTypes.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-29 09:23:01.761009 ttxt-0.0.6.6/ttxt/utils/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.6.6/ttxt/utils/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.6.6/ttxt/utils/general.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.6.6/ttxt/utils/xtUtils.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-29 09:23:01.753732 ttxt-0.0.6.6/ttxt.egg-info/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-29 09:23:01.000000 ttxt-0.0.6.6/ttxt.egg-info/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      871 2024-05-29 09:23:01.000000 ttxt-0.0.6.6/ttxt.egg-info/SOURCES.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-05-29 09:23:01.000000 ttxt-0.0.6.6/ttxt.egg-info/dependency_links.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-05-29 09:23:01.000000 ttxt-0.0.6.6/ttxt.egg-info/top_level.txt
```

### Comparing `ttxt-0.0.6.5/LICENSE` & `ttxt-0.0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/__init__.py` & `ttxt-0.0.6.6/ttxt/__init__.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/base/baseFuturesExchange.py` & `ttxt-0.0.6.6/ttxt/base/baseFuturesExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/base/baseSpotExchange.py` & `ttxt-0.0.6.6/ttxt/base/baseSpotExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/ascendex.py` & `ttxt-0.0.6.6/ttxt/exchanges/ascendex.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/biconomy.py` & `ttxt-0.0.6.6/ttxt/exchanges/biconomy.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/binance.py` & `ttxt-0.0.6.6/ttxt/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/bingx.py` & `ttxt-0.0.6.6/ttxt/exchanges/bingx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/bitget.py` & `ttxt-0.0.6.6/ttxt/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/bitgetFutures.py` & `ttxt-0.0.6.6/ttxt/exchanges/bitgetFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/bitmart.py` & `ttxt-0.0.6.6/ttxt/exchanges/bitmart.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/bybit.py` & `ttxt-0.0.6.6/ttxt/exchanges/bybit.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,16 +352,16 @@
             parsedTrade["takerOrMaker"] = "maker" if trade["isMaker"] else "taker"
             if "execTime" in trade:
                 parsedTrade["timestamp"] = int(float(trade["execTime"]))
                 parsedTrade["datetime"] = general.ts_to_datetime(parsedTrade["timestamp"])
             else: 
                 parsedTrade["timestamp"] = None
                 parsedTrade["datetime"] = None
-            parsedTrade["feeCurrency"] = trade["feeCurrency"]
-            parsedTrade["fee"] = trade["feeRate"]
+            parsedTrade["feeCurrency"] = trade.get("feeCurrency", None)
+            parsedTrade["fee"] = trade.get("feeRate", None)
             return parsedTrade
         parsedTradeList = []
         if trades['retCode'] != 0: raise Exception(trades['retMsg'])
         for trade in trades['result']['list']:
             parsedTradeList.append(parseTrade(trade))
         return parsedTradeList
```

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/bybitFutures.py` & `ttxt-0.0.6.6/ttxt/exchanges/bybitFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/cryptocom.py` & `ttxt-0.0.6.6/ttxt/exchanges/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/gateFutures.py` & `ttxt-0.0.6.6/ttxt/exchanges/gateFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/gateio.py` & `ttxt-0.0.6.6/ttxt/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/huobi.py` & `ttxt-0.0.6.6/ttxt/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/kucoin.py` & `ttxt-0.0.6.6/ttxt/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/mexc.py` & `ttxt-0.0.6.6/ttxt/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/exchanges/okx.py` & `ttxt-0.0.6.6/ttxt/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/tests/testExchange.py` & `ttxt-0.0.6.6/ttxt/tests/testExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/types/baseTypes.py` & `ttxt-0.0.6.6/ttxt/types/baseTypes.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/utils/general.py` & `ttxt-0.0.6.6/ttxt/utils/general.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt/utils/xtUtils.py` & `ttxt-0.0.6.6/ttxt/utils/xtUtils.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.5/ttxt.egg-info/SOURCES.txt` & `ttxt-0.0.6.6/ttxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

