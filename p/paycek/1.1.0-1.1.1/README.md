# Comparing `tmp/paycek-1.1.0.tar.gz` & `tmp/paycek-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paycek-1.1.0.tar", last modified: Tue Apr  4 14:04:16 2023, max compression
+gzip compressed data, was "paycek-1.1.1.tar", last modified: Wed May 29 19:16:56 2024, max compression
```

## Comparing `paycek-1.1.0.tar` & `paycek-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 antun      (501) staff       (20)        0 2023-04-04 14:04:16.777439 paycek-1.1.0/
--rw-r--r--   0 antun      (501) staff       (20)     1075 2022-12-23 10:33:04.000000 paycek-1.1.0/LICENSE
--rw-r--r--   0 antun      (501) staff       (20)     1446 2023-04-04 14:04:16.777268 paycek-1.1.0/PKG-INFO
--rw-r--r--   0 antun      (501) staff       (20)      794 2023-02-01 15:36:42.000000 paycek-1.1.0/README.md
--rw-r--r--   0 antun      (501) staff       (20)      683 2023-04-03 14:34:16.000000 paycek-1.1.0/pyproject.toml
--rw-r--r--   0 antun      (501) staff       (20)       38 2023-04-04 14:04:16.777483 paycek-1.1.0/setup.cfg
--rw-r--r--   0 antun      (501) staff       (20)       61 2023-01-13 12:19:40.000000 paycek-1.1.0/setup.py
-drwxr-xr-x   0 antun      (501) staff       (20)        0 2023-04-04 14:04:16.776378 paycek-1.1.0/src/
--rw-r--r--   0 antun      (501) staff       (20)        0 2022-12-22 16:50:08.000000 paycek-1.1.0/src/__init__.py
-drwxr-xr-x   0 antun      (501) staff       (20)        0 2023-04-04 14:04:16.777083 paycek-1.1.0/src/paycek.egg-info/
--rw-r--r--   0 antun      (501) staff       (20)     1446 2023-04-04 14:04:16.000000 paycek-1.1.0/src/paycek.egg-info/PKG-INFO
--rw-r--r--   0 antun      (501) staff       (20)      207 2023-04-04 14:04:16.000000 paycek-1.1.0/src/paycek.egg-info/SOURCES.txt
--rw-r--r--   0 antun      (501) staff       (20)        1 2023-04-04 14:04:16.000000 paycek-1.1.0/src/paycek.egg-info/dependency_links.txt
--rw-r--r--   0 antun      (501) staff       (20)       16 2023-04-04 14:04:16.000000 paycek-1.1.0/src/paycek.egg-info/top_level.txt
--rw-r--r--   0 antun      (501) staff       (20)     7274 2023-04-03 14:28:48.000000 paycek-1.1.0/src/paycek.py
+drwxr-xr-x   0 antun      (501) staff       (20)        0 2024-05-29 19:16:56.619252 paycek-1.1.1/
+-rw-r--r--   0 antun      (501) staff       (20)     1075 2023-05-05 14:16:40.000000 paycek-1.1.1/LICENSE
+-rw-r--r--   0 antun      (501) staff       (20)     1446 2024-05-29 19:16:56.619008 paycek-1.1.1/PKG-INFO
+-rw-r--r--   0 antun      (501) staff       (20)      794 2023-05-05 14:16:40.000000 paycek-1.1.1/README.md
+-rw-r--r--   0 antun      (501) staff       (20)      683 2024-05-29 15:27:35.000000 paycek-1.1.1/pyproject.toml
+-rw-r--r--   0 antun      (501) staff       (20)       38 2024-05-29 19:16:56.619297 paycek-1.1.1/setup.cfg
+-rw-r--r--   0 antun      (501) staff       (20)       61 2023-05-05 14:16:40.000000 paycek-1.1.1/setup.py
+drwxr-xr-x   0 antun      (501) staff       (20)        0 2024-05-29 19:16:56.617739 paycek-1.1.1/src/
+-rw-r--r--   0 antun      (501) staff       (20)        0 2023-05-05 14:16:40.000000 paycek-1.1.1/src/__init__.py
+drwxr-xr-x   0 antun      (501) staff       (20)        0 2024-05-29 19:16:56.618773 paycek-1.1.1/src/paycek.egg-info/
+-rw-r--r--   0 antun      (501) staff       (20)     1446 2024-05-29 19:16:56.000000 paycek-1.1.1/src/paycek.egg-info/PKG-INFO
+-rw-r--r--   0 antun      (501) staff       (20)      207 2024-05-29 19:16:56.000000 paycek-1.1.1/src/paycek.egg-info/SOURCES.txt
+-rw-r--r--   0 antun      (501) staff       (20)        1 2024-05-29 19:16:56.000000 paycek-1.1.1/src/paycek.egg-info/dependency_links.txt
+-rw-r--r--   0 antun      (501) staff       (20)       16 2024-05-29 19:16:56.000000 paycek-1.1.1/src/paycek.egg-info/top_level.txt
+-rw-r--r--   0 antun      (501) staff       (20)     7310 2024-05-29 15:29:16.000000 paycek-1.1.1/src/paycek.py
```

### Comparing `paycek-1.1.0/LICENSE` & `paycek-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paycek-1.1.0/PKG-INFO` & `paycek-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paycek
-Version: 1.1.0
+Version: 1.1.1
 Summary: A connector library for communicating with PayCek public API
 Author: Electrocoin d.o.o.
 Project-URL: Website, https://paycek.io
 Project-URL: Source Code, https://github.com/electrocoin-eu/paycek-python
 Project-URL: Bug Tracker, https://github.com/electrocoin-eu/paycek-python/issues
 Keywords: paycek,cryptocurrency,bitcoin,ether,payment,cryptopayment,exchange
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paycek-1.1.0/README.md` & `paycek-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `paycek-1.1.0/pyproject.toml` & `paycek-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "paycek"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name = "Electrocoin d.o.o." }
 ]
 description = "A connector library for communicating with PayCek public API"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `paycek-1.1.0/src/paycek.egg-info/PKG-INFO` & `paycek-1.1.1/src/paycek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paycek
