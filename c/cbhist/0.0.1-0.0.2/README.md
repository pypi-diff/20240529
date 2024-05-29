# Comparing `tmp/cbhist-0.0.1.tar.gz` & `tmp/cbhist-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbhist-0.0.1.tar", last modified: Mon May 13 18:04:05 2024, max compression
+gzip compressed data, was "cbhist-0.0.2.tar", last modified: Wed May 29 21:33:21 2024, max compression
```

## Comparing `cbhist-0.0.1.tar` & `cbhist-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-13 18:04:05.456975 cbhist-0.0.1/
--rw-r--r--   0 sackfield   (501) staff       (20)     1071 2024-05-13 13:28:37.000000 cbhist-0.0.1/LICENSE
--rw-r--r--   0 sackfield   (501) staff       (20)       85 2024-05-13 13:30:18.000000 cbhist-0.0.1/MANIFEST.in
--rw-r--r--   0 sackfield   (501) staff       (20)     2346 2024-05-13 18:04:05.456775 cbhist-0.0.1/PKG-INFO
--rw-r--r--   0 sackfield   (501) staff       (20)     1770 2024-05-13 14:01:20.000000 cbhist-0.0.1/README.md
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-13 18:04:05.455897 cbhist-0.0.1/cbhist/
--rw-r--r--   0 sackfield   (501) staff       (20)       46 2024-05-13 13:48:38.000000 cbhist-0.0.1/cbhist/__init__.py
--rw-r--r--   0 sackfield   (501) staff       (20)     1217 2024-05-13 17:54:30.000000 cbhist-0.0.1/cbhist/candles.py
--rw-r--r--   0 sackfield   (501) staff       (20)     1785 2024-05-13 18:01:38.000000 cbhist-0.0.1/cbhist/historical.py
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-13 18:04:05.456549 cbhist-0.0.1/cbhist.egg-info/
--rw-r--r--   0 sackfield   (501) staff       (20)     2346 2024-05-13 18:04:05.000000 cbhist-0.0.1/cbhist.egg-info/PKG-INFO
--rw-r--r--   0 sackfield   (501) staff       (20)      291 2024-05-13 18:04:05.000000 cbhist-0.0.1/cbhist.egg-info/SOURCES.txt
--rw-r--r--   0 sackfield   (501) staff       (20)        1 2024-05-13 18:04:05.000000 cbhist-0.0.1/cbhist.egg-info/dependency_links.txt
--rw-r--r--   0 sackfield   (501) staff       (20)        1 2024-05-13 18:04:05.000000 cbhist-0.0.1/cbhist.egg-info/not-zip-safe
--rw-r--r--   0 sackfield   (501) staff       (20)       60 2024-05-13 18:04:05.000000 cbhist-0.0.1/cbhist.egg-info/requires.txt
--rw-r--r--   0 sackfield   (501) staff       (20)        7 2024-05-13 18:04:05.000000 cbhist-0.0.1/cbhist.egg-info/top_level.txt
--rw-r--r--   0 sackfield   (501) staff       (20)       60 2024-05-13 13:48:02.000000 cbhist-0.0.1/requirements.txt
--rw-r--r--   0 sackfield   (501) staff       (20)       38 2024-05-13 18:04:05.457012 cbhist-0.0.1/setup.cfg
--rw-r--r--   0 sackfield   (501) staff       (20)     1289 2024-05-13 13:32:52.000000 cbhist-0.0.1/setup.py
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-29 21:33:21.926887 cbhist-0.0.2/
+-rw-r--r--   0 sackfield   (501) staff       (20)     1071 2024-05-13 13:28:37.000000 cbhist-0.0.2/LICENSE
+-rw-r--r--   0 sackfield   (501) staff       (20)       85 2024-05-13 13:30:18.000000 cbhist-0.0.2/MANIFEST.in
+-rw-r--r--   0 sackfield   (501) staff       (20)     2306 2024-05-29 21:33:21.926655 cbhist-0.0.2/PKG-INFO
+-rw-r--r--   0 sackfield   (501) staff       (20)     1730 2024-05-29 21:32:50.000000 cbhist-0.0.2/README.md
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-29 21:33:21.925707 cbhist-0.0.2/cbhist/
+-rw-r--r--   0 sackfield   (501) staff       (20)       46 2024-05-13 13:48:38.000000 cbhist-0.0.2/cbhist/__init__.py
+-rw-r--r--   0 sackfield   (501) staff       (20)     1217 2024-05-13 17:54:30.000000 cbhist-0.0.2/cbhist/candles.py
+-rw-r--r--   0 sackfield   (501) staff       (20)     1785 2024-05-13 18:01:38.000000 cbhist-0.0.2/cbhist/historical.py
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-29 21:33:21.926419 cbhist-0.0.2/cbhist.egg-info/
+-rw-r--r--   0 sackfield   (501) staff       (20)     2306 2024-05-29 21:33:21.000000 cbhist-0.0.2/cbhist.egg-info/PKG-INFO
+-rw-r--r--   0 sackfield   (501) staff       (20)      291 2024-05-29 21:33:21.000000 cbhist-0.0.2/cbhist.egg-info/SOURCES.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)        1 2024-05-29 21:33:21.000000 cbhist-0.0.2/cbhist.egg-info/dependency_links.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)        1 2024-05-13 18:04:05.000000 cbhist-0.0.2/cbhist.egg-info/not-zip-safe
+-rw-r--r--   0 sackfield   (501) staff       (20)       60 2024-05-29 21:33:21.000000 cbhist-0.0.2/cbhist.egg-info/requires.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)        7 2024-05-29 21:33:21.000000 cbhist-0.0.2/cbhist.egg-info/top_level.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)       60 2024-05-29 21:32:24.000000 cbhist-0.0.2/requirements.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)       38 2024-05-29 21:33:21.926935 cbhist-0.0.2/setup.cfg
+-rw-r--r--   0 sackfield   (501) staff       (20)     1289 2024-05-29 21:32:29.000000 cbhist-0.0.2/setup.py
```

### Comparing `cbhist-0.0.1/LICENSE` & `cbhist-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cbhist-0.0.1/PKG-INFO` & `cbhist-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cbhist
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library for pulling in historical candles from coinbase.
 Home-page: https://github.com/8W9aG/cbhist
 Author: Will Sackfield
 Author-email: will.sackfield@gmail.com
 License: MIT
 Keywords: coinbase history historical price candle
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
-Requires-Dist: pandas>=2.2.2
+Requires-Dist: pandas>=2.2.1
 Requires-Dist: tqdm>=4.66.4
 Requires-Dist: tenacity>=8.3.0
 
 # cbhist
 
 <a href="https://pypi.org/project/cbhist/">
     <img alt="PyPi" src="https://img.shields.io/pypi/v/cbhist">
