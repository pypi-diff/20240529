# Comparing `tmp/codal_tsetmc-0.0.8.tar.gz` & `tmp/codal_tsetmc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codal_tsetmc-0.0.8.tar", max compression
+gzip compressed data, was "codal_tsetmc-0.0.9.tar", max compression
```

## Comparing `codal_tsetmc-0.0.8.tar` & `codal_tsetmc-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rwxr-xr-x   0        0        0     1073 2022-08-31 09:49:59.670121 codal_tsetmc-0.0.8/LICENSE
--rwxr-xr-x   0        0        0     3874 2024-05-26 18:07:54.261461 codal_tsetmc-0.0.8/README.md
--rwxr-xr-x   0        0        0      881 2024-05-26 18:21:35.582076 codal_tsetmc-0.0.8/pyproject.toml
--rwxr-xr-x   0        0        0      939 2024-05-26 20:11:40.824220 codal_tsetmc-0.0.8/src/codal_tsetmc/__init__.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:46:33.499975 codal_tsetmc-0.0.8/src/codal_tsetmc/config/__init__.py
--rwxr-xr-x   0        0        0      100 2022-07-29 09:25:17.071258 codal_tsetmc-0.0.8/src/codal_tsetmc/config/config.default.yml
--rwxr-xr-x   0        0        0     2281 2024-05-26 19:38:11.337203 codal_tsetmc-0.0.8/src/codal_tsetmc/config/engine.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:13:27.157561 codal_tsetmc-0.0.8/src/codal_tsetmc/download/__init__.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:20:38.526565 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/__init__.py
--rwxr-xr-x   0        0        0     4071 2024-05-26 16:53:41.440402 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/category.py
--rwxr-xr-x   0        0        0      525 2023-08-30 22:03:38.205743 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/company.py
--rwxr-xr-x   0        0        0     8343 2024-05-26 17:37:07.978458 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/letters.py
--rwxr-xr-x   0        0        0    10242 2024-05-26 17:37:08.468597 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/query.py
--rwxr-xr-x   0        0        0    10615 2024-05-26 17:37:09.202565 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/report.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:17:32.818433 codal_tsetmc-0.0.8/src/codal_tsetmc/download/other/__init__.py
--rwxr-xr-x   0        0        0     4370 2024-05-26 22:40:01.079750 codal_tsetmc-0.0.8/src/codal_tsetmc/download/other/commodity.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:17:20.138410 codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/__init__.py
--rwxr-xr-x   0        0        0     4112 2024-05-26 22:40:00.827227 codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/capital.py
--rwxr-xr-x   0        0        0     6819 2024-05-27 00:19:09.779013 codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/price.py
--rwxr-xr-x   0        0        0     4397 2024-05-26 22:22:20.459155 codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/stock.py
--rwxr-xr-x   0        0        0     1483 2024-05-26 20:13:00.609132 codal_tsetmc-0.0.8/src/codal_tsetmc/initializer.py
--rwxr-xr-x   0        0        0        0 2023-08-30 23:17:18.742542 codal_tsetmc-0.0.8/src/codal_tsetmc/models/__init__.py
--rwxr-xr-x   0        0        0     4550 2024-05-26 18:40:15.029397 codal_tsetmc-0.0.8/src/codal_tsetmc/models/companies.py
--rwxr-xr-x   0        0        0      920 2024-05-26 20:11:41.962655 codal_tsetmc-0.0.8/src/codal_tsetmc/models/create.py
--rwxr-xr-x   0        0        0     7723 2024-05-26 23:55:50.253175 codal_tsetmc-0.0.8/src/codal_tsetmc/models/stocks.py
--rwxr-xr-x   0        0        0        1 2023-08-30 22:12:41.957284 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/__init__.py
--rwxr-xr-x   0        0        0     1781 2024-05-26 21:32:15.445757 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/api.py
--rwxr-xr-x   0        0        0      879 2024-05-26 20:21:43.474048 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/database.py
--rwxr-xr-x   0        0        0      895 2024-05-26 17:37:09.431876 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/exception.py
--rwxr-xr-x   0        0        0     9710 2024-05-26 16:28:57.230356 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/string.py
--rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 codal_tsetmc-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2022-08-31 09:49:59.670121 codal_tsetmc-0.0.9/LICENSE
+-rwxr-xr-x   0        0        0     3874 2024-05-26 18:07:54.261461 codal_tsetmc-0.0.9/README.md
+-rwxr-xr-x   0        0        0      881 2024-05-27 18:48:10.182561 codal_tsetmc-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0      915 2024-05-27 17:49:55.154239 codal_tsetmc-0.0.9/src/codal_tsetmc/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:46:33.499975 codal_tsetmc-0.0.9/src/codal_tsetmc/config/__init__.py
+-rwxr-xr-x   0        0        0      100 2022-07-29 09:25:17.071258 codal_tsetmc-0.0.9/src/codal_tsetmc/config/config.default.yml
+-rwxr-xr-x   0        0        0     2281 2024-05-26 19:38:11.337203 codal_tsetmc-0.0.9/src/codal_tsetmc/config/engine.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:13:27.157561 codal_tsetmc-0.0.9/src/codal_tsetmc/download/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:20:38.526565 codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/__init__.py
+-rwxr-xr-x   0        0        0     4071 2024-05-26 16:53:41.440402 codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/category.py
+-rwxr-xr-x   0        0        0      525 2023-08-30 22:03:38.205743 codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/company.py
+-rwxr-xr-x   0        0        0     8634 2024-05-27 21:40:59.127148 codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/letters.py
+-rwxr-xr-x   0        0        0    10231 2024-05-27 19:45:46.428902 codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/query.py
+-rwxr-xr-x   0        0        0    10615 2024-05-27 15:46:00.168333 codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/report.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:17:32.818433 codal_tsetmc-0.0.9/src/codal_tsetmc/download/other/__init__.py
+-rwxr-xr-x   0        0        0     4370 2024-05-26 22:40:01.079750 codal_tsetmc-0.0.9/src/codal_tsetmc/download/other/commodity.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:17:20.138410 codal_tsetmc-0.0.9/src/codal_tsetmc/download/tsetmc/__init__.py
+-rwxr-xr-x   0        0        0     4112 2024-05-26 22:40:00.827227 codal_tsetmc-0.0.9/src/codal_tsetmc/download/tsetmc/capital.py
+-rwxr-xr-x   0        0        0     6789 2024-05-27 16:03:47.562907 codal_tsetmc-0.0.9/src/codal_tsetmc/download/tsetmc/price.py
+-rwxr-xr-x   0        0        0     4554 2024-05-27 18:18:05.275970 codal_tsetmc-0.0.9/src/codal_tsetmc/download/tsetmc/stock.py
+-rwxr-xr-x   0        0        0     1426 2024-05-27 17:49:54.817047 codal_tsetmc-0.0.9/src/codal_tsetmc/initializer.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 23:17:18.742542 codal_tsetmc-0.0.9/src/codal_tsetmc/models/__init__.py
+-rwxr-xr-x   0        0        0     4550 2024-05-26 18:40:15.029397 codal_tsetmc-0.0.9/src/codal_tsetmc/models/companies.py
+-rwxr-xr-x   0        0        0      920 2024-05-26 20:11:41.962655 codal_tsetmc-0.0.9/src/codal_tsetmc/models/create.py
+-rwxr-xr-x   0        0        0     7857 2024-05-27 15:57:18.165512 codal_tsetmc-0.0.9/src/codal_tsetmc/models/stocks.py
+-rwxr-xr-x   0        0        0        1 2023-08-30 22:12:41.957284 codal_tsetmc-0.0.9/src/codal_tsetmc/tools/__init__.py
+-rwxr-xr-x   0        0        0     1781 2024-05-26 21:32:15.445757 codal_tsetmc-0.0.9/src/codal_tsetmc/tools/api.py
+-rwxr-xr-x   0        0        0      960 2024-05-27 17:03:07.260032 codal_tsetmc-0.0.9/src/codal_tsetmc/tools/database.py
+-rwxr-xr-x   0        0        0      895 2024-05-26 17:37:09.431876 codal_tsetmc-0.0.9/src/codal_tsetmc/tools/exception.py
+-rwxr-xr-x   0        0        0     9710 2024-05-26 16:28:57.230356 codal_tsetmc-0.0.9/src/codal_tsetmc/tools/string.py
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 codal_tsetmc-0.0.9/PKG-INFO
```

### Comparing `codal_tsetmc-0.0.8/LICENSE` & `codal_tsetmc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/README.md` & `codal_tsetmc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/pyproject.toml` & `codal_tsetmc-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codal-tsetmc"
-version = "0.0.8"
+version = "0.0.9"
 description = "Data Downloader for Codal and Tehran stock market"
 authors = ["Mohsen Ebrahimi <mohsenebrahimy.ir@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mohsenebrahimyir.github.io/codal-tsetmc/"
 repository = "https://github.com/mohsenebrahimyir/codal-tsetmc.git"
 packages = [
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/__init__.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import os
 
 from .config.engine import HOME_PATH, CDL_TSE_FOLDER, default_db_path, CONFIG_PATH
 from .models.create import models
-from .tools.database import read_table_by_conditions
+from .tools.database import read_table_by_conditions, read_table_by_sql_query
 from .models.stocks import Stocks
 from .models.companies import Companies
 from .download.codal.query import CodalQuery
 
 from .config import engine as db
 from .initializer import (
+    create_db,
     init_db,
-    init_table,
     fill_db,
     fill_companies_table,
     fill_categories_table,
-    fill_interim_financial_statements_letters,
     fill_stocks_table,
     fill_stocks_prices_table,
     fill_stocks_capitals_table,
     fill_commodities_prices_table,
 )
 
 
@@ -32,9 +31,9 @@
         print(e.__context__)
         return True
     finally:
         pass
 
 
 if db_is_empty():
+    create_db()
     init_db()
-    init_table()
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/config/engine.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/config/engine.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/category.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/category.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/company.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/company.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/letters.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/letters.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,36 +35,36 @@
         "Symbol", "Name",
     ]]
     df = df_col_to_snake_case(df)
 
     return df
 
 
