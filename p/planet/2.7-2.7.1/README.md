# Comparing `tmp/planet-2.7.tar.gz` & `tmp/planet-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-w0l3qrjp/planet-2.7.tar", last modified: Tue May 21 17:55:11 2024, max compression
+gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-klwk12g2/planet-2.7.1.tar", last modified: Wed May 29 17:32:07 2024, max compression
```

## Comparing `planet-2.7.tar` & `planet-2.7.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-21 17:54:54.000000 planet-2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-21 17:55:11.000000 planet-2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-21 17:54:54.000000 planet-2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-21 17:54:54.000000 planet-2.7/planet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 17:54:54.000000 planet-2.7/planet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-21 17:54:54.000000 planet-2.7/planet/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)    22507 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-21 17:54:54.000000 planet-2.7/planet/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23066 2024-05-21 17:54:54.000000 planet-2.7/planet/clients/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-21 17:54:54.000000 planet-2.7/planet/clients/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-21 17:54:54.000000 planet-2.7/planet/clients/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-21 17:54:54.000000 planet-2.7/planet/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet/data/
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-21 17:54:54.000000 planet-2.7/planet/data/Feature.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-21 17:54:54.000000 planet-2.7/planet/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-05-21 17:54:54.000000 planet-2.7/planet/data/orders_product_bundle_2023-02-24.json
--rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-05-21 17:54:54.000000 planet-2.7/planet/data_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-21 17:54:54.000000 planet-2.7/planet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-21 17:54:54.000000 planet-2.7/planet/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-21 17:54:54.000000 planet-2.7/planet/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-21 17:54:54.000000 planet-2.7/planet/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-05-21 17:54:54.000000 planet-2.7/planet/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19209 2024-05-21 17:54:54.000000 planet-2.7/planet/order_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-21 17:54:54.000000 planet-2.7/planet/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-21 17:54:54.000000 planet-2.7/planet/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28579 2024-05-21 17:54:54.000000 planet-2.7/planet/subscription_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 17:55:11.000000 planet-2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-21 17:54:54.000000 planet-2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:32:07.000000 planet-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-29 17:31:50.000000 planet-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-29 17:32:07.000000 planet-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-29 17:31:50.000000 planet-2.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:32:07.000000 planet-2.7.1/planet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 17:31:50.000000 planet-2.7.1/planet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 17:31:50.000000 planet-2.7.1/planet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-29 17:31:50.000000 planet-2.7.1/planet/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:32:07.000000 planet-2.7.1/planet/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22507 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-29 17:31:50.000000 planet-2.7.1/planet/cli/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:32:07.000000 planet-2.7.1/planet/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-29 17:31:50.000000 planet-2.7.1/planet/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22981 2024-05-29 17:31:50.000000 planet-2.7.1/planet/clients/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-29 17:31:50.000000 planet-2.7.1/planet/clients/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-29 17:31:50.000000 planet-2.7.1/planet/clients/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-29 17:31:50.000000 planet-2.7.1/planet/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:32:07.000000 planet-2.7.1/planet/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-29 17:31:50.000000 planet-2.7.1/planet/data/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-29 17:31:50.000000 planet-2.7.1/planet/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-05-29 17:31:50.000000 planet-2.7.1/planet/data/orders_product_bundle_2023-02-24.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-05-29 17:31:50.000000 planet-2.7.1/planet/data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-29 17:31:50.000000 planet-2.7.1/planet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-29 17:31:50.000000 planet-2.7.1/planet/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-29 17:31:50.000000 planet-2.7.1/planet/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-29 17:31:50.000000 planet-2.7.1/planet/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-05-29 17:31:50.000000 planet-2.7.1/planet/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19209 2024-05-29 17:31:50.000000 planet-2.7.1/planet/order_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-29 17:31:50.000000 planet-2.7.1/planet/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-29 17:31:50.000000 planet-2.7.1/planet/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28579 2024-05-29 17:31:50.000000 planet-2.7.1/planet/subscription_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:32:07.000000 planet-2.7.1/planet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-29 17:32:07.000000 planet-2.7.1/planet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-29 17:32:07.000000 planet-2.7.1/planet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:32:07.000000 planet-2.7.1/planet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 17:32:07.000000 planet-2.7.1/planet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:32:07.000000 planet-2.7.1/planet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-29 17:32:07.000000 planet-2.7.1/planet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 17:32:07.000000 planet-2.7.1/planet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-29 17:32:07.000000 planet-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-29 17:31:50.000000 planet-2.7.1/setup.py
```

### Comparing `planet-2.7/LICENSE` & `planet-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `planet-2.7/PKG-INFO` & `planet-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.7
+Version: 2.7.1
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.7/README.md` & `planet-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/__init__.py` & `planet-2.7.1/planet/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/auth.py` & `planet-2.7.1/planet/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/auth.py` & `planet-2.7.1/planet/cli/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/cli.py` & `planet-2.7.1/planet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/cmds.py` & `planet-2.7.1/planet/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/collect.py` & `planet-2.7.1/planet/cli/collect.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/data.py` & `planet-2.7.1/planet/cli/data.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/io.py` & `planet-2.7.1/planet/cli/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/options.py` & `planet-2.7.1/planet/cli/options.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/orders.py` & `planet-2.7.1/planet/cli/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/subscriptions.py` & `planet-2.7.1/planet/cli/subscriptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/types.py` & `planet-2.7.1/planet/cli/types.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/cli/validators.py` & `planet-2.7.1/planet/cli/validators.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/clients/__init__.py` & `planet-2.7.1/planet/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/clients/data.py` & `planet-2.7.1/planet/clients/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,19 +109,19 @@
         return f'{self._base_url}{SEARCHES_PATH}'
 
     def _item_url(self, item_type, item_id):
         return f'{self._base_url}/item-types/{item_type}/items/{item_id}'
 
     async def search(self,
                      item_types: List[str],
-                     geometry: Optional[dict] = None,
                      search_filter: Optional[dict] = None,
                      name: Optional[str] = None,
                      sort: Optional[str] = None,
-                     limit: int = 100) -> AsyncIterator[dict]:
+                     limit: int = 100,
+                     geometry: Optional[dict] = None) -> AsyncIterator[dict]:
         """Iterate over results from a quick search.
 
         Quick searches are saved for a short period of time (~month). The
         `name` parameter of the search defaults to the id of the generated
         search id if `name` is not specified.
 
         Note:
@@ -132,18 +132,18 @@
         Parameters:
             item_types: The item types to include in the search.
             search_filter: Structured search criteria to apply. If None,
                 no search criteria is applied.
             sort: Field and direction to order results by. Valid options are
             given in SEARCH_SORT.
             name: The name of the saved search.
-            geometry: GeoJSON, a feature reference or a list of feature
-                references
             limit: Maximum number of results to return. When set to 0, no
                 maximum is applied.
+            geometry: GeoJSON, a feature reference or a list of feature
+                references
 
         Yields:
             Description of an item.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
@@ -169,20 +169,22 @@
         response = await self._session.request(method='POST',
                                                url=url,
                                                json=request_json,
                                                params=params)
         async for i in Items(response, self._session.request, limit=limit):
             yield i
 
-    async def create_search(self,
-                            item_types: List[str],
-                            search_filter: dict,
-                            name: str,
-                            geometry: Optional[dict] = None,
-                            enable_email: bool = False) -> dict:
+    async def create_search(
+        self,
+        item_types: List[str],
+        search_filter: dict,
+        name: str,
+        enable_email: bool = False,
+        geometry: Optional[dict] = None,
+    ) -> dict:
         """Create a new saved structured item search.
 
         To filter to items you have access to download which are of standard
         (aka not test) quality, use the following:
 
         ```python
         >>> from planet import data_filter
