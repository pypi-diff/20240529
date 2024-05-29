# Comparing `tmp/opower-0.4.5.tar.gz` & `tmp/opower-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opower-0.4.5.tar", last modified: Sun May 12 19:50:10 2024, max compression
+gzip compressed data, was "opower-0.4.6.tar", last modified: Wed May 29 20:50:53 2024, max compression
```

## Comparing `opower-0.4.5.tar` & `opower-0.4.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:10.079658 opower-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 19:50:03.000000 opower-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-12 19:50:10.079658 opower-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-12 19:50:03.000000 opower-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-12 19:50:03.000000 opower-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-12 19:50:10.079658 opower-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:10.071658 opower-0.4.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-12 19:50:03.000000 opower-0.4.5/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:10.071658 opower-0.4.5/src/opower/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/opower.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:10.079658 opower-0.4.5/src/opower/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/aepbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/aepohio.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/aeptexas.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/appalachianpower.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/atlanticcityelectric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/bge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/coautilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/comed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/coned.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/delmarva.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/duquesnelight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/enmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/evergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/exelon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/indianamichiganpower.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/kentuckypower.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/oru.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/peco.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/pepco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/pge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/portlandgeneral.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/pse.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/psoklahoma.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/scl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/smud.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-12 19:50:03.000000 opower-0.4.5/src/opower/utilities/swepco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:10.079658 opower-0.4.5/src/opower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-12 19:50:10.000000 opower-0.4.5/src/opower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-12 19:50:10.000000 opower-0.4.5/src/opower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:50:10.000000 opower-0.4.5/src/opower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 19:50:10.000000 opower-0.4.5/src/opower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 19:50:10.000000 opower-0.4.5/src/opower.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:10.079658 opower-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-12 19:50:03.000000 opower-0.4.5/tests/test_opower.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:50:53.763671 opower-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 20:50:49.000000 opower-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-29 20:50:53.763671 opower-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-29 20:50:49.000000 opower-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-29 20:50:49.000000 opower-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 20:50:53.763671 opower-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:50:53.755670 opower-0.4.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-29 20:50:49.000000 opower-0.4.6/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:50:53.755670 opower-0.4.6/src/opower/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22459 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/opower.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:50:53.763671 opower-0.4.6/src/opower/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/aepbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/aepohio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/aeptexas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/appalachianpower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/atlanticcityelectric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/bge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/coautilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/comed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/coned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/delmarva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/duquesnelight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/enmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/evergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/exelon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/indianamichiganpower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/kentuckypower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/oru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/peco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/pepco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/pge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/portlandgeneral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/psoklahoma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/scl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/smud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 20:50:49.000000 opower-0.4.6/src/opower/utilities/swepco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:50:53.763671 opower-0.4.6/src/opower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-29 20:50:53.000000 opower-0.4.6/src/opower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-29 20:50:53.000000 opower-0.4.6/src/opower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:50:53.000000 opower-0.4.6/src/opower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 20:50:53.000000 opower-0.4.6/src/opower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 20:50:53.000000 opower-0.4.6/src/opower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:50:53.763671 opower-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 20:50:49.000000 opower-0.4.6/tests/test_opower.py
```

### Comparing `opower-0.4.5/LICENSE` & `opower-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/PKG-INFO` & `opower-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8
+Requires-Dist: aiozoneinfo>=0.1
 Requires-Dist: arrow>=1.2
 Requires-Dist: pyotp>=2.0
 Provides-Extra: dev
 Requires-Dist: pytest<8,>=7; extra == "dev"
 Requires-Dist: python-dotenv<2,>=1; extra == "dev"
 
 # opower
```

### Comparing `opower-0.4.5/README.md` & `opower-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/pyproject.toml` & `opower-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "opower"
-version = "0.4.5"
+version = "0.4.6"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "aiohttp>=3.8",
+    "aiozoneinfo>=0.1",
     "arrow>=1.2",
     "pyotp>=2.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tronikos/opower"
 "Bug Tracker" = "https://github.com/tronikos/opower/issues"