@@ -41,15 +41,15 @@
 
 This is a python package hosted on pypi, so to install simply run the following command:
 
 `pip install cbhist`
 
 ## Usage example :eyes:
 
-To pull a dataframe containing all the information for a particular league, the following example can be used:
+To pull a dataframe containing all the candles for a coinbase product:
 
 ```python
 import datetime
 
 from cbhist.historical import fetch_historical
 
 granularity = 60 # Candle for every minute
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: cbhist Version: 0.0.1 Summary: A python library for
+Metadata-Version: 2.1 Name: cbhist Version: 0.0.2 Summary: A python library for
 pulling in historical candles from coinbase. Home-page: https://github.com/
 8W9aG/cbhist Author: Will Sackfield Author-email: will.sackfield@gmail.com
 License: MIT Keywords: coinbase history historical price candle Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: requests>=2.31.0 Requires-Dist: pandas>=2.2.2 Requires-Dist:
+Requires-Dist: requests>=2.31.0 Requires-Dist: pandas>=2.2.1 Requires-Dist:
 tqdm>=4.66.4 Requires-Dist: tenacity>=8.3.0 # cbhist _[_P_y_P_i_]A python library for
 pulling in historical candles from coinbase. ## Dependencies :
 globe_with_meridians: Python 3.11.6: - [pandas](https://pandas.pydata.org/) -
 [requests](https://requests.readthedocs.io/en/latest/) - [tqdm](https://
 github.com/tqdm/tqdm) - [tenacity](https://tenacity.readthedocs.io/en/latest/
 ) ## Raison D'Ãªtre :thought_balloon: The [coinbase exchange API](https://
 docs.cloud.coinbase.com/exchange/reference/exchangerestapi_getproductcandles)
@@ -17,14 +17,13 @@
 Typically the approach is to iterate across a time series and perform a request
 for each time chunk, however this can be sped up greatly by doing a binary
 search before doing an iterative pull to determine when the asset begins to
 have candles. Formalising this into a proper library produces a dataframe made
 it easier to work in different projects than re-inventing the wheel each time.
 ## Installation :inbox_tray: This is a python package hosted on pypi, so to
 install simply run the following command: `pip install cbhist` ## Usage example
-:eyes: To pull a dataframe containing all the information for a particular
-league, the following example can be used: ```python import datetime from
-cbhist.historical import fetch_historical granularity = 60 # Candle for every
-minute df = fetch_coinbase("ETH-USD", granularity, datetime.datetime(2010, 1,
-1)) ``` This results in a dataframe with a datetime index and OHLC (+ volume)
-columns. ## License :memo: The project is available under the [MIT License]
-(LICENSE).
+:eyes: To pull a dataframe containing all the candles for a coinbase product:
+```python import datetime from cbhist.historical import fetch_historical
+granularity = 60 # Candle for every minute df = fetch_coinbase("ETH-USD",
+granularity, datetime.datetime(2010, 1, 1)) ``` This results in a dataframe
+with a datetime index and OHLC (+ volume) columns. ## License :memo: The
+project is available under the [MIT License](LICENSE).
```

