# Comparing `tmp/abses-0.6.6.tar.gz` & `tmp/abses-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.6.6.tar", max compression
+gzip compressed data, was "abses-0.6.7.tar", max compression
```

## Comparing `abses-0.6.6.tar` & `abses-0.6.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.6/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.6/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.6/README.md
--rw-r--r--   0        0        0     1131 2024-05-19 13:14:11.539321 abses-0.6.6/abses/__init__.py
--rw-r--r--   0        0        0    11469 2024-05-19 09:46:33.897240 abses-0.6.6/abses/_bases/base_container.py
--rw-r--r--   0        0        0     2598 2024-05-18 08:54:14.557507 abses-0.6.6/abses/_bases/bases.py
--rw-r--r--   0        0        0     3124 2024-05-16 03:43:18.344259 abses-0.6.6/abses/_bases/components.py
--rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.6/abses/_bases/dynamic.py
--rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.6/abses/_bases/errors.py
--rw-r--r--   0        0        0     1564 2024-05-16 11:19:52.124908 abses-0.6.6/abses/_bases/logging.py
--rw-r--r--   0        0        0     6575 2024-05-16 09:25:00.885690 abses-0.6.6/abses/_bases/modules.py
--rw-r--r--   0        0        0     3157 2024-05-18 14:49:08.436242 abses-0.6.6/abses/_bases/objects.py
--rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.6/abses/_bases/states.py
--rw-r--r--   0        0        0    10588 2024-05-19 10:17:00.008167 abses-0.6.6/abses/actor.py
--rw-r--r--   0        0        0     5534 2024-05-19 09:46:33.898054 abses-0.6.6/abses/cells.py
--rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.6/abses/conf/__init__.py
--rw-r--r--   0        0        0      311 2024-05-16 10:46:33.609412 abses-0.6.6/abses/conf/default.yaml
--rw-r--r--   0        0        0    11590 2024-05-19 13:10:29.734790 abses-0.6.6/abses/container.py
--rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.6/abses/decision.py
--rw-r--r--   0        0        0    16424 2024-05-16 12:59:51.694497 abses-0.6.6/abses/experiment.py
--rw-r--r--   0        0        0     3845 2024-05-19 13:10:29.735156 abses-0.6.6/abses/human.py
--rw-r--r--   0        0        0    22297 2024-05-19 13:10:29.735424 abses-0.6.6/abses/links.py
--rw-r--r--   0        0        0    15614 2024-05-19 09:46:33.899490 abses-0.6.6/abses/main.py
--rw-r--r--   0        0        0     8295 2024-05-19 09:46:33.899859 abses-0.6.6/abses/move.py
--rw-r--r--   0        0        0    12661 2024-05-19 05:49:39.650125 abses-0.6.6/abses/nature.py
--rw-r--r--   0        0        0    30977 2024-05-19 09:46:33.900107 abses-0.6.6/abses/patch.py
--rw-r--r--   0        0        0     8193 2024-05-17 02:47:03.678593 abses-0.6.6/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.6/abses/selection.py
--rw-r--r--   0        0        0    13800 2024-05-19 09:46:33.900478 abses-0.6.6/abses/sequences.py
--rw-r--r--   0        0        0    15523 2024-05-16 08:29:09.798671 abses-0.6.6/abses/time.py
--rw-r--r--   0        0        0      969 2024-05-19 09:46:33.900596 abses-0.6.6/abses/tools/data.py
--rw-r--r--   0        0        0     6780 2024-05-19 09:46:33.901051 abses-0.6.6/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.6/abses/tools/regex.py
--rw-r--r--   0        0        0     1205 2024-05-19 09:46:33.901287 abses-0.6.6/abses/tools/viz.py
--rw-r--r--   0        0        0     4046 2024-05-19 13:10:29.735954 abses-0.6.6/abses/viz/viz_actors.py
--rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.6/abses/viz/viz_model.py
--rw-r--r--   0        0        0     1709 2024-05-19 09:46:33.901856 abses-0.6.6/abses/viz/viz_nature.py
--rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.6/data/.DS_Store
--rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.6/data/YR_cities.zip
--rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.6/data/farmland.tif
--rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.6/data/irr_lands.csv
--rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.6/data/precipitation.nc
--rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.6/icons/fa-regular-400.otf
--rw-r--r--   0        0        0     2784 2024-05-19 13:14:11.538040 abses-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     7262 1970-01-01 00:00:00.000000 abses-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.7/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.7/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.7/README.md
+-rw-r--r--   0        0        0     1082 2024-05-29 02:46:49.169573 abses-0.6.7/abses/__init__.py
+-rw-r--r--   0        0        0    11469 2024-05-19 09:46:33.897240 abses-0.6.7/abses/_bases/base_container.py
+-rw-r--r--   0        0        0     2598 2024-05-18 08:54:14.557507 abses-0.6.7/abses/_bases/bases.py
+-rw-r--r--   0        0        0     3282 2024-05-29 01:55:32.022487 abses-0.6.7/abses/_bases/components.py
+-rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.7/abses/_bases/dynamic.py
+-rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.7/abses/_bases/errors.py
+-rw-r--r--   0        0        0     1564 2024-05-16 11:19:52.124908 abses-0.6.7/abses/_bases/logging.py
+-rw-r--r--   0        0        0     6575 2024-05-16 09:25:00.885690 abses-0.6.7/abses/_bases/modules.py
+-rw-r--r--   0        0        0     3157 2024-05-28 12:41:48.289253 abses-0.6.7/abses/_bases/objects.py
+-rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.7/abses/_bases/states.py
+-rw-r--r--   0        0        0    10588 2024-05-23 12:16:42.445010 abses-0.6.7/abses/actor.py
+-rw-r--r--   0        0        0     5534 2024-05-19 09:46:33.898054 abses-0.6.7/abses/cells.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.7/abses/conf/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-16 10:46:33.609412 abses-0.6.7/abses/conf/default.yaml
+-rw-r--r--   0        0        0    11723 2024-05-29 02:35:45.569572 abses-0.6.7/abses/container.py
+-rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.7/abses/decision.py
+-rw-r--r--   0        0        0    16424 2024-05-16 12:59:51.694497 abses-0.6.7/abses/experiment.py
+-rw-r--r--   0        0        0     3845 2024-05-19 13:10:29.735156 abses-0.6.7/abses/human.py
+-rw-r--r--   0        0        0    22297 2024-05-19 13:10:29.735424 abses-0.6.7/abses/links.py
+-rw-r--r--   0        0        0    15815 2024-05-28 12:57:03.080474 abses-0.6.7/abses/main.py
+-rw-r--r--   0        0        0     8295 2024-05-23 12:16:54.570938 abses-0.6.7/abses/move.py
+-rw-r--r--   0        0        0    12661 2024-05-19 05:49:39.650125 abses-0.6.7/abses/nature.py
+-rw-r--r--   0        0        0    31017 2024-05-24 03:40:28.801411 abses-0.6.7/abses/patch.py
+-rw-r--r--   0        0        0     8202 2024-05-29 02:45:58.678885 abses-0.6.7/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.7/abses/selection.py
+-rw-r--r--   0        0        0    13928 2024-05-29 02:41:01.736926 abses-0.6.7/abses/sequences.py
+-rw-r--r--   0        0        0    15523 2024-05-28 12:39:27.070320 abses-0.6.7/abses/time.py
+-rw-r--r--   0        0        0      969 2024-05-23 11:28:15.720978 abses-0.6.7/abses/tools/data.py
+-rw-r--r--   0        0        0     6780 2024-05-28 12:39:41.192474 abses-0.6.7/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.7/abses/tools/regex.py
+-rw-r--r--   0        0        0     1205 2024-05-19 09:46:33.901287 abses-0.6.7/abses/tools/viz.py
+-rw-r--r--   0        0        0     4046 2024-05-28 12:41:42.378154 abses-0.6.7/abses/viz/viz_actors.py
+-rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.7/abses/viz/viz_model.py
+-rw-r--r--   0        0        0     1709 2024-05-19 09:46:33.901856 abses-0.6.7/abses/viz/viz_nature.py
+-rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.7/data/.DS_Store
+-rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.7/data/YR_cities.zip
+-rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.7/data/farmland.tif
+-rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.7/data/irr_lands.csv
+-rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.7/data/precipitation.nc
+-rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.7/icons/fa-regular-400.otf
+-rw-r--r--   0        0        0     2784 2024-05-29 02:44:08.218338 abses-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     7262 1970-01-01 00:00:00.000000 abses-0.6.7/PKG-INFO
```

### Comparing `abses-0.6.6/LICENSE` & `abses-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/README.md` & `abses-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/__init__.py` & `abses-0.6.7/abses/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,17 @@
     "ActorsList",
     "PatchCell",
     "perception",
     "alive_required",
     "time_condition",
     "Experiment",
     "load_data",
