# Comparing `tmp/vgis_gis-1.3.6.tar.gz` & `tmp/vgis_gis-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_gis-1.3.6.tar", last modified: Thu May 23 10:37:20 2024, max compression
+gzip compressed data, was "dist\vgis_gis-1.3.7.tar", last modified: Wed May 29 10:18:13 2024, max compression
```

## Comparing `vgis_gis-1.3.6.tar` & `vgis_gis-1.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 10:37:20.916919 vgis_gis-1.3.6/
--rw-rw-rw-   0        0        0      981 2024-05-23 10:37:20.915896 vgis_gis-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      117 2023-09-25 02:35:06.000000 vgis_gis-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 10:37:20.916919 vgis_gis-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     2189 2024-05-23 10:37:15.000000 vgis_gis-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:37:20.905924 vgis_gis-1.3.6/vgis_gis/
--rw-rw-rw-   0        0        0    10927 2023-12-21 07:26:16.000000 vgis_gis-1.3.6/vgis_gis/PoiTools.py
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_gis-1.3.6/vgis_gis/__init__.py
--rw-rw-rw-   0        0        0     1491 2023-09-25 02:57:23.000000 vgis_gis-1.3.6/vgis_gis/arcgisTools.py
--rw-rw-rw-   0        0        0     3475 2021-08-30 10:03:04.000000 vgis_gis-1.3.6/vgis_gis/coordTools.py
--rw-rw-rw-   0        0        0     5166 2023-12-05 05:41:00.000000 vgis_gis-1.3.6/vgis_gis/geocodeTools.py
--rw-rw-rw-   0        0        0     3909 2024-03-22 01:58:29.000000 vgis_gis-1.3.6/vgis_gis/geojsonTools.py
--rw-rw-rw-   0        0        0    13904 2023-10-27 02:59:01.000000 vgis_gis-1.3.6/vgis_gis/geoserverTools.py
--rw-rw-rw-   0        0        0    24356 2024-05-23 10:37:01.000000 vgis_gis-1.3.6/vgis_gis/gisTools.py
--rw-rw-rw-   0        0        0     2581 2023-06-13 09:19:32.000000 vgis_gis-1.3.6/vgis_gis/projTools.py
--rw-rw-rw-   0        0        0      216 2021-11-05 05:26:50.000000 vgis_gis-1.3.6/vgis_gis/qgisTools.py
--rw-rw-rw-   0        0        0    71648 2024-03-20 07:15:51.000000 vgis_gis-1.3.6/vgis_gis/shpTools.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:37:20.914924 vgis_gis-1.3.6/vgis_gis.egg-info/
--rw-rw-rw-   0        0        0      981 2024-05-23 10:37:20.000000 vgis_gis-1.3.6/vgis_gis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-05-23 10:37:20.000000 vgis_gis-1.3.6/vgis_gis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 10:37:20.000000 vgis_gis-1.3.6/vgis_gis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-23 10:37:20.000000 vgis_gis-1.3.6/vgis_gis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 10:37:20.000000 vgis_gis-1.3.6/vgis_gis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 10:18:13.743740 vgis_gis-1.3.7/
+-rw-rw-rw-   0        0        0      981 2024-05-29 10:18:13.743740 vgis_gis-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2023-09-25 02:35:06.000000 vgis_gis-1.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:18:13.743740 vgis_gis-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2189 2024-05-29 10:17:50.000000 vgis_gis-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:18:13.691768 vgis_gis-1.3.7/vgis_gis/
+-rw-rw-rw-   0        0        0    10927 2023-12-21 07:26:16.000000 vgis_gis-1.3.7/vgis_gis/PoiTools.py
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_gis-1.3.7/vgis_gis/__init__.py
+-rw-rw-rw-   0        0        0     1491 2023-09-25 02:57:23.000000 vgis_gis-1.3.7/vgis_gis/arcgisTools.py
+-rw-rw-rw-   0        0        0     3475 2021-08-30 10:03:04.000000 vgis_gis-1.3.7/vgis_gis/coordTools.py
+-rw-rw-rw-   0        0        0     5166 2023-12-05 05:41:00.000000 vgis_gis-1.3.7/vgis_gis/geocodeTools.py
+-rw-rw-rw-   0        0        0     4671 2024-05-29 10:17:35.000000 vgis_gis-1.3.7/vgis_gis/geojsonTools.py
+-rw-rw-rw-   0        0        0    13904 2023-10-27 02:59:01.000000 vgis_gis-1.3.7/vgis_gis/geoserverTools.py
+-rw-rw-rw-   0        0        0    24356 2024-05-23 10:37:01.000000 vgis_gis-1.3.7/vgis_gis/gisTools.py
+-rw-rw-rw-   0        0        0     2581 2023-06-13 09:19:32.000000 vgis_gis-1.3.7/vgis_gis/projTools.py
+-rw-rw-rw-   0        0        0      216 2021-11-05 05:26:50.000000 vgis_gis-1.3.7/vgis_gis/qgisTools.py
+-rw-rw-rw-   0        0        0    71648 2024-03-20 07:15:51.000000 vgis_gis-1.3.7/vgis_gis/shpTools.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:18:13.708765 vgis_gis-1.3.7/vgis_gis.egg-info/
+-rw-rw-rw-   0        0        0      981 2024-05-29 10:18:13.000000 vgis_gis-1.3.7/vgis_gis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-05-29 10:18:13.000000 vgis_gis-1.3.7/vgis_gis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:18:13.000000 vgis_gis-1.3.7/vgis_gis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-29 10:18:13.000000 vgis_gis-1.3.7/vgis_gis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 10:18:13.000000 vgis_gis-1.3.7/vgis_gis.egg-info/top_level.txt
```

### Comparing `vgis_gis-1.3.6/PKG-INFO` & `vgis_gis-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_gis
-Version: 1.3.6
+Version: 1.3.7
 Summary: A libary for gis operator
 Home-page: https://github.com/gisfanmachel/vgisGis
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Keywords: gis,setuptools,development
 Platform: UNKNOWN