### Comparing `cbhist-0.0.1/README.md` & `cbhist-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 This is a python package hosted on pypi, so to install simply run the following command:
 
 `pip install cbhist`
 
 ## Usage example :eyes:
 
-To pull a dataframe containing all the information for a particular league, the following example can be used:
+To pull a dataframe containing all the candles for a coinbase product:
 
 ```python
 import datetime
 
 from cbhist.historical import fetch_historical
 
 granularity = 60 # Candle for every minute
```

#### html2text {}

```diff
@@ -10,13 +10,13 @@
 across a time series and perform a request for each time chunk, however this
 can be sped up greatly by doing a binary search before doing an iterative pull
 to determine when the asset begins to have candles. Formalising this into a
 proper library produces a dataframe made it easier to work in different
 projects than re-inventing the wheel each time. ## Installation :inbox_tray:
 This is a python package hosted on pypi, so to install simply run the following
 command: `pip install cbhist` ## Usage example :eyes: To pull a dataframe
-containing all the information for a particular league, the following example
-can be used: ```python import datetime from cbhist.historical import
-fetch_historical granularity = 60 # Candle for every minute df = fetch_coinbase
-("ETH-USD", granularity, datetime.datetime(2010, 1, 1)) ``` This results in a
-dataframe with a datetime index and OHLC (+ volume) columns. ## License :memo:
-The project is available under the [MIT License](LICENSE).
+containing all the candles for a coinbase product: ```python import datetime
+from cbhist.historical import fetch_historical granularity = 60 # Candle for
+every minute df = fetch_coinbase("ETH-USD", granularity, datetime.datetime
+(2010, 1, 1)) ``` This results in a dataframe with a datetime index and OHLC (+
+volume) columns. ## License :memo: The project is available under the [MIT
+License](LICENSE).
```

### Comparing `cbhist-0.0.1/cbhist/candles.py` & `cbhist-0.0.2/cbhist/candles.py`

 * *Files identical despite different names*

### Comparing `cbhist-0.0.1/cbhist/historical.py` & `cbhist-0.0.2/cbhist/historical.py`

 * *Files identical despite different names*