-    "logger",
 ]
-__version__ = "v0.6.6"
+__version__ = "v0.6.7"
 
-from ._bases.logging import logger
 from .actor import Actor, alive_required, perception
 from .decision import Decision
 from .experiment import Experiment
 from .human import BaseHuman
 from .main import MainModel
 from .nature import BaseNature, PatchCell, PatchModule
 from .sequences import ActorsList
```

### Comparing `abses-0.6.6/abses/_bases/base_container.py` & `abses-0.6.7/abses/_bases/base_container.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/_bases/bases.py` & `abses-0.6.7/abses/_bases/bases.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/_bases/components.py` & `abses-0.6.7/abses/_bases/components.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,7 +100,14 @@
                 Model's parameters to be added as component's arguments.
         """
         args_set = set(make_list(args))
         for arg in args_set:
             if arg not in self.params:
                 raise KeyError(f"Argument {arg} not found.")
             self._args.add(arg)
+
+    @property
+    def datasets(self) -> DictConfig:
+        """Get the data source configurations."""
+        return self._model.datasets
+
+    ds = datasets
```

### Comparing `abses-0.6.6/abses/_bases/dynamic.py` & `abses-0.6.7/abses/_bases/dynamic.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/_bases/logging.py` & `abses-0.6.7/abses/_bases/logging.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/_bases/modules.py` & `abses-0.6.7/abses/_bases/modules.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/_bases/objects.py` & `abses-0.6.7/abses/_bases/objects.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/_bases/states.py` & `abses-0.6.7/abses/_bases/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/actor.py` & `abses-0.6.7/abses/actor.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/cells.py` & `abses-0.6.7/abses/cells.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/container.py` & `abses-0.6.7/abses/container.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if unique_id is None:
             unique_id = f"{breed}[{self._unique_ids[breed]}]"
             self._unique_ids[breed] += 1
         if not isinstance(unique_id, (int, str)):
             raise ABSESpyError(
                 f"Unique ID should be an integer or string, got {type(unique_id)}."
             )
-        if unique_id in self.get().array("unique_id"):
+        if unique_id in set(self.get().array("unique_id")):
             raise ABSESpyError(f"Unique ID {unique_id} already exists.")
         return unique_id
 
     def _check_crs(self, gdf: gpd.GeoDataFrame) -> bool:
         if gdf.crs:
             gdf.to_crs(self.crs, inplace=True)
         else:
@@ -216,14 +216,15 @@
 
     def new_from_gdf(
         self,
         gdf: gpd.GeoDataFrame,
         unique_id: Optional[str] = None,
         agent_cls: type[Actor] = Actor,
         attrs: IncludeFlag = False,
+        **kwargs,
     ) -> ActorsList[Actor]:
         """Create actors from a `geopandas.GeoDataFrame` object.
 
         Parameters:
             gdf:
                 The `geopandas.GeoDataFrame` object to convert.
             unique_id:
@@ -251,15 +252,20 @@
         set_attributes = clean_attrs(gdf.columns, attrs, exclude=geo_col)
         if not isinstance(set_attributes, dict):
             set_attributes = {col: col for col in set_attributes}
         # 创建主体
         agents = []
         for index, row in gdf.iterrows():
             geometry = row[geo_col]
-            new_agent = self._new_one(geometry=geometry, unique_id=index)
+            new_agent = self._new_one(
+                geometry=geometry,
+                unique_id=index,
+                agent_cls=agent_cls,
+                **kwargs,
+            )
             new_agent.crs = self.crs
 
             for col, name in set_attributes.items():
                 setattr(new_agent, name, row[col])
             agents.append(new_agent)
         # 添加主体到模型容器里
         self.add(agents)
```

### Comparing `abses-0.6.6/abses/decision.py` & `abses-0.6.7/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/experiment.py` & `abses-0.6.7/abses/experiment.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/human.py` & `abses-0.6.7/abses/human.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/links.py` & `abses-0.6.7/abses/links.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/main.py` & `abses-0.6.7/abses/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,14 +299,22 @@
         """The global parameters of this model."""
         return self.settings.get("model", DictConfig({}))
 
     # alias for model's parameters
     p = params
 
     @property
+    def datasets(self) -> DictConfig:
+        """All datasets in the model."""
+        return self.settings.get("ds", DictConfig({}))
+
+    # alias for model's datasets
+    ds = datasets
+
+    @property
     def breeds(self) -> Dict[str, Type[Actor]]:
         """All breeds in the model."""
         return self._breeds
 
     @breeds.setter
     def breeds(self, breed: Type[Actor]) -> None:
         """Register a new breed of agents in the model."""
