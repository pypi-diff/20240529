# Comparing `tmp/pycocap-1.2.0.tar.gz` & `tmp/pycocap-1.3.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycocap-1.2.0.tar", last modified: Tue Nov 14 14:42:30 2023, max compression
+gzip compressed data, was "pycocap-1.3.3.dev2.tar", last modified: Wed May 29 09:49:37 2024, max compression
```

## Comparing `pycocap-1.2.0.tar` & `pycocap-1.3.3.dev2.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 14:42:30.884257 pycocap-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-11-14 14:42:11.000000 pycocap-1.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-11-14 14:42:11.000000 pycocap-1.2.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     3002 2023-11-14 14:42:30.884257 pycocap-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1697 2023-11-14 14:42:11.000000 pycocap-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 14:42:30.878258 pycocap-1.2.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 14:42:30.879258 pycocap-1.2.0/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)     2406 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/source/contents.rst
--rw-rw-rw-   0 root         (0) root         (0)     1763 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/source/package.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 14:42:30.881258 pycocap-1.2.0/docs/source/pics/
--rw-rw-rw-   0 root         (0) root         (0)    11218 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/source/pics/COCAP.ico
--rw-rw-rw-   0 root         (0) root         (0)  1656592 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/source/pics/COCAP.png
--rw-rw-rw-   0 root         (0) root         (0)    25697 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/source/pics/COCAP_logo.png
--rw-rw-rw-   0 root         (0) root         (0)   396861 2023-11-14 14:42:11.000000 pycocap-1.2.0/docs/source/pics/COCAP_small.png
--rw-rw-rw-   0 root         (0) root         (0)     1533 2023-11-14 14:42:11.000000 pycocap-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-14 14:42:30.884257 pycocap-1.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 14:42:30.876258 pycocap-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 14:42:30.882258 pycocap-1.2.0/src/pycocap/
--rw-rw-rw-   0 root         (0) root         (0)      818 2023-11-14 14:42:11.000000 pycocap-1.2.0/src/pycocap/__init__.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-11-14 14:42:30.000000 pycocap-1.2.0/src/pycocap/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    25379 2023-11-14 14:42:11.000000 pycocap-1.2.0/src/pycocap/pycocap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 14:42:30.883257 pycocap-1.2.0/src/pycocap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3002 2023-11-14 14:42:30.000000 pycocap-1.2.0/src/pycocap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-11-14 14:42:30.000000 pycocap-1.2.0/src/pycocap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-14 14:42:30.000000 pycocap-1.2.0/src/pycocap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-11-14 14:42:30.000000 pycocap-1.2.0/src/pycocap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-11-14 14:42:30.000000 pycocap-1.2.0/src/pycocap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 14:42:30.883257 pycocap-1.2.0/tables/
--rw-rw-rw-   0 root         (0) root         (0)     2985 2023-11-14 14:42:11.000000 pycocap-1.2.0/tables/all_countries_timeseries_availability.csv
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.506691 pycocap-1.3.3.dev2/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      174 2022-08-25 13:53:24.000000 pycocap-1.3.3.dev2/.gitignore
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      700 2024-05-29 09:48:44.000000 pycocap-1.3.3.dev2/.gitlab-ci.yml
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     3007 2024-05-29 09:49:37.506691 pycocap-1.3.3.dev2/PKG-INFO
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     1697 2022-09-09 09:22:19.000000 pycocap-1.3.3.dev2/README.md
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.403358 pycocap-1.3.3.dev2/docs/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      638 2022-08-23 10:18:42.000000 pycocap-1.3.3.dev2/docs/Makefile
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      804 2022-08-23 10:18:42.000000 pycocap-1.3.3.dev2/docs/make.bat
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.423358 pycocap-1.3.3.dev2/docs/source/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     2406 2022-08-25 13:51:55.000000 pycocap-1.3.3.dev2/docs/source/conf.py
+-rw-r--r--   0 lennart   (1000) lennart   (1000)       97 2022-08-25 13:40:45.000000 pycocap-1.3.3.dev2/docs/source/contents.rst
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     1763 2022-09-09 09:22:29.000000 pycocap-1.3.3.dev2/docs/source/index.rst
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      119 2022-08-25 13:41:17.000000 pycocap-1.3.3.dev2/docs/source/package.rst
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.460024 pycocap-1.3.3.dev2/docs/source/pics/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    11218 2022-08-23 11:56:35.000000 pycocap-1.3.3.dev2/docs/source/pics/COCAP.ico
+-rw-r--r--   0 lennart   (1000) lennart   (1000)  1656592 2022-01-26 15:04:58.000000 pycocap-1.3.3.dev2/docs/source/pics/COCAP.png
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    25697 2022-08-23 11:56:16.000000 pycocap-1.3.3.dev2/docs/source/pics/COCAP_logo.png
+-rw-r--r--   0 lennart   (1000) lennart   (1000)   396861 2022-08-23 11:54:22.000000 pycocap-1.3.3.dev2/docs/source/pics/COCAP_small.png
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     1533 2023-01-24 16:00:16.000000 pycocap-1.3.3.dev2/pyproject.toml
+-rw-r--r--   0 lennart   (1000) lennart   (1000)       38 2024-05-29 09:49:37.506691 pycocap-1.3.3.dev2/setup.cfg
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.393358 pycocap-1.3.3.dev2/src/
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.480024 pycocap-1.3.3.dev2/src/pycocap/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      818 2023-11-01 16:13:18.000000 pycocap-1.3.3.dev2/src/pycocap/__init__.py
+-rw-r--r--   0 lennart   (1000) lennart   (1000)       26 2024-05-29 09:49:37.000000 pycocap-1.3.3.dev2/src/pycocap/_version.py
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    25498 2024-05-29 08:30:32.000000 pycocap-1.3.3.dev2/src/pycocap/pycocap.py
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.506691 pycocap-1.3.3.dev2/src/pycocap.egg-info/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     3007 2024-05-29 09:49:37.000000 pycocap-1.3.3.dev2/src/pycocap.egg-info/PKG-INFO
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      604 2024-05-29 09:49:37.000000 pycocap-1.3.3.dev2/src/pycocap.egg-info/SOURCES.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)        1 2024-05-29 09:49:37.000000 pycocap-1.3.3.dev2/src/pycocap.egg-info/dependency_links.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)       82 2024-05-29 09:49:37.000000 pycocap-1.3.3.dev2/src/pycocap.egg-info/requires.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)        8 2024-05-29 09:49:37.000000 pycocap-1.3.3.dev2/src/pycocap.egg-info/top_level.txt
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.480024 pycocap-1.3.3.dev2/tables/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     2985 2023-02-06 16:02:59.000000 pycocap-1.3.3.dev2/tables/all_countries_timeseries_availability.csv
+drwxr-xr-x   0 lennart   (1000) lennart   (1000)        0 2024-05-29 09:49:37.496691 pycocap-1.3.3.dev2/tests/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     3518 2022-09-08 13:53:50.000000 pycocap-1.3.3.dev2/tests/test_pycocap.py
```

### Comparing `pycocap-1.2.0/PKG-INFO` & `pycocap-1.3.3.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycocap
-Version: 1.2.0
+Version: 1.3.3.dev2
 Summary: PyCOCAP: The Python interface to the COCAP database
 Author-email: Lennart Schüler <lennart.schueler@ufz.de>
 Project-URL: Documentation, https://cocap.pages.hzdr.de/pycocap/
 Project-URL: Source, https://gitlab.hzdr.de/cocap/pycocap/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `pycocap-1.2.0/README.md` & `pycocap-1.3.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/docs/Makefile` & `pycocap-1.3.3.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/docs/make.bat` & `pycocap-1.3.3.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/docs/source/conf.py` & `pycocap-1.3.3.dev2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/docs/source/index.rst` & `pycocap-1.3.3.dev2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/docs/source/pics/COCAP.ico` & `pycocap-1.3.3.dev2/docs/source/pics/COCAP.ico`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/docs/source/pics/COCAP.png` & `pycocap-1.3.3.dev2/docs/source/pics/COCAP.png`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/docs/source/pics/COCAP_logo.png` & `pycocap-1.3.3.dev2/docs/source/pics/COCAP_logo.png`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/docs/source/pics/COCAP_small.png` & `pycocap-1.3.3.dev2/docs/source/pics/COCAP_small.png`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/pyproject.toml` & `pycocap-1.3.3.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/src/pycocap/__init__.py` & `pycocap-1.3.3.dev2/src/pycocap/__init__.py`

 * *Files identical despite different names*