### Comparing `cbhist-0.0.1/cbhist.egg-info/PKG-INFO` & `cbhist-0.0.2/cbhist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cbhist
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library for pulling in historical candles from coinbase.
 Home-page: https://github.com/8W9aG/cbhist
 Author: Will Sackfield
 Author-email: will.sackfield@gmail.com
 License: MIT
 Keywords: coinbase history historical price candle
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
-Requires-Dist: pandas>=2.2.2
+Requires-Dist: pandas>=2.2.1
 Requires-Dist: tqdm>=4.66.4
 Requires-Dist: tenacity>=8.3.0
 
 # cbhist
 
 <a href="https://pypi.org/project/cbhist/">
     <img alt="PyPi" src="https://img.shields.io/pypi/v/cbhist">
@@ -41,15 +41,15 @@
 
 This is a python package hosted on pypi, so to install simply run the following command:
 
 `pip install cbhist`
 
 ## Usage example :eyes:
 
-To pull a dataframe containing all the information for a particular league, the following example can be used:
+To pull a dataframe containing all the candles for a coinbase product:
 
 ```python
 import datetime
 
 from cbhist.historical import fetch_historical
 
 granularity = 60 # Candle for every minute
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: cbhist Version: 0.0.1 Summary: A python library for
+Metadata-Version: 2.1 Name: cbhist Version: 0.0.2 Summary: A python library for
 pulling in historical candles from coinbase. Home-page: https://github.com/
 8W9aG/cbhist Author: Will Sackfield Author-email: will.sackfield@gmail.com
 License: MIT Keywords: coinbase history historical price candle Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: requests>=2.31.0 Requires-Dist: pandas>=2.2.2 Requires-Dist:
+Requires-Dist: requests>=2.31.0 Requires-Dist: pandas>=2.2.1 Requires-Dist:
 tqdm>=4.66.4 Requires-Dist: tenacity>=8.3.0 # cbhist _[_P_y_P_i_]A python library for
 pulling in historical candles from coinbase. ## Dependencies :
 globe_with_meridians: Python 3.11.6: - [pandas](https://pandas.pydata.org/) -
 [requests](https://requests.readthedocs.io/en/latest/) - [tqdm](https://
 github.com/tqdm/tqdm) - [tenacity](https://tenacity.readthedocs.io/en/latest/
 ) ## Raison D'Ãªtre :thought_balloon: The [coinbase exchange API](https://
 docs.cloud.coinbase.com/exchange/reference/exchangerestapi_getproductcandles)
@@ -17,14 +17,13 @@
 Typically the approach is to iterate across a time series and perform a request
 for each time chunk, however this can be sped up greatly by doing a binary
 search before doing an iterative pull to determine when the asset begins to
 have candles. Formalising this into a proper library produces a dataframe made
 it easier to work in different projects than re-inventing the wheel each time.
 ## Installation :inbox_tray: This is a python package hosted on pypi, so to
 install simply run the following command: `pip install cbhist` ## Usage example
-:eyes: To pull a dataframe containing all the information for a particular
-league, the following example can be used: ```python import datetime from
-cbhist.historical import fetch_historical granularity = 60 # Candle for every
-minute df = fetch_coinbase("ETH-USD", granularity, datetime.datetime(2010, 1,
-1)) ``` This results in a dataframe with a datetime index and OHLC (+ volume)
-columns. ## License :memo: The project is available under the [MIT License]
-(LICENSE).
+:eyes: To pull a dataframe containing all the candles for a coinbase product:
+```python import datetime from cbhist.historical import fetch_historical
+granularity = 60 # Candle for every minute df = fetch_coinbase("ETH-USD",
+granularity, datetime.datetime(2010, 1, 1)) ``` This results in a dataframe
+with a datetime index and OHLC (+ volume) columns. ## License :memo: The
+project is available under the [MIT License](LICENSE).
```

### Comparing `cbhist-0.0.1/setup.py` & `cbhist-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             if not x.startswith(".") and not x.startswith("-e")
         ]
     return requires
 
 
 setup(
     name='cbhist',
-    version='0.0.1',
+    version='0.0.2',
     description='A python library for pulling in historical candles from coinbase.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
```