```

### Comparing `abses-0.6.6/abses/move.py` & `abses-0.6.7/abses/move.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/nature.py` & `abses-0.6.7/abses/nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/patch.py` & `abses-0.6.7/abses/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 """PatchModule class
 """
 from __future__ import annotations
 
 import copy
 import functools
+from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterator,
     Literal,
@@ -198,26 +199,26 @@
             module.mask = xda.notnull().to_numpy()
         if apply_raster:
             module.apply_raster(xda.to_numpy(), attr_name=attr_name, **kwargs)
         return module
 
     def from_vector(
         self,
-        vector_file: str | gpd.GeoDataFrame,
+        vector_file: str | Path | gpd.GeoDataFrame,
         resolution: Tuple[float, float] | float,
         model: MainModel[Any, Any],
         module_cls: Optional[Type[PatchModule]] = None,
         name: str | None = None,
         attr_name: Optional[str] = None,
         apply_raster: bool = False,
         masked: bool = True,
         cell_cls: type[PatchCell] = PatchCell,
     ) -> PatchModule:
         """Create a layer module from a shape file."""
-        if isinstance(vector_file, str):
+        if isinstance(vector_file, (str, Path)):
             gdf = gpd.read_file(vector_file)
         elif isinstance(vector_file, gpd.GeoDataFrame):
             gdf = vector_file
         else:
             raise TypeError(f"Unsupported vector {type(vector_file)}.")
         if attr_name is None:
             gdf, attr_name = gdf.reset_index(), "index"