### Comparing `pycocap-1.2.0/src/pycocap/pycocap.py` & `pycocap-1.3.3.dev2/src/pycocap/pycocap.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 import numpy as np
 import pandas as pd
 
 
 API_URL = 'https://web.app.ufz.de/cocap/'
 
 
+Date = Union[date, np.datetime64]
+
+
 def cut_at_dates(
     df: pd.DataFrame,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
 ) -> pd.DataFrame:
     """Cut a DataFrame at given dates."""
     if (start_date is not None or end_date is not None) and start_date == end_date:
         raise ValueError('start_date and end_date cannot be equal')
     mask = None
     if start_date is not None:
         start_date = pd.to_datetime(start_date)
@@ -33,16 +36,16 @@
     if mask is not None:
         df = df[mask]
     return df
 
 def regularize_timeseries(
     df: pd.DataFrame,
     fill_value: Optional[Union[float, str]] = None,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
 ) -> pd.DataFrame:
     """Fill missing data with NaNs, or fill_value to get a regular timeseries"""
     # TODO can all this be done cleaner?!
     sd = start_date if start_date is not None else df['date'].iloc[0]
     ed = end_date if end_date is not None else df['date'].iloc[-1]
     idx = pd.date_range(sd, ed, freq='D', inclusive='left')
     df = df.set_index('date')
