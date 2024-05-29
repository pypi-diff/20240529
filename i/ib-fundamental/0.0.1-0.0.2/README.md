# Comparing `tmp/ib_fundamental-0.0.1.tar.gz` & `tmp/ib_fundamental-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ib_fundamental-0.0.1.tar", last modified: Mon May 27 18:22:32 2024, max compression
+gzip compressed data, was "ib_fundamental-0.0.2.tar", last modified: Wed May 29 15:56:57 2024, max compression
```

## Comparing `ib_fundamental-0.0.1.tar` & `ib_fundamental-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:22:32.740058 ib_fundamental-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22502 2024-05-27 18:22:32.740058 ib_fundamental-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:22:32.736058 ib_fundamental-0.0.1/ib_fundamental/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/ib_fundamental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/ib_fundamental/fundamental.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/ib_fundamental/ib_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/ib_fundamental/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/ib_fundamental/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/ib_fundamental/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/ib_fundamental/xml_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:22:32.736058 ib_fundamental-0.0.1/ib_fundamental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22502 2024-05-27 18:22:32.000000 ib_fundamental-0.0.1/ib_fundamental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-27 18:22:32.000000 ib_fundamental-0.0.1/ib_fundamental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:22:32.000000 ib_fundamental-0.0.1/ib_fundamental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 18:22:32.000000 ib_fundamental-0.0.1/ib_fundamental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 18:22:32.000000 ib_fundamental-0.0.1/ib_fundamental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-27 18:22:27.000000 ib_fundamental-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 18:22:32.740058 ib_fundamental-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:56:57.640407 ib_fundamental-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26633 2024-05-29 15:56:57.640407 ib_fundamental-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:56:57.636407 ib_fundamental-0.0.2/ib_fundamental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/ib_fundamental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/ib_fundamental/fundamental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/ib_fundamental/ib_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/ib_fundamental/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/ib_fundamental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/ib_fundamental/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/ib_fundamental/xml_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:56:57.636407 ib_fundamental-0.0.2/ib_fundamental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26633 2024-05-29 15:56:57.000000 ib_fundamental-0.0.2/ib_fundamental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-29 15:56:57.000000 ib_fundamental-0.0.2/ib_fundamental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:56:57.000000 ib_fundamental-0.0.2/ib_fundamental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 15:56:57.000000 ib_fundamental-0.0.2/ib_fundamental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 15:56:57.000000 ib_fundamental-0.0.2/ib_fundamental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-29 15:56:52.000000 ib_fundamental-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:56:57.640407 ib_fundamental-0.0.2/setup.cfg
```

### Comparing `ib_fundamental-0.0.1/LICENSE.txt` & `ib_fundamental-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ib_fundamental-0.0.1/PKG-INFO` & `ib_fundamental-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib_fundamental
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interactive Brokers Fundamental data for humans
 Author: gnzsnz
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -222,19 +222,20 @@
 Requires-Dist: pylint>=3.1.1; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: pre-commit>=3.7.1; extra == "dev"
 Requires-Dist: pandas-stubs>=2.2.1.240316; extra == "dev"
 Requires-Dist: bandit[toml]>=1.7.8; extra == "dev"
 Requires-Dist: flake8>=7.0.0; extra == "dev"
+Requires-Dist: flake8-pytest-style>=2.0.0; extra == "dev"
 Requires-Dist: pytest>=8.2.1; extra == "dev"
 Requires-Dist: pytest-env>=1.1.3; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: pylint-pytest>=1.1.7; extra == "dev"
-Requires-Dist: flake8-pytest-style>=2.0.0; extra == "dev"
+Requires-Dist: tox>=4.0.0; extra == "dev"
 
 # IB Fundamental
 
 Interactive Brokers Fundamental data for humans.
 
 This package will bring all fundamental data available through IBKR TWS API
 into ready-to-use pandas data frames.
@@ -269,15 +270,15 @@
 ticker               AAPL
 company_name    Apple Inc
 cik            0000320193
 exchange_code        NASD
 exchange           NASDAQ
 irs             942404110
 
