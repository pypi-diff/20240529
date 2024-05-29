# Comparing `tmp/va_am-0.1.5.tar.gz` & `tmp/va_am-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "va_am-0.1.5.tar", last modified: Mon May 27 16:09:24 2024, max compression
+gzip compressed data, was "va_am-0.1.6.tar", last modified: Wed May 29 16:01:29 2024, max compression
```

## Comparing `va_am-0.1.5.tar` & `va_am-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.534761 va_am-0.1.5/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.5/LICENSE
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-27 16:09:24.534761 va_am-0.1.5/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.5/README.md
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-05-27 11:43:55.000000 va_am-0.1.5/pyproject.toml
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-05-27 16:09:24.534761 va_am-0.1.5/setup.cfg
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.5/setup.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.530761 va_am-0.1.5/src/
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.530761 va_am-0.1.5/src/va_am/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.5/src/va_am/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.5/src/va_am/__main__.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.530761 va_am-0.1.5/src/va_am/utils/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    60986 2024-05-20 13:28:39.000000 va_am-0.1.5/src/va_am/utils/AutoEncoders.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.5/src/va_am/utils/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.5/src/va_am/utils/functions.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)   103130 2024-05-27 11:43:55.000000 va_am-0.1.5/src/va_am/va_am.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.534761 va_am-0.1.5/src/va_am.egg-info/
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      517 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/entry_points.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/requires.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/top_level.txt
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.534761 va_am-0.1.5/test/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_AutoEncoders.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1232 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_aux_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_io_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_main_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_utils_functions.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.129001 va_am-0.1.6/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.6/LICENSE
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-29 16:01:29.129001 va_am-0.1.6/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.6/README.md
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-05-29 16:00:07.000000 va_am-0.1.6/pyproject.toml
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-05-29 16:01:29.129001 va_am-0.1.6/setup.cfg
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.6/setup.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.125001 va_am-0.1.6/src/
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.125001 va_am-0.1.6/src/va_am/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.6/src/va_am/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.6/src/va_am/__main__.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.129001 va_am-0.1.6/src/va_am/utils/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    60986 2024-05-20 13:28:39.000000 va_am-0.1.6/src/va_am/utils/AutoEncoders.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.6/src/va_am/utils/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.6/src/va_am/utils/functions.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)   104327 2024-05-29 16:00:07.000000 va_am-0.1.6/src/va_am/va_am.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.129001 va_am-0.1.6/src/va_am.egg-info/
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      517 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/entry_points.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/requires.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/top_level.txt
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.129001 va_am-0.1.6/test/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_AutoEncoders.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1232 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_aux_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_io_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_main_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_utils_functions.py
```

### Comparing `va_am-0.1.5/LICENSE` & `va_am-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `va_am-0.1.5/PKG-INFO` & `va_am-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.5
+Version: 0.1.6
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `va_am-0.1.5/README.md` & `va_am-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `va_am-0.1.5/pyproject.toml` & `va_am-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "va_am"
-version = "0.1.5"
+version = "0.1.6"
 authors = [{name="cosminmarina", email="cosmin.marina@uah.es" }]
 description = "VA-AM method implementation"
 readme = "README.md"
 dependencies = ["requests","sympy","keras","tensorflow","xarray","netcdf4","matplotlib","pandas","numpy"]
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `va_am-0.1.5/src/va_am/utils/AutoEncoders.py` & `va_am-0.1.6/src/va_am/utils/AutoEncoders.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.5/src/va_am/utils/functions.py` & `va_am-0.1.6/src/va_am/utils/functions.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.5/src/va_am/va_am.py` & `va_am-0.1.6/src/va_am/va_am.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,34 +271,28 @@
     if is_not_encoded:
         selected_psr = prsf[idx,:,:,:]
     else:
         selected_psr = prsf[idx,:]
 
     return selected_psr, selected_temp, selected_time
 
