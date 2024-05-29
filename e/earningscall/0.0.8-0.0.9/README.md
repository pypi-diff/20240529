# Comparing `tmp/earningscall-0.0.8.tar.gz` & `tmp/earningscall-0.0.9.tar.gz`

## Comparing `earningscall-0.0.8.tar` & `earningscall-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 earningscall-0.0.8/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 earningscall-0.0.8/DEVELOPMENT.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 earningscall-0.0.8/TODO.md
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 earningscall-0.0.8/requirements-dev.lock
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 earningscall-0.0.8/requirements.lock
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 earningscall-0.0.8/.github/workflows/release.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/__init__.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/api.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/company.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/errors.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/event.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/exports.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/sectors.py
--rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/symbols.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/transcript.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 earningscall-0.0.8/earningscall/utils.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 earningscall-0.0.8/scripts/get_all_company_transcripts.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 earningscall-0.0.8/scripts/get_single_transcript.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 earningscall-0.0.8/scripts/list_all_companies.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/test_earnings_event.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/test_get_transcript.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/test_helper.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/test_simple.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/test_symbols.py
--rw-r--r--   0        0        0    60613 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/data/demo-symbols-v2-alpha.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/data/demo-symbols-v2.yaml
--rw-r--r--   0        0        0    60484 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/data/msft-transcript-response.yaml
--rw-r--r--   0        0        0   264578 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/data/symbols-v2.yaml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/data/symbols.txt
--rw-r--r--   0        0        0   216684 2020-02-02 00:00:00.000000 earningscall-0.0.8/tests/data/symbols.yaml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 earningscall-0.0.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 earningscall-0.0.8/LICENSE
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 earningscall-0.0.8/README.md
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 earningscall-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 earningscall-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 earningscall-0.0.9/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 earningscall-0.0.9/DEVELOPMENT.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 earningscall-0.0.9/TODO.md
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 earningscall-0.0.9/requirements-dev.lock
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 earningscall-0.0.9/requirements.lock
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 earningscall-0.0.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/api.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/company.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/errors.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/event.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/exports.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/sectors.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/symbols.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/transcript.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 earningscall-0.0.9/earningscall/utils.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 earningscall-0.0.9/scripts/get_all_company_transcripts.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 earningscall-0.0.9/scripts/get_single_transcript.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 earningscall-0.0.9/scripts/list_companies.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/test_earnings_event.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/test_get_transcript.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/test_helper.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/test_symbols.py
+-rw-r--r--   0        0        0    60613 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/data/demo-symbols-v2-alpha.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/data/demo-symbols-v2.yaml
+-rw-r--r--   0        0        0    60484 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/data/msft-transcript-response.yaml
+-rw-r--r--   0        0        0   264578 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/data/symbols-v2.yaml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/data/symbols.txt
+-rw-r--r--   0        0        0   216684 2020-02-02 00:00:00.000000 earningscall-0.0.9/tests/data/symbols.yaml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 earningscall-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 earningscall-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 earningscall-0.0.9/README.md
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 earningscall-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 earningscall-0.0.9/PKG-INFO
```

### Comparing `earningscall-0.0.8/DEVELOPMENT.md` & `earningscall-0.0.9/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/requirements-dev.lock` & `earningscall-0.0.9/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/requirements.lock` & `earningscall-0.0.9/requirements.lock`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/.github/workflows/release.yml` & `earningscall-0.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/earningscall/api.py` & `earningscall-0.0.9/earningscall/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import logging
 import os
 from typing import Optional
 
-import earningscall
 import requests
 
+import earningscall
 
 log = logging.getLogger(__file__)
 
 DOMAIN = os.environ.get("ECALL_DOMAIN", "earningscall.biz")
 API_BASE = f"https://v2.api.{DOMAIN}"
 
 
 def get_api_key():
     api_key = earningscall.api_key
     if not api_key:
         return os.environ.get("ECALL_API_KEY", "demo")
     return api_key
 
 
+def api_key_param():
+    return {"apikey": get_api_key()}
+
+
 def is_demo_account():
     return get_api_key() == "demo"
 
 
 def get_events(exchange: str,
                symbol: str):
 
     log.debug(f"get_events exchange: {exchange} symbol: {symbol}")
     params = {
-        "apikey": get_api_key(),
+        **api_key_param(),
         "exchange": exchange,
         "symbol": symbol,
     }
     response = requests.get(f"{API_BASE}/events", params=params)
     if response.status_code != 200:
         return None
     return response.json()
@@ -41,15 +45,15 @@
 def get_transcript(exchange: str,
                    symbol: str,
                    year: int,
                    quarter: int) -> Optional[str]:
 
     log.debug(f"get_transcript year: {year} quarter: {quarter}")
     params = {
-        "apikey": get_api_key(),
+        **api_key_param(),
         "exchange": exchange,
         "symbol": symbol,
         "year": str(year),
         "quarter": str(quarter),
     }
     response = requests.get(f"{API_BASE}/transcript", params=params)
     if response.status_code != 200:
@@ -61,14 +65,18 @@
     response = requests.get(f"{API_BASE}/symbols.txt")
     if response.status_code != 200:
         return None
     return response.text
 
 
 def get_symbols_v2():
-    params = {
-        "apikey": get_api_key(),
-    }
-    response = requests.get(f"{API_BASE}/symbols-v2.txt", params=params)
+    response = requests.get(f"{API_BASE}/symbols-v2.txt", params=api_key_param())
+    if response.status_code != 200:
+        return None
+    return response.text
+
+
+def get_sp500_companies_txt_file():
+    response = requests.get(f"{API_BASE}/symbols/sp500.txt", params=api_key_param())
     if response.status_code != 200:
         return None
     return response.text
```