-Version: 1.1.0
+Version: 1.1.1
 Summary: A connector library for communicating with PayCek public API
 Author: Electrocoin d.o.o.
 Project-URL: Website, https://paycek.io
 Project-URL: Source Code, https://github.com/electrocoin-eu/paycek-python
 Project-URL: Bug Tracker, https://github.com/electrocoin-eu/paycek-python/issues
 Keywords: paycek,cryptocurrency,bitcoin,ether,payment,cryptopayment,exchange
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paycek-1.1.0/src/paycek.py` & `paycek-1.1.1/src/paycek.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,21 @@
 		:param headers: callback headers
 		:param endpoint: callback endpoint
 		:param body_bytes: callback body bytes
 		:param http_method: callback http method
 		:param content_type: callback content type
 		:return: True if the generated mac digest is equal to the one received in headers, False otherwise
 		"""
-		headers_lower = {key.lower(): headers[key] for key in headers}
-		generated_mac = self._generate_mac_hash(headers_lower['apikeyauth-nonce'], endpoint, body_bytes, http_method, content_type)
+		try:
+			headers_lower = {key.lower(): headers[key] for key in headers}
+			generated_mac = self._generate_mac_hash(headers_lower['apikeyauth-nonce'], endpoint, body_bytes, http_method, content_type)
 
-		return hmac.compare_digest(generated_mac, headers_lower['apikeyauth-mac'])
+			return hmac.compare_digest(generated_mac, headers_lower['apikeyauth-mac'])
+		except:
+			return False
 
 	def generate_payment_url(self, profile_code: str, dst_amount: str, **optional_fields):
 		"""
 		:param optional_fields: Optional fields:
 			payment_id: string
 			location_id: string
 			items: array
```

