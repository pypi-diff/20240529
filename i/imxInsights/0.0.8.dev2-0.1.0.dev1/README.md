# Comparing `tmp/imxinsights-0.0.8.dev2.tar.gz` & `tmp/imxinsights-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imxinsights-0.0.8.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "imxinsights-0.1.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `imxinsights-0.0.8.dev2.tar` & `imxinsights-0.1.0.dev1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     5229 2024-05-21 10:52:12.169187 imxinsights-0.0.8.dev2/README.md
--rw-r--r--   0        0        0     2227 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/__init__.py
--rw-r--r--   0        0        0     1103 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/custom_puic_config.yaml
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/diff/__init__.py
--rw-r--r--   0        0        0      904 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/diff/areaStatusEnum.py
--rw-r--r--   0        0        0     5025 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/diff/change.py
--rw-r--r--   0        0        0    13116 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/diff/compair.py
--rw-r--r--   0        0        0      889 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/diff/diffStatusEnum.py
--rw-r--r--   0        0        0    25271 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/diff/imxDiff.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/area/__init__.py
--rw-r--r--   0        0        0      657 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/area/area.py
--rw-r--r--   0        0        0      638 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/area/areaClassifiedTypeEnum.py
--rw-r--r--   0        0        0     5590 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/area/areaClassifier.py
--rw-r--r--   0        0        0     3120 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/area/imxProjectArea.py
--rw-r--r--   0        0        0     8875 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/imx.py
--rw-r--r--   0        0        0     3660 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/models/ImxRailConnectionInfo.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/models/__init__.py
--rw-r--r--   0        0        0      753 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/models/imxEnums.py
--rw-r--r--   0        0        0     1002 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/models/imxGeometry.py
--rw-r--r--   0        0        0    10192 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/models/imxMetadata.py
--rw-r--r--   0        0        0     5675 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/models/imxPuic.py
--rw-r--r--   0        0        0      885 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/models/imxRelation.py
--rw-r--r--   0        0        0     4168 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/domain/models/imxSituations.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/__init__.py
--rw-r--r--   0        0        0    15065 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/imxGraph.py
--rw-r--r--   0        0        0    10886 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/imxGraphBuilder.py
--rw-r--r--   0        0        0    13194 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/imxGraphJunction.py
--rw-r--r--   0        0        0    12682 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/imxGraphModels.py
--rw-r--r--   0        0        0      484 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/imxGraphSituationProtocol.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/queries/__init__.py
--rw-r--r--   0        0        0      283 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/queries/graphQueries.py
--rw-r--r--   0        0        0      473 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/queries/imxGraphProtocol.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/queries/objectRouteQuery.py
--rw-r--r--   0        0        0     4007 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/graph/queries/sectionGeometryQuery.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/repo/__init__.py
--rw-r--r--   0        0        0    24991 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/repo/imxRepo.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/repo/tree/__init__.py
--rw-r--r--   0        0        0     1199 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/repo/tree/imxTopoTreeObject.py
--rw-r--r--   0        0        0     8332 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/repo/tree/imxTreeObject.py
--rw-r--r--   0        0        0     4132 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/repo/tree/objectTree.py
--rw-r--r--   0        0        0     2804 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/repo/tree/objectTreeProtocol.py
--rw-r--r--   0        0        0        0 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/report/__init__.py
--rw-r--r--   0        0        0     1972 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/report/file_info.py
--rw-r--r--   0        0        0     3951 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/report/imxObjectDisplay.py
--rw-r--r--   0        0        0     4206 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/report/refDisplay.py
--rw-r--r--   0        0        0       56 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/utils/__init__.py
--rw-r--r--   0        0        0     2416 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/utils/geodata_gis.py
--rw-r--r--   0        0        0     6487 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/utils/helpers.py
--rw-r--r--   0        0        0     1580 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/utils/log.py
--rw-r--r--   0        0        0     6209 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/utils/shapely_geojson.py
--rw-r--r--   0        0        0    11841 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/utils/shapely_helpers.py
--rw-r--r--   0        0        0     4717 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/imxInsights/utils/xml_helpers.py
--rw-r--r--   0        0        0     2108 2024-05-21 10:52:12.189187 imxinsights-0.0.8.dev2/pyproject.toml
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 imxinsights-0.0.8.dev2/setup.py
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 imxinsights-0.0.8.dev2/PKG-INFO
+-rw-r--r--   0        0        0     5229 2024-05-29 20:17:30.756614 imxinsights-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0     2227 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/custom_puic_config.yaml
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/diff/__init__.py
+-rw-r--r--   0        0        0      904 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/diff/areaStatusEnum.py
+-rw-r--r--   0        0        0     5025 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/diff/change.py
+-rw-r--r--   0        0        0    13116 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/diff/compair.py
+-rw-r--r--   0        0        0      889 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/diff/diffStatusEnum.py
+-rw-r--r--   0        0        0    25790 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/diff/imxDiff.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/area/__init__.py
+-rw-r--r--   0        0        0      657 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/area/area.py
+-rw-r--r--   0        0        0      638 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/area/areaClassifiedTypeEnum.py
+-rw-r--r--   0        0        0     5590 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/area/areaClassifier.py
+-rw-r--r--   0        0        0     3120 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/area/imxProjectArea.py
+-rw-r--r--   0        0        0     8678 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/imx.py
+-rw-r--r--   0        0        0     3660 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/models/ImxRailConnectionInfo.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/models/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/models/imxEnums.py
+-rw-r--r--   0        0        0     1002 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/models/imxGeometry.py
+-rw-r--r--   0        0        0    10192 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/models/imxMetadata.py
+-rw-r--r--   0        0        0     5675 2024-05-29 20:17:30.776614 imxinsights-0.1.0.dev1/imxInsights/domain/models/imxPuic.py
+-rw-r--r--   0        0        0      885 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/domain/models/imxRelation.py
+-rw-r--r--   0        0        0     4168 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/domain/models/imxSituations.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/__init__.py
+-rw-r--r--   0        0        0    15065 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/imxGraph.py
+-rw-r--r--   0        0        0    10886 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/imxGraphBuilder.py
+-rw-r--r--   0        0        0    13194 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/imxGraphJunction.py
+-rw-r--r--   0        0        0    12682 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/imxGraphModels.py
+-rw-r--r--   0        0        0      484 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/imxGraphSituationProtocol.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/queries/__init__.py
+-rw-r--r--   0        0        0      283 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/queries/graphQueries.py
+-rw-r--r--   0        0        0      473 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/queries/imxGraphProtocol.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/queries/objectRouteQuery.py
+-rw-r--r--   0        0        0     4007 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/graph/queries/sectionGeometryQuery.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/repo/__init__.py
+-rw-r--r--   0        0        0    24991 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/repo/imxRepo.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/repo/tree/__init__.py
+-rw-r--r--   0        0        0     1199 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/repo/tree/imxTopoTreeObject.py
+-rw-r--r--   0        0        0     8332 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/repo/tree/imxTreeObject.py
+-rw-r--r--   0        0        0     4132 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/repo/tree/objectTree.py
+-rw-r--r--   0        0        0     2804 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/repo/tree/objectTreeProtocol.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/report/__init__.py
+-rw-r--r--   0        0        0     1972 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/report/file_info.py
+-rw-r--r--   0        0        0     3951 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/report/imxObjectDisplay.py
+-rw-r--r--   0        0        0     4206 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/report/refDisplay.py
+-rw-r--r--   0        0        0       56 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/utils/__init__.py
+-rw-r--r--   0        0        0     2416 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/utils/geodata_gis.py
+-rw-r--r--   0        0        0     6487 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/utils/helpers.py
+-rw-r--r--   0        0        0     1580 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/utils/log.py
+-rw-r--r--   0        0        0     6209 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/utils/shapely_geojson.py
+-rw-r--r--   0        0        0    11841 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/utils/shapely_helpers.py
+-rw-r--r--   0        0        0     4717 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/imxInsights/utils/xml_helpers.py
+-rw-r--r--   0        0        0     2108 2024-05-29 20:17:30.780614 imxinsights-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 imxinsights-0.1.0.dev1/setup.py
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 imxinsights-0.1.0.dev1/PKG-INFO
```

### Comparing `imxinsights-0.0.8.dev2/README.md` & `imxinsights-0.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/__init__.py` & `imxinsights-0.1.0.dev1/imxInsights/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8-dev2"
+__version__ = "0.1.0-dev1"
 
 from .diff.areaStatusEnum import AreaStatusEnum
 from .diff.change import Change, ChangeList
 from .diff.compair import ImxObjectCompare, ImxPropertyCompare
 from .diff.diffStatusEnum import DiffStatusEnum
 from .diff.imxDiff import ImxDiff
 from .domain.area.areaClassifiedTypeEnum import AreaClassifiedTypeEnum