```

### Comparing `abses-0.6.6/abses/random.py` & `abses-0.6.7/abses/random.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from __future__ import annotations
 
 from itertools import combinations
 from typing import (
     TYPE_CHECKING,
     Any,
+    Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Tuple,
     Type,
     Union,
@@ -194,24 +195,24 @@
             others, remain_size, replace=False
         )
         return self._to_actors_list([*first_chosen, *second_chosen])
 
     def new(
         self,
         actor_cls: Type[Actor],
-        num: int = 1,
-        replace: bool = False,
-        prob: np.ndarray | None = None,
+        actor_attrs: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> ActorsList[Actor]:
         """Randomly creating new agents for a given actor type."""
-        cells = self.choice(as_list=True, size=num, replace=replace, prob=prob)
+        if actor_attrs is None:
+            actor_attrs = {}
+        cells = self.choice(as_list=True, **kwargs)
         objs = cells.apply(
             lambda c: c.agents.new(
-                breed_cls=actor_cls, singleton=True, **kwargs
+                breed_cls=actor_cls, singleton=True, **actor_attrs
             )
         )
         return self._to_actors_list(objs)
 
     def link(
         self, link: str, p: float = 1.0, mutual: bool = True
     ) -> List[Tuple[Actor, Actor]]:
```

### Comparing `abses-0.6.6/abses/selection.py` & `abses-0.6.7/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/sequences.py` & `abses-0.6.7/abses/sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 from abses._bases.errors import ABSESpyError
 from abses.random import ListRandom
 from abses.selection import selecting
 from abses.tools.func import make_list
 from abses.viz.viz_actors import _VizNodeList
 
 if TYPE_CHECKING:
+    from abses._bases.base_container import UniqueID
     from abses.actor import Actor, GeoType, TargetName
     from abses.links import _LinkNode
     from abses.main import MainModel
 
 Selection: TypeAlias = Union[str, Iterable[bool], Dict[str, Any]]
 HOW: TypeAlias = Literal["only", "random", "item"]
 Link = TypeVar("Link", bound="_LinkNode")
@@ -180,15 +181,15 @@
         elif isinstance(selection, (list, tuple, np.ndarray)):
             bool_ = make_list(selection)
         else:
             raise TypeError(f"Invalid selection type {type(selection)}")
         selected = [a for a, s in zip(actors, bool_) if s]
         return ActorsList(self._model, selected)
 
-    def ids(self, ids: Iterable[int]) -> ActorsList[Link]:
+    def ids(self, ids: Iterable[UniqueID] | UniqueID) -> ActorsList[Link]:
         """Subsets ActorsList by a `ids`.
 
         Parameters:
             ids:
                 an iterable id list. List[id], ID is an attr of agent obj.
 
         Returns:
@@ -249,25 +250,26 @@
             ValueError:
                 If the length of the values iterable does not match the length of the sequence.
         """
         self._is_same_length(cast(Sized, values), rep_error=True)
         for agent, val in zip(self, values):
             setattr(agent, attr, val)
 
-    def split(self, where: NDArray[Any]) -> List[NDArray[np.object_]]:
+    def split(self, where: NDArray[Any]) -> List[ActorsList[Link]]:
         """Split agents into N+1 groups.
 
         Parameters:
             where:
                 indexes [size=N] denotes where to split.
 
         Returns:
             np.ndarray: N+1 groups: agents array
         """
-        return np.hsplit(np.array(self), where)
+        split = np.hsplit(np.array(self), where)
+        return [ActorsList(self._model, group) for group in split]
 
     def array(self, attr: str) -> np.ndarray:
         """Convert the specified attribute of all actors to a numpy array.
 
         Parameters:
             attr:
                 The name of the attribute to convert to a numpy array.
@@ -381,15 +383,15 @@
     def _check_crs_consistent(self) -> CRS:
         crs_set = set(self.array("crs"))
         if None in crs_set:
             logger.warning("Some agents don't have a crs.")
             crs_set.remove(None)
         if len(crs_set) > 1:
             raise ValueError(f"More than one crs: {crs_set}.")
-        if len(crs_set) == 0:
+        if not crs_set:
             logger.warning("No crs when init a GeoDataFrame.")
         return crs_set.pop()
 
     @overload
     def summary(self, geometry: bool = True, **kwargs) -> gpd.GeoDataFrame:
         ...
```

### Comparing `abses-0.6.6/abses/time.py` & `abses-0.6.7/abses/time.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/tools/data.py` & `abses-0.6.7/abses/tools/data.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/tools/func.py` & `abses-0.6.7/abses/tools/func.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/tools/regex.py` & `abses-0.6.7/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/tools/viz.py` & `abses-0.6.7/abses/tools/viz.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/viz/viz_actors.py` & `abses-0.6.7/abses/viz/viz_actors.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/viz/viz_model.py` & `abses-0.6.7/abses/viz/viz_model.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/abses/viz/viz_nature.py` & `abses-0.6.7/abses/viz/viz_nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/data/.DS_Store` & `abses-0.6.7/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/data/YR_cities.zip` & `abses-0.6.7/data/YR_cities.zip`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/data/farmland.tif` & `abses-0.6.7/data/farmland.tif`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/data/irr_lands.csv` & `abses-0.6.7/data/irr_lands.csv`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/data/precipitation.nc` & `abses-0.6.7/data/precipitation.nc`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/icons/fa-regular-400.otf` & `abses-0.6.7/icons/fa-regular-400.otf`

 * *Files identical despite different names*

### Comparing `abses-0.6.6/pyproject.toml` & `abses-0.6.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.6.6"
+version = "0.6.7"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 include = [
   "icons/fa-regular-400.otf",
   "abses/conf/**/*.yaml",
```

### Comparing `abses-0.6.6/PKG-INFO` & `abses-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.6.6
+Version: 0.6.7
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abses Version: 0.6.6 Summary: ABSESpy makes it
+Metadata-Version: 2.1 Name: abses Version: 0.6.7 Summary: ABSESpy makes it
 easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.10,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: fiona
 (>1.8) Requires-Dist: fontawesome (>=5) Requires-Dist: geocube (>=0.5.2,<0.6.0)
```

