# Comparing `tmp/thingspire-datasets-0.1.4.tar.gz` & `tmp/thingspire-datasets-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingspire-datasets-0.1.4.tar", last modified: Wed May  8 05:54:57 2024, max compression
+gzip compressed data, was "thingspire-datasets-0.1.5.tar", last modified: Wed May 29 09:00:44 2024, max compression
```

## Comparing `thingspire-datasets-0.1.4.tar` & `thingspire-datasets-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 05:54:57.313547 thingspire-datasets-0.1.4/
--rw-rw-rw-   0        0        0      594 2024-05-08 05:54:57.313547 thingspire-datasets-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-08 05:54:57.314550 thingspire-datasets-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      821 2024-05-08 05:54:51.000000 thingspire-datasets-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:54:57.285359 thingspire-datasets-0.1.4/thingspire/
--rw-rw-rw-   0        0        0      149 2024-05-08 05:46:46.000000 thingspire-datasets-0.1.4/thingspire/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:54:57.298976 thingspire-datasets-0.1.4/thingspire/dataset/
--rw-rw-rw-   0        0        0      133 2024-05-08 05:46:46.000000 thingspire-datasets-0.1.4/thingspire/dataset/__init__.py
--rw-rw-rw-   0        0        0     5190 2024-05-07 08:50:18.000000 thingspire-datasets-0.1.4/thingspire/dataset/get_calendar.py
--rw-rw-rw-   0        0        0     7520 2024-05-07 06:40:21.000000 thingspire-datasets-0.1.4/thingspire/dataset/get_weather.py
--rw-rw-rw-   0        0        0    15557 2024-05-02 01:56:43.000000 thingspire-datasets-0.1.4/thingspire/dataset/resource-id-name.py
--rw-rw-rw-   0        0        0     1879 2024-05-02 01:55:42.000000 thingspire-datasets-0.1.4/thingspire/dataset/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:54:57.310541 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/
--rw-rw-rw-   0        0        0      594 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 thingspire  (1000) thingspire  (1000)        0 2024-05-29 09:00:44.916252 thingspire-datasets-0.1.5/
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)      637 2024-05-29 09:00:44.916252 thingspire-datasets-0.1.5/PKG-INFO
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)     2372 2024-05-10 05:16:12.000000 thingspire-datasets-0.1.5/README.md
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)       79 2024-05-29 09:00:44.916252 thingspire-datasets-0.1.5/setup.cfg
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)      832 2024-05-29 00:56:24.000000 thingspire-datasets-0.1.5/setup.py
+drwxrwxr-x   0 thingspire  (1000) thingspire  (1000)        0 2024-05-29 09:00:44.916252 thingspire-datasets-0.1.5/thingspire/
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)      137 2024-05-29 07:08:11.000000 thingspire-datasets-0.1.5/thingspire/__init__.py
+drwxrwxr-x   0 thingspire  (1000) thingspire  (1000)        0 2024-05-29 09:00:44.916252 thingspire-datasets-0.1.5/thingspire/datasets/
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)      119 2024-05-29 04:37:00.000000 thingspire-datasets-0.1.5/thingspire/datasets/__init__.py
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)    15557 2024-05-02 01:56:43.000000 thingspire-datasets-0.1.5/thingspire/datasets/resource-id-name.py
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)     6103 2024-05-28 09:03:58.000000 thingspire-datasets-0.1.5/thingspire/datasets/ts_calendar.py
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)     9363 2024-05-29 08:56:31.000000 thingspire-datasets-0.1.5/thingspire/datasets/ts_weather.py
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)     1879 2024-05-02 01:55:42.000000 thingspire-datasets-0.1.5/thingspire/datasets/utils.py
+drwxrwxr-x   0 thingspire  (1000) thingspire  (1000)        0 2024-05-29 09:00:44.916252 thingspire-datasets-0.1.5/thingspire_datasets.egg-info/
+-rw-r--r--   0 thingspire  (1000) thingspire  (1000)      637 2024-05-29 09:00:44.000000 thingspire-datasets-0.1.5/thingspire_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 thingspire  (1000) thingspire  (1000)      435 2024-05-29 09:00:44.000000 thingspire-datasets-0.1.5/thingspire_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 thingspire  (1000) thingspire  (1000)        1 2024-05-29 09:00:44.000000 thingspire-datasets-0.1.5/thingspire_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 thingspire  (1000) thingspire  (1000)       41 2024-05-29 09:00:44.000000 thingspire-datasets-0.1.5/thingspire_datasets.egg-info/requires.txt
+-rw-rw-r--   0 thingspire  (1000) thingspire  (1000)       11 2024-05-29 09:00:44.000000 thingspire-datasets-0.1.5/thingspire_datasets.egg-info/top_level.txt
```

### Comparing `thingspire-datasets-0.1.4/setup.py` & `thingspire-datasets-0.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 setuptools.setup(
     name="thingspire-datasets",
-    version="0.1.4",
+    version="0.1.5",
     author="Inho Kim",
     author_email="inho@thingspire.com",
     description="thingspire feature package",
     long_description="A package that collects and processes weather and "
                      "special day information by local government and "
                      "applies it to various projects",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    install_requires=['Bottleneck', 'numpy', 'pandas', 'requests'],
+    install_requires=['Bottleneck', 'numpy', 'pandas', 'requests', 'aiohttp'],
     keywords=['thingspire', 'thingspire'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6'
```

### Comparing `thingspire-datasets-0.1.4/thingspire/dataset/get_weather.py` & `thingspire-datasets-0.1.5/thingspire/datasets/ts_weather.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,63 @@
-from datetime import datetime, timedelta
+import aiohttp
+import asyncio
+from datetime import datetime
 import json
 import time
 import pandas as pd
-import requests
-from io import StringIO
 import numpy as np
+from io import StringIO
 import os
 
 from .utils import flomon_url, api_payload, region_name
 
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 
 current_dir = os.path.dirname(__file__)
 json_path = os.path.join(current_dir, 'resource-id-name.py')
 
 
+class ThingsAPIError(Exception):
+    pass
+
+class InvalidAPIKeyError(ThingsAPIError):
+    pass
+
+class InvalidAPIURLError(ThingsAPIError):
+    pass
+
+class InvalidLocationError(ThingsAPIError):
+    pass
+
+class InvalidDateFormatError(ThingsAPIError):
+    pass
+
+class InvalidDiffError(ThingsAPIError):
+    pass
+
+class InvalidDataError(ThingsAPIError):
+    pass
+
+class DateDifferenceError(ThingsAPIError):
+    pass
+
+
+def validate_date(date_text):
+    try:
+        datetime.strptime(date_text, '%Y%m%d')
+    except ValueError:
+        raise InvalidDateFormatError(f"Incorrect data format for date: {date_text}. It should be YYYYMMDD.")
+
+
 def find_sido(input_name, region_dict):
     for key, names in region_dict.items():
         if input_name in names:
             return key
-    return "해당 지역을 찾을 수 없습니다."
 
 
 def filter_by_name(start_str, df=pd.read_json(json_path)):
     result_df = df[df['name'].str.startswith(start_str)]
     return result_df.to_json(force_ascii=False)
 
 
@@ -81,15 +113,18 @@
         for time, values in times.items():
             row = values.copy()
             row['region'] = district
             row['time'] = time
             rows_list.append(row)
 
     df = pd.DataFrame(rows_list)
-    df['datetime'] = pd.to_datetime(df['time'], unit='ms')
+    try:
+        df['datetime'] = pd.to_datetime(df['time'], unit='ms')
+    except:
+        raise InvalidDataError("No data exists for that time. Data exists from March 12, 2024.")
     df['datetime'] = df['datetime'].dt.tz_localize('UTC')
     df['datetime'] = df['datetime'].dt.tz_convert('Asia/Seoul')
 
     return df
 
 
 def slice_outter(group, start, end):
@@ -100,15 +135,17 @@
 
     return group
 
 
 def region_inter(df, start, end):
     for col in df.columns:
         if df[col].apply(lambda x: isinstance(x, list)).any():
-            df[col] = df[col].apply(lambda x: x[0] if isinstance(x, list) else x)
+            values = df[col].values
+            mask = np.array([isinstance(x, list) for x in values])
+            df.loc[mask, col] = [x[0] if isinstance(x, list) else x for x in values[mask]]
 
     df.set_index('datetime', inplace=True)
     results = []
     for name, group in df.groupby('region'):
         full_index = pd.date_range(start=group.index.min(), end=group.index.max(), freq='h')
         group = group.reindex(full_index)
         group.interpolate(method='time', inplace=True)
@@ -128,21 +165,22 @@
     df = kor_time(js)
     df = region_inter(df, start, end)
 
     required_columns = ['windGust', 'windDirection', 'windSpeed']
     for col in required_columns:
         if col not in df.columns:
             df[col] = 0
-
-    df = df[['region', 'datetime', 'time',
+    try:
+        df = df[['region', 'datetime', 'time',
              'sunrise', 'sunset', 'temp', 'sensibleTemp',
              'humidity', 'pressure', 'clouds', 'visibility',
              'precipitationIntensity', 'snowfall', 'windGust',
              'windDirection', 'windSpeed', 'weatherCode']]
-
+    except:
+        raise InvalidDataError("No data exists for that time. Data exists from March 12, 2024.")
     df['datetime'] = df['datetime'].dt.tz_localize(None)
     df = df.fillna(0)
 
     return df
 
 
 def adjust_column_names(cols):
@@ -154,68 +192,77 @@
             else:
                 new_cols.append(col[0])
         else:
             new_cols.append(col)
     return new_cols
 
 
-def hourly_to_daily(df):
-    df['date'] = df['datetime'].dt.date
+async def fetch(url, api_key, api_payload, semaphore):
+    headers = {'Authorization': api_key}
+    async with semaphore:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, headers=headers, data=api_payload) as response:
+                if response.status == 401:
+                    raise InvalidAPIKeyError("The API key provided is invalid.")
+                elif response.status == 404:
+                    raise InvalidLocationError("The API URL is invalid.")
+                elif response.status != 200:
+                    raise ThingsAPIError(f"Failed to fetch weather data: {await response.text()}")
+                return await response.json()
+
+
+async def get_weather_async(api_key, api_url,
+                            sido, gungu="",
+                            start=datetime.today().strftime('%Y%m%d'),
+                            end=datetime.today().strftime('%Y%m%d')):
+    if int(end) - int(start) >= 0:
+        validate_date(start)
+        validate_date(end)
+    else:
+        raise InvalidDiffError("The start date is greater than the end date.")
+
+    start_date = datetime.strptime(start, "%Y%m%d")
+    end_date = datetime.strptime(end, "%Y%m%d")
+    if (end_date - start_date).days > 32:
+        raise DateDifferenceError("Weather data requests can only be made for up to one month.")
 
-    daily_data = df.groupby(['region', 'date']).agg({
-        'sunrise': 'min',
-        'sunset': 'max',
-        'temp': ['max', 'mean', 'min'],
-        'sensibleTemp': ['max', 'mean', 'min'],
-        'humidity': 'mean',
-        'pressure': 'mean',
-        'clouds': 'mean',
-        'visibility': 'mean',
-        'precipitationIntensity':'sum',
-        'snowfall':'sum',
-        'windGust': 'max',
-        'windDirection': 'mean',
-        'windSpeed': 'mean',
-        'weatherCode': lambda x: x.mode()[0]
-    })
-
-    daily_data.columns = adjust_column_names(daily_data.columns)
-    daily_data.reset_index(inplace=True)
-
-    return daily_data
-
-
-def select_weather(weather_key, weather_url,
-                   sido, gungu = "",
-                   start = datetime.today().strftime('%Y%m%d'),
-                   end = datetime.today().strftime('%Y%m%d'),
-                   period="hourly"):
 
     region_df = pd.read_json(json_path)
     id_names = load_id_names(json_path)
+
     specific_sido = find_sido(sido, region_name)
-    specific_gungu = specific_sido + gungu
+    if specific_sido is None:
+        raise InvalidLocationError("The 'sido' parameter is invalid, please check it.")
 
+    specific_gungu = specific_sido + gungu
     region_list = filter_by_name(specific_gungu, region_df)
     region_list = pd.read_json(StringIO(region_list))
     region_list = region_list["id"].tolist()
-    region_len = len(region_list)
-    region_params = ""
-    for i in range(len(region_list)):
-        region_params += f"resourceIds={region_list[i]}&"
-
-    start_time = (time.mktime(datetime.strptime(start, "%Y%m%d").timetuple()) -1800) *1000
-    end_time = (time.mktime(datetime.strptime(end, "%Y%m%d").timetuple()) +86300 +1800) *1000
-    limit = (end_time-start_time)//(3600*1000)*3
-    if limit == 0 : limit = 24*3
+    if not region_list:
+        raise InvalidLocationError("The 'gungu' parameter is invalid, please check it.")
 
-    url = weather_url + flomon_url + f"limit={int(limit)}&" + region_params + f"startTime={int(start_time)}&" + f"endTime={int(end_time)}"
-    response = requests.request("GET", url, headers={'Authorization': weather_key}, data=api_payload)
+    region_params = "&".join([f"resourceIds={region_id}" for region_id in region_list])
 
-    processed_data = round_time_and_aggregate(response.json())
+    start_time = (time.mktime(datetime.strptime(start, "%Y%m%d").timetuple()) - 1800) * 1000
+    end_time = (time.mktime(datetime.strptime(end, "%Y%m%d").timetuple()) + 86300 + 1800) * 1000
+    limit = (end_time - start_time) // (3600 * 1000) * 3
+    if limit == 0:
+        limit = 24 * 3
+
+    url = f"{api_url}{flomon_url}limit={int(limit)}&{region_params}&startTime={int(start_time)}&endTime={int(end_time)}"
+
+    semaphore = asyncio.Semaphore(10)  # 동시 요청 수 제한
+
+    try:
+        response = await fetch(url, api_key, api_payload, semaphore)
+    except aiohttp.ClientError as e:
+        raise InvalidAPIURLError("The API URL is invalid.") from e
+
+    processed_data = round_time_and_aggregate(response)
     named_data = ids_to_names(processed_data, id_names)
     output = js_to_dataframe(named_data, start, end)
 
-    if period == "daily":
-        output = hourly_to_daily(output)
+    return output
+
 
-    return output
+def get_weather(api_key, api_url, sido, gungu="", start=datetime.today().strftime('%Y%m%d'), end=datetime.today().strftime('%Y%m%d')):
+    return asyncio.run(get_weather_async(api_key, api_url, sido, gungu, start, end))
```

### Comparing `thingspire-datasets-0.1.4/thingspire/dataset/resource-id-name.py` & `thingspire-datasets-0.1.5/thingspire/datasets/resource-id-name.py`

 * *Files identical despite different names*

### Comparing `thingspire-datasets-0.1.4/thingspire/dataset/utils.py` & `thingspire-datasets-0.1.5/thingspire/datasets/utils.py`

 * *Files identical despite different names*

