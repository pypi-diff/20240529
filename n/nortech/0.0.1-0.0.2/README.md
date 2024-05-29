# Comparing `tmp/nortech-0.0.1.tar.gz` & `tmp/nortech-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nortech-0.0.1.tar", max compression
+gzip compressed data, was "nortech-0.0.2.tar", max compression
```

## Comparing `nortech-0.0.1.tar` & `nortech-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.0.1/LICENSE
--rw-r--r--   0        0        0     6228 2023-12-04 14:04:21.033886 nortech-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.0.1/nortech/__init__.py
--rw-r--r--   0        0        0      263 2023-12-03 16:08:08.271434 nortech-0.0.1/nortech/datatools/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.0.1/nortech/datatools/handlers/__init__.py
--rw-r--r--   0        0        0     2732 2023-12-03 20:06:53.859704 nortech-0.0.1/nortech/datatools/handlers/pandas.py
--rw-r--r--   0        0        0     5777 2023-12-04 14:00:13.514284 nortech-0.0.1/nortech/datatools/handlers/polars.py
--rw-r--r--   0        0        0     5210 2023-12-03 19:54:12.668941 nortech-0.0.1/nortech/datatools/repositories/S3.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.0.1/nortech/datatools/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.0.1/nortech/datatools/services/__init__.py
--rw-r--r--   0        0        0      615 2023-12-03 17:32:02.599887 nortech-0.0.1/nortech/datatools/services/config.py
--rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.0.1/nortech/datatools/values/__init__.py
--rw-r--r--   0        0        0      347 2023-12-03 19:51:26.287501 nortech-0.0.1/nortech/datatools/values/errors.py
--rw-r--r--   0        0        0     2159 2023-12-03 19:51:44.164402 nortech-0.0.1/nortech/datatools/values/signals.py
--rw-r--r--   0        0        0     1617 2023-12-04 14:00:47.189471 nortech-0.0.1/nortech/datatools/values/test.py
--rw-r--r--   0        0        0      741 2023-12-04 14:29:31.953612 nortech-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7114 1970-01-01 00:00:00.000000 nortech-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6228 2023-12-04 14:04:21.033886 nortech-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.0.2/nortech/__init__.py
+-rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.0.2/nortech/datatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.0.2/nortech/datatools/handlers/__init__.py
+-rw-r--r--   0        0        0     2828 2023-12-04 17:38:39.495516 nortech-0.0.2/nortech/datatools/handlers/pandas.py
+-rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.0.2/nortech/datatools/handlers/polars.py
+-rw-r--r--   0        0        0     5200 2023-12-04 16:16:06.875409 nortech-0.0.2/nortech/datatools/repositories/S3.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.0.2/nortech/datatools/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.0.2/nortech/datatools/services/__init__.py
+-rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.0.2/nortech/datatools/services/config.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.0.2/nortech/datatools/values/__init__.py
+-rw-r--r--   0        0        0      347 2023-12-03 19:51:26.287501 nortech-0.0.2/nortech/datatools/values/errors.py
+-rw-r--r--   0        0        0     2159 2023-12-03 19:51:44.164402 nortech-0.0.2/nortech/datatools/values/signals.py
+-rw-r--r--   0        0        0      700 2023-12-18 17:23:35.942876 nortech-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7068 1970-01-01 00:00:00.000000 nortech-0.0.2/PKG-INFO
```

### Comparing `nortech-0.0.1/LICENSE` & `nortech-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nortech-0.0.1/README.md` & `nortech-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nortech-0.0.1/nortech/datatools/handlers/pandas.py` & `nortech-0.0.2/nortech/datatools/handlers/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     NoSignalsRequestedError
         Raised when no signals are requested.
     InvalidTimeWindow
         Raised when the start date is after the end date.
 
     Example
     -------
+    >>> from datetime import datetime
     >>> from nortech.datatools import get_df, TimeWindow
     >>> search_json = \"""[
         {
             "name": "signal_1",
             "dataType": "float",
             "alias": 0,
             "asset": {
@@ -88,14 +89,19 @@
     ]\"""
     >>> time_window = TimeWindow(
                 start=datetime(2020, 1, 1),
                 end=datetime(2020, 1, 1),
         )
     >>> df = get_df(search_json=search_json, time_window=time_window)
     >>> df.columns
-        ['timestamp', 'asset_1/division_1/unit_1/signal_1', 'asset_1/division_1/unit_1/signal_2', 'asset_2/division_2/unit_2/signal_3']
+        [
+            'timestamp',
+            'asset_1/division_1/unit_1/signal_1',
+            'asset_1/division_1/unit_1/signal_2',
+            'asset_2/division_2/unit_2/signal_3'
+        ]
     """
     polars_df = get_polars_df(search_json=search_json, time_window=time_window)
 
     df = polars_df.to_pandas()
 
     return df
```

### Comparing `nortech-0.0.1/nortech/datatools/handlers/polars.py` & `nortech-0.0.2/nortech/datatools/handlers/polars.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     NoSignalsRequestedError
         Raised when no signals are requested.
     InvalidTimeWindow
         Raised when the start date is after the end date.
 
     Example
     -------
