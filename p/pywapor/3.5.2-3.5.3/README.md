# Comparing `tmp/pywapor-3.5.2.tar.gz` & `tmp/pywapor-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywapor-3.5.2.tar", last modified: Wed May 22 14:00:32 2024, max compression
+gzip compressed data, was "pywapor-3.5.3.tar", last modified: Wed May 29 08:39:11 2024, max compression
```

## Comparing `pywapor-3.5.2.tar` & `pywapor-3.5.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.784295 pywapor-3.5.2/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2024-03-27 14:46:37.000000 pywapor-3.5.2/LICENSE
--rw-r--r--   0 hmcoerver   (501) staff       (20)      518 2024-03-27 14:46:37.000000 pywapor-3.5.2/MANIFEST.in
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1086 2024-05-22 14:00:32.784088 pywapor-3.5.2/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13150 2024-03-27 14:46:52.000000 pywapor-3.5.2/README.md
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.743734 pywapor-3.5.2/pywapor/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      432 2024-05-20 13:50:40.000000 pywapor-3.5.2/pywapor/__init__.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.744791 pywapor-3.5.2/pywapor/collect/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      241 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15485 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/accounts.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10593 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/downloader.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.771397 pywapor-3.5.2/pywapor/collect/product/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5782 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/CHIRPS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8398 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/COPERNICUS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8540 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/ERA5.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9011 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/GEOS5.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1084450 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/GLO30.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1085475 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/GLO90.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5808 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/GLOBCOVER.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    39183 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/LANDSAT.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8549 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/MERRA2.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13898 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/MODIS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1232314 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/MODIS_tiles.geojson
--rw-r--r--   0 hmcoerver   (501) staff       (20)    21329 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/SENTINEL2.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7765 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/SENTINEL3.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7379 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/SRTM.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  3610761 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/SRTM30_tiles.geojson
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8376 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/STATICS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11418 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/TERRA.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    26513 2024-05-20 12:31:05.000000 pywapor-3.5.2/pywapor/collect/product/VIIRSL1.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      370 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/product/__init__.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.772387 pywapor-3.5.2/pywapor/collect/protocol/
--rw-r--r--   0 hmcoerver   (501) staff       (20)       33 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9316 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/cds.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     4705 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/cog.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12151 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/copernicus_odata.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9959 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/crawler.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    19421 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/opendap.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1572 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/collect/protocol/projections.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.774043 pywapor-3.5.2/pywapor/configs/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    17059 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR2_level_1.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    17360 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR2_level_2.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    21071 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR2_level_3.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    20940 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR3_level_2.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    20842 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/WaPOR3_level_3.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    30166 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/all_in.json
--rw-r--r--   0 hmcoerver   (501) staff       (20)    20467 2024-05-22 13:49:41.000000 pywapor-3.5.2/pywapor/configs/nrt.json
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.775307 pywapor-3.5.2/pywapor/enhancers/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      223 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1597 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/apply_enhancers.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2773 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dem.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.776437 pywapor-3.5.2/pywapor/enhancers/dms/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      175 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dms/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    36143 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dms/pyDMS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10174 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dms/pyDMS_utils.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    16289 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/dms/thermal_sharpener.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2066 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/gap_fill.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8897 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/lulc.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      616 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/other.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      348 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/pressure.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.777132 pywapor-3.5.2/pywapor/enhancers/smooth/
--rw-r--r--   0 hmcoerver   (501) staff       (20)        0 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    17945 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/archive.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6710 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/core.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10601 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/plotters.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13855 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/smooth/whittaker.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10210 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/temperature.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1003 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/enhancers/wind.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    16310 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.780768 pywapor-3.5.2/pywapor/et_look_v2_v3/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7216 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9037 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/biomass.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12950 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/clear_sky_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3891 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/constants.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5008 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/evapotranspiration.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5403 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/leaf.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    31410 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/meteo.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7248 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/neutral.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13996 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3833 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/resistance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6885 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/roughness.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32038 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/soil_moisture.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15852 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/solar_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5011 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/stress.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    24188 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/et_look_v2_v3/unstable.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.783288 pywapor-3.5.2/pywapor/general/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      304 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9590 2024-05-22 13:55:32.000000 pywapor-3.5.2/pywapor/general/aligner.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    22239 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/bitmasks.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13267 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/compositer.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2746 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/curvilinear.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3065 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/lazifier.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32054 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/levels.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15505 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/log_indenter.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2241 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/logger.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2373 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/performance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1885 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/pre_defaults.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15740 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/processing_functions.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12558 2024-05-22 13:49:43.000000 pywapor-3.5.2/pywapor/general/reproject.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2538 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/units.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32644 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/general/variables.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    24332 2024-05-22 13:49:37.000000 pywapor-3.5.2/pywapor/main.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    18087 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/post_et_look.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7259 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/pre_et_look.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6973 2024-05-22 13:55:50.000000 pywapor-3.5.2/pywapor/pre_se_root.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12004 2024-03-27 14:46:37.000000 pywapor-3.5.2/pywapor/se_root.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-22 14:00:32.783809 pywapor-3.5.2/pywapor.egg-info/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1086 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3160 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/SOURCES.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/dependency_links.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)      203 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/requires.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2024-05-22 14:00:32.000000 pywapor-3.5.2/pywapor.egg-info/top_level.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2024-05-22 14:00:32.784350 pywapor-3.5.2/setup.cfg
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1354 2024-05-20 13:50:31.000000 pywapor-3.5.2/setup.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.342570 pywapor-3.5.3/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2024-03-27 14:46:37.000000 pywapor-3.5.3/LICENSE
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      518 2024-03-27 14:46:37.000000 pywapor-3.5.3/MANIFEST.in
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1086 2024-05-29 08:39:11.342352 pywapor-3.5.3/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13140 2024-05-22 14:01:25.000000 pywapor-3.5.3/README.md
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.298094 pywapor-3.5.3/pywapor/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      432 2024-05-29 08:35:39.000000 pywapor-3.5.3/pywapor/__init__.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.299139 pywapor-3.5.3/pywapor/collect/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      241 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15485 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/accounts.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10593 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/downloader.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.326064 pywapor-3.5.3/pywapor/collect/product/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5782 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/CHIRPS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8398 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/COPERNICUS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8540 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/ERA5.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9011 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/GEOS5.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1084450 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/GLO30.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1085475 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/GLO90.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5808 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/GLOBCOVER.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    39183 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/LANDSAT.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8549 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/MERRA2.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13898 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/MODIS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1232314 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/MODIS_tiles.geojson
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    21329 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/SENTINEL2.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7765 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/SENTINEL3.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7379 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/SRTM.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  3610761 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/SRTM30_tiles.geojson
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8376 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/STATICS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11418 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/TERRA.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    26552 2024-05-29 08:28:44.000000 pywapor-3.5.3/pywapor/collect/product/VIIRSL1.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      370 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/product/__init__.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.329248 pywapor-3.5.3/pywapor/collect/protocol/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       33 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/protocol/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9316 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/protocol/cds.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     4705 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/protocol/cog.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12151 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/protocol/copernicus_odata.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10020 2024-05-28 12:00:25.000000 pywapor-3.5.3/pywapor/collect/protocol/crawler.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    19421 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/protocol/opendap.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1572 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/collect/protocol/projections.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.332026 pywapor-3.5.3/pywapor/configs/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    17059 2024-05-22 13:49:41.000000 pywapor-3.5.3/pywapor/configs/WaPOR2_level_1.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    17360 2024-05-22 13:49:41.000000 pywapor-3.5.3/pywapor/configs/WaPOR2_level_2.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    21071 2024-05-22 13:49:41.000000 pywapor-3.5.3/pywapor/configs/WaPOR2_level_3.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    20940 2024-05-22 13:49:41.000000 pywapor-3.5.3/pywapor/configs/WaPOR3_level_2.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    20842 2024-05-22 13:49:41.000000 pywapor-3.5.3/pywapor/configs/WaPOR3_level_3.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    30166 2024-05-22 13:49:41.000000 pywapor-3.5.3/pywapor/configs/all_in.json
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    20467 2024-05-22 13:49:41.000000 pywapor-3.5.3/pywapor/configs/nrt.json
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.334236 pywapor-3.5.3/pywapor/enhancers/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      223 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1597 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/apply_enhancers.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2773 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/dem.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.335534 pywapor-3.5.3/pywapor/enhancers/dms/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      175 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/dms/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    36143 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/dms/pyDMS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10174 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/dms/pyDMS_utils.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    16289 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/dms/thermal_sharpener.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2066 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/gap_fill.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8897 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/lulc.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      616 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/other.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      348 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/pressure.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.336633 pywapor-3.5.3/pywapor/enhancers/smooth/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        0 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/smooth/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    17945 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/smooth/archive.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6710 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/smooth/core.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10601 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/smooth/plotters.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13855 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/smooth/whittaker.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10210 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/temperature.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1003 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/enhancers/wind.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    16310 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.339340 pywapor-3.5.3/pywapor/et_look_v2_v3/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7216 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9037 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/biomass.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12950 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/clear_sky_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3891 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/constants.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5008 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/evapotranspiration.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5403 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/leaf.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    31410 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/meteo.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7248 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/neutral.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13996 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3833 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/resistance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6885 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/roughness.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32038 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/soil_moisture.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15852 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/solar_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5011 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/stress.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    24188 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/et_look_v2_v3/unstable.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.341873 pywapor-3.5.3/pywapor/general/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      304 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9590 2024-05-22 13:55:32.000000 pywapor-3.5.3/pywapor/general/aligner.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    22239 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/bitmasks.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13267 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/compositer.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2746 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/curvilinear.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3065 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/lazifier.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32054 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/levels.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15505 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/log_indenter.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2241 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/logger.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2373 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/performance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1885 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/pre_defaults.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15740 2024-05-29 08:20:36.000000 pywapor-3.5.3/pywapor/general/processing_functions.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12558 2024-05-22 13:49:43.000000 pywapor-3.5.3/pywapor/general/reproject.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2538 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/units.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32644 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/general/variables.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    26392 2024-05-29 08:33:26.000000 pywapor-3.5.3/pywapor/main.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    18087 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/post_et_look.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7259 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/pre_et_look.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6973 2024-05-22 13:55:50.000000 pywapor-3.5.3/pywapor/pre_se_root.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12004 2024-03-27 14:46:37.000000 pywapor-3.5.3/pywapor/se_root.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-05-29 08:39:11.342071 pywapor-3.5.3/pywapor.egg-info/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1086 2024-05-29 08:39:11.000000 pywapor-3.5.3/pywapor.egg-info/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3160 2024-05-29 08:39:11.000000 pywapor-3.5.3/pywapor.egg-info/SOURCES.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2024-05-29 08:39:11.000000 pywapor-3.5.3/pywapor.egg-info/dependency_links.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      203 2024-05-29 08:39:11.000000 pywapor-3.5.3/pywapor.egg-info/requires.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2024-05-29 08:39:11.000000 pywapor-3.5.3/pywapor.egg-info/top_level.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2024-05-29 08:39:11.342616 pywapor-3.5.3/setup.cfg
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1354 2024-05-29 08:35:44.000000 pywapor-3.5.3/setup.py
```

### Comparing `pywapor-3.5.2/LICENSE` & `pywapor-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/MANIFEST.in` & `pywapor-3.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/PKG-INFO` & `pywapor-3.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywapor
-Version: 3.5.2
+Version: 3.5.3
 Home-page: https://www.fao.org/aquastat/py-wapor/
 Author: FAO
 Author-email: bert.coerver@fao.org
 License: Apache
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pywapor-3.5.2/README.md` & `pywapor-3.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     'meteorological': {'GEOS5.tavg1_2d_slv_Nx'},
     'optical': {'SENTINEL2.S2MSI2A_R20m'},
     'precipitation': {'CHIRPS.P05'},
     'solar radiation': {'ERA5.sis-agrometeorological-indicators'},
     'statics': {'STATICS.WaPOR3'},
     'thermal': {'VIIRSL1.VNP02IMG'},
     # Use se_root output as soil moisture data.