```

### Comparing `opower-0.4.5/src/demo.py` & `opower-0.4.6/src/demo.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/__init__.py` & `opower-0.4.6/src/opower/__init__.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/opower.py` & `opower-0.4.6/src/opower/opower.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import json
 import logging
 from typing import Any, Optional, Union
 from urllib.parse import urlencode
 
 import aiohttp
 from aiohttp.client_exceptions import ClientResponseError
+import aiozoneinfo
 import arrow
 
 from .const import USER_AGENT
 from .exceptions import CannotConnect, InvalidAuth
 from .utilities import UtilityBase
 
 _LOGGER = logging.getLogger(__file__)
@@ -466,16 +467,17 @@
                 return await self._async_fetch(
                     account, aggregate_type, start_date, end_date, usage_only
                 )
             raise ValueError("start_date is required unless aggregate_type=BILL")
         if end_date is None:
             raise ValueError("end_date is required unless aggregate_type=BILL")
 
-        start = arrow.get(start_date.date(), self.utility.timezone())
-        end = arrow.get(end_date.date(), self.utility.timezone()).shift(days=1)
+        tzinfo = await aiozoneinfo.async_get_time_zone(self.utility.timezone())
+        start = arrow.get(start_date.date(), tzinfo)
+        end = arrow.get(end_date.date(), tzinfo).shift(days=1)
 
         max_request_days = None
         if aggregate_type == AggregateType.DAY:
             max_request_days = 363
         elif aggregate_type == AggregateType.HOUR:
             max_request_days = 26
```

### Comparing `opower-0.4.5/src/opower/utilities/aepbase.py` & `opower-0.4.6/src/opower/utilities/aepbase.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/atlanticcityelectric.py` & `opower-0.4.6/src/opower/utilities/atlanticcityelectric.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/base.py` & `opower-0.4.6/src/opower/utilities/base.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/bge.py` & `opower-0.4.6/src/opower/utilities/bge.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/coautilities.py` & `opower-0.4.6/src/opower/utilities/coautilities.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/comed.py` & `opower-0.4.6/src/opower/utilities/comed.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/coned.py` & `opower-0.4.6/src/opower/utilities/coned.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/delmarva.py` & `opower-0.4.6/src/opower/utilities/delmarva.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/duquesnelight.py` & `opower-0.4.6/src/opower/utilities/duquesnelight.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/enmax.py` & `opower-0.4.6/src/opower/utilities/enmax.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/evergy.py` & `opower-0.4.6/src/opower/utilities/evergy.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/exelon.py` & `opower-0.4.6/src/opower/utilities/exelon.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/helpers.py` & `opower-0.4.6/src/opower/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/oru.py` & `opower-0.4.6/src/opower/utilities/oru.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/peco.py` & `opower-0.4.6/src/opower/utilities/peco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/pepco.py` & `opower-0.4.6/src/opower/utilities/pepco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/pge.py` & `opower-0.4.6/src/opower/utilities/pge.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/portlandgeneral.py` & `opower-0.4.6/src/opower/utilities/portlandgeneral.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/pse.py` & `opower-0.4.6/src/opower/utilities/pse.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/psoklahoma.py` & `opower-0.4.6/src/opower/utilities/psoklahoma.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/scl.py` & `opower-0.4.6/src/opower/utilities/scl.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/smud.py` & `opower-0.4.6/src/opower/utilities/smud.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower/utilities/swepco.py` & `opower-0.4.6/src/opower/utilities/swepco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.5/src/opower.egg-info/PKG-INFO` & `opower-0.4.6/src/opower.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8
+Requires-Dist: aiozoneinfo>=0.1
 Requires-Dist: arrow>=1.2
 Requires-Dist: pyotp>=2.0
 Provides-Extra: dev
 Requires-Dist: pytest<8,>=7; extra == "dev"
 Requires-Dist: python-dotenv<2,>=1; extra == "dev"
 
 # opower
```

### Comparing `opower-0.4.5/src/opower.egg-info/SOURCES.txt` & `opower-0.4.6/src/opower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