-# Income statement, aapl.income_quarter will pull the quarterly report
+# Annual income statement, while aapl.income_quarter will pull the quarterly report
 aapl.income_annual
 
                                        map_item  2018-09-29  2019-09-28  2020-09-26  2021-09-25  2022-09-24  2023-09-30    statement_type
 line_id
 0                                        period      Annual      Annual      Annual      Annual      Annual      Annual  Income Statement
 1                                      end_date  2018-09-29  2019-09-28  2020-09-26  2021-09-25  2022-09-24  2023-09-30  Income Statement
 2                                   fiscal_year        2018        2019        2020        2021        2022        2023  Income Statement
@@ -303,15 +304,15 @@
 1530                         Diluted Net Income     59531.0     55256.0     57411.0     94680.0     99803.0     96995.0  Income Statement
 1540            Diluted Weighted Average Shares   20000.436   18595.652   17528.214   16864.919   16325.819   15812.547  Income Statement
 1550       Diluted EPS Excluding ExtraOrd Items     3.05148     2.97145     3.27535     5.61402      6.1132     6.13405  Income Statement
 1570           DPS - Common Stock Primary Issue        0.68        0.75       0.795        0.85         0.9        0.94  Income Statement
 1770                     Diluted Normalized EPS     3.05148     2.97145     3.27535     5.61402      6.1132     6.13405  Income Statement
 
 # get earnings per share, appl.eps_ttm will pull trailing twelve months eps
-aapl.eps_q
+aapl.eps_ttm
 
            report_type period     eps
 as_of_date
 2017-06-30         TTM    12M   8.870
 2017-09-30         TTM    12M   9.270
 2017-12-31         TTM    12M   9.810
 2018-03-31         TTM    12M  10.460
@@ -336,14 +337,22 @@
 2022-12-31         TTM    12M   5.930
 2023-03-31         TTM    12M   5.920
 2023-06-30         TTM    12M   5.980
 2023-09-30         TTM    12M   6.160
 2023-12-31         TTM    12M   6.460
 2024-03-31         TTM    12M   6.460
 
+# get data in json format
+
+from ib_fundamental.utils import to_json
+
+# CompanyFinancials.data property contains all data in dataclass format
+to_json(aapl.data.eps_ttm)
+'[{"as_of_date": "2024-03-31T00:00:00", "report_type": "TTM", "period": "12M", "eps": 6.46}, {"as_of_date": "2023-12-31T00:00:00", "report_type": "TTM", "period": "12M", "eps": 6.46}, ...'
+
 # and much more
 ```
 
 ## What fundamental data is available?
 
 `ib_fundamental` is a wrapper around IBKR TWS API. It will connect to a running TWS or
 ibgateway instance and request fundamental data through
@@ -386,16 +395,17 @@
 - income_annual
 - income_quarter
 - ownership
 - ratios
 - revenue_q
 - revenue_tt
 
-You can use `FundamentalData` class that will return company
-fundamental information in `dataclass` format
+You can use `FundamentalData` class that will return company fundamental
+information in `dataclass` format. Each instance of `CompanyFinancials`
+contains an instance of `FundamentalData` in its `data` property.
 
 ```python
 from ib_fundamental.fundamental import FundamentalData
 
 [_m for _m in dir(FundamentalData) if _m[:1] != "_"]
 
 ['analyst_forecast',
@@ -416,12 +426,61 @@
  'income_annual',
  'income_quarter',
  'ownership_report',
  'ratios',
  'revenue_q',
  'revenue_ttm']
 
