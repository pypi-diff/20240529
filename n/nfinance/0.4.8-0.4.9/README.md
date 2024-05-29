# Comparing `tmp/nfinance-0.4.8.tar.gz` & `tmp/nfinance-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nfinance-0.4.8.tar", last modified: Tue May 28 05:09:23 2024, max compression
+gzip compressed data, was "nfinance-0.4.9.tar", last modified: Tue May 28 05:24:42 2024, max compression
```

## Comparing `nfinance-0.4.8.tar` & `nfinance-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:09:23.471641 nfinance-0.4.8/
--rw-r--r--   0 root         (0) root         (0)     1064 2024-05-28 05:02:34.000000 nfinance-0.4.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3562 2024-05-28 05:09:23.471641 nfinance-0.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2962 2024-05-28 05:02:34.000000 nfinance-0.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:09:23.469640 nfinance-0.4.8/nfinance/
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-28 05:02:34.000000 nfinance-0.4.8/nfinance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-28 05:02:34.000000 nfinance-0.4.8/nfinance/financials.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-05-28 05:02:34.000000 nfinance-0.4.8/nfinance/rsi.py
--rw-r--r--   0 root         (0) root         (0)     3101 2024-05-28 05:07:07.000000 nfinance-0.4.8/nfinance/stock_data.py
--rw-r--r--   0 root         (0) root         (0)     4027 2024-05-28 05:02:34.000000 nfinance-0.4.8/nfinance/stock_listing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:09:23.470641 nfinance-0.4.8/nfinance.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3562 2024-05-28 05:09:23.000000 nfinance-0.4.8/nfinance.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2024-05-28 05:09:23.000000 nfinance-0.4.8/nfinance.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 05:09:23.000000 nfinance-0.4.8/nfinance.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-28 05:09:23.000000 nfinance-0.4.8/nfinance.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-28 05:09:23.000000 nfinance-0.4.8/nfinance.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 05:09:23.471641 nfinance-0.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-28 05:06:54.000000 nfinance-0.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:09:23.470641 nfinance-0.4.8/tests/
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-28 05:02:34.000000 nfinance-0.4.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3101 2024-05-28 05:04:33.000000 nfinance-0.4.8/tests/stock_data.py
--rw-r--r--   0 root         (0) root         (0)     1485 2024-05-28 05:02:34.000000 nfinance-0.4.8/tests/test_stock_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:24:42.852223 nfinance-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)     1064 2024-05-28 05:02:34.000000 nfinance-0.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3562 2024-05-28 05:24:42.852223 nfinance-0.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-05-28 05:02:34.000000 nfinance-0.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:24:42.850223 nfinance-0.4.9/nfinance/
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-28 05:02:34.000000 nfinance-0.4.9/nfinance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-28 05:02:34.000000 nfinance-0.4.9/nfinance/financials.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-05-28 05:02:34.000000 nfinance-0.4.9/nfinance/rsi.py
+-rw-r--r--   0 root         (0) root         (0)     3104 2024-05-28 05:23:15.000000 nfinance-0.4.9/nfinance/stock_data.py
+-rw-r--r--   0 root         (0) root         (0)     4027 2024-05-28 05:02:34.000000 nfinance-0.4.9/nfinance/stock_listing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:24:42.851223 nfinance-0.4.9/nfinance.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3562 2024-05-28 05:24:42.000000 nfinance-0.4.9/nfinance.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-28 05:24:42.000000 nfinance-0.4.9/nfinance.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 05:24:42.000000 nfinance-0.4.9/nfinance.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-28 05:24:42.000000 nfinance-0.4.9/nfinance.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-28 05:24:42.000000 nfinance-0.4.9/nfinance.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 05:24:42.852223 nfinance-0.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-28 05:23:01.000000 nfinance-0.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:24:42.852223 nfinance-0.4.9/tests/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-28 05:02:34.000000 nfinance-0.4.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3101 2024-05-28 05:04:33.000000 nfinance-0.4.9/tests/stock_data.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-28 05:02:34.000000 nfinance-0.4.9/tests/test_stock_data.py
```

### Comparing `nfinance-0.4.8/LICENSE` & `nfinance-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.8/PKG-INFO` & `nfinance-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfinance
-Version: 0.4.8
+Version: 0.4.9
 Summary: A simple finance data fetching library for Naver Finance data.
 Home-page: https://github.com/lega001/nfinance
 Author: lega001
 Author-email: lega01077970523@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nfinance-0.4.8/README.md` & `nfinance-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.8/nfinance/financials.py` & `nfinance-0.4.9/nfinance/financials.py`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.8/nfinance/stock_data.py` & `nfinance-0.4.9/tests/stock_data.py`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.8/nfinance/stock_listing.py` & `nfinance-0.4.9/nfinance/stock_listing.py`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.8/nfinance.egg-info/PKG-INFO` & `nfinance-0.4.9/nfinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfinance
-Version: 0.4.8
+Version: 0.4.9
 Summary: A simple finance data fetching library for Naver Finance data.
 Home-page: https://github.com/lega001/nfinance
 Author: lega001
 Author-email: lega01077970523@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nfinance-0.4.8/setup.py` & `nfinance-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='nfinance',
-    version='0.4.8',
+    version='0.4.9',
     author='lega001',
     author_email='lega01077970523@gmail.com',
     packages=find_packages(),
     install_requires=[
         'pandas',  # 예시: pandas 라이브러리가 필요한 경우
         'requests',  # 예시: HTTP 요청을 위해 requests 라이브러리가 필요한 경우
         'tqdm',
```

### Comparing `nfinance-0.4.8/tests/stock_data.py` & `nfinance-0.4.9/nfinance/stock_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.end_date = end_date
         self.interval = interval
         self.max_retries = max_retries
         self.retry_delay = retry_delay
         self.base_url = self.set_base_url()
 
     def set_base_url(self):
-        if re.match(r'^\d{6}$', self.ticker) or re.match(r'^\d{5}K$', self.ticker):
+        if re.match(r'^\d{6}$', self.ticker) or re.match(r'^\d{5}[KL]$', self.ticker):
             return "https://api.stock.naver.com/chart/domestic/item/"
         else:
             return "https://api.stock.naver.com/chart/foreign/item/"
 
     def download(self):
         start_datetime = datetime.strptime(self.start_date, '%Y-%m-%d')
         end_datetime = datetime.strptime(self.end_date, '%Y-%m-%d')
```

### Comparing `nfinance-0.4.8/tests/test_stock_data.py` & `nfinance-0.4.9/tests/test_stock_data.py`

 * *Files identical despite different names*