-async def get_letters_urls_from_page_100000_async(ses, url):
+async def get_letters_urls_from_page_100000_async(ses, url: str):
     headers = {
         'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 '
                       'Safari/537.36',
     }
     async with ses.get(url, cookies={}, headers=headers, data="") as response:
         data = await response.json()
 
     u = url.split("100000")
     return [f'{u[0]}{data["Page"] + 1 - i}{u[1]}' for i in range(1, data["Page"] + 1)]
 
 
-async def get_letters_urls_async(urls):
+async def get_letters_urls_async(urls: list):
     tasks = []
     async with aiohttp.ClientSession() as ses:
         for url in urls:
             tasks.append(get_letters_urls_from_page_100000_async(ses, url))
         results = await asyncio.gather(*tasks)
     return results
 
 
-def get_letter_urls_parallel(urls):
+def get_letter_urls_parallel(urls: list):
     if sys.platform == 'win32':
         loop = asyncio.ProactorEventLoop()
         asyncio.set_event_loop(loop)
     else:
         loop = asyncio.get_event_loop()
 
     try:
@@ -82,15 +82,15 @@
         print("import nest_asyncio; nest_asyncio.apply()")
         print("```")
         raise RuntimeError
 
     return results
 
 
-def get_letters_urls_by_symbols(query, symbols, msg=""):
+def get_letters_urls_by_symbols(query: CodalQuery, symbols: list, msg: str = ""):
     print(f"update letters urls ", end="\r")
 
     query.set_page_number(100000)
     urls = []
 
     for symbol in symbols:
         query.set_symbol(symbol)
