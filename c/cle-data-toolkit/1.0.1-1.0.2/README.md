# Comparing `tmp/cle-data-toolkit-1.0.1.tar.gz` & `tmp/cle_data_toolkit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cle-data-toolkit-1.0.1.tar", last modified: Thu Mar 28 17:28:05 2024, max compression
+gzip compressed data, was "cle_data_toolkit-1.0.2.tar", last modified: Wed May 29 20:21:04 2024, max compression
```

## Comparing `cle-data-toolkit-1.0.1.tar` & `cle_data_toolkit-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:28:05.867900 cle-data-toolkit-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-28 17:28:01.000000 cle-data-toolkit-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23801 2024-03-28 17:28:05.867900 cle-data-toolkit-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23080 2024-03-28 17:28:01.000000 cle-data-toolkit-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-28 17:28:01.000000 cle-data-toolkit-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:28:05.867900 cle-data-toolkit-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:28:05.863900 cle-data-toolkit-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:28:05.867900 cle-data-toolkit-1.0.1/src/cle_data_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23801 2024-03-28 17:28:05.000000 cle-data-toolkit-1.0.1/src/cle_data_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-28 17:28:05.000000 cle-data-toolkit-1.0.1/src/cle_data_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:28:05.000000 cle-data-toolkit-1.0.1/src/cle_data_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 17:28:05.000000 cle-data-toolkit-1.0.1/src/cle_data_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 17:28:05.000000 cle-data-toolkit-1.0.1/src/cle_data_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:28:05.867900 cle-data-toolkit-1.0.1/src/cledatatoolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-28 17:28:01.000000 cle-data-toolkit-1.0.1/src/cledatatoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-03-28 17:28:01.000000 cle-data-toolkit-1.0.1/src/cledatatoolkit/ago_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-28 17:28:01.000000 cle-data-toolkit-1.0.1/src/cledatatoolkit/census.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-28 17:28:01.000000 cle-data-toolkit-1.0.1/src/cledatatoolkit/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-03-28 17:28:01.000000 cle-data-toolkit-1.0.1/src/cledatatoolkit/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:04.146172 cle_data_toolkit-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 20:21:00.000000 cle_data_toolkit-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26683 2024-05-29 20:21:04.146172 cle_data_toolkit-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25892 2024-05-29 20:21:00.000000 cle_data_toolkit-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-29 20:21:00.000000 cle_data_toolkit-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:21:04.146172 cle_data_toolkit-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:04.146172 cle_data_toolkit-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:04.146172 cle_data_toolkit-1.0.2/src/cle_data_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26683 2024-05-29 20:21:04.000000 cle_data_toolkit-1.0.2/src/cle_data_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-29 20:21:04.000000 cle_data_toolkit-1.0.2/src/cle_data_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:21:04.000000 cle_data_toolkit-1.0.2/src/cle_data_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 20:21:04.000000 cle_data_toolkit-1.0.2/src/cle_data_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 20:21:04.000000 cle_data_toolkit-1.0.2/src/cle_data_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:04.146172 cle_data_toolkit-1.0.2/src/cledatatoolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-29 20:21:00.000000 cle_data_toolkit-1.0.2/src/cledatatoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-05-29 20:21:00.000000 cle_data_toolkit-1.0.2/src/cledatatoolkit/ago_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-29 20:21:00.000000 cle_data_toolkit-1.0.2/src/cledatatoolkit/census.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-29 20:21:00.000000 cle_data_toolkit-1.0.2/src/cledatatoolkit/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-29 20:21:00.000000 cle_data_toolkit-1.0.2/src/cledatatoolkit/spatial.py
```

### Comparing `cle-data-toolkit-1.0.1/LICENSE` & `cle_data_toolkit-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cle-data-toolkit-1.0.1/PKG-INFO` & `cle_data_toolkit-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: cle-data-toolkit
-Version: 1.0.1
+Version: 1.0.2
 Summary: A project developed by the City of Cleveland Office of Urban Analytics and Innovation, built to simplify civic data processing for the public.
 Author-email: Shelley Murphy <smurphy3@clevelandohio.gov>, Sam Martinez <smartinez2@clevelandohio.gov>, Dro Sohrabian <dsohrabian@clevelandohio.gov>
 Project-URL: Homepage, https://github.com/City-of-Cleveland/cledatatoolkit/
 Project-URL: Issues, https://github.com/City-of-Cleveland/cledatatoolkit/issues
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: pandas
-Requires-Dist: requests
+Requires-Dist: requests==2.31.0
 Requires-Dist: ipykernel
