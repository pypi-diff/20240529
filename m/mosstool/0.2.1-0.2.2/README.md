# Comparing `tmp/mosstool-0.2.1.tar.gz` & `tmp/mosstool-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosstool-0.2.1.tar", max compression
+gzip compressed data, was "mosstool-0.2.2.tar", max compression
```

## Comparing `mosstool-0.2.1.tar` & `mosstool-0.2.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      106 2024-05-28 11:11:04.791999 mosstool-0.2.1/README.md
--rw-r--r--   0        0        0      268 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/__init__.py
--rw-r--r--   0        0        0    16340 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/add_aoi_pop.py
--rw-r--r--   0        0        0    70559 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/aoi_matcher.py
--rw-r--r--   0        0        0    16237 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/aoiutils.py
--rw-r--r--   0        0        0     2956 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/const.py
--rw-r--r--   0        0        0    11404 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/convert_aoi.py
--rw-r--r--   0        0        0    16609 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/format_checker.py
--rw-r--r--   0        0        0    21033 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/gen_traffic_light.py
--rw-r--r--   0        0        0     2045 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/map_aois_matchers.py
--rw-r--r--   0        0        0     1155 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/osm_const.py
--rw-r--r--   0        0        0        0 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_util/__init__.py
--rw-r--r--   0        0        0      444 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_util/angle.py
--rw-r--r--   0        0        0     3626 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_util/bezier.py
--rw-r--r--   0        0        0    12436 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_util/line.py
--rw-r--r--   0        0        0      100 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/builder/__init__.py
--rw-r--r--   0        0        0   206163 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/builder/builder.py
--rw-r--r--   0        0        0      185 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/__init__.py
--rw-r--r--   0        0        0     7162 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/_motif.py
--rw-r--r--   0        0        0     2643 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/_wayutil.py
--rw-r--r--   0        0        0    14567 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/building.py
--rw-r--r--   0        0        0    28323 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/roadnet.py
--rw-r--r--   0        0        0      373 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/public_transport/__init__.py
--rw-r--r--   0        0        0    12458 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/public_transport/get_bus.py
--rw-r--r--   0        0        0    12224 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/public_transport/get_subway.py
--rw-r--r--   0        0        0    21211 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/public_transport/get_transitland.py
--rw-r--r--   0        0        0    16145 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/public_transport/public_transport_post.py
--rw-r--r--   0        0        0       92 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/sumo/__init__.py
--rw-r--r--   0        0        0    37747 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/sumo/map.py
--rw-r--r--   0        0        0       79 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/vis/__init__.py
--rw-r--r--   0        0        0     9999 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/vis/map.py
--rw-r--r--   0        0        0       36 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/__init__.py
--rw-r--r--   0        0        0      758 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/AIGC.py
--rw-r--r--   0        0        0      347 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/__init__.py
--rw-r--r--   0        0        0      688 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/_util/const.py
--rw-r--r--   0        0        0      406 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/_util/utils.py
--rw-r--r--   0        0        0    19820 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/generate_from_od.py
--rw-r--r--   0        0        0     3774 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/gravity.py
--rw-r--r--   0        0        0     5190 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/random.py
--rw-r--r--   0        0        0      702 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/template.py
--rw-r--r--   0        0        0      119 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/route/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/route/client.py
--rw-r--r--   0        0        0     3398 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/route/preroute.py
--rw-r--r--   0        0        0      100 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/sumo/__init__.py
--rw-r--r--   0        0        0    37589 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/sumo/route.py
--rw-r--r--   0        0        0       78 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/vis/__init__.py
--rw-r--r--   0        0        0     8307 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/vis/trip.py
--rw-r--r--   0        0        0      783 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/type/__init__.py
--rw-r--r--   0        0        0       22 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/__init__.py
--rw-r--r--   0        0        0      481 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/color.py
--rw-r--r--   0        0        0     4519 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/format_converter.py
--rw-r--r--   0        0        0    14922 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/geo_match_pop.py
--rw-r--r--   0        0        0     2039 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/map_merger.py
--rw-r--r--   0        0        0     6538 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/map_splitter.py
--rw-r--r--   0        0        0        0 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/test/__init__.py
--rw-r--r--   0        0        0      194 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/test/test_color.py
--rw-r--r--   0        0        0     1150 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/test/test_format_conveter.py
--rw-r--r--   0        0        0      853 2024-05-28 11:11:05.452002 mosstool-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 mosstool-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-28 14:00:46.538107 mosstool-0.2.2/README.md
+-rw-r--r--   0        0        0      268 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/__init__.py
+-rw-r--r--   0        0        0    16340 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/add_aoi_pop.py
+-rw-r--r--   0        0        0    70559 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/aoi_matcher.py
+-rw-r--r--   0        0        0    16237 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/aoiutils.py
+-rw-r--r--   0        0        0     2956 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/const.py
+-rw-r--r--   0        0        0    11404 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/convert_aoi.py
+-rw-r--r--   0        0        0    16617 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/format_checker.py
+-rw-r--r--   0        0        0    21033 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/gen_traffic_light.py
+-rw-r--r--   0        0        0     2045 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/map_aois_matchers.py
+-rw-r--r--   0        0        0     1155 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_map_util/osm_const.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_util/__init__.py
+-rw-r--r--   0        0        0      444 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_util/angle.py
+-rw-r--r--   0        0        0     3626 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_util/bezier.py
+-rw-r--r--   0        0        0    12436 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/_util/line.py
+-rw-r--r--   0        0        0      100 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/builder/__init__.py
+-rw-r--r--   0        0        0   206163 2024-05-28 14:00:47.194106 mosstool-0.2.2/mosstool/map/builder/builder.py
+-rw-r--r--   0        0        0      185 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/osm/__init__.py
+-rw-r--r--   0        0        0     7162 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/osm/_motif.py
+-rw-r--r--   0        0        0     2643 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/osm/_wayutil.py
+-rw-r--r--   0        0        0    14567 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/osm/building.py
+-rw-r--r--   0        0        0    28323 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/osm/roadnet.py
+-rw-r--r--   0        0        0      373 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/public_transport/__init__.py
+-rw-r--r--   0        0        0    12458 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/public_transport/get_bus.py
+-rw-r--r--   0        0        0    12224 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/public_transport/get_subway.py
+-rw-r--r--   0        0        0    21211 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/public_transport/get_transitland.py
+-rw-r--r--   0        0        0    16145 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/public_transport/public_transport_post.py
+-rw-r--r--   0        0        0       92 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/sumo/__init__.py
+-rw-r--r--   0        0        0    37747 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/sumo/map.py
+-rw-r--r--   0        0        0       79 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/vis/__init__.py
+-rw-r--r--   0        0        0     9999 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/map/vis/map.py
+-rw-r--r--   0        0        0       36 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/generator/AIGC.py
+-rw-r--r--   0        0        0      347 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/generator/__init__.py
+-rw-r--r--   0        0        0      688 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/generator/_util/const.py
+-rw-r--r--   0        0        0      406 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/generator/_util/utils.py
+-rw-r--r--   0        0        0    19820 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/generator/generate_from_od.py
+-rw-r--r--   0        0        0     3774 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/generator/gravity.py
+-rw-r--r--   0        0        0     5190 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/generator/random.py
+-rw-r--r--   0        0        0      702 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/generator/template.py
+-rw-r--r--   0        0        0      119 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/route/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/route/client.py
+-rw-r--r--   0        0        0     3398 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/route/preroute.py
+-rw-r--r--   0        0        0      100 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/sumo/__init__.py
+-rw-r--r--   0        0        0    37589 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/sumo/route.py
+-rw-r--r--   0        0        0       78 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/vis/__init__.py
+-rw-r--r--   0        0        0     8307 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/trip/vis/trip.py
+-rw-r--r--   0        0        0      783 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/type/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/color.py
+-rw-r--r--   0        0        0     4519 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/format_converter.py
+-rw-r--r--   0        0        0    14922 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/geo_match_pop.py
+-rw-r--r--   0        0        0     2039 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/map_merger.py
+-rw-r--r--   0        0        0     6538 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/map_splitter.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/test/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/test/test_color.py
+-rw-r--r--   0        0        0     1150 2024-05-28 14:00:47.198106 mosstool-0.2.2/mosstool/util/test/test_format_conveter.py
+-rw-r--r--   0        0        0      853 2024-05-28 14:00:47.202106 mosstool-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 mosstool-0.2.2/PKG-INFO
```

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/add_aoi_pop.py` & `mosstool-0.2.2/mosstool/map/_map_util/add_aoi_pop.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/aoi_matcher.py` & `mosstool-0.2.2/mosstool/map/_map_util/aoi_matcher.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/aoiutils.py` & `mosstool-0.2.2/mosstool/map/_map_util/aoiutils.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/const.py` & `mosstool-0.2.2/mosstool/map/_map_util/const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/convert_aoi.py` & `mosstool-0.2.2/mosstool/map/_map_util/convert_aoi.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/format_checker.py` & `mosstool-0.2.2/mosstool/map/_map_util/format_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.messages = []
 
     def emit(self, record):
         self.messages.append(self.format(record))
 
     def trigger_warnings(self):
         if self.messages:
-            sys.exit("Mapbuilder terminated due to warning messages above.")
+            raise ValueError("Mapbuilder terminated due to warning messages above.")
         else:
             pass
 
 
 def geojson_format_check(
     topo: FeatureCollection,
 ) -> None:
```

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/gen_traffic_light.py` & `mosstool-0.2.2/mosstool/map/_map_util/gen_traffic_light.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/map_aois_matchers.py` & `mosstool-0.2.2/mosstool/map/_map_util/map_aois_matchers.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_map_util/osm_const.py` & `mosstool-0.2.2/mosstool/map/_map_util/osm_const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_util/bezier.py` & `mosstool-0.2.2/mosstool/map/_util/bezier.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/_util/line.py` & `mosstool-0.2.2/mosstool/map/_util/line.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/builder/builder.py` & `mosstool-0.2.2/mosstool/map/builder/builder.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/osm/_motif.py` & `mosstool-0.2.2/mosstool/map/osm/_motif.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/osm/_wayutil.py` & `mosstool-0.2.2/mosstool/map/osm/_wayutil.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/osm/building.py` & `mosstool-0.2.2/mosstool/map/osm/building.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/osm/roadnet.py` & `mosstool-0.2.2/mosstool/map/osm/roadnet.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/public_transport/get_bus.py` & `mosstool-0.2.2/mosstool/map/public_transport/get_bus.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/public_transport/get_subway.py` & `mosstool-0.2.2/mosstool/map/public_transport/get_subway.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/public_transport/get_transitland.py` & `mosstool-0.2.2/mosstool/map/public_transport/get_transitland.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/public_transport/public_transport_post.py` & `mosstool-0.2.2/mosstool/map/public_transport/public_transport_post.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/sumo/map.py` & `mosstool-0.2.2/mosstool/map/sumo/map.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/map/vis/map.py` & `mosstool-0.2.2/mosstool/map/vis/map.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/generator/AIGC.py` & `mosstool-0.2.2/mosstool/trip/generator/AIGC.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/generator/_util/const.py` & `mosstool-0.2.2/mosstool/trip/generator/_util/const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/generator/generate_from_od.py` & `mosstool-0.2.2/mosstool/trip/generator/generate_from_od.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/generator/gravity.py` & `mosstool-0.2.2/mosstool/trip/generator/gravity.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/generator/random.py` & `mosstool-0.2.2/mosstool/trip/generator/random.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/generator/template.py` & `mosstool-0.2.2/mosstool/trip/generator/template.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/route/client.py` & `mosstool-0.2.2/mosstool/trip/route/client.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/route/preroute.py` & `mosstool-0.2.2/mosstool/trip/route/preroute.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/sumo/route.py` & `mosstool-0.2.2/mosstool/trip/sumo/route.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/trip/vis/trip.py` & `mosstool-0.2.2/mosstool/trip/vis/trip.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/type/__init__.py` & `mosstool-0.2.2/mosstool/type/__init__.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/util/format_converter.py` & `mosstool-0.2.2/mosstool/util/format_converter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/util/geo_match_pop.py` & `mosstool-0.2.2/mosstool/util/geo_match_pop.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/util/map_merger.py` & `mosstool-0.2.2/mosstool/util/map_merger.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/util/map_splitter.py` & `mosstool-0.2.2/mosstool/util/map_splitter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/mosstool/util/test/test_format_conveter.py` & `mosstool-0.2.2/mosstool/util/test/test_format_conveter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.1/pyproject.toml` & `mosstool-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosstool"
-version = "0.2.1"
+version = "0.2.2"
 description = "MObility Simulation System toolbox "
 authors = ["Jun Zhang <zhangjun990222@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `mosstool-0.2.1/PKG-INFO` & `mosstool-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosstool
-Version: 0.2.1
+Version: 0.2.2
 Summary: MObility Simulation System toolbox 
 License: MIT
 Author: Jun Zhang
 Author-email: zhangjun990222@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