### Comparing `earningscall-0.0.8/earningscall/company.py` & `earningscall-0.0.9/earningscall/company.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/earningscall/event.py` & `earningscall-0.0.9/earningscall/event.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
-from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Optional
 
+from dataclasses import dataclass, field
 from dataclasses_json import config
 from dataclasses_json import dataclass_json
 from marshmallow import fields
 
 log = logging.getLogger(__file__)
```

### Comparing `earningscall-0.0.8/earningscall/exports.py` & `earningscall-0.0.9/earningscall/exports.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from earningscall.symbols import get_symbols
-
+from earningscall.api import get_sp500_companies_txt_file
 from earningscall.company import Company
+from earningscall.symbols import get_symbols
 
 
 def get_company(symbol: str) -> Optional[Company]:
     company_info = get_symbols().lookup_company(symbol)
     if company_info:
         return Company(company_info=company_info)
     return None
@@ -14,10 +14,14 @@
 
 def get_all_companies() -> [Company]:
     for company_info in get_symbols().get_all():
         yield Company(company_info=company_info)
 
 
 def get_sp500_companies() -> [Company]:
-    ## TODO: Actually only return SP500 companies.
-    for company_info in get_symbols().get_all():
-        yield Company(company_info=company_info)
+    resp = get_sp500_companies_txt_file()
+    if not resp:
+        return []
+    for ticker_symbol in resp.split("\n"):
+        company_info = get_symbols().lookup_company(ticker_symbol)
+        if company_info:
+            yield Company(company_info=company_info)
```

### Comparing `earningscall-0.0.8/earningscall/sectors.py` & `earningscall-0.0.9/earningscall/sectors.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/earningscall/symbols.py` & `earningscall-0.0.9/earningscall/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,16 @@
             try:
                 _symbol = self.get(exchange, symbol.upper())
                 if _symbol:
                     return _symbol
             except KeyError:
                 pass
         if is_demo_account():
-            raise InsufficientApiAccessError(f"For full access, please get an API Key.  See: "
-                                             f"https://earningscall.biz/api-pricing")
+            raise InsufficientApiAccessError(f"\"{symbol}\" requires an API Key for access.  To get your API Key,"
+                                             f" see: https://earningscall.biz/api-pricing")
         return None
 
     def remove_exchange_symbol(self, exchange_symbol: str):
         _symbol = self.by_exchange_and_sym[exchange_symbol]
         del self.by_name[_symbol.name]
         del self.by_exchange_and_sym[exchange_symbol]
```

### Comparing `earningscall-0.0.8/earningscall/utils.py` & `earningscall-0.0.9/earningscall/utils.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/tests/test_earnings_event.py` & `earningscall-0.0.9/tests/test_earnings_event.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/tests/test_get_transcript.py` & `earningscall-0.0.9/tests/test_get_transcript.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/tests/test_symbols.py` & `earningscall-0.0.9/tests/test_symbols.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/tests/data/demo-symbols-v2-alpha.yaml` & `earningscall-0.0.9/tests/data/demo-symbols-v2-alpha.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/tests/data/msft-transcript-response.yaml` & `earningscall-0.0.9/tests/data/msft-transcript-response.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/tests/data/symbols-v2.yaml` & `earningscall-0.0.9/tests/data/symbols-v2.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/tests/data/symbols.yaml` & `earningscall-0.0.9/tests/data/symbols.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/LICENSE` & `earningscall-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.8/README.md` & `earningscall-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 * Python 3.8+ (PyPI supported)
 
 ## Get Transcript for a Single Quarter
 
 ```python
 from earningscall import get_company
 
-
 company = get_company("aapl")  # Lookup Apple, Inc by its ticker symbol, "AAPL"
 
 transcript = company.get_transcript(year=2021, quarter=3)
 print(f"{company} Q3 2021 Transcript Text: \"{transcript.text[:100]}...\"")
 ```
 
 Output