-def calculate_interest_region(interest_region: Union[list, np.ndarray], latitude_min: int, latitude_max: int, longitude_min: int, longitude_max: int, resolution: Union[int, float] = 2, is_teleg: bool = False, secret_file:str = './secret.txt') -> list:
+def calculate_interest_region(interest_region: Union[list, np.ndarray], dims_list: int, resolution: Union[int, float, str] = 2, is_teleg: bool = False, secret_file:str = './secret.txt') -> list:
     """
       calculate_interest_region
        
       Method which transform latitude/longitude degrees to index. It is used to increase the speed of the methods by using numpy arrays insted of Dataset or DataArray.
         
       Parameters
       ----------
       interest_region: list or ndarray
           List which contains the latitude and longitude degrees to be converted as index. 
-      latitude_min: int
-          The latitude minimum limit.
-      latitude_max: int
-          The latitude maximum limit.
-      longitude_min: int
-          The longitude minimum limit.
-      longitude_max: int
-          The longitude maximum limit.
-      resolution: int or float
-          Degrees resolution employed. Default value is 2º.
+      dims_list: list of int
+          List that contain, in this order, the minimum latitude, maximum latitude, minumin longitude, maximum longitude. When resolution is 'auto', dims_list should be a tuple with (latitude, longitude).
+      resolution: int, float or str
+          Degrees resolution employed. Default value is 2º. If resolution is 'auto' it will infer automatically the resolution (useful when resolution is not constant along the dimensions)
       is_teleg: bool
           Flag that indicate if the warnings have to be sent to Telegram or not.
       secret_file: str
           Auxiliar variable only needed if is_teleg True to read token and chat_id values.
         
       Returns
       ----------
@@ -310,35 +304,44 @@
     if is_teleg:
         with open(secret_file) as f:
             token = f.readline().strip()
             chat_id = f.readline().strip()
             user_name = f.readline().strip()
         f.close()
 
-    value_list = [latitude_min, latitude_max, longitude_min, longitude_max]
-    new_interest_region = []
-    for idx, elem in enumerate(interest_region):
-        if idx%2==0:
-            if elem < value_list[idx]:
-                message = 'Your interest region is out of lat or lon minimum limits. I correct it, but be aware'
-                if is_teleg:
-                    url = f"https://api.telegram.org/bot{token}/sendMessage?chat_id={chat_id}&text={'[WARN]: '+message}"
-                    requests.get(url).json()
-                warnings.warn(message, stacklevel=2)
-            new_elem = int(max((elem - value_list[idx]) // resolution, 0))
-            new_interest_region.append(new_elem)
-        else:
-            if elem > value_list[idx]:
-                message = 'Your interest region is out of lat or lon maximum limits. I correct it, but be aware'
-                if is_teleg:
-                    url = f"https://api.telegram.org/bot{token}/sendMessage?chat_id={chat_id}&text={'[WARN]: '+message}"
-                    requests.get(url).json()
-                warnings.warn(message, stacklevel=2)
-            new_elem = int(min((elem - value_list[idx-1]) // resolution , (value_list[idx] - value_list[idx-1]) // resolution) + 1)
-            new_interest_region.append(new_elem)
+    
+    if resolution=='auto':
+        new_interest_region = np.zeros(4)
+        lat, lon = dims_list
+        new_interest_region[0] = np.where(np.isclose(interest_region[0], lat))[0][0]
+        new_interest_region[1] = np.where(np.isclose(interest_region[1], lat))[0][0]
+        new_interest_region[2] = np.where(np.isclose(interest_region[2], lon))[0][0]
+        new_interest_region[3] = np.where(np.isclose(interest_region[3], lon))[0][0] + 1
+        new_interest_region = new_interest_region.astype(int).tolist()
+    else:
+        new_interest_region = []
+        for idx, elem in enumerate(interest_region):
+            if idx%2==0:
+                if elem < dims_list[idx]:
+                    message = 'Your interest region is out of lat or lon minimum limits. I correct it, but be aware'
+                    if is_teleg:
+                        url = f"https://api.telegram.org/bot{token}/sendMessage?chat_id={chat_id}&text={'[WARN]: '+message}"
+                        requests.get(url).json()
+                    warnings.warn(message, stacklevel=2)
+                new_elem = int(max((elem - dims_list[idx]) // resolution, 0))
+                new_interest_region.append(new_elem)
+            else:
+                if elem > dims_list[idx]:
+                    message = 'Your interest region is out of lat or lon maximum limits. I correct it, but be aware'
+                    if is_teleg:
+                        url = f"https://api.telegram.org/bot{token}/sendMessage?chat_id={chat_id}&text={'[WARN]: '+message}"
+                        requests.get(url).json()
+                    warnings.warn(message, stacklevel=2)
+                new_elem = int(min((elem - dims_list[idx-1]) // resolution , (dims_list[idx] - dims_list[idx-1]) // resolution) + 1)
+                new_interest_region.append(new_elem)
     return new_interest_region
 
 def save_reconstruction(params: dict, reconstructions_Pre_Analog: list, reconstructions_Post_Analog: list, reconstructions_Pre_AE: list, reconstructions_Post_AE: list):
     """
       save_reconstruction
        
       Method that save the target reconstruction based on the runs maded. It do not return anything, only save the Xarray Datasets on the corresponding file on data folder. Each file have the format [name]-[period]-[method]-[time].nc.
@@ -789,15 +792,18 @@
         print(f'len AE: {len(encoded)}')
         print(f'len th AE: {len(encoded[encoded < (encoded.mean() - 0.3*encoded.std())])}')
 
     ## Time and interest region
     current = datetime.datetime.now()
     int_reg = params["interest_region"]
     if params["interest_region_type"] == "coord":