+# get quarterly revenue
+aapl.data.revenue_q
+
+[Revenue(as_of_date=datetime.datetime(2024, 3, 31, 0, 0), report_type='R', period='3M', revenue=90753000000.0),
+ Revenue(as_of_date=datetime.datetime(2023, 12, 31, 0, 0), report_type='R', period='3M', revenue=119575000000.0),
+ Revenue(as_of_date=datetime.datetime(2023, 9, 30, 0, 0), report_type='R', period='3M', revenue=89498000000.0),
+ Revenue(as_of_date=datetime.datetime(2023, 6, 30, 0, 0), report_type='R', period='3M', revenue=81797000000.0),
+ Revenue(as_of_date=datetime.datetime(2023, 3, 31, 0, 0), report_type='R', period='3M', revenue=94836000000.0),
+ Revenue(as_of_date=datetime.datetime(2022, 12, 31, 0, 0), report_type='R', period='3M', revenue=117154000000.0),
+ Revenue(as_of_date=datetime.datetime(2022, 9, 30, 0, 0), report_type='R', period='3M', revenue=90146000000.0),
+ Revenue(as_of_date=datetime.datetime(2022, 6, 30, 0, 0), report_type='R', period='3M', revenue=82959000000.0),
+ Revenue(as_of_date=datetime.datetime(2022, 3, 31, 0, 0), report_type='R', period='3M', revenue=97278000000.0),
+ Revenue(as_of_date=datetime.datetime(2021, 12, 31, 0, 0), report_type='R', period='3M', revenue=123945000000.0),
+ Revenue(as_of_date=datetime.datetime(2021, 9, 30, 0, 0), report_type='R', period='3M', revenue=83360000000.0),
+ Revenue(as_of_date=datetime.datetime(2021, 6, 30, 0, 0), report_type='R', period='3M', revenue=81434000000.0),
+ Revenue(as_of_date=datetime.datetime(2021, 3, 31, 0, 0), report_type='R', period='3M', revenue=89584000000.0),
+ Revenue(as_of_date=datetime.datetime(2020, 12, 31, 0, 0), report_type='R', period='3M', revenue=111439000000.0),
+ Revenue(as_of_date=datetime.datetime(2020, 9, 30, 0, 0), report_type='R', period='3M', revenue=64698000000.0),
+ Revenue(as_of_date=datetime.datetime(2020, 6, 30, 0, 0), report_type='R', period='3M', revenue=59685000000.0),
+ Revenue(as_of_date=datetime.datetime(2020, 3, 31, 0, 0), report_type='R', period='3M', revenue=58313000000.0),
+ Revenue(as_of_date=datetime.datetime(2019, 12, 31, 0, 0), report_type='R', period='3M', revenue=91819000000.0),
+ Revenue(as_of_date=datetime.datetime(2019, 9, 30, 0, 0), report_type='R', period='3M', revenue=64040000000.0),
+ Revenue(as_of_date=datetime.datetime(2019, 6, 30, 0, 0), report_type='R', period='3M', revenue=53809000000.0),
+ Revenue(as_of_date=datetime.datetime(2019, 3, 31, 0, 0), report_type='R', period='3M', revenue=58015000000.0),
+ Revenue(as_of_date=datetime.datetime(2018, 12, 31, 0, 0), report_type='R', period='3M', revenue=84310000000.0),
+ Revenue(as_of_date=datetime.datetime(2018, 9, 30, 0, 0), report_type='R', period='3M', revenue=62900000000.0),
+ Revenue(as_of_date=datetime.datetime(2018, 6, 30, 0, 0), report_type='R', period='3M', revenue=53265000000.0),
+ Revenue(as_of_date=datetime.datetime(2018, 3, 31, 0, 0), report_type='R', period='3M', revenue=61137000000.0),
+ Revenue(as_of_date=datetime.datetime(2017, 12, 31, 0, 0), report_type='R', period='3M', revenue=88293000000.0),
+ Revenue(as_of_date=datetime.datetime(2017, 9, 30, 0, 0), report_type='R', period='3M', revenue=52579000000.0),
+ Revenue(as_of_date=datetime.datetime(2017, 6, 30, 0, 0), report_type='R', period='3M', revenue=45408000000.0)]
+
 ````
 
+## Contributing
+
+If you find a bug please open an issue, pull requests are always welcome.
+
+To develop with `ib_fundamental` please follow these steps
+
+```bash
+git clone https://github.com/quantbelt/ib_fundamental.git
+cd ib_fundamental
+# install development dependencies
+pip install .[dev]
+# do your things
+# run linters and code quality checks
+pre-commit
+# run tests with tox, requires pypy310,py{310,311,312}
+tox
+```
 
 [reqFundamental]: https://ib-api-reloaded.github.io/ib_async/api.html#ib_async.ib.IB.reqFundamentalData
 [fin_ratios]: http://web.archive.org/web/20200725010343/https://interactivebrokers.github.io/tws-api/fundamental_ratios_tags.html