@@ -195,18 +197,18 @@
 
         To avoid filtering out any imagery, supply a blank AndFilter, which can
         be created with `data_filter.and_filter([])`.
 
 
         Parameters:
             item_types: The item types to include in the search.
-            geometry: A feature reference or a GeoJSON
             search_filter: Structured search criteria.
             name: The name of the saved search.
             enable_email: Send a daily email when new results are added.
+            geometry: A feature reference or a GeoJSON
 
         Returns:
             Description of the saved search.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
@@ -229,25 +231,25 @@
         return response.json()
 
     async def update_search(self,
                             search_id: str,
                             item_types: List[str],
                             search_filter: dict,
                             name: str,
-                            geometry: Optional[dict] = None,
-                            enable_email: bool = False) -> dict:
+                            enable_email: bool = False,
+                            geometry: Optional[dict] = None) -> dict:
         """Update an existing saved search.
 
         Parameters:
             search_id: Saved search identifier.
             item_types: The item types to include in the search.
-            geometry: A feature reference or a GeoJSON
             search_filter: Structured search criteria.
             name: The name of the saved search.
             enable_email: Send a daily email when new results are added.
+            geometry: A feature reference or a GeoJSON
 
         Returns:
             Description of the saved search.
         """
         url = f'{self._searches_url()}/{search_id}'
 
         item_types = [validate_data_item_type(item) for item in item_types]
```

### Comparing `planet-2.7/planet/clients/orders.py` & `planet-2.7.1/planet/clients/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/clients/subscriptions.py` & `planet-2.7.1/planet/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/constants.py` & `planet-2.7.1/planet/constants.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/data/Feature.json` & `planet-2.7.1/planet/data/Feature.json`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/data/README.md` & `planet-2.7.1/planet/data/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/data/orders_product_bundle_2023-02-24.json` & `planet-2.7.1/planet/data/orders_product_bundle_2023-02-24.json`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/data_filter.py` & `planet-2.7.1/planet/data_filter.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/exceptions.py` & `planet-2.7.1/planet/exceptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/geojson.py` & `planet-2.7.1/planet/geojson.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/http.py` & `planet-2.7.1/planet/http.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/io.py` & `planet-2.7.1/planet/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/models.py` & `planet-2.7.1/planet/models.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/order_request.py` & `planet-2.7.1/planet/order_request.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/reporting.py` & `planet-2.7.1/planet/reporting.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/specs.py` & `planet-2.7.1/planet/specs.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet/subscription_request.py` & `planet-2.7.1/planet/subscription_request.py`

 * *Files identical despite different names*

### Comparing `planet-2.7/planet.egg-info/PKG-INFO` & `planet-2.7.1/planet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.7
+Version: 2.7.1
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.7/planet.egg-info/SOURCES.txt` & `planet-2.7.1/planet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planet-2.7/setup.py` & `planet-2.7.1/setup.py`

 * *Files identical despite different names*