```

### Comparing `vgis_gis-1.3.6/setup.py` & `vgis_gis-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_gis",  # Required 项目名称
-    version="1.3.6",  # Required 发布版本号
+    version="1.3.7",  # Required 发布版本号
 
     description="A libary for gis operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisGis",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
```

### Comparing `vgis_gis-1.3.6/vgis_gis/PoiTools.py` & `vgis_gis-1.3.7/vgis_gis/PoiTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.6/vgis_gis/arcgisTools.py` & `vgis_gis-1.3.7/vgis_gis/arcgisTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.6/vgis_gis/coordTools.py` & `vgis_gis-1.3.7/vgis_gis/coordTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.6/vgis_gis/geocodeTools.py` & `vgis_gis-1.3.7/vgis_gis/geocodeTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.6/vgis_gis/geojsonTools.py` & `vgis_gis-1.3.7/vgis_gis/geojsonTools.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ===================================
 """
 
 import json
 import os
 
 import geopandas as gpd
+from osgeo import gdal, osr, ogr
 
 from vgis_utils.vgis_file.fileTools import FileHelper
 
 
 class GeoJsonHelper:
 
     def __init__(self):
@@ -46,14 +47,33 @@
     @staticmethod
     def convert_geojson_to_shp(geojson_path, shp_path):
         # 读取 GeoJSON 文件
         gdf = gpd.read_file(geojson_path, engine='pyogrio')
         # 保存为 Shapefile
         gdf.to_file(shp_path, driver='ESRI Shapefile', engine='pyogrio')
 
+    @staticmethod
+    def convert_geojson_to_shp2(geojson_path, shp_path):
+        gdal.SetConfigOption("GDAL_FILENAME_IS_UTF8", "YES")
+        gdal.SetConfigOption("SHAPE_ENCODING", "")
+        geojson_ds = ogr.Open(geojson_path, 0)
+        geojson_layer = geojson_ds.GetLayer(0)
+
+        # 创建Shapefile输出数据源
+        driver = ogr.GetDriverByName('ESRI Shapefile')
+        # if driver.Exists(out_shp_file_path):
+        #     driver.DeleteDataSource(out_shp_file_path)
+        shp_ds = driver.CreateDataSource(shp_path)
+
+        # 复制层并转换
+        shp_layer = shp_ds.CopyLayer(geojson_layer, 'shp_layer')
+        # 关闭数据源
+        shp_ds.Destroy()
+        geojson_ds.Destroy()
+
     # geojson里增加epsg
     @staticmethod
     def add_epsg_value_in_geojson(geojson_path, espg_value):
         encoding = FileHelper.get_file_encoding(geojson_path)
         data = json.load(open(geojson_path, encoding=encoding))
         if "crs" not in data:
             data['crs'] = {"type": "name", "properties": {"name": "urn:ogc:def:crs:EPSG::{}".format(espg_value)}}
```

### Comparing `vgis_gis-1.3.6/vgis_gis/geoserverTools.py` & `vgis_gis-1.3.7/vgis_gis/geoserverTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.6/vgis_gis/gisTools.py` & `vgis_gis-1.3.7/vgis_gis/gisTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.6/vgis_gis/projTools.py` & `vgis_gis-1.3.7/vgis_gis/projTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.6/vgis_gis/shpTools.py` & `vgis_gis-1.3.7/vgis_gis/shpTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.6/vgis_gis.egg-info/PKG-INFO` & `vgis_gis-1.3.7/vgis_gis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-gis
-Version: 1.3.6
+Version: 1.3.7
 Summary: A libary for gis operator
 Home-page: https://github.com/gisfanmachel/vgisGis
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Keywords: gis,setuptools,development
 Platform: UNKNOWN
```