```

### Comparing `ib_fundamental-0.0.1/ib_fundamental/fundamental.py` & `ib_fundamental-0.0.2/ib_fundamental/fundamental.py`

 * *Files identical despite different names*

### Comparing `ib_fundamental-0.0.1/ib_fundamental/ib_client.py` & `ib_fundamental-0.0.2/ib_fundamental/ib_client.py`

 * *Files identical despite different names*

### Comparing `ib_fundamental-0.0.1/ib_fundamental/objects.py` & `ib_fundamental-0.0.2/ib_fundamental/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,24 +253,26 @@
 @dataclass
 class Revenue:
     """Revenue"""
 
     as_of_date: datetime
     report_type: str
     period: str
+    currency: str
     revenue: float
 
 
 @dataclass
 class EarningsPerShare:
     """Earnings per share"""
 
     as_of_date: datetime
     report_type: str
     period: str
+    currency: str
     eps: float
 
 
 @dataclass
 class AnalystForecast:
     """Analyst Forecast"""
```

### Comparing `ib_fundamental-0.0.1/ib_fundamental/utils.py` & `ib_fundamental-0.0.2/ib_fundamental/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """
-Created on Thu May 9 18:21:58 2021
-
-@author: gnzsnz
+ib_fundamental utility functions
 """
 
+import dataclasses
+import datetime
+import json
 import re
 from typing import Any, Optional
 