@@ -42,15 +41,14 @@
 
 ## Get All Transcripts for a company
 
 
 ```python
 from earningscall import get_company
 
-
 company = get_company("aapl")  # Lookup Apple, Inc by its ticker symbol, "AAPL"
 
 print(f"Getting all transcripts for: {company}..")
 # Retrieve all earnings conference call events for a company, and iterate through each one
 for event in company.events():
     transcript = company.get_transcript(event=event)  # Fetch the earnings call transcript for this event
     print(f"* Q{event.quarter} {event.year}")
@@ -82,14 +80,23 @@
 
 ```python
 from earningscall import get_all_companies
 
 for company in get_all_companies():
     print(f"{company.company_info} -- {company.company_info.sector} -- {company.company_info.industry}")
 ```
+
+## List S&P 500 Companies
+
+```python
+from earningscall import get_all_companies
+
+for company in get_all_companies():
+    print(f"{company.company_info} -- {company.company_info.sector} -- {company.company_info.industry}")
+```
 
 By default, this library grants you access to only two companies, Apple Inc. and Microsoft, Inc.
 
 To gain access to 5,000+ companies please [signup here](https://earningscall.biz/api-pricing) to get your API key.
 
 Once you have access to your API key, you can set the API Key like this:
```

### Comparing `earningscall-0.0.8/pyproject.toml` & `earningscall-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "earningscall"
-version = "0.0.8"
+version = "0.0.9"
 description = "The EarningsCall Python library."
 readme = "README.md"
 authors = [
     {name = "EarningsCall", email = "dev@earningscall.biz"},
 ]
 requires-python = ">= 3.8"
 dependencies = [
```

### Comparing `earningscall-0.0.8/PKG-INFO` & `earningscall-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: earningscall
-Version: 0.0.8
+Version: 0.0.9
 Summary: The EarningsCall Python library.
 Project-URL: Homepage, https://earningscall.biz
 Project-URL: Documentation, https://github.com/EarningsCall/earningscall-python
 Project-URL: Repository, https://github.com/EarningsCall/earningscall-python
 Project-URL: Issues, https://github.com/EarningsCall/earningscall-python/issues
 Project-URL: Source, https://github.com/EarningsCall/earningscall-python
 Project-URL: Changelog, https://github.com/EarningsCall/earningscall-python/blob/master/CHANGELOG.md
@@ -40,15 +40,14 @@
 * Python 3.8+ (PyPI supported)
 
 ## Get Transcript for a Single Quarter
 
 ```python
 from earningscall import get_company
 
-
 company = get_company("aapl")  # Lookup Apple, Inc by its ticker symbol, "AAPL"
 
 transcript = company.get_transcript(year=2021, quarter=3)
 print(f"{company} Q3 2021 Transcript Text: \"{transcript.text[:100]}...\"")
 ```
 
 Output
@@ -60,15 +59,14 @@
 
 ## Get All Transcripts for a company
 
 
 ```python
 from earningscall import get_company
 
-
 company = get_company("aapl")  # Lookup Apple, Inc by its ticker symbol, "AAPL"
 
 print(f"Getting all transcripts for: {company}..")
 # Retrieve all earnings conference call events for a company, and iterate through each one
 for event in company.events():
     transcript = company.get_transcript(event=event)  # Fetch the earnings call transcript for this event
     print(f"* Q{event.quarter} {event.year}")
@@ -100,14 +98,23 @@
 
 ```python
 from earningscall import get_all_companies
 
 for company in get_all_companies():
     print(f"{company.company_info} -- {company.company_info.sector} -- {company.company_info.industry}")
 ```
+
+## List S&P 500 Companies
+
+```python
+from earningscall import get_all_companies
+
+for company in get_all_companies():
+    print(f"{company.company_info} -- {company.company_info.sector} -- {company.company_info.industry}")
+```
 
 By default, this library grants you access to only two companies, Apple Inc. and Microsoft, Inc.
 
 To gain access to 5,000+ companies please [signup here](https://earningscall.biz/api-pricing) to get your API key.
 
 Once you have access to your API key, you can set the API Key like this:
```

