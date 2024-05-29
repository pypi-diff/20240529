# Comparing `tmp/py_alpaca_daily_losers-0.3.1.tar.gz` & `tmp/py_alpaca_daily_losers-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_daily_losers-0.3.1.tar", max compression
+gzip compressed data, was "py_alpaca_daily_losers-0.3.2.tar", max compression
```

## Comparing `py_alpaca_daily_losers-0.3.1.tar` & `py_alpaca_daily_losers-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/LICENSE
--rw-r--r--   0        0        0    13887 2024-05-27 04:08:54.588515 py_alpaca_daily_losers-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/__init__.py
--rw-r--r--   0        0        0    21144 2024-05-28 23:12:37.168330 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/daily_losers.py
--rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/__init__.py
--rw-r--r--   0        0        0     1407 2024-05-27 03:42:55.091127 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/article_extractor.py
--rw-r--r--   0        0        0      481 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/global_fuctions.py
--rw-r--r--   0        0        0      936 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/marketaux.py
--rw-r--r--   0        0        0     2527 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/openai.py
--rw-r--r--   0        0        0     1927 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/slack.py
--rw-r--r--   0        0        0      906 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/yahoo.py
--rw-r--r--   0        0        0      713 2024-05-28 23:12:37.168330 py_alpaca_daily_losers-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    14591 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.2/LICENSE
+-rw-r--r--   0        0        0    13887 2024-05-27 04:08:54.588515 py_alpaca_daily_losers-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/__init__.py
+-rw-r--r--   0        0        0    21108 2024-05-28 23:53:31.295493 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/daily_losers.py
+-rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/__init__.py
+-rw-r--r--   0        0        0     1407 2024-05-27 03:42:55.091127 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/article_extractor.py
+-rw-r--r--   0        0        0      481 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/global_fuctions.py
+-rw-r--r--   0        0        0      936 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/marketaux.py
+-rw-r--r--   0        0        0     2527 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/openai.py
+-rw-r--r--   0        0        0     1927 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/slack.py
+-rw-r--r--   0        0        0      906 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/yahoo.py
+-rw-r--r--   0        0        0      713 2024-05-28 23:53:31.295493 py_alpaca_daily_losers-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    14591 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.3.2/PKG-INFO
```

### Comparing `py_alpaca_daily_losers-0.3.1/LICENSE` & `py_alpaca_daily_losers-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.1/README.md` & `py_alpaca_daily_losers-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/daily_losers.py` & `py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/daily_losers.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,14 @@
 
         Returns:
         None
 
         Raises:
         ValueError: If an error occurs while updating the watchlist, a new watchlist will be created instead.
         """
-        symbols = ','.join(symbols)
         try:
             self.alpaca.watchlist.update(watchlist_name=name, symbols=symbols)
         except Exception:
             self.alpaca.watchlist.create(name=name, symbols=symbols)
 
     ########################################################
     # Define the filter_tickers_with_news method
```

### Comparing `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/article_extractor.py` & `py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/article_extractor.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/marketaux.py` & `py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/marketaux.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/openai.py` & `py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/openai.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/slack.py` & `py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/slack.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/yahoo.py` & `py_alpaca_daily_losers-0.3.2/py_alpaca_daily_losers/src/yahoo.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.1/pyproject.toml` & `py_alpaca_daily_losers-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-daily-losers"
-version = "0.3.1"
+version = "0.3.2"
 description = "Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration."
 authors = ["TexasCoding <jeff10278@me.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 python-dotenv = "^1.0.1"
```

### Comparing `py_alpaca_daily_losers-0.3.1/PKG-INFO` & `py_alpaca_daily_losers-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-daily-losers
-Version: 0.3.1
+Version: 0.3.2
 Summary: Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration.
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.30.1,<2.0.0)
```