@@ -56,22 +59,23 @@
     if fill_value is not None:
         if fill_value == 'interpolate':
             # interpolate does not like dates...
             df.loc[:, df.columns!='date'] = (
                 df.loc[:, df.columns!='date'].interpolate()
             )
         else:
-            df = df.fillna(fill_value)
+            with pd.option_context('future.no_silent_downcasting', True):
+                df = df.fillna(fill_value)
     return df
 
 def _convert_json_to_df(
     json,
     rename_cols: Optional[dict] = None,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     date_format: Optional[str] = None,
 ) -> pd.DataFrame:
     df = pd.DataFrame(json)
     if rename_cols is not None:
         df = df.rename(columns=rename_cols)
     try:
         df['date'] = pd.to_datetime(df['date'], format=date_format)
@@ -80,16 +84,16 @@
     df = cut_at_dates(df, start_date, end_date)
     return df
 
 
 def reports(
     country: str,
     report_type: str,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
     fill_value: Union[float, str] = np.nan,
     return_population: bool = False,
 ) -> Any:
     """Get cases or deaths timeseries as a DataFrame from the db.
 
     Parameters
@@ -150,16 +154,16 @@
     r = df
     if return_population:
         r = (df, N)
     return r
 
 def cases(
     country: str,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
     fill_value: Union[float, str] = np.nan,
     return_population: bool = False,
 ) -> Any :
     """Get cases timeseries as a DataFrame from the db.
 
     Parameters
@@ -201,16 +205,16 @@
         params,
         fill_value,
         return_population,
     )
 
 def deaths(
     country: str,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
     fill_value: Union[float, str] = np.nan,
     return_population: bool = False,
 ) -> Any:
     """Get death timeseries as a DataFrame from the db.
 
     Parameters
@@ -254,29 +258,29 @@
         return_population,
     )
 
 def _report_nuts3(
     country: str,
     county_ids: List[int],
     report_type: str,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
 ) -> Optional[pd.DataFrame]:
     if country != 'Germany':
         raise ValueError("Local data only available for country = 'Germany'")
     county_ids_str = '_'.join(map(str, county_ids))
     response = requests.get(
         API_URL + f'nuts3/{country}/{county_ids_str}/{report_type}', params=params
     )
     if response.status_code == 200:
         r_json = response.json()
         if len(r_json['report']) == 0:
             warnings.warn(
-                f'Empty response for {country=}, {county_id=}, '
+                f'Empty response for {country=}, {county_ids_str=}, '
                 f' and {report_type=}, with {params=}'
             )
             df = None
         df = _convert_json_to_df(
             r_json['report'],
             {'count': report_type},
             start_date,
@@ -287,16 +291,16 @@
         df = None
     return df
 
 def reports_nuts3(
     country: str,
     county_ids: Union[List[int], int],
     report_types: Optional[Union[List[str], str]] = None,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     age_classes: Optional[Union[List[str], str]] = None,
     params: Optional[dict] = None,
 ) -> Optional[pd.DataFrame]:
     """Get multiple cummulative reports as a DataFrame for a county.
 
     Parameters
     ----------