-    'soil moisture': {'FILE:{folder}{sep}se_root_out*.nc.from_file'},
+    'soil moisture': {'FILE:{folder}{sep}se_root_out*.nc'},
     # Define which product to reproject the other products to.
     '_EXAMPLE_': 'SENTINEL2.S2MSI2A_R20m', 
     # Define any special functions to apply to a specific variable.
     '_ENHANCE_': {"bt": ["pywapor.enhancers.dms.thermal_sharpener.sharpen"],},
     # Choose which products should be gapfilled.
     '_WHITTAKER_': {
         'SENTINEL2.S2MSI2A_R20m': {'lmbdas': 1000.0, 'method': 'whittaker'},
```

#### html2text {}

```diff
@@ -27,23 +27,22 @@
 by passing a name to `Project.load_configuration` (as done above), by passing a
 summary or by loading a configuration from a JSON-file: ```python summary = { #
 Define which products to use. 'elevation': {'COPERNICUS.GLO30'},
 'meteorological': {'GEOS5.tavg1_2d_slv_Nx'}, 'optical':
 {'SENTINEL2.S2MSI2A_R20m'}, 'precipitation': {'CHIRPS.P05'}, 'solar radiation':
 {'ERA5.sis-agrometeorological-indicators'}, 'statics': {'STATICS.WaPOR3'},
 'thermal': {'VIIRSL1.VNP02IMG'}, # Use se_root output as soil moisture data.
-'soil moisture': {'FILE:{folder}{sep}se_root_out*.nc.from_file'}, # Define
-which product to reproject the other products to. '_EXAMPLE_':
-'SENTINEL2.S2MSI2A_R20m', # Define any special functions to apply to a specific
-variable. '_ENHANCE_': {"bt":
-["pywapor.enhancers.dms.thermal_sharpener.sharpen"],}, # Choose which products
-should be gapfilled. '_WHITTAKER_': { 'SENTINEL2.S2MSI2A_R20m': {'lmbdas':
-1000.0, 'method': 'whittaker'}, 'VIIRSL1.VNP02IMG': {'a': 0.85, 'lmbdas':
-1000.0, 'method': 'whittaker'}}, } project.load_configuration(summary =
-summary) ``` Save a configuration to a JSON-file like this: ```python
+'soil moisture': {'FILE:{folder}{sep}se_root_out*.nc'}, # Define which product
+to reproject the other products to. '_EXAMPLE_': 'SENTINEL2.S2MSI2A_R20m', #
+Define any special functions to apply to a specific variable. '_ENHANCE_':
+{"bt": ["pywapor.enhancers.dms.thermal_sharpener.sharpen"],}, # Choose which
+products should be gapfilled. '_WHITTAKER_': { 'SENTINEL2.S2MSI2A_R20m':
+{'lmbdas': 1000.0, 'method': 'whittaker'}, 'VIIRSL1.VNP02IMG': {'a': 0.85,
+'lmbdas': 1000.0, 'method': 'whittaker'}}, } project.load_configuration(summary
+= summary) ``` Save a configuration to a JSON-file like this: ```python
 project.configuration.to_json("/path/to/my/configuration.json") ``` Load a
 configuration from a JSON-file: ```python project.load_configuration(json = "/
 path/to/my/configuration.json") ``` Changing model parameters (or entire
 variables) can be done in between the `project.run_pre_se_root()` and
 `project.run_se_root()` steps (same goes for `et_look`) by making changes to
 the `xarray.Dataset` returned by `project.run_pre_se_root` (and stored at
 `project.se_root_in`): ```python print(se_root_in["r0_bare"].values) >>> 0.38
```

### Comparing `pywapor-3.5.2/pywapor/collect/accounts.py` & `pywapor-3.5.3/pywapor/collect/accounts.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/downloader.py` & `pywapor-3.5.3/pywapor/collect/downloader.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/CHIRPS.py` & `pywapor-3.5.3/pywapor/collect/product/CHIRPS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/COPERNICUS.py` & `pywapor-3.5.3/pywapor/collect/product/COPERNICUS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/ERA5.py` & `pywapor-3.5.3/pywapor/collect/product/ERA5.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/GEOS5.py` & `pywapor-3.5.3/pywapor/collect/product/GEOS5.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/GLO30.txt` & `pywapor-3.5.3/pywapor/collect/product/GLO30.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/GLO90.txt` & `pywapor-3.5.3/pywapor/collect/product/GLO90.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/GLOBCOVER.py` & `pywapor-3.5.3/pywapor/collect/product/GLOBCOVER.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/LANDSAT.py` & `pywapor-3.5.3/pywapor/collect/product/LANDSAT.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/MERRA2.py` & `pywapor-3.5.3/pywapor/collect/product/MERRA2.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/MODIS.py` & `pywapor-3.5.3/pywapor/collect/product/MODIS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/MODIS_tiles.geojson` & `pywapor-3.5.3/pywapor/collect/product/MODIS_tiles.geojson`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/SENTINEL2.py` & `pywapor-3.5.3/pywapor/collect/product/SENTINEL2.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/SENTINEL3.py` & `pywapor-3.5.3/pywapor/collect/product/SENTINEL3.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/SRTM.py` & `pywapor-3.5.3/pywapor/collect/product/SRTM.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/SRTM30_tiles.geojson` & `pywapor-3.5.3/pywapor/collect/product/SRTM30_tiles.geojson`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/STATICS.py` & `pywapor-3.5.3/pywapor/collect/product/STATICS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/TERRA.py` & `pywapor-3.5.3/pywapor/collect/product/TERRA.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/product/VIIRSL1.py` & `pywapor-3.5.3/pywapor/collect/product/VIIRSL1.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 import urllib
 import copy
 import os
 import multiprocessing
 import xarray as xr
 import numpy as np
 import tqdm
+import posixpath
 from osgeo import gdal
 from functools import partial
 from pywapor.collect import accounts
 from pywapor.collect.protocol.crawler import download_urls, download_url
 from joblib import Parallel, delayed, Memory
 from pywapor.enhancers.apply_enhancers import apply_enhancers
-from pywapor.general.processing_functions import save_ds, remove_ds, adjust_timelim_dtype, is_corrupt_or_empty, open_ds
+from pywapor.general.processing_functions import save_ds, remove_ds, adjust_timelim_dtype, is_corrupt_or_empty, open_ds, urljoin
 from pywapor.general.logger import log, adjust_logger
 from pywapor.enhancers.other import drop_empty_times
 from pywapor.general.curvilinear import curvi_to_recto, create_grid
 from pywapor.collect.protocol.opendap import make_opendap_url
 gdal.UseExceptions()
 
 def get_token():
@@ -410,17 +411,17 @@
 
         elif dl_method == "get_request":
             base_url = "https://ladsweb.modaps.eosdis.nasa.gov/archive/allData/"
             nc02_parts = os.path.normpath(nc02).split(os.sep)
             nc03_parts = os.path.normpath(nc03).split(os.sep)
             nc_cloud_parts = os.path.normpath(nc_cloud).split(os.sep)
             year_doy = nc02_parts[-1].split(".")[1][1:]
-            nc02_url = os.path.join(base_url, "5200", nc02_parts[-2], year_doy[:4], year_doy[4:], nc02_parts[-1])
-            nc03_url = os.path.join(base_url, "5200", nc03_parts[-2], year_doy[:4], year_doy[4:], nc03_parts[-1])
-            ncqa_url = os.path.join(base_url, "5110", nc_cloud_parts[-2], year_doy[:4], year_doy[4:], nc_cloud_parts[-1])
+            nc02_url = posixpath.join(base_url, "5200", nc02_parts[-2], year_doy[:4], year_doy[4:], nc02_parts[-1])
+            nc03_url = posixpath.join(base_url, "5200", nc03_parts[-2], year_doy[:4], year_doy[4:], nc03_parts[-1])
+            ncqa_url = posixpath.join(base_url, "5110", nc_cloud_parts[-2], year_doy[:4], year_doy[4:], nc_cloud_parts[-1])
             urls = [nc02_url, nc03_url, ncqa_url]
             groups = ["observation_data", "geolocation_data", "geophysical_data"]
             for group, url in zip(groups, urls.copy()):
                 fp_ = os.path.join(folder, os.path.split(url)[-1])
                 if os.path.isfile(fp_):
                     corrupt = is_corrupt_or_empty(fp_, group = group)
                     if corrupt:
@@ -446,17 +447,18 @@
         elif dl_method == "opendap":
 
             base_url = "https://ladsweb.modaps.eosdis.nasa.gov/opendap/RemoteResources/laads/allData"
             nc02_parts = os.path.normpath(nc02).split(os.sep)
             nc03_parts = os.path.normpath(nc03).split(os.sep)
             nc_cloud_parts = os.path.normpath(nc_cloud).split(os.sep)
             year_doy = nc02_parts[-1].split(".")[1][1:]
-            base_url02 = os.path.join(base_url, "5200", nc02_parts[-2], year_doy[:4], year_doy[4:], nc02_parts[-1])
-            base_url03 = os.path.join(base_url, "5200", nc03_parts[-2], year_doy[:4], year_doy[4:], nc03_parts[-1])
-            base_cloud = os.path.join(base_url, "5110", nc_cloud_parts[-2], year_doy[:4], year_doy[4:], nc_cloud_parts[-1])
+
+            base_url02 = posixpath.join(base_url, "5200", nc02_parts[-2], year_doy[:4], year_doy[4:], nc02_parts[-1])
+            base_url03 = posixpath.join(base_url, "5200", nc03_parts[-2], year_doy[:4], year_doy[4:], nc03_parts[-1])
+            base_cloud = posixpath.join(base_url, "5110", nc_cloud_parts[-2], year_doy[:4], year_doy[4:], nc_cloud_parts[-1])
 
             # Download geolocation data.
             order = {
                 "/geolocation_data/longitude": {},
                 "/geolocation_data/latitude": {},
             }
             url = make_opendap_url(base_url03, order)
```

### Comparing `pywapor-3.5.2/pywapor/collect/protocol/cds.py` & `pywapor-3.5.3/pywapor/collect/protocol/cds.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/protocol/cog.py` & `pywapor-3.5.3/pywapor/collect/protocol/cog.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/protocol/copernicus_odata.py` & `pywapor-3.5.3/pywapor/collect/protocol/copernicus_odata.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/protocol/crawler.py` & `pywapor-3.5.3/pywapor/collect/protocol/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,15 @@
         log.warning(f"--> Didn't succeed to download {len(urls)} files.")
     return relevant_fps
 
 
 def _download_url(url, fp, session = None, waitbar = True, headers = None):
 
     if os.path.isfile(fp):
+        log.add().info(f"--> Reusing existing `{fp}` file.")
         return fp
 
     folder, fn = os.path.split(fp)
     if not os.path.exists(folder):
         os.makedirs(folder)
 
     ext = os.path.splitext(fp)[-1]
```

### Comparing `pywapor-3.5.2/pywapor/collect/protocol/opendap.py` & `pywapor-3.5.3/pywapor/collect/protocol/opendap.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/collect/protocol/projections.py` & `pywapor-3.5.3/pywapor/collect/protocol/projections.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/configs/WaPOR2_level_1.json` & `pywapor-3.5.3/pywapor/configs/WaPOR2_level_1.json`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/configs/WaPOR2_level_2.json` & `pywapor-3.5.3/pywapor/configs/WaPOR2_level_2.json`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/configs/WaPOR2_level_3.json` & `pywapor-3.5.3/pywapor/configs/WaPOR2_level_3.json`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/configs/WaPOR3_level_2.json` & `pywapor-3.5.3/pywapor/configs/WaPOR3_level_2.json`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/configs/WaPOR3_level_3.json` & `pywapor-3.5.3/pywapor/configs/WaPOR3_level_3.json`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/configs/all_in.json` & `pywapor-3.5.3/pywapor/configs/all_in.json`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/configs/nrt.json` & `pywapor-3.5.3/pywapor/configs/nrt.json`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/apply_enhancers.py` & `pywapor-3.5.3/pywapor/enhancers/apply_enhancers.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/dem.py` & `pywapor-3.5.3/pywapor/enhancers/dem.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/dms/pyDMS.py` & `pywapor-3.5.3/pywapor/enhancers/dms/pyDMS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/dms/pyDMS_utils.py` & `pywapor-3.5.3/pywapor/enhancers/dms/pyDMS_utils.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/dms/thermal_sharpener.py` & `pywapor-3.5.3/pywapor/enhancers/dms/thermal_sharpener.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/gap_fill.py` & `pywapor-3.5.3/pywapor/enhancers/gap_fill.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/lulc.py` & `pywapor-3.5.3/pywapor/enhancers/lulc.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/other.py` & `pywapor-3.5.3/pywapor/enhancers/other.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/smooth/archive.py` & `pywapor-3.5.3/pywapor/enhancers/smooth/archive.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/smooth/core.py` & `pywapor-3.5.3/pywapor/enhancers/smooth/core.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/smooth/plotters.py` & `pywapor-3.5.3/pywapor/enhancers/smooth/plotters.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/smooth/whittaker.py` & `pywapor-3.5.3/pywapor/enhancers/smooth/whittaker.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/temperature.py` & `pywapor-3.5.3/pywapor/enhancers/temperature.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/enhancers/wind.py` & `pywapor-3.5.3/pywapor/enhancers/wind.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look.py` & `pywapor-3.5.3/pywapor/et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/__init__.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/biomass.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/biomass.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/clear_sky_radiation.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/clear_sky_radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/constants.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/constants.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/evapotranspiration.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/evapotranspiration.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/leaf.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/leaf.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/meteo.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/meteo.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/neutral.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/neutral.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/radiation.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/resistance.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/resistance.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/roughness.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/roughness.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/soil_moisture.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/soil_moisture.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/solar_radiation.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/solar_radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/stress.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/stress.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/et_look_v2_v3/unstable.py` & `pywapor-3.5.3/pywapor/et_look_v2_v3/unstable.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/aligner.py` & `pywapor-3.5.3/pywapor/general/aligner.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/bitmasks.py` & `pywapor-3.5.3/pywapor/general/bitmasks.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/compositer.py` & `pywapor-3.5.3/pywapor/general/compositer.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/curvilinear.py` & `pywapor-3.5.3/pywapor/general/curvilinear.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/lazifier.py` & `pywapor-3.5.3/pywapor/general/lazifier.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/levels.py` & `pywapor-3.5.3/pywapor/general/levels.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/log_indenter.py` & `pywapor-3.5.3/pywapor/general/log_indenter.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/logger.py` & `pywapor-3.5.3/pywapor/general/logger.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/performance.py` & `pywapor-3.5.3/pywapor/general/performance.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/pre_defaults.py` & `pywapor-3.5.3/pywapor/general/pre_defaults.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/processing_functions.py` & `pywapor-3.5.3/pywapor/general/processing_functions.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/reproject.py` & `pywapor-3.5.3/pywapor/general/reproject.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/units.py` & `pywapor-3.5.3/pywapor/general/units.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/general/variables.py` & `pywapor-3.5.3/pywapor/general/variables.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/main.py` & `pywapor-3.5.3/pywapor/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -532,59 +532,94 @@
         log.sub().info("< PASSWORDS")
 
     def download_data(self, buffer_timelim = True):
         assert not isinstance(self.configuration, type(None)), "Please load a configuration before continueing."
 
         log.info("> DOWNLOADER").add()
 
+        example_t_vars = [x for x in ["lst", "bt"] if x in self.configuration.full.keys()]
+        example_sources = {k:v for k,v in self.configuration.full.items() if k in example_t_vars}
+        other_sources = {k:v for k,v in self.configuration.full.items() if k not in example_t_vars}
+
         if buffer_timelim:
             bins = time_bins(self.period, 1)
             adjusted_timelim = [bins[0], bins[-1]]
             buffered_timelim = [adjusted_timelim[0] - np.timedelta64(3, "D"), 
                                 adjusted_timelim[1] + np.timedelta64(3, "D")]
         else:
             adjusted_timelim = self.period
             buffered_timelim = self.period
 
-        self.dss, _ = collect_sources(
+        example_dss, _ = collect_sources(
+                            self.folder,
+                            example_sources,
+                            self.latlim,
+                            self.lonlim,
+                            adjusted_timelim,
+                            landsat_order_only = True
+                            )
+        
+        other_dss, _ = collect_sources(
                             self.folder,
-                            self.configuration.full,
+                            other_sources,
                             self.latlim,
                             self.lonlim,
                             buffered_timelim,
                             )
         
+        # If there are example-t variables that rely on landsat, try one more time to collect them.
+        if np.any(list({var: np.any([product_info["source"] == "LANDSAT" for product_info in info["products"]]) for var, info in example_sources.items()}.values())):
+            example_dss, _ = collect_sources(
+                                            self.folder, 
+                                            example_sources, 
+                                            self.latlim, 
+                                            self.lonlim, 
+                                            adjusted_timelim
+                                            )
+
+        self.dss = {**example_dss, **other_dss}
+        
         log.sub().info("< DOWNLOADER")
     
         return self.dss
     
     def run_pre_se_root(self, forced = False):
         if isinstance(self.se_root_in, type(None)) or forced:
             self.se_root_in = pywapor.pre_se_root.main(self.folder, self.latlim, self.lonlim, self.period, sources = self.configuration.se_root)
         else:
             log.info("> PRE_SE_ROOT").add()
             log.info(f"--> Re-using `{os.path.split(self.se_root_in.encoding['source'])[-1]}`.")
             log.sub().info("< PRE_SE_ROOT")
         return self.se_root_in
 
-    def run_se_root(self, se_root_version = "v3"):
-        self.se_root_out = pywapor.se_root.main(self.se_root_in, se_root_version = se_root_version)
+    def run_se_root(self, se_root_version = "v3", export_vars = "default", chunks = {"time": -1, "x": 500, "y": 500}):
+        self.se_root_out = pywapor.se_root.main(
+                                                self.se_root_in, 
+                                                se_root_version = se_root_version, 
+                                                export_vars = export_vars, 
+                                                chunks = chunks
+                                                )
         return self.se_root_out
     
     def run_pre_et_look(self, forced = False):
         if isinstance(self.et_look_in, type(None)) or forced:
             self.et_look_in = pywapor.pre_et_look.main(self.folder, self.latlim, self.lonlim, self.period, sources = self.configuration.et_look)
         else:
             log.info("> PRE_ET_LOOK").add()
             log.info(f"--> Re-using `{os.path.split(self.et_look_in.encoding['source'])[-1]}`.")
             log.sub().info("< PRE_ET_LOOK")
         return self.et_look_in
 
-    def run_et_look(self, et_look_version = "v3"):
-        self.et_look_out = pywapor.et_look.main(self.et_look_in, et_look_version = et_look_version)
+    def run_et_look(self, et_look_version = "v3", export_vars = "default", chunks = {"time_bins": -1, "x": 500, "y": 500}):
+        self.et_look_out = pywapor.et_look.main(
+                                                self.et_look_in, 
+                                                et_look_version = et_look_version, 
+                                                export_vars = export_vars, 
+                                                chunks = chunks
+                                                )
         return self.et_look_out
 
 if __name__ == "__main__":
 
     timelim = ["2022-01-01", "2023-12-31"]
     latlim = [21.9692194682626933, 21.9939120838340507]
     lonlim = [91.9371349243682801, 91.9657566608824339]
@@ -639,13 +674,13 @@
 
     project.set_passwords()
     dss = project.download_data()
     
     se_root_in = project.run_pre_se_root()
     # se_root = project.run_se_root()
     # et_look_in = project.run_pre_et_look()
-    # et_look = project.run_et_look()
+    et_look = project.run_et_look()
```

### Comparing `pywapor-3.5.2/pywapor/post_et_look.py` & `pywapor-3.5.3/pywapor/post_et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/pre_et_look.py` & `pywapor-3.5.3/pywapor/pre_et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/pre_se_root.py` & `pywapor-3.5.3/pywapor/pre_se_root.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor/se_root.py` & `pywapor-3.5.3/pywapor/se_root.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/pywapor.egg-info/PKG-INFO` & `pywapor-3.5.3/pywapor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywapor
-Version: 3.5.2
+Version: 3.5.3
 Home-page: https://www.fao.org/aquastat/py-wapor/
 Author: FAO
 Author-email: bert.coerver@fao.org
 License: Apache
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pywapor-3.5.2/pywapor.egg-info/SOURCES.txt` & `pywapor-3.5.3/pywapor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.5.2/setup.py` & `pywapor-3.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pywapor',
-    version = '3.5.2',
+    version = '3.5.3',
     url = 'https://www.fao.org/aquastat/py-wapor/',
     author = "FAO",
     author_email = "bert.coerver@fao.org",
     license = "Apache",
     packages = find_packages(include = ['pywapor', 'pywapor.*']),
     include_package_data=True,
     python_requires='>=3.7',
```