@@ -98,15 +98,15 @@
 
     results = get_letter_urls_parallel(urls)
     print(msg, end="\r")
 
     return results
 
 
-async def update_letters_for_each_url_async(ses, url):
+async def update_letters_for_each_url_async(ses, url: str):
     try:
         headers = {
             'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 '
                           'Safari/537.36',
         }
         async with ses.get(url, cookies={}, headers=headers, data="") as response:
             data = await response.json()
@@ -116,25 +116,25 @@
 
             return True
 
     except Exception as e:
         return e
 
 
-async def update_letters_for_urls_async(urls):
+async def update_letters_for_urls_async(urls: list):
     tasks = []
     async with aiohttp.ClientSession() as ses:
         for url in urls:
             tasks.append(update_letters_for_each_url_async(ses, url))
         results = await asyncio.gather(*tasks)
 
     return results
 
 
-def update_letter_urls_parallel(urls):
+def update_letter_table_by_urls(urls: list):
     results = None
     if sys.platform == 'win32':
         ##############################################################################
         from functools import wraps
 
         from asyncio.proactor_events import _ProactorBasePipeTransport
 
@@ -154,87 +154,97 @@
         ##############################################################################
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
     loop = asyncio.get_event_loop()
 
     try:
         results = loop.run_until_complete(update_letters_for_urls_async(urls))