@@ -371,15 +375,15 @@
             params,
             ) for report_type in _report_types  # pyright: ignore
     ]
     try:
         dfs = reduce(
             lambda df1, df2: pd.merge(df1, df2, on=['date', 'id_region']), dfs
         )  # pyright: ignore
-    except (KeyError, TyepError):
+    except (KeyError, TypeError):
         ...
     # move `id_region` to end of columns
     try:
         cols = list(dfs.columns.values)
         id_idx = cols.index('id_region')
         cols.append(cols.pop(id_idx))
         dfs = dfs[cols]
@@ -387,16 +391,16 @@
         ...
     return dfs
 
 def _report_nuts1(
     country: str,
     region_id: int,
     report_type: str,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
 ) -> Optional[pd.DataFrame]:
     if country != 'Germany':
         raise ValueError("Subnational data only available for country = 'Germany'")
     response = requests.get(
         API_URL + f'nuts1/{country}/{region_id}/{report_type}', params=params
     )
@@ -416,16 +420,16 @@
         df = None
     return df
 
 def reports_nuts1(
     country: str,
     region_id: Union[List[int], int],
     report_types: Optional[Union[List[str], str]] = None,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     age_classes: Optional[Union[List[str], str]] = None,
     params: Optional[dict] = None,
 ) -> Optional[pd.DataFrame]:
     """Get multiple cummulative reports as a DataFrame for a region.
 
     Parameters
     ----------
@@ -530,16 +534,16 @@
         ...
 
     return dfs
 
 def timeseries(
     country: str,
     report_type: str,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
     fill_value: Union[float, str] = np.nan,
 ) -> Optional[pd.DataFrame]:
     """Get a timeseries as a DataFrame from the db.
 
     Parameters
     ----------
@@ -619,16 +623,16 @@
         print(f'Response code: {response.status_code}')
         df = None
     return df
 
 def nfc(
     country: str,
     nfc_type: str,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
 ) -> Optional[pd.DataFrame]:
     """Get National Framework Conditions as a DataFrame from db.
 
     Parameters
     ----------
     country
@@ -694,16 +698,16 @@
         print(f'Response code: {response.status_code}')
         df = None
     return df
 
 def npi(
     country: str,
     npi_type: str,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
     fill_value: Union[float, str] = np.nan,
 ) -> Optional[pd.DataFrame]:
     """Get NPI timeseries as a DataFrame from the db.
 
     Parameters
     ----------
@@ -775,16 +779,16 @@
         print(f'Response code: {response.status_code}')
         df = None
     return df
 
 def npis(
     country: str,
     npi_types: Optional[Union[List, str]] = None,
-    start_date: Optional[date] = None,
-    end_date: Optional[date] = None,
+    start_date: Optional[Date] = None,
+    end_date: Optional[Date] = None,
     params: Optional[dict] = None,
     fill_value: Union[float, str] = np.nan,
 ) -> Optional[pd.DataFrame]:
     """Get multiple NPI timeseries as a DataFrame from the db.
 
     Parameters
     ----------
```

### Comparing `pycocap-1.2.0/src/pycocap.egg-info/PKG-INFO` & `pycocap-1.3.3.dev2/src/pycocap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycocap
-Version: 1.2.0
+Version: 1.3.3.dev2
 Summary: PyCOCAP: The Python interface to the COCAP database
 Author-email: Lennart Schüler <lennart.schueler@ufz.de>
 Project-URL: Documentation, https://cocap.pages.hzdr.de/pycocap/
 Project-URL: Source, https://gitlab.hzdr.de/cocap/pycocap/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `pycocap-1.2.0/src/pycocap.egg-info/SOURCES.txt` & `pycocap-1.3.3.dev2/src/pycocap.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 src/pycocap/_version.py
 src/pycocap/pycocap.py
 src/pycocap.egg-info/PKG-INFO
 src/pycocap.egg-info/SOURCES.txt
 src/pycocap.egg-info/dependency_links.txt
 src/pycocap.egg-info/requires.txt
 src/pycocap.egg-info/top_level.txt
-tables/all_countries_timeseries_availability.csv
+tables/all_countries_timeseries_availability.csv
+tests/test_pycocap.py
```

### Comparing `pycocap-1.2.0/tables/all_countries_timeseries_availability.csv` & `pycocap-1.3.3.dev2/tables/all_countries_timeseries_availability.csv`

 * *Files identical despite different names*

