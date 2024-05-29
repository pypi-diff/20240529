# Comparing `tmp/french_cities-0.3.3.tar.gz` & `tmp/french_cities-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.3.3.tar", max compression
+gzip compressed data, was "french_cities-0.3.4.tar", max compression
```

## Comparing `french_cities-0.3.3.tar` & `french_cities-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10260 2024-05-07 16:45:25.659349 french_cities-0.3.3/README.fr.md
--rw-r--r--   0        0        0     8729 2024-05-07 16:45:25.659349 french_cities-0.3.3/README.md
--rw-r--r--   0        0        0      477 2024-05-07 16:45:25.663349 french_cities-0.3.3/french_cities/__init__.py
--rw-r--r--   0        0        0    31778 2024-05-07 16:45:25.663349 french_cities-0.3.3/french_cities/city_finder.py
--rw-r--r--   0        0        0    10968 2024-05-07 16:45:25.663349 french_cities-0.3.3/french_cities/departement_finder.py
--rw-r--r--   0        0        0      519 2024-05-07 16:45:25.663349 french_cities-0.3.3/french_cities/utils.py
--rw-r--r--   0        0        0     8302 2024-05-07 16:45:25.663349 french_cities-0.3.3/french_cities/vintage.py
--rw-r--r--   0        0        0     1308 2024-05-07 16:45:25.663349 french_cities-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    20579 1970-01-01 00:00:00.000000 french_cities-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    10260 2024-05-29 20:17:27.103324 french_cities-0.3.4/README.fr.md
+-rw-r--r--   0        0        0     8729 2024-05-29 20:17:27.103324 french_cities-0.3.4/README.md
+-rw-r--r--   0        0        0      477 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/__init__.py
+-rw-r--r--   0        0        0    31689 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/city_finder.py
+-rw-r--r--   0        0        0    11143 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      805 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/utils.py
+-rw-r--r--   0        0        0     8302 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/vintage.py
+-rw-r--r--   0        0        0     1358 2024-05-29 20:17:27.103324 french_cities-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    20579 1970-01-01 00:00:00.000000 french_cities-0.3.4/PKG-INFO
```

### Comparing `french_cities-0.3.3/README.fr.md` & `french_cities-0.3.4/README.fr.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.3.3/README.md` & `french_cities-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.3.3/french_cities/city_finder.py` & `french_cities-0.3.4/french_cities/city_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from geopy.geocoders import Nominatim
 except ModuleNotFoundError:
     pass
 
 
 from french_cities.vintage import set_vintage
 from french_cities.departement_finder import find_departements
-from french_cities.utils import init_pynsee
+from french_cities.utils import init_pynsee, patch_the_patch
 
 
 logger = logging.getLogger(__name__)
 
 
 def find_city(
     df: pd.DataFrame,
@@ -192,17 +192,15 @@
             )  # Neuville-Housset (La) -> Neuville-Housset
             .str.upper()
             .apply(unidecode)  # A voir si on conserve
             .str.split(r"\W+")
             .str.join(" ")
             .str.replace(r"(^|\s)(ST)\s", " SAINT ", regex=True)
             .str.replace(r"(^|\s)(STE)\s", " SAINTE ", regex=True)
-            .str.replace(
-                r"[0-9]* ?EME KM", "", regex=True
-            )  # TAMPON 14EME KM
+            .str.replace(r"[0-9]* ?EME KM", "", regex=True)  # TAMPON 14EME KM
             .str.strip(" ")
             .str.replace(r" ?CEDEX$", "", regex=True)  # LOOS CEDEX -> LOOS
         )
 
     # Control which configuration can be used
     # Note that the order is relevant here, as this will determine the result's
     # preference
@@ -272,17 +270,15 @@
             if isinstance(x, str) and x.startswith("candidat_")
         ]
 
         ix = addresses[
             np.all(
                 [addresses[col].isnull() for col in cols_candidates], axis=0
             )
-            & np.all(
-                [addresses[col].notnull() for col in components], axis=0
-            )
+            & np.all([addresses[col].notnull() for col in components], axis=0)
         ].index
         if len(ix) == 0:
             addresses[f"candidat_{k+1}"] = np.nan
             continue
 
         temp_addresses = addresses.loc[ix].drop(cols_candidates, axis=1)
         temp_addresses = temp_addresses.drop_duplicates().fillna("")