-        int_reg = calculate_interest_region(params["interest_region"], params["latitude_min"], params["latitude_max"], params["longitude_min"], params["longitude_max"], params["resolution"], is_teleg, params["secret_file"])
+        if params["resolution"] == 'auto':
+            int_reg = calculate_interest_region(params["interest_region"], (data_temp.latitude.data, data_temp.longitude.data), params["resolution"], is_teleg, params["secret_file"])
+        else:
+            int_reg = calculate_interest_region(params["interest_region"], [params["latitude_min"], params["latitude_max"], params["longitude_min"], params["longitude_max"]], params["resolution"], is_teleg, params["secret_file"])
 
     print(f'int_reg:\n{int_reg}\n')
     ## This is the threshold of difference between driver/predictor maps and target
     ## to be acepted as low difference
     ## Only used for the local proximity of enhanced distance
     threshold = 0
     threshold_AE = 0
@@ -946,15 +952,18 @@
     data_temp = data_temp.sel(latitude=slice(params["latitude_min"],params["latitude_max"]),longitude=slice(params["longitude_min"],params["longitude_max"]))
     
     time_x = data_temp.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"])).get_index('time')
 
     ## Extract interest data
     idx_interest = params["interest_region"]
     if params["interest_region_type"] == "coord":
-        idx_interest = calculate_interest_region(params["interest_region"], params["latitude_min"], params["latitude_max"], params["longitude_min"], params["longitude_max"], params["resolution"], params["teleg"], params["secret_file"])
+        if params["resolution"] == 'auto':
+            idx_interest = calculate_interest_region(params["interest_region"], (data_temp.latitude.data, data_temp.longitude.data), params["resolution"], params["teleg"], params["secret_file"])
+        else:
+            idx_interest = calculate_interest_region(params["interest_region"], [params["latitude_min"], params["latitude_max"], params["longitude_min"], params["longitude_max"]], params["resolution"], params["teleg"], params["secret_file"])
     data_temp = data_temp.isel(latitude=slice(idx_interest[0], idx_interest[1]),longitude=slice(idx_interest[2], idx_interest[3]))
     data_temp = data_temp.mean(dim=['latitude', 'longitude'])
     
     
     ## Percentil
     which_percentile = 90
     if "percentile" in params.keys():
@@ -1116,17 +1125,17 @@
                 heatwave_period = identify_heatwave_days(params_multiple)
                 params_multiple["data_of_interest_init"] = heatwave_period
                 params_multiple["data_of_interest_end"] = heatwave_period
             else:
                 if params_multiple["per_what"] == "per_month":
                     heatwave_period = (pd.date_range(start=params_multiple["data_of_interest_init"], end=params_multiple["data_of_interest_end"], freq='MS')).to_numpy()
                 elif params_multiple["per_what"] == "per_week":
-                    heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d'), datetime.timedelta(weeks=1))
+                    heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d')+datetime.timedelta(days=1), datetime.timedelta(weeks=1))
                 else:
-                    heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d'), datetime.timedelta(days=1))
+                    heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d')+datetime.timedelta(days=1), datetime.timedelta(days=1))
                 heatwave_period = np.array(list(map(pd.Timestamp, heatwave_period)))
                 params_multiple["data_of_interest_init"] = heatwave_period
                 params_multiple["data_of_interest_end"] = heatwave_period
             params = params_multiple.copy()
             file_params.close()
         if verb is not None:
             params["verbose"] = verb
@@ -1424,17 +1433,17 @@
                 heatwave_period = identify_heatwave_days(params_multiple)
                 params_multiple["data_of_interest_init"] = heatwave_period
                 params_multiple["data_of_interest_end"] = heatwave_period
             else:
                 if params_multiple["per_what"] == "per_month":
                     heatwave_period = (pd.date_range(start=params_multiple["data_of_interest_init"], end=params_multiple["data_of_interest_end"], freq='MS')).to_numpy()
                 elif params_multiple["per_what"] == "per_week":
-                    heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d'), datetime.timedelta(weeks=1))
+                    heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d')+datetime.timedelta(days=1), datetime.timedelta(weeks=1))
                 else:
-                    heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d'), datetime.timedelta(days=1))
+                    heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d')+datetime.timedelta(days=1), datetime.timedelta(days=1))
                 heatwave_period = np.array(list(map(pd.Timestamp, heatwave_period)))
                 params_multiple["data_of_interest_init"] = heatwave_period
                 params_multiple["data_of_interest_end"] = heatwave_period
             params = params_multiple.copy()
             file_params.close()
         if verb is not None:
             params["verbose"] = verb
```

### Comparing `va_am-0.1.5/src/va_am.egg-info/PKG-INFO` & `va_am-0.1.6/src/va_am.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.5
+Version: 0.1.6
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `va_am-0.1.5/src/va_am.egg-info/SOURCES.txt` & `va_am-0.1.6/src/va_am.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `va_am-0.1.5/test/test_aux_va_am.py` & `va_am-0.1.6/test/test_aux_va_am.py`

 * *Files identical despite different names*