+        loop.close()
+        return results
 
     except RuntimeError:
         warning_color = "\033[93m"
         ending_color = "\033[0m"
         print(warning_color, "Please update stock table", ending_color)
         print(
             f"{warning_color}If you are using jupyter notebook, please run following command:{ending_color}"
         )
         print("```")
         print("%pip install nest_asyncio")
         print("import nest_asyncio; nest_asyncio.apply()")
         print("```")
-        raise RuntimeError
-
-    finally:
-        loop.close()
-        return results
+    except Exception as e:
+        print(e.__context__)
 
 
-def update_letters_table_by_symbols(query, symbols, msg=""):
+def update_letters_table_by_query_and_symbols(query: CodalQuery, symbols: list, msg: str = ""):
     print(f"update letters ", end="\r")
     urls_list = get_letters_urls_by_symbols(query, symbols)
 
     letter_urls = []
     for urls in urls_list:
         for url in urls:
             letter_urls += [url]
 
-    results = update_letter_urls_parallel(letter_urls)
+    results = update_letter_table_by_urls(letter_urls)
     print(msg)
     return results
 
 
-def update_companies_group_letters(query, group_code):
+def update_companies_group_letters(query: CodalQuery, group_code: str):
     stocks = session.query(Stocks.symbol).filter_by(group_code=group_code).all()
     print(f"{' ' * 25} group: {group_code}", end="\r")
     symbols = [stock[0] for stock in stocks]
     msg = "group " + group_code + " updated"
-    results = update_letters_table_by_symbols(query, symbols, msg)
+    results = update_letters_table_by_query_and_symbols(query, symbols, msg)
     return results
 
 
-def fill_letters_table(query):
+def fill_letters_table(query: CodalQuery):
     codes = session.query(Stocks.group_code).distinct().all()
     for i, code in enumerate(codes):
         print(f"{' ' * 35} total progress: {100 * (i + 1) / len(codes):.2f}%", end="\r")
         update_companies_group_letters(query, code[0])
 
     print("letters Download Finished.", " " * 50)
 
 
-def fill_interim_financial_statements_letters(from_date="1300/01/01", to_date="1500/01/01"):
+def fill_interim_financial_statements_letters(
+        from_date: str = "1300/01/01",
+        to_date: str = "1500/01/01"
+):
     query = CodalQuery()
     query.set_from_date(from_date)
     query.set_to_date(to_date)
     query.set_category('اطلاعات و صورت مالی سالانه')
     query.set_letter_type('اطلاعات و صورتهای مالی میاندوره ای')
 
     fill_letters_table(query)
 
 