@@ -301,17 +297,15 @@
             list_map(temp_addresses.copy(), components).to_frame("full")
         )
         temp_addresses = temp_addresses.drop_duplicates("full", keep="first")
 
         if "full" in set(addresses.columns):
             addresses = addresses.drop("full", axis=1)
         addresses = addresses.join(
-            list_map(addresses.fillna("").copy(), components).to_frame(
-                "full"
-            )
+            list_map(addresses.fillna("").copy(), components).to_frame("full")
         )
 
         results_api = _query_BAN_csv_geocoder(
             addresses=temp_addresses,
             components=components,
             session=session,
             dep=dep,
@@ -663,17 +657,15 @@
             "setting: the querying of cities using coordinates WILL have "
             "approximative results."
         )
 
     com = get_geodata("ADMINEXPRESS-COG-CARTO.LATEST:commune")
     com = gpd.GeoDataFrame(com).set_crs("EPSG:3857")
 
-    transformer = Transformer.from_crs(
-        epsg, 3857, accuracy=1, always_xy=True
-    )
+    transformer = Transformer.from_crs(epsg, 3857, accuracy=1, always_xy=True)
 
     temp = transformer.transform(df[x].tolist(), df[y].tolist())
     temp = gpd.GeoSeries(
         gpd.points_from_xy(x=temp[0], y=temp[1], crs=3857),
         name="geometry",
         index=df.index,
     )
@@ -727,18 +719,19 @@
         ("type", (None, "municipality")),
         ("result_columns", (None, "full")),
         ("result_columns", (None, "result_score")),
         ("result_columns", (None, "result_city")),
         ("result_columns", (None, "result_citycode")),
     ]
 
-    r = session.post(
-        "https://api-adresse.data.gouv.fr/search/csv/",
-        files=files,
-    )
+    with patch_the_patch():
+        r = session.post(
+            "https://api-adresse.data.gouv.fr/search/csv/",
+            files=files,
+        )
     if not r.ok:
         raise Exception(
             f"Failed to query BAN's API with {files=} - response was {r}"
         )
 
     logger.info("résultat obtenu")
 
@@ -927,17 +920,17 @@
     results_api["result_city"] = (
         results_api["result_city"]
         .str.upper()
         .apply(unidecode)
         .str.split(r"\W+")
         .str.join(" ")
     )
-    results_api["score"] = results_api[
-        ["city_cleaned", "result_city"]
-    ].apply(lambda xy: fuzz.token_set_ratio(*xy), axis=1)
+    results_api["score"] = results_api[["city_cleaned", "result_city"]].apply(
+        lambda xy: fuzz.token_set_ratio(*xy), axis=1
+    )
 
     ix = results_api[
         # Either a good fuzzy match
         (
             (results_api["city_cleaned"] != "")
             & (results_api["score"] > fuzzymatch_threshold)
         )
@@ -946,29 +939,26 @@
         | (
             (results_api["city_cleaned"] != "")
             & (results_api["result_score"] > ban_score_threshold_city_known)
         )
         # Or a goodish match on BAN but no available city label:
         | (
             (results_api["city_cleaned"] == "")
-            & (
-                results_api["result_score"]
-                > ban_score_threshold_city_unknown
-            )
+            & (results_api["result_score"] > ban_score_threshold_city_unknown)
         )
     ].index
 
     if rename_candidat in addresses.columns:
         results_api = results_api.loc[ix, ["full", "result_citycode"]]
         addresses = addresses.merge(results_api, on="full", how="left")
         ix = addresses[addresses.result_citycode.notnull()].index
         addresses.loc[ix, rename_candidat] = addresses.loc[
             ix, "result_citycode"
         ]
         addresses = addresses.drop("result_citycode", axis=1)
 
     else:
-        results_api = results_api.loc[
-            ix, ["full", "result_citycode"]
-        ].rename({"result_citycode": rename_candidat}, axis=1)
+        results_api = results_api.loc[ix, ["full", "result_citycode"]].rename(
+            {"result_citycode": rename_candidat}, axis=1
+        )
         addresses = addresses.merge(results_api, on="full", how="left")
     return addresses
```

### Comparing `french_cities-0.3.3/french_cities/departement_finder.py` & `french_cities-0.3.4/french_cities/departement_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import time
 from tqdm import tqdm
 from pebble import ThreadPool
 from pynsee.localdata import get_area_list
 from rapidfuzz import fuzz, process
 from unidecode import unidecode
 
-from french_cities.utils import init_pynsee
+from french_cities.utils import init_pynsee, patch_the_patch
 
 
 logger = logging.getLogger(__name__)
 
 
 def _process_departements_from_postal(
     df: pd.DataFrame, source: str, alias: str, session: Session = None
@@ -53,33 +53,41 @@
         session = CachedSession(
             allowable_methods=("GET", "POST"),
             expire_after=timedelta(days=30),
         )
 
     postal_codes = df[[source]].drop_duplicates(keep="first")
     files = [
-        ("data", postal_codes.to_csv(index=False)),
+        (
+            "data",
+            (
+                "data.csv",
+                postal_codes.to_csv(index=False, encoding="utf8"),
+                "text/csv; charset=utf-8",
+            ),
+        ),
         ("postcode", (None, source)),
         ("result_columns", (None, source)),
         ("result_columns", (None, "result_context")),
     ]
-    r = session.post(
-        # recherche grâce à l'API de la BAN
-        "https://api-adresse.data.gouv.fr/search/csv/",
-        files=files,
-    )
+
+    with patch_the_patch():
+        r = session.post(
+            # recherche grâce à l'API de la BAN
+            "https://api-adresse.data.gouv.fr/search/csv/",
+            files=files,
+        )
+
     if not r.ok:
         raise Exception(
             f"Failed to query BAN's API with {files=} - response was {r}"
         )
     result = pd.read_csv(io.BytesIO(r.content), dtype=str)
     result[alias] = (
-        result["result_context"]
-        .str.split(",", expand=True)[0]
-        .str.strip(" ")
+        result["result_context"].str.split(",", expand=True)[0].str.strip(" ")
     )
     result = result.drop("result_context", axis=1)
 
     # where code is unknown, use Christian Quest Dataset with Cedex codes and
     # OpenDataSoft API (v2.1 contrairement à la doc disponible) en Freemium
     # https://www.data.gouv.fr/fr/datasets/liste-des-cedex/#_
     # https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr
@@ -157,17 +165,15 @@
                 r" CEDEX", ""
             )
             results_cedex["score"] = results_cedex[
                 ["libelle", "nom_com"]
             ].apply(lambda xy: fuzz.token_set_ratio(*xy), axis=1)
 
             results_cedex = results_cedex.sort_values([source, "score"])
-            results_cedex = results_cedex.drop_duplicates(
-                source, keep="last"
-            )
+            results_cedex = results_cedex.drop_duplicates(source, keep="last")
             results_cedex = results_cedex.drop(
                 ["nom_com", "score", "libelle"], axis=1
             )
             results_cedex = results_cedex.drop_duplicates()
 
             results_cedex = _process_departements_from_insee_code(
                 results_cedex,
```

### Comparing `french_cities-0.3.3/french_cities/vintage.py` & `french_cities-0.3.4/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.3.3/pyproject.toml` & `french_cities-0.3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.3.3"
+version = "0.3.4"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "GPL-3.0-or-later"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
@@ -37,12 +37,14 @@
 [tool.poetry.extras]
 full = ["geopy"]
 
 [tool.poetry.group.dev.dependencies]
 spyder = "^5.4.3"
 pytest = "^7.4.0"
 licensecheck = "^2024.2"
+pyqt5-qt5 = "5.15.2"
+pyqtwebengine-qt5 = "5.15.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `french_cities-0.3.3/PKG-INFO` & `french_cities-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.3.3
+Version: 0.3.4
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: GPL-3.0-or-later
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.9,<4.0
```