```

### Comparing `imxinsights-0.0.8.dev2/imxInsights/custom_puic_config.yaml` & `imxinsights-0.1.0.dev1/imxInsights/custom_puic_config.yaml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/diff/areaStatusEnum.py` & `imxinsights-0.1.0.dev1/imxInsights/diff/areaStatusEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/diff/change.py` & `imxinsights-0.1.0.dev1/imxInsights/diff/change.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/diff/compair.py` & `imxinsights-0.1.0.dev1/imxInsights/diff/compair.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/diff/diffStatusEnum.py` & `imxinsights-0.1.0.dev1/imxInsights/diff/diffStatusEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/diff/imxDiff.py` & `imxinsights-0.1.0.dev1/imxInsights/diff/imxDiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,17 +156,17 @@
             columns_with_zero = [_ for _ in list(df.columns) if ".0." in _]
             # replace the .0. and find the non zero'ed colum
             columns_without_zero = [_.replace(".0.", ".") for _ in columns_with_zero]
             columns_to_change = [_ for _ in df.columns if _ in columns_without_zero]
             column_mapping = list(zip(columns_to_change, columns_with_zero))
 
             for item in column_mapping:
-                df[item[1]].replace("", np.nan, inplace=True)
-                df[item[1]].fillna(df[item[0]], inplace=True)
-                df[item[1]].replace(np.nan, "", inplace=True)
+                df[item[1]] = df[item[1]].replace("", np.nan)
+                df[item[1]] = df[item[1]].fillna(df[item[0]])
+                df[item[1]] = df[item[1]].replace(np.nan, "")
                 del df[item[0]]
 
         return df
 
     def pandas_dataframe_dict(self, geometry: Optional[bool] = False) -> Dict[str, pd.DataFrame]:
         """
         Returns a dictionary of all difference as pandas dataframe, key is path of imx object.
@@ -282,14 +282,17 @@
         #####################################
         # todo: refactor below to make more readable
         def create_puic_path(df: pd.DataFrame):
 
             def construct_parent_path(row):
                 parent = row["parent"]
                 if parent:
+                    if "->" in parent:
+                        raise ValueError("The parent has changed. This is not supported and was not intended as a concept.")
+
                     parent_row = df[df["puic"] == parent].iloc[0]
                     temp = construct_parent_path(parent_row) + "." + parent
                     if temp[0] == ".":
                         return temp[1:]
                     return temp
                 else:
                     return ""
@@ -304,129 +307,133 @@
 
                 if path_first == path_last:
                     return path_first + row["parent_path"] + "." + row["puic"] + ".00000." + row["diff_status"]
 
                 return path_first + "." + row["parent_path"] + "." + row["puic"] + ".00000." + path_last + ".00000." + row["diff_status"]
 
             # Apply the function to each row
-            df["parent_path"] = df.apply(construct_parent_path, axis=1)
-            df["new_index"] = df.apply(construct_index, axis=1)
+            if parent_path:
+                df["parent_path"] = df.apply(construct_parent_path, axis=1)
+                df["new_index"] = df.apply(construct_index, axis=1)
 
             max_levels = df["path"].str.count(r"\.") + 1
             max_levels = max_levels.max()
             split_columns = [f"lvl{i + 1}" for i in range(max_levels)]
             df[split_columns] = df["path"].str.split(".", expand=True)
 
-            sorted_df = df.sort_values(by=["new_index"])
-
-            sorted_df.set_index("new_index", inplace=False)
-            sorted_df.reset_index(drop=True, inplace=True)
-            sorted_df = sorted_df[
-                ["new_index", "path", "tag", "puic", "area_status", "diff_status"]
-                + split_columns
-                + ["Metadata.@lifeCycleStatus", "Metadata.@source", "Metadata.@isInService", "Metadata.@registrationTime", "@name"]
-            ]
+            if parent_path:
+                sorted_df = df.sort_values(by=["new_index"])
+                sorted_df.set_index("new_index", inplace=False)
+                sorted_df.reset_index(drop=True, inplace=True)
+
+                sorted_df = sorted_df[
+                    ["new_index", "path", "tag", "puic", "area_status", "diff_status"]
+                    + split_columns
+                    + ["Metadata.@lifeCycleStatus", "Metadata.@source", "Metadata.@isInService", "Metadata.@registrationTime", "@name"]
+                ]
+            else:
+                df.reset_index(drop=True, inplace=True)
+                sorted_df = df
 
             return sorted_df, split_columns
 
         basic_columns = ["path", "tag", "puic", "parent", "area_a", "area_b", "area_status", "diff_status", "@name"]
         metadata_columns = list(set([col for key, df in df_dict.items() for col in df.columns if col.startswith("Metadata")]))
         columns_to_keep = basic_columns + [col for col in metadata_columns if col not in basic_columns]
         dfs_with_selected_columns = {
             key: df[[col for col in columns_to_keep if col in columns_to_keep and col in df.columns]] for key, df in df_dict.items()
         }
         concatenated_df = pd.concat(dfs_with_selected_columns.values())
 
         concatenated_df, split_columns = create_puic_path(concatenated_df)
 
-        overview_sheet = workbook.add_worksheet("meta-overview")
+        if overview:
+            overview_sheet = workbook.add_worksheet("meta-overview")
 
-        tree_not_visible_style = workbook.add_format({"font_color": "#FFFFFF"})
-        created_style = workbook.add_format({"font_color": "red", "bold": True})
-        deleted_style = workbook.add_format({"font_color": "blue", "bold": True, "font_strikeout": True})
-        changed_style = workbook.add_format({"font_color": "green", "bold": True})
-        error_style = workbook.add_format({"font_color": "purple", "bold": True})
-
-        first_after_levels = 5 + len(split_columns)
-
-        overview_sheet.write(0, 0, "index")
-        overview_sheet.write(0, 1, "path")
-        overview_sheet.write(0, 2, "tag")
-        overview_sheet.write(0, 3, "puic")
-        overview_sheet.write(0, 4, "area_status")
-        overview_sheet.write(0, 5, "diff_status")
-        for i in range(6, (6 + len(split_columns))):
-            overview_sheet.write(0, i, f"lvl_{i - len(split_columns)}")
-
-        overview_sheet.write(0, first_after_levels + 1, "@name")
-        overview_sheet.write(0, first_after_levels + 2, "Metadata.@lifeCycleStatus")
-        overview_sheet.write(0, first_after_levels + 3, "Metadata.@source")
-        overview_sheet.write(0, first_after_levels + 4, "Metadata.@isInService")
-        overview_sheet.write(0, first_after_levels + 5, "Metadata.@registrationTime")
-
-        for index, row in concatenated_df.iterrows():
-            index = index + 1
-            status = row["diff_status"]
-            if status == "NO_CHANGE":
-                cell_format = None
-            elif status == "CREATED":
-                cell_format = created_style
-            elif status == "DELETED":
-                cell_format = deleted_style
-            elif status in ["UPDATED", "UPGRADED"]:
-                cell_format = changed_style
-            else:
-                cell_format = error_style
+            tree_not_visible_style = workbook.add_format({"font_color": "#FFFFFF"})
+            created_style = workbook.add_format({"font_color": "red", "bold": True})
+            deleted_style = workbook.add_format({"font_color": "blue", "bold": True, "font_strikeout": True})
+            changed_style = workbook.add_format({"font_color": "green", "bold": True})
+            error_style = workbook.add_format({"font_color": "purple", "bold": True})
+
+            first_after_levels = 5 + len(split_columns)
+
+            overview_sheet.write(0, 0, "index")
+            overview_sheet.write(0, 1, "path")
+            overview_sheet.write(0, 2, "tag")
+            overview_sheet.write(0, 3, "puic")
+            overview_sheet.write(0, 4, "area_status")
+            overview_sheet.write(0, 5, "diff_status")
+            for i in range(6, (6 + len(split_columns))):
+                overview_sheet.write(0, i, f"lvl_{i - len(split_columns)}")
+
+            overview_sheet.write(0, first_after_levels + 1, "@name")
+            overview_sheet.write(0, first_after_levels + 2, "Metadata.@lifeCycleStatus")
+            overview_sheet.write(0, first_after_levels + 3, "Metadata.@source")
+            overview_sheet.write(0, first_after_levels + 4, "Metadata.@isInService")
+            overview_sheet.write(0, first_after_levels + 5, "Metadata.@registrationTime")
+
+            for index, row in concatenated_df.iterrows():
+                index = index + 1
+                status = row["diff_status"]
+                if status == "NO_CHANGE":
+                    cell_format = None
+                elif status == "CREATED":
+                    cell_format = created_style
+                elif status == "DELETED":
+                    cell_format = deleted_style
+                elif status in ["UPDATED", "UPGRADED"]:
+                    cell_format = changed_style
+                else:
+                    cell_format = error_style
 
-            overview_sheet.write(index, 0, index)
-            overview_sheet.write(index, 1, row["path"])
-            overview_sheet.write(index, 2, row["tag"])
-            overview_sheet.write(index, 3, row["puic"])
-            overview_sheet.write(index, 4, row["area_status"])
-            overview_sheet.write(index, 5, row["diff_status"], cell_format)
-
-            overview_sheet.write(index, first_after_levels + 1, str(row["@name"]))
-            overview_sheet.write(index, first_after_levels + 2, str(row["Metadata.@lifeCycleStatus"]))
-            overview_sheet.write(index, first_after_levels + 3, str(row["Metadata.@source"]))
-            overview_sheet.write(index, first_after_levels + 4, str(row["Metadata.@isInService"]))
-            overview_sheet.write(index, first_after_levels + 5, str(row["Metadata.@registrationTime"]))
-
-            for idx, value in enumerate(split_columns, start=1):
-                if idx < len(split_columns):
-                    if row[split_columns[idx]] is None:
-                        overview_sheet.write(index, 5 + idx, row[value], cell_format)
+                overview_sheet.write(index, 0, index)
+                overview_sheet.write(index, 1, row["path"])
+                overview_sheet.write(index, 2, row["tag"])
+                overview_sheet.write(index, 3, row["puic"])
+                overview_sheet.write(index, 4, row["area_status"])
+                overview_sheet.write(index, 5, row["diff_status"], cell_format)
+
+                overview_sheet.write(index, first_after_levels + 1, str(row.get("@name")))
+                overview_sheet.write(index, first_after_levels + 2, str(row.get("Metadata.@lifeCycleStatus", "")))
+                overview_sheet.write(index, first_after_levels + 3, str(row.get("Metadata.@source", "")))
+                overview_sheet.write(index, first_after_levels + 4, str(row.get("Metadata.@isInService", "")))
+                overview_sheet.write(index, first_after_levels + 5, str(row.get("Metadata.@registrationTime", "")))
+
+                for idx, value in enumerate(split_columns, start=1):
+                    if idx < len(split_columns):
+                        if row[split_columns[idx]] is None:
+                            overview_sheet.write(index, 5 + idx, row[value], cell_format)
+                        else:
+                            overview_sheet.write(index, 5 + idx, row[value], tree_not_visible_style)
                     else:
-                        overview_sheet.write(index, 5 + idx, row[value], tree_not_visible_style)
-                else:
-                    overview_sheet.write(index, 5 + idx, row[value], cell_format)
+                        overview_sheet.write(index, 5 + idx, row[value], cell_format)
 
-        overview_sheet.autofit()
+            overview_sheet.autofit()
 
-        for i in range(6, (6 + len(split_columns))):
-            if i == (6 + len(split_columns) - 1):
-                overview_sheet.set_column(i, i, 50)
-            else:
-                overview_sheet.set_column(i, i, 3)
+            for i in range(6, (6 + len(split_columns))):
+                if i == (6 + len(split_columns) - 1):
+                    overview_sheet.set_column(i, i, 50)
+                else:
+                    overview_sheet.set_column(i, i, 3)
 
-        overview_sheet.set_column(1, 2, options={"level": 1, "collapsed": True})
-        overview_sheet.set_tab_color("#6699ff")
+            overview_sheet.set_column(1, 2, options={"level": 1, "collapsed": True})
+            overview_sheet.set_tab_color("#6699ff")
 
         #####################################
 
         puic_ref_display = ImxRefDisplay(self.situation_repo_1, self.situation_repo_2)
         wrapped_text = workbook.add_format({"text_wrap": True})
 
         for key, df in sorted(df_dict.items()):
             logger.info(f"generating sheet {key}")
             # first column order
             column_order_list = ["puic", "path", "tag", "parent", "area_a", "area_b", "area_status", "diff_status", "@name"]
             df = sort_pandas_dataframe_columns(df, column_order_list)
 
-            # todo: get all columns containing a path ".x." and check if one with .0. is present.
-
             # sort on diff status
             df["diff_status"] = pd.Categorical(df["diff_status"], categories=sort_status_list, ordered=True)
             df = df.sort_values("diff_status")
             df = df.reset_index(drop=True)
 
             # make color book 😂
             if colors:
@@ -545,16 +552,14 @@
 
         Args:
             key_based_on_type (bool): Whether to use object type as the key in the dictionary, defaults to False.
 
         Returns:
             (Dict[str, GeoJsonFeatureCollection]): A dictionary of GeoJsonFeatureCollections representing the differences.
         """
