# Comparing `tmp/sunweg-2.1.1.tar.gz` & `tmp/sunweg-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunweg-2.1.1.tar", last modified: Mon Mar 18 21:41:14 2024, max compression
+gzip compressed data, was "sunweg-3.0.0.tar", last modified: Wed May 29 20:11:10 2024, max compression
```

## Comparing `sunweg-2.1.1.tar` & `sunweg-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:41:14.331138 sunweg-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-18 21:41:05.000000 sunweg-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-18 21:41:14.331138 sunweg-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-18 21:41:05.000000 sunweg-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 21:41:14.331138 sunweg-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-18 21:41:05.000000 sunweg-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:41:14.331138 sunweg-2.1.1/sunweg/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-18 21:41:05.000000 sunweg-2.1.1/sunweg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-03-18 21:41:05.000000 sunweg-2.1.1/sunweg/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-18 21:41:05.000000 sunweg-2.1.1/sunweg/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-03-18 21:41:05.000000 sunweg-2.1.1/sunweg/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-03-18 21:41:05.000000 sunweg-2.1.1/sunweg/plant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-18 21:41:05.000000 sunweg-2.1.1/sunweg/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:41:14.331138 sunweg-2.1.1/sunweg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-18 21:41:14.000000 sunweg-2.1.1/sunweg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-18 21:41:14.000000 sunweg-2.1.1/sunweg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 21:41:14.000000 sunweg-2.1.1/sunweg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-18 21:41:14.000000 sunweg-2.1.1/sunweg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-18 21:41:14.000000 sunweg-2.1.1/sunweg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:41:14.331138 sunweg-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17776 2024-03-18 21:41:05.000000 sunweg-2.1.1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:11:10.202229 sunweg-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-29 20:11:06.000000 sunweg-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-29 20:11:10.202229 sunweg-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-29 20:11:06.000000 sunweg-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:11:10.202229 sunweg-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-29 20:11:06.000000 sunweg-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:11:10.198229 sunweg-3.0.0/sunweg/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 20:11:06.000000 sunweg-3.0.0/sunweg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-29 20:11:06.000000 sunweg-3.0.0/sunweg/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-29 20:11:06.000000 sunweg-3.0.0/sunweg/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-29 20:11:06.000000 sunweg-3.0.0/sunweg/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-29 20:11:06.000000 sunweg-3.0.0/sunweg/plant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-29 20:11:06.000000 sunweg-3.0.0/sunweg/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:11:10.202229 sunweg-3.0.0/sunweg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-29 20:11:10.000000 sunweg-3.0.0/sunweg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-29 20:11:10.000000 sunweg-3.0.0/sunweg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:11:10.000000 sunweg-3.0.0/sunweg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 20:11:10.000000 sunweg-3.0.0/sunweg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 20:11:10.000000 sunweg-3.0.0/sunweg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:11:10.202229 sunweg-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17776 2024-05-29 20:11:06.000000 sunweg-3.0.0/tests/test_api.py
```

### Comparing `sunweg-2.1.1/LICENSE` & `sunweg-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sunweg-2.1.1/PKG-INFO` & `sunweg-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sunweg
-Version: 2.1.1
+Version: 3.0.0
 Summary: A library to retrieve data from sunweg.net
 Home-page: https://github.com/rokam/sunweg
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
 Requires-Dist: requests
 
 # SunWeg
 
 [![Python build](https://github.com/rokam/sunweg/actions/workflows/python-build.yml/badge.svg)](https://github.com/rokam/sunweg/actions/workflows/python-build.yml)
 ![Python tests](https://raw.githubusercontent.com/rokam/sunweg/badges/tests.svg)
 ![Python coverage](https://raw.githubusercontent.com/rokam/sunweg/badges/coverage.svg)
```

### Comparing `sunweg-2.1.1/README.md` & `sunweg-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sunweg-2.1.1/setup.py` & `sunweg-3.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requires = [
+    "python-dateutil",
     "requests",
 ]
 
 setuptools.setup(
     name="sunweg",
-    version="2.1.1",
+    version="3.0.0",
     author="rokam",
     author_email="lucas@mindello.com.br",
     description="A library to retrieve data from sunweg.net",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rokam/sunweg",
```

### Comparing `sunweg-2.1.1/sunweg/api.py` & `sunweg-3.0.0/sunweg/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """API Helper."""
 
 import json
-from datetime import datetime
+from dateutil import parser
 from typing import Any
 
 from requests import Response, session
 
 from .const import (
     SUNWEG_INVERTER_DETAIL_PATH,
     SUNWEG_LOGIN_PATH,
@@ -114,29 +114,29 @@
         """
         Authenticate with provided username and password.
 
         :return: True on authentication success
         :rtype: bool
         """
         user_data = json.dumps(
-            {"usuario": self._username, "senha": self._password},
+            {"usuario": self._username, "senha": self._password, "rememberMe": True},
             default=lambda o: o.__dict__,
         )
 
         result = self._post(SUNWEG_LOGIN_PATH, user_data, False)
         if not result["success"]:
             return False
         self._token = result["token"]
         return result["success"]
 
     def _headers(self):
         """Retrieve headers with authentication token."""
         if self._token is None:
-            return {}
-        return {"X-Auth-Token-Update": self._token}
+            return {"Content-Type": "application/json"}
+        return {"Content-Type": "application/json", "X-Auth-Token-Update": self._token}
 
     def listPlants(self, retry=True) -> list[Plant]:
         """
         Retrieve the list of plants with incomplete inverter information.
 
         You may want to call `complete_inverter()` to complete the Inverter information.
 
@@ -144,15 +144,15 @@
         :type retry: bool
         :return: list of Plant
         :rtype: list[Plant]
         """
         try:
             result = self._get(SUNWEG_PLANT_LIST_PATH)
             ret_list = []
-            for plant in result["usinas"]:
+            for plant in result["conectadas"]:
                 if (plant := self.plant(plant["id"])) is not None:
                     ret_list.append(plant)
             return ret_list
         except LoginError:
             if retry:
                 self.authenticate()
                 return self.listPlants(False)
@@ -169,33 +169,29 @@
         :return: Plant or None if `id` not found.
         :rtype: Plant | None
         """
         try:
             result = self._get(SUNWEG_PLANT_DETAIL_PATH + str(id))
 
             (today_energy, today_energy_metric) = separate_value_metric(
-                result["energiaGeradaHoje"], "kWh"
+                result["energiadia"], "kWh"
             )
             total_power = separate_value_metric(result["AcumuladoPotencia"])[0]
             plant = Plant(
                 id=id,
                 name=result["usinas"]["nome"],
                 total_power=total_power,
-                kwh_per_kwp=float(str(result["KWHporkWp"]).replace(",", "."))
-                if result["KWHporkWp"] != ""
-                else float(0),
-                performance_rate=result["taxaPerformance"],
+                kwh_per_kwp=float(0),
+                performance_rate=float(0),
                 saving=result["economia"],
                 today_energy=today_energy,
                 today_energy_metric=today_energy_metric,
                 total_energy=float(result["energiaacumuladanumber"]),
                 total_carbon_saving=result["reduz_carbono_total_number"],
-                last_update=datetime.strptime(
-                    result["ultimaAtualizacao"], "%Y-%m-%d %H:%M:%S"
-                )
+                last_update=parser.parse(result["ultimaAtualizacao"])
                 if result["ultimaAtualizacao"] is not None
                 else None,
             )
 
             plant.inverters.extend(
                 [
                     Inverter(
@@ -347,15 +343,15 @@
         try:
             result = self._get(
                 SUNWEG_MONTH_STATS_PATH
                 + f"idusina={plant_id}&idinversor={inverter_str}&date={format(month,'02')}/{year}"
             )
             return [
                 ProductionStats(
-                    datetime.strptime(item["tempoatual"], "%Y-%m-%d").date(),
+                    parser.parse(item["tempoatual"]).date(),
                     float(item["energiapordia"]),
                     float(item["prognostico"]),
                 )
                 for item in result["graficomes"]
             ]
         except LoginError:
             if retry:
```

### Comparing `sunweg-2.1.1/sunweg/device.py` & `sunweg-3.0.0/sunweg/device.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.1.1/sunweg/plant.py` & `sunweg-3.0.0/sunweg/plant.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Sunweg API plant."""
 
 from datetime import datetime
+import warnings
 
 from .device import Inverter
 
 
 class Plant:
     """Plant details."""
 
@@ -90,29 +91,41 @@
         :rtype: float
         """
         return self._total_power
 
     @property
     def kwh_per_kwp(self) -> float:
         """
+        Deprecated as API v2 doesn't return it anymore.
         Get plant kWh/kWp.
 
         :return: plant kWh/kWp
         :rtype: float
         """
+        warnings.warn(
+            "The 'kwh_per_kwp' property is deprecated and will return 0.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._kwh_per_kwp
 
     @property
     def performance_rate(self) -> float:
         """
+        Deprecated as API v2 doesn't return it anymore.
         Get plant performance rate.
 
         :return: plant performance rate
         :rtype: float
         """
+        warnings.warn(
+            "The 'performance_rate' property is deprecated and will return 0.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._performance_rate
 
     @property
     def saving(self) -> float:
         """
         Get plant saving in R$.
```

### Comparing `sunweg-2.1.1/sunweg/util.py` & `sunweg-3.0.0/sunweg/util.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.1.1/sunweg.egg-info/PKG-INFO` & `sunweg-3.0.0/sunweg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sunweg
-Version: 2.1.1
+Version: 3.0.0
 Summary: A library to retrieve data from sunweg.net
 Home-page: https://github.com/rokam/sunweg
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
 Requires-Dist: requests
 
 # SunWeg
 
 [![Python build](https://github.com/rokam/sunweg/actions/workflows/python-build.yml/badge.svg)](https://github.com/rokam/sunweg/actions/workflows/python-build.yml)
 ![Python tests](https://raw.githubusercontent.com/rokam/sunweg/badges/tests.svg)
 ![Python coverage](https://raw.githubusercontent.com/rokam/sunweg/badges/coverage.svg)
```

### Comparing `sunweg-2.1.1/tests/test_api.py` & `sunweg-3.0.0/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,16 +163,16 @@
             api = APIHelper("user@acme.com", "password")
             plant = api.plant(16925)
             assert plant is not None
             assert plant.id == 16925
             assert plant.name == "Plant Name"
             assert plant.total_power == 25.23
             assert plant.last_update == datetime(2023, 2, 25, 8, 4, 22)
-            assert plant.kwh_per_kwp == 1.2
-            assert plant.performance_rate == 1.48
+            assert plant.kwh_per_kwp == 0.0
+            assert plant.performance_rate == 0.0
             assert plant.saving == 12.786912
             assert plant.today_energy == 1.23
             assert plant.today_energy_metric == "kWh"
             assert plant.total_carbon_saving == 0.012296
             assert plant.total_energy == 23.2
             assert plant.__str__().startswith("<class 'sunweg.plant.Plant'>")
             assert len(plant.inverters) == 1
@@ -201,16 +201,16 @@
             api = APIHelper("user@acme.com", "password")
             plant = api.plant(16925)
             assert plant is not None
             assert plant.id == 16925
             assert plant.name == "Plant Name"
             assert plant.total_power == 25.23
             assert plant.last_update is None
-            assert plant.kwh_per_kwp == 1.2
-            assert plant.performance_rate == 1.48
+            assert plant.kwh_per_kwp == 0.0
+            assert plant.performance_rate == 0.0
             assert plant.saving == 12.786912
             assert plant.today_energy == 1.23
             assert plant.today_energy_metric == "kWh"
             assert plant.total_carbon_saving == 0.012296
             assert plant.total_energy == 23.2
             assert plant.__str__().startswith("<class 'sunweg.plant.Plant'>")
             assert len(plant.inverters) == 1
@@ -414,14 +414,14 @@
             api = APIHelper("user@acme.com", "password")
             plant = MagicMock()
             plant.id = 1
             stats = api.month_stats_production(2023, 12, plant)
             assert len(stats) > 0
             i: int = 1
             for stat in stats:
-                assert stat.date == date(2023, 12, i)
+                assert stat.date == date(2024, 5, i)
                 assert isinstance(stat.production, float)
-                assert stat.prognostic == 98.774193548387
+                assert stat.prognostic == 111.03225806451613
                 assert stat.__str__().startswith(
                     "<class 'sunweg.util.ProductionStats'>"
                 )
                 i += 1
```