-def fill_symbols_interim_financial_statements_letters(symbols, from_date="1300/01/01", to_date="1500/01/01"):
+def fill_symbols_interim_financial_statements_letters(
+        symbols: list,
+        from_date: str = "1300/01/01",
+        to_date: str = "1500/01/01"
+):
     query = CodalQuery()
     query.set_from_date(from_date)
     query.set_to_date(to_date)
     query.set_category('اطلاعات و صورت مالی سالانه')
     query.set_letter_type('اطلاعات و صورتهای مالی میاندوره ای')
 
-    results = update_letters_table_by_symbols(query, symbols)
+    results = update_letters_table_by_query_and_symbols(query, symbols)
     return results
 
 
-def update_symbol_interim_financial_statements_letters(symbol, from_date="1300/01/01", to_date="1500/01/01"):
+def update_symbol_interim_financial_statements_letters(
+        symbol: str,
+        from_date: str = "1300/01/01",
+        to_date: str = "1500/01/01"
+):
     query = CodalQuery()
     query.set_to_date(to_date)
     query.set_category('اطلاعات و صورت مالی سالانه')
     query.set_letter_type('اطلاعات و صورتهای مالی میاندوره ای')
 
     q = (
         f"SELECT max(publish_date_time) AS date FROM letters WHERE symbol = '{symbol}' "
@@ -248,9 +258,9 @@
         last_date = num_to_datetime(max_date.date.iat[0], datetime=False)
 
         if last_date > from_date:
             query.set_from_date(last_date)
         else:
             query.set_from_date(from_date)
 
-    results = update_letters_table_by_symbols(query, [symbol])
+    results = update_letters_table_by_query_and_symbols(query, [symbol])
     return results
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/query.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
             letters += self.get_api_single_page()
         
         letters += last_letters
 
         return letters
 
     # گرفتن اطلاعات کلی تمام صفحات به صورت یک فرمت داده
-    def get_letters(self, pages: int = 0, show=False) -> pd.DataFrame:
+    def get_letters(self, pages: int = 0, show=False) -> None | pd.DataFrame:
         letters = self.get_api_multi_page(pages)
         df = pd.DataFrame(letters).replace(regex=FA_TO_EN_DIGITS)
         df["LetterSerial"] = df["Url"].replace(regex={
             r"^.*LetterSerial=": "",
             r"\&.*$": ""
         })
         df["LetterTypes"] = df["LetterCode"].replace(regex=LETTERS_CODE_TO_TITLE)
@@ -266,11 +266,10 @@
         df["CompanySymbol"] = df["Symbol"]
         df = df[[
             "PublishDateTime", "SentDateTime", "TracingNo",
             "LetterSerial", "LetterCode", "LetterTypes", "LetterTitle",
             "CompanySymbol", "CompanyName",
         ]]
         df = df_col_to_snake_case(df)
+        self.letters = df
         if show:
             return df
-        else:
-            self.letters = df
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/report.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/codal/report.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,28 @@
     datetime_to_num,
     replace_all,
 )
 from codal_tsetmc.tools.database import fill_table_of_db_with_df
 from codal_tsetmc.models.companies import Letters
 
 
+TABLES_WHIT_SINGLE_ITEM = [
+    "Balance Sheet",
+    "Income Statement",
+    "Cash Flow",
+    "Sales trend and cost over the last 5 years",
+    "The cost of the sold goods",
+    "Staff status",
+    "Other operating income",
+    "Other operating expenses",
+    "Non-operation income and expenses investment income",
+    "Non-operation income and expenses miscellaneous items"
+]
+
+
 def extract_sheet_id(sheet: str) -> str:
     if sheet in SHEET_NAME_TO_ID.keys():
         return f"&sheetId={SHEET_NAME_TO_ID[sheet]}"
     elif sheet in SHEET_NAME_TO_ID.values():
         return f"&sheetId={sheet}"
     else:
         return ""