+from ib_async import FundamentalRatios
 from pandas import DataFrame
 
 re_pattern = re.compile(r"(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])")
 
 
 def to_dataframe(table: Any, key: Optional[str] = None) -> DataFrame:
     """converts a list of dicts to a data frame
@@ -44,7 +46,26 @@
     return df
 
 
 def camel_to_snake(camel: str) -> str:
     """Convert CamelCase to snake_case"""
     # https://stackoverflow.com/questions/1175208/elegant-python-function-to-convert-camelcase-to-snake-case
     return re_pattern.sub("_", camel).lower()
+
+
+def to_json(obj: Any, **kwargs: Any) -> str:
+    """Convert FundamentalData attributes to JSON"""
+
+    class EnhancedJSONEncoder(json.JSONEncoder):
+        """JSON encoder for dataclasses and datetime"""
+
+        def default(self, o):
+            if dataclasses.is_dataclass(o):
+                return dataclasses.asdict(o)
+            elif isinstance(o, (datetime.date, datetime.datetime)):
+                return o.isoformat()
+            elif isinstance(o, FundamentalRatios):
+                return vars(o)
+
+            return super().default(o)
+
+    return json.dumps(obj, cls=EnhancedJSONEncoder, **kwargs)
```

### Comparing `ib_fundamental-0.0.1/ib_fundamental/xml_parser.py` & `ib_fundamental-0.0.2/ib_fundamental/xml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,19 +260,22 @@
         self,
         report_type: SummaryReportType = None,
         period: SummaryPeriod = None,
     ) -> list[Revenue]:
         """Revenue"""
         fa = "./TotalRevenues"
         fs = self.xml_report.fin_summary.find(fa)
+        curr = fs.attrib["currency"]
+
         _revenue = [
             Revenue(
                 as_of_date=fromisoformat(tr.attrib["asofDate"]),
                 report_type=tr.attrib["reportType"],
                 period=tr.attrib["period"],
+                currency=curr,
                 revenue=float(tr.text),
             )
             for tr in fs
             if (
                 report_type is None
                 or (report_type is not None and tr.attrib["reportType"] == report_type)
             )
@@ -286,19 +289,22 @@
         self,
         report_type: SummaryReportType = None,
         period: SummaryPeriod = None,
     ) -> list[EarningsPerShare]:
         """Earnings per share"""
         fa = "./EPSs"
         fs = self.xml_report.fin_summary.find(fa)
+        curr = fs.attrib["currency"]
+
         _eps = [
             EarningsPerShare(
                 as_of_date=fromisoformat(tr.attrib["asofDate"]),
                 report_type=tr.attrib["reportType"],
                 period=tr.attrib["period"],
+                currency=curr,
                 eps=float(tr.text),
             )
             for tr in fs
             if (
                 report_type is None
                 or (report_type is not None and tr.attrib["reportType"] == report_type)
             )
```

### Comparing `ib_fundamental-0.0.1/ib_fundamental/xml_report.py` & `ib_fundamental-0.0.2/ib_fundamental/xml_report.py`

 * *Files identical despite different names*

### Comparing `ib_fundamental-0.0.1/ib_fundamental.egg-info/PKG-INFO` & `ib_fundamental-0.0.2/ib_fundamental.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib_fundamental
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interactive Brokers Fundamental data for humans
 Author: gnzsnz
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -222,19 +222,20 @@
 Requires-Dist: pylint>=3.1.1; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: pre-commit>=3.7.1; extra == "dev"
 Requires-Dist: pandas-stubs>=2.2.1.240316; extra == "dev"
 Requires-Dist: bandit[toml]>=1.7.8; extra == "dev"
 Requires-Dist: flake8>=7.0.0; extra == "dev"
+Requires-Dist: flake8-pytest-style>=2.0.0; extra == "dev"
 Requires-Dist: pytest>=8.2.1; extra == "dev"
 Requires-Dist: pytest-env>=1.1.3; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: pylint-pytest>=1.1.7; extra == "dev"
-Requires-Dist: flake8-pytest-style>=2.0.0; extra == "dev"
+Requires-Dist: tox>=4.0.0; extra == "dev"
 
 # IB Fundamental
 
 Interactive Brokers Fundamental data for humans.
 
 This package will bring all fundamental data available through IBKR TWS API
 into ready-to-use pandas data frames.
@@ -269,15 +270,15 @@
 ticker               AAPL
 company_name    Apple Inc
 cik            0000320193
 exchange_code        NASD
 exchange           NASDAQ
 irs             942404110
 
-# Income statement, aapl.income_quarter will pull the quarterly report
+# Annual income statement, while aapl.income_quarter will pull the quarterly report
 aapl.income_annual
 
                                        map_item  2018-09-29  2019-09-28  2020-09-26  2021-09-25  2022-09-24  2023-09-30    statement_type
 line_id
 0                                        period      Annual      Annual      Annual      Annual      Annual      Annual  Income Statement
 1                                      end_date  2018-09-29  2019-09-28  2020-09-26  2021-09-25  2022-09-24  2023-09-30  Income Statement
 2                                   fiscal_year        2018        2019        2020        2021        2022        2023  Income Statement
@@ -303,15 +304,15 @@
 1530                         Diluted Net Income     59531.0     55256.0     57411.0     94680.0     99803.0     96995.0  Income Statement
 1540            Diluted Weighted Average Shares   20000.436   18595.652   17528.214   16864.919   16325.819   15812.547  Income Statement
 1550       Diluted EPS Excluding ExtraOrd Items     3.05148     2.97145     3.27535     5.61402      6.1132     6.13405  Income Statement
 1570           DPS - Common Stock Primary Issue        0.68        0.75       0.795        0.85         0.9        0.94  Income Statement
 1770                     Diluted Normalized EPS     3.05148     2.97145     3.27535     5.61402      6.1132     6.13405  Income Statement
 
 # get earnings per share, appl.eps_ttm will pull trailing twelve months eps
-aapl.eps_q
+aapl.eps_ttm
 
            report_type period     eps
 as_of_date
 2017-06-30         TTM    12M   8.870
 2017-09-30         TTM    12M   9.270
 2017-12-31         TTM    12M   9.810
 2018-03-31         TTM    12M  10.460
@@ -336,14 +337,22 @@
 2022-12-31         TTM    12M   5.930
 2023-03-31         TTM    12M   5.920
 2023-06-30         TTM    12M   5.980
 2023-09-30         TTM    12M   6.160
 2023-12-31         TTM    12M   6.460
 2024-03-31         TTM    12M   6.460
 
+# get data in json format
+
+from ib_fundamental.utils import to_json
+
+# CompanyFinancials.data property contains all data in dataclass format
+to_json(aapl.data.eps_ttm)
+'[{"as_of_date": "2024-03-31T00:00:00", "report_type": "TTM", "period": "12M", "eps": 6.46}, {"as_of_date": "2023-12-31T00:00:00", "report_type": "TTM", "period": "12M", "eps": 6.46}, ...'
+
 # and much more
 ```
 
 ## What fundamental data is available?
 
 `ib_fundamental` is a wrapper around IBKR TWS API. It will connect to a running TWS or
 ibgateway instance and request fundamental data through
@@ -386,16 +395,17 @@
 - income_annual
 - income_quarter
 - ownership
 - ratios
 - revenue_q
 - revenue_tt
 
-You can use `FundamentalData` class that will return company
-fundamental information in `dataclass` format
+You can use `FundamentalData` class that will return company fundamental
+information in `dataclass` format. Each instance of `CompanyFinancials`
+contains an instance of `FundamentalData` in its `data` property.
 
 ```python
 from ib_fundamental.fundamental import FundamentalData
 
 [_m for _m in dir(FundamentalData) if _m[:1] != "_"]
 
 ['analyst_forecast',
@@ -416,12 +426,61 @@
  'income_annual',
  'income_quarter',
  'ownership_report',
  'ratios',
  'revenue_q',
  'revenue_ttm']
 
+# get quarterly revenue
+aapl.data.revenue_q
+
+[Revenue(as_of_date=datetime.datetime(2024, 3, 31, 0, 0), report_type='R', period='3M', revenue=90753000000.0),
+ Revenue(as_of_date=datetime.datetime(2023, 12, 31, 0, 0), report_type='R', period='3M', revenue=119575000000.0),
+ Revenue(as_of_date=datetime.datetime(2023, 9, 30, 0, 0), report_type='R', period='3M', revenue=89498000000.0),
+ Revenue(as_of_date=datetime.datetime(2023, 6, 30, 0, 0), report_type='R', period='3M', revenue=81797000000.0),
+ Revenue(as_of_date=datetime.datetime(2023, 3, 31, 0, 0), report_type='R', period='3M', revenue=94836000000.0),
+ Revenue(as_of_date=datetime.datetime(2022, 12, 31, 0, 0), report_type='R', period='3M', revenue=117154000000.0),
+ Revenue(as_of_date=datetime.datetime(2022, 9, 30, 0, 0), report_type='R', period='3M', revenue=90146000000.0),
+ Revenue(as_of_date=datetime.datetime(2022, 6, 30, 0, 0), report_type='R', period='3M', revenue=82959000000.0),
+ Revenue(as_of_date=datetime.datetime(2022, 3, 31, 0, 0), report_type='R', period='3M', revenue=97278000000.0),
+ Revenue(as_of_date=datetime.datetime(2021, 12, 31, 0, 0), report_type='R', period='3M', revenue=123945000000.0),
+ Revenue(as_of_date=datetime.datetime(2021, 9, 30, 0, 0), report_type='R', period='3M', revenue=83360000000.0),
+ Revenue(as_of_date=datetime.datetime(2021, 6, 30, 0, 0), report_type='R', period='3M', revenue=81434000000.0),
+ Revenue(as_of_date=datetime.datetime(2021, 3, 31, 0, 0), report_type='R', period='3M', revenue=89584000000.0),
+ Revenue(as_of_date=datetime.datetime(2020, 12, 31, 0, 0), report_type='R', period='3M', revenue=111439000000.0),
+ Revenue(as_of_date=datetime.datetime(2020, 9, 30, 0, 0), report_type='R', period='3M', revenue=64698000000.0),
+ Revenue(as_of_date=datetime.datetime(2020, 6, 30, 0, 0), report_type='R', period='3M', revenue=59685000000.0),
+ Revenue(as_of_date=datetime.datetime(2020, 3, 31, 0, 0), report_type='R', period='3M', revenue=58313000000.0),
+ Revenue(as_of_date=datetime.datetime(2019, 12, 31, 0, 0), report_type='R', period='3M', revenue=91819000000.0),
+ Revenue(as_of_date=datetime.datetime(2019, 9, 30, 0, 0), report_type='R', period='3M', revenue=64040000000.0),
+ Revenue(as_of_date=datetime.datetime(2019, 6, 30, 0, 0), report_type='R', period='3M', revenue=53809000000.0),
+ Revenue(as_of_date=datetime.datetime(2019, 3, 31, 0, 0), report_type='R', period='3M', revenue=58015000000.0),
+ Revenue(as_of_date=datetime.datetime(2018, 12, 31, 0, 0), report_type='R', period='3M', revenue=84310000000.0),
+ Revenue(as_of_date=datetime.datetime(2018, 9, 30, 0, 0), report_type='R', period='3M', revenue=62900000000.0),
+ Revenue(as_of_date=datetime.datetime(2018, 6, 30, 0, 0), report_type='R', period='3M', revenue=53265000000.0),
+ Revenue(as_of_date=datetime.datetime(2018, 3, 31, 0, 0), report_type='R', period='3M', revenue=61137000000.0),
+ Revenue(as_of_date=datetime.datetime(2017, 12, 31, 0, 0), report_type='R', period='3M', revenue=88293000000.0),
+ Revenue(as_of_date=datetime.datetime(2017, 9, 30, 0, 0), report_type='R', period='3M', revenue=52579000000.0),
+ Revenue(as_of_date=datetime.datetime(2017, 6, 30, 0, 0), report_type='R', period='3M', revenue=45408000000.0)]
+
 ````
 
+## Contributing
+
+If you find a bug please open an issue, pull requests are always welcome.
+
+To develop with `ib_fundamental` please follow these steps
+
+```bash
+git clone https://github.com/quantbelt/ib_fundamental.git
+cd ib_fundamental
+# install development dependencies
+pip install .[dev]
+# do your things
+# run linters and code quality checks
+pre-commit
+# run tests with tox, requires pypy310,py{310,311,312}
+tox
+```
 
 [reqFundamental]: https://ib-api-reloaded.github.io/ib_async/api.html#ib_async.ib.IB.reqFundamentalData
 [fin_ratios]: http://web.archive.org/web/20200725010343/https://interactivebrokers.github.io/tws-api/fundamental_ratios_tags.html
```

### Comparing `ib_fundamental-0.0.1/pyproject.toml` & `ib_fundamental-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ib_fundamental"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "gnzsnz" }]
 description = "Interactive Brokers Fundamental data for humans"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE.txt" }
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Development Status :: 3 - Alpha",
 ]
-dependencies = [
-  "ib_async>=1.0.1",
-  "pandas>=2.2.2",
-  "defusedxml>=0.7.1",
-]
+dependencies = ["ib_async>=1.0.1", "pandas>=2.2.2", "defusedxml>=0.7.1"]
 
 [project.urls]
 "Homepage" = "https://github.com/quantbelt/ib_fundamental"
 "Bug Tracker" = "https://github.com/quantbelt/ib_fundamental/issues"
 
 [project.optional-dependencies] # Optional
 dev = [
@@ -32,19 +28,20 @@
   "pylint>=3.1.1",
   "isort>=5.13.2",
   "mypy>=1.10.0",
   "pre-commit>=3.7.1",
   "pandas-stubs>=2.2.1.240316",
   "bandit[toml]>=1.7.8",
   "flake8>=7.0.0",
+  "flake8-pytest-style>=2.0.0",
   "pytest>=8.2.1",
   "pytest-env>=1.1.3",
   "pytest-cov>=4.1.0",
   "pylint-pytest>=1.1.7",
-  "flake8-pytest-style>=2.0.0"
+  "tox>=4.0.0",
 ]
 #test = ["coverage"]
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
@@ -56,30 +53,29 @@
 [tool.pylint.format]
 # black compatibility
 # https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#pylint
 max-line-length = "88"
 
 [tool.bandit]
 #exclude_dirs = ["tests"]
-skips = ["B101","B405"]
+skips = ["B101", "B405"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "-ra"
 log_cli = true
 #log_cli_level = "INFO"
 log_format = "%(asctime)s %(levelname)s %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
-log_disable = ["ib_async.ib","ib_async.client","ib_async.wrapper"]
+log_disable = ["ib_async.ib", "ib_async.client", "ib_async.wrapper"]
 minversion = "6.0"
 filterwarnings = "ignore"
 norecursedirs = ["docs", "build"]
 
 # Specify a custom directory for pytest cache
 cache_dir = "tests/.pytest_cache"
 # environment
 env = [
-    "IBFUND_SYMBOL=IBKR",
-    "IBFUND_HOST=localhost",
-    "IBFUND_PORT=7497",
-    "IBFUND_CLI_ID=120",
+  "IBFUND_HOST=localhost",
+  "IBFUND_PORT=7497",
+  "IBFUND_CLI_ID=120",
 ]
```