+    >>> from datetime import datetime
     >>> from nortech.datatools import get_lazy_polars_df, TimeWindow
     >>> search_json = \"""[
         {
             "name": "signal_1",
             "dataType": "float",
             "alias": 0,
             "asset": {
@@ -92,15 +93,20 @@
     ]\"""
     >>> time_window = TimeWindow(
                 start=datetime(2020, 1, 1),
                 end=datetime(2020, 1, 1),
         )
     >>> lazy_polars_df = get_lazy_polars_df(search_json=search_json, time_window=time_window)
     >>> lazy_polars_df.columns
-        ['timestamp', 'asset_1/division_1/unit_1/signal_1', 'asset_1/division_1/unit_1/signal_2', 'asset_2/division_2/unit_2/signal_3']
+        [
+            'timestamp',
+            'asset_1/division_1/unit_1/signal_1',
+            'asset_1/division_1/unit_1/signal_2',
+            'asset_2/division_2/unit_2/signal_3'
+        ]
     """
     signal_list = get_signal_list_from_search_json(search_json=search_json)
     parquet_paths = get_parquet_paths_from_search_list(signal_list=signal_list)
     lazy_polars_df = get_lazy_polars_df_from_S3(
         parquet_paths=parquet_paths, time_window=time_window
     )
 
@@ -128,14 +134,15 @@
     NoSignalsRequestedError
         Raised when no signals are requested.
     InvalidTimeWindow
         Raised when the start date is after the end date.
 
     Example
     -------
+    >>> from datetime import datetime
     >>> from nortech.datatools import get_polars_df, TimeWindow
     >>> search_json = \"""[
         {
             "name": "signal_1",
             "dataType": "float",
             "alias": 0,
             "asset": {
@@ -191,15 +198,20 @@
     ]\"""
     >>> time_window = TimeWindow(
                 start=datetime(2020, 1, 1),
                 end=datetime(2020, 1, 1),
         )
     >>> polars_df = get_polars_df(search_json=search_json, time_window=time_window)
     >>> polars_df.columns
-        ['timestamp', 'asset_1/division_1/unit_1/signal_1', 'asset_1/division_1/unit_1/signal_2', 'asset_2/division_2/unit_2/signal_3']
+        [
+            'timestamp',
+            'asset_1/division_1/unit_1/signal_1',
+            'asset_1/division_1/unit_1/signal_2',
+            'asset_2/division_2/unit_2/signal_3'
+        ]
     """
     lazy_polars_df = get_lazy_polars_df(
         search_json=search_json, time_window=time_window
     )
     polars_df = lazy_polars_df.collect()
 
     return polars_df
```

### Comparing `nortech-0.0.1/nortech/datatools/repositories/S3.py` & `nortech-0.0.2/nortech/datatools/repositories/S3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timedelta
 from os import getenv
 from typing import List, Tuple
 
 import pyarrow as pa
 from polars import Expr, LazyFrame, col, from_epoch, scan_pyarrow_dataset
 from pyarrow import DataType, Schema, schema
 from pyarrow.dataset import dataset, partitioning
```

### Comparing `nortech-0.0.1/nortech/datatools/services/config.py` & `nortech-0.0.2/nortech/datatools/services/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Dict, List
+from typing import List
 
 from nortech.datatools.values.signals import ParquetPaths, Signal, SignalConfig
 
 
 def get_parquet_paths_from_search_list(signal_list: List[Signal]) -> ParquetPaths:
     parquet_paths: ParquetPaths = defaultdict(list)
```

### Comparing `nortech-0.0.1/nortech/datatools/values/signals.py` & `nortech-0.0.2/nortech/datatools/values/signals.py`

 * *Files identical despite different names*

### Comparing `nortech-0.0.1/pyproject.toml` & `nortech-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nortech"
-version = "0.0.1"
+version = "0.0.2"
 description = "The official Python library for Nortech AI"
 authors = ["Nortech AI <info@nortech.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://nortech.ai/"
 repository = "https://github.com/Nortech-ai/nortech-python"
 
@@ -12,22 +12,18 @@
 python = "^3.9"
 pandas = "^2.1.3"
 polars = "^0.19.19"
 pyarrow = "^13.0.0"
 s3fs = "2023.6.0"
 aiobotocore = "2.5.2"
 pydantic = "^2.5.2"
-moto = {extras = ["server"], version = "^4.2.11"}
-
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 ipykernel = "^6.27.1"
 black = "^23.11.0"
-
-
-[tool.poetry.group.boto3.dependencies]
-moto = "^4.2.11"
+flake8 = "^6.1.0"
+moto = {extras = ["server"], version = "^4.2.11"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nortech-0.0.1/PKG-INFO` & `nortech-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: nortech
-Version: 0.0.1
+Version: 0.0.2
 Summary: The official Python library for Nortech AI
 Home-page: https://nortech.ai/
 License: Apache-2.0
 Author: Nortech AI
 Author-email: info@nortech.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiobotocore (==2.5.2)
-Requires-Dist: moto[server] (>=4.2.11,<5.0.0)
 Requires-Dist: pandas (>=2.1.3,<3.0.0)
 Requires-Dist: polars (>=0.19.19,<0.20.0)
 Requires-Dist: pyarrow (>=13.0.0,<14.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: s3fs (==2023.6.0)
 Project-URL: Repository, https://github.com/Nortech-ai/nortech-python
 Description-Content-Type: text/markdown
```