-Requires-Dist: arcgis
+Requires-Dist: arcgis==2.2.0
+Requires-Dist: libpysal
+Requires-Dist: dask[dataframe]
 
 <p align="center"><img src="branding/logo.svg"></img></p>
 
 # cledatatoolkit
 ...is a library of tools published by the City of Cleveland's [Office of Urban Analytics & Innovation](https://www.clevelandohio.gov/city-hall/office-mayor/urban-ai) (Urban AI). The package is meant for civic data analysis using local, county and regional data sources. Many city datasets can be found using the City of Cleveland [Open Data Portal](https://data.clevelandohio.gov).
 
 This package is divided into a series of modules. These modules can be used to perform a variety of functions, but are not necessarily related to one another. To learn more about what each module does, please visit the [Documentation](#documentation) section.
@@ -83,14 +85,16 @@
 * [`Regular Expression Library`](#cledatatoolkitproperty-regular-expression-library)
 
 [`cledatatoolkit.spatial`](#cledatatoolkitspatial-module) module
 * [`largest_overlap()`](#cledatatoolkitspatiallargest_overlap)
 * [`fix_missing_sjoins()`](#cledatatoolkitspatialfix_missing_sjoins)
 * [`build_aggregator()`](#cledatatoolkitspatialbuild_aggregator)
 * [`apportion()`](#cledatatoolkitspatialapportion)
+* [`optimal_single_location()`](#cledatatoolkitspatialoptimal_single_location)
+* [`apportion()`](#cledatatoolkitspatialarcgis_query_to_geodataframe)
 
 ### `cledatatoolkit.ago_helpers` module
 
 #### `cledatatoolkit.ago_helpers.FLCWrapper(layer_id, container_id, gis)`
 >FLCWrapper stands for FeatureLayerCollection Wrapper. This is a class that contains various "quality of life" functions for working with the ArcGIS Online API, specifically FeatureLayerCollections. FeatureLayerCollections are FeatureServices that contain one or more FeatureLayers.
 
 ***Parameters:***
@@ -366,10 +370,43 @@
 * `group_key` (*str*): The ID field of the `right` dataframe.
 * `target_key` (*str*): The ID field of the `left` dataframe.
 * `aggregator` (*str*): A dictionary of aggregation rules for each column in the `left` dataframe. This can be built with `build_aggregator`
 
 ***Returns:***  
 GeoDataFrame: An apportioned GeoDataFrame, containing all fields from `right`, and aggregated fields from `left`.
 
+#### `cledatatoolkit.spatial.optimal_single_location()`
+
+Given a point GeoDataFrame that represents a limited resource of interest, and a polygon GeoDataFrame of target areas with numeric attributes (like by population), this function returns the one target area that will increase access to that POI the most if you added a POI there.
+
+It does this based on spatial proximity you provide in `search_distance` the and weight column (summed).
+
+For example, if you wanted to know which single location in the City would most increase the number of people within 1/2 a mile to ice cream shops, you would pass ice cream point locations to `poi_gdf`,  population data (Census areas) as `targeted_areas`, pass total population column to `weight_col`, and enter search distance (assuming feet, 2640). See below for description of results.
+
+***Parameters:***  
+* `poi_gdf` (*gpd.GeoDataFrame*): The points of interest that you're seeking to maximize access to
+* `targeted_areas` (*gpd.GeoDataFrame*): The reference geographies, ideally census blocks, block groups, or points
+* `targeted_col` (*str*): The column of interest, typically number of people or things you seek to maximize
+* `search_distance` (*int*): Threshold for measuring "access" in feet as the crow flies to center of the area
+* `method`: (*str*):
+    * "brute" will check every candidate area by generating a buffer from its center, checking for overlap, and summing targeted metric column
+    * "clustered" will use libpysal to generate a list of edge neighbors, and sum total impact based on those neighboring clusters. This method guarantees that all target areas that gain access are contiguous.
+
+***Returns:***  
+*dict*: Returns three key dictionary with the following keys.
+* "optimal_idx": *list*, single index value from targeted_areas that is the optimal location for maximum gain
+* "added": *list*, all index values added, optimal + its neighbors according to the method
+* "total_gain": *int*, the total sum of your
+
+You can pass the lists to `.loc()` method of the original dataframe as needed. Use "optimal_idx" index values to map the specific optimum location. Use "added" indexes to show all newly served tracts, including the optimum.
+
+#### `cledatatoolkit.spatial.arcgisquery_to_geodataframe()`
+***Parameters:***  
+* `query_result` (*arcgis.features.FeatureSet*): FeatureSet from a .query() call. Typically the all the data froma service.
+* `crs` (*str*): Optional, EPSG id for the coordinate system of the data source. Needed only if the service isn't noting in query result.
+
+***Returns:***  
+geopandas.GeoDataFrame: GeoDataFrame of the query with validated geometries, ready to use.
+
 ## Additional Resources
 ### Guide
 See our tutorial notebook repo, [**open-data-examples**](https://github.com/City-of-Cleveland/open-data-examples), for curated tutorials of how you might use this package with Cleveland civic data sources!
```

### Comparing `cle-data-toolkit-1.0.1/README.md` & `cle_data_toolkit-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 * [`Regular Expression Library`](#cledatatoolkitproperty-regular-expression-library)
 
 [`cledatatoolkit.spatial`](#cledatatoolkitspatial-module) module
 * [`largest_overlap()`](#cledatatoolkitspatiallargest_overlap)
 * [`fix_missing_sjoins()`](#cledatatoolkitspatialfix_missing_sjoins)
 * [`build_aggregator()`](#cledatatoolkitspatialbuild_aggregator)
 * [`apportion()`](#cledatatoolkitspatialapportion)
+* [`optimal_single_location()`](#cledatatoolkitspatialoptimal_single_location)
+* [`apportion()`](#cledatatoolkitspatialarcgis_query_to_geodataframe)
 
 ### `cledatatoolkit.ago_helpers` module
 
 #### `cledatatoolkit.ago_helpers.FLCWrapper(layer_id, container_id, gis)`
 >FLCWrapper stands for FeatureLayerCollection Wrapper. This is a class that contains various "quality of life" functions for working with the ArcGIS Online API, specifically FeatureLayerCollections. FeatureLayerCollections are FeatureServices that contain one or more FeatureLayers.
 
 ***Parameters:***
@@ -350,10 +352,43 @@
 * `group_key` (*str*): The ID field of the `right` dataframe.
 * `target_key` (*str*): The ID field of the `left` dataframe.
 * `aggregator` (*str*): A dictionary of aggregation rules for each column in the `left` dataframe. This can be built with `build_aggregator`
 
 ***Returns:***  
 GeoDataFrame: An apportioned GeoDataFrame, containing all fields from `right`, and aggregated fields from `left`.
 
+#### `cledatatoolkit.spatial.optimal_single_location()`
+
+Given a point GeoDataFrame that represents a limited resource of interest, and a polygon GeoDataFrame of target areas with numeric attributes (like by population), this function returns the one target area that will increase access to that POI the most if you added a POI there.
+
+It does this based on spatial proximity you provide in `search_distance` the and weight column (summed).
+
+For example, if you wanted to know which single location in the City would most increase the number of people within 1/2 a mile to ice cream shops, you would pass ice cream point locations to `poi_gdf`,  population data (Census areas) as `targeted_areas`, pass total population column to `weight_col`, and enter search distance (assuming feet, 2640). See below for description of results.
+
+***Parameters:***  
+* `poi_gdf` (*gpd.GeoDataFrame*): The points of interest that you're seeking to maximize access to
+* `targeted_areas` (*gpd.GeoDataFrame*): The reference geographies, ideally census blocks, block groups, or points
+* `targeted_col` (*str*): The column of interest, typically number of people or things you seek to maximize
+* `search_distance` (*int*): Threshold for measuring "access" in feet as the crow flies to center of the area
+* `method`: (*str*):
+    * "brute" will check every candidate area by generating a buffer from its center, checking for overlap, and summing targeted metric column
+    * "clustered" will use libpysal to generate a list of edge neighbors, and sum total impact based on those neighboring clusters. This method guarantees that all target areas that gain access are contiguous.
+
+***Returns:***  
+*dict*: Returns three key dictionary with the following keys.
+* "optimal_idx": *list*, single index value from targeted_areas that is the optimal location for maximum gain
+* "added": *list*, all index values added, optimal + its neighbors according to the method
+* "total_gain": *int*, the total sum of your
+
+You can pass the lists to `.loc()` method of the original dataframe as needed. Use "optimal_idx" index values to map the specific optimum location. Use "added" indexes to show all newly served tracts, including the optimum.
+
+#### `cledatatoolkit.spatial.arcgisquery_to_geodataframe()`
+***Parameters:***  
+* `query_result` (*arcgis.features.FeatureSet*): FeatureSet from a .query() call. Typically the all the data froma service.
+* `crs` (*str*): Optional, EPSG id for the coordinate system of the data source. Needed only if the service isn't noting in query result.
+
+***Returns:***  
+geopandas.GeoDataFrame: GeoDataFrame of the query with validated geometries, ready to use.
+
 ## Additional Resources
 ### Guide
 See our tutorial notebook repo, [**open-data-examples**](https://github.com/City-of-Cleveland/open-data-examples), for curated tutorials of how you might use this package with Cleveland civic data sources!
```

### Comparing `cle-data-toolkit-1.0.1/pyproject.toml` & `cle_data_toolkit-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cle-data-toolkit"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Shelley Murphy", email="smurphy3@clevelandohio.gov"},
   { name="Sam Martinez", email="smartinez2@clevelandohio.gov"},
   { name="Dro Sohrabian", email="dsohrabian@clevelandohio.gov"}
 ]
 description="A project developed by the City of Cleveland Office of Urban Analytics and Innovation, built to simplify civic data processing for the public."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 dependencies = [
   "geopandas",
   "pandas",
-  "requests",
+  "requests==2.31.0",
   "ipykernel",
-  "arcgis"
+  "arcgis==2.2.0",
+  "libpysal",
+  "dask[dataframe]"
 ]
 
 [project.urls]
 Homepage="https://github.com/City-of-Cleveland/cledatatoolkit/"
 Issues="https://github.com/City-of-Cleveland/cledatatoolkit/issues"
```

### Comparing `cle-data-toolkit-1.0.1/src/cle_data_toolkit.egg-info/PKG-INFO` & `cle_data_toolkit-1.0.2/src/cle_data_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: cle-data-toolkit
-Version: 1.0.1
+Version: 1.0.2
 Summary: A project developed by the City of Cleveland Office of Urban Analytics and Innovation, built to simplify civic data processing for the public.
 Author-email: Shelley Murphy <smurphy3@clevelandohio.gov>, Sam Martinez <smartinez2@clevelandohio.gov>, Dro Sohrabian <dsohrabian@clevelandohio.gov>
 Project-URL: Homepage, https://github.com/City-of-Cleveland/cledatatoolkit/
 Project-URL: Issues, https://github.com/City-of-Cleveland/cledatatoolkit/issues
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: pandas
-Requires-Dist: requests
+Requires-Dist: requests==2.31.0
 Requires-Dist: ipykernel
-Requires-Dist: arcgis
+Requires-Dist: arcgis==2.2.0
+Requires-Dist: libpysal
+Requires-Dist: dask[dataframe]
 
 <p align="center"><img src="branding/logo.svg"></img></p>
 
 # cledatatoolkit
 ...is a library of tools published by the City of Cleveland's [Office of Urban Analytics & Innovation](https://www.clevelandohio.gov/city-hall/office-mayor/urban-ai) (Urban AI). The package is meant for civic data analysis using local, county and regional data sources. Many city datasets can be found using the City of Cleveland [Open Data Portal](https://data.clevelandohio.gov).
 
 This package is divided into a series of modules. These modules can be used to perform a variety of functions, but are not necessarily related to one another. To learn more about what each module does, please visit the [Documentation](#documentation) section.
@@ -83,14 +85,16 @@
 * [`Regular Expression Library`](#cledatatoolkitproperty-regular-expression-library)
 
 [`cledatatoolkit.spatial`](#cledatatoolkitspatial-module) module
 * [`largest_overlap()`](#cledatatoolkitspatiallargest_overlap)
 * [`fix_missing_sjoins()`](#cledatatoolkitspatialfix_missing_sjoins)
 * [`build_aggregator()`](#cledatatoolkitspatialbuild_aggregator)
 * [`apportion()`](#cledatatoolkitspatialapportion)
+* [`optimal_single_location()`](#cledatatoolkitspatialoptimal_single_location)
+* [`apportion()`](#cledatatoolkitspatialarcgis_query_to_geodataframe)
 
 ### `cledatatoolkit.ago_helpers` module
 
 #### `cledatatoolkit.ago_helpers.FLCWrapper(layer_id, container_id, gis)`
 >FLCWrapper stands for FeatureLayerCollection Wrapper. This is a class that contains various "quality of life" functions for working with the ArcGIS Online API, specifically FeatureLayerCollections. FeatureLayerCollections are FeatureServices that contain one or more FeatureLayers.
 
 ***Parameters:***
@@ -366,10 +370,43 @@
 * `group_key` (*str*): The ID field of the `right` dataframe.
 * `target_key` (*str*): The ID field of the `left` dataframe.
 * `aggregator` (*str*): A dictionary of aggregation rules for each column in the `left` dataframe. This can be built with `build_aggregator`
 
 ***Returns:***  
 GeoDataFrame: An apportioned GeoDataFrame, containing all fields from `right`, and aggregated fields from `left`.
 
+#### `cledatatoolkit.spatial.optimal_single_location()`
+
+Given a point GeoDataFrame that represents a limited resource of interest, and a polygon GeoDataFrame of target areas with numeric attributes (like by population), this function returns the one target area that will increase access to that POI the most if you added a POI there.
+
+It does this based on spatial proximity you provide in `search_distance` the and weight column (summed).
+
+For example, if you wanted to know which single location in the City would most increase the number of people within 1/2 a mile to ice cream shops, you would pass ice cream point locations to `poi_gdf`,  population data (Census areas) as `targeted_areas`, pass total population column to `weight_col`, and enter search distance (assuming feet, 2640). See below for description of results.
+
+***Parameters:***  
+* `poi_gdf` (*gpd.GeoDataFrame*): The points of interest that you're seeking to maximize access to
+* `targeted_areas` (*gpd.GeoDataFrame*): The reference geographies, ideally census blocks, block groups, or points
+* `targeted_col` (*str*): The column of interest, typically number of people or things you seek to maximize
+* `search_distance` (*int*): Threshold for measuring "access" in feet as the crow flies to center of the area
+* `method`: (*str*):
+    * "brute" will check every candidate area by generating a buffer from its center, checking for overlap, and summing targeted metric column
+    * "clustered" will use libpysal to generate a list of edge neighbors, and sum total impact based on those neighboring clusters. This method guarantees that all target areas that gain access are contiguous.
+
+***Returns:***  
+*dict*: Returns three key dictionary with the following keys.
+* "optimal_idx": *list*, single index value from targeted_areas that is the optimal location for maximum gain
+* "added": *list*, all index values added, optimal + its neighbors according to the method
+* "total_gain": *int*, the total sum of your
+
+You can pass the lists to `.loc()` method of the original dataframe as needed. Use "optimal_idx" index values to map the specific optimum location. Use "added" indexes to show all newly served tracts, including the optimum.
+
+#### `cledatatoolkit.spatial.arcgisquery_to_geodataframe()`
+***Parameters:***  
+* `query_result` (*arcgis.features.FeatureSet*): FeatureSet from a .query() call. Typically the all the data froma service.
+* `crs` (*str*): Optional, EPSG id for the coordinate system of the data source. Needed only if the service isn't noting in query result.
+
+***Returns:***  
+geopandas.GeoDataFrame: GeoDataFrame of the query with validated geometries, ready to use.
+
 ## Additional Resources
 ### Guide
 See our tutorial notebook repo, [**open-data-examples**](https://github.com/City-of-Cleveland/open-data-examples), for curated tutorials of how you might use this package with Cleveland civic data sources!
```

### Comparing `cle-data-toolkit-1.0.1/src/cledatatoolkit/ago_helpers.py` & `cle_data_toolkit-1.0.2/src/cledatatoolkit/ago_helpers.py`

 * *Files identical despite different names*

### Comparing `cle-data-toolkit-1.0.1/src/cledatatoolkit/census.py` & `cle_data_toolkit-1.0.2/src/cledatatoolkit/census.py`

 * *Files identical despite different names*

### Comparing `cle-data-toolkit-1.0.1/src/cledatatoolkit/property.py` & `cle_data_toolkit-1.0.2/src/cledatatoolkit/property.py`

 * *Files identical despite different names*