-        # TODO: add area and schema geojson
-
         out_dict = {}
         if key_based_on_type:
             for imx_type in self._get_all_types():
                 out_dict[imx_type] = self.as_geojson(imx_type)
 
         for imx_path in self._get_all_paths():
             out_dict[imx_path] = self.as_geojson(imx_path)
```

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/area/area.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/area/area.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/area/areaClassifiedTypeEnum.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/area/areaClassifiedTypeEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/area/areaClassifier.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/area/areaClassifier.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/area/imxProjectArea.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/area/imxProjectArea.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/imx.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/imx.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,15 @@
         if isinstance(gis_service, GisRailDataLayer):
             self._add_km(gis_service)
         elif gis_service is True:
             gis_service = get_gis_rail_data_layer()
             self._add_km(gis_service)
 
     def _add_km(self, gis_layer: GisRailDataLayer):
-        logger.info("add km value to objects in all situations" "warning: this is a temp feature ad will be deleted without deprecation wearings!")
-        logger.info("fetching GIS data")
+        logger.info("add km value to objects in all situations")
 
         # todo: make async
         if self.project is not None:
             if self.project.initial_situation is not None:
                 for item in self.project.initial_situation.tree.objects():
                     self._add_km_to_all_items(item, gis_layer)
             if self.project.new_situation is not None:
@@ -82,15 +81,14 @@
 
     @property
     def imx_version(self) -> str:
         """Returns the IMX version of the file, *read only property*."""
         return self._imx_version
 
     def get_situation_repository(self, situation_type: ImxSituationsEnum) -> Optional[SituationRepo]:
-        # TODO: this can return a project sitution.... gives type errors
         """
         Get a specific situation repository  from an IMX project or situation file.
 
         Args:
             situation_type (ImxSituationsEnum): The IMX situation to get the repo.
 
         Returns:
```

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/models/ImxRailConnectionInfo.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/models/ImxRailConnectionInfo.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/models/imxEnums.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/models/imxEnums.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/models/imxGeometry.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/models/imxGeometry.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/models/imxMetadata.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/models/imxMetadata.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/models/imxPuic.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/models/imxPuic.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/models/imxRelation.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/models/imxRelation.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/domain/models/imxSituations.py` & `imxinsights-0.1.0.dev1/imxInsights/domain/models/imxSituations.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/graph/imxGraph.py` & `imxinsights-0.1.0.dev1/imxInsights/graph/imxGraph.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/graph/imxGraphBuilder.py` & `imxinsights-0.1.0.dev1/imxInsights/graph/imxGraphBuilder.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/graph/imxGraphJunction.py` & `imxinsights-0.1.0.dev1/imxInsights/graph/imxGraphJunction.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/graph/imxGraphModels.py` & `imxinsights-0.1.0.dev1/imxInsights/graph/imxGraphModels.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/graph/queries/sectionGeometryQuery.py` & `imxinsights-0.1.0.dev1/imxInsights/graph/queries/sectionGeometryQuery.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/repo/imxRepo.py` & `imxinsights-0.1.0.dev1/imxInsights/repo/imxRepo.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/repo/tree/imxTopoTreeObject.py` & `imxinsights-0.1.0.dev1/imxInsights/repo/tree/imxTopoTreeObject.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/repo/tree/imxTreeObject.py` & `imxinsights-0.1.0.dev1/imxInsights/repo/tree/imxTreeObject.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/repo/tree/objectTree.py` & `imxinsights-0.1.0.dev1/imxInsights/repo/tree/objectTree.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/repo/tree/objectTreeProtocol.py` & `imxinsights-0.1.0.dev1/imxInsights/repo/tree/objectTreeProtocol.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/report/file_info.py` & `imxinsights-0.1.0.dev1/imxInsights/report/file_info.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/report/imxObjectDisplay.py` & `imxinsights-0.1.0.dev1/imxInsights/report/imxObjectDisplay.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/report/refDisplay.py` & `imxinsights-0.1.0.dev1/imxInsights/report/refDisplay.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/utils/geodata_gis.py` & `imxinsights-0.1.0.dev1/imxInsights/utils/geodata_gis.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/utils/helpers.py` & `imxinsights-0.1.0.dev1/imxInsights/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/utils/log.py` & `imxinsights-0.1.0.dev1/imxInsights/utils/log.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/utils/shapely_geojson.py` & `imxinsights-0.1.0.dev1/imxInsights/utils/shapely_geojson.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/utils/shapely_helpers.py` & `imxinsights-0.1.0.dev1/imxInsights/utils/shapely_helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/imxInsights/utils/xml_helpers.py` & `imxinsights-0.1.0.dev1/imxInsights/utils/xml_helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/pyproject.toml` & `imxinsights-0.1.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.8.dev2/setup.py` & `imxinsights-0.1.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
          'pymdown-extensions',
          'python-dotenv',
          'cryptography',
          'matplotlib'],
  'jupyter': ['jupyterlab', 'pygwalker']}
 
 setup(name='imxInsights',
-      version='0.0.8.dev2',
+      version='0.1.0.dev1',
       description='python imx insights module to get information from imx files',
       author=None,
       author_email='Hzd <Hazedd@users.noreply.github.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `imxinsights-0.0.8.dev2/PKG-INFO` & `imxinsights-0.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imxInsights
-Version: 0.0.8.dev2
+Version: 0.1.0.dev1
 Summary: python imx insights module to get information from imx files
 Author-email: Hzd <Hazedd@users.noreply.github.com>
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3.10
```