@@ -248,28 +262,14 @@
     df["table_title_en"] = table["title_en"]
     df["table_title_fa"] = table["title_fa"]
     df["description"] = table["description"]
     df["alias_name"] = table["alias_name"]
     return df
 
 
-TABLES_WHIT_SINGLE_ITEM = [
-    "Balance Sheet",
-    "Income Statement",
-    "Cash Flow",
-    "Sales trend and cost over the last 5 years",
-    "The cost of the sold goods",
-    "Staff status",
-    "Other operating income",
-    "Other operating expenses",
-    "Non-operation income and expenses investment income",
-    "Non-operation income and expenses miscellaneous items"
-]
-
-
 def update_financial_statement_table(datasource, sheet, table):
     sheet = edit_sheet_detail(sheet)
     table = edit_table_detail(table)
     if table["title_en"] in TABLES_WHIT_SINGLE_ITEM:
         df = extract_table_with_single_item(table)
         db_table = "financial_statement_table_with_single_item"
         df = add_sheet_and_table_detail(df, datasource, sheet, table)
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/other/commodity.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/other/commodity.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/capital.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/tsetmc/capital.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/price.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/tsetmc/price.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
 
 def cleanup_stock_prices_records(data):
     df = pd.read_csv(io.StringIO(data), delimiter="@", lineterminator=";", engine="c", header=None)
     df.columns = "date high low price close open yesterday value volume count".split()
     df["date"] = df["date"].apply(lambda x: datetime.strptime(str(x), "%Y%m%d"))
     df["date"] = df["date"].jalali.to_jalali().apply(lambda x: x.strftime('%Y%m%d000000'))
-    df["price"] = df["close"]
     df = df.sort_values("date")
 
     return df[["date", "volume", "value", "price"]]
 
 
 def get_stock_prices_history(code: str) -> pd.DataFrame:
     url = f"http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={code}&Top=999999&A=0"
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/stock.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/download/tsetmc/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,22 @@
         print(e.__context__)
         session.rollback()
 
 
 async def update_stock_table(code: str) -> tuple[bool, str] | tuple[Exception, str]:
     try:
         stock = Stocks.query.filter_by(code=code).first()
-        if stock.code == code:
-            print(f"stock with code {code} exist")
-            return True, code
+        try:
+            if stock.code is not None:
+                if stock.code == code:
+                    print(f"stock with code {code} exist")
+                    return True, code
+        except Exception as e:
+            print(e.__context__)
+            pass
 
         url = f"http://cdn.tsetmc.com/api/Instrument/GetInstrumentInfo/{code}"
         headers = {
             'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 '
                           'Safari/537.36'
         }
         async with aiohttp.ClientSession() as ses:
@@ -107,15 +112,15 @@
 
 def get_stocks_groups(timeout=10):
     url = "http://old.tsetmc.com/Loader.aspx?ParTree=111C1213"
     r = requests.get(url, timeout=timeout)
     return re.findall(r"\d{2}", r.text)
 
 
-def fill_stocks_table(timeout=10, repeat=30):
+def fill_stocks_table(timeout=10, repeat=15):
     print("This may take several minutes")
     index = ["32097828799138957"]
     bonds = get_csv_from_github("treasury_bill")
     update_stocks_table(index + list(bonds.code))
     for i in range(repeat):
         print(f"Downloading group ids... series: {i + 1}")
         ids = get_stock_ids(timeout=timeout)
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/initializer.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/initializer.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,43 +4,42 @@
 from .models.create import create
 from .download.codal.company import fill_companies_table
 from .download.codal.category import fill_categories_table
 from .download.tsetmc.stock import fill_stocks_table
 from .download.tsetmc.price import fill_stocks_prices_table
 from .download.tsetmc.capital import fill_stocks_capitals_table
 from .download.other.commodity import fill_commodities_prices_table
-from .download.codal.letters import fill_interim_financial_statements_letters
 
 
-def init_db():
+def create_db():
     print("creating database")
     path = os.path.join(HOME_PATH, CDL_TSE_FOLDER)
     try:
         os.mkdir(path)
         print("making package folder...")
         print("Includes: config.yml and companies-stocks.db  if you are using sqlite.")
         print("you can change config.yml to your needs.")
     except FileExistsError:
         print("folder already exists")
     create()
     print(f"Database created in: {path}")
 
 
-def init_table():
+def init_db():
+    print("downloading company and stock info from CODAL and TSETMC")
     fill_companies_table()
     fill_categories_table()
+    fill_stocks_table()
 
 
 def fill_db():
     print("downloading company and stock details from CODAL and TSETMC")
     print("may take few minutes")
-    fill_stocks_table()
     fill_stocks_prices_table()
     fill_stocks_capitals_table()
     fill_commodities_prices_table()
-    fill_interim_financial_statements_letters()
     print("For more info go to:")
     print("https://github.com/mohsenebrahimyir/codal-tsetmc")
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/models/companies.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/models/companies.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/models/create.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/models/create.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/models/stocks.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/models/stocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             return self._price
 
         df["jdate"] = df["date"].replace(regex={"000000$": ""})
         df["date"] = df["date"].jalali.parse_jalali("%Y%m%d%H%M%S").jalali.to_gregorian()
         df.set_index("date", inplace=True)
         self._price_cached = True
         self._price = df[[
-            "jdate", "ticker", "symbol", "code", "price", "value", "volume"
+            "jdate", "symbol", "code", "price", "value", "volume"
         ]].dropna()
 
         return self._price
 
     @property
     def market(self) -> pd.DataFrame:
         """dataframe of stock price with date and OHLC"""
@@ -177,18 +177,18 @@
 
         try:
             return update_stocks_capitals([self.code])
         except:
             return False
 
     def __repr__(self):
-        return f"{self.symbol}-{self.name}-{self.group_name}"
+        return f"symbol: {self.symbol}, code: {self.code}, name: {self.name}, group: {self.group_name}"
 
     def __str__(self):
-        return self.name
+        return f"symbol: {self.symbol}, code: {self.code}, name: {self.name}, group: {self.group_name}"
 
     @staticmethod
     def get_group():
         return (
             session.query(Stocks.group_code, Stocks.group_name)
             .group_by(Stocks.group_code)
             .all()
@@ -204,15 +204,15 @@
     date = Column(String)
     volume = Column(BIGINT)
     value = Column(BIGINT)
     price = Column(Float)
     up_date = Column(String)
 
     def __repr__(self):
-        return f"({self.stock.name}, {self.date}, {self.close:.0f})"
+        return f"(symbol: {self.symbol}, instrument: {self.stock.name}, code: {self.code})"
 
 
 class StockCapital(Base):
     __tablename__ = "stock_capital"
 
     id = Column(Integer, primary_key=True)
     code = Column(String, ForeignKey("stocks.code"), index=True)
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/tools/api.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/tools/api.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/tools/database.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/tools/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,7 +28,11 @@
     if conditions != "":
         query = f"{query} WHERE {conditions}"
     
     if variable != "" and value != "":
         query = f"{query} WHERE {variable} = '{value}'"
 
     return pd.read_sql(query, engine)
+
+
+def read_table_by_sql_query(query: str):
+    return pd.read_sql(query, engine)
```

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/tools/exception.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/tools/exception.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/src/codal_tsetmc/tools/string.py` & `codal_tsetmc-0.0.9/src/codal_tsetmc/tools/string.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.8/PKG-INFO` & `codal_tsetmc-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codal-tsetmc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Data Downloader for Codal and Tehran stock market
 Home-page: https://mohsenebrahimyir.github.io/codal-tsetmc/
 License: MIT
 Author: Mohsen Ebrahimi
 Author-email: mohsenebrahimy.ir@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

