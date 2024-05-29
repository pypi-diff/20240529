# Comparing `tmp/veg2hab-0.2.2a1.tar.gz` & `tmp/veg2hab-0.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veg2hab-0.2.2a1.tar", max compression
+gzip compressed data, was "veg2hab-0.2.3a0.tar", max compression
```

## Comparing `veg2hab-0.2.2a1.tar` & `veg2hab-0.2.3a0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7626 2024-05-17 17:11:00.254874 veg2hab-0.2.2a1/LICENSE.md
--rw-r--r--   0        0        0    12995 2024-05-17 17:11:00.254874 veg2hab-0.2.2a1/README.md
--rw-r--r--   0        0        0     1328 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/pyproject.toml
--rw-r--r--   0        0        0       72 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/__init__.py
--rw-r--r--   0        0        0     1086 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/__main__.py
--rw-r--r--   0        0        0     6540 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/access_db.py
--rw-r--r--   0        0        0      411 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/constants.py
--rw-r--r--   0        0        0     6408 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/criteria.py
--rw-r--r--   0        0        0     8640 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/definitietabel.py
--rw-r--r--   0        0        0     5151 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/enums.py
--rw-r--r--   0        0        0      576 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/fgr.py
--rw-r--r--   0        0        0    15989 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/habitat.py
--rw-r--r--   0        0        0     6946 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/io/arcgis.py
--rw-r--r--   0        0        0     2673 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/io/cli.py
--rw-r--r--   0        0        0     5305 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/io/common.py
--rw-r--r--   0        0        0     3051 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/main.py
--rw-r--r--   0        0        0    10867 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/mozaiek.py
--rw-r--r--   0        0        0 13900219 2024-05-17 17:11:00.706874 veg2hab-0.2.2a1/veg2hab/package_data/FGR.json
--rw-r--r--   0        0        0    39321 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
--rw-r--r--   0        0        0    19151 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/package_data/opgeschoonde_waswordt.xlsx
--rw-r--r--   0        0        0     2626 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/package_data/veg2hab.pyt
--rw-r--r--   0        0        0    13084 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/validation.py
--rw-r--r--   0        0        0    15272 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/vegetatietypen.py
--rw-r--r--   0        0        0    47885 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/vegkartering.py
--rw-r--r--   0        0        0     4585 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/waswordtlijst.py
--rw-r--r--   0        0        0    14101 1970-01-01 00:00:00.000000 veg2hab-0.2.2a1/PKG-INFO
+-rw-r--r--   0        0        0     7626 2024-05-29 12:27:38.283365 veg2hab-0.2.3a0/LICENSE.md
+-rw-r--r--   0        0        0    13020 2024-05-29 12:27:38.283365 veg2hab-0.2.3a0/README.md
+-rw-r--r--   0        0        0     1316 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/__init__.py
+-rw-r--r--   0        0        0     1086 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/__main__.py
+-rw-r--r--   0        0        0     6513 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/access_db.py
+-rw-r--r--   0        0        0     6016 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/bronnen.py
+-rw-r--r--   0        0        0      566 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/constants.py
+-rw-r--r--   0        0        0    10014 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/criteria.py
+-rw-r--r--   0        0        0     8640 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/definitietabel.py
+-rw-r--r--   0        0        0    14776 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/enums.py
+-rw-r--r--   0        0        0    15989 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/habitat.py
+-rw-r--r--   0        0        0     5217 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/io/arcgis.py
+-rw-r--r--   0        0        0     2736 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/io/cli.py
+-rw-r--r--   0        0        0     5534 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/io/common.py
+-rw-r--r--   0        0        0     3210 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/main.py
+-rw-r--r--   0        0        0    10867 2024-05-29 12:27:57.583485 veg2hab-0.2.3a0/veg2hab/mozaiek.py
+-rw-r--r--   0        0        0 13900219 2024-05-29 12:27:57.635485 veg2hab-0.2.3a0/veg2hab/package_data/FGR.json
+-rw-r--r--   0        0        0    39387 2024-05-29 12:27:57.635485 veg2hab-0.2.3a0/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
+-rw-r--r--   0        0        0    19152 2024-05-29 12:27:57.635485 veg2hab-0.2.3a0/veg2hab/package_data/opgeschoonde_waswordt.xlsx
+-rw-r--r--   0        0        0     3105 2024-05-29 12:27:57.635485 veg2hab-0.2.3a0/veg2hab/package_data/toolbox.pyt
+-rw-r--r--   0        0        0    13084 2024-05-29 12:27:57.635485 veg2hab-0.2.3a0/veg2hab/validation.py
+-rw-r--r--   0        0        0    15272 2024-05-29 12:27:57.635485 veg2hab-0.2.3a0/veg2hab/vegetatietypen.py
+-rw-r--r--   0        0        0    47779 2024-05-29 12:27:57.635485 veg2hab-0.2.3a0/veg2hab/vegkartering.py
+-rw-r--r--   0        0        0     4585 2024-05-29 12:27:57.635485 veg2hab-0.2.3a0/veg2hab/waswordtlijst.py
+-rw-r--r--   0        0        0    14051 1970-01-01 00:00:00.000000 veg2hab-0.2.3a0/PKG-INFO
```

### Comparing `veg2hab-0.2.2a1/LICENSE.md` & `veg2hab-0.2.3a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/README.md` & `veg2hab-0.2.3a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,35 +24,35 @@
 
 veg2hab wordt gedistribueerd via PyPI, waar alle toekomstige versies aan toe worden gevoegd.
 
 ## Installatie instructies
 
 ### Installatie binnen ArcGIS Pro
 
-Gebruik van veg2hab is ontwikkeld voor en getest in ArcGIS Pro versie 3.0 en hoger.
-Installatie vanaf PyPI is veruit het eenvoudigst, en wordt hieronder omschreven:
+Gebruik van veg2hab is ontwikkeld voor en getest in ArcGIS Pro versie 3.0 en hoger. 
+Installatie vanaf PyPI is veruit het eenvoudigst, en wordt hieronder omschreven: 
 
  1. Open ArcGIS Pro
- 2. Maak een nieuwe python environment aan voor veg2hab (de default conda environment is read-only en niet geschikt om veg2hab in te installeren):
-    - Open de 'Package Manager'
+ 2. Maak een nieuwe python environment aan voor veg2hab (de default conda environment is read-only en niet geschikt om veg2hab in te installeren): 
+    - Open de 'Package Manager'  
         <img src="./images/package_manager.png" alt="package manager" width="400"/>
-    - Klik op het tandwiel naast 'Active Environment'
-    - Maak een nieuwe environment aan op een locatie naar keuze. Gebruik als 'Source' de default Environment.
-        <img src="./images/new_environment.png" alt="new python environment" width="400"/>
+    - Klik op het tandwiel naast 'Active Environment'  
+    - Maak een nieuwe environment aan op een locatie naar keuze. Gebruik als 'Source' de default Environment.  
+        <img src="./images/new_environment.png" alt="new python environment" width="400"/>  
         <img src="./images/environment_location.png" alt="location of new environment" width="400"/>
     - Selecteer de environment en druk op 'OK'.
  3. Download en installeer veg2hab:
-    - Klik op 'New notebook'
+    - Klik op 'New notebook'  
         <img src="./images/new_notebook.png" alt="new notebook" width="400"/>
-    - Download veg2hab met het commando `!pip install --upgrade veg2hab`
+    - Download veg2hab met het commando `!pip install --upgrade veg2hab`  
         <img src="./images/notebook_prompts.png" alt="prompts in notebook to install veg2hab" width="400"/>
     - Installeer veg2hab met het commando `import veg2hab`
  4. Installeer de veg2hab Python Toolbox:
     - Gebruik het commando `veg2hab.installatie_instructies()` om de locatie van de toolbox te vinden
-    - Ga naar 'Add Toolbox (file)' en voeg de toolbox toe vanaf de locatie
+    - Ga naar 'Add Toolbox (file)' en voeg de toolbox toe vanaf de locatie  
         <img src="./images/add_toolbox.png" alt="adding the veg2hab Python Toolbox" width="400"/>
 
 Als het goed is, wordt de veg2hab toolbox nu getoond in de Geoprocessing tab:
 
 <img src="./images/geoprocessing_tab.png" alt="geoprocessing tab" width="400"/>
 
 
@@ -67,31 +67,31 @@
 
 ### Gebruik in ArcGIS Pro
 
 De omzetting van veg2hab van vegetatiekarteringen naar habitattypekaarten gebeurt in tools in de veg2hab Python Toolbox. Om de omzetting te doen, dient de gebruiker eerst de betreffende vegetatiekarteringen in te laden als kaart in ArcGIS Pro.
 
 De omzettool komt in twee smaken:
 1. `digitale_standaard`, voor het omzetten van vegetatiekarteringen die de landelijke digitale standaard gebruiken, die bestaat uit een shapefile gecombineerd met een access database. De gebruiker voert in welke vegetatiekarteringen omgezet moet worden en waar de bijhorende access database te vinden is.
-2. `vector_bestand`, voor het omzetten van vegetatiekarteringen die alle benodigde informatie in de shapefile zelf bevatten. Omdat shapefiles geen standaard kolomnamen hebben, dient de gebruiker hier een handvol inputvelden in te vullen, bijvoorbeeld welke kolom de te gebruiken landelijke typologie bevat.
+2. `vector_bestand`, voor het omzetten van vegetatiekarteringen die alle benodigde informatie in de shapefile zelf bevatten. Omdat shapefiles geen standaard kolomnamen hebben, dient de gebruiker hier een handvol inputvelden in te vullen, bijvoorbeeld welke kolom de te gebruiken landelijke typologie bevat. 
 
 Let op:
 - Wanneer de gebruiker beschikt over een access database, raden wij aan de  `digitale_standaard` omzetting te gebruiken, ook als de shapefile alle informatie bevat. Hierbij is de kans op handmatige fouten kleiner.
-- Vegetatiekarteringen die omgezet worden met `vector_bestand` moeten beschikken over een landelijke typologie (SBB, VvN of rVvN).
+- Vegetatiekarteringen die omgezet worden met `vector_bestand` moeten beschikken over een landelijke typologie (SBB, VvN of rVvN). 
 
 
 ### Bronbestanden die veg2hab gebruikt
 
-veg2hab is afhankelijk van verschillende bronbestanden tijdens het omzetten van vegetatiekarteringen.
+veg2hab is afhankelijk van verschillende bronbestanden tijdens het omzetten van vegetatiekarteringen. 
 
-Sommige bestanden zijn landelijk beschikbaar. Deze bestanden worden automatisch mee geïnstalleerd met veg2hab en zijn niet aanpasbaar door de gebruiker:
+Sommige bestanden zijn landelijk beschikbaar. Deze bestanden worden automatisch mee geïnstalleerd met veg2hab en zijn niet aanpasbaar door de gebruiker: 
 
  - [WasWordtLijst](./data/5.%20Was-wordt-lijst-vegetatietypen-en-habitattypen-09-02-2021.xlsx) (versie 09-feb-2021): dit bestand wordt gebruikt om landelijke vegetatietypologieën in elkaar om te zetten
  - [DefinitieTabel](./data/definitietabel%20habitattypen%20(versie%2024%20maart%202009)_0.xls) (versie 24 maart 2009): dit is een samenvatting van de profieldocumenten
  - [Fysisch-Geografische Regio kaart](./data/bronbestanden/FGR.json) (versie 2013, [link naar origineel op Nationaal georegister](https://nationaalgeoregister.nl/geonetwork/srv/dut/catalog.search#/metadata/c8b5668f-c354-42f3-aafc-d15ae54cf170))
-
+  
 Let op: bij volgende versies komen er waarschijnlijk meer bronbestanden bij.
 
 
 
 ## Handleiding voor ontwikkelaars
 ### Lokale ontwikkeling
 Download de git repository:
@@ -120,15 +120,15 @@
 poetry run pytest tests/
 ```
 
 ### Nieuwe release
 1. Zorg ervoor dat de laatste bronbestanden in package_data staan met `poetry run python release.py create-package-data`.
 2. Maak een nieuwe versie met poetry (major, minor, patch): `poetry version {{rule}}`
 3. Pas de [\_\_init\_\_.py](veg2hab/__init__.py) __version__ variabele aan zodat deze overeen komt met de nieuw poetry version
-4. Pas [veg2hab.pyt](veg2hab/package_data/veg2hab.pyt) zodat de nieuwe version in SUPPORTED_VERSIONS staat. Heb je aanpassingen gedaan aan veg2hab.pyt sinds de laatste release, zorg er dan voor dat de `SUPPORTED_VERSIONS = [{{new_version}}]` wordt gezet.
+4. Pas [toolbox.pyt](veg2hab/package_data/toolbox.pyt) zodat de nieuwe version in SUPPORTED_VERSIONS staat. Heb je aanpassingen gedaan aan toolbox.pyt sinds de laatste release, zorg er dan voor dat de `SUPPORTED_VERSIONS = [{{new_version}}]` wordt gezet.
 5. Draai `python release.py check-versions` om te checken dat je geen fouten hebt gemaakt.
 6. Push nu eerst je nieuwe wijzigingen (mochten die er zijn), naar github. (`git add`, `git commit`, `git push`)
 7. Maak een nieuwe tag: `git tag v$(poetry version -s)`
 8. Push de tag naar git `git push origin tag v$(poetry version -s)`
 9. Github actions zal automatisch de nieuwe versie op PyPI zetten.
 
 
@@ -143,18 +143,18 @@
 
 **ElmID**: Een voor ieder vlak uniek ID. Deze kan vanuit de bronkartering komen, maar kan ook nieuw zijn gegenereerd. Dit gebeurt de als ElmID (of een ElmID equivalent zoals OBJECTID) in de bronkartering niet voor ieder vlak uniek is; als dit het geval is is hierover een warning gegeven.
 
 **_Samnvttng**: Weergave van hoeveel procent van het vlak bedekt is met welk habitattype. Dit is een combinatie van alle kolommen `Habtype{i}` en `Perc{i}`.
 
 **_LokVegTyp**: Het in de bronkartering opgegeven lokale vegetatietype, als er een lokaal vegetatietype kolom is opgegeven.
 
-**_LokVrtNar**: Of de oorspronkelijk opgegeven lokale vegetatietypen in de bronkartering primair is vertaald naar SBB, VvN of beide. Als er naar SBB is vertaald, zijn er bijbehorende VvN uit de waswordtlijst gehaald. Als er naar VvN of naar beide is vertaald, is dit niet gedaan.
+**_LokVrtNar**: Of de oorspronkelijk opgegeven lokale vegetatietypen in de bronkartering primair is vertaald naar SBB, VvN of beide. Als er naar SBB is vertaald, zijn er bijbehorende VvN uit de waswordtlijst gehaald. Als er naar VvN of naar beide is vertaald, is dit niet gedaan. 
 
 ### Complex-deel-specifieke kolommen
-**Habtype{i}**: Habitattype van het complex-deel. HXXXX hier betekend dat er menselijk oordeel nodig is over dit complex-deel.
+**Habtype{i}**: Habitattype van het complex-deel. HXXXX hier betekend dat er menselijk oordeel nodig is over dit complex-deel. 
 
 **Perc{i}**: Percentage van het gehele vlak wat door dit complex-deel wordt bedekt.
 
 **Opp{i}**: Oppervlakte van dit complex-deel in m2.
 
 **Kwal{i}**: Kwaliteit van dit complex-deel. Dit kan zijn G (goed), M (matig) of X (nvt).
```

### Comparing `veg2hab-0.2.2a1/pyproject.toml` & `veg2hab-0.2.3a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "veg2hab"
-version = "0.2.2a1"
+version = "0.2.3a0"
 description = "Package voor automatisch omzetten van vegetatiekarteringen naar habitatkaarten"
 authors = ["Spheer.ai <info@spheer.ai>"]
 readme = "README.md"
-license = "LGPLv3"
+license = "LGPLv3" 
 classifiers = [
   "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
 
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -19,21 +19,20 @@
 Issues = "https://github.com/Spheer-ai/veg2hab/issues"
 Source = "https://github.com/Spheer-ai/veg2hab"
 
 [tool.poetry.scripts]
 veg2hab = "veg2hab.__main__:veg2hab"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<4.0"
-pandas = "^1.3.0"
-geopandas = "^0.10.0"
-openpyxl = "^3.1.0"
-xlrd = "^2.0.1"
-pyodbc= "^4.0.1"
-pydantic = "^1.10.0"
+python = ">=3.7,<4.0"
+geopandas = ">=0.10.0"
+openpyxl = ">=3.0.0"
+xlrd = ">=2.0.1"
+pyodbc= ">=4.0.1"
+pydantic = ">=1.0,<2.0"
 setuptools = "<60.0.0"
 pygeos = "^0.14"
 typing-extensions = "4.7.1"
 click = "^8.1.7"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = ">=6.0.0"
```

### Comparing `veg2hab-0.2.2a1/veg2hab/__main__.py` & `veg2hab-0.2.3a0/veg2hab/__main__.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/veg2hab/access_db.py` & `veg2hab-0.2.3a0/veg2hab/access_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     # the pyodb is not officially suppported by pandas, so we suppress that
     # warning:
     with warnings.catch_warnings():
         warnings.simplefilter(action="ignore", category=UserWarning)
         return pd.read_sql(
             f"SELECT {','.join(col_names.keys())} FROM {table_name.value}",
             conn,
-            columns=col_names.keys(),
-        ).astype(col_names)
+            dtype=col_names,
+        )
 
 
 @read_table.register
 def _(folder: Path, table_name: TableNames, col_names: Dict[str, Any]) -> pd.DataFrame:
     return pd.read_csv(
         folder / f"{table_name.value}.csv",
         usecols=list(col_names.keys()),
```

### Comparing `veg2hab-0.2.2a1/veg2hab/definitietabel.py` & `veg2hab-0.2.3a0/veg2hab/definitietabel.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/veg2hab/habitat.py` & `veg2hab-0.2.3a0/veg2hab/habitat.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/veg2hab/io/arcgis.py` & `veg2hab-0.2.3a0/veg2hab/io/arcgis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 import logging
 import os.path
 import random
 import string
-import tempfile
 from pathlib import Path
 from typing import List, Optional
 
 import geopandas as gpd
-from pydantic import validator
 from typing_extensions import Self, override
 
 from .common import AccessDBInputs, Interface, ShapefileInputs
 
 
 class ArcGISInterface(Interface):
-    def _get_temp_dir(self):
-        import arcpy
-
-        if arcpy.env.scratchWorkspace is not None:
-            return os.path.abspath(os.path.join(arcpy.env.scratchWorkspace, ".."))
-        if arcpy.env.scratchFolder is not None:
-            return arcpy.env.scratchFolder
-
-        return tempfile.gettempdir()
-
     def _generate_random_gpkg_name(self, basename: str) -> str:
         import arcpy
 
+        file_location = os.path.abspath(os.path.join(arcpy.env.scratchWorkspace, ".."))
+
         random_name = f"{basename}_{''.join(random.choices(string.ascii_letters + string.digits, k=8))}.gpkg"
-        return os.path.join(self._get_temp_dir(), random_name)
+        return os.path.join(file_location, random_name)
 
     @override
     def shape_id_to_filename(self, shapefile_id: str) -> Path:
         import arcpy
 
         filename = self._generate_random_gpkg_name("vegkart")
 
@@ -123,33 +113,30 @@
 
         # get the description from the field
         param = arcpy.Parameter(
             name=field_name,
             displayName=field_info["description"],
             datatype=datatype,
             parameterType="Required" if is_required else "Optional",
-            direction="Output" if field_name == "output" else "Input",
-            multiValue=field_info.get("type") == "array",
+            direction="Input",
         )
 
         if field_name == "shapefile":
             shapefile_param = param
 
         if field_name == "access_mdb_path":
             param.filter.list = ["mdb", "accdb"]
 
-        if field_name == "output":
-            param.filter.list = ["gpkg"]
-
         if "enum" in field_info.keys():
             param.filter.type = "ValueList"
             param.filter.list = field_info["enum"]
 
         outputs.append(param)
 
+    # TODO: fix this for multi field inputs
     for param in outputs:
         if param.name.endswith("_col"):
             param.parameterDependencies = [shapefile_param.name]
 
     return outputs
 
 
@@ -159,46 +146,17 @@
         as_dict = {p.name: p.valueAsText for p in parameters}
         return cls(**as_dict)
 
     @classmethod
     def to_parameter_list(cls) -> List["arcpy.Parameter"]:
         return _schema_to_param_list(cls.schema())
 
-    @classmethod
-    def update_parameters(cls, parameters: List["arcpy.Parameter"]) -> None:
-        pass
-
 
 class ArcGISShapefileInputs(ShapefileInputs):
     @classmethod
     def from_parameter_list(cls, parameters: List["arcpy.Parameter"]) -> Self:
         as_dict = {p.name: p.valueAsText for p in parameters}
-        for col in ["sbb_col", "vvn_col", "perc_col", "lok_vegtypen_col"]:
-            if as_dict.get(col) is None:
-                as_dict[col] = []
-            else:
-                as_dict[col] = as_dict[col].split(";")
-
         return cls(**as_dict)
 
     @classmethod
     def to_parameter_list(cls) -> List["arcpy.Parameter"]:
         return _schema_to_param_list(cls.schema())
-
-    @classmethod
-    def update_parameters(cls, parameters: List["arcpy.Parameter"]) -> None:
-        as_dict = {p.name: p for p in parameters}
-        if as_dict["vegtype_col_format"].altered:
-            is_multivalue_per_column = (
-                as_dict["vegtype_col_format"].valueAsText == "single"
-            )
-            as_dict["split_char"].enabled = is_multivalue_per_column
-
-            # TODO: ik heb het idee dat dit niks doet, maar moet nog even checken.
-            as_dict["sbb_col"].multiValue = not is_multivalue_per_column
-            as_dict["vvn_col"].multiValue = not is_multivalue_per_column
-            as_dict["perc_col"].multiValue = not is_multivalue_per_column
-            as_dict["lok_vegtypen_col"].multiValue = not is_multivalue_per_column
-
-        if as_dict["sbb_of_vvn"].altered:
-            as_dict["sbb_col"].enabled = as_dict["sbb_of_vvn"].valueAsText != "VvN"
-            as_dict["vvn_col"].enabled = as_dict["sbb_of_vvn"].valueAsText != "SBB"
```

### Comparing `veg2hab-0.2.2a1/veg2hab/io/cli.py` & `veg2hab-0.2.3a0/veg2hab/io/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,21 +26,24 @@
 
 
 def _decorate_click(func: Callable, param_schema: Dict):
     for field_name, field_info in reversed(list(param_schema["properties"].items())):
         is_required = field_name in param_schema["required"]
 
         if field_info.get("format", "") == "path":
-            writable = field_name == "output"
-            param_type = click.Path(exists=False, writable=writable)
-        elif "enum" in field_info:
-            param_type = click.Choice(field_info["enum"])
+            if field_name == "output":
+                param_type = click.Path(exists=False, writable=True)
+            else:
+                param_type = click.Path(exists=True)
         else:
             param_type = str
 
+        if "enum" in field_info:
+            param_type = click.Choice(field_info["enum"])
+
         if is_required:
             func = click.argument(
                 field_name,
                 type=param_type,
                 required=is_required,
             )(func)
         else:
```

### Comparing `veg2hab-0.2.2a1/veg2hab/io/common.py` & `veg2hab-0.2.3a0/veg2hab/io/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
-from typing import ClassVar, List, Optional
+from typing import ClassVar, Optional
 
 import geopandas as gpd
 from pydantic import BaseModel, BaseSettings, Field
 from typing_extensions import List, Literal, Union
 
 
 class AccessDBInputs(BaseModel):
@@ -41,67 +41,67 @@
         extra = "forbid"
 
     label: ClassVar[str] = "vector_bestand"
     description: ClassVar[str] = "Draai veg2hab o.b.v. een vector bestand"
     shapefile: str = Field(
         description="Locatie van de vegetatiekartering",
     )
-    elmid_col: Optional[str] = Field(
-        description="De kolomnaam van de ElementID in de Shapefile; uniek per vlak",
-    )
     vegtype_col_format: Literal["single", "multi"] = Field(
         description='"single" als complexen in 1 kolom zitten of "multi" als er meerdere kolommen zijn',
     )
-    sbb_of_vvn: Literal["SBB", "VvN", "beide"] = Field(
+    sbb_of_vvn: Literal["VvN", "SBB", "beide"] = Field(
         description='"VvN" als VvN de voorname vertaling is vanuit het lokale type, "SBB" voor SBB en "beide" als beide er zijn.'
     )
-    sbb_col: List[str] = Field(
-        default_factory=list,
-        description="SBB kolom(men) (verplicht wanneer het voorname type 'SBB' of 'beide' is)",
-    )
-    vvn_col: List[str] = Field(
-        default_factory=list,
-        description="VvN kolom(men) (verplicht wanneer het voorname type 'VvN' of 'beide' is)",
-    )
-    perc_col: List[str] = Field(
-        default_factory=list,
-        description="Percentage kolom(men) (optioneel)",
-    )
-    lok_vegtypen_col: List[str] = Field(
-        default_factory=list,
-        description="Lokale vegetatietypen kolom(men) (optioneel)",
-    )
-    split_char: Optional[str] = Field(
-        default="+",
-        description='Karakter waarop de complexe vegetatietypen gesplitst moeten worden (voor complexen (bv "16aa2+15aa"))',
+    elmid_col: Optional[str] = Field(
+        description="De kolomnaam van de ElementID in de Shapefile; uniek per vlak",
     )
     datum_col: Optional[str] = Field(
         default=None,
         description="Datum kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
     opmerking_col: Optional[str] = Field(
         default=None,
         description="Opmerking kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
+    sbb_col: Optional[str] = Field(
+        default=None,
+        description="kolomnaam van de SBB vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)",
+    )
+    vvn_col: Optional[str] = Field(
+        default=None,
+        description="kolomnaam van de VvN vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)",
+    )
+    split_char: Optional[str] = Field(
+        default="+",
+        description='karakter waarop de vegetatietypen gesplitst moeten worden (voor complexen (bv "16aa2+15aa")) (wordt bij mutli_col gebruikt om de kolommen te scheiden)',
+    )
+    perc_col: Optional[str] = Field(
+        default=None,
+        description="kolomnaam van de percentage als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))",
+    )
+    lok_vegtypen_col: Optional[str] = Field(
+        default=None,
+        description="kolomnaam van de lokale vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))",
+    )
     output: Optional[Path] = Field(
         default=None,
         description="Output bestand (optioneel), indien niet gegeven wordt er een bestandsnaam gegenereerd",
     )
 
 
 class Veg2HabConfig(BaseSettings):
     class Config:
         env_prefix = "VEG2HAB_"
 
     mozaiek_threshold: Union[int, float] = Field(
-        default=95.0,  # todo number/float
+        default=95.0,
         description="Threshold voor het bepalen of een vlak in het mozaiek ligt",
     )
     mozaiek_als_rand_langs_threshold: Union[int, float] = Field(
-        default=50.0,  # todo number/float
+        default=25.0,
         description="Threshold voor het bepalen of een vlak langs de rand van het mozaiek ligt",
     )
     niet_geautomatiseerde_sbb: List[str] = Field(
         default=[
             "100",
             "200",
             "300",
```

### Comparing `veg2hab-0.2.2a1/veg2hab/main.py` & `veg2hab-0.2.3a0/veg2hab/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 from pathlib import Path
 from textwrap import dedent
 from typing import Union
 
 import geopandas as gpd
 
 from veg2hab import constants
+from veg2hab.bronnen import FGR, LBK, Bodemkaart
 from veg2hab.definitietabel import DefinitieTabel
-from veg2hab.fgr import FGR
 from veg2hab.io.common import AccessDBInputs, Interface, ShapefileInputs
 from veg2hab.vegkartering import Kartering
 from veg2hab.waswordtlijst import WasWordtLijst
 
 
-def installatie_instructies():
+def installation_instructions():
     print(
         dedent(
             f"""
-    Om veg2hab te kunnen draaien, moet de veg2hab toolbox geïnstalleerd worden in ArcGIS Pro.
-    Ga naar "add Python toolbox" in ArcGIS Pro en selecteer het bestand op de volgende locatie:
+    To install the veg2hab toolbox, go to add Python toolbox in ArcGIS Pro and select the file at the following location:
         {constants.TOOLBOX_PYT_PATH}
 """
         )
     )
 
 
 def run(params: Union[AccessDBInputs, ShapefileInputs]):
@@ -36,14 +35,22 @@
 
     logging.info(f"Definitietabel is ingelezen van {constants.DEFTABEL_PATH}")
 
     fgr = FGR(Path(constants.FGR_PATH))
 
     logging.info(f"FGR is ingelezen van {constants.FGR_PATH}")
 
+    bodemkaart = Bodemkaart.from_github()
+
+    logging.info(f"Bodemkaart is ingelezen")
+
+    lbk = LBK.from_github()
+
+    logging.info(f"LBK is ingelezen")
+
     filename = Interface.get_instance().shape_id_to_filename(params.shapefile)
 
     if filename != params.shapefile:
         logging.info(
             f"Tijdelijke versie van {params.shapefile} is opgeslagen in {filename}"
         )
 
@@ -78,15 +85,19 @@
 
     logging.info(f"Was wordt lijst is toegepast op de vegetatie kartering")
 
     kartering.apply_deftabel(deftabel)
 
     logging.info(f"Definitietabel is toegepast op de vegetatie kartering")
 
-    kartering.bepaal_habitatkeuzes(fgr)
+    kartering.bepaal_habitatkeuzes(
+        fgr,
+        bodemkaart,
+        lbk,
+    )
 
     logging.info(f"Mitsen zijn gecheckt")
 
     final_format = kartering.as_final_format()
 
     logging.info("Omzetting is successvol, wordt nu weggeschreven naar een geopackage")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `veg2hab-0.2.2a1/veg2hab/mozaiek.py` & `veg2hab-0.2.3a0/veg2hab/mozaiek.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/veg2hab/package_data/FGR.json` & `veg2hab-0.2.3a0/veg2hab/package_data/FGR.json`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/veg2hab/package_data/opgeschoonde_waswordt.xlsx` & `veg2hab-0.2.3a0/veg2hab/package_data/opgeschoonde_waswordt.xlsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,1197 +1,1197 @@
-00000000: 504b 0304 1400 0000 0800 f00b b158 465a  PK...........XFZ
+00000000: 504b 0304 1400 0000 0800 e254 a758 465a  PK.........T.XFZ
 00000010: c10c 8200 0000 b100 0000 1000 0000 646f  ..............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 4d0b c230 1044 ff4a e9dd 6e55 f020 3120  M..0.D.J..nU. 1 
 00000040: d4a3 e0c9 7b48 3736 9064 4376 85fc 7c53  ....{H76.dCv..|S
 00000050: c18f db3c de30 8cba 15ca 58c4 2377 3586  ...<.0....X.#w5.
 00000060: c4a7 7e11 c947 00b6 0b46 c343 d3a9 1947  ..~..G...F.C...G
 00000070: 251a 6958 1e40 ce79 8b13 d967 c424 b01b  %.iX.@.y...g.$..
 00000080: c703 6015 4c33 ce9b fc1d ecb5 3ae7 1cbc  ..`.L3......:...
 00000090: 35e2 29e9 abb7 8598 9c74 976a 3128 f897  5.)......t.j1(..
 000000a0: 6bf3 8e85 d7bc 1fb6 6ff9 6105 bf93 fa05  k.......o.a.....
-000000b0: 504b 0304 1400 0000 0800 f00b b158 e3e8  PK...........X..
-000000c0: 222f ea00 0000 cb01 0000 1100 0000 646f  "/............do
+000000b0: 504b 0304 1400 0000 0800 e254 a758 3afa  PK.........T.X:.
+000000c0: b57b eb00 0000 cb01 0000 1100 0000 646f  .{............do
 000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6ca5  cProps/core.xml.
-000000e0: 914d 4fc3 300c 86ff ca94 7beb b681 1da2  .MO.0.....{.....
-000000f0: 2e97 214e 2021 3109 c42d 4abc ada2 f950  ..!N !1..-J....P
-00000100: 62d4 eedf 9396 ad03 c18d 63fc 3e7e 6c2b  b.........c.>~l+
-00000110: ad0e 42fb 884f d107 8cd4 615a 8db6 7749  ..B..O....aZ..wI
-00000120: e8b0 6147 a220 0092 3ea2 55a9 cc84 cbe1  ..aG. ..>.U.....
-00000130: de47 ab28 3fe3 0182 d2ef ea80 d054 d51a  .G.(?........T..
-00000140: 2c92 328a 144c c222 2c46 7656 1abd 28c3  ,.2..L.",FvV..(.
-00000150: 47ec 6781 d180 3d5a 7494 a02e 6bb8 b284  G.g...=Zt...k...
-00000160: d1a6 3f1b e664 21c7 d42d d430 0ce5 c067  ..?..d!..-.0...g
-00000170: 2e6f 54c3 ebe3 c3f3 bc7c d1b9 44ca 6964  .oT......|..D.id
-00000180: b235 5ae8 888a 7c94 d345 e134 f62d 7c2b  .5Z...|..E.4.-|+
-00000190: b6e7 d95f 0534 ab3c 41d0 29e0 865d 9217  ..._.4.<A.)..]..
-000001a0: bebd dbdd 33d9 54cd 4d51 dd16 f57a d770  ....3.T.MQ...z.p
-000001b0: c16b c1f9 dbe4 fad1 7f15 5a6f ba7d f70f  .k........Zo.}..
-000001c0: e345 205b f8f5 6ff2 1350 4b03 0414 0000  .E [..o..PK.....
-000001d0: 0008 00f0 0bb1 5899 5c9c 2310 0600 009c  ......X.\.#.....
-000001e0: 2700 0013 0000 0078 6c2f 7468 656d 652f  '......xl/theme/
-000001f0: 7468 656d 6531 2e78 6d6c ed5a 5b73 da38  theme1.xml.Z[s.8
-00000200: 147e efaf d078 67f6 6d0b c636 81b6 b413  .~...xg.m..6....
-00000210: 7369 76db b499 84ed 4e1f 8511 588d 6c79  siv.....N...X.ly
-00000220: 6491 847f bf47 3610 cb96 0ded 924d ba9b  d....G6......M..
-00000230: 3c04 2ce9 fbce 4547 e7e8 3879 f3ee 2e62  <.,...EG..8y...b
-00000240: e886 8894 f278 60d9 2fdb d6bb b72f dee0  .....x`./..../..
-00000250: 5732 2411 4130 19a7 aff0 c00a a54c 5eb5  W2$.A0.......L^.
-00000260: 5a69 00c3 387d c913 12c3 dc82 8b08 4b78  Zi..8}........Kx
-00000270: 14cb d65c e05b 1a2f 23d6 eab4 dbdd 5684  ...\.[./#.....V.
-00000280: 696c a118 4764 607d 5e2c 6840 d054 515a  il..Gd`}^,h@.TQZ
-00000290: 6f5f 20b4 e51f 33f8 15cb 548d 65a3 0113  o_ ...3...T.e...
-000002a0: 5741 26b9 88b4 f2f9 6cc5 fcda de3e 65cf  WA&.....l....>e.
-000002b0: e93a 1d32 816e 301b 5820 7fce 6fa7 e44e  .:.2.n0.X ..o..N
-000002c0: 5a88 e154 c2c4 c06a 673f 566b c7d1 d248  Z..T...jg?Vk...H
-000002d0: 8082 c97d 9405 ba49 f6a3 d315 0832 0d3b  ...}...I.....2.;
-000002e0: 3a9d 58ce 767c f6c4 ed9f 8cca da74 346d  :.X.v|.......t4m
-000002f0: 1ae0 e3f1 7838 b6cb d28b 701c 04e0 51bb  ....x8....p...Q.
-00000300: 9ec2 9df4 6cbf a441 09b4 a369 d064 d8f6  ....l..A...i.d..
-00000310: daae 91a6 aa8d 534f d3f7 7ddf eb9b 689c  ......SO..}...h.
-00000320: 0a8d 5b4f d36b 77dd d38e 89c6 add0 780d  ..[O.kw.......x.
-00000330: bef1 4f87 c3ae 89c6 abd0 74eb 6926 27fd  ..O.......t.i&'.
-00000340: ae6b a4e9 1668 4246 e3eb 7a12 15b5 e540  .k...hBF..z....@
-00000350: d320 0058 7076 d6cc d203 965e 29fa 7594  . .Xpv.....^).u.
-00000360: 1ad9 1dbb dd41 5cf0 58ee 3989 11fe c6c5  .....A\.X.9.....
-00000370: 04d6 69d2 1996 3446 729d 9005 0e00 37c4  ..i...4Fr.....7.
-00000380: d14c 507c af41 b68a e0c2 92d2 5c90 d6cf  .LP|.A......\...
-00000390: 29b5 501a 089a c881 f547 8221 c5dc affd  ).P......G.!....
-000003a0: f597 bbc9 a433 7a9d 7d3a ce6b 947f 69ab  .....3z.}:.k..i.
-000003b0: 01a7 edbb 9bcf 93fc 73e8 e49f a793 d74d  ........s......M
-000003c0: 42ce 70bc 2c09 f1fb 235b 6187 276e 3b13  B.p.,...#[a.'n;.
-000003d0: 723a 1c67 427c cff6 f691 a525 32cf eff9  r:.gB|.....%2...
-000003e0: 0aeb 4e3c 671f 5696 b05d cfcf e49e 8c72  ..N<g.V..].....r
-000003f0: 23bb ddf6 587d f64f 476e 23d7 a9c0 b322  #...X}.OGn#...."
-00000400: d794 4624 459f c82d bae4 1138 b549 0d32  ..F$E..-...8.I.2
-00000410: 133f 089d 8698 6a50 1c02 a409 3196 a186  .?....jP....1...
-00000420: f8b4 c6ac 11e0 137d b7be 08c8 df8d 88f7  .......}........
-00000430: ab6f 9a3d 57a1 5849 da84 f810 461a e29c  .o.=W.XI....F...
-00000440: 73e6 73d1 6cfb 07a5 46d1 f655 bcdc a397  s.s.l...F..U....
-00000450: 5815 0197 18df 34aa 352c c5d6 7895 c0f1  X.....4.5,..x...
-00000460: ad9c 3c1d 1312 cd94 0b06 4186 9724 2612  ..<.......A..$&.
-00000470: a939 7e4d 4813 fe2b a5da fe9c d340 f094  .9~MH..+.....@..
-00000480: 2f24 fa4a 918f 69b3 23a7 7426 cde8 331a  /$.J..i.#.t&..3.
-00000490: c146 af1b 7587 68d2 3c7a fe05 f99c 350a  .F..u.h.<z....5.
-000004a0: 1c91 1b1d 0267 1bb3 4621 8469 bbf0 1eaf  .....g..F!.i....
-000004b0: 248e 9aad c211 2b42 3e62 1936 1a72 b516  $.....+B>b.6.r..
-000004c0: 81b6 71a9 8460 5a12 c6d1 784e d2b4 11fc  ..q..`Z...xN....
-000004d0: 59ac 3593 3e60 c8ec cd91 75ce d691 0e11  Y.5.>`....u.....
-000004e0: 925e 3742 3e62 ce8b 9011 bf1e 8638 4a9a  .^7B>b.......8J.
-000004f0: eda2 7158 04fd 9e5e c349 c1e8 82cb 66fd  ..qX...^.I....f.
-00000500: b87e 86d5 336c 2c8e f747 d417 4ae4 0f26  .~..3l,..G..J..&
-00000510: a73f e932 3407 a39a 5909 bd84 566a 9faa  .?.24...Y...Vj..
-00000520: 8734 3ea8 1e32 0a05 f1b9 1e3e e57a 780a  .4>..2.....>.zx.
-00000530: 3796 c6bc 50ae 827b 01ff d1da 37c2 abf8  7...P..{....7...
-00000540: 82c0 397f 2e7d cfa5 efb9 f43d a1d2 b737  ..9..}.....=...7
-00000550: 237d 67c1 d38b 5bde 466e 5bc4 fbae 31da  #}g...[.Fn[...1.
-00000560: d734 2e28 6357 72cd c8c7 54af 9329 d839  .4.(cWr...T..).9
-00000570: 9fc0 ecfd 683e 9ef1 edfa d924 84af 9a59  ....h>.....$...Y
-00000580: 2d23 1690 4b81 b341 24b8 fc8b caf0 2ac4  -#..K..A$.....*.
-00000590: 09e8 645b 2509 cb54 d365 378a 129e 421b  ..d[%..T.e7...B.
-000005a0: 6ee9 53f5 4a95 d7e5 afb9 28b8 3c5b e4e9  n.S.J.....(.<[..
-000005b0: afa1 743e 2ccf f93c 5fe7 b4cd 0b33 43b7  ..t>,..<_....3C.
-000005c0: 724b eab6 94be b526 384a f4b1 cc70 4e1e  rK.....&8J...pN.
-000005d0: cb0c 3b67 3c92 1db6 77a0 1d35 fbf6 5d76  ..;g<...w..5..]v
-000005e0: e423 a530 5397 43b8 1a42 be03 6dba 9ddc  .#.0S.C..B..m...
-000005f0: 3a38 9e98 91b9 0ad3 5290 6fc3 f9e9 c578  :8......R.o....x
-00000600: 1ae2 39d9 04b9 7d98 576d e7d8 d1d1 fbe7  ..9...}.Wm......
-00000610: c151 b0a3 ef3c 961d c788 f2a2 21ee a186  .Q...<......!...
-00000620: 98cf c343 8779 7b5f 9867 95c6 5034 146d  ...C.y{_.g..P4.m
-00000630: 6cac 242c 46b7 60b8 d7f1 2c14 e064 602d  l.$,F.`...,..d`-
-00000640: a007 83af 5102 f252 5560 315b c603 2b90  ....Q..RU`1[..+.
-00000650: a27c 4c8c 45e8 70e7 975c 5fe3 d192 e3db  .|L.E.p..\_.....
-00000660: a665 b56e af29 7719 6d22 5239 c269 9813  .e.n.)w.m"R9.i..
-00000670: 67ab cade 65b1 c155 1dcf 555b f2b0 be6a  g...e..U..U[...j
-00000680: 3db4 154e cffe 59ad c89f 0c11 4e16 0b12  =..N..Y.....N...
-00000690: 4863 9417 a64a a2f3 1953 bee7 2b49 c455  Hc...J...S..+I.U
-000006a0: 38bf 4533 b612 9718 bce3 e6c7 714e 53b8  8.E3........qNS.
-000006b0: 1276 b60f 0232 b9bb 39a9 7a65 3167 a6f2  .v...2..9.ze1g..
-000006c0: df2d 0c09 2c5b 8859 12e2 4d5d edd5 e79b  .-..,[.Y..M]....
-000006d0: 9cae 7a22 76fa 9777 c160 f2fd 70c9 470f  ..z"v..w.`..p.G.
-000006e0: e53b e75f f45d 43ae 7ef6 dde3 fa6e 933b  .;._.]C.~....n.;
-000006f0: 484c 9c79 c511 0174 4502 2395 1c06 1617  HL.y...tE.#.....
-00000700: 32e4 50ee 9290 0613 01cd 94c9 44f0 0282  2.P.........D...
-00000710: 64a6 1c80 98fa 0bbd f20c b929 15ce ad3e  d..........)...>
-00000720: 397f 452c 8386 4e5e d225 1214 8ab0 0c05  9.E,..N^.%......
-00000730: 2117 72e3 efef 936a 778c d7fa 2c81 6d84  !.r....jw...,.m.
-00000740: 5432 64d5 17ca 4389 c13d 3372 43d8 5425  T2d...C..=3rC.T%
-00000750: f3ae da26 0b85 dbe2 54cd bb1a be26 604b  ...&....T....&`K
-00000760: c37a 6e9d 2d27 ffdb 5ed4 3db4 173d 46f3  .zn.-'..^.=..=F.
-00000770: a399 e01e b387 739b 7ab8 c245 acff 58d6  ......s.z..E..X.
-00000780: 1ef9 32df 3970 db3a de03 5ee6 132c 43a4  ..2.9p.:..^..,C.
-00000790: 7ec1 7d8a 8a80 11ab 62be baaf 4ff9 259c  ~.}.....b...O.%.
-000007a0: 3bb4 7bf1 8120 9bfc d6db a4f6 dde0 0c7c  ;.{.. .........|
-000007b0: d4ab 5aa5 642b 113f 4b07 7c1f 9206 638c  ..Z.d+.?K.|...c.
-000007c0: 5bf4 345f 8f14 62ad a6b1 adc6 da31 0c79  [.4_..b......1.y
-000007d0: 8058 f30c a166 38df 8745 9a1a 33d5 8bac  .X...f8..E..3...
-000007e0: 398d 0a6f 41d5 40e5 3fdb d40d 68f6 0d34  9..oA.@.?...h..4
-000007f0: 1c91 055e 3199 b636 a3e4 4e0a 3cdc feef  ...^1..6..N.<...
-00000800: 0db0 c2c4 8ee1 ed8b bf01 504b 0304 1400  ..........PK....
-00000810: 0000 0800 f00b b158 8889 ce2f f238 0000  .......X.../.8..
-00000820: f0f2 0100 1800 0000 786c 2f77 6f72 6b73  ........xl/works
-00000830: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
-00000840: 9d9d 5b8f e646 7aa4 ff8a a0fb 7617 f344  ..[..Fz.....v..D
-00000850: d2d0 08d8 b1b1 d8bd d885 e181 bdd7 555f  ..............U_
-00000860: 955a ede9 56cb a51e 6bf7 df2f 4977 15a3  .Z..V...k../Iw..
-00000870: 98ef 1329 f86a d4c3 2f32 8a87 8c3c f061  ...).j../2...<.a
-00000880: e60f bf7f 79fe eb6f 3f3f 3d7d fdee ff7e  ....y..o??=}...~
-00000890: fef4 cb6f 7ffa fee7 af5f 7ffd fbf7 ef7f  ...o....._......
-000008a0: bbfd fcf4 f9fe b7bf fbf2 ebd3 2fdb 919f  ............/...
-000008b0: be3c 7fbe ffba fdf3 f9c3 fbdf 7e7d 7eba  .<..........~}~.
-000008c0: 7f3c 449f 3fbd 4f77 77ed fde7 fb8f bf7c  .<D.?.Oww......|
-000008d0: ffe3 0fc7 fff7 4fcf 3ffe f0e5 6f5f 3f7d  ......O.?...o_?}
-000008e0: fce5 e99f 9ebf fbed 6f9f 3fdf 3fff bf3f  ........o.?.?..?
-000008f0: 3f7d faf2 fb9f be9f be7f f93f fef9 e387  ?}.........?....
-00000900: 9fbf 1eff c7fb 1f7f f8f5 fec3 d35f 9ebe  ............._..
-00000910: fecb af9b 60fb e7fb d772 1e3f 7e7e fae5  ....`....r.?~~..
-00000920: b78f 5f7e f9ee f9e9 a73f 7dff dfa6 bfff  .._~.....?}.....
-00000930: f334 e57c 888e 1ffd ebc7 a7df 7f93 fffe  .4.|............
-00000940: 6e3f 9f87 2f5f feba ffe3 7f3e fee9 fbbb  n?../_.....>....
-00000950: fdcf 7afa f474 fbba 9772 bffd cf7f 3cfd  ..z..t...r....<.
-00000960: c3d3 a74f 7b61 db1f f3ef dfca fdfe f4dd  ...O{a..........
-00000970: 95fa df2f c5ff f7e3 126c 7fe1 c3fd 6f4f  .../.....l....oO
-00000980: fff0 e5d3 fff9 f8f8 f5e7 3f7d bf7c ffdd  ..........?}.|..
-00000990: e3d3 4ff7 7ffb f4f5 9fbf fcfe 3f9e be9d  ..O.........?...
-000009a0: 563d ffc4 7fbc ff7a ffe3 0fcf 5f7e ffee  V=.....z...._~..
-000009b0: 793f df1f 7fb8 edff 71b8 1fe7 bffd fce3  y?......q.......
-000009c0: 2ffb d5fa cbd7 e7ed e8c7 cdef eb8f fffa  /...............
-000009d0: 1fff fb87 f75f b73f 63ff e7fb db37 d19f  ....._.?c....7..
-000009e0: bde8 2f7f fef3 5bd1 fbcd f5d5 3abd 5a27  ../...[.....:.Z'
-000009f0: d04f e5f9 c374 17f9 b2e2 dd27 6399 5f2d  .O...t.....'c._-
-00000a00: f3a5 80fd eafc 67d1 d723 2f45 cfef ee4d  ......g..#/E...M
-00000a10: c9e5 b5e4 8225 5f8f bc94 bc3c bc7b 3045  .....%_....<.{0E
-00000a20: d7d7 a22b 167d 3df2 7a3d a6f7 3753 747b  ...+.}=.z=..7St{
-00000a30: 2dba 61d1 d723 67d1 f7f6 cf9e 5fcb 9eb1  -.a..#g....._...
-00000a40: eceb 91f3 36be ffc9 14bd bc16 bd60 d1d7  ....6........`..
-00000a50: 23af 45af ef5c d1eb 6bd1 2b16 7d3d 2245  #.E..\..k.+.}="E
-00000a60: ff6c 8a9e eece ba76 8785 7787 5e4a 4f77  .l.....v..w.^JOw
-00000a70: f793 bb97 9354 e56b 8594 e2a9 aee6 7c3f  .....T.k......|?
-00000a80: bbd2 cfda 3a5d 2b9f 94ce f5f2 bdab 3dd3  ....:]+.......=.
-00000a90: 5931 27ae 99dd a1d7 d29b 7d5c a6b3 724e  Y1'.......}\..rN
-00000aa0: 5c3b bb43 af57 c6d7 fce9 ac9f 1357 d0ee  \;.C.W.......W..
-00000ab0: d04b e9e5 eefe dda3 2bfe aca3 1357 d2ee  .K......+....W..
-00000ac0: d06b f1d3 fd7b 574b a7b3 9a4e 5c4f bb43  .k...{WK...N\O.C
-00000ad0: afc5 a777 4fae f4b3 a64e 5c55 bb43 afa5  ...wO....N\U.C..
-00000ae0: e777 f689 3f2b ebc4 b5b5 3b24 a5bb bf3d  .w..?+....;$...=
-00000af0: 9dd5 3571 75ed 0e49 e9ee 994c 676d 4d5c  ..5qu..I...LgmM\
-00000b00: 5bbb 43d2 ce7d 76a5 4bdb cab5 b53b f45a  [.C..}v.K....;.Z
-00000b10: 7ab5 8f64 3a6b 6bc2 2a19 b6da 51dd 7e5b  z..d:kk.*...Q.~[
-00000b20: f459 5513 d5c7 e93e 2c3b aad9 6fcb 3e2b  .YU....>,;..o.>+
-00000b30: 6ac2 f6f2 3e2e 3caa d86f 0b3f ab69 c216  j...>.<..o.?.i..
-00000b40: f3fe 3ebe 2c2c 98dc 6d38 ab6e c286 74b3  ..>.,,..m8.n..t.
-00000b50: 8ccf 8815 d6f3 acd0 095b d8cd f321 f464  .........[...!.d
-00000b60: 85f5 3cab 79c2 a6f7 fe3e 8596 2c48 ae9f  ..<.y....>..,H..
-00000b70: 78d6 fd4c 157c b70c 2fad 5158 cf33 1132  x..L.|../.QX.3.2
-00000b80: 56fb cd33 bcb4 4661 3dcf 9cc8 1806 f7b1  V..3..Fa=.......
-00000b90: 6394 2b6f 0b97 de36 c6c4 fd43 5825 5870  c.+o...6...CX%Xp
-00000ba0: fdfd 5bcb 333e 32c7 c743 5c25 58d1 09de  ..[.3>2..C\%X...
-00000bb0: 9a9e b992 3957 1ee2 3ac1 8a81 e999 3719  ....9W..:.....7.
-00000bc0: e3e3 f943 5829 58d0 fd91 6f3d cfc0 c918  ...CX)X...o=....
-00000bd0: 1fdb 882d f444 81ed 5ce5 336f 3277 20c2  ...-.D..\.3o2w .
-00000be0: 436f cb39 3324 5324 406d 8e7a 166f 877e  Co.93$S$@m.z.o.~
-00000bf0: 6758 14ec bcc7 ed4a f7fb bef0 3315 0ad5  gX.....J....3...
-00000c00: f104 ed8a 11b8 4a54 ce50 2814 0a09 f2d6  ......JT.P(.....
-00000c10: 085c 0e95 332a 0ad5 fc1c fa0d 7b14 4546  .\..3*......{.EF
-00000c20: e6d8 c38f 6fce b047 51ce 9a5f a81e 67b8  ....o..GQ.._..g.
-00000c30: f3c3 1e45 396b 78a1 0a9b e9ce b3c0 def9  ...E9kx.........
-00000c40: b382 17aa af99 ee3c 0bec 9d3f 2b78 c161  .......<...?+x.a
-00000c50: 40e8 37ac f3e5 acf3 05c7 00f1 cd19 d6f9  @.7.............
-00000c60: 7ad6 f98a 2380 f8ce 77bf ef0b 3feb 7ca5  z...#...w...?.|.
-00000c70: 2a5c e0ce 1b81 bbf3 f5ac f395 aa70 091b  *\...........p..
-00000c80: b0ee e7fd e99c 95bb 52e5 2e0f f1b5 1a56  ........R......V
-00000c90: ef7a 56ef 4ad5 7b2b 3cbe 562c b0d7 4a26  .zV.J.{+<.V,..J&
-00000ca0: e470 54ff 10d7 1223 70b5 a49e 5950 71a4  .pT....#p...YPq.
-00000cb0: ff70 1f46 a411 6467 7966 41c5 d1ff 43fc  .p.F..dgyfA...C.
-00000cc0: 4844 1309 6f0b 3f6b 7dc5 5aff 1077 0d59  HD..o.?k}.Z..w.Y
-00000cd0: 70b3 77ed 4c83 8a69 f070 bd0b df2c 5170  p.w.L..i.p...,Qp
-00000ce0: 7377 ad9d 21d1 3024 1eae 77e1 dbac 2b0a  sw..!.0$..w...+.
-00000cf0: 6eee aeb5 333a 1a26 c12d 348c 6621 de96  n...3:.&.-4.f!..
-00000d00: 7d66 44c3 8cb8 85f5 b8fb 7d5f f819 120d  }fD.......}_....
-00000d10: 43e2 16d7 6316 3cba 27a2 9dd1 d130 09c8  C...c.<.'....0..
-00000d20: 1205 8fb6 dbde ceec 6818 05e4 8982 47db  ........h.....G.
-00000d30: 6d6f 32cb 8f59 00dd 7616 d86e 7b3b c3a3  mo2..Y..v..n{;..
-00000d40: f1ac 6277 e86c ab7c e967 7a34 0a83 1a9e  ..bw.l.|.gz4....
-00000d50: cdb0 cfd0 ce94 6854 e96b fc88 0ffb 0cf3  ......hT.k......
-00000d60: 1907 33d5 ee1a f719 badf f785 9f15 7fa6  ..3.............
-00000d70: 8a5f a1cf 6004 aefe cc67 1ecc 9407 157a  ._..`....g.....z
-00000d80: 8b46 e012 753e 5362 a64a bf59 8689 6a04  .F..u>Sb.J.Y..j.
-00000d90: 2e51 e733 2566 aaf4 bb65 7cdf 5871 15bc  .Q.3%f...e|.Xq..
-00000da0: 353d 6362 a65a bf9b 86cd af51 5c05 6f4d  5=cb.Z.....Q\.oM
-00000db0: cf9c 98a9 dad7 d831 7a31 f1b6 6c79 1b48  .......1z1..ly.H
-00000dc0: b5be c67d c0ee f77d e167 1ecc 9807 d007  ...}...}.g......
-00000dd0: 3402 fbec 9f39 3163 4e90 250b 6cdb b19c  4....91cN.%.l...
-00000de0: f9b1 607e 80a7 11d8 b663 3963 65c1 9480  ..`~.....c9ce...
-00000df0: beae 11b8 3abe 9cb1 b260 4a90 250b aeb3  ....:....`J.%...
-00000e00: 3b6f 3dcf 5c59 3026 c893 05d7 b9da b79e  ;o=.\Y0&........
-00000e10: 67b0 2c18 13d0 a737 0297 65cb 192b 0b86  g.,....7..e..+..
-00000e20: 0459 b2c0 46d9 72a6 cac2 a902 9e2c b049  .Y..F.r......,.I
-00000e30: b69c 69b3 98b4 09e7 158c a038 4b61 1238  ..i........8Ka.8
-00000e40: 52c2 f4ec 7edf 05dc 72a6 cdc2 e111 0f97  R...~...r.......
-00000e50: 5860 874b eb19 362b 6747 3c5c 6281 1d2e  X`.K..6+gG<\b...
-00000e60: ad67 d6ac 1c1d e1e0 a5fb 7d77 09d7 3355  .g........}w..3U
-00000e70: 560e 89eb 25f9 563a 0aec f862 3d43 65e5  V...%.V:...b=Ce.
-00000e80: 8cb8 5e92 6f96 2878 b497 f0cc 9495 23e2  ..^.o.(x......#.
-00000e90: 3a82 fc66 8982 4797 29eb 9929 2b47 c42d  :..f..G.)..)+G.-
-00000ea0: ac6b 2c78 7475 6d3d 2365 e584 b885 4300  .k,xtum=#e....C.
-00000eb0: 163c 5667 7926 caca 0101 9628 78bc 0e25  .<Vgy&.....(x..%
-00000ec0: de7a 9e91 b272 a480 270a 1eaf 5db8 b79e  .z...r..'...]...
-00000ed0: c23f 7170 848e c3f1 cf74 a700 1467 44d8  .?qp.....t...gD.
-00000ee0: 0bec 0541 f942 40dd 6182 c0e8 da28 9e5c  ...A.B@.a....(.\
-00000ef0: 2d9f ee92 b862 52dc e2ce 8351 3cb9 8a3e  -....bR....Q<..>
-00000f00: dd09 3175 8761 718b db55 a378 7275 7dba  ..1u.aq..U.xru}.
-00000f10: 1392 ea0e f3e2 16b7 ac46 f1e4 aafb 7427  .........F....t'
-00000f20: 84d5 1d46 c6f3 0738 571e 0e79 aeeb 4ec8  ...F...8W..y..N.
-00000f30: ab3b 835e 75c7 5e0d de7d b0e5 0b7a 7567  .;.^u.^..}...zug
-00000f40: d8ab eed8 f9ea d492 5d77 025f dd61 1e3c  ........]w._.a.<
-00000f50: 7f08 03c4 281e 0797 4da8 ac3b cc90 e70f  ....(...M..;....
-00000f60: 2db6 4585 47c1 14ae 4484 7273 9d43 5756  -.E.G...D.rs.CWV
-00000f70: 3cfa 6bfc 06ba c400 79fe 1057 0856 7824  <.k.....y..W.Vx$
-00000f80: 5061 4c47 6322 8e59 9ffc 3d54 1ed3 0199  PaLGc".Y..=T....
-00000f90: 4864 6ed7 cddf 2e09 1204 2f2b 4c4a 1a85  Hdn......./+LJ..
-00000fa0: 65ee 2645 3511 c8ac 404d 18c5 e019 911c  e.&E5...@M......
-00000fb0: 414e 7373 5d62 574e 174b 5e2a d8e9 c84e  ANss]bWN.K^*...N
-00000fc0: 443b ab87 9915 ed74 6c27 c29d 75f0 084a  D;.....tl'..u..J
-00000fd0: 8c20 c219 6748 0883 5e68 6689 0b44 385b  . ..gH..^hf..D8[
-00000fe0: dc13 0969 d04b f112 0bc8 70b6 78ae b717  ...i.K....p.x...
-00000ff0: 04e5 4b00 20c5 d960 bad7 296c 4f47 b8cf  ..K. ..`..)lOG..
-00001000: 09c1 cf46 c4a1 93d8 79af 49a0 d009 a9d0  ...F....y.I.....
-00001010: 46d4 a193 d8b9 af49 80d1 0989 d1dd 37ec  F......I......7.
-00001020: 103b 8907 f985 259d 900d dd7d 1f63 5f96  .;....%....}.c_.
-00001030: 5c15 175f 890c e443 5b8c 03f6 82e0 a995  \.._...C[.......
-00001040: c840 16b4 0111 6814 76a6 7612 7c74 421c  .@....h.v.v.|tB.
-00001050: 7473 8d43 9f15 7612 7312 8274 4220 b4dd  ts.C..v.s..tB ..
-00001060: c74f 4e27 e8af a5d0 a213 c29f 5bf9 f1b5  .ON'........[...
-00001070: 6485 9d14 9a84 179d 1018 dd5c e36b c90a  d..........\.k..
-00001080: 3b2f 3465 fd3a 8443 249e d630 0afb 267d  ;/4e.:.C$..0..&}
-00001090: 1296 7442 3474 738d bb76 acb8 0a2e ae92  ..tB4ts..v......
-000010a0: 39c8 86b6 fbb8 e677 82e0 b991 6c41 0e74  9......w....lA.t
-000010b0: 2b1f 9e1b 54d8 99b0 49c8 d109 49d0 46dd  +...T...I...I.F.
-000010c0: 3d56 f82e 84c0 a353 8788 8a2b 3cad a8f0  =V.....S...+<...
-000010d0: dd3d 414d 2764 4d1b 8d56 59e1 3bd4 02a1  .=AM'dM..VY.;...
-000010e0: 4e48 a1a2 2b2a a63b 3f86 153c 7542 dcb4  NH..+*.;?..<uB..
-000010f0: d1f8 8715 7efc 2384 ea84 c429 bb22 e97e  ....~.#....).".~
-00001100: e787 0f42 a94e 88a9 c603 cc31 a73a 15fd  ...B.N.....1.:..
-00001110: 4a8d d263 8ebb 5663 5475 1256 7542 5875  J..c..VcTu.VuBXu
-00001120: 862e e998 569d 0457 9d10 3f9d a94b 6a14  ....V..W..?..Kj.
-00001130: 3658 8458 9d90 409d b14b 6a24 be6b 28d8  6X.X..@..Kj$.k(.
-00001140: ea84 dcea 8c5d 5223 f15d 4361 5a27 845a  .....]R#.]CaZ'.Z
-00001150: 67ec 921a 89ef 1a0a ef3a 21f0 3a63 97d4  g........:!.:c..
-00001160: 487c d75f 50d8 09d1 d619 2013 a7b0 1d0e  H|._P..... .....
-00001170: a161 27c4 6167 fafe c749 ec5b e849 48d9  .a'.ag...I.[.IH.
-00001180: 0951 d999 be01 7292 c117 ac12 3d08 c5ee  .Q....r.....=...
-00001190: bef1 5365 24f6 0df8 54f5 d359 9349 71a3  ..Se$...T..Y.Iq.
-000011a0: 6514 83d3 95a8 423a 7626 a6c7 4906 be12  e.....B:v&..I...
-000011b0: 56c8 d4ce 84f5 38c9 c057 c20a e9d9 dd17  V.....8..W......
-000011c0: 6e2f 4b06 be12 5688 d0c6 b35e ddcf fb06  n/K...V....^....
-000011d0: 47e8 da09 69d9 25be 85dd ef83 e225 7910  G...i.%......%y.
-000011e0: a55d a0bd 1cc3 b453 938c 6914 180b b597  .].....S..i.....
-000011f0: 4661 db4b c16c 27c4 6617 ca53 a3b0 792a  Fa.K.l'.f..S..y*
-00001200: a4ed 84e4 ec42 f5dc 28ec 004e 58db 09d9  .....B..(..NX...
-00001210: d9cd 35ee 251a 851d c035 fd5e 9f92 6281  ..5.%....5.^..b.
-00001220: 4994 4e10 3c37 1222 08d0 2e34 8962 147e  I.N.<7."...4.b.~
-00001230: 5423 cced 84d0 ed42 b328 46e1 deba 4f82  T#.....B.(F...O.
-00001240: e34e c8e3 b22b 2bec 8bf7 4948 dd09 515d  .N...++...IH..Q]
-00001250: b435 0afb ee7d 1286 7742 2677 899f 9cee  .5...}..wB&w....
-00001260: f7fd 9323 bcee 84fc ed12 4398 bd20 285f  ...#......C.. (_
-00001270: b205 61db 0500 45a3 b8f9 aeb8 00ba 13f2  ..a...E.........
-00001280: b66c 8b0a bb90 d024 84ee 84c0 ed02 c8a0  .l.....$........
-00001290: 51f8 f937 4174 2764 74d9 1515 373f ea98  Q..7At'dt...7?..
-000012a0: 7591 104c 9007 ea0f b3e4 e67b ff02 f64e  u..L.......{...N
-000012b0: 08ea eebe 5027 5072 f3a3 1da1 7b27 a475  ....P'Pr....{'.u
-000012c0: 9798 e6eb 057d 4d11 9277 4232 7701 a0cf  .....}M..wB2w...
-000012d0: 29ec c323 2cef 846c eeee 1adf 4523 f1b6  )..#,..l....E#..
-000012e0: 123b c8e7 eeb6 f1e5 3412 6f2b 6984 88ee  .;......4.o+i...
-000012f0: 0204 a353 f821 8d50 bd13 52ba 0b7c f4e5  ...S.!.P..R..|..
-00001300: 14b6 8325 60ef 84a0 eeee 0ab7 9625 7ec0  ...%`........%~.
-00001310: 2a70 ef84 b0ee ee0b f796 25d7 a1e6 c557  *p........%....W
-00001320: 0209 81dd dd37 1ed1 1849 b2c1 b0e8 7a46  .....7...I....zF
-00001330: 1c48 0f39 9e06 3192 e497 5192 4042 a077  .H.9..1...Q.@B.w
-00001340: f38d bbb2 4661 3bd0 c200 4fc8 f4ee aef1  ....Fa;...O.....
-00001350: 5365 24d7 eb73 f195 a042 1278 f78d 9f2a  Se$..s...B.x...*
-00001360: 23b1 d4f8 248c f084 ccef ee1b 3f55 4662  #...$.......?UFb
-00001370: 09f9 4940 e109 c15f e38b 123f 9d2d b0f0  ..I@..._...?.-..
-00001380: 84f0 ef6e 1b3f cc46 72ad 7617 5f09 2b24  ...n.?.Fr.v._.+$
-00001390: 808d 2f4a defd 9bb5 95ac 420a 7889 f9f2  ../J......B.x...
-000013a0: 5ed0 37ea 8208 4f88 fc2e 8098 1bc5 cd4f  ^.7...O........O
-000013b0: b208 253c 21f5 bb00 666e 14fe 95ec aa4b  ..%<!...fn.....K
-000013c0: af71 bcdc a047 c892 9b0d fe74 a78b b271  .q...G.....t...q
-000013d0: be80 af91 748a 8baf 2cd7 86a0 f0ee 1b2f  ....t...,....../
-000013e0: 7cc5 924e 71f1 4de2 cbf9 12bf fa36 0afb  |..Nq.M......6..
-000013f0: ea3b 095c 9c10 155e 00ea 370a fbea 3b09  .;.\...^..7...;.
-00001400: 5c9c 1015 6657 54dc aeed d3c5 5696 8543  \...fWT.....V..C
-00001410: 5698 6d79 2477 6d9e 2eb6 b260 1c12 c4cb  V.my$wm....`....
-00001420: 4398 81bd a05f 8f4e e8e2 8404 f156 7ebc  C...._.N.....V~.
-00001430: 221d 2bae df1b 5c5c 657d 3824 88d9 95d3  ".+...\\e}8$....
-00001440: c84e d824 618e 1312 c46c cb69 6427 6c92  .N.$a....l.id'l.
-00001450: 40c7 0911 62b4 65c5 edfa 89c5 c556 d78e  @...b.e......V..
-00001460: e430 225b cea2 6a57 7d14 ea38 2159 bcd9  .0"[..jW}..8!Y..
-00001470: c60b f1b1 e266 c986 242c 7242 de78 b38d  .....f..$,rB.x..
-00001480: 2390 15b7 665d 258c 1037 6657 0ea3 2b54  #...f]%..7fW..+T
-00001490: 7ab1 9530 42de 986d 398c 9a7f 9025 8c10  z..0B..m9....%..
-000014a0: 3866 5b9e 576a fed6 4a46 1946 b93f 26b3  8f[.Wj..JF.F.?&.
-000014b0: d6de 40e2 0841 e405 3e81 308a 771f adab  ..@..A..>.0.w...
-000014c0: a411 a2cb ec8a 4b56 a687 777f 75be ba62  ......KV..w.u..b
-000014d0: 2d42 cde8 8b8a a93d d825 8493 ae65 8bb4  -B.....=.%...e..
-000014e0: f302 5f7c 18c5 e06c 258e 9068 6657 52ac  .._|...l%..hfWR.
-000014f0: 7e51 605d fb16 81e6 0560 7ea3 b8d9 d72f  ~Q`].....`~..../
-00001500: 49d7 c545 9e79 b35d 635b 9ee4 f6ae 9246  I..E.y.]c[.....F
-00001510: 4833 2ff0 518d 51dc 06d7 58d2 0861 66b6  H3/.Q.Q...X..af.
-00001520: 25c5 6ac7 8749 97d3 45fa 7901 46d1 28ec  %.j..I..E.y.F.(.
-00001530: f02d e982 ba48 382f c028 1a85 cf45 5d52  .-...H8/.(...E]R
-00001540: 1709 e705 6841 a318 2c1b 2df9 1422 cedf  ....hA..,.-.."..
-00001550: ca47 5e7a b19f a424 61a2 5347 386b f99c  .G^z...$a.SG8k..
-00001560: 3876 516d a19f 13b2 cc0b 6087 46e1 6b43  8vQm......`.F.kC
-00001570: d6d5 b6f9 5bac fe98 3492 f611 14d0 3975  ....[...4.....9u
-00001580: d8b2 1a70 a766 70df 2546 4244 f9c5 0003  ...p.fp.%FBD....
-00001590: c36e 1e90 8469 4e48 28c7 c9d8 fdbc 1f48  .n...iNH(......H
-000015a0: 09bb 9c90 445e e3f9 86ee f741 f112 0088  ....D^.....A....
-000015b0: 1caf b02c f978 e1db 2438 7242 b878 a595  ...,.x..$8rB.x..
-000015c0: c98d c22e d92d 3872 42b8 78a5 45bb 8dc2  .....-8rB.x.E...
-000015d0: cd4a 25a1 9113 b2c5 ec8a 6b68 4f3e 7704  .J%.......khO>w.
-000015e0: 474e 0817 af84 0b3a 899f 9412 1e39 218f  GN.....:.....9!.
-000015f0: bc12 2ee8 247e 52aa e822 fd14 0a2b e03c  ....$~R.."...+.<
-00001600: 4e61 27a5 0460 4e08 30af 44ed 3989 9d9d  Na'..`N.0.D.9...
-00001610: 4f02 3627 c494 8d2f 4bec db88 2468 7342  O.6'.../K...$hsB
-00001620: 4ed9 f8b2 c44e cf27 419b 1372 ca2b 518a  N....N.'A..r.+Q.
-00001630: 46e2 df25 2641 9b13 72ca c617 25fe ad4f  F..%&A..r...%..O
-00001640: 12b4 3921 a7bc c6a6 e3b5 7c93 10cc 0979  ..9!......|....y
-00001650: e435 a66e 8cc0 de42 e197 13c2 c82b 2031  .5.n...B.....+ 1
-00001660: 4e61 2ba8 d0cb 0951 6476 6585 af9f 022f  Na+....Qdve..../
-00001670: 2724 9157 6062 8cc2 9238 a9ea 6622 182d  '$.W`b...8..f".-
-00001680: b0ae 9551 dc06 0fab 8411 72c8 2b2c 6d65  ...Q......r.+,me
-00001690: 14fe 7d80 80cb 0929 e4dd 159e 6294 dc06  ..}....)....b...
-000016a0: b756 a208 29e4 dd17 6a27 4a6e 3e02 055c  .V..)...j'Jn>..\
-000016b0: 4e08 2e6f bef1 440a 2b06 fd64 219a 5348  N..o..D.+..d!.SH
-000016c0: 287f 3340 da79 f5a3 3e41 9a53 4828 bf94  (.3@.y..>A.SH(..
-000016d0: 6f3a 42f6 e96c 923b 0d53 8406 b3ac 180c  o:B..l.;.S......
-000016e0: 6004 6a4e 8828 b32d ef2a 3698 5d14 ac39  `.jN.(.-.*6.]..9
-000016f0: 7590 b25e 4fcc 183f 8f28 0073 ea70 642d  u..^O..?.(.s.pd-
-00001700: 1ff7 10d9 cec0 8e2d 9bee 5ac4 4bdc f4c7  .......-..Z.K...
-00001710: 5ecf c06e 2f98 0456 4e88 1eaf 34cf c00a  ^..n/..VN...4...
-00001720: fb51 6212 5639 854b febe 948f f9e0 b7ee  .Qb.V9.K........
-00001730: 122a 3985 cbfe be94 cfd1 e1eb 91f0 c729  .*9............)
-00001740: 5cfa f79b 0192 c6ab 7d7b 9f04 344e 2138  \.......}{..4N!8
-00001750: fc52 3e77 3f06 2720 4110 92c3 2f06 f829  .R>w?.' A.../..)
-00001760: 661a 5d22 a9f3 1d3a ac0e 9807 96ef 4d42  f.]"...:......MB
-00001770: 15a7 8e11 d6f2 71d3 a0ad eed9 a754 08e2  ......q......T..
-00001780: 843c f04a f38d acf0 6d8c 10c4 295c b6f7  .<.J....m...)\..
-00001790: a57c ee2a f830 9e75 5732 f34e 07a1 e0fd  .|.*.0.uW2.N....
-000017a0: d67b 07a9 de1d e2ab 0ee3 c911 017d 1382  .{...........}..
-000017b0: bed3 1dec a036 047d 9380 be09 b1dd 8966  .....6.}.......f
-000017c0: 773a 4560 2035 1901 dded 04a0 d3dd 4902  w:E` 5........I.
-000017d0: 07a9 cac8 e21e 0e70 1246 63e9 ef24 046f  .......p.Fc..$.o
-000017e0: 421e f770 86dd e68c c67e 5290 04e2 4d88  B..p.....~R...M.
-000017f0: e4ee ce71 8fc2 496c 2e0b c69b 90c9 35be  ...q..Il......5.
-00001800: 46e2 ab94 70bc 09a1 dcc3 186e b2d1 f833  F...p......n...3
-00001810: 96b4 402a f730 867b 6c34 de58 3732 c47d  ..@*.0.{l4.X72.}
-00001820: 09ef 6812 cb49 ec50 4a48 de84 5cee 5608  ..h..I.PJH..\.V.
-00001830: 9cee 3872 04da 4d48 e0ee 0671 22a0 6434  ..8r..MH...q".d4
-00001840: 7d23 d06e 4202 d7f8 f2d4 889f 8c14 6837  }#.nB.........h7
-00001850: 2181 6b7c 79b2 c393 8802 ed26 2470 a7bb  !.k|y......&$p..
-00001860: 4768 bf8d c477 4c84 da4d 88e0 1a5f 1e8b  Gh...wL..M..._..
-00001870: d8b7 ed02 ed26 2470 8d2d 6f50 3e38 5d49  .....&$p.-oP>8]I
-00001880: 26a4 7677 5fd8 fe13 17ac f1af 9404 e64d  &.vw_..........M
-00001890: 88e6 1a5b 9678 9442 68de d4b1 b9d2 b741  ...[.x.Bh......A
-000018a0: 6e77 b55f c5a4 55f7 5235 4317 0474 d7c1  nw._..U.R5C..t..
-000018b0: b694 77ba 732a 0f5d fa63 6260 f7a0 1412  ..w.s*.].cb`....
-000018c0: 3723 563b ddd1 3694 4662 07fb 5948 dcdc  7#V;..6.Fb..YH..
-000018d0: 71b5 7a62 6675 1937 dacf 02dd e60e a155  q.zbfu.7.......U
-000018e0: 034c 8ee9 6170 0ab2 3b2a e2b2 fba5 8b77  .L..ap..;*.....w
-000018f0: 0d45 c96a 876a 5900 db8c b8ac b165 89df  .E.j.jY......e..
-00001900: 3a54 08db 8c84 adf1 45c9 60cb 5221 6f33  :T......E.`.R!o3
-00001910: afdd 7b07 b31e 2c59 07b6 b255 2a82 b4c6  ..{...,Y...U*...
-00001920: 9625 83db 2b5b ab22 49bb fb86 73d2 4e62  .%..+[."I...s.Nb
-00001930: e7ae b2c0 b7b9 4369 a5be 2066 bbfa 7166  ......Ci.. f..qf
-00001940: 9e74 4366 9e25 e98f c919 b8b1 7816 a036  .tCf.%......x..6
-00001950: 9b65 7cfb 63e7 ec9b bd33 42ce 66b3 8a6f  .e|.c....3B.f..o
-00001960: 7f4c 4ec0 2153 5920 d9dc 21af 6ac0 6163  .LN.!SY ..!.j.ac
-00001970: 7b1d 5970 d8dc c1ad 6a30 5c9f 2a0b e29a  {.Yp....j0\.*...
-00001980: 1158 9d60 67e8 4e10 942f b51e 79d5 09f6  .X.`g.N../..y...
-00001990: 97ef 1581 81d4 6f24 5327 da63 de4a ec96  ......o$S'.c.J..
-000019a0: da42 b366 6653 d9d7 487c 5742 70d6 cc70  .B.ffS..H|WBp..p
-000019b0: 2a1a 3b89 ef62 08cf 9a91 4e35 c6e6 f589  *.;..b....N5....
-000019c0: ad4e 42b4 66e4 5327 daea de4a fc26 f092  .NB.f.S'...J.&..
-000019d0: 1348 a81a 5f23 f109 2b54 6b46 46d5 18b3  .H.._#..+TkFF...
-000019e0: c4c7 8a70 ad19 2955 e36b 0633 b6c9 12b0  ...p..)U.k.3....
-000019f0: 3523 a66a 7c4d 8fc4 3f58 924d 08aa 1ebe  5#.j|M..?X.M....
-00001a00: 713a 398d 9d15 c882 b766 8455 9d33 6b2c  q:9......f.U.3k,
-00001a10: 9395 8570 cdc8 ab1e c6e1 4c8b d5d8 0989  ...p......L.....
-00001a20: 2c94 6b46 92f5 700e 3f35 b51a 3b25 9185  ,.kF..p.?5..;%..
-00001a30: 7fcd c8b8 3a67 a349 ee8d 5816 3236 23e7  ....:g.I..X.26#.
-00001a40: 7a38 87df b359 8dfd 223f 0b1d 9b91 803d  z8...Y.."?.....=
-00001a50: 9c9f 6267 a3b1 dfe4 67c1 6633 a2b1 bb73  ..bg....g.f3...s
-00001a60: dcdf 7612 3783 9885 a6cd 48cc 1a5f 23b1  ..v.7.....H.._#.
-00001a70: 5444 16cc 3623 667b 18c7 75d9 692c 0792  TD..6#f{..u.i,..
-00001a80: 05c1 cd88 e01e ce71 6576 1acb db64 a173  .......qev...d.s
-00001a90: 33d2 b953 fc02 a217 f49d 3aa1 7333 b2b6  3..S......:.s3..
-00001aa0: 5bf9 7045 87d3 c159 40dc ccab fc4e 4065  [.pE...Y@....N@e
-00001ab0: 5989 ed35 0a8a 9b0d 588b bea6 0f65 6ba5  Y..5....X....ek.
-00001ac0: b0b8 9917 fa65 5f23 f19d 4681 7133 92b5  .....e_#..F.q3..
-00001ad0: 8771 7c2f 9dc6 0f23 05c7 cd08 d73a 67a3  .q|/...#.....:g.
-00001ae0: f1fd 3741 7233 f2b5 8773 5c41 9cc6 8f0d  ..7Ar3...s\A....
-00001af0: 04ca cd48 d83a 67a3 f1d3 1d82 e566 646c  ...H.:g......fdl
-00001b00: 77e7 b80f e724 b693 2e58 6e46 c6d6 f89a  w....$...XnF....
-00001b10: 8e94 af50 9250 c8d8 1ebe f074 198d 3d61  ...P.P.....t..=a
-00001b20: e172 3372 b987 717c 8b9d c61b 4b74 7500  .r3r..q|....Ktu.
-00001b30: ae4c 3a20 9cbb 5d52 db5b 123c 3723 6c3b  .L: ..]R.[.<7#l;
-00001b40: 4d34 85cd 923b df27 1640 3723 6e6b 7c59  M4...;.'.@7#nk|Y
-00001b50: e2e7 9d85 d0cd c8db 1a5f 33cc b3c1 288c  ........._3...(.
-00001b60: 6e46 e276 f78d ab8c 91f8 997c 8174 3322  nF.v.......|.t3"
-00001b70: b7c6 d70c f31c 5194 05d3 cd1d 73ab 0fee  ......Q.....s...
-00001b80: 78b2 49c8 db8c 18ed 0455 be13 04e5 4baa  x.I......U....K.
-00001b90: 202f bb95 0f06 e37e 8fb0 b419 79d9 dd20   /.....~....y.. 
-00001ba0: 7ee6 9cc4 f67b 84b1 cdcc d126 c265 acc6  ~....{.....&.e..
-00001bb0: 3789 4d52 a531 5747 b88c d5f8 ae8f f0b7  7.MR.1WG........
-00001bc0: 9969 da44 abd2 5b8d 5d98 320b 819b 91b2  .i.D..[.].2.....
-00001bd0: 3d9c e371 a7d3 d825 22b3 b0b9 99f9 db44  =..q...%"......D
-00001be0: 5339 4e62 1b27 2176 3352 b987 2f3c 5f46  S9Nb.'!v3R../<_F
-00001bf0: e3a7 7284 e5cd 48e6 1ece f07c 198d 9f51  ..r...H....|...Q
-00001c00: 119e 3723 b37b 38c3 f365 347e 4645 48df  ..7#.{8..e4~FEH.
-00001c10: 8c34 efee 1c8f b59d c48e f105 00ce 08f9  .4..............
-00001c20: 1ebe f15d 761a 3fd4 1634 3823 fe7b 38c7  ...]v.?..48#.{8.
-00001c30: 77d9 69fc 505b 98e1 ecb8 e0d8 76b8 3c71  w.i.P[......v.<q
-00001c40: 1662 3823 15bc 950f 5774 b881 4b16 6438  .b8#....Wt..K.d8
-00001c50: 3316 9c68 e8e9 24b6 c911 9038 2316 6c7c  3..h..$....8#.l|
-00001c60: 8dc4 f7af 8425 cec8 0b1b 6323 f11d 4a61  .....%....c#..Ja
-00001c70: 8cb3 e388 a991 751a dfd4 097b 9c71 79e1  ......u....{.qy.
-00001c80: c319 9e53 a3f1 cdbb a0ca 9951 e5dd 390e  ...S.......Q..9.
-00001c90: 41a7 f18d ac40 cc99 21e6 dd39 6e64 9dc6  A....@..!..9nd..
-00001ca0: 37b2 4237 67a6 9b13 8d79 9dc4 36b2 c23c  7.B7g....y..6..<
-00001cb0: 67e6 97d9 d77d d5e0 2fb5 6414 e3cb 0907  g....}../.d.....
-00001cc0: db4e e35b 7741 9e33 f3cb 0947 db4e e35b  .N.[wA.3...G.N.[
-00001cd0: 7781 9e33 13cc bb73 fc60 3b8d 6fdd 857a  w..3...s.`;.o..z
-00001ce0: ce4c 301b 67a3 f16f 2d04 7bce 8c30 27f8  .L0.g..o-.{..0'.
-00001cf0: 7cd4 4a6c bf42 a8e7 cc08 f3ee 0bcf 97d1  |.Jl.B..........
-00001d00: f87e 8570 cf99 b967 e36c 34fe b585 00d1  .~.p...g.l4.....
-00001d10: 9981 e8dd 397e b29d c6f7 6804 89ce 8c44  ....9~....h....D
-00001d20: 27f8 5ad7 4adc 429a 5990 e8cc 4874 a2ef  '.Z.J.B.Y...Ht..
-00001d30: 75ad c6ae a599 058a ce4c 3827 fa62 d76a  u........L8'.b.j
-00001d40: ec72 9a59 b0e8 cc58 7422 facd 481e fcbb  .r.Y...Xt"..H...
-00001d50: 7501 a333 53ce 6ccc df6e 7a86 41c0 e8cc  u..3S.l..nz.A...
-00001d60: 6074 22ec ce48 1efc ec96 a0d1 b9e3 9c65  `t"..H.........e
-00001d70: 9689 19e8 cdc1 4e39 0b04 9d0d 04dd 1f53  ......N9.......S
-00001d80: 073b 132a 1874 3618 747f ecc5 61b1 3371  .;.*.t6.t...a.3q
-00001d90: 4528 e862 28e8 fe98 9e81 5b8b aa08 065d  E(.b(.....[....]
-00001da0: 3aa6 591d 7819 1cfb 9ea3 08ef 5c0c efdc  :.Y.x.......\...
-00001db0: 1f7b bd44 f776 f450 8477 2ecc 3427 58ae  .{.D.v.P.w..4'X.
-00001dc0: d049 1eec f47b 110c ba30 06cd c6fc c5e7  .I...{...0......
-00001dd0: e084 abf8 baa4 087b 954e e231 ab22 2074  .......{.N.1." t
-00001de0: 61aa 39c1 fcbb 930c 7c67 f1e5 3440 5f94  a.9.....|g..4@_.
-00001df0: b441 dd58 c417 3322 cce3 fef7 dd38 bf08  .A.X..3".....8..
-00001e00: f05c 985e 8efb 31bd a02f 5fc0 e682 f0f2  .\.^..1../_.....
-00001e10: 567e 6c10 a2d0 1703 c90e 8697 33cc 8d5b  V~l.........3..[
-00001e20: 891b 5615 e19d 0b32 cdbb 6f5c 019c c44d  ..V....2..o\...M
-00001e30: 9014 e1a0 8be1 a0e3 6397 a224 3b98 6a8e  ........c..$;.j.
-00001e40: fb55 bd20 285f 3202 57f3 ddca 0783 2106  .U. (_2.W.....!.
-00001e50: 5d04 832e 8c41 17bc f746 e2ef 8164 01e3  ]....A...F...d..
-00001e60: d1ec cb12 3ba2 2e42 4d17 46a0 0bbd 8fb1  ....;..BM.F.....
-00001e70: 1a3b 5554 849b 2e0c 4117 7a1f 6335 76aa  .;UT....A.z.c5v.
-00001e80: a808 385d 9882 2e54 cf9c c4d6 6fe1 a60b  ..8]...T....o...
-00001e90: 43d0 eccb 127f 8f85 9b2e 0c41 177a 2762  C..........A.z'b
-00001ea0: 3576 d6a4 0839 5d18 832e f44e c46a ecac  5v...9]....N.j..
-00001eb0: 4911 74ba 3007 1d0f b37a 419f 1382 4817  I.t.0....zA...H.
-00001ec0: e69d 4b3c 5bde 2b02 0309 2206 9b0b 4c1e  ..K<[.+..."...L.
-00001ed0: 3b89 5db8 ab08 0b5d 986b 665f 96f8 cdec  ;.]....].kf_....
-00001ee0: 8aa0 d085 b1e6 12ef 2ad7 2b82 2b2a 81c3  ........*.+.+*..
-00001ef0: f872 816d e59c e4d1 776c 8578 2e4c 2fa3  .r.m....wl.x.L/.
-00001f00: b191 bcfb 77eb 2b79 c3ec 32fb a2a4 0d7c  ....w.+y..2....|
-00001f10: 256f 985c 2eb4 939e d35c f76c b818 4bdc  %o.\.....\.l..K.
-00001f20: 30b8 5c68 2f3d a7b9 eeda 7031 96b4 6170  0.\h/=....p1..ap
-00001f30: 7937 0e67 4a9d e6d1 67bb d0ce 85d1 65e3  y7.gJ...g.....e.
-00001f40: 6ce6 57bc b1e4 1393 cb05 3610 7492 516d  l.W.......6.t.Qm
-00001f50: 9280 6270 998d 5932 3296 8062 d679 3786  ..bp..Y22..b.y7.
-00001f60: c79a 35ef 9ead b104 1743 d0bb 313c d626  ..5......C..1<.&
-00001f70: b9dc 4469 1138 ba30 e95c e23d c17a 451f  ..Di.8.0.\.=.zE.
-00001f80: c942 4117 469a 0b6c 0ae6 24d7 ad38 2ebe  .BA.F..l..$..8..
-00001f90: 9250 8c34 efbe f1ad 349a 473b cf5f 0483  .P.4....4.G;._..
-00001fa0: 2e8c 34ef cef1 bd34 9a47 3bdb 5e04 832e  ..4....4.G;.^...
-00001fb0: 8c34 17d8 09cd 48aa 1fd9 0804 5d18 682e  .4....H.....].h.
-00001fc0: b427 99d1 d441 3f5f 20e8 c240 73a1 5dc9  .'...A?_ ..@s.].
-00001fd0: 8ca6 0ec6 3602 4117 269a e3fd 0a7b 4150  ....6.A.&....{AP
-00001fe0: 6f24 8a98 5c2e 37b8 a2e3 be92 50cd 8509  o$..\.7.....P...
-00001ff0: e5cd 002a a649 29fb b008 d45c 1850 de7d  ...*.I)....\.P.}
-00002000: e353 331a cf0f 14a1 9a0b 93cb bb73 fcb0  .S3..........s..
-00002010: 188d 6726 8ae0 ce85 d9e5 dd39 7e5e 8cc6  ..g&.......9~^..
-00002020: 930b 4580 e7c2 f4f2 e61c 4782 9178 70a1  ..E.......G..xp.
-00002030: 08f1 5c18 5fde 8de1 369b fc1a 384b 1a31  ..\._...6...8K.1
-00002040: c0bc 3bc3 6d36 0936 7096 3462 8479 7786  ..;.m6.6p.4b.yw.
-00002050: db6c 126c e02c 6984 6b0d efce f194 ef18  .l.l.,i.k.......
-00002060: 872e 8243 17c6 a177 07b8 9fe3 4412 22ba  ...C...w....D.".
-00002070: 3011 bd5b c08d 1b4f 2c0b 135d 1870 2eb7  0..[...O,..].p..
-00002080: d820 5c91 f862 2019 c320 f366 10a7 6ab8  . \..b .. .f..j.
-00002090: 26f1 c541 b2a4 992c 2107 94cc 8377 28c2  &..A...,!....w(.
-000020a0: 3817 e695 77e3 f809 309a 271f 9fc2 3817  8...w...0.'...8.
-000020b0: e695 7767 b86f ac79 f24d 8630 ce85 81e5  ..wg.o.y.M.0....
-000020c0: dd39 aed1 46f3 34b8 da92 254c 2c1b 67d4  .9..F.4...%L,.g.
-000020d0: cc83 d79e 4239 1726 9677 e710 7673 9a27  ....B9.&.w..vs.'
-000020e0: df58 09e5 5c98 58de 9ce3 c68a 25d5 cfda  .X..\.X.....%...
-000020f0: 0ae3 5c18 58de 7de1 c946 4d1d cc9e 0ae5  ..\.X.}..FM.....
-00002100: 5c98 58de 9de3 279b 3575 307b 2a94 7361  \.X...'.5u0{*.sa
-00002110: 62b9 c06a 764e 6257 e429 c238 17b3 2e72  b..jvNbW.).8...r
-00002120: 7f4c 86d2 b629 14c8 b998 6591 fb63 7fd8  .L...)....e..c..
-00002130: 40d2 8889 e502 0be3 39c9 bd5d 91af 08e5  @.......9..]....
-00002140: 5c18 592e b0f3 9e93 3cfa 2c12 cab9 30b2  \.Y.....<.,...0.
-00002150: 5c60 a341 2779 f7ab f595 2462 6099 7dcd  \`.A'y....$b`.}.
-00002160: db73 c7f7 1441 9c0b e3ca eccb 92c1 fc93  .s...A..........
-00002170: 10ce 8569 6536 6689 c58d 8af0 cd85 59e5  ...ie6f.......Y.
-00002180: 02fb 0d3a 89e7 5084 6e2e e142 cc2f 0626  ...:..P.n..B./.&
-00002190: 6dfc 8949 da30 93bc 9dd8 14c7 9cd1 7800  m..I.0........x.
-000021a0: 4330 e6c2 48b2 3146 4df5 8f90 50cc a523  C0..H.1FM...P..#
-000021b0: 92f5 9262 0c8d fa81 422b 978e 3c56 07ce  ...b....B+..<V..
-000021c0: 1b8b a615 8192 0b03 c605 b6fa 7412 cb13  ............t...
-000021d0: 1641 920b f3c5 ec8b 92ea e7d9 0549 2e8c  .A...........I..
-000021e0: 1717 a2a2 8ca4 9b62 bc18 4bdc 305d 5c00  .......b..K.0]\.
-000021f0: dc74 12cf 060a 8f5c 982d 2e00 6e3a 89ef  .t.....\.-..n:..
-00002200: d90a 8d5c 182d 2e44 6319 8905 648b d0c8  ...\.-.Dc...d...
-00002210: 85c9 62f6 3521 f4c5 fa4a 0875 5cb1 d454  ..b.5!...J.u\..T
-00002220: 668e fd36 2345 90e3 d2f1 c36a 6080 416f  f..6#E.....j`.Ao
-00002230: 2059 d371 c26a 307e db2e b470 61f4 b7c6   Y.q.j0~...pa...
-00002240: 3dfc 4e10 942f e9c1 e06f 056e 29c4 882f  =.N../...o.n)../
-00002250: 0612 13cc fd56 e287 9cc4 be49 1152 b818  .....V.....I.R..
-00002260: 52b8 3f26 f9e7 aa65 1554 b832 0e7c dd35  R.?&...e.T.2.|.5
-00002270: fe3f 5d7b 4177 e1aa 80c2 9517 3fa6 f287  .?]{Aw......?...
-00002280: 3332 5538 e1ca 6b1f b7f8 ce5b 85bd 6a59  32U8..k....[..jY
-00002290: 5ccd 064e f1e3 6025 6efe be0a 3b5c 0d08  \..N..`%n...;\..
-000022a0: 8cbe 4632 b9be 5c15 78b8 3209 dc88 63b3  ..F2..\.x.2...c.
-000022b0: 1adb 4e56 a187 2ba3 c08d 3836 abb1 f34f  ..NV..+...86...O
-000022c0: 55f8 e16a 6060 5a57 c06a ec5c 4c15 82b8  U..j``ZW.j.\L...
-000022d0: 3241 dc68 5d01 abb1 73d9 55e0 e2ca 7071  2A.h]...s.U...pq
-000022e0: 83ed 0cac c4cd 0255 818e 2b43 c7e8 eb24  .......U..+C...$
-000022f0: 7612 a80a 8c5c 992c 6663 23b1 7340 5568  v....\.,fc#.s@Uh
-00002300: e4ca 6831 1b1b 89fd ecb0 0a8e 5c79 e965  ..h1........\y.e
-00002310: 3676 fbd5 d967 4be0 e5ca f072 8bf7 1e71  6v...gK....r...q
-00002320: 0a7f 9d25 b918 69de 5cc3 0ebe 93d8 6f1d  ...%..i.\.....o.
-00002330: ab90 ce95 b1e5 cd37 ecdf 3b89 5f21 ac0a  .......7..;._!..
-00002340: ea5c 995b de8d e3a8 369a 073b 4756 0576  .\.[....6..;GV.v
-00002350: ae0c 2eef ce70 8b59 e357 82ab 023b 5706  .....p.Y.W...;W.
-00002360: 9737 e770 50e3 24f6 7d7a 15d4 b932 b78c  .7.pP.$.}z...2..
-00002370: be46 e25f a757 619d 2b83 cb6c cc12 ff4e  .F._.Wa.+..l...N
-00002380: bb0a ec5c 195c 6663 96f8 b7ac 5558 e7ca  ...\.\fc....UX..
-00002390: dc32 1bb3 e461 72f3 6455 50e7 caa8 331b  .2...ar.dUP...3.
-000023a0: 9bdc b253 1355 18e8 ca0c f46e 1c57 64a3  ...S.U.....n.Wd.
-000023b0: f1c8 4415 38ba 32e9 bc3b c715 d968 1e7c  ..D.8.2..;...h.|
-000023c0: 3f53 f0e8 caac f3e6 1c7e 1ce7 24f6 9be5  ?S.......~..$...
-000023d0: 2a74 7465 3a7a f30d 277f 9dc4 2ef5 5005  *tte:z..'.....P.
-000023e0: 9aae 4c40 5f5b b817 d7e1 3bf7 2a6c 7465  ..L@_[....;.*lte
-000023f0: d0b9 c51c 7daf 080c 2488 0cd1 0c3c bb93  ....}...$....<..
-00002400: 588e be0a 045d 1968 6eb4 068b d378 90be  X....].hn....x..
-00002410: 0a05 5d99 686e b406 8bd3 8c9c 2589 1869  ..].hn......%..i
-00002420: 6eb4 068b d3f8 c9ca 2a18 7435 4833 ac48  n.......*.t5H3.H
-00002430: e224 76a7 d82a 1474 65a4 b9c5 1f2d f48a  .$v..*.te....-..
-00002440: e0f1 95bc 6174 b901 c3ef 2476 4bf3 2ab0  ....at....$vK.*.
-00002450: 7365 7099 7d59 72b3 1b9a 5581 9d2b 83cb  sep.}Yr...U..+..
-00002460: 8d3e 1e70 1abf 9b7a 15da b932 eddc e8eb  .>.p...z...2....
-00002470: 01a7 f1bb d657 c1a0 2b33 cdc6 d984 94ef  .....W..+3......
-00002480: 970a 085d 196a 36ce 26a5 ec7b 9c2a 2074  ...].j6.&..{.* t
-00002490: 65a8 b9d1 870b 4ee3 77af af02 4257 a69a  e.....N.w...BW..
-000024a0: 77e7 78f2 c268 6ed9 7611 0585 ae8c 351b  w.x..hn.v.....5.
-000024b0: 6713 53d9 765b 0485 ae8c 35b7 98e4 ef15  g.S.v[....5.....
-000024c0: 7d4e 09f1 5c99 786e 40f2 f792 c041 1289  }N..\.xn@....A..
-000024d0: 9967 76f8 2f27 92b0 d095 c1e6 461f 0b38  .gv./'......F..8
-000024e0: cdcd 2e17 5385 86ae 4c36 37fa 58c0 69ec  ....S...L67.X.i.
-000024f0: abf7 2a30 7465 b079 378e 1f18 a3b9 15ef  ..*0te.y7.......
-00002500: 2c81 c460 b371 668d cf23 61a1 2b83 cdbb  ,..`.qf..#a.+...
-00002510: 715c 378d e676 05fd 2fce 9247 0c36 1b67  q\7..v../..G.6.g
-00002520: 9347 7651 a02a 3074 65b0 d938 9b3c 2a36  .GvQ.*0te..8.<*6
-00002530: 0905 86ae 0c36 37f8 18c5 48aa 6fef 0485  .....67...H.o...
-00002540: ae8c 42b3 afe9 4e15 1bc0 4248 5726 a4d9  ..B...N...BHW&..
-00002550: f8bf 9c5e c24d 57e6 a61b ace6 e224 9e04  ...^.MW......$..
-00002560: a942 5357 a6a9 1be0 4a4e e297 47aa 4259  .BSW....JN..G.BY
-00002570: 57a6 ac1b 800b 4ee2 43b3 4974 358e 2120  W.....N.C.It5.! 
-00002580: 359c 6470 a125 b918 a36e 004c 3889 fd2c  5.dp.%...n.L8..,
-00002590: b10a 785d 3b88 fa7c f5db 1fd3 67d7 e693  ..x];..|....g...
-000025a0: 00d6 b583 a5d5 c164 d77b 9bbd 0252 5786  .......d.{...RW.
-000025b0: a21b 5093 4e72 f3ef 1a84 a3ae cc44 b3b1  ..P.Nr.......D..
-000025c0: 0922 cb9e 55c1 a82b 33d1 9bf1 7417 3bbb  ."..U..+3...t.;.
-000025d0: 2472 e064 1590 ba32 14bd 3b43 0571 1fe0  $r.d...2..;C.q..
-000025e0: dbe7 4840 eaca 5034 3b1b cdcd 6791 80d4  ..H@..P4;...g...
-000025f0: 95a9 e806 d498 93dc 2c55 5485 a4ae 4c4b  ........,UT...LK
-00002600: 3780 369d e4e6 2785 85b0 ae4c 5137 621b  7.6...'....LQ7b.
-00002610: 9dc6 d29c 55c8 ebca 18b5 3176 31e5 d0c0  ....U.....1v1...
-00002620: 2ae8 75ed 386a 8929 66ac 3707 dbb4 0863  *.u.8j.)f.7....c
-00002630: 5d3b 605a 1d5c 1e39 96aa 0a4d 5d0d 1a0d  ];`Z.\.9...M]...
-00002640: 149a 93f8 ee89 d0d4 b543 a3f5 ccdc 5a86  .........C....Z.
-00002650: fecc 2476 3a06 5a1d 3892 7c1d 173e ba76  ..$v:.Z.8.|..>.v
-00002660: b0b3 1830 08dd 2ce9 5e05 84ae 0684 ee8f  ...0..,.^.......
-00002670: 8981 cd47 01a1 6b07 35ab 8179 9fe6 1f60  ...G..k.5..y...`
-00002680: 219e 6b47 2fab 8319 79f9 0655 d0e6 6ad0  !.kG/...y..U..j.
-00002690: e6fe 989e 83bf 4a52 cd0d da1c 1fbb 1425  ......JR.......%
-000026a0: f599 89e4 399e 4fe8 0441 f952 9b99 3c9e  ....9.O..A.R..<.
-000026b0: 013a eb14 8181 545b 468c 67e2 bc9c c4be  .:....T[F.g.....
-000026c0: 5511 28b9 3261 3c23 e6e5 34d6 58a8 e4ca  U.(.2a<#..4.X...
-000026d0: 88f1 8c94 97d3 7863 a9fc cc18 cfb0 6898  ......xc......h.
-000026e0: 95d8 371b 8225 d78e 3196 a73d 3c76 294a  ..7..%..1..=<v)J
-000026f0: 2a3f d3c4 4b7c c742 34f9 52be 547d 8689  *?..K|.B4.R.T}..
-00002700: 1778 da43 34f9 6220 359f 1724 5ee8 6977  .x.C4.b 5..$^.iw
-00002710: 127f ef25 2698 4a5e f0de 1b89 bff7 121f  ...%&.J^........
-00002720: 6609 e3fe d869 e087 ac42 2b57 468f 17ea  f....i...B+WF...
-00002730: 6d18 898f 70a1 95ab a195 fb63 72e5 ec99  m...p......cr...
-00002740: 35c1 959b 59d9 383e 7629 6a92 a2b0 1aaf  5...Y.8>v)j.....
-00002750: e153 dd0b 82f2 9394 8f2d fb1a 579b 5e11  .S.......-..W.^.
-00002760: 1864 31e0 af08 a0da 5889 ab36 4d20 e4c6  .d1.....X..6M ..
-00002770: 4431 fb1a 89ed 8334 8190 1b03 c56c 4c92  D1.....4.....lL.
-00002780: 7437 7aea 9a18 63ad 6763 96d8 be75 1302  t7z...c.gc...u..
-00002790: b975 34b1 3eed 1814 ab1d 4d36 018d 1b43  .u4.>.....M6...C
-000027a0: c32b 24a0 95b8 046c 8219 3766 86d9 d748  .+$....l..7f...H
-000027b0: 6c42 35e1 8c1b 43c3 2bec a865 25ee 7d7f  lB5...C.+..e%.}.
-000027c0: 13cc b831 33bc f986 9388 56e2 b8a6 2694  ...13.....V...&.
-000027d0: 71eb 9061 7982 1827 5e07 7543 70e2 6656  q..ay..'^.uCp.fV
-000027e0: 37ee 8fa9 837d 4885 1b6e e11a c62f 0e1c  7....}H..n.../..
-000027f0: 2c83 8742 7285 79df 159a 4b27 195c 3a89  ,..Br.y...K'.\:.
-00002800: 15e6 7d57 98d1 7612 9fa3 4208 37a6 7dd9  ..}W..v...B.7.}.
-00002810: 9724 e96e 709d 256d 3ad6 576f e470 b99a  .$.np.%m:.Wo.p..
-00002820: 26c0 6f43 7a77 cbf5 f804 86dc 5c13 b0b7  &.oCzw......\...
-00002830: 21a5 bb95 1f1b 748a c040 0201 69dc dd20  !.....t..@..i.. 
-00002840: 7ee6 9cc4 4264 4d00 de86 34ee 610c e766  ~...BdM...4.a..f
-00002850: 3416 226b 42f0 36c4 710f e770 8c67 3596  4."kB.6.q..p.g5.
-00002860: 2a6d 82f0 36e4 710f e7f0 adb7 d50c 9c25  *m..6.q........%
-00002870: 5a90 c73d 9cc3 57c0 5663 79e9 260c 6f43  Z..=..W.Vcy.&.oC
-00002880: 1e77 778e 2bb9 93d8 a65d 08de 8638 aef1  .ww.+....]...8..
-00002890: 3512 fb25 4f13 84b7 218f 6b8c 8dc4 7ec9  5..%O...!.k...~.
-000028a0: d384 e16d c8f0 6ea5 c053 3d0e 2381 781b  ...m..n..S=.#.x.
-000028b0: 42bc bb41 9c15 4e62 c1b9 2670 6f43 5277  B..A..Nb..&poCRw
-000028c0: 378e 2fa9 9358 86ac 09dd db90 d4dd 8de3  7./..X..........
-000028d0: 6e9a 9358 48b1 09dc db10 d435 c646 62d9  n..XH......5.Fb.
-000028e0: b526 6c6f 634e 9736 ed36 92d5 ceae 3721  .&locN.6.6....7!
-000028f0: 7b5b 87e9 4a9b 1c1e bb14 2589 83b0 6e82  {[..J.....%...n.
-00002900: 6665 ccea 3661 751b 82b7 5bf9 6030 9c75  fe..6au...[.`0.u
-00002910: 6d02 e536 246c 7703 a867 e36e 8bd0 b70d  m..6$lw..g.n....
-00002920: 49da dd01 eef2 382b 84b2 6d48 cc6e 0e71  I.....8+..mH.n.q
-00002930: 188d d714 6e02 d336 0463 7783 f822 7592  ....n..6.cw.."u.
-00002940: c041 2a3f 02b0 bb43 7c91 3a49 e020 b51c  .A*?...C|.:I. ..
-00002950: 41d7 3401 c2d2 4b02 07a9 ce08 b4ee 0ef1  A.4...K.........
-00002960: 78af 9304 0e52 7111 5cdd 1de0 3e8c ebb3  x....Rq.\...>...
-00002970: 40ad 0da1 d684 9134 a65a 9b50 ad2d 4454  @......4.Z.P.-DT
-00002980: 5f8a 1ad7 5dc1 571b b2a8 295e 43ae 1704  _...].W...)^C...
-00002990: e54b cd45 e274 2b1f 0cc6 1557 60d4 8660  .K.E.t+....W`..`
-000029a0: e96e 10df 4f27 b1b3 79c2 a236 e44a 0fdf  .n..O'..y..6.J..
-000029b0: f8d4 9cc6 8f44 8445 6dc8 951e ce71 5839  .....D.Em....qX9
-000029c0: 8d1f 8908 8cda 102c dd4a 01df 71f5 17e6  .......,.J..q...
-000029d0: b421 3fba 1bc0 cd64 89fd 1eb5 0971 da90  .!?....d.....q..
-000029e0: 1e3d 7ce1 66b2 c67f 90da 8438 6d88 8f1e  .=|.f......8m...
-000029f0: ce70 5159 e33f 566c c29c 3604 4813 6df3  .pQY.?Vl..6.H.m.
-00002a00: e624 7ef6 4690 d316 2eb0 fb62 300e 1781  .$~.F......b0...
-00002a10: 481b 12a1 29fe 5ebb 17f4 e50b 2bda 10fc  H...).^.....+...
-00002a20: 4cb0 a55b af08 0c24 4410 f04c b4a5 9b95  L..[...$D..L....
-00002a30: d8e7 bd49 8434 8c83 0c15 b953 0427 2649  ...I.4.....S.'&I
-00002a40: 8124 e76e 0027 c612 5f91 05fe 6c08 781e  .$.n.'.._...l.x.
-00002a50: be70 cf58 33a8 c802 8536 043f 9d33 6bfc  .p.X3....6.?.3k.
-00002a60: a7e5 4d60 d186 e4e7 e10c b793 3583 0811  ..M`........5...
-00002a70: 5ab4 21fa 9968 6b4c 27f1 eb16 34a1 451b  Z.!..hkL'...4.E.
-00002a80: 929f c618 25d9 cfc4 0a2b da90 fb4c 9932  ....%....+...L.2
-00002a90: d348 fcf9 0a29 da90 fa64 5fb3 4aaf 6563  .H...)...d_.J.ec
-00002aa0: 9b70 a2ad 833e 25ab c363 97a2 2472 10e3  .p...>%..c..$r..
-00002ab0: 4cf1 27f9 bd20 285f 1207 61cd 045b 30f6  L.'.. (_..a..[0.
-00002ac0: 8ac0 40a2 05a1 cc44 5b21 5a89 8d34 c138  ..@....D[!Z..4.8
-00002ad0: 1ba2 9a89 b6e7 b312 3b21 2970 6733 7067  ........;!)pg3pg
-00002ae0: 7cec 5294 e404 2299 295e c6ae 1704 e54b  |.R...".)^.....K
-00002af0: 1c20 9199 6019 bb5e 1118 48bd 4720 33d1  . ..`..^..H.G 3.
-00002b00: 3276 5662 efbd 309c 0d39 cddd 37be f74e  2vVb..0..9..7..N
-00002b10: 62ef bda0 9d0d f1cd dd37 1ee8 3b89 0f3a  b........7..;..:
-00002b20: 413e 9b41 3ee3 6397 a224 1090 df4c f10a  A>.A>.c..$...L..
-00002b30: 7abd 2028 5ff2 00e9 cd04 2be8 f58a c040  z. (_.....+....@
-00002b40: 2a3e ae4b 9b68 d13a 2bf1 0f9d 547c a440  *>.K.h.:+...T|.@
-00002b50: 13ae 5967 35be 0f25 7c68 433e d439 1b8d  ..Yg5..%|hC>.9..
-00002b60: 7f57 2ee0 6843 0a34 e16a 7956 e3fb 5082  .W..hC.4.jyV..P.
-00002b70: 8e36 c440 13ae 9667 35be ae09 3bda 9003  .6.@...g5...;...
-00002b80: dd9d e370 7112 1b2e 828e 36e4 4077 df38  ...pq.....6.@w.8
-00002b90: 5c9c c4b2 2482 8e36 5c9e 36c1 3a6a bda2  \...$..6\.6.:j..
-00002ba0: afb0 0294 3604 4a13 ad10 e724 7ed0 23a0  ....6.J....$~.#.
-00002bb0: 6943 d0f4 f08d ab8d d10c 063d 42a0 36c4  iC.........=B.6.
-00002bc0: 490f 67b8 a8ac 190c 3d84 416d 0894 265a  I.g.....=.Am..&Z
-00002bd0: 9ece 49ec c243 4d18 d486 9c69 a2e5 e99c  ..I..CM....i....
-00002be0: c42e 8bd7 044d 6dc8 9926 5a4d cb49 ec02  .....Mm..&ZM.I..
-00002bf0: 4f4d d0d4 86f8 e9e6 1b87 5308 b3be 3198  OM........S...1.
-00002c00: 854c 9d71 21dd dd20 ac34 4e62 1742 9a05  .L.q!.. .4Nb.B..
-00002c10: 639d 1163 3d7c c34a e334 7e39 a259 00d7  c..c=|.J.4~9.Y..
-00002c20: 1901 d7c3 39ac 344e e397 239a 857c 9d11  ....9.4N..#..|..
-00002c30: 63dd 9dc3 4ae3 247e 3d97 59d0 d719 3956  c...J.$~=.Y...9V
-00002c40: 63cc 12ff a9ee 2ce8 ebcc 1ceb 661c 5657  c.....,.....f.VW
-00002c50: 27b1 0b30 cd42 bece 88b1 eebe 6175 7512  '..0.B......auu.
-00002c60: bb3e d22c e4eb 8c74 ebee 1b7e 56ef 24b6  .>.,...t...~V.$.
-00002c70: ff34 0b10 3b23 ddba fb86 5fd5 3b89 45f2  .4..;#...._.;.E.
-00002c80: 6601 6267 a45b 77df f07b 5227 b1af ff67  f.bg.[w..{R'...g
-00002c90: e161 6784 5b13 7ddc ee24 1ec4 9d05 889d  .ag.[.}..$......
-00002ca0: 916e 4df4 41a4 930c 7c25 b410 7a4d b48a  .nM.A...|%..zM..
-00002cb0: 8093 f80f 7767 e164 6764 6113 2d9b e024  ....wg.dgda.-..$
-00002cc0: 3eb2 849e 9d0d 3d1b 1fbb 1425 2184 d06b  >.....=....%!..k
-00002cd0: 8a3f abeb 0541 f912 3608 b726 f8ac ae57  .?...A..6..&...W
-00002ce0: 0406 922a 4cb1 d267 7556 62db 6801 5f67  ...*L..guVb.h._g
-00002cf0: 5ce4 36e1 6775 56e3 8d25 5618 93c5 cfea  \.6.guV..%V.....
-00002d00: acc6 1a0b 3f3b 333f 4b9f d559 896d af04  ....?;3?K..Y.m..
-00002d10: ab9d 9991 dd7d e32b ed34 de58 7285 11d9  .....}.+.4.Xr...
-00002d20: dd38 bed2 4ee3 8d25 5798 90dd 8dc3 aead  .8..N..%W.......
-00002d30: d578 6309 960e 9095 6009 8f5d 8a92 6061  .xc.....`..]..`a
-00002d40: e235 fe82 b117 04e5 4bb0 30d8 0a5f 30f6  .5......K.0.._0.
-00002d50: 8ac0 4082 8509 56fa 82d1 4a7c 3593 6061  ..@...V...J|5.`a
-00002d60: 8075 c160 711a 6f2c c1c2 cceb 82c1 e234  .u.`q.o,.......4
-00002d70: d658 58d8 99c1 56fa 66d3 4aec d32e 28ec  .XX...V.f.J...(.
-00002d80: cc5c eb82 c1e2 34de 5882 85b9 d605 83c5  .\....4.X.......
-00002d90: 69bc b104 0b73 ad0b 068b d378 6309 16e4  i....s.....xc...
-00002da0: 5a77 e3b8 a7d4 49fa ea2a d0eb 8c6b d3ee  Zw....I..*...k..
-00002db0: 0e71 afd7 49ec a846 08d9 9909 d9dd 171e  .q..I..F........
-00002dc0: 22a3 f1c6 924f 8cce eec6 f010 198d 3796  "....O........7.
-00002dd0: 8062 a496 be44 7612 dfeb 15d0 760e a9d9  .b...Dv.....v...
-00002de0: 1783 f1c4 8e10 b533 13b5 f177 c2bd 2028  .......3...w.. (
-00002df0: 5f92 8581 5af8 4eb8 5704 0692 20cc d3d2  _...Z.N.W... ...
-00002e00: d7ab 5662 a35a 28db 9929 5bf6 6589 1f69  ..Vb.Z(..)[.e..i
-00002e10: 097b 3b33 7b4b 1f97 5a89 cd2d 2172 6726  .{;3{K..Z..-!rg&
-00002e20: 7257 6c22 9cc6 1b4b ac30 a8bb 6213 e134  rWl"...K.0..b..4
-00002e30: de58 6205 57a5 4df4 35ad 95d8 5411 d877  .Xb.W.M.5...T..w
-00002e40: 66d8 77f7 852b 6d34 de58 6285 29e0 dd18  f.w..+m4.Xb.)...
-00002e50: aeb4 d158 63a1 8367 467d 77e3 b831 761a  ...Xc..gF}w..1v.
-00002e60: 6f2c e9c4 a82f 7db8 6c25 6ebe 7e16 3878  o,.../}.l%n.~.8x
-00002e70: 66d0 97be c975 12df 7008 1a3c 331a 4cdf  f....u..p..<3.L.
-00002e80: c63a 899f 9712 6278 eef0 5f69 b0c2 6397  .:....bx.._i..c.
-00002e90: a224 8710 e8cd f1b7 b1bd 2028 5fe2 06b1  .$........ (_...
-00002ea0: dd0c dfc6 f68a c040 6205 f1dc 4cdf c65a  .......@b...L..Z
-00002eb0: 896d b084 e89d 7145 d88c 9fc6 5a8d 3796  .m....qE....Z.7.
-00002ec0: 5841 fe37 e397 b156 638d 050c 9e11 0cce  XA.7...Vc.......
-00002ed0: f4cd a495 d886 4378 e119 e1df 4c5f 343a  ......Cx....L_4:
-00002ee0: 897d c33c 3749 9546 1171 f8c6 77d8 6806  .}.<7I.F.q..w.h.
-00002ef0: c612 2b08 051f c6f1 1d36 9a81 b1e4 0a42  ..+......6.....B
-00002f00: c199 3ee1 7412 fb7e 7916 8c78 4624 38d3  ..>.t..~y..xF$8.
-00002f10: 8794 4e62 df2f cf02 11cf 0804 6f85 4076  ..Nb./......o.@v
-00002f20: 1889 7f0d 2b08 f18c 3cf0 e10b 4f16 6b06  ....+...<...O.k.
-00002f30: c612 5ac8 031f c6f0 64b1 6660 2ca1 d501  ..Z.....d.f`,...
-00002f40: c1d2 6221 2cbc 19d8 4748 60e1 19c9 dffd  ..b!,...GH`.....
-00002f50: cca0 3f6d 3403 6349 275c 22f6 308e 2fa9  ..?m4.cI'\".0./.
-00002f60: d10c 8c25 9e78 89d8 028b 89b3 24df f9b7  ...%.x......$...
-00002f70: 80c2 1ccf bc40 2cfb b2c4 77b6 0445 9e91  .....@,...w..E..
-00002f80: 2b3e 2e74 dcab 359a c185 9674 42b0 7833  +>.t..5....tB.x3
-00002f90: 86fb 3bee 2309 743c e3aa b1bb 411c 4346  ..;.#.t<....A.CF
-00002fa0: f268 2ba5 10ca 3312 ca87 2fd4 19d6 0c8c  .h+...3.../.....
-00002fb0: 2586 105d 3e8c e19a b266 602c 3184 7cf2  %..]>....f`,1.|.
-00002fc0: 6e1c 3770 46f2 681f 2141 9a67 e493 0fdf  n.7pF.h.!A.g....
-00002fd0: f84a 1bcd c058 d209 01e5 c338 bed2 4633  .J...X.....8..F3
-00002fe0: 3096 74c2 a56a f31d 0d8d 8cc4 0f8d 0480  0.t..j..........
-00002ff0: 9e11 80de 7de3 ae84 910c 681f 21a3 6724  ....}.....h.!.g$
-00003000: a377 e318 0631 9201 ed23 c4f4 8cf8 f36e  .w...1...#.....n
-00003010: 1c0f ba8d c4cf 9c09 313d 23fd bcfb c6ed  ........1=#.....
-00003020: 8091 0c2e b4a4 16b2 cfbb 6f9c 9646 e2a9  ..........o..F..
-00003030: 1ba1 a5e7 8e7c 962e 4c78 ec52 94c4 10a2  .....|..Lx.R....
-00003040: cc19 52b7 13f4 e50b e43c 23b1 9c61 f18b  ..R......<#..a..
-00003050: 5e11 1848 ac20 9a9c 69f1 0b2b b1f9 2d34  ^..H. ..i..+..-4
-00003060: f38c 3473 a625 31ac c4a6 9940 ce33 12cb  ..4s.%1....@.3..
-00003070: 872f 5c52 a3f1 c692 2a48 2c1f c671 7e3b  ./\R....*H,..q~;
-00003080: 8d37 9654 4160 39c3 d220 bd22 7884 243e  .7.TA`9.. ."x.$>
-00003090: 104c ceb4 3488 93f8 31ae b0cc 3382 c987  .L..4...1...3...
-000030a0: 2fdc 4ad6 0c8c 253f 904c 3e8c e19a b266  /.J...%?.L>....f
-000030b0: 602c 6983 34f3 611c 779c 8dc6 1a2f 4239  `,i.4.a.w..../B9
-000030c0: 2f88 2c67 5a9b c549 ec74 c222 94f3 82c4  /.,gZ..I.t."....
-000030d0: f2e1 1bde 62a7 1918 2731 3659 03bd 2da7  ....b...'16Y..-.
-000030e0: 1918 6731 3659 f310 8f8d 9c66 605c c4d8  ..g16Y.....f`\..
-000030f0: 644d 3c73 e324 76e6 6611 c479 415e f9f0  dM<s.$v.f..yA^..
-00003100: 855b cc9a 8171 1363 175b f14b 1da7 1918  .[...q.c.[.K....
-00003110: cf62 ec72 2b7e a9e3 3403 e345 8c4d 06c5  .b.r+~..4..E.M..
-00003120: aec3 ced0 2234 f382 68f2 563e dcc8 616f  ...."4..h.V>..ao
-00003130: 6811 6c79 4106 7937 085b 1a27 b173 5e8b  h.lyA.y7.[.'.s^.
-00003140: 50cb 0b22 c887 6f7c 6a46 3330 9618 4206  P.."..o|jF30..B.
-00003150: f930 8e6f 9ad1 0c8c 2586 9041 ce71 33d3  .0.o....%..A.q3.
-00003160: 0b82 3b29 6983 0bf8 6ee5 c3f5 1cbe 0d5b  ..;)i...n......[
-00003170: 045a 5e10 5ade 0de0 5161 899d 9758 0466  .Z^.Z...Qa...X.f
-00003180: 5e10 663e 7ce1 d458 3330 9654 4162 f930  ^.f>|..X30.TAb.0
-00003190: 8647 8535 0363 4915 2496 77e3 b86f 6024  .G.5.cI.$.w..o`$
-000031a0: 765e 6211 c879 4160 79f7 8d1b acf1 6ac0  v^b..yA`y.....j.
-000031b0: 8bd0 cc0b a2c9 8743 7c2f 5133 95f7 6e80  .......C|/Q3..n.
-000031c0: ba08 cebc 209a 7c18 c7f7 b2d3 04e7 26c9  .... .|.......&.
-000031d0: 8210 729e 60a7 3c27 b11b c22e c22d 2fc8  ..r.`.<'.....-/.
-000031e0: 201b 5fb3 ade2 2fd6 5702 07d7 f5dd 7dc3   ._.../.W.....}.
-000031f0: 2de3 9cc4 2e41 b208 e3bc 20e3 6c7c 7973  -....A.... .l|ys
-00003200: b377 5fac afe4 10b2 cf99 d609 7412 3ba7  .w_.........t.;.
-00003210: b308 12bd 20df 9c69 f540 27b1 7367 8b20  .... ..i.@'.sg. 
-00003220: d10b e2cd 99d6 7674 123b 77b6 0811 bd20  ......vt.;w.... 
-00003230: dd9c 69c5 4727 b173 588b 00d1 0bd2 cdec  ..i.G'.sX.......
-00003240: 8b92 a9d9 ad3d 1701 a217 849b 77df 70ae  .....=......w.p.
-00003250: d049 ecbb aa45 78e8 05d9 66e3 8baf d5da  .I...Ex...f.....
-00003260: 7bfb 5c09 0ebd 20da bcfb 8693 c14e 62b7  {.\... ......Nb.
-00003270: 765b 8486 5e90 8636 be28 493e af84 915e  v[..^..6.(I>...^
-00003280: 1078 de7d c32f 129d c4ee 79b2 0823 bd20  .x.}./....y..#. 
-00003290: ef6c 7c71 5384 e473 4310 e925 5c2b f8c5  .l|qS..sC..%\+..
-000032a0: 60b8 8ccf 22d0 f382 0473 8699 8af1 2ac2  `..."....s....*.
-000032b0: 8bc0 cd0b ae22 9c61 2d52 ab70 1748 38e8  .....".a-R.p.H8.
-000032c0: 0539 e84c 0b94 5a89 ed56 0a1f bd20 1f9d  .9.L..Z..V... ..
-000032d0: 7181 52ab f1c6 9234 0841 675c 9fd4 6abc  q.R....4.Ag\..j.
-000032e0: b144 0d52 d087 713c ec72 1a6f 2c59 8318  .D.R..q<.r.o,Y..
-000032f0: 7486 99ae f19a c58b 10d2 0bd2 ce5b f970  t............[.p
-00003300: 238d c29e 9524 0aa2 cebb 2b3c b846 e2af  #....$....+<.F..
-00003310: a624 0aa2 cebb 6fdc 0372 123b 1e12 3a7a  .$....o..r.;..:z
-00003320: 41d2 f9f0 85eb 6c34 de58 7209 49e7 c318  A.....l4.Xr.I...
-00003330: 9e20 a3b1 c642 472f 483a efc6 719f cf49  . ...BG/H:..q..I
-00003340: ec3c 9ac0 d10b 92ce 393d 42df da48 dedb  .<......9=B..H..
-00003350: 2816 387a e948 6769 ab90 82de 82c0 f7de  (.8z.Hgi........
-00003360: 0583 5ec2 f58e 5f1c 286a 66df da0a eebc  ..^..._.(jf.....
-00003370: 18dc b93f 7676 d71e 7cbf 4928 e885 29e8  ...?vv..|.I(..).
-00003380: 44e3 4b23 f1e3 5aa1 a317 a6a3 6939 6227  D.K#..Z.....i9b'
-00003390: 19dc 3149 1b26 a069 2951 2719 dc49 491b  ..1I.&.i)Q'..II.
-000033a0: 06a0 138d b78c c48f b784 995e 987f 4e34  ...........^..N4
-000033b0: ee31 123f de12 647a 61fe 39d1 f8c3 48fc  .1.?..dza.9...H.
-000033c0: b847 90e9 85f9 e744 e300 23f1 f5a8 49d6  .G.....D..#...I.
-000033d0: 34ce 13ea 8f1b 891f 0708 31bd 30fd ccbe  4.........1.0...
-000033e0: 383f 941e ec96 e98b 10d3 4b87 3f4b 3421  8?........K.?K4!
-000033f0: 1a3d b577 ff66 0d24 993a ce59 0d28 8216  .=.w.f.$.:.Y.(..
-00003400: bf9d fd22 0cf4 d201 cd6a c0db d9fb 9d38  ...".....j.....8
-00003410: 17a1 9d97 8e5c 5687 f160 49f8 e585 5964  .....\V..`I...Yd
-00003420: 9858 ed04 41f9 9213 8c22 c3da e756 e12e  .X..A...."...V..
-00003430: 90b0 cb0b 73c8 b420 ba95 d83e a7a0 cb0b  ....s.. ...>....
-00003440: 63c8 1968 1a2b b13d 3021 9717 c690 337c  c..h.+.=0!....3|
-00003450: 0968 25b6 0726 e4f2 8218 f2e1 1bdf 5fa7  .h%..&........_.
-00003460: f1c6 9212 8c21 67fa 12d0 6abc b1a4 07a3  .....!g...j.....
-00003470: cb19 3ec8 b312 f741 de22 44f3 c278 72a6  ..>....A."D..xr.
-00003480: 6fd7 adc6 1b4b d630 9e9c e9db 75ab f1c6  o....K.0....u...
-00003490: 924c 8c27 efc6 f130 dc69 bcb1 4416 f3c9  .L.'...0.i..D...
-000034a0: 9b71 dcc5 7092 ea7c 0569 5e18 4fde 7de3  .q..p..|.i^.O.}.
-000034b0: 5bec 34de 5852 8bf1 e4dd 38be c54e e38d  [.4.XR....8..N..
-000034c0: 25b6 984f de8d e35b ec34 de58 728b 01e5  %..O...[.4.Xr...
-000034d0: dd38 dc17 d26a bcb1 e416 03ca 9b71 dc8d  .8...j.......q..
-000034e0: 7492 667d 25b6 3a3e 597a 0ccc 2e67 ff3e  t.f}%.:>Yz...g.>
-000034f0: 42d8 e5a5 0391 d580 73c8 bf00 1048 7961  B.......s....Hya
-00003500: e298 f62e 7012 3fb0 1348 79c1 e599 77df  ....p.?..Hy...w.
-00003510: b849 3712 3fb0 13a2 7961 a239 d3c0 ce48  .I7.?...ya.9...H
-00003520: fcc0 4e48 e725 e496 bf19 3005 3d18 290b  ..NH.%....0.=.).
-00003530: e9bc 74d8 b21a e0a6 dbcd 4fcf 08d2 bc84  ..t.......O.....
-00003540: cb2d bf18 0c97 625e 8452 5e98 3886 26b7  .-....b^.R^.8.&.
-00003550: 1304 e54b 1c30 580c bb4d f48a c040 ea3d  ...K.0X..M...@.=
-00003560: 43c7 b4db 8495 d88e b0b0 c80b 83c5 05df  C...............
-00003570: 1a38 8d37 9698 60b0 b8e0 5b03 a7f1 c692  .8.7..`...[.....
-00003580: 130c 1617 7c6b e034 de58 8222 5c28 f9c5  ....|k.4.X."\(..
-00003590: 6008 daac 8217 afcc 0ac7 dd8f 5e10 943f  `...........^..?
-000035a0: 49f9 d869 800d 367a 4560 90c4 003b 07b4  I..i..6zE`...;..
-000035b0: c186 95b8 7bb0 0a2d bc76 e4ef 790f fa63  ....{..-.v..y..c
-000035c0: 7fd8 a088 01cf 8af4 c7fe b041 1503 acf5  ...........A....
-000035d0: b445 8895 b891 eb2a f4ef ca24 6f85 66dd  .E.....*...$o.f.
-000035e0: 49fc 14fb 2af4 efda 91bc 7a45 7947 6cdb  I...*.....zEyGl.
-000035f0: 0cad 42f9 aebc 3031 7d55 e524 b601 5f85  ..B...01}U.$.._.
-00003600: fe5d 91fe 9dca e67b 171b 63cf 61b6 2fdc  .].....{..c.a./.
-00003610: 56a1 82d7 0ef1 952b caf8 effc e04f 4df8  V......+.....OM.
-00003620: dfb5 6379 d501 b365 7370 336b ab80 be6b  ..cy...esp3k...k
-00003630: 07ed aa03 26c5 e6e0 2692 5721 7a57 267a  ....&...&.W!zW&z
-00003640: 677a 2cc6 4cef 2a4c efca 4c2f 3b0c 7b15  gz,.L.*L..L/;.{.
-00003650: ab40 bd2b 13ba 33f4 897b 49e0 20b1 c028  .@.+..3..{I. ..(
-00003660: ee0c bddf 5e12 3848 fd67 e676 860d 037a  ....^.8H.g.v...z
-00003670: 49e0 2001 c04b 08df c15e 0b2c 597d ee08  I. ..K...^.,Y}..
-00003680: 8fbb 8670 ed4b f954 cf57 bf94 f62a 38ee  ...p.K.T.W...*8.
-00003690: daa1 b562 c0ab 08fb ef51 57c1 6e57 c66e  ...b.....QW.nW.n
-000036a0: f1d6 1889 0f30 6171 5706 6b67 d85e c049  .....0aqW.kg.^.I
-000036b0: 06be 1209 cce2 6285 3592 81af 0405 83b5  ......b.5.......
-000036c0: 588d 8d64 e02b f1c1 2c2e 566e 2319 f84a  X..d.+..,.Vn#..J
-000036d0: a884 ab0a bf18 70e0 5810 6215 e876 ed08  ......p.X.b..v..
-000036e0: 5a35 e0bc 19b4 8082 d7ae 1d2b ab0e 389a  Z5.........+..8.
-000036f0: 18b5 8002 d2ae 1d15 ab0e a69b e05b 4041  .............[@A
-00003700: 6657 4666 f171 ef24 7df2 0a1c bb32 e98a  fWFf.q.$}....2..
-00003710: 0f76 2709 1c24 2a18 83c5 47b8 9304 0e12  .v'..$*...G.....
-00003720: 0a4c af62 081a 890f 5f01 5e57 a657 3104  .L.b...._.^W.W1.
-00003730: c7cb ffae 82b6 aecc a9f2 b51b f71e 0462  ...............b
-00003740: 5d19 62e5 6b37 ee3d 08ae bae2 eabc 4727  ].b.k7.=......G'
-00003750: 1b2c 58f3 eeb3 bd3d 1200 08b7 3a63 d454  .,X....=....:c.T
-00003760: 9f0b 42bd aecc b0ce 007c b064 3b61 f7c1  ..B......|.d;a..
-00003770: c82a dceb ca10 2bfa a264 3b5f 9b52 c2bd  .*....+..d;_.R..
-00003780: aecc b0b2 af1b 8238 7c60 15ee 75ed 1856  .......8|`..u..V
-00003790: 09e0 f0d8 a528 c910 a652 e3bd 2b7b 4150  .....(...R..+{AP
-000037a0: be64 0503 abb0 7765 af08 0c24 2a98 3fa5  .d....we...$*.?.
-000037b0: bd2b adc4 f614 8459 5d19 406d b43a 85d5  .+.....Y].@m.:..
-000037c0: d81e 8440 ab2b 13a8 c678 3c2c 113e 7565  ...@.+...x<,.>ue
-000037d0: d6b4 d102 18bd 26b0 90ac 60aa b4d1 daf5  ......&...`.....
-000037e0: bda6 b710 e674 4580 74a5 dac9 0a4b 17ae  .....tE.t....K..
-000037f0: 429c ae8c 8fd2 f645 2c19 d94a 2420 54ca  B......E,..J$ T.
-00003800: 278b fd93 c12e 51ab 60a8 2ba2 a6e6 744d  '.....Q.`.+...tM
-00003810: e40c 8c25 5890 41cd b43d 9593 0c66 0505  ...%X.A..=...f..
-00003820: 5b5d 9141 9de8 f335 27f1 8376 c156 d770  [].A...5'..v.V.p
-00003830: 89de 1783 71d7 4448 d495 b1d2 789b a85e  ....q.DH....x..^
-00003840: 1094 2ff9 c1f8 286c 13d5 2b02 0349 8f8e  ../...(l..+..I..
-00003850: 13d5 6bc1 bd10 1fb2 c290 ae1d 102a 0608  ..k..........*..
-00003860: 8b4e edbd adaf 028b ae1d f9a9 0666 72c3  .N...........fr.
-00003870: b64f 4d02 a199 990a 6817 9dc4 5f39 0904  .OM.....h..._9..
-00003880: a642 d997 bf1a 1e5c 50c9 0303 85f6 c764  .B.....\P......d
-00003890: d463 7b7b 0285 aebc f8ed 1c2f ced4 2bfa  .c{{......./..+.
-000038a0: 875a a0d0 9557 b99d 6171 2627 f113 0682  .Z...W..aq&'....
-000038b0: 8aae bcc8 2dfb b2c4 27b8 70a5 2b73 a5ec  ....-...'.p.+s..
-000038c0: 8bc3 94f6 de71 cbab f0a6 2bd3 a333 2d46  .....q....+..3-F
-000038d0: d56b fa5b 2970 e9ca a4e8 4ccb 4e39 8d7f  .k.[)p....L.N9..
-000038e0: 4885 2e5d 1915 9d69 d9a9 5e13 9c9b 040b  H..]...i..^.....
-000038f0: 53a1 bb45 0846 398d 1f5e 0a49 ba32 15ba  S..E.F9..^.I.2..
-00003900: 19c7 5d8d 4e12 9c9a 6408 e39f 73bc 0571  ..].N...d...s..q
-00003910: af08 0c24 4398 f39c 6193 5827 b19f 41ad  ...$C...a.X'..A.
-00003920: 8286 ae8c 79b2 af89 165b d584 0c5d 99f2  ....y....[...]..
-00003930: 645f 9c02 a9be af24 60e8 ca90 e70c 9be2  d_.....$`.......
-00003940: 3a89 1f98 0b17 ba32 e439 c3a6 b84e e2ab  :......2.9...N..
-00003950: 8670 a12b 339e 15e0 6e2b b1cf 9560 a1ab  .p.+3...n+...`..
-00003960: 413c e1f3 3a27 f1f7 57a8 d0b5 233c a5b1  A<..:'..W...#<..
-00003970: 0f8f 5d8a 9254 6166 33de d9b0 1704 e54b  ..]..Taf3......K
-00003980: a630 9b09 3b1b f68a c040 3285 d94c dad9  .0..;....@2..L..
-00003990: d04a 6c07 5370 ce95 914d dcd9 d06a ecb6  .Jl.Sp...M...j..
-000039a0: e6ab 709e 2b43 9bb8 b5a1 d5d8 6dcd 5721  ..p.+C......m.W!
-000039b0: 3d57 c636 696f 432b b19d 6a21 3d57 c636  =W.6ioC+..j!=W.6
-000039c0: 716f 43ab b16b 0aac c27a aecc 73e2 e686  qoC..k...z..s...
-000039d0: 5663 3f0a 5f05 025d 79ed 5ada 64d0 4a6c  Vc?._..]y.Z.d.Jl
-000039e0: a609 1bba f2da b50b 7db0 6235 f693 a455  ........}.b5...U
-000039f0: 50d2 9551 d285 be58 b19a abe4 e22c 21c5  P..Q...X.....,!.
-00003a00: 90e9 429b 5759 cd55 7271 96f4 6294 7477  ..B.WY.Urq..b.tw
-00003a10: 8e7b 934e 7395 5c9c 25bf 9825 5da8 ed32  .{.Ns.\.%..%]..2
-00003a20: 927b df78 097f ba32 4bca c624 291e 8f5f  .{.x...2K..$).._
-00003a30: 053f 5d19 25a5 9d1e 9d64 3063 26f8 e96a  .?].%....d0c&..j
-00003a40: f0d3 f8d8 9ba2 a63b e14f 8f7f c09f 146f  .......;.O.....o
-00003a50: f618 2822 8b49 2d30 4660 bfc7 4012 7924  ..(".I-0F`..@.y$
-00003a60: f5c0 c4a0 ad17 034d 6492 d504 c361 a526  .......Md....a.&
-00003a70: da8b 6c1b bd49 8b9a 633e acd4 4a7b 916d  ..l..I..c>..J{.m
-00003a80: a637 6955 738c 8895 506b 2fba 6aae e64d  .7iUs...Pk/.j..M
-00003a90: cd31 2668 7bcb 4013 dddb 594d 3045 702f  .1&h{.@...YM0Ep/
-00003aa0: 4b2f b27d 824d baa8 39e6 02ee 67e9 45b6  K/.}.M..9...g.E.
-00003ab0: 5bb0 4957 35c7 8ecd 4aaf 8ebc e8aa b998  [.IW5...J.......
-00003ac0: 4f1a 3f4c a9ee e661 7be5 4557 cdd5 5c83  O.?L...a{.EW..\.
-00003ad0: 8901 d6dd fc09 cc8d e8aa b99a 6b62 31db  ............kb1.
-00003ae0: 4afb 3d5a 8d6f 3f36 a906 1913 b1b4 e7a3  J.=Z.o?6........
-00003af0: d5f8 d74c 9b54 738c 5959 e34d 9a92 3d67  ...L.Ts.YY.M..=g
-00003b00: b549 35c6 98a2 5de1 5d93 d5dc db49 e14d  .I5...].]....I.M
-00003b10: aa29 c67c 2dbd 52b4 1abf 76c1 26d5 700b  .).|-.R...v.&.p.
-00003b20: 31da 5713 1362 76a6 7493 6a88 7524 ed1b  1.W..bv.t.j.u$..
-00003b30: 93e1 0ba9 ed37 9a4a c8cd 9678 4fcf 4011  .....7.J...xO.@.
-00003b40: 5824 cd1e 2467 0b6e 42e9 4583 1635 69f6  X$..$g.nB.E..5i.
-00003b50: 203e 5b60 4fd1 4012 9da0 460c a2b2 85b6   >[`O.@...F.....
-00003b60: 150d 3491 8966 0972 b105 f710 f5a2 41a7  ..4..f.r......A.
-00003b70: 2869 9820 1c7b 9843 dbe5 4483 244b 9a26  (i. .{.C..D.$K.&
-00003b80: 48c8 16da 4b34 d044 9757 6303 29d9 c384  H...K4.D.Wc.)...
-00003b90: 2eaf cb0d 37fb ba49 3537 90a0 3dcc a986  ....7..I57..=...
-00003ba0: 1891 9ba1 d994 1a27 c8d6 963b 18d6 598d  .......'...;..Y.
-00003bb0: 1f50 6e52 0d1f a46e 0b7d 4864 35a3 b639  .PnR...n.}Hd5..9
-00003bc0: 6b2a 21ab 5b68 d331 ab19 3dd1 5943 0929  k*!.[h.1..=.YC.)
-00003bd0: de42 1b8f 59cd a87d cc1a 5621 acfb 6af2  .B..Y..}..V!..j.
-00003be0: 0752 296b 2a21 985b 2892 3a45 64a1 d983  .R)k*!.[(.:Ed...
-00003bf0: d86e 810d aa02 49e4 a111 83e0 6ea1 3daa  .n....I.....n.=.
-00003c00: 024d 64a2 1183 ecee 6142 a762 4483 c15d  .Md.....aB.bD..]
-00003c10: d688 4144 f730 8788 7122 37e1 be29 3562  ..AD.0..q"7..)5b
-00003c20: 90d2 2db4 1397 d70c 5aae ac11 83a4 6ec1  ..-.....Z.....n.
-00003c30: ddb8 bc68 d0f9 289a 3188 eb16 dc91 cb8b  ...h..(.1.......
-00003c40: 7cae 17cd 1844 7677 6fc8 18a7 198c b38b  |....Dvwo.......
-00003c50: 660c 2e56 7b78 d379 1bd1 609c 5d34 9210  f..V{x.y..`.]4..
-00003c60: 0d3e cce1 8e3b 919b 82df 949a 5588 0d1f  .>...;......U...
-00003c70: de30 cc76 223b 0bbf 4935 c490 0f3e cca1  .0.v";..I5...>..
-00003c80: 93e6 4483 26ad 68b8 758c b036 2b08 10ef  ..D.&.h.u..6+...
-00003c90: 6738 30d1 100b 79e0 5713 1356 7662 7f93  g80...y.W..Vvb..
-00003ca0: 6a5a 2145 5ca6 476a 9c8d e6de ae34 b349  jZ!E\.Gj.....4.I
-00003cb0: 35ad 102f 2e04 695a cda8 4354 35ac 9022  5../..iZ..CT5.."
-00003cc0: 2eb4 9f83 d58c ac35 ab90 242e b4a5 83d5  .......5..$.....
-00003cd0: 0c9e dbaa 5165 56bc 8583 d7d2 347b 9011  ....QeV.....4{..
-00003ce0: 2ed4 d484 ebe1 5e2d 3462 9006 2eb0 467b  ......^-4b....F{
-00003cf0: 2089 3c34 4910 fc2d b832 ba17 0d5a ecaa   .<4I..-.2...Z..
-00003d00: 4982 8bd6 165a 0ede 6b7c 47a5 6abe 2060  I....Z..k|G.j. `
-00003d10: 5c70 6176 2f1a 7416 aae6 0ed2 c705 1767  \pav/.t........g
-00003d20: f7a2 41f7 b06a f020 7d7c 9843 c3e5 4457  ..A..j. }|.C..DW
-00003d30: cdc5 bc69 f220 99bc 9b43 f50f 49e7 ab89  ...i. ...C..I...
-00003d40: 660c d2c9 8709 3cd3 4e34 e810 354d 9986  f.....<.N4..5M..
-00003d50: 7d9b c41d 4127 1a74 889a 8612 72ca 8739  }...A'.t....r..9
-00003d60: 3c58 4634 48f6 a669 8508 b3f5 36a2 c14b  <XF4H..i....6..K
-00003d70: 8fa6 3186 e8f3 610e 0fb5 130d 5e7a 348d  ..1...a.....^z4.
-00003d80: 3164 9c0f 7378 e9e1 4483 971e 4d83 0c41  1d..sx..D...M..A
-00003d90: e7dd 1cfa 11e3 e575 b7df 6860 21d5 7c98  .......u..h`!.|.
-00003da0: 508d 32a2 d183 a581 8534 f461 4e35 ca88  P.2......4.aN5..
-00003db0: 069d 8659 030b 99e7 c31c 9e6a 231a 796b  ...Y.......j#.yk
-00003dc0: 8e21 2abd 79c3 698f 49e9 ed37 1a57 c83d  .!*.y.i.I..7.W.=
-00003dd0: ef1e d004 1b8d 5dc7 6053 6a58 212d 5dd2  ......].`SjX!-].
-00003de0: 2375 058d e6de 7226 9b54 c30a 39ea bde7  #u....r&.T..9...
-00003df0: 4fa7 6db2 6a30 153a 6b56 212f 5d68 c707  O.m.j0.:kV!/]h..
-00003e00: ab19 7a6b 5421 33ed cedb 0ce9 46de 9a54  ..zkT!3.....F..T
-00003e10: c84d bbf3 3623 bd91 b706 18b2 d385 7636  .M..6#........v6
-00003e20: b09a c19b c259 e3ab c3a7 75d8 816c f51e  .....Y....u..l..
-00003e30: 53be fd5b 34a6 9095 2eb4 6384 d58c ac35  S..[4.....c....5
-00003e40: a510 9776 d626 d926 dff8 2d9a 5eb8 8eae  ...v.&.&..-.^...
-00003e50: f3fe 0323 bd45 730a f9eb a3c3 0ccd fb98  ...#.Es.........
-00003e60: c1de 7ea3 8984 14f6 5e33 e109 65cd e809  ..~.....^3..e...
-00003e70: 5d34 9010 b636 95c3 6846 d69a 4788 5b3b  ]4...6..hF..G.[;
-00003e80: 6bd6 8cac 358e 90b7 b6b7 f50f f49c 160d  k...5...........
-00003e90: 1e84 abad cb1f 78b5 bf68 c674 24b5 664c  ......x..h.t$.fL
-00003ea0: 78f0 52da aa61 8274 74a1 ae5e b8de eed5  x.R..a.tt..^....
-00003eb0: 4243 0339 e802 3b2a 0492 c843 c301 91e7  BC.9..;*...C....
-00003ec0: 42fb 2778 8def daac 1a19 c83c 1fd6 7482  B.'x.......<..t.
-00003ed0: 4634 9855 5935 4910 7b3e cca1 e3e8 4483  F4.UY5I.{>....D.
-00003ee0: a98d 55b3 04c9 676b 6e44 830e f3aa 6982  ..U...gknD....i.
-00003ef0: f4b3 3567 91dd e972 536a 9c18 009a e774  ..5g...rSj.....t
-00003f00: 9c68 30a7 b36a ca20 055d 68cb 0eaf 19e4  .h0..j. .]h.....
-00003f10: e8aa d9d3 f1d1 6fbc e959 6791 5d51 629a  ......o..Yg.]Qb.
-00003f20: 14b5 9e10 b53e bce3 1b6e 459e ce9a 14c2  .....>...nE.....
-00003f30: 9e10 c22e b45f 49a0 e943 6c52 0a7b 420a  ....._I..ClR.{B.
-00003f40: bbe0 e624 5664 b718 da94 59bd 5d8a a1b7  ...$Vd....Y.]...
-00003f50: 59d4 cf8f fa27 85b3 27e4 ac0b 6e8e 6245  Y....'..'...n.bE
-00003f60: 0f3e 4826 85b3 27e4 acad b9f9 0e76 64de  .>H&..'......vd.
-00003f70: d4dc a558 8c35 3a8d 1f92 4f8a 6c4f 485f  ...X.5:...O.lOH_
-00003f80: 17da 35c4 6aec a283 9b72 516b 1347 74c1  ..5.j....rQk.Gt.
-00003f90: c7dd a449 b9ec 0911 ebdd 03da 0727 baf9  ...I.........'..
-00003fa0: 9671 522e 7b42 c4da 991b d1cd 3710 9372  .qR.{B......7..r
-00003fb0: d913 22d6 8779 dc3a f5a2 e0fa 2a80 3d21  .."..y.:....*.=!
-00003fc0: 4c7d b8c4 b3b0 4e74 f363 c149 09ec 0969  L}....Nt.c.I...i
-00003fd0: 6a6b cea2 db64 b1be 4911 ecc9 e0d4 c69c  jk...d..I.......
-00003fe0: 45b7 c97d c1be 4935 ad90 a7b6 e62c ba4d  E..}..I5.....,.M
-00003ff0: be09 5608 7b42 a0da 9ab3 e836 d94e d7a4  ..V.{B.....6.N..
-00004000: 14f6 84a0 f561 0e2d 9411 dd7c 3f7b 523a  .....a.-...|?{R:
-00004010: 7bc2 758e 0ff3 9fc0 fc0f 6496 52db 9359  {.u.......d.R..Y
-00004020: 0939 38a8 a762 fb70 9372 db93 590d 3938  .98..b.p.r..Y.98
-00004030: a826 6e4b c44d aa19 14c2 d6af 261c 50b7  .&nK.M......&.P.
-00004040: e9af de44 2328 84ad 5f4d 386a fc64 e2a4  ...D#(.._M8j.d..
-00004050: 7cf6 c4a8 35ed e263 3583 5e91 d2d9 1383  |...5..c5.^.....
-00004060: d6b4 918f d50c e618 2785 b3a7 10b4 7e35  ........'.....~5
-00004070: e138 b18b 716c 4a4d 13c6 ac33 cd82 b166  .8..qlJM...3...f
-00004080: eff4 0dce 4fc3 8429 6bda acc8 6a86 de9a  ....O..)k...j...
-00004090: 2566 49e4 e0e0 1fbf b69a 2466 51e4 e0a0  %fI.......$fQ...
-000040a0: 78f8 4e8e a2d6 53b8 c6f1 8b07 33d5 d90f  x.N...S.....3...
-000040b0: 3827 45aa a770 95e3 570f 9e59 1e79 688c  8'E..p..W..Y.yh.
-000040c0: 3874 ba3f a859 e5c7 574a 544f 211f fd6a  8t.?.Y..WJTO!..j
-000040d0: e230 c5f0 4cde fff6 f3d3 d3d7 7fbc ff7a  .0..L..........z
-000040e0: ffe3 0fbf de7f 78fa 5ff7 cf1f 3efe f2db  ......x._...>...
-000040f0: 779f 9e7e da0a bafb bbfd 1dd2 f3c7 0f3f  w..~...........?
-00004100: bffe e3eb 975f b7bf e9fb ef1e be7c fdfa  ....._.......|..
-00004110: e5f3 f19f 3f3f dd3f 3e3d ef3f d88e fff4  ....??.?>=.?....
-00004120: e5cb d7d7 7fec cdd4 ef5f 9eff 7a98 fcf8  ........._..z...
-00004130: ff01 504b 0304 1400 0000 0800 f00b b158  ..PK...........X
-00004140: f7f6 8f09 a702 0000 6d0b 0000 0d00 0000  ........m.......
-00004150: 786c 2f73 7479 6c65 732e 786d 6cdd 56db  xl/styles.xml.V.
-00004160: 8e9b 3010 fd15 c407 944d 5051 a842 a436  ..0......MPQ.B.6
-00004170: d24a 95da 6aa5 dd87 be9a 6082 255f a831  .J..j.....`.%_.1
-00004180: ab64 bfbe 33b6 1392 ec0e ddf6 b1a0 84f1  .d..3...........
-00004190: 1c9f b93b 643d b8a3 e48f 1de7 2e39 28a9  ...;d=.......9(.
-000041a0: 872a ed9c eb3f 65d9 b0eb b862 c307 d373  .*...?e....b...s
-000041b0: 0d48 6bac 620e 9676 9f0d bde5 ac19 90a4  .Hk.b..v........
-000041c0: 64b6 bcbb 2b32 c584 4e37 6b3d aa7b e586  d...+2..N7k=.{..
-000041d0: 6467 46ed aaf4 2e4d b2cd ba35 7a52 2dd3  dgF....M...5zR-.
-000041e0: a080 bd4c f1e4 99c9 2add 3229 6a2b c266  ...L....*.2)j+.f
-000041f0: a684 3c06 fdd2 6b76 461a 9b38 8886 57e9  ..<...kvF..8..W.
-00004200: c2ab 8697 b061 1197 186a b4a5 8436 d66b  .....a...j...6.k
-00004210: b3e0 267c d791 7089 f8c7 003b 8494 d7f1  ..&|..p....;....
-00004220: 8162 b3ee 9973 dcea 7b58 0492 d7be c6a2  .b...s..{X......
-00004230: fc74 ec21 bebd 65c7 c5f2 637a c1f0 0f70  .t.!..e...cz...p
-00004240: 531b db70 7be5 28a8 366b c95b 870c 2bf6  S..p{.(.6k.[..+.
-00004250: 9d17 9ce9 f151 1be7 8c42 a911 6c6f 340b  .....Q...B..lo4.
-00004260: 919c 6857 74df c82a 751d 3462 b275 ab45  ..hWt..*u.4b.u.E
-00004270: c3b7 bae8 e556 7d76 1305 4861 c7a5 7cc4  .....V}v..Ha..|.
-00004280: 6d3f db73 1e0b c8e3 d026 a1f3 5f1b df74  m?.s.....&.._..t
-00004290: 2cec 4984 e4a3 18cc c405 3ab8 3417 8c5f  ,.I.......:.4.._
-000042a0: d85d fe9b dd5e 3c1b f765 848c b45f ff1a  .]...^<..e..._..
-000042b0: 8de3 0f96 b7e2 e0d7 8776 0a80 32bf 20cc  .........v..2. .
-000042c0: 839e f5bd 3c7e 9662 af15 0fd9 bfdb e366  ....<~.b.......f
-000042d0: cd4e bca4 3356 bc80 379c c91d 2838 8cec  .N..3V..7...(8..
-000042e0: 33b7 4eec 5003 4d0a 053a b4b1 4ae7 02f9  3.N.P.M..:..J...
-000042f0: 725d d5fe ac4d f040 55e9 0f3c a8f2 22d1  r]...M.@U..<..".
-00004300: 7a14 d209 1d57 9d68 1aae 5fb7 00ec 3b56  z....W.h.._...;V
-00004310: c34f c195 03d8 d5f0 968d d23d 9dc1 2a9d  .O.........=..*.
-00004320: e4ef bc11 a32a cfbb 1eb0 1671 d724 7fc3  .....*.....q.$..
-00004330: 515c 14d3 6906 6742 37fc c09b 6d5c da7d  Q\..i.gB7...m\.}
-00004340: edc5 0404 701b af30 c837 d0bd bf08 8864  ....p..0.7.....d
-00004350: 0590 8010 247d 9161 90ac c023 7dfd 8f79  ....$}.a...#}..y
-00004360: ade8 bc02 4846 b87a 1b5a d1ac 15cd 0abc  ....HF.z.Z......
-00004370: 37a1 adbf 495f 04ab 848b 48b9 2cf3 bc28  7...I_....H.,..(
-00004380: c8f2 6eb7 6f87 b125 6b58 14f8 210c 9211  ..n.o..%kX..!...
-00004390: 2287 f485 defe b6f2 3303 3033 367f 980d  ".......3.036...
-000043a0: b2cb b363 43a6 3c33 a264 ca33 9547 88a8  ...cC.<3.d.3.G..
-000043b0: 2172 ca92 1800 d217 72c8 a690 1385 4110  !r......r.....A.
-000043c0: be70 d408 569e 639f c908 c963 3e03 9525  .p..V.c....c>..%
-000043d0: 09e1 9012 d35b 1454 a10a bc89 7e91 8728  .....[.T....~..(
-000043e0: cfcb 9280 1024 c2c8 7312 c203 3b03 9161  .....$..s...;..a
-000043f0: 6020 2494 e7e1 457a f33e cb4e efb9 6cfa  ` $...Ez.>.N..l.
-00004400: 83bd f90d 504b 0304 1400 0000 0800 f00b  ....PK..........
-00004410: b158 b747 eb8a c000 0000 1602 0000 0b00  .X.G............
-00004420: 0000 5f72 656c 732f 2e72 656c 739d 924b  .._rels/.rels..K
-00004430: 6e02 310c 40af 1265 5f4c a9c4 0231 acd8  n.1.@..e_L...1..
-00004440: b043 880b b889 e7a3 99c4 9163 c4f4 f68d  .C.........c....
-00004450: d8c0 2068 114b ff9e 9e2d af0f 34a0 761c  .. h.K...-..4.v.
-00004460: 73db a56c c630 c45c d956 35ad 00b2 6b29  s..l.0.\.V5...k)
-00004470: 609e 71a2 582a 354b 402d a134 90d0 f5d8  `.q.X*5K@-.4....
-00004480: 102c e6f3 25c8 2dc3 6ed6 b74c 73fc 49f4  .,..%.-.n..Ls.I.
-00004490: 0a91 ebba 73b4 6577 0a14 f501 f8ae c39a  ....s.ew........
-000044a0: 234a 435a d971 8033 4bff cddc cf0a d49a  #JCZ.q.3K.......
-000044b0: 9daf acec fca7 35f0 a6cc f3f5 2090 a247  ......5..... ..G
-000044c0: 4570 2cf4 91a4 4c8b 7694 af3e 9edd bea4  Ep,...L.v..>....
-000044d0: f3a5 6362 b478 dfe8 fff3 d0a8 143d f9bf  ..cb.x.......=..
-000044e0: 9d30 a589 d2d7 4509 266f b0f9 0550 4b03  .0....E.&o...PK.
-000044f0: 0414 0000 0008 00f0 0bb1 58f6 7501 aa30  ..........X.u..0
-00004500: 0100 0029 0200 000f 0000 0078 6c2f 776f  ...).......xl/wo
-00004510: 726b 626f 6f6b 2e78 6d6c 8d90 d14e c330  rkbook.xml...N.0
-00004520: 0c45 7fa5 ca07 d06e 8249 4ceb 5e98 8049  .E.....n.IL.^..I
-00004530: 0810 437b cf5a 77b5 96c4 95e3 6eb0 af27  ..C{.Zw.....n..'
-00004540: 4929 4ce2 8527 c7d7 d6c9 bd5e 9c88 0f3b  I)L..'.....^...;
-00004550: a243 f661 8df3 732e 552b d2cd f3dc 572d  .C.a..s.U+....W-
-00004560: 58ed afa8 0317 660d b1d5 125a dee7 d434  X.....f....Z...4
-00004570: 58c1 8aaa de82 937c 5a14 b39c c168 4172  X......|Z....hAr
-00004580: bec5 ceab 81f6 1f96 ef18 74ed 5b00 b166  ..........t.[..f
-00004590: 4059 8d4e 2d17 a3b3 57ce f2cb 8e04 aaf8  @Y.N-...W.......
-000045a0: 5354 a3b2 4538 f9df 85d8 6647 f4b8 4383  ST..E8....fG..C.
-000045b0: f259 aaf4 36a0 328b 0e2d 9ea1 2e55 a132  .Y..6.2..-...U.2
-000045c0: dfd2 e991 18cf e444 9b4d c564 4ca9 26c3  .......D.M.dL.&.
-000045d0: 600b 2c58 fd91 37d1 e6bb def9 a488 debd  `.,X..7.........
-000045e0: c5cc a59a 1501 d820 7b49 1b89 af83 c923  ....... {I.....#
-000045f0: 84e5 a1eb 85ee d108 f04a 0b3c 30f5 1dba  .........J.<0...
-00004600: 7dc2 8418 f945 8e74 8ab1 664e 5b28 55a2  }....E.t..fN[(U.
-00004610: 260f a1ae ebc1 8f04 d045 3a9e 6318 f0ba  &........E:.c...
-00004620: fe46 8e9c 1a1a 7450 3f07 908f 8390 aa0a  .F....tP?.......
-00004630: 278d 2591 a6d7 3793 dbe0 be37 e62e 682f  '.%...7....7..h/
-00004640: ee89 74fd 636c bcea f20b 504b 0304 1400  ..t.cl....PK....
-00004650: 0000 0800 f00b b158 33eb e3ba ad00 0000  .......X3.......
-00004660: fb01 0000 1a00 0000 786c 2f5f 7265 6c73  ........xl/_rels
-00004670: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
-00004680: 6c73 b591 3d0e 8330 0c85 af12 e500 18a8  ls..=..0........
-00004690: d4a1 02a6 2eac 1517 8882 f911 8144 b1ab  .............D..
-000046a0: c2ed 1bc1 0048 1dba 3059 cf96 bff7 6467  .....H..0Y....dg
-000046b0: 2f34 8a7b 3b51 d73b 12f3 6826 ca65 c7ec  /4.{;Q.;..h&.e..
-000046c0: 1e00 a43b 1c15 45d6 e114 268d f5a3 e220  ...;..E...&.... 
-000046d0: 7d0b 4ee9 41b5 0869 1cdf c11f 19b2 c88e  }.N.A..i........
-000046e0: 4c51 2d0e ff21 daa6 e935 3ead 7e8f 38f1  LQ-..!...5>.~.8.
-000046f0: 0f30 7cac 1fa8 4364 292a e55b e45c c26c  .0|...Cd)*.[.\.l
-00004700: f636 c15a 9228 90a5 28eb 5cfa b24e a480  .6.Z.(..(.\..N..
-00004710: cb12 112f 0669 8fb3 e993 7f7a a53f 875d  .../.i.....z.?.]
-00004720: dced 57b9 35cf 47b8 ad21 e0f4 ebe2 0b50  ..W.5.G..!.....P
-00004730: 4b03 0414 0000 0008 00f0 0bb1 589b 8642  K...........X..B
-00004740: 841b 0100 00d7 0300 0013 0000 005b 436f  .............[Co
-00004750: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-00004760: ad93 cf4e c330 0cc6 5fa5 ea75 6a33 3870  ...N.0.._..uj38p
-00004770: 40eb 2e8c 2bec c00b 84c4 5da3 e69f 626f  @...+.....]...bo
-00004780: 746f 8fdb b24a a0b1 0d95 4ba3 c6f6 f773  to...J....K....s
-00004790: fc25 abb7 6304 cc3a 673d 5679 4314 1f85  .%..c..:g=VyC...
-000047a0: 40d5 8093 5886 089e 2375 484e 12ff a69d  @...X...#uHN....
-000047b0: 8852 b572 07e2 7eb9 7c10 2a78 024f 05f5  .R.r..~.|.*x.O..
-000047c0: 1af9 7ab5 815a ee2d 65cf 1d6f a309 beca  ..z..Z.-e..o....
-000047d0: 1358 ccb3 a731 b167 55b9 8cd1 1a25 89e3  .X...1.gU....%..
-000047e0: e2e0 f50f 4af1 4528 b972 c8c1 c644 5c70  ....J.E(.r...D\p
-000047f0: 429e 89b3 8821 f42b e154 f87a 8094 8c86  B....!.+.T.z....
-00004800: 6c2b 13bd 48c7 69a2 b302 e968 01cb cb1a  l+..H.i....h....
-00004810: 67ba 0c75 6d14 e8a0 f68e 4b4a 8c09 a4c6  g..um.....KJ....
-00004820: 0680 9c2d 47d1 c515 34f1 9061 fcde cd6e  ...-G...4..a...n
-00004830: 6090 b948 e4d4 6d0a 11d9 b504 7fe7 9d6c  `..H..m........l
-00004840: e9ab 8bc8 4290 c85c 39e4 8464 edd9 2784  ....B..\9..d..'.
-00004850: de71 0dfa 5638 4ff8 23a4 76f0 04c5 b0cc  .q..V8O.#.v.....
-00004860: 1ff3 779f 27fd 5b1a 790f a1fd ef7b d6af  ..w.'.[.y....{..
-00004870: a593 c64f 0d88 e13d af3f 0150 4b01 0214  ...O...=.?.PK...
-00004880: 0314 0000 0008 00f0 0bb1 5846 5ac1 0c82  ..........XFZ...
-00004890: 0000 00b1 0000 0010 0000 0000 0000 0000  ................
-000048a0: 0000 0080 0100 0000 0064 6f63 5072 6f70  .........docProp
-000048b0: 732f 6170 702e 786d 6c50 4b01 0214 0314  s/app.xmlPK.....
-000048c0: 0000 0008 00f0 0bb1 58e3 e822 2fea 0000  ........X.."/...
-000048d0: 00cb 0100 0011 0000 0000 0000 0000 0000  ................
-000048e0: 0080 01b0 0000 0064 6f63 5072 6f70 732f  .......docProps/
-000048f0: 636f 7265 2e78 6d6c 504b 0102 1403 1400  core.xmlPK......
-00004900: 0000 0800 f00b b158 995c 9c23 1006 0000  .......X.\.#....
-00004910: 9c27 0000 1300 0000 0000 0000 0000 0000  .'..............
-00004920: 8001 c901 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
-00004930: 6865 6d65 312e 786d 6c50 4b01 0214 0314  heme1.xmlPK.....
-00004940: 0000 0008 00f0 0bb1 5888 89ce 2ff2 3800  ........X.../.8.
-00004950: 00f0 f201 0018 0000 0000 0000 0000 0000  ................
-00004960: 0080 810a 0800 0078 6c2f 776f 726b 7368  .......xl/worksh
-00004970: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
-00004980: 4b01 0214 0314 0000 0008 00f0 0bb1 58f7  K.............X.
-00004990: f68f 09a7 0200 006d 0b00 000d 0000 0000  .......m........
-000049a0: 0000 0000 0000 0080 0132 4100 0078 6c2f  .........2A..xl/
-000049b0: 7374 796c 6573 2e78 6d6c 504b 0102 1403  styles.xmlPK....
-000049c0: 1400 0000 0800 f00b b158 b747 eb8a c000  .........X.G....
-000049d0: 0000 1602 0000 0b00 0000 0000 0000 0000  ................
-000049e0: 0000 8001 0444 0000 5f72 656c 732f 2e72  .....D.._rels/.r
-000049f0: 656c 7350 4b01 0214 0314 0000 0008 00f0  elsPK...........
-00004a00: 0bb1 58f6 7501 aa30 0100 0029 0200 000f  ..X.u..0...)....
-00004a10: 0000 0000 0000 0000 0000 0080 01ed 4400  ..............D.
-00004a20: 0078 6c2f 776f 726b 626f 6f6b 2e78 6d6c  .xl/workbook.xml
-00004a30: 504b 0102 1403 1400 0000 0800 f00b b158  PK.............X
-00004a40: 33eb e3ba ad00 0000 fb01 0000 1a00 0000  3...............
-00004a50: 0000 0000 0000 0000 8001 4a46 0000 786c  ..........JF..xl
-00004a60: 2f5f 7265 6c73 2f77 6f72 6b62 6f6f 6b2e  /_rels/workbook.
-00004a70: 786d 6c2e 7265 6c73 504b 0102 1403 1400  xml.relsPK......
-00004a80: 0000 0800 f00b b158 9b86 4284 1b01 0000  .......X..B.....
-00004a90: d703 0000 1300 0000 0000 0000 0000 0000  ................
-00004aa0: 8001 2f47 0000 5b43 6f6e 7465 6e74 5f54  ../G..[Content_T
-00004ab0: 7970 6573 5d2e 786d 6c50 4b05 0600 0000  ypes].xmlPK.....
-00004ac0: 0009 0009 003e 0200 007b 4800 0000 00    .....>...{H....
+000000e0: 914d 4fc3 300c 86ff ca94 7beb b4dd f888  .MO.0.....{.....
+000000f0: ba5e 9838 8184 c424 10b7 28f1 b68a e643  .^.8...$..(....C
+00000100: 8951 bb7f 4f5a b60e 0437 8ef1 fbf8 b1ad  .Q..OZ...7......
+00000110: d4ca 0be5 023e 05e7 3150 8b71 3198 ce46  .....>..1P.q1..F
+00000120: a1fc 9a1d 88bc 0088 ea80 46c6 3c11 3685  ..........F.<.6.
+00000130: 3b17 8ca4 f40c 7bf0 52bd cb3d 42c9 f915  ;.....{.R..=B...
+00000140: 1824 a925 4918 8599 9f8d eca4 d46a 56fa  .$.%I........jV.
+00000150: 8fd0 4d02 ad00 3b34 6829 4291 1770 6109  ..M...;4h)B..pa.
+00000160: 8389 7f36 4cc9 4c0e b19d a9be eff3 be9a  ...6L.L.........
+00000170: b8b4 5101 af8f 0fcf d3f2 596b 2349 ab90  ..Q.......Yk#I..
+00000180: 35b5 5642 0594 e442 335e e48f 4357 c3b7  5.VB...B3^..CW..
+00000190: 627d 9afd 5540 bd48 1304 1d3d aed9 3979  b}..U@.H...=..9y
+000001a0: a9ee 36db 7bd6 94bc 5c66 7c95 f1eb 2dbf  ..6.{...\f|...-.
+000001b0: 11d5 ade0 abb7 d1f5 a3ff 2234 4eb7 bbf6  .........."4N...
+000001c0: 1fc6 b3a0 a9e1 d7bf 359f 504b 0304 1400  ........5.PK....
+000001d0: 0000 0800 e254 a758 995c 9c23 1006 0000  .....T.X.\.#....
+000001e0: 9c27 0000 1300 0000 786c 2f74 6865 6d65  .'......xl/theme
+000001f0: 2f74 6865 6d65 312e 786d 6ced 5a5b 73da  /theme1.xml.Z[s.
+00000200: 3814 7eef afd0 7867 f66d 0bc6 3681 b6b4  8.~...xg.m..6...
+00000210: 1373 6976 dbb4 9984 ed4e 1f85 1158 8d6c  .siv.....N...X.l
+00000220: 7964 9184 7fbf 4736 10cb 960d ed92 4dba  yd....G6......M.
+00000230: 9b3c 042c e9fb ce45 47e7 e838 79f3 ee2e  .<.,...EG..8y...
+00000240: 62e8 8688 94f2 7860 d92f dbd6 bbb7 2fde  b.....x`./..../.
+00000250: e057 3224 1141 3019 a7af f0c0 0aa5 4c5e  .W2$.A0.......L^
+00000260: b55a 6900 c338 7dc9 1312 c3dc 828b 084b  .Zi..8}........K
+00000270: 7814 cbd6 5ce0 5b1a 2f23 d6ea b4db dd56  x...\.[./#.....V
+00000280: 8469 6ca1 1847 6460 7d5e 2c68 40d0 5451  .il..Gd`}^,h@.TQ
+00000290: 5a6f 5f20 b4e5 1f33 f815 cb54 8d65 a301  Zo_ ...3...T.e..
+000002a0: 1357 4126 b988 b4f2 f96c c5fc dade 3e65  .WA&.....l....>e
+000002b0: cfe9 3a1d 3281 6e30 1b58 207f ce6f a7e4  ..:.2.n0.X ..o..
+000002c0: 4e5a 88e1 54c2 c4c0 6a67 3f56 6bc7 d1d2  NZ..T...jg?Vk...
+000002d0: 4880 82c9 7d94 05ba 49f6 a3d3 1508 320d  H...}...I.....2.
+000002e0: 3b3a 9d58 ce76 7cf6 c4ed 9f8c cada 7434  ;:.X.v|.......t4
+000002f0: 6d1a e0e3 f178 38b6 cbd2 8b70 1c04 e051  m....x8....p...Q
+00000300: bb9e c29d f46c bfa4 4109 b4a3 69d0 64d8  .....l..A...i.d.
+00000310: f6da ae91 a6aa 8d53 4fd3 f77d dfeb 9b68  .......SO..}...h
+00000320: 9c0a 8d5b 4fd3 6b77 ddd3 8e89 c6ad d078  ...[O.kw.......x
+00000330: 0dbe f14f 87c3 ae89 c6ab d074 eb69 2627  ...O.......t.i&'
+00000340: fdae 6ba4 e916 6842 46e3 eb7a 1215 b5e5  ..k...hBF..z....
+00000350: 40d3 2000 5870 76d6 ccd2 0396 5e29 fa75  @. .Xpv.....^).u
+00000360: 941a d91d bbdd 415c f058 ee39 8911 fec6  ......A\.X.9....
+00000370: c504 d669 d219 9634 4672 9d90 050e 0037  ...i...4Fr.....7
+00000380: c4d1 4c50 7caf 41b6 8ae0 c292 d25c 90d6  ..LP|.A......\..
+00000390: cf29 b550 1a08 9ac8 81f5 4782 21c5 dcaf  .).P......G.!...
+000003a0: fdf5 97bb c9a4 337a 9d7d 3ace 6b94 7f69  ......3z.}:.k..i
+000003b0: ab01 a7ed bb9b cf93 fc73 e8e4 9fa7 93d7  .........s......
+000003c0: 4d42 ce70 bc2c 09f1 fb23 5b61 8727 6e3b  MB.p.,...#[a.'n;
+000003d0: 1372 3a1c 6742 7ccf f6f6 91a5 2532 cfef  .r:.gB|.....%2..
+000003e0: f90a eb4e 3c67 1f56 96b0 5dcf cfe4 9e8c  ...N<g.V..].....
+000003f0: 7223 bbdd f658 7df6 4f47 6e23 d7a9 c0b3  r#...X}.OGn#....
+00000400: 22d7 9446 2445 9fc8 2dba e411 38b5 490d  "..F$E..-...8.I.
+00000410: 3213 3f08 9d86 986a 501c 02a4 0931 96a1  2.?....jP....1..
+00000420: 86f8 b4c6 ac11 e013 7db7 be08 c8df 8d88  ........}.......
+00000430: f7ab 6f9a 3d57 a158 49da 84f8 1046 1ae2  ..o.=W.XI....F..
+00000440: 9c73 e673 d16c fb07 a546 d1f6 55bc dca3  .s.s.l...F..U...
+00000450: 9758 1501 9718 df34 aa35 2cc5 d678 95c0  .X.....4.5,..x..
+00000460: f1ad 9c3c 1d13 12cd 940b 0641 8697 2426  ...<.......A..$&
+00000470: 12a9 397e 4d48 13fe 2ba5 dafe 9cd3 40f0  ..9~MH..+.....@.
+00000480: 942f 24fa 4a91 8f69 b323 a774 26cd e833  ./$.J..i.#.t&..3
+00000490: 1ac1 46af 1b75 8768 d23c 7afe 05f9 9c35  ..F..u.h.<z....5
+000004a0: 0a1c 911b 1d02 671b b346 2184 69bb f01e  ......g..F!.i...
+000004b0: af24 8e9a adc2 112b 423e 6219 361a 72b5  .$.....+B>b.6.r.
+000004c0: 1681 b671 a984 605a 12c6 d178 4ed2 b411  ...q..`Z...xN...
+000004d0: fc59 ac35 933e 60c8 eccd 9175 ced6 910e  .Y.5.>`....u....
+000004e0: 1192 5e37 423e 62ce 8b90 11bf 1e86 384a  ..^7B>b.......8J
+000004f0: 9aed a271 5804 fd9e 5ec3 49c1 e882 cb66  ...qX...^.I....f
+00000500: fdb8 7e86 d533 6c2c 8ef7 47d4 174a e40f  ..~..3l,..G..J..
+00000510: 26a7 3fe9 3234 07a3 9a59 09bd 8456 6a9f  &.?.24...Y...Vj.
+00000520: aa87 343e a81e 320a 05f1 b91e 3ee5 7a78  ..4>..2.....>.zx
+00000530: 0a37 96c6 bc50 ae82 7b01 ffd1 da37 c2ab  .7...P..{....7..
+00000540: f882 c039 7f2e 7dcf a5ef b9f4 3da1 d2b7  ...9..}.....=...
+00000550: 3723 7d67 c1d3 8b5b de46 6e5b c4fb ae31  7#}g...[.Fn[...1
+00000560: dad7 342e 2863 5772 cdc8 c754 af93 29d8  ..4.(cWr...T..).
+00000570: 399f c0ec fd68 3e9e f1ed fad9 2484 af9a  9....h>.....$...
+00000580: 592d 2316 904b 81b3 4124 b8fc 8bca f02a  Y-#..K..A$.....*
+00000590: c409 e864 5b25 09cb 54d3 6537 8a12 9e42  ...d[%..T.e7...B
+000005a0: 1b6e e953 f54a 95d7 e5af b928 b83c 5be4  .n.S.J.....(.<[.
+000005b0: e9af a174 3e2c cff9 3c5f e7b4 cd0b 3343  ...t>,..<_....3C
+000005c0: b772 4bea b694 beb5 2638 4af4 b1cc 704e  .rK.....&8J...pN
+000005d0: 1ecb 0c3b 673c 921d b677 a01d 35fb f65d  ...;g<...w..5..]
+000005e0: 76e4 23a5 3053 9743 b81a 42be 036d ba9d  v.#.0S.C..B..m..
+000005f0: dc3a 389e 9891 b90a d352 906f c3f9 e9c5  .:8......R.o....
+00000600: 781a e239 d904 b97d 9857 6de7 d8d1 d1fb  x..9...}.Wm.....
+00000610: e7c1 51b0 a3ef 3c96 1dc7 88f2 a221 eea1  ..Q...<......!..
+00000620: 8698 cfc3 4387 797b 5f98 6795 c650 3414  ....C.y{_.g..P4.
+00000630: 6d6c ac24 2c46 b760 b8d7 f12c 14e0 6460  ml.$,F.`...,..d`
+00000640: 2da0 0783 af51 02f2 5255 6031 5bc6 032b  -....Q..RU`1[..+
+00000650: 90a2 7c4c 8c45 e870 e797 5c5f e3d1 92e3  ..|L.E.p..\_....
+00000660: dba6 65b5 6eaf 2977 196d 2252 39c2 6998  ..e.n.)w.m"R9.i.
+00000670: 1367 abca de65 b1c1 551d cf55 5bf2 b0be  .g...e..U..U[...
+00000680: 6a3d b415 4ecf fe59 adc8 9f0c 114e 160b  j=..N..Y.....N..
+00000690: 1248 6394 17a6 4aa2 f319 53be e72b 49c4  .Hc...J...S..+I.
+000006a0: 5538 bf45 33b6 1297 18bc e3e6 c771 4e53  U8.E3........qNS
+000006b0: b812 76b6 0f02 32b9 bb39 a97a 6531 67a6  ..v...2..9.ze1g.
+000006c0: f2df 2d0c 092c 5b88 5912 e24d 5ded d5e7  ..-..,[.Y..M]...
+000006d0: 9b9c ae7a 2276 fa97 77c1 60f2 fd70 c947  ...z"v..w.`..p.G
+000006e0: 0fe5 3be7 5ff4 5d43 ae7e f6dd e3fa 6e93  ..;._.]C.~....n.
+000006f0: 3b48 4c9c 79c5 1101 7445 0223 951c 0616  ;HL.y...tE.#....
+00000700: 1732 e450 ee92 9006 1301 cd94 c944 f002  .2.P.........D..
+00000710: 8264 a61c 8098 fa0b bdf2 0cb9 2915 cead  .d..........)...
+00000720: 3e39 7f45 2c83 864e 5ed2 2512 148a b00c  >9.E,..N^.%.....
+00000730: 0521 1772 e3ef ef93 6a77 8cd7 fa2c 816d  .!.r....jw...,.m
+00000740: 8454 3264 d517 ca43 89c1 3d33 7243 d854  .T2d...C..=3rC.T
+00000750: 25f3 aeda 260b 85db e254 cdbb 1abe 2660  %...&....T....&`
+00000760: 4bc3 7a6e 9d2d 27ff db5e d43d b417 3d46  K.zn.-'..^.=..=F
+00000770: f3a3 99e0 1eb3 8773 9b7a b8c2 45ac ff58  .......s.z..E..X
+00000780: d61e f932 df39 70db 3ade 035e e613 2c43  ...2.9p.:..^..,C
+00000790: a47e c17d 8a8a 8011 ab62 beba af4f f925  .~.}.....b...O.%
+000007a0: 9c3b b47b f181 209b fcd6 dba4 f6dd e00c  .;.{.. .........
+000007b0: 7cd4 ab5a a564 2b11 3f4b 077c 1f92 0663  |..Z.d+.?K.|...c
+000007c0: 8c5b f434 5f8f 1462 ada6 b1ad c6da 310c  .[.4_..b......1.
+000007d0: 7980 58f3 0ca1 6638 df87 459a 1a33 d58b  y.X...f8..E..3..
+000007e0: ac39 8d0a 6f41 d540 e53f dbd4 0d68 f60d  .9..oA.@.?...h..
+000007f0: 341c 9105 5e31 99b6 36a3 e44e 0a3c dcfe  4...^1..6..N.<..
+00000800: ef0d b0c2 c48e e1ed 8bbf 0150 4b03 0414  ...........PK...
+00000810: 0000 0008 00e2 54a7 5888 89ce 2ff2 3800  ......T.X.../.8.
+00000820: 00f0 f201 0018 0000 0078 6c2f 776f 726b  .........xl/work
+00000830: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
+00000840: 6c9d 9d5b 8fe6 467a a4ff 8aa0 fb76 17f3  l..[..Fz.....v..
+00000850: 44d2 d008 d8b1 b1d8 bdd8 85e1 81bd d755  D..............U
+00000860: 5f95 5aed e956 cba5 1e6b f7df 2f49 7715  _.Z..V...k../Iw.
+00000870: a398 ef13 29f8 6ad4 c32f 328a 878c 3cf0  ....).j../2...<.
+00000880: 61e6 0fbf 7f79 feeb 6f3f 3f3d 7dfd eeff  a....y..o??=}...
+00000890: 7efe f4cb 6f7f fafe e7af 5f7f fdfb f7ef  ~...o....._.....
+000008a0: 7fbb fdfc f4f9 feb7 bffb f2eb d32f db91  ............./..
+000008b0: 9fbe 3c7f beff bafd f3f9 c3fb df7e 7d7e  ..<..........~}~
+000008c0: ba7f 3c44 9f3f bd4f 7777 edfd e7fb 8fbf  ..<D.?.Oww......
+000008d0: 7cff e30f c7ff f74f cf3f fef0 e56f 5f3f  |......O.?...o_?
+000008e0: 7dfc e5e9 9f9e bffb ed6f 9f3f df3f ffbf  }........o.?.?..
+000008f0: 3f3f 7dfa f2fb 9fbe 9fbe 7ff9 3ffe f9e3  ??}.........?...
+00000900: 879f bf1e ffc7 fb1f 7ff8 f5fe c3d3 5f9e  .............._.
+00000910: befe cbaf 9b60 fbe7 fbd7 721e 3f7e 7efa  .....`....r.?~~.
+00000920: e5b7 8f5f 7ef9 eef9 e9a7 3f7d ffdf a6bf  ..._~.....?}....
+00000930: fff3 34e5 7c88 8e1f fdeb c7a7 df7f 93ff  ..4.|...........
+00000940: fe6e 3f9f 872f 5ffe baff e37f 3efe e9fb  .n?../_.....>...
+00000950: bbfd cf7a faf4 74fb ba97 72bf fdcf 7f3c  ...z..t...r....<
+00000960: fdc3 d3a7 4f7b 61db 1ff3 efdf cafd fef4  ....O{a.........
+00000970: dd95 fadf 2fc5 fff7 e312 6c7f e1c3 fd6f  ..../.....l....o
+00000980: 4fff f0e5 d3ff f9f8 f8f5 e73f 7dbf 7cff  O..........?}.|.
+00000990: dde3 d34f f77f fbf4 f59f bffc fe3f 9ebe  ...O.........?..
+000009a0: 9d56 3dff c47f bcff 7aff e30f cf5f 7eff  .V=.....z...._~.
+000009b0: ee79 3fdf 1f7f b8ed ff71 b81f e7bf fdfc  .y?......q......
+000009c0: e32f fbd5 facb d7e7 ede8 c7cd efeb 8fff  ./..............
+000009d0: fa1f fffb 87f7 5fb7 3f63 ffe7 fbdb 37d1  ......_.?c....7.
+000009e0: 9fbd e82f 7ffe f35b d1fb cdf5 d53a bd5a  .../...[.....:.Z
+000009f0: 27d0 4fe5 f9c3 7417 f9b2 e2dd 2763 995f  '.O...t.....'c._
+00000a00: 2df3 a580 fdea fc67 d1d7 232f 45cf efee  -......g..#/E...
+00000a10: 4dc9 e5b5 e482 255f 8fbc 94bc 3cbc 7b30  M.....%_....<.{0
+00000a20: 45d7 d7a2 2b16 7d3d f27a 3da6 f737 5374  E...+.}=.z=..7St
+00000a30: 7b2d ba61 d1d7 2367 d1f7 f6cf 9e5f cb9e  {-.a..#g....._..
+00000a40: b1ec eb91 f336 beff c914 bdbc 16bd 60d1  .....6........`.
+00000a50: d723 af45 afef 5cd1 eb6b d12b 167d 3d22  .#.E..\..k.+.}="
+00000a60: 45ff 6c8a 9eee ceba 7687 8577 875e 4a4f  E.l.....v..w.^JO
+00000a70: 77f7 93bb 9793 54e5 6b85 94e2 a9ae e67c  w.....T.k......|
+00000a80: 3fbb d2cf da3a 5d2b 9f94 cef5 f2bd ab3d  ?....:]+.......=
+00000a90: d359 3127 ae99 dda1 d7d2 9b7d 5ca6 b372  .Y1'.......}\..r
+00000aa0: 4e5c 3bbb 43af 57c6 d7fc e9ac 9f13 57d0  N\;.C.W.......W.
+00000ab0: eed0 4be9 e5ee fedd a32b feac a313 57d2  ..K......+....W.
+00000ac0: eed0 6bf1 d3fd 7b57 4ba7 b39a 4e5c 4fbb  ..k...{WK...N\O.
+00000ad0: 43af c5a7 774f aef4 b3a6 4e5c 55bb 43af  C...wO....N\U.C.
+00000ae0: a5e7 77f6 893f 2beb c4b5 b53b 24a5 bbbf  ..w..?+....;$...
+00000af0: 3d9d d535 7175 ed0e 49e9 ee99 4c67 6d4d  =..5qu..I...LgmM
+00000b00: 5c5b bb43 d2ce 7d76 a54b dbca b5b5 3bf4  \[.C..}v.K....;.
+00000b10: 5a7a b58f 643a 6b6b c22a 19b6 da51 dd7e  Zz..d:kk.*...Q.~
+00000b20: 5bf4 5955 13d5 c7e9 3e2c 3baa d96f cb3e  [.YU....>,;..o.>
+00000b30: 2b6a c2f6 f23e 2e3c aad8 6f0b 3fab 69c2  +j...>.<..o.?.i.
+00000b40: 16f3 fe3e be2c 2c98 dc6d 38ab 6ec2 8674  ...>.,,..m8.n..t
+00000b50: b38c cf88 15d6 f3ac d009 5bd8 cdf3 21f4  ..........[...!.
+00000b60: 6485 f53c ab79 c2a6 f7fe 3e85 962c 48ae  d..<.y....>..,H.
+00000b70: 9f78 d6fd 4c15 7cb7 0c2f ad51 58cf 3311  .x..L.|../.QX.3.
+00000b80: 3256 fbcd 33bc b446 613d cf9c c818 06f7  2V..3..Fa=......
+00000b90: b163 942b 6f0b 97de 36c6 c4fd 4358 2558  .c.+o...6...CX%X
+00000ba0: 70fd fd5b cb33 3e32 c7c7 435c 2558 d109  p..[.3>2..C\%X..
+00000bb0: de9a 9eb9 9239 571e e23a c18a 81e9 9937  .....9W..:.....7
+00000bc0: 19e3 e3f9 4358 2958 d0fd 916f 3dcf c0c9  ....CX)X...o=...
+00000bd0: 181f db88 2df4 4481 ed5c e533 6f32 7720  ....-.D..\.3o2w 
+00000be0: c243 6fcb 3933 2453 2440 6d8e 7a16 6f87  .Co.93$S$@m.z.o.
+00000bf0: 7e67 5814 ecbc c7ed 4af7 fbbe f033 150a  ~gX.....J....3..
+00000c00: d5f1 04ed 8a11 b84a 54ce 5028 140a 09f2  .......JT.P(....
+00000c10: d608 5c0e 9533 2a0a d5fc 1cfa 0d7b 1445  ..\..3*......{.E
+00000c20: 46e6 d8c3 8f6f ceb0 4751 ce9a 5fa8 1e67  F....o..GQ.._..g
+00000c30: b8f3 c31e 4539 6b78 a10a 9be9 ceb3 c0de  ....E9kx........
+00000c40: f9b3 8217 aaaf 99ee 3c0b ec9d 3f2b 78c1  ........<...?+x.
+00000c50: 6140 e837 acf3 e5ac f305 c700 f1cd 19d6  a@.7............
+00000c60: f97a d6f9 8a23 80f8 ce77 bfef 0b3f eb7c  .z...#...w...?.|
+00000c70: a52a 5ce0 ce1b 81bb f3f5 acf3 95aa 7009  .*\...........p.
+00000c80: 1bb0 eee7 fde9 9c95 bb52 e52e 0ff1 b51a  .........R......
+00000c90: 56ef 7a56 ef4a d57b 2b3c be56 2cb0 d74a  V.zV.J.{+<.V,..J
+00000ca0: 26e4 7054 ff10 d712 2370 b5a4 9e59 5071  &.pT....#p...YPq
+00000cb0: a4ff 701f 46a4 1164 6779 6641 c5d1 ff43  ..p.F..dgyfA...C
+00000cc0: fc48 4413 096f 0b3f 6b7d c55a ff10 770d  .HD..o.?k}.Z..w.
+00000cd0: 5970 b377 ed4c 838a 69f0 70bd 0bdf 2c51  Yp.w.L..i.p...,Q
+00000ce0: 7073 77ad 9d21 d130 241e ae77 e1db ac2b  psw..!.0$..w...+
+00000cf0: 0a6e eeae b533 3a1a 26c1 2d34 8c66 21de  .n...3:.&.-4.f!.
+00000d00: 967d 6644 c38c b885 f5b8 fb7d 5ff8 1912  .}fD.......}_...
+00000d10: 0d43 e216 d763 163c ba27 a29d d1d1 3009  .C...c.<.'....0.
+00000d20: c812 058f b6db dece ec68 1805 e489 8247  .........h.....G
+00000d30: db6d 6f32 cb8f 5900 dd76 16d8 6e7b 3bc3  .mo2..Y..v..n{;.
+00000d40: a3f1 ac62 77e8 6cab 7ce9 677a 340a 831a  ...bw.l.|.gz4...
+00000d50: 9ecd b0cf d0ce 9468 54e9 6bfc 880f fb0c  .......hT.k.....
+00000d60: f319 0733 d5ee 1af7 19ba dff7 859f 157f  ...3............
+00000d70: a68a 5fa1 cf60 04ae fecc 671e cc94 0715  .._..`....g.....
+00000d80: 7a8b 46e0 1275 3e53 62a6 4abf 5986 896a  z.F..u>Sb.J.Y..j
+00000d90: 042e 51e7 3325 66aa f4bb 657c df58 7115  ..Q.3%f...e|.Xq.
+00000da0: bc35 3d63 62a6 5abf 9b86 cdaf 515c 056f  .5=cb.Z.....Q\.o
+00000db0: 4dcf 9c98 a9da d7d8 317a 31f1 b66c 791b  M.......1z1..ly.
+00000dc0: 48b5 bec6 7dc0 eef7 7de1 671e cc98 07d0  H...}...}.g.....
+00000dd0: 0734 02fb ec9f 3931 634e 9025 0b6c dbb1  .4....91cN.%.l..
+00000de0: 9cf9 b160 7e80 a711 d8b6 6339 6365 c194  ...`~.....c9ce..
+00000df0: 80be ae11 b83a be9c b1b2 604a 9025 0bae  .....:....`J.%..
+00000e00: b33b 6f3d cf5c 5930 26c8 9305 d7b9 dab7  .;o=.\Y0&.......
+00000e10: 9e67 b02c 1813 d0a7 3702 9765 cb19 2b0b  .g.,....7..e..+.
+00000e20: 8604 59b2 c046 d972 a6ca c2a9 029e 2cb0  ..Y..F.r......,.
+00000e30: 49b6 9c69 b398 b409 e715 8ca0 384b 6112  I..i........8Ka.
+00000e40: 3852 c2f4 ec7e df05 dc72 a6cd c2e1 110f  8R...~...r......
+00000e50: 9758 6087 4beb 1936 2b67 473c 5c62 811d  .X`.K..6+gG<\b..
+00000e60: 2ead 67d6 ac1c 1de1 e0a5 fb7d 7709 d733  ..g........}w..3
+00000e70: 5556 0e89 eb25 f956 3a0a ecf8 623d 4365  UV...%.V:...b=Ce
+00000e80: e58c b85e 926f 9628 78b4 97f0 cc94 9523  ...^.o.(x......#
+00000e90: e23a 82fc 6689 8247 9729 eb99 292b 47c4  .:..f..G.)..)+G.
+00000ea0: 2dac 6b2c 7874 756d 3d23 65e5 84b8 8543  -.k,xtum=#e....C
+00000eb0: 0016 3c56 6779 26ca ca01 0196 2878 bc0e  ..<Vgy&.....(x..
+00000ec0: 25de 7a9e 91b2 72a4 8027 0a1e af5d b8b7  %.z...r..'...]..
+00000ed0: 9ec2 3f71 7084 8ec3 f1cf 74a7 0014 6744  ..?qp.....t...gD
+00000ee0: d80b ec05 41f9 4240 dd61 82c0 e8da 289e  ....A.B@.a....(.
+00000ef0: 5c2d 9fee 92b8 6252 dce2 ce83 513c b98a  \-....bR....Q<..
+00000f00: 3edd 0931 7587 6171 8bdb 55a3 7872 757d  >..1u.aq..U.xru}
+00000f10: ba13 92ea 0ef3 e216 b7ac 46f1 e4aa fb74  ..........F....t
+00000f20: 2784 d51d 46c6 f307 3857 1e0e 79ae eb4e  '...F...8W..y..N
+00000f30: c8ab 3b83 5e75 c75e 0dde 7db0 e50b 7a75  ..;.^u.^..}...zu
+00000f40: 67d8 abee d8f9 ead4 925d 7702 5fdd 611e  g........]w._.a.
+00000f50: 3c7f 0803 c428 1e07 974d a8ac 3bcc 90e7  <....(...M..;...
+00000f60: 0f2d b645 8547 c114 ae44 8472 739d 4357  .-.E.G...D.rs.CW
+00000f70: 563c fa6b fc06 bac4 0079 fe10 5708 5678  V<.k.....y..W.Vx
+00000f80: 2450 614c 4763 228e 599f fc3d 541e d301  $PaLGc".Y..=T...
+00000f90: 9948 646e d7cd df2e 0912 042f 2b4c 4a1a  .Hdn......./+LJ.
+00000fa0: 8565 ee26 4535 11c8 ac40 4d18 c5e0 1991  .e.&E5...@M.....
+00000fb0: 1c41 4e73 735d 6257 4e17 4b5e 2ad8 e9c8  .ANss]bWN.K^*...
+00000fc0: 4e44 3bab 8799 15ed 746c 27c2 9d75 f008  ND;.....tl'..u..
+00000fd0: 4a8c 20c2 1967 4808 835e 6866 890b 4438  J. ..gH..^hf..D8
+00000fe0: 5bdc 1309 69d0 4bf1 120b c870 b678 aeb7  [...i.K....p.x..
+00000ff0: 1704 e54b 0020 c5d9 60ba d729 6c4f 47b8  ...K. ..`..)lOG.
+00001000: cf09 c1cf 46c4 a193 d879 af49 a0d0 09a9  ....F....y.I....
+00001010: d046 d4a1 93d8 b9af 4980 d109 89d1 dd37  .F......I......7
+00001020: ec10 3b89 07f9 8525 9d90 0ddd 7d1f 635f  ..;....%....}.c_
+00001030: 965c 1517 5f89 0ce4 435b 8c03 f682 e0a9  .\.._...C[......
+00001040: 95c8 4016 b401 1168 1476 a676 127c 7442  ..@....h.v.v.|tB
+00001050: 1c74 738d 439f 1576 1273 1282 7442 20b4  .ts.C..v.s..tB .
+00001060: ddc7 4f4e 27e8 afa5 d0a2 13c2 9f5b f9f1  ..ON'........[..
+00001070: b564 859d 149a 8417 9d10 18dd 5ce3 6bc9  .d..........\.k.
+00001080: 0a3b 2f34 65fd 3a84 4324 9ed6 300a fb26  .;/4e.:.C$..0..&
+00001090: 7d12 9674 4234 7473 8dbb 76ac b80a 2eae  }..tB4ts..v.....
+000010a0: 9239 c886 b6fb b8e6 7782 e0b9 916c 410e  .9......w....lA.
+000010b0: 742b 1f9e 1b54 d899 b049 c8d1 0949 d046  t+...T...I...I.F
+000010c0: dd3d 56f8 2e84 c0a3 5387 888a 2b3c ada8  .=V.....S...+<..
+000010d0: f0dd 3d41 4d27 644d 1b8d 5659 e13b d402  ..=AM'dM..VY.;..
+000010e0: a14e 48a1 a22b 2aa6 3b3f 8615 3c75 42dc  .NH..+*.;?..<uB.
+000010f0: b4d1 f887 157e fc23 84ea 84c4 29bb 22e9  .....~.#....).".
+00001100: 7ee7 870f 42a9 4e88 a9c6 03cc 31a7 3a15  ~...B.N.....1.:.
+00001110: fd4a 8dd2 638e bb56 6354 7512 5675 4258  .J..c..VcTu.VuBX
+00001120: 7586 2ee9 9856 9d04 579d 103f 9da9 4b6a  u....V..W..?..Kj
+00001130: 1436 5884 589d 9040 9db1 4b6a 24be 6b28  .6X.X..@..Kj$.k(
+00001140: d8ea 84dc ea8c 5d52 23f1 5d43 615a 2784  ......]R#.]CaZ'.
+00001150: 5a67 ec92 1a89 ef1a 0aef 3a21 f03a 6397  Zg........:!.:c.
+00001160: d448 7cd7 5f50 d809 d1d6 1920 13a7 b01d  .H|._P..... ....
+00001170: 0ea1 6127 c461 67fa fec7 49ec 5be8 4948  ..a'.ag...I.[.IH
+00001180: d909 51d9 99be 0172 92c1 17ac 123d 08c5  ..Q....r.....=..
+00001190: eebe f153 6524 f60d f854 f5d3 5993 4971  ...Se$...T..Y.Iq
+000011a0: a365 1483 d395 a842 3a76 26a6 c749 06be  .e.....B:v&..I..
+000011b0: 1256 c8d4 ce84 f538 c9c0 57c2 0ae9 d9dd  .V.....8..W.....
+000011c0: 176e 2f4b 06be 1256 88d0 c6b3 5edd cffb  .n/K...V....^...
+000011d0: 0647 e8da 0969 d925 be85 ddef 83e2 2579  .G...i.%......%y
+000011e0: 10a5 5da0 bd1c c3b4 5393 8c69 1418 0bb5  ..].....S..i....
+000011f0: 9746 61db 4bc1 6c27 c466 17ca 53a3 b079  .Fa.K.l'.f..S..y
+00001200: 2aa4 ed84 e4ec 42f5 dc28 ec00 4e58 db09  *.....B..(..NX..
+00001210: d9d9 cd35 ee25 1a85 1dc0 35fd 5e9f 9262  ...5.%....5.^..b
+00001220: 8149 944e 103c 3712 2208 d02e 3489 6214  .I.N.<7."...4.b.
+00001230: 7e54 23cc ed84 d0ed 42b3 2846 e1de ba4f  ~T#.....B.(F...O
+00001240: 82e3 4ec8 e3b2 2b2b ec8b f749 48dd 0951  ..N...++...IH..Q
+00001250: 5db4 350a fbee 7d12 8677 4226 7789 9f9c  ].5...}..wB&w...
+00001260: eef7 fd93 23bc ee84 fced 1243 98bd 2028  ....#......C.. (
+00001270: 5fb2 0561 db05 0045 a3b8 f9ae b800 ba13  _..a...E........
+00001280: f2b6 6c8b 0abb 90d0 2484 ee84 c0ed 02c8  ..l.....$.......
+00001290: a051 f8f9 3741 7427 6474 d915 1537 3fea  .Q..7At'dt...7?.
+000012a0: 9875 9110 4c90 07ea 0fb3 e4e6 7bff 02f6  .u..L.......{...
+000012b0: 4e08 eaee be50 2750 72f3 a31d a17b 27a4  N....P'Pr....{'.
+000012c0: 7597 98e6 eb05 7d4d 1192 7742 3277 01a0  u.....}M..wB2w..
+000012d0: cf29 ecc3 232c ef84 6cee ee1a df45 23f1  .)..#,..l....E#.
+000012e0: b612 3bc8 e7ee b6f1 e534 126f 2b69 8488  ..;......4.o+i..
+000012f0: ee02 04a3 53f8 218d 50bd 1352 ba0b 7cf4  ....S.!.P..R..|.
+00001300: e514 b683 2560 ef84 a0ee ee0a b796 257e  ....%`........%~
+00001310: c02a 70ef 84b0 eeee 0bf7 9625 d7a1 e6c5  .*p........%....
+00001320: 5702 0981 dddd 371e d118 49b2 c1b0 e87a  W.....7...I....z
+00001330: 461c 480f 399e 0631 92e4 9751 9240 42a0  F.H.9..1...Q.@B.
+00001340: 77f3 8dbb b246 613b d0c2 004f c8f4 eeae  w....Fa;...O....
+00001350: f153 6524 d7eb 73f1 95a0 4212 78f7 8d9f  .Se$..s...B.x...
+00001360: 2a23 b1d4 f824 8cf0 84cc efee 1b3f 5546  *#...$.......?UF
+00001370: 6209 f949 40e1 09c1 5fe3 8b12 3f9d 2db0  b..I@..._...?.-.
+00001380: f084 f0ef 6e1b 3fcc 4672 ad76 175f 092b  ....n.?.Fr.v._.+
+00001390: 2480 8d2f 4ade fd9b b595 ac42 0a78 89f9  $../J......B.x..
+000013a0: f25e d037 ea82 084f 88fc 2e80 981b c5cd  .^.7...O........
+000013b0: 4fb2 0825 3c21 f5bb 0066 6e14 fe95 ecaa  O..%<!...fn.....
+000013c0: 4baf 71bc dca0 47c8 929b 0dfe 74a7 8bb2  K.q...G.....t...
+000013d0: 71be 80af 9174 8a8b af2c d786 a0f0 ee1b  q....t...,......
+000013e0: 2f7c c592 4e71 f14d e2cb f912 bffa 360a  /|..Nq.M......6.
+000013f0: fbea 3b09 5c9c 1015 5e00 ea37 0afb ea3b  ..;.\...^..7...;
+00001400: 095c 9c10 1566 5754 dcae edd3 c556 9685  .\...fWT.....V..
+00001410: 4356 986d 7924 776d 9e2e b6b2 601c 12c4  CV.my$wm....`...
+00001420: cb43 9881 bda0 5f8f 4ee8 e284 04f1 567e  .C...._.N.....V~
+00001430: bc22 1d2b aedf 1b5c 5c65 7d38 2488 d995  .".+...\\e}8$...
+00001440: d3c8 4ed8 2461 8e13 12c4 6ccb 6964 276c  ..N.$a....l.id'l
+00001450: 9240 c709 1162 b465 c5ed fa89 c5c5 56d7  .@...b.e......V.
+00001460: 8ee4 3022 5bce a26a 577d 14ea 3821 59bc  ..0"[..jW}..8!Y.
+00001470: d9c6 0bf1 b1e2 66c9 8624 2c72 42de 78b3  ......f..$,rB.x.
+00001480: 8d23 9015 b766 5d25 8c10 3766 570e a32b  .#...f]%..7fW..+
+00001490: 547a b195 3042 de98 6d39 8c9a 7f90 258c  Tz..0B..m9....%.
+000014a0: 1038 665b 9e57 6afe d64a 4619 46b9 3f26  .8f[.Wj..JF.F.?&
+000014b0: b3d6 de40 e208 41e4 053e 8130 8a77 1fad  ...@..A..>.0.w..
+000014c0: aba4 11a2 cbec 8a4b 56a6 8777 7f75 beba  .......KV..w.u..
+000014d0: 622d 42cd e88b 8aa9 3dd8 2584 93ae 658b  b-B.....=.%...e.
+000014e0: b4f3 025f 7c18 c5e0 6c25 8e90 6866 5752  ..._|...l%..hfWR
+000014f0: ac7e 5160 5dfb 1681 e605 607e a3b8 d9d7  .~Q`].....`~....
+00001500: 2f49 d7c5 459e 79b3 5d63 5b9e e4f6 ae92  /I..E.y.]c[.....
+00001510: 4648 332f f051 8d51 dc06 d758 d208 6166  FH3/.Q.Q...X..af
+00001520: b625 c56a c787 4997 d345 fa79 0146 d128  .%.j..I..E.y.F.(
+00001530: ecf0 2de9 82ba 4838 2fc0 281a 85cf 455d  ..-...H8/.(...E]
+00001540: 5217 09e7 0568 41a3 182c 1b2d f914 22ce  R....hA..,.-..".
+00001550: dfca 475e 7ab1 9fa4 2461 a253 4738 6bf9  ..G^z...$a.SG8k.
+00001560: 9c38 7651 6da1 9f13 b2cc 0b60 8746 e16b  .8vQm......`.F.k
+00001570: 43d6 d5b6 f95b acfe 9834 92f6 1114 d039  C....[...4.....9
+00001580: 75d8 b21a 70a7 6670 df25 4642 44f9 c500  u...p.fp.%FBD...
+00001590: 03c3 6e1e 9084 694e 4828 c7c9 d8fd bc1f  ..n...iNH(......
+000015a0: 4809 bb9c 9044 5ee3 f986 eef7 41f1 1200  H....D^.....A...
+000015b0: 881c afb0 2cf9 78e1 db24 3872 42b8 78a5  ....,.x..$8rB.x.
+000015c0: 95c9 8dc2 2ed9 2d38 7242 b878 a545 bb8d  ......-8rB.x.E..
+000015d0: c2cd 4a25 a191 13b2 c5ec 8a6b 684f 3e77  ..J%.......khO>w
+000015e0: 0447 4e08 17af 840b 3a89 9f94 121e 3921  .GN.....:.....9!
+000015f0: 8fbc 122e e824 7e52 aae8 22fd 140a 2be0  .....$~R.."...+.
+00001600: 3c4e 6127 a504 604e 0830 af44 ed39 899d  <Na'..`N.0.D.9..
+00001610: 9d4f 0236 27c4 948d 2f4b ecdb 8824 6873  .O.6'.../K...$hs
+00001620: 424e d9f8 b2c4 4ecf 2741 9b13 72ca 2b51  BN....N.'A..r.+Q
+00001630: 8a46 e2df 2526 419b 1372 cac6 1725 fead  .F..%&A..r...%..
+00001640: 4f12 b439 21a7 bcc6 a6e3 b57c 9310 cc09  O..9!......|....
+00001650: 79e4 35a6 6e8c c0de 42e1 9713 c2c8 2b20  y.5.n...B.....+ 
+00001660: 314e 612b a8d0 cb09 5164 7665 85af 9f02  1Na+....Qdve....
+00001670: 2f27 2491 5760 628c c292 38a9 ea66 2218  /'$.W`b...8..f".
+00001680: 2db0 ae95 51dc 060f ab84 1172 c82b 2c6d  -...Q......r.+,m
+00001690: 6514 fe7d 8080 cb09 29e4 dd15 9e62 94dc  e..}....)....b..
+000016a0: 06b7 56a2 0829 e4dd 176a 274a 6e3e 0205  ..V..)...j'Jn>..
+000016b0: 5c4e 082e 6fbe f144 0a2b 06fd 6421 9a53  \N..o..D.+..d!.S
+000016c0: 4828 7f33 40da 79f5 a33e 419a 5348 28bf  H(.3@.y..>A.SH(.
+000016d0: 946f 3a42 f6e9 6c92 3b0d 5384 06b3 ac18  .o:B..l.;.S.....
+000016e0: 0c60 046a 4e88 28b3 2def 2a36 985d 14ac  .`.jN.(.-.*6.]..
+000016f0: 3975 90b2 5e4f cc18 3f8f 2800 73ea 7064  9u..^O..?.(.s.pd
+00001700: 2d1f f710 d9ce c08e 2d9b ee5a c44b dcf4  -.......-..Z.K..
+00001710: c75e cfc0 6e2f 9804 564e 881e af34 cfc0  .^..n/..VN...4..
+00001720: 0afb 5162 1256 3985 4bfe be94 8ff9 e0b7  ..Qb.V9.K.......
+00001730: ee12 2a39 85cb febe 94cf d1e1 eb91 f0c7  ..*9............
+00001740: 295c faf7 9b01 92c6 ab7d 7b9f 0434 4e21  )\.......}{..4N!
+00001750: 38fc 523e 773f 0627 2041 1092 c32f 06f8  8.R>w?.' A.../..
+00001760: 2966 1a5d 22a9 f31d 3aac 0e98 0796 ef4d  )f.]"...:......M
+00001770: 4215 a78e 11d6 f271 d3a0 adee d9a7 5408  B......q......T.
+00001780: e284 3cf0 4af3 8dac f06d 8c10 c429 5cb6  ..<.J....m...)\.
+00001790: f7a5 7cee 2af8 309e 7557 32f3 4e07 a1e0  ..|.*.0.uW2.N...
+000017a0: fdd6 7b07 a9de 1de2 ab0e e3c9 1101 7d13  ..{...........}.
+000017b0: 82be d31d eca0 3604 7d93 80be 09b1 dd89  ......6.}.......
+000017c0: 6677 3a45 6020 3519 01dd ed04 a0d3 dd49  fw:E` 5........I
+000017d0: 0207 a9ca c8e2 1e0e 7012 4663 e9ef 2404  ........p.Fc..$.
+000017e0: 6f42 1ef7 7086 dde6 8cc6 7e52 9004 e24d  oB..p.....~R...M
+000017f0: 88e4 eece 718f c249 6c2e 0bc6 9b90 c935  ....q..Il......5
+00001800: be46 e2ab 9470 bc09 a1dc c318 6eb2 d1f8  .F...p......n...
+00001810: 3396 b440 2af7 3086 7b6c 34de 5837 32c4  3..@*.0.{l4.X72.
+00001820: 7d09 ef68 12cb 49ec 504a 48de 845c ee56  }..h..I.PJH..\.V
+00001830: 089c ee38 7204 da4d 48e0 ee06 7122 a064  ...8r..MH...q".d
+00001840: 347d 23d0 6e42 02d7 f8f2 d488 9f8c 1468  4}#.nB.........h
+00001850: 3721 816b 7c79 b2c3 9388 02ed 2624 70a7  7!.k|y......&$p.
+00001860: bb47 68bf 8dc4 774c 84da 4d88 e01a 5f1e  .Gh...wL..M..._.
+00001870: 8bd8 b7ed 02ed 2624 708d 2d6f 503e 385d  ......&$p.-oP>8]
+00001880: 4926 a476 775f d8fe 1317 acf1 af94 04e6  I&.vw_..........
+00001890: 4d88 e61a 5b96 7894 4268 ded4 b1b9 d2b7  M...[.x.Bh......
+000018a0: 416e 77b5 5fc5 a455 f752 3543 1704 74d7  Anw._..U.R5C..t.
+000018b0: c1b6 9477 ba73 2a0f 5dfa 6362 60f7 a014  ...w.s*.].cb`...
+000018c0: 1237 2356 3bdd d136 9446 6207 fb59 48dc  .7#V;..6.Fb..YH.
+000018d0: dc71 b57a 6266 7519 37da cf02 dde6 0ea1  .q.zbfu.7.......
+000018e0: 5503 4c8e e961 700a b23b 2ae2 b2fb a58b  U.L..ap..;*.....
+000018f0: 770d 45c9 6a87 6a59 00db 8cb8 acb1 6589  w.E.j.jY......e.
+00001900: df3a 5408 db8c 84ad f145 c960 cb52 216f  .:T......E.`.R!o
+00001910: 33af dd7b 07b3 1e2c 5907 b6b2 552a 82b4  3..{...,Y...U*..
+00001920: c696 2583 db2b 5bab 2249 bbfb 8673 d24e  ..%..+[."I...s.N
+00001930: 62e7 aeb2 c0b7 b943 69a5 be20 66bb fa71  b......Ci.. f..q
+00001940: 669e 7443 669e 25e9 8fc9 19b8 b178 16a0  f.tCf.%......x..
+00001950: 369b 657c fb63 e7ec 9bbd 3342 ce66 b38a  6.e|.c....3B.f..
+00001960: 6f7f 4c4e c021 5359 20d9 dc21 af6a c061  o.LN.!SY ..!.j.a
+00001970: 637b 1d59 70d8 dcc1 ad6a 305c 9f2a 0be2  c{.Yp....j0\.*..
+00001980: 9a11 589d 6067 e84e 1094 2fb5 1e79 d509  ..X.`g.N../..y..
+00001990: f697 ef15 8181 d46f 2453 27da 63de 4aec  .......o$S'.c.J.
+000019a0: 96da 42b3 6666 53d9 d748 7c57 4270 d6cc  ..B.ffS..H|WBp..
+000019b0: 702a 1a3b 89ef 6208 cf9a 914e 35c6 e6f5  p*.;..b....N5...
+000019c0: 89ad 4e42 b466 e453 27da eade 4afc 26f0  ..NB.f.S'...J.&.
+000019d0: 9213 48a8 1a5f 23f1 092b 546b 4646 d518  ..H.._#..+TkFF..
+000019e0: b3c4 c78a 70ad 1929 55e3 6b06 33b6 c912  ....p..)U.k.3...
+000019f0: b035 23a6 6a7c 4d8f c43f 5892 4d08 aa1e  .5#.j|M..?X.M...
+00001a00: be71 3a39 8d9d 15c8 82b7 6684 559d 336b  .q:9......f.U.3k
+00001a10: 2c93 9585 70cd c8ab 1ec6 e14c 8bd5 d809  ,...p......L....
+00001a20: 892c 946b 4692 f570 0e3f 35b5 1a3b 2591  .,.kF..p.?5..;%.
+00001a30: 857f cdc8 b83a 67a3 49ee 8d58 1632 3623  .....:g.I..X.26#
+00001a40: e77a 3887 dfb3 598d fd22 3f0b 1d9b 9180  .z8...Y.."?.....
+00001a50: 3d9c 9f62 67a3 b1df e467 c166 33a2 b1bb  =..bg....g.f3...
+00001a60: 73dc df76 1237 8398 85a6 cd48 cc1a 5f23  s..v.7.....H.._#
+00001a70: b154 4416 cc36 2366 7b18 c775 d969 2c07  .TD..6#f{..u.i,.
+00001a80: 9205 c1cd 88e0 1ece 7165 761a cbdb 64a1  ........qev...d.
+00001a90: 7333 d2b9 53fc 02a2 17f4 9d3a a173 33b2  s3..S......:.s3.
+00001aa0: b65b f970 4587 d3c1 5940 dccc abfc 4e40  .[.pE...Y@....N@
+00001ab0: 6559 89ed 350a 8a9b 0d58 8bbe a60f 656b  eY..5....X....ek
+00001ac0: a5b0 b899 17fa 655f 23f1 9d46 8171 3392  ......e_#..F.q3.
+00001ad0: b587 717c 2f9d c60f 2305 c7cd 08d7 3a67  ..q|/...#.....:g
+00001ae0: a3f1 fd37 4172 33f2 b587 735c 419c c68f  ...7Ar3...s\A...
+00001af0: 0d04 cacd 48d8 3a67 a3f1 d31d 82e5 6664  ....H.:g......fd
+00001b00: 6c77 e7b8 0fe7 24b6 932e 586e 46c6 d6f8  lw....$...XnF...
+00001b10: 9a8e 94af 5092 50c8 d81e bef0 7419 8d3d  ....P.P.....t..=
+00001b20: 61e1 7233 72b9 8771 7c8b 9dc6 1b4b 7475  a.r3r..q|....Ktu
+00001b30: 00ae 4c3a 209c bb5d 52db 5b12 3c37 236c  ..L: ..]R.[.<7#l
+00001b40: 3b4d 3485 cd92 3bdf 2716 4037 236e 6b7c  ;M4...;.'.@7#nk|
+00001b50: 59e2 e79d 85d0 cdc8 db1a 5f33 ccb3 c128  Y........._3...(
+00001b60: 8c6e 46e2 76f7 8dab 8c91 f899 7c81 7433  .nF.v.......|.t3
+00001b70: 22b7 c6d7 0cf3 1c51 9405 d3cd 1d73 ab0f  "......Q.....s..
+00001b80: ee78 b249 c8db 8c18 ed04 55be 1304 e54b  .x.I......U....K
+00001b90: aa20 2fbb 950f 06e3 7e8f b0b4 1979 d9dd  . /.....~....y..
+00001ba0: 207e e69c c4f6 7b84 b1cd ccd1 26c2 65ac   ~....{.....&.e.
+00001bb0: c637 894d 52a5 3157 47b8 8cd5 f8ae 8ff0  .7.MR.1WG.......
+00001bc0: b799 69da 44ab d25b 8d5d 9832 0b81 9b91  ..i.D..[.].2....
+00001bd0: b23d 9ce3 71a7 d3d8 2522 b3b0 b999 f9db  .=..q...%"......
+00001be0: 4453 394e 621b 2721 7633 52b9 872f 3c5f  DS9Nb.'!v3R../<_
+00001bf0: 46e3 a772 84e5 cd48 e61e cef0 7c19 8d9f  F..r...H....|...
+00001c00: 5111 9e37 23b3 7b38 c3f3 6534 7e46 4548  Q..7#.{8..e4~FEH
+00001c10: df8c 34ef ee1c 8fb5 9dc4 8ef1 0500 ce08  ..4.............
+00001c20: f91e bef1 5d76 1a3f d416 3438 23fe 7b38  ....]v.?..48#.{8
+00001c30: c777 d969 fc50 5b98 e1ec b8e0 d876 b83c  .w.i.P[......v.<
+00001c40: 7116 6238 2315 bc95 0f57 74b8 814b 1664  q.b8#....Wt..K.d
+00001c50: 3833 169c 68e8 e924 b6c9 1190 3823 166c  83..h..$....8#.l
+00001c60: 7c8d c4f7 af84 25ce c80b 1b63 23f1 1d4a  |.....%....c#..J
+00001c70: 618c b3e3 88a9 9175 1adf d409 7b9c 7179  a......u....{.qy
+00001c80: e1c3 199e 53a3 f1cd bba0 ca99 51e5 dd39  ....S.......Q..9
+00001c90: 0e41 a7f1 8dac 40cc 9921 e6dd 396e 649d  .A....@..!..9nd.
+00001ca0: c637 b242 3767 a69b 138d 799d c436 b2c2  .7.B7g....y..6..
+00001cb0: 3c67 e697 d9d7 7dd5 e02f b564 14e3 cb09  <g....}../.d....
+00001cc0: 07db 4ee3 5b77 419e 33f3 cb09 47db 4ee3  ..N.[wA.3...G.N.
+00001cd0: 5b77 819e 3313 ccbb 73fc 603b 8d6f dd85  [w..3...s.`;.o..
+00001ce0: 7ace 4c30 1b67 a3f1 6f2d 047b ce8c 3027  z.L0.g..o-.{..0'
+00001cf0: f87c d44a 6cbf 42a8 e7cc 08f3 ee0b cf97  .|.Jl.B.........
+00001d00: d1f8 7e85 70cf 99b9 67e3 6c34 feb5 8500  ..~.p...g.l4....
+00001d10: d199 81e8 dd39 7eb2 9dc6 f768 0489 ce8c  .....9~....h....
+00001d20: 4427 f85a d74a dc42 9a59 90e8 cc48 74a2  D'.Z.J.B.Y...Ht.
+00001d30: ef75 adc6 aea5 9905 8ace 4c38 27fa 62d7  .u........L8'.b.
+00001d40: 6aec 729a 59b0 e8cc 5874 22fa cd48 1efc  j.r.Y...Xt"..H..
+00001d50: bb75 01a3 3353 ce6c ccdf 6e7a 8641 c0e8  .u..3S.l..nz.A..
+00001d60: cc60 7422 ecce 481e fcec 96a0 d1b9 e39c  .`t"..H.........
+00001d70: 6596 8919 e8cd c14e 390b 049d 0d04 dd1f  e......N9.......
+00001d80: 5307 3b13 2a18 7436 1874 7fec c561 b133  S.;.*.t6.t...a.3
+00001d90: 7145 28e8 6228 e8fe 989e 815b 8baa 0806  qE(.b(.....[....
+00001da0: 5d3a a659 1d78 191c fb9e a308 ef5c 0cef  ]:.Y.x.......\..
+00001db0: dc1f 7bbd 44f7 76f4 5084 772e cc34 2758  ..{.D.v.P.w..4'X
+00001dc0: aed0 491e ecf4 7b11 0cba 3006 cdc6 fcc5  ..I...{...0.....
+00001dd0: e7e0 84ab f8ba a408 7b95 4ee2 31ab 2220  ........{.N.1." 
+00001de0: 7461 aa39 c1fc bb93 0c7c 67f1 e534 405f  ta.9.....|g..4@_
+00001df0: 94b4 41dd 58c4 1733 22cc e3fe f7dd 38bf  ..A.X..3".....8.
+00001e00: 08f0 5c98 5e8e fb31 bda0 2f5f c0e6 82f0  ..\.^..1../_....
+00001e10: f256 7e6c 10a2 d017 03c9 0e86 9733 cc8d  .V~l.........3..
+00001e20: 5b89 1b56 15e1 9d0b 32cd bb6f 5c01 9cc4  [..V....2..o\...
+00001e30: 4d90 14e1 a08b e1a0 e363 97a2 243b 986a  M........c..$;.j
+00001e40: 8efb 55bd 2028 5f32 0257 f3dd ca07 8321  ..U. (_2.W.....!
+00001e50: 065d 0483 2e8c 4117 bcf7 46e2 ef81 6401  .]....A...F...d.
+00001e60: e3d1 eccb 123b a22e 424d 1746 a00b bd8f  .....;..BM.F....
+00001e70: b11a 3b55 5484 9b2e 0c41 177a 1f63 3576  ..;UT....A.z.c5v
+00001e80: aaa8 0838 5d98 822e 54cf 9cc4 d66f e1a6  ...8]...T....o..
+00001e90: 0b43 d0ec cb12 7f8f 859b 2e0c 4117 7a27  .C..........A.z'
+00001ea0: 6235 76d6 a408 395d 1883 2ef4 4ec4 6aec  b5v...9]....N.j.
+00001eb0: ac49 1174 ba30 071d 0fb3 7a41 9f13 8248  .I.t.0....zA...H
+00001ec0: 17e6 9d4b 3c5b de2b 0203 0922 069b 0b4c  ...K<[.+..."...L
+00001ed0: 1e3b 895d b8ab 080b 5d98 6b66 5f96 f8cd  .;.]....].kf_...
+00001ee0: ec8a a0d0 85b1 e612 ef2a d72b 822b 2a81  .........*.+.+*.
+00001ef0: c3f8 7281 6de5 9ce4 d177 6c85 782e 4c2f  ..r.m....wl.x.L/
+00001f00: a3b1 91bc fb77 eb2b 79c3 ec32 fba2 a40d  .....w.+y..2....
+00001f10: 7c25 6f98 5c2e b493 9ed3 5cf7 6cb8 184b  |%o.\.....\.l..K
+00001f20: dc30 b85c 682f 3da7 b9ee da70 3196 b461  .0.\h/=....p1..a
+00001f30: 7079 370e 674a 9de6 d167 bbd0 ce85 d165  py7.gJ...g.....e
+00001f40: e36c e657 bcb1 e413 93cb 0536 1074 9251  .l.W.......6.t.Q
+00001f50: 6d92 8062 7099 8d59 3232 9680 62d6 7937  m..bp..Y22..b.y7
+00001f60: 86c7 9a35 ef9e adb1 0417 43d0 bb31 3cd6  ...5......C..1<.
+00001f70: 26b9 dc44 6911 38ba 30e9 5ce2 3dc1 7a45  &..Di.8.0.\.=.zE
+00001f80: 1fc9 4241 1746 9a0b 6c0a e624 d7ad 382e  ..BA.F..l..$..8.
+00001f90: be92 508c 34ef bef1 ad34 9a47 3bcf 5f04  ..P.4....4.G;._.
+00001fa0: 832e 8c34 efce f1bd 349a 473b db5e 0483  ...4....4.G;.^..
+00001fb0: 2e8c 3417 d809 cd48 aa1f d908 045d 1868  ..4....H.....].h
+00001fc0: 2eb4 2799 d1d4 413f 5f20 e8c2 4073 a15d  ..'...A?_ ..@s.]
+00001fd0: c98c a60e c636 0241 1726 9ae3 fd0a 7b41  .....6.A.&....{A
+00001fe0: 506f 248a 985c 2e37 b8a2 e3be 9250 cd85  Po$..\.7.....P..
+00001ff0: 09e5 cd00 2aa6 4929 fbb0 08d4 5c18 50de  ....*.I)....\.P.
+00002000: 7de3 5333 1acf 0f14 a19a 0b93 cbbb 73fc  }.S3..........s.
+00002010: b018 8d67 268a e0ce 85d9 e5dd 397e 5e8c  ...g&.......9~^.
+00002020: c693 0b45 80e7 c2f4 f2e6 1c47 8291 7870  ...E.......G..xp
+00002030: a108 f15c 185f de8d e136 9bfc 1a38 4b1a  ...\._...6...8K.
+00002040: 31c0 bc3b c36d 3609 3670 9634 6284 7977  1..;.m6.6p.4b.yw
+00002050: 86db 6c12 6ce0 2c69 846b 0def cef1 94ef  ..l.l.,i.k......
+00002060: 1887 2e82 4317 c6a1 7707 b89f e344 1222  ....C...w....D."
+00002070: ba30 11bd 5bc0 8d1b 4f2c 0b13 5d18 702e  .0..[...O,..].p.
+00002080: b7d8 205c 91f8 6220 19c3 20f3 6610 a76a  .. \..b .. .f..j
+00002090: b826 f1c5 41b2 a499 2c21 0794 cc83 7728  .&..A...,!....w(
+000020a0: c238 17e6 9577 e3f8 0930 9a27 1f9f c238  .8...w...0.'...8
+000020b0: 17e6 9577 67b8 6fac 79f2 4d86 30ce 8581  ...wg.o.y.M.0...
+000020c0: e5dd 39ae d146 f334 b8da 9225 4c2c 1b67  ..9..F.4...%L,.g
+000020d0: d4cc 83d7 9e42 3917 2696 77e7 1076 739a  .....B9.&.w..vs.
+000020e0: 27df 5809 e55c 9858 de9c e3c6 8a25 d5cf  '.X..\.X.....%..
+000020f0: da0a e35c 1858 de7d e1c9 464d 1dcc 9e0a  ...\.X.}..FM....
+00002100: e55c 9858 de9d e327 9b35 7530 7b2a 9473  .\.X...'.5u0{*.s
+00002110: 6162 b9c0 6a76 4e62 57e4 29c2 3817 b32e  ab..jvNbW.).8...
+00002120: 727f 4c86 d2b6 2914 c8b9 9865 91fb 637f  r.L...)....e..c.
+00002130: d840 d288 89e5 020b e339 c9bd 5d91 af08  .@.......9..]...
+00002140: e55c 1859 2eb0 f39e 933c fa2c 12ca b930  .\.Y.....<.,...0
+00002150: b25c 60a3 4127 79f7 abf5 9524 6260 997d  .\`.A'y....$b`.}
+00002160: cddb 73c7 f714 419c 0be3 caec cb92 c1fc  ..s...A.........
+00002170: 9310 ce85 6965 3666 89c5 8d8a f0cd 8559  ....ie6f.......Y
+00002180: e502 fb0d 3a89 e750 846e 2ee1 42cc 2f06  ....:..P.n..B./.
+00002190: 266d fc89 49da 3093 bc9d d814 c79c d178  &m..I.0........x
+000021a0: 0043 30e6 c248 b231 464d f58f 9050 cca5  .C0..H.1FM...P..
+000021b0: 2392 f592 620c 8dfa 8142 2b97 8e3c 5607  #...b....B+..<V.
+000021c0: ce1b 8ba6 1581 920b 03c6 05b6 fa74 12cb  .............t..
+000021d0: 1316 4192 0bf3 c5ec 8b92 eae7 d905 492e  ..A...........I.
+000021e0: 8c17 17a2 a28c a49b 62bc 184b dc30 5d5c  ........b..K.0]\
+000021f0: 00dc 7412 cf06 0a8f 5c98 2d2e 006e 3a89  ..t.....\.-..n:.
+00002200: efd9 0a8d 5c18 2d2e 4463 1989 0564 8bd0  ....\.-.Dc...d..
+00002210: c885 c962 f635 21f4 c5fa 4a08 755c b1d4  ...b.5!...J.u\..
+00002220: 5466 8efd 3623 4590 e3d2 f1c3 6a60 8041  Tf..6#E.....j`.A
+00002230: 6f20 59d3 71c2 6a30 7edb 2eb4 7061 f4b7  o Y.q.j0~...pa..
+00002240: c63d fc4e 1094 2fe9 c1e0 6f05 6e29 c488  .=.N../...o.n)..
+00002250: 2f06 1213 ccfd 56e2 879c c4be 4911 52b8  /.....V.....I.R.
+00002260: 1852 b83f 26f9 e7aa 6515 54b8 320e 7cdd  .R.?&...e.T.2.|.
+00002270: 35fe 3f5d 7b41 77e1 aa80 c295 173f a6f2  5.?]{Aw......?..
+00002280: 8733 3255 38e1 ca6b 1fb7 f8ce 5b85 bd6a  .32U8..k....[..j
+00002290: 595c cd06 4ef1 e360 256e febe 0a3b 5c0d  Y\..N..`%n...;\.
+000022a0: 088c be46 32b9 be5c 1578 b832 09dc 8863  ...F2..\.x.2...c
+000022b0: b31a db4e 56a1 872b a3c0 8d38 36ab b1f3  ...NV..+...86...
+000022c0: 4f55 f8e1 6a60 605a 57c0 6aec 5c4c 1582  OU..j``ZW.j.\L..
+000022d0: b832 41dc 685d 01ab b173 d955 e0e2 ca70  .2A.h]...s.U...p
+000022e0: 7183 ed0c acc4 cd02 5581 8e2b 43c7 e8eb  q.......U..+C...
+000022f0: 2476 12a8 0a8c 5c99 2c66 6323 b173 4055  $v....\.,fc#.s@U
+00002300: 68e4 ca68 311b 1b89 fdec b00a 8e5c 79e9  h..h1........\y.
+00002310: 6536 76fb d5d9 674b e0e5 caf0 728b f71e  e6v...gK....r...
+00002320: 710a 7f9d 25b9 1869 de5c c30e be93 d86f  q...%..i.\.....o
+00002330: 1dab 90ce 95b1 e5cd 37ec df3b 895f 21ac  ........7..;._!.
+00002340: 0aea 5c99 5bde 8de3 a836 9a07 3b47 5605  ..\.[....6..;GV.
+00002350: 76ae 0c2e efce 708b 59e3 5782 ab02 3b57  v.....p.Y.W...;W
+00002360: 0697 37e7 7050 e324 f67d 7a15 d4b9 32b7  ..7.pP.$.}z...2.
+00002370: 8cbe 46e2 5fa7 5761 9d2b 83cb 6ccc 12ff  ..F._.Wa.+..l...
+00002380: 4ebb 0aec 5c19 5c66 6396 f8b7 ac55 58e7  N...\.\fc....UX.
+00002390: cadc 321b b3e4 6172 f364 5550 e7ca a833  ..2...ar.dUP...3
+000023a0: 1b9b dcb2 5313 5518 e8ca 0cf4 6e1c 5764  ....S.U.....n.Wd
+000023b0: a3f1 c844 1538 ba32 e9bc 3bc7 15d9 681e  ...D.8.2..;...h.
+000023c0: 7c3f 53f0 e8ca acf3 e61c 7e1c e724 f69b  |?S.......~..$..
+000023d0: e52a 7474 653a 7af3 0d27 7f9d c42e f550  .*tte:z..'.....P
+000023e0: 059a ae4c 405f 5bb8 17d7 e13b f72a 6c74  ...L@_[....;.*lt
+000023f0: 65d0 b9c5 1c7d af08 0c24 880c d10c 3cbb  e....}...$....<.
+00002400: 9358 8ebe 0a04 5d19 686e b406 8bd3 7890  .X....].hn....x.
+00002410: be0a 055d 9968 6eb4 068b d38c 9c25 8918  ...].hn......%..
+00002420: 696e b406 8bd3 f8c9 ca2a 1874 3548 33ac  in.......*.t5H3.
+00002430: 48e2 2476 a7d8 2a14 7465 a4b9 c51f 2df4  H.$v..*.te....-.
+00002440: 8ae0 f195 bc61 74b9 01c3 ef24 764b f32a  .....at....$vK.*
+00002450: b073 6570 997d 5972 b31b 9a55 819d 2b83  .sep.}Yr...U..+.
+00002460: cb8d 3e1e 701a bf9b 7a15 dab9 32ed dce8  ..>.p...z...2...
+00002470: eb01 a7f1 bbd6 57c1 a02b 33cd c6d9 8494  ......W..+3.....
+00002480: ef97 0a08 5d19 6a36 ce26 a5ec 7b9c 2a20  ....].j6.&..{.* 
+00002490: 7465 a8b9 d187 0b4e e377 afaf 0242 57a6  te.....N.w...BW.
+000024a0: 9a77 e778 f2c2 686e d976 1105 85ae 8c35  .w.x..hn.v.....5
+000024b0: 1b67 1353 d976 5b04 85ae 8c35 b798 e4ef  .g.S.v[....5....
+000024c0: 157d 4e09 f15c 9978 6e40 f2f7 92c0 4112  .}N..\.xn@....A.
+000024d0: 8999 6776 f82f 2792 b0d0 95c1 e646 1f0b  ..gv./'......F..
+000024e0: 38cd cd2e 1753 8586 ae4c 3637 fa58 c069  8....S...L67.X.i
+000024f0: ecab f72a 3074 65b0 7937 8e1f 18a3 b915  ...*0te.y7......
+00002500: ef2c 81c4 60b3 7166 8dcf 2361 a12b 83cd  .,..`.qf..#a.+..
+00002510: bb71 5c37 8de6 7605 fd2f ce92 470c 361b  .q\7..v../..G.6.
+00002520: 6793 4776 51a0 2a30 7465 b0d9 389b 3c2a  g.GvQ.*0te..8.<*
+00002530: 3609 0586 ae0c 3637 f818 c548 aa6f ef04  6.....67...H.o..
+00002540: 85ae 8c42 b3af e94e 151b c042 4857 26a4  ...B...N...BHW&.
+00002550: d9f8 bf9c 5ec2 4d57 e6a6 1bac e6e2 249e  ....^.MW......$.
+00002560: 04a9 4253 57a6 a91b e04a 4ee2 9747 aa42  ..BSW....JN..G.B
+00002570: 5957 a6ac 1b80 0b4e e243 b349 7435 8e21  YW.....N.C.It5.!
+00002580: 2035 9c64 70a1 25b9 18a3 6e00 4c38 89fd   5.dp.%...n.L8..
+00002590: 2cb1 0a78 5d3b 88fa 7cf5 db1f d367 d7e6  ,..x];..|....g..
+000025a0: 9300 d6b5 83a5 d5c1 64d7 7b9b bd02 5257  ........d.{...RW
+000025b0: 86a2 1b50 934e 72f3 ef1a 84a3 aecc 44b3  ...P.Nr.......D.
+000025c0: b109 22cb 9e55 c1a8 2b33 d19b f174 173b  .."..U..+3...t.;
+000025d0: bb24 72e0 6415 90ba 3214 bd3b 4305 711f  .$r.d...2..;C.q.
+000025e0: e0db e748 40ea ca50 343b 1bcd cd67 9180  ...H@..P4;...g..
+000025f0: d495 a9e8 06d4 9893 dc2c 5554 85a4 ae4c  .........,UT...L
+00002600: 4b37 8036 9de4 e627 8585 b0ae 4c51 3762  K7.6...'....LQ7b
+00002610: 1b9d c6d2 9c55 c8eb ca18 b531 7631 e5d0  .....U.....1v1..
+00002620: c02a e875 ed38 6a89 2966 ac37 07db b408  .*.u.8j.)f.7....
+00002630: 635d 3b60 5a1d 5c1e 3996 aa0a 4d5d 0d1a  c];`Z.\.9...M]..
+00002640: 0d14 9a93 f8ee 89d0 d4b5 43a3 f5cc dc5a  ..........C....Z
+00002650: 86fe cc24 763a 065a 1d38 927c 1d17 3eba  ...$v:.Z.8.|..>.
+00002660: 76b0 b318 3008 dd2c e95e 0584 ae06 84ee  v...0..,.^......
+00002670: 8f89 81cd 4701 a16b 0735 ab81 799f e61f  ....G..k.5..y...
+00002680: 6021 9e6b 472f ab83 1979 f906 55d0 e66a  `!.kG/...y..U..j
+00002690: d0e6 fe98 9e83 bf4a 52cd 0dda 1c1f bb14  .......JR.......
+000026a0: 25f5 9989 e439 9e4f e804 41f9 529b 993c  %....9.O..A.R..<
+000026b0: 9e01 3aeb 1481 8154 5b46 8c67 e2bc 9cc4  ..:....T[F.g....
+000026c0: be55 1128 b932 613c 23e6 e534 d658 a8e4  .U.(.2a<#..4.X..
+000026d0: ca88 f18c 9497 d378 63a9 fccc 18cf b068  .......xc......h
+000026e0: 9895 d837 1b82 25d7 8e31 96a7 3d3c 7629  ...7..%..1..=<v)
+000026f0: 4a2a 3fd3 c44b 7cc7 4234 f952 be54 7d86  J*?..K|.B4.R.T}.
+00002700: 8917 78da 4334 f962 2035 9f17 245e e869  ..x.C4.b 5..$^.i
+00002710: 7712 7fef 2526 984a 5ef0 de1b 89bf f712  w...%&.J^.......
+00002720: 1f66 09e3 fed8 69e0 87ac 422b 5746 8f17  .f....i...B+WF..
+00002730: ea6d 1889 8f70 a195 aba1 95fb 6372 e5ec  .m...p......cr..
+00002740: 9935 c195 9b59 d938 3e76 296a 92a2 b01a  .5...Y.8>v)j....
+00002750: afe1 53dd 0b82 f293 948f 2dfb 1a57 9b5e  ..S.......-..W.^
+00002760: 1118 6431 e0af 08a0 da58 89ab 364d 20e4  ..d1.....X..6M .
+00002770: c644 31fb 1a89 ed83 3481 901b 03c5 6c4c  .D1.....4.....lL
+00002780: 9274 377a ea9a 1863 ad67 6396 d8be 7513  .t7z...c.gc...u.
+00002790: 02b9 7534 b13e ed18 14ab 1d4d 3601 8d1b  ..u4.>.....M6...
+000027a0: 43c3 2b24 a095 b804 6c82 1937 6686 d9d7  C.+$....l..7f...
+000027b0: 486c 4235 e18c 1b43 c32b eca8 6525 ee7d  HlB5...C.+..e%.}
+000027c0: 7f13 ccb8 3133 bcf9 8693 8856 e2b8 a626  ....13.....V...&
+000027d0: 9471 eb90 6179 8218 275e 0775 4370 e266  .q..ay..'^.uCp.f
+000027e0: 5637 ee8f a983 7d48 851b 6ee1 1ac6 2f0e  V7....}H..n.../.
+000027f0: 1c2c 8387 4272 8579 df15 9a4b 2719 5c3a  .,..Br.y...K'.\:
+00002800: 8915 e67d 5798 d176 129f a342 0837 a67d  ...}W..v...B.7.}
+00002810: d997 24e9 6e70 9d25 6d3a d657 6fe4 70b9  ..$.np.%m:.Wo.p.
+00002820: 9a26 c06f 437a 77cb f5f8 0486 dc5c 13b0  .&.oCzw......\..
+00002830: b721 a5bb 951f 1b74 8ac0 4002 0169 dcdd  .!.....t..@..i..
+00002840: 207e e69c c442 644d 00de 8634 ee61 0ce7   ~...BdM...4.a..
+00002850: 6634 1622 6b42 f036 c471 0fe7 708c 6735  f4."kB.6.q..p.g5
+00002860: 962a 6d82 f036 e471 0fe7 f0ad b7d5 0c9c  .*m..6.q........
+00002870: 255a 90c7 3d9c c357 c056 6379 e926 0c6f  %Z..=..W.Vcy.&.o
+00002880: 431e 7777 8e2b b993 d8a6 5d08 de86 38ae  C.ww.+....]...8.
+00002890: f135 12fb 254f 1384 b721 8f6b 8c8d c47e  .5..%O...!.k...~
+000028a0: c9d3 84e1 6dc8 f06e a5c0 533d 0e23 8178  ....m..n..S=.#.x
+000028b0: 1b42 bcbb 419c 154e 62c1 b926 706f 4352  .B..A..Nb..&poCR
+000028c0: 7737 8e2f a993 5886 ac09 dddb 90d4 dd8d  w7./..X.........
+000028d0: e36e 9a93 5848 b109 dcdb 10d4 35c6 4662  .n..XH......5.Fb
+000028e0: d9b5 266c 6f63 4e97 36ed 3692 d5ce ae37  ..&locN.6.6....7
+000028f0: 217b 5b87 e94a 9b1c 1ebb 1425 8983 b06e  !{[..J.....%...n
+00002900: 8266 65cc ea36 6175 1b82 b75b f960 309c  .fe..6au...[.`0.
+00002910: 756d 02e5 3624 6c77 03a8 67e3 6e8b d0b7  um..6$lw..g.n...
+00002920: 0d49 dadd 01ee f238 2b84 b26d 48cc 6e0e  .I.....8+..mH.n.
+00002930: 7118 8dd7 146e 02d3 3604 6377 83f8 2275  q....n..6.cw.."u
+00002940: 92c0 412a 3f02 b0bb 437c 913a 49e0 20b5  ..A*?...C|.:I. .
+00002950: 1c41 d734 01c2 d24b 0207 a9ce 08b4 ee0e  .A.4...K........
+00002960: f178 af93 040e 5271 115c dd1d e03e 8ceb  .x....Rq.\...>..
+00002970: b340 ad0d a1d6 8491 34a6 5a9b 50ad 2d44  .@......4.Z.P.-D
+00002980: 545f 8a1a d75d c157 1bb2 a829 5e43 ae17  T_...].W...)^C..
+00002990: 04e5 4bcd 45e2 742b 1f0c c615 5760 d486  ..K.E.t+....W`..
+000029a0: 60e9 6e10 df4f 27b1 b379 c2a2 36e4 4a0f  `.n..O'..y..6.J.
+000029b0: dff8 d49c c68f 4484 456d c895 1ece 7158  ......D.Em....qX
+000029c0: 398d 1f89 088c da10 2cdd 4a01 df71 f517  9.......,.J..q..
+000029d0: e6b4 213f ba1b c0cd 6489 fd1e b509 71da  ..!?....d.....q.
+000029e0: 901e 3d7c e166 b2c6 7f90 da84 386d 888f  ..=|.f......8m..
+000029f0: 1ece 7051 59e3 3f56 6cc2 9c36 0448 136d  ..pQY.?Vl..6.H.m
+00002a00: f3e6 247e f646 90d3 162e b0fb 6230 0e17  ..$~.F......b0..
+00002a10: 8148 1b12 a129 fe5e bb17 f4e5 0b2b da10  .H...).^.....+..
+00002a20: fc4c b0a5 5baf 080c 2444 10f0 4cb4 a59b  .L..[...$D..L...
+00002a30: 95d8 e7bd 4984 348c 830c 15b9 5304 2726  ....I.4.....S.'&
+00002a40: 4981 24e7 6e00 27c6 125f 9105 fe6c 0878  I.$.n.'.._...l.x
+00002a50: 1ebe 70cf 5833 a8c8 0285 3604 3f9d 336b  ..p.X3....6.?.3k
+00002a60: fca7 e54d 60d1 86e4 e7e1 0cb7 9335 8308  ...M`........5..
+00002a70: 115a b421 fa99 686b 4c27 f1eb 1634 a145  .Z.!..hkL'...4.E
+00002a80: 1b92 9fc6 1825 d9cf c40a 2bda 90fb 4c99  .....%....+...L.
+00002a90: 32d3 48fc f90a 29da 90fa 645f b34a af65  2.H...)...d_.J.e
+00002aa0: 639b 70a2 ad83 3e25 abc3 6397 a224 7210  c.p...>%..c..$r.
+00002ab0: e34c f127 f9bd 2028 5f12 0761 cd04 5b30  .L.'.. (_..a..[0
+00002ac0: f68a c040 a205 a1cc 445b 215a 898d 34c1  ...@....D[!Z..4.
+00002ad0: 381b a29a 89b6 e7b3 123b 2129 7067 3370  8........;!)pg3p
+00002ae0: 677c ec52 94e4 0422 9929 5ec6 ae17 04e5  g|.R...".)^.....
+00002af0: 4b1c 2091 9960 19bb 5e11 1848 bd47 2033  K. ..`..^..H.G 3
+00002b00: d132 7656 62ef bd30 9c0d 39cd dd37 bef7  .2vVb..0..9..7..
+00002b10: 4e62 efbd a09d 0df1 cddd 371e e83b 890f  Nb........7..;..
+00002b20: 3a41 3e9b 413e e363 97a2 2410 90df 4cf1  :A>.A>.c..$...L.
+00002b30: 0a7a bd20 285f f200 e9cd 042b e8f5 8ac0  .z. (_.....+....
+00002b40: 402a 3eae 4b9b 68d1 3a2b f10f 9d54 7ca4  @*>.K.h.:+...T|.
+00002b50: 4013 ae59 6735 be0f 257c 6843 3ed4 391b  @..Yg5..%|hC>.9.
+00002b60: 8d7f 572e e068 430a 34e1 6a79 56e3 fb50  ..W..hC.4.jyV..P
+00002b70: 828e 36c4 4013 ae96 6735 beae 093b da90  ..6.@...g5...;..
+00002b80: 03dd 9de3 7071 121b 2e82 8e36 e440 77df  ....pq.....6.@w.
+00002b90: 385c 9cc4 b224 828e 365c 9e36 c13a 6abd  8\...$..6\.6.:j.
+00002ba0: a2af b002 9436 044a 13ad 10e7 247e d023  .....6.J....$~.#
+00002bb0: a069 43d0 f4f0 8dab 8dd1 0c06 3d42 a036  .iC.........=B.6
+00002bc0: c449 0f67 b8a8 ac19 0c3d 8441 6d08 9426  .I.g.....=.Am..&
+00002bd0: 5a9e ce49 ecc2 434d 18d4 869c 69a2 e5e9  Z..I..CM....i...
+00002be0: 9cc4 2e8b d704 4d6d c899 265a 4dcb 49ec  ......Mm..&ZM.I.
+00002bf0: 024f 4dd0 d486 f8e9 e61b 8753 08b3 be31  .OM........S...1
+00002c00: 9885 4c9d 7121 dddd 20ac 344e 6217 429a  ..L.q!.. .4Nb.B.
+00002c10: 0563 9d11 633d 7cc3 4ae3 347e 39a2 5900  .c..c=|.J.4~9.Y.
+00002c20: d719 01d7 c339 ac34 4ee3 9723 9a85 7c9d  .....9.4N..#..|.
+00002c30: 1163 dd9d c34a e324 7e3d 9759 d0d7 1939  .c...J.$~=.Y...9
+00002c40: 5663 cc12 ffa9 ee2c e8eb cc1c eb66 1c56  Vc.....,.....f.V
+00002c50: 5727 b10b 30cd 42be ce88 b1ee be61 7575  W'..0.B......auu
+00002c60: 12bb 3ed2 2ce4 eb8c 74eb ee1b 7e56 ef24  ..>.,...t...~V.$
+00002c70: b6ff 340b 103b 23dd bafb 865f d53b 8945  ..4..;#...._.;.E
+00002c80: f266 0162 67a4 5b77 dff0 7b52 27b1 afff  .f.bg.[w..{R'...
+00002c90: 67e1 6167 845b 137d dcee 241e c49d 0588  g.ag.[.}..$.....
+00002ca0: 9d91 6e4d f441 a493 0c7c 25b4 107a 4db4  ..nM.A...|%..zM.
+00002cb0: 8a80 93f8 0f77 67e1 6467 6461 132d 9be0  .....wg.dgda.-..
+00002cc0: 243e b284 9e9d 0d3d 1b1f bb14 2521 84d0  $>.....=....%!..
+00002cd0: 6b8a 3fab eb05 41f9 1236 08b7 26f8 acae  k.?...A..6..&...
+00002ce0: 5704 0692 2a4c b1d2 6775 5662 db68 015f  W...*L..guVb.h._
+00002cf0: 675c e436 e167 7556 e38d 2556 1893 c5cf  g\.6.guV..%V....
+00002d00: eaac c61a 0b3f 3b33 3f4b 9fd5 5989 6daf  .....?;3?K..Y.m.
+00002d10: 04ab 9d99 91dd 7de3 2bed 34de 5872 8511  ......}.+.4.Xr..
+00002d20: d9dd 38be d24e e38d 2557 9890 dd8d c3ae  ..8..N..%W......
+00002d30: add5 7863 0996 0e90 9560 098f 5d8a 9260  ..xc.....`..]..`
+00002d40: 61e2 35fe 82b1 1704 e54b b030 d80a 5f30  a.5......K.0.._0
+00002d50: f68a c040 8285 0956 fa82 d14a 7c35 9360  ...@...V...J|5.`
+00002d60: 6180 75c1 6071 1a6f 2cc1 c2cc eb82 c1e2  a.u.`q.o,.......
+00002d70: 34d6 5858 d899 c156 fa66 d34a ecd3 2e28  4.XX...V.f.J...(
+00002d80: eccc 5ceb 82c1 e234 de58 8285 b9d6 0583  ..\....4.X......
+00002d90: c569 bcb1 040b 73ad 0b06 8bd3 7863 0916  .i....s.....xc..
+00002da0: e45a 77e3 b8a7 d449 faea 2ad0 eb8c 6bd3  .Zw....I..*...k.
+00002db0: ee0e 71af d749 eca8 4608 d999 09d9 dd17  ..q..I..F.......
+00002dc0: 1e22 a3f1 c692 4f8c ceee c6f0 1019 8d37  ."....O........7
+00002dd0: 9680 62a4 96be 4476 12df eb15 d076 0ea9  ..b...Dv.....v..
+00002de0: d917 83f1 c48e 10b5 3313 b5f1 77c2 bd20  ........3...w.. 
+00002df0: 285f 9285 815a f84e b857 0406 9220 ccd3  (_...Z.N.W... ..
+00002e00: d2d7 ab56 62a3 5a28 db99 295b f665 891f  ...Vb.Z(..)[.e..
+00002e10: 6909 7b3b 337b 4b1f 975a 89cd 2d21 7267  i.{;3{K..Z..-!rg
+00002e20: 2672 576c 229c c61b 4bac 30a8 bb62 13e1  &rWl"...K.0..b..
+00002e30: 34de 5862 0557 a54d f435 ad95 d854 11d8  4.Xb.W.M.5...T..
+00002e40: 7766 d877 f785 2b6d 34de 5862 8529 e0dd  wf.w..+m4.Xb.)..
+00002e50: 18ae b4d1 5863 a183 6746 7d77 e3b8 3176  ....Xc..gF}w..1v
+00002e60: 1a6f 2ce9 c4a8 2f7d b86c 256e be7e 1638  .o,.../}.l%n.~.8
+00002e70: 7866 d097 bec9 7512 df70 081a 3c33 1a4c  xf....u..p..<3.L
+00002e80: dfc6 3a89 9f97 1262 78ee f05f 69b0 c263  ..:....bx.._i..c
+00002e90: 97a2 2487 10e8 cdf1 b7b1 bd20 285f e206  ..$........ (_..
+00002ea0: b1dd 0cdf c6f6 8ac0 4062 05f1 dc4c dfc6  ........@b...L..
+00002eb0: 5a89 6db0 84e8 9d71 45d8 8c9f c65a 8d37  Z.m....qE....Z.7
+00002ec0: 9658 41fe 37e3 97b1 5663 8d05 0c9e 110c  .XA.7...Vc......
+00002ed0: cef4 cda4 95d8 8643 78e1 19e1 df4c 5f34  .......Cx....L_4
+00002ee0: 3a89 7dc3 3c37 4995 4611 71f8 c677 d868  :.}.<7I.F.q..w.h
+00002ef0: 06c6 122b 0805 1fc6 f11d 369a 81b1 e40a  ...+......6.....
+00002f00: 42c1 993e e174 12fb 7e79 168c 7846 2438  B..>.t..~y..xF$8
+00002f10: d387 944e 62df 2fcf 0211 cf08 046f 8540  ...Nb./......o.@
+00002f20: 7618 897f 0d2b 08f1 8c3c f0e1 0b4f 166b  v....+...<...O.k
+00002f30: 06c6 125a c803 1fc6 f064 b166 602c a1d5  ...Z.....d.f`,..
+00002f40: 01c1 d262 212c bc19 d847 4860 e119 c9df  ...b!,...GH`....
+00002f50: fdcc a03f 6d34 0363 4927 5c22 f630 8e2f  ...?m4.cI'\".0./
+00002f60: a9d1 0c8c 259e 7889 d802 8b89 b324 dff9  ....%.x......$..
+00002f70: b780 c21c cfbc 402c fbb2 c477 b604 459e  ......@,...w..E.
+00002f80: 912b 3e2e 74dc ab35 9ac1 8596 7442 b078  .+>.t..5....tB.x
+00002f90: 3386 fb3b ee23 0974 3ce3 aab1 bb41 1c43  3..;.#.t<....A.C
+00002fa0: 46f2 682b a510 ca33 12ca 872f d419 d60c  F.h+...3.../....
+00002fb0: 8c25 8610 5d3e 8ce1 9ab2 6660 2c31 847c  .%..]>....f`,1.|
+00002fc0: f26e 1c37 7046 f268 1f21 419a 67e4 930f  .n.7pF.h.!A.g...
+00002fd0: dff8 4a1b cdc0 58d2 0901 e5c3 38be d246  ..J...X.....8..F
+00002fe0: 3330 9674 c2a5 6af3 1d0d 8d8c c40f 8d04  30.t..j.........
+00002ff0: 809e 1180 de7d e3ae 8491 0c68 1f21 a367  .....}.....h.!.g
+00003000: 24a3 77e3 1806 3192 01ed 23c4 f48c f8f3  $.w...1...#.....
+00003010: 6e1c 0fba 8dc4 cf9c 0931 3d23 fdbc fbc6  n........1=#....
+00003020: ed80 910c 2eb4 a416 b2cf bb6f 9c96 46e2  ...........o..F.
+00003030: a91b a1a5 e78e 7c96 2e4c 78ec 5294 c410  ......|..Lx.R...
+00003040: a2cc 1952 b713 f4e5 0be4 3c23 b19c 61f1  ...R......<#..a.
+00003050: 8b5e 1118 48ac 209a 9c69 f10b 2bb1 f92d  .^..H. ..i..+..-
+00003060: 34f3 8c34 73a6 2531 acc4 a699 40ce 3312  4..4s.%1....@.3.
+00003070: cb87 2f5c 52a3 f1c6 922a 482c 1fc6 717e  ../\R....*H,..q~
+00003080: 3b8d 3796 5441 6039 c3d2 20bd 2278 8424  ;.7.TA`9.. ."x.$
+00003090: 3e10 4cce b434 8893 f831 aeb0 cc33 82c9  >.L..4...1...3..
+000030a0: 872f dc4a d60c 8c25 3f90 4c3e 8ce1 9ab2  ./.J...%?.L>....
+000030b0: 6660 2c69 8334 f361 1c77 9c8d c61a 2f42  f`,i.4.a.w..../B
+000030c0: 392f 882c 675a 9bc5 49ec 74c2 2294 f382  9/.,gZ..I.t."...
+000030d0: c4f2 e11b de62 a719 1827 3136 5903 bd2d  .....b...'16Y..-
+000030e0: a719 1867 3136 59f3 108f 8d9c 6660 5cc4  ...g16Y.....f`\.
+000030f0: d864 4d3c 73e3 2476 e666 11c4 7941 5ef9  .dM<s.$v.f..yA^.
+00003100: f085 5bcc 9a81 7113 6317 5bf1 4b1d a719  ..[...q.c.[.K...
+00003110: 18cf 62ec 722b 7ea9 e334 03e3 458c 4d06  ..b.r+~..4..E.M.
+00003120: c5ae c3ce d022 34f3 8268 f256 3edc c861  ....."4..h.V>..a
+00003130: 6f68 116c 7941 0679 3708 5b1a 27b1 735e  oh.lyA.y7.[.'.s^
+00003140: 8b50 cb0b 22c8 876f 7c6a 4633 3096 1842  .P.."..o|jF30..B
+00003150: 06f9 308e 6f9a d10c 8c25 8690 41ce 7133  ..0.o....%..A.q3
+00003160: d30b 823b 2969 830b f86e e5c3 f51c be0d  ...;)i...n......
+00003170: 5b04 5a5e 105a de0d e051 6189 9d97 5804  [.Z^.Z...Qa...X.
+00003180: 665e 1066 3e7c e1d4 5833 3096 5441 62f9  f^.f>|..X30.TAb.
+00003190: 3086 4785 3503 6349 1524 9677 e3b8 6f60  0.G.5.cI.$.w..o`
+000031a0: 2476 5e62 11c8 7941 6079 f78d 1bac f16a  $v^b..yA`y.....j
+000031b0: c08b d0cc 0ba2 c987 437c 2f51 3395 f76e  ........C|/Q3..n
+000031c0: 80ba 08ce bc20 9a7c 18c7 f7b2 d304 e726  ..... .|.......&
+000031d0: c982 1072 9e60 a73c 27b1 1bc2 2ec2 2d2f  ...r.`.<'.....-/
+000031e0: c820 1b5f b3ad e22f d657 0207 d7f5 dd7d  . ._.../.W.....}
+000031f0: c32d e39c c42e 41b2 08e3 bc20 e36c 7c79  .-....A.... .l|y
+00003200: 73b3 775f acaf e410 b2cf 99d6 0974 123b  s.w_.........t.;
+00003210: a7b3 0812 bd20 df9c 69f5 4027 b173 678b  ..... ..i.@'.sg.
+00003220: 20d1 0be2 cd99 d676 7412 3b77 b608 11bd   ......vt.;w....
+00003230: 20dd 9c69 c547 27b1 7358 8b00 d10b d2cd   ..i.G'.sX......
+00003240: ec8b 92a9 d9ad 3d17 01a2 1784 9b77 df70  ......=......w.p
+00003250: aed0 49ec bbaa 4578 e805 d966 e38b afd5  ..I...Ex...f....
+00003260: da7b fb5c 090e bd20 dabc fb86 93c1 4e62  .{.\... ......Nb
+00003270: b776 5b84 865e 9086 36be 2849 3eaf 8491  .v[..^..6.(I>...
+00003280: 5e10 78de 7dc3 2f12 9dc4 ee79 b208 23bd  ^.x.}./....y..#.
+00003290: 20ef 6c7c 7153 84e4 7343 10e9 255c 2bf8   .l|qS..sC..%\+.
+000032a0: c560 b88c cf22 d0f3 8204 7386 998a f12a  .`..."....s....*
+000032b0: c28b c0cd 0bae 229c 612d 52ab 7017 4838  ......".a-R.p.H8
+000032c0: e805 39e8 4c0b 945a 89ed 560a 1fbd 201f  ..9.L..Z..V... .
+000032d0: 9d71 8152 abf1 c692 3408 4167 5c9f d46a  .q.R....4.Ag\..j
+000032e0: bcb1 440d 52d0 8771 3cec 721a 6f2c 5983  ..D.R..q<.r.o,Y.
+000032f0: 1874 8699 aef1 9ac5 8b10 d20b d2ce 5bf9  .t............[.
+00003300: 7023 8dc2 9e95 240a a2ce bb2b 3cb8 46e2  p#....$....+<.F.
+00003310: afa6 240a a2ce bb6f dc03 7212 3b1e 123a  ..$....o..r.;..:
+00003320: 7a41 d2f9 f085 eb6c 34de 5872 0949 e7c3  zA.....l4.Xr.I..
+00003330: 189e 20a3 b1c6 4247 2f48 3aef c671 9fcf  .. ...BG/H:..q..
+00003340: 49ec 3c9a c0d1 0b92 ce39 3d42 dfda 48de  I.<......9=B..H.
+00003350: db28 1638 7ae9 4867 69ab 9082 de82 c0f7  .(.8z.Hgi.......
+00003360: de05 835e c2f5 8e5f 1c28 6a66 dfda 0aee  ...^..._.(jf....
+00003370: bc18 dcb9 3f76 76d7 1e7c bf49 28e8 8529  ....?vv..|.I(..)
+00003380: e844 e34b 23f1 e35a a1a3 17a6 a369 3962  .D.K#..Z.....i9b
+00003390: 2719 dc31 491b 26a0 6929 5127 19dc 4949  '..1I.&.i)Q'..II
+000033a0: 1b06 a013 8db7 8cc4 8fb7 8499 5e98 7f4e  ............^..N
+000033b0: 34ee 3112 3fde 1264 7a61 fe39 d1f8 c348  4.1.?..dza.9...H
+000033c0: fcb8 4790 e985 f9e7 44e3 0023 f1f5 a849  ..G.....D..#...I
+000033d0: d634 ce13 ea8f 1b89 1f07 0831 bd30 fdcc  .4.........1.0..
+000033e0: be38 3f94 1eec 96e9 8b10 d34b 873f 4b34  .8?........K.?K4
+000033f0: 211a 3db5 77ff 660d 2499 3ace 590d 2882  !.=.w.f.$.:.Y.(.
+00003400: 16bf 9dfd 220c f4d2 01cd 6ac0 dbd9 fb9d  ....".....j.....
+00003410: 3817 a19d 978e 5c56 87f1 6049 f8e5 8559  8.....\V..`I...Y
+00003420: 6498 58ed 0441 f992 138c 22c3 dae7 56e1  d.X..A...."...V.
+00003430: 2e90 b0cb 0b73 c8b4 20ba 95d8 3ea7 a0cb  .....s.. ...>...
+00003440: 0b63 c819 681a 2bb1 3d30 2197 17c6 9033  .c..h.+.=0!....3
+00003450: 7c09 6825 b607 26e4 f282 18f2 e11b df5f  |.h%..&........_
+00003460: a7f1 c692 128c 2167 fa12 d06a bcb1 a407  ......!g...j....
+00003470: a3cb 193e c8b3 12f7 41de 2244 f3c2 7872  ...>....A."D..xr
+00003480: a66f d7ad c61b 4bd6 309e 9ce9 db75 abf1  .o....K.0....u..
+00003490: c692 4c8c 27ef c6f1 30dc 69bc b144 16f3  ..L.'...0.i..D..
+000034a0: c99b 71dc c570 92ea 7c05 695e 184f de7d  ..q..p..|.i^.O.}
+000034b0: e35b ec34 de58 528b f1e4 dd38 bec5 4ee3  .[.4.XR....8..N.
+000034c0: 8d25 b698 4fde 8de3 5bec 34de 5872 8b01  .%..O...[.4.Xr..
+000034d0: e5dd 38dc 17d2 6abc b1e4 1603 ca9b 71dc  ..8...j.......q.
+000034e0: 8d74 9266 7d25 b63a 3e59 7a0c cc2e 67ff  .t.f}%.:>Yz...g.
+000034f0: 3e42 d8e5 a503 91d5 8073 c8bf 0010 4879  >B.......s....Hy
+00003500: 61e2 98f6 2e70 123f b013 4879 c1e5 9977  a....p.?..Hy...w
+00003510: dfb8 4937 123f b013 a279 61a2 39d3 c0ce  ..I7.?...ya.9...
+00003520: 48fc c04e 48e7 25e4 96bf 1930 053d 1829  H..NH.%....0.=.)
+00003530: 0be9 bc74 d8b2 1ae0 a6db cd4f cf08 d2bc  ...t.......O....
+00003540: 84cb 2dbf 180c 9762 5e84 525e 9838 8626  ..-....b^.R^.8.&
+00003550: b713 04e5 4b1c 3058 0cbb 4df4 8ac0 40ea  ....K.0X..M...@.
+00003560: 3d43 c7b4 db84 95d8 8eb0 b0c8 0b83 c505  =C..............
+00003570: df1a 388d 3796 9860 b0b8 e05b 03a7 f1c6  ..8.7..`...[....
+00003580: 9213 0c16 177c 6be0 34de 5882 225c 28f9  .....|k.4.X."\(.
+00003590: c560 08da ac82 17af cc0a c7dd 8f5e 1094  .`...........^..
+000035a0: 3f49 f9d8 6980 0d36 7a45 6090 c400 3b07  ?I..i..6zE`...;.
+000035b0: b4c1 8695 b87b b00a 2dbc 76e4 ef79 0ffa  .....{..-.v..y..
+000035c0: 637f d8a0 8801 cf8a f4c7 feb0 4115 03ac  c...........A...
+000035d0: f5b4 4588 95b8 91eb 2af4 efca 246f 8566  ..E.....*...$o.f
+000035e0: dd49 fc14 fb2a f4ef da91 bc7a 4579 476c  .I...*.....zEyGl
+000035f0: db0c ad42 f9ae bc30 317d 55e5 24b6 015f  ...B...01}U.$.._
+00003600: 85fe 5d91 fe9d cae6 7b17 1b63 cf61 b62f  ..].....{..c.a./
+00003610: dc56 a182 d70e f195 2bca f8ef fce0 4f4d  .V......+.....OM
+00003620: f8df b563 79d5 01b3 6573 7033 6bab 80be  ...cy...esp3k...
+00003630: 6b07 edaa 0326 c5e6 e026 9257 217a 5726  k....&...&.W!zW&
+00003640: 7a67 7a2c c64c ef2a 4cef ca4c 2f3b 0c7b  zgz,.L.*L..L/;.{
+00003650: 15ab 40bd 2b13 ba33 f489 7b49 e020 b1c0  ..@.+..3..{I. ..
+00003660: 28ee 0cbd df5e 1238 48fd 67e6 7686 0d03  (....^.8H.g.v...
+00003670: 7a49 e020 01c0 4b08 dfc1 5e0b 2c59 7dee  zI. ..K...^.,Y}.
+00003680: 088f bb86 70ed 4bf9 54cf 57bf 94f6 2a38  ....p.K.T.W...*8
+00003690: eeda a1b5 62c0 ab08 fbef 5157 c16e 57c6  ....b.....QW.nW.
+000036a0: 6ef1 d618 890f 3061 7157 066b 67d8 5ec0  n.....0aqW.kg.^.
+000036b0: 4906 be12 09cc e262 8535 9281 af04 0583  I......b.5......
+000036c0: b558 8d8d 64e0 2bf1 c12c 2e56 6e23 19f8  .X..d.+..,.Vn#..
+000036d0: 4aa8 84ab 0abf 1870 e058 1062 15e8 76ed  J......p.X.b..v.
+000036e0: 085a 35e0 bc19 b480 82d7 ae1d 2bab 0e38  .Z5.........+..8
+000036f0: 9a18 b580 02d2 ae1d 15ab 0ea6 9be0 5b40  ..............[@
+00003700: 4166 5746 66f1 71ef 247d f20a 1cbb 32e9  AfWFf.q.$}....2.
+00003710: 8a0f 7627 091c 242a 1883 c547 b893 040e  ..v'..$*...G....
+00003720: 120a 4caf 6208 1a89 0f5f 015e 57a6 5731  ..L.b...._.^W.W1
+00003730: 04c7 cbff ae82 b6ae cca9 f2b5 1bf7 1e04  ................
+00003740: 625d 1962 e56b 37ee 3d08 aeba e2ea bc47  b].b.k7.=......G
+00003750: 271b 2c58 f3ee b3bd 3d12 0008 b73a 63d4  '.,X....=....:c.
+00003760: 549f 0b42 bdae ccb0 ce00 7cb0 643b 61f7  T..B......|.d;a.
+00003770: c1c8 2adc ebca 102b faa2 643b 5f9b 52c2  ..*....+..d;_.R.
+00003780: bdae ccb0 b2af 1b82 387c 6015 ee75 ed18  ........8|`..u..
+00003790: 5609 e0f0 d8a5 28c9 10a6 52e3 bd2b 7b41  V.....(...R..+{A
+000037a0: 50be 6405 03ab b077 65af 080c 242a 983f  P.d....we...$*.?
+000037b0: a5bd 2bad c4f6 1484 595d 1940 6db4 3a85  ..+.....Y].@m.:.
+000037c0: d5d8 1e84 40ab 2b13 a8c6 783c 2c11 3e75  ....@.+...x<,.>u
+000037d0: 65d6 b4d1 0218 bd26 b090 ac60 aab4 d1da  e......&...`....
+000037e0: f5bd a6b7 10e6 7445 8074 a5da c90a 4b17  ......tE.t....K.
+000037f0: ae42 9cae 8c8f d2f6 452c 19d9 4a24 2054  .B......E,..J$ T
+00003800: ca27 8bfd 93c1 2e51 ab60 a82b a2a6 e674  .'.....Q.`.+...t
+00003810: 4de4 0c8c 2558 9041 cdb4 3d95 930c 6605  M...%X.A..=...f.
+00003820: 055b 5d91 419d e8f3 3527 f183 76c1 56d7  .[].A...5'..v.V.
+00003830: 7089 de17 8371 d744 48d4 95b1 d278 9ba8  p....q.DH....x..
+00003840: 5e10 942f f9c1 f828 6c13 d52b 0203 498f  ^../...(l..+..I.
+00003850: 8e13 d56b c1bd 101f b2c2 90ae 1d10 2a06  ...k..........*.
+00003860: 088b 4eed bdad af02 8bae 1df9 a906 6672  ..N...........fr
+00003870: c3b6 4f4d 02a1 9999 0a68 179d c45f 3909  ..OM.....h..._9.
+00003880: 04a6 42d9 97bf 1a1e 5c50 c903 0385 f6c7  ..B.....\P......
+00003890: 64d4 637b 7b02 85ae bcf8 ed1c 2fce d42b  d.c{{......./..+
+000038a0: fa87 5aa0 d095 57b9 9d61 7126 27f1 1306  ..Z...W..aq&'...
+000038b0: 828a aebc c82d fbb2 c427 b870 a52b 73a5  .....-...'.p.+s.
+000038c0: ec8b c394 f6de 71cb abf0 a62b d3a3 332d  ......q....+..3-
+000038d0: 46d5 6bfa 5b29 70e9 caa4 e84c cb4e 398d  F.k.[)p....L.N9.
+000038e0: 7f48 852e 5d19 159d 69d9 a95e 139c 9b04  .H..]...i..^....
+000038f0: 0b53 a1bb 4508 4639 8d1f 5e0a 49ba 3215  .S..E.F9..^.I.2.
+00003900: ba19 c75d 8d4e 129c 9a64 08e3 9f73 bc05  ...].N...d...s..
+00003910: 71af 080c 2443 98f3 9c61 9358 27b1 9f41  q...$C...a.X'..A
+00003920: ad82 86ae 8c79 b2af 8916 5bd5 840c 5d99  .....y....[...].
+00003930: f264 5f9c 02a9 beaf 2460 e8ca 90e7 0c9b  .d_.....$`......
+00003940: e23a 891f 980b 17ba 32e4 39c3 a6b8 4ee2  .:......2.9...N.
+00003950: ab86 70a1 2b33 9e15 e06e 2bb1 cf95 60a1  ..p.+3...n+...`.
+00003960: ab41 3ce1 f33a 27f1 f757 a8d0 b523 3ca5  .A<..:'..W...#<.
+00003970: b10f 8f5d 8a92 5461 6633 ded9 b017 04e5  ...]..Taf3......
+00003980: 4ba6 309b 093b 1bf6 8ac0 4032 85d9 4cda  K.0..;....@2..L.
+00003990: d9d0 4a6c 0753 70ce 9591 4ddc d9d0 6aec  ..Jl.Sp...M...j.
+000039a0: b6e6 ab70 9e2b 439b b8b5 a1d5 d86d cd57  ...p.+C......m.W
+000039b0: 213d 57c6 3669 6f43 2bb1 9d6a 213d 57c6  !=W.6ioC+..j!=W.
+000039c0: 3671 6f43 abb1 6b0a acc2 7aae cc73 e2e6  6qoC..k...z..s..
+000039d0: 8656 633f 0a5f 0502 5d79 ed5a da64 d04a  .Vc?._..]y.Z.d.J
+000039e0: 6ca6 091b baf2 dab5 0b7d b062 35f6 93a4  l........}.b5...
+000039f0: 5550 d295 51d2 85be 58b1 9aab e4e2 2c21  UP..Q...X.....,!
+00003a00: c590 e942 9b57 59cd 5572 7196 f462 9474  ...B.WY.Urq..b.t
+00003a10: 778e 7b93 4e73 955c 9c25 bf98 255d a8ed  w.{.Ns.\.%..%]..
+00003a20: 3292 7bdf 7809 7fba 324b cac6 2429 1e8f  2.{.x...2K..$)..
+00003a30: 5f05 3f5d 1925 a59d 1e9d 6430 6326 f8e9  _.?].%....d0c&..
+00003a40: 6af0 d3f8 d89b a2a6 3be1 4f8f 7fc0 9f14  j.......;.O.....
+00003a50: 6ff6 1828 228b 492d 3046 60bf c740 1279  o..(".I-0F`..@.y
+00003a60: 24f5 c0c4 a0ad 1703 4d64 92d5 04c3 61a5  $.......Md....a.
+00003a70: 26da 8b6c 1bbd 498b 9a63 3eac d44a 7b91  &..l..I..c>..J{.
+00003a80: 6da6 3769 5573 8c88 9550 6b2f ba6a aee6  m.7iUs...Pk/.j..
+00003a90: 4dcd 3126 687b cb40 13dd db59 4d30 4570  M.1&h{.@...YM0Ep
+00003aa0: 2f4b 2fb2 7d82 4dba a839 e602 ee67 e945  /K/.}.M..9...g.E
+00003ab0: b65b b049 5735 c78e cd4a af8e bce8 aab9  .[.IW5...J......
+00003ac0: 984f 1a3f 4ca9 eee6 617b e545 57cd d55c  .O.?L...a{.EW..\
+00003ad0: 8389 01d6 ddfc 09cc 8de8 aab9 9a6b 6231  .............kb1
+00003ae0: db4a fb3d 5a8d 6f3f 36a9 0619 13b1 b4e7  .J.=Z.o?6.......
+00003af0: a3d5 f8d7 4c9b 5473 8c59 59e3 4d9a 923d  ....L.Ts.YY.M..=
+00003b00: 67b5 4935 c698 a25d e15d 93d5 dcdb 49e1  g.I5...].]....I.
+00003b10: 4daa 29c6 7c2d bd52 b41a bf76 c126 d570  M.).|-.R...v.&.p
+00003b20: 0b31 da57 1313 6276 a674 936a 8875 24ed  .1.W..bv.t.j.u$.
+00003b30: 1b93 e10b a9ed 379a 4ac8 cd96 784f cf40  ......7.J...xO.@
+00003b40: 1158 24cd 1e24 670b 6e42 e945 8316 3569  .X$..$g.nB.E..5i
+00003b50: f620 3e5b 604f d140 129d a046 0ca2 b285  . >[`O.@...F....
+00003b60: b615 0d34 9189 6609 72b1 05f7 10f5 a241  ...4..f.r......A
+00003b70: a728 6998 201c 7b98 43db e544 8324 4b9a  .(i. .{.C..D.$K.
+00003b80: 2648 c816 da4b 34d0 4497 5763 0329 d9c3  &H...K4.D.Wc.)..
+00003b90: 842e afcb 0d37 fbba 4935 3790 a03d cca9  .....7..I57..=..
+00003ba0: 8618 919b a1d9 941a 27c8 d696 3b18 d659  ........'...;..Y
+00003bb0: 8d1f 506e 520d 1fa4 6e0b 7d48 6435 a3b6  ..PnR...n.}Hd5..
+00003bc0: 396b 2a21 ab5b 68d3 31ab 193d d159 4309  9k*!.[h.1..=.YC.
+00003bd0: 29de 421b 8f59 cda8 7dcc 1a56 21ac fb6a  ).B..Y..}..V!..j
+00003be0: f207 5229 6b2a 2198 5b28 923a 4564 a1d9  ..R)k*!.[(.:Ed..
+00003bf0: 83d8 6e81 0daa 0249 e4a1 1183 e06e a13d  ..n....I.....n.=
+00003c00: aa02 4d64 a211 83ec ee61 42a7 6244 83c1  ..Md.....aB.bD..
+00003c10: 5dd6 8841 44f7 3087 8871 2237 e1be 2935  ]..AD.0..q"7..)5
+00003c20: 6290 d22d b413 97d7 0c5a aeac 1183 a46e  b..-.....Z.....n
+00003c30: c1dd b8bc 68d0 f928 9a31 88eb 16dc 91cb  ....h..(.1......
+00003c40: 8b7c ae17 cd18 4476 776f c818 a719 8cb3  .|....Dvwo......
+00003c50: 8b66 0c2e 567b 78d3 791b d160 9c5d 3492  .f..V{x.y..`.]4.
+00003c60: 100d 3ecc e18e 3b91 9b82 df94 9a55 880d  ..>...;......U..
+00003c70: 1fde 30cc 7622 3b0b bf49 35c4 900f 3ecc  ..0.v";..I5...>.
+00003c80: a193 e644 8326 ad68 b875 8cb0 362b 0810  ...D.&.h.u..6+..
+00003c90: ef67 3830 d110 0b79 e057 1313 5676 627f  .g80...y.W..Vvb.
+00003ca0: 936a 5a21 455c a647 6a9c 8de6 deae 34b3  .jZ!E\.Gj.....4.
+00003cb0: 4935 ad10 2f2e 0469 5acd a843 5435 ac90  I5../..iZ..CT5..
+00003cc0: 222e b49f 83d5 8cac 35ab 9024 2eb4 a583  ".......5..$....
+00003cd0: d50c 9edb aa51 6556 bc85 83d7 d234 7b90  .....QeV.....4{.
+00003ce0: 112e d4d4 84eb e15e 2d34 6290 062e b046  .......^-4b....F
+00003cf0: 7b20 893c 3449 10fc 2db8 32ba 170d 5aec  { .<4I..-.2...Z.
+00003d00: aa49 828b d616 5a0e de6b 7c47 a56a be20  .I....Z..k|G.j. 
+00003d10: 605c 7061 762f 1a74 16aa e60e d2c7 0517  `\pav/.t........
+00003d20: 67f7 a241 f7b0 6af0 207d 7c98 43c3 e544  g..A..j. }|.C..D
+00003d30: 57cd c5bc 69f2 2099 bc9b 43f5 0f49 e7ab  W...i. ...C..I..
+00003d40: 8966 0cd2 c987 093c d34e 34e8 1035 4d99  .f.....<.N4..5M.
+00003d50: 867d 9bc4 1d41 271a 7488 9a86 1272 ca87  .}...A'.t....r..
+00003d60: 393c 5846 3448 f6a6 6985 08b3 f536 a2c1  9<XF4H..i....6..
+00003d70: 4b8f a631 86e8 f361 0e0f b513 0d5e 7a34  K..1...a.....^z4
+00003d80: 8d31 649c 0f73 78e9 e144 8397 1e4d 830c  .1d..sx..D...M..
+00003d90: 41e7 dd1c fa11 e3e5 75b7 df68 6021 d57c  A.......u..h`!.|
+00003da0: 9850 8d32 a2d1 83a5 8185 34f4 614e 35ca  .P.2......4.aN5.
+00003db0: 8806 9d86 5903 0b99 e7c3 1c9e 6a23 1a79  ....Y.......j#.y
+00003dc0: 6b8e 212a bd79 c369 8f49 e9ed 371a 57c8  k.!*.y.i.I..7.W.
+00003dd0: 3def 1ed0 041b 8d5d c760 536a 5821 2d5d  =......].`SjX!-]
+00003de0: d223 7505 8de6 de72 269b 54c3 0a39 eabd  .#u....r&.T..9..
+00003df0: e74f a76d b26a 3015 3a6b 5621 2f5d 68c7  .O.m.j0.:kV!/]h.
+00003e00: 07ab 197a 6b54 2133 edce db0c e946 de9a  ...zkT!3.....F..
+00003e10: 54c8 4dbb f336 23bd 91b7 0618 b2d3 8576  T.M..6#........v
+00003e20: 36b0 9ac1 9bc2 59e3 abc3 a775 d881 6cf5  6.....Y....u..l.
+00003e30: 1e53 befd 5b34 a690 952e b463 84d5 8cac  .S..[4.....c....
+00003e40: 35a5 1097 76d6 26d9 26df f82d 9a5e b88e  5...v.&.&..-.^..
+00003e50: aef3 fe03 23bd 4573 0af9 eba3 c30c cdfb  ....#.Es........
+00003e60: 98c1 de7e a389 8414 f65e 33e1 0965 cde8  ...~.....^3..e..
+00003e70: 095d 3490 10b6 3695 c368 46d6 9a47 885b  .]4...6..hF..G.[
+00003e80: 3b6b d68c ac35 8e90 b7b6 b7f5 0ff4 9c16  ;k...5..........
+00003e90: 0d1e 84ab adcb 1f78 b5bf 68c6 7424 b566  .......x..h.t$.f
+00003ea0: 4c78 f052 daaa 6182 7474 a1ae 5eb8 deee  Lx.R..a.tt..^...
+00003eb0: d542 4303 39e8 023b 2a04 92c8 43c3 0191  .BC.9..;*...C...
+00003ec0: e742 fb27 788d efda ac1a 19c8 3c1f d674  .B.'x.......<..t
+00003ed0: 8246 3498 5559 3549 107b 3ecc a1e3 e844  .F4.UY5I.{>....D
+00003ee0: 83a9 8d55 b304 c967 6b6e 4483 0ef3 aa69  ...U...gknD....i
+00003ef0: 82f4 b335 6791 dde9 7253 6a9c 1800 9ae7  ...5g...rSj.....
+00003f00: 749c 6830 a7b3 6aca 2005 5d68 cb0e af19  t.h0..j. .]h....
+00003f10: e4e8 aad9 d3f1 d16f bce9 5967 915d 5162  .......o..Yg.]Qb
+00003f20: 9a14 b59e 10b5 3ebc e31b 6e45 9ece 9a14  ......>...nE....
+00003f30: c29e 10c2 2eb4 5f49 a0e9 436c 520a 7b42  ......_I..ClR.{B
+00003f40: 0abb e0e6 2456 64b7 18da 9459 bd5d 8aa1  ....$Vd....Y.]..
+00003f50: b759 d4cf 8ffa 2785 b327 e4ac 0b6e 8e62  .Y....'..'...n.b
+00003f60: 450f 3e48 2685 b327 e4ac adb9 f90e 7664  E.>H&..'......vd
+00003f70: ded4 dca5 588c 353a 8d1f 924f 8a6c 4f48  ....X.5:...O.lOH
+00003f80: 5f17 da35 c46a eca2 839b 7251 6b13 4774  _..5.j....rQk.Gt
+00003f90: c1c7 dda4 49b9 ec09 11eb dd03 da07 27ba  ....I.........'.
+00003fa0: f996 7152 2e7b 42c4 da99 1bd1 cd37 1093  ..qR.{B......7..
+00003fb0: 72d9 1322 d687 79dc 3af5 a2e0 fa2a 803d  r.."..y.:....*.=
+00003fc0: 214c 7db8 c4b3 b04e 74f3 63c1 4909 ec09  !L}....Nt.c.I...
+00003fd0: 696a 6bce a2db 64b1 be49 11ec c9e0 d4c6  ijk...d..I......
+00003fe0: 9c45 b7c9 7dc1 be49 35ad 90a7 b6e6 2cba  .E..}..I5.....,.
+00003ff0: 4dbe 0956 087b 42a0 da9a b3e8 36d9 4ed7  M..V.{B.....6.N.
+00004000: a414 f684 a0f5 610e 2d94 11dd 7c3f 7b52  ......a.-...|?{R
+00004010: 3a7b c275 8e0f f39f c0fc 0f64 9652 db93  :{.u.......d.R..
+00004020: 5909 3938 a8a7 62fb 7093 72db 9359 0d39  Y.98..b.p.r..Y.9
+00004030: 38a8 266e 4bc4 4daa 1914 c2d6 af26 1c50  8.&nK.M......&.P
+00004040: b7e9 afde 4423 2884 ad5f 4d38 6afc 64e2  ....D#(.._M8j.d.
+00004050: a47c f6c4 a835 ede2 6335 835e 91d2 d913  .|...5..c5.^....
+00004060: 83d6 b491 8fd5 0ce6 1827 85b3 a710 b47e  .........'.....~
+00004070: 35e1 38b1 8b71 6c4a 4d13 c6ac 33cd 82b1  5.8..qlJM...3...
+00004080: 66ef f40d ce4f c384 296b daac c86a 86de  f....O..)k...j..
+00004090: 9a25 6649 e4e0 e01f bfb6 9a24 6651 e4e0  .%fI.......$fQ..
+000040a0: a078 f84e 8ea2 d653 b8c6 f18b 0733 d5d9  .x.N...S.....3..
+000040b0: 0f38 2745 aaa7 7095 e357 0f9e 591e 7968  .8'E..p..W..Y.yh
+000040c0: 8c38 74ba 3fa8 59e5 c757 4a54 4f21 1ffd  .8t.?.Y..WJTO!..
+000040d0: 6ae2 30c5 f04c deff f6f3 d3d3 d77f bcff  j.0..L..........
+000040e0: 7aff e30f bfde 7f78 fa5f f7cf 1f3e fef2  z......x._...>..
+000040f0: db77 9f9e 7eda 0aba fbbb fd1d d2f3 c70f  .w..~...........
+00004100: 3fbf fee3 eb97 5fb7 bfe9 fbef 1ebe 7cfd  ?....._.......|.
+00004110: fae5 f3f1 9f3f 3fdd 3f3e 3def 3fd8 8eff  .....??.?>=.?...
+00004120: f4e5 cbd7 d77f eccd d4ef 5f9e ff7a 98fc  .........._..z..
+00004130: f8ff 0150 4b03 0414 0000 0008 00e2 54a7  ...PK.........T.
+00004140: 58f7 f68f 09a7 0200 006d 0b00 000d 0000  X........m......
+00004150: 0078 6c2f 7374 796c 6573 2e78 6d6c dd56  .xl/styles.xml.V
+00004160: db8e 9b30 10fd 15c4 0794 4d50 51a8 42a4  ...0......MPQ.B.
+00004170: 36d2 4a95 da6a a5dd 87be 9a60 8225 5fa8  6.J..j.....`.%_.
+00004180: 31ab 64bf be33 b613 92ec 0edd f6b1 a084  1.d..3..........
+00004190: f11c 9fb9 3b64 3db8 a3e4 8f1d e72e 3928  ....;d=.......9(
+000041a0: a987 2aed 9ceb 3f65 d9b0 ebb8 62c3 07d3  ..*...?e....b...
+000041b0: 730d 486b ac62 0e96 769f 0dbd e5ac 1990  s.Hk.b..v.......
+000041c0: a464 b6bc bb2b 32c5 844e 376b 3daa 7be5  .d...+2..N7k=.{.
+000041d0: 8664 6746 edaa f42e 4db2 cdba 357a 522d  .dgF....M...5zR-
+000041e0: d3a0 80bd 4cf1 e499 c92a dd32 296a 2bc2  ....L....*.2)j+.
+000041f0: 66a6 843c 06fd d26b 7646 1a9b 3888 8657  f..<...kvF..8..W
+00004200: e9c2 ab86 97b0 6111 9718 6ab4 a584 36d6  ......a...j...6.
+00004210: 6bb3 e026 7cd7 9170 89f8 c700 3b84 94d7  k..&|..p....;...
+00004220: f181 62b3 ee99 73dc ea7b 5804 92d7 bec6  ..b...s..{X.....
+00004230: a2fc 74ec 21be bd65 c7c5 f263 7ac1 f00f  ..t.!..e...cz...
+00004240: 7053 1bdb 707b e528 a836 6bc9 5b87 0c2b  pS..p{.(.6k.[..+
+00004250: f69d 179c e9f1 511b e78c 42a9 116c 6f34  ......Q...B..lo4
+00004260: 0b91 9c68 5774 dfc8 2a75 1d34 62b2 75ab  ...hWt..*u.4b.u.
+00004270: 45c3 b7ba e8e5 567d 7613 0548 61c7 a57c  E.....V}v..Ha..|
+00004280: c46d 3fdb 731e 0bc8 e3d0 26a1 f35f 1bdf  .m?.s.....&.._..
+00004290: 742c ec49 84e4 a318 ccc4 053a b834 178c  t,.I.......:.4..
+000042a0: 5fd8 5dfe 9bdd 5e3c 1bf7 6584 8cb4 5fff  _.]...^<..e..._.
+000042b0: 1a8d e30f 96b7 e2e0 d787 760a 8032 bf20  ..........v..2. 
+000042c0: cc83 9ef5 bd3c 7e96 62af 150f d9bf dbe3  .....<~.b.......
+000042d0: 66cd 4ebc a433 56bc 8037 9cc9 1d28 388c  f.N..3V..7...(8.
+000042e0: ec33 b74e ec50 034d 0a05 3ab4 b14a e702  .3.N.P.M..:..J..
+000042f0: f972 5dd5 feac 4df0 4055 e90f 3ca8 f222  .r]...M.@U..<.."
+00004300: d17a 14d2 091d 579d 681a ae5f b700 ec3b  .z....W.h.._...;
+00004310: 56c3 4fc1 9503 d8d5 f096 8dd2 3d9d c12a  V.O.........=..*
+00004320: 9de4 efbc 11a3 2acf bb1e b016 71d7 247f  ......*.....q.$.
+00004330: c351 5c14 d369 0667 4237 fcc0 9b6d 5cda  .Q\..i.gB7...m\.
+00004340: 7ded c504 0470 1baf 30c8 37d0 bdbf 0888  }....p..0.7.....
+00004350: 6405 9080 1024 7d91 6190 acc0 237d fd8f  d....$}.a...#}..
+00004360: 79ad e8bc 0248 46b8 7a1b 5ad1 ac15 cd0a  y....HF.z.Z.....
+00004370: bc37 a1ad bf49 5f04 ab84 8b48 b92c f3bc  .7...I_....H.,..
+00004380: 28c8 f26e b76f 87b1 256b 5814 f821 0c92  (..n.o..%kX..!..
+00004390: 1122 87f4 85de feb6 f233 0330 3336 7f98  .".......3.036..
+000043a0: 0db2 cbb3 6343 a63c 33a2 64ca 3395 4788  ....cC.<3.d.3.G.
+000043b0: a821 72ca 9218 00d2 1772 c8a6 9013 8541  .!r......r.....A
+000043c0: 10be 70d4 0856 9e63 9fc9 08c9 633e 0395  ..p..V.c....c>..
+000043d0: 2509 e190 12d3 5b14 54a1 0abc 897e 9187  %.....[.T....~..
+000043e0: 28cf cb92 8010 24c2 c873 12c2 033b 0391  (.....$..s...;..
+000043f0: 6160 2024 94e7 e145 7af3 3ecb 4eef b96c  a` $...Ez.>.N..l
+00004400: fa83 bdf9 0d50 4b03 0414 0000 0008 00e2  .....PK.........
+00004410: 54a7 58b7 47eb 8ac0 0000 0016 0200 000b  T.X.G...........
+00004420: 0000 005f 7265 6c73 2f2e 7265 6c73 9d92  ..._rels/.rels..
+00004430: 4b6e 0231 0c40 af12 655f 4ca9 c402 31ac  Kn.1.@..e_L...1.
+00004440: d8b0 4388 0bb8 89e7 a399 c491 63c4 f4f6  ..C.........c...
+00004450: 8dd8 c020 6811 4bff 9e9e 2daf 0f34 a076  ... h.K...-..4.v
+00004460: 1c73 dba5 6cc6 30c4 5cd9 5635 ad00 b26b  .s..l.0.\.V5...k
+00004470: 2960 9e71 a258 2a35 4b40 2da1 3490 d0f5  )`.q.X*5K@-.4...
+00004480: d810 2ce6 f325 c82d c36e d6b7 4c73 fc49  ..,..%.-.n..Ls.I
+00004490: f40a 91eb ba73 b465 770a 14f5 01f8 aec3  .....s.ew.......
+000044a0: 9a23 4a43 5ad9 7180 334b ffcd dccf 0ad4  .#JCZ.q.3K......
+000044b0: 9a9d afac ecfc a735 f0a6 ccf3 f520 90a2  .......5..... ..
+000044c0: 4745 702c f491 a44c 8b76 94af 3e9e ddbe  GEp,...L.v..>...
+000044d0: a4f3 a563 62b4 78df e8ff f3d0 a814 3df9  ...cb.x.......=.
+000044e0: bf9d 30a5 89d2 d745 0926 6fb0 f905 504b  ..0....E.&o...PK
+000044f0: 0304 1400 0000 0800 e254 a758 f675 01aa  .........T.X.u..
+00004500: 3001 0000 2902 0000 0f00 0000 786c 2f77  0...).......xl/w
+00004510: 6f72 6b62 6f6f 6b2e 786d 6c8d 90d1 4ec3  orkbook.xml...N.
+00004520: 300c 457f a5ca 07d0 6e82 494c eb5e 9880  0.E.....n.IL.^..
+00004530: 4908 1043 7bcf 5a77 b596 c495 e36e b0af  I..C{.Zw.....n..
+00004540: 2749 294c e285 27c7 d7d6 c9bd 5e9c 880f  'I)L..'.....^...
+00004550: 3ba2 43f6 618d f373 2e55 2bd2 cdf3 dc57  ;.C.a..s.U+....W
+00004560: 2d58 edaf a803 1766 0db1 d512 5ade e7d4  -X.....f....Z...
+00004570: 3458 c18a aade 8293 7c5a 14b3 9cc1 6841  4X......|Z....hA
+00004580: 72be c5ce ab81 f61f 96ef 1874 ed5b 00b1  r..........t.[..
+00004590: 6640 598d 4e2d 17a3 b357 cef2 cb8e 04aa  f@Y.N-...W......
+000045a0: f853 54a3 b245 38f9 df85 d866 47f4 b843  .ST..E8....fG..C
+000045b0: 83f2 59aa f436 a032 8b0e 2d9e a12e 55a1  ..Y..6.2..-...U.
+000045c0: 32df d2e9 9118 cfe4 449b 4dc5 644c a926  2.......D.M.dL.&
+000045d0: c360 0b2c 58fd 9137 d1e6 bbde f9a4 88de  .`.,X..7........
+000045e0: bdc5 cca5 9a15 01d8 207b 491b 89af 83c9  ........ {I.....
+000045f0: 2384 e5a1 eb85 eed1 08f0 4a0b 3c30 f51d  #.........J.<0..
+00004600: ba7d c284 18f9 458e 748a b166 4e5b 2855  .}....E.t..fN[(U
+00004610: a226 0fa1 aeeb c18f 04d0 453a 9e63 18f0  .&........E:.c..
+00004620: bafe 468e 9c1a 1a74 503f 0790 8f83 90aa  ..F....tP?......
+00004630: 0a27 8d25 91a6 d737 93db e0be 37e6 2e68  .'.%...7....7..h
+00004640: 2fee 8974 fd63 6cbc eaf2 0b50 4b03 0414  /..t.cl....PK...
+00004650: 0000 0008 00e2 54a7 5833 ebe3 baad 0000  ......T.X3......
+00004660: 00fb 0100 001a 0000 0078 6c2f 5f72 656c  .........xl/_rel
+00004670: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
+00004680: 656c 73b5 913d 0e83 300c 85af 12e5 0018  els..=..0.......
+00004690: a8d4 a102 a62e ac15 1788 82f9 1181 44b1  ..............D.
+000046a0: abc2 ed1b c100 481d ba30 59cf 96bf f764  ......H..0Y....d
+000046b0: 672f 348a 7b3b 51d7 3b12 f368 26ca 65c7  g/4.{;Q.;..h&.e.
+000046c0: ec1e 00a4 3b1c 1545 d6e1 1426 8df5 a3e2  ....;..E...&....
+000046d0: 207d 0b4e e941 b508 691c dfc1 1f19 b2c8   }.N.A..i.......
+000046e0: 8e4c 512d 0eff 21da a6e9 353e ad7e 8f38  .LQ-..!...5>.~.8
+000046f0: f10f 307c ac1f a843 6429 2ae5 5be4 5cc2  ..0|...Cd)*.[.\.
+00004700: 6cf6 36c1 5a92 2890 a528 eb5c fab2 4ea4  l.6.Z.(..(.\..N.
+00004710: 80cb 1211 2f06 698f b3e9 937f 7aa5 3f87  ..../.i.....z.?.
+00004720: 5ddc ed57 b935 cf47 b8ad 21e0 f4eb e20b  ]..W.5.G..!.....
+00004730: 504b 0304 1400 0000 0800 e254 a758 9b86  PK.........T.X..
+00004740: 4284 1b01 0000 d703 0000 1300 0000 5b43  B.............[C
+00004750: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
+00004760: 6cad 93cf 4ec3 300c c65f a5ea 756a 3338  l...N.0.._..uj38
+00004770: 7040 eb2e 8c2b ecc0 0b84 c45d a3e6 9f62  p@...+.....]...b
+00004780: 6f74 6f8f dbb2 4aa0 b10d 954b a3c6 f6f7  oto...J....K....
+00004790: 73fc 25ab b763 04cc 3a67 3d56 7943 141f  s.%..c..:g=VyC..
+000047a0: 8540 d580 9358 8608 9e23 7548 4e12 ffa6  .@...X...#uHN...
+000047b0: 9d88 52b5 7207 e27e b97c 102a 7802 4f05  ..R.r..~.|.*x.O.
+000047c0: f51a f97a b581 5aee 2d65 cf1d 6fa3 09be  ...z..Z.-e..o...
+000047d0: ca13 58cc b3a7 31b1 6755 b98c d11a 2589  ..X...1.gU....%.
+000047e0: e3e2 e0f5 0f4a f145 28b9 72c8 c1c6 445c  .....J.E(.r...D\
+000047f0: 7042 9e89 b388 21f4 2be1 54f8 7a80 948c  pB....!.+.T.z...
+00004800: 866c 2b13 bd48 c769 a2b3 02e9 6801 cbcb  .l+..H.i....h...
+00004810: 1a67 ba0c 756d 14e8 a0f6 8e4b 4a8c 09a4  .g..um.....KJ...
+00004820: c606 809c 2d47 d1c5 1534 f190 61fc decd  ....-G...4..a...
+00004830: 6e60 90b9 48e4 d46d 0a11 d9b5 047f e79d  n`..H..m........
+00004840: 6ce9 ab8b c842 90c8 5c39 e484 64ed d927  l....B..\9..d..'
+00004850: 84de 710d fa56 384f f823 a476 f004 c5b0  ..q..V8O.#.v....
+00004860: cc1f f377 9f27 fd5b 1a79 0fa1 fdef 7bd6  ...w.'.[.y....{.
+00004870: afa5 93c6 4f0d 88e1 3daf 3f01 504b 0102  ....O...=.?.PK..
+00004880: 1403 1400 0000 0800 e254 a758 465a c10c  .........T.XFZ..
+00004890: 8200 0000 b100 0000 1000 0000 0000 0000  ................
+000048a0: 0000 0000 8001 0000 0000 646f 6350 726f  ..........docPro
+000048b0: 7073 2f61 7070 2e78 6d6c 504b 0102 1403  ps/app.xmlPK....
+000048c0: 1400 0000 0800 e254 a758 3afa b57b eb00  .......T.X:..{..
+000048d0: 0000 cb01 0000 1100 0000 0000 0000 0000  ................
+000048e0: 0000 8001 b000 0000 646f 6350 726f 7073  ........docProps
+000048f0: 2f63 6f72 652e 786d 6c50 4b01 0214 0314  /core.xmlPK.....
+00004900: 0000 0008 00e2 54a7 5899 5c9c 2310 0600  ......T.X.\.#...
+00004910: 009c 2700 0013 0000 0000 0000 0000 0000  ..'.............
+00004920: 0080 01ca 0100 0078 6c2f 7468 656d 652f  .......xl/theme/
+00004930: 7468 656d 6531 2e78 6d6c 504b 0102 1403  theme1.xmlPK....
+00004940: 1400 0000 0800 e254 a758 8889 ce2f f238  .......T.X.../.8
+00004950: 0000 f0f2 0100 1800 0000 0000 0000 0000  ................
+00004960: 0000 8081 0b08 0000 786c 2f77 6f72 6b73  ........xl/works
+00004970: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
+00004980: 504b 0102 1403 1400 0000 0800 e254 a758  PK...........T.X
+00004990: f7f6 8f09 a702 0000 6d0b 0000 0d00 0000  ........m.......
+000049a0: 0000 0000 0000 0000 8001 3341 0000 786c  ..........3A..xl
+000049b0: 2f73 7479 6c65 732e 786d 6c50 4b01 0214  /styles.xmlPK...
+000049c0: 0314 0000 0008 00e2 54a7 58b7 47eb 8ac0  ........T.X.G...
+000049d0: 0000 0016 0200 000b 0000 0000 0000 0000  ................
+000049e0: 0000 0080 0105 4400 005f 7265 6c73 2f2e  ......D.._rels/.
+000049f0: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
+00004a00: e254 a758 f675 01aa 3001 0000 2902 0000  .T.X.u..0...)...
+00004a10: 0f00 0000 0000 0000 0000 0000 8001 ee44  ...............D
+00004a20: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
+00004a30: 6c50 4b01 0214 0314 0000 0008 00e2 54a7  lPK...........T.
+00004a40: 5833 ebe3 baad 0000 00fb 0100 001a 0000  X3..............
+00004a50: 0000 0000 0000 0000 0080 014b 4600 0078  ...........KF..x
+00004a60: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+00004a70: 2e78 6d6c 2e72 656c 7350 4b01 0214 0314  .xml.relsPK.....
+00004a80: 0000 0008 00e2 54a7 589b 8642 841b 0100  ......T.X..B....
+00004a90: 00d7 0300 0013 0000 0000 0000 0000 0000  ................
+00004aa0: 0080 0130 4700 005b 436f 6e74 656e 745f  ...0G..[Content_
+00004ab0: 5479 7065 735d 2e78 6d6c 504b 0506 0000  Types].xmlPK....
+00004ac0: 0000 0900 0900 3e02 0000 7c48 0000 0000  ......>...|H....
```

### Comparing `veg2hab-0.2.2a1/veg2hab/package_data/veg2hab.pyt` & `veg2hab-0.2.3a0/veg2hab/package_data/toolbox.pyt`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Type, Union
 
 import veg2hab.io.arcgis
 import veg2hab.main
 import veg2hab.constants
 import logging
 
-SUPPORTED_VERSIONS = ["0.2.2a1"]
+SUPPORTED_VERSIONS = ["0.1.0", "0.1.1", "0.2.1", "0.2.3a0"]
 
 # this instantiates the arcgis interface and configures the logging
 veg2hab.io.arcgis.ArcGISInterface.get_instance().instantiate_loggers()
 
 class Toolbox:
     def __init__(self):
         """Define the toolbox (the name of the toolbox is the name of the
@@ -42,27 +42,37 @@
         """Set whether the tool is licensed to execute."""
         return True
 
     def updateParameters(self, parameters):
         """Modify the values and properties of parameters before internal
         validation is performed.  This method is called whenever a parameter
         has been changed."""
-        return self.param_type.update_parameters(parameters)
+        # TODO: we could do some more validation here
+        # and or make some parameters dependent on others
+        # validate that the column exists
+        # if parameters[0].altered:
+        #     try:
+        #         layer = parameters[0].valueAsText
+        #         fields = [f.name for f in arcpy.ListFields(layer)]
+        #         parameters[1].filter.list = fields
+        #     except Exception as e:
+        #         # hmm, dit doet het nog niet helemaal..
+        #         logging.error(e)
 
     def updateMessages(self, parameters):
         """Modify the messages created by internal validation for each tool
         parameter. This method is called after internal validation."""
 
     def execute(self, parameters, messages):
         """The source code of the tool."""
         if veg2hab.__version__ not in SUPPORTED_VERSIONS:
             logging.warning(
                 "Deze versie van de toolbox is niet getest met deze versie van de software.\n"
                 "Gelieve de toolbox opnieuw toe te voegen aan ArcGIS, zie installatie instructies.\n"
-                f"De locatie van veg2hab.pyt is: {veg2hab.constants.TOOLBOX_PYT_PATH}"
+                f"De locatie van toolbox.pyt is: {veg2hab.constants.TOOLBOX_PYT_PATH}"
             )
 
         input_params = self.param_type.from_parameter_list(parameters)
         veg2hab.main.run(input_params)
 
     def postExecute(self, parameters):
         """This method takes place after outputs are processed and
```

### Comparing `veg2hab-0.2.2a1/veg2hab/validation.py` & `veg2hab-0.2.3a0/veg2hab/validation.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/veg2hab/vegetatietypen.py` & `veg2hab-0.2.3a0/veg2hab/vegetatietypen.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/veg2hab/vegkartering.py` & `veg2hab-0.2.3a0/veg2hab/vegkartering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import logging
+import warnings
 from collections import defaultdict
 from dataclasses import dataclass
 from numbers import Number
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Union
 
 import geopandas as gpd
 import pandas as pd
 from typing_extensions import Literal, Self
 
 from veg2hab.access_db import read_access_tables
-from veg2hab.criteria import FGRCriterium, is_criteria_type_present
+from veg2hab.bronnen import FGR, LBK, Bodemkaart
+from veg2hab.criteria import (
+    BodemCriterium,
+    FGRCriterium,
+    LBKCriterium,
+    is_criteria_type_present,
+)
 from veg2hab.enums import KeuzeStatus, Kwaliteit
-from veg2hab.fgr import FGR
 from veg2hab.habitat import (
     HabitatVoorstel,
     calc_nr_of_unresolved_habitatkeuzes_per_row,
     rank_habitatkeuzes,
     try_to_determine_habkeuze,
 )
 from veg2hab.mozaiek import (
@@ -107,39 +113,39 @@
 
     def __hash__(self):
         return hash((self.percentage, tuple(self.VvN), tuple(self.SBB)))
 
 
 def ingest_vegtype(
     gdf: gpd.GeoDataFrame,
-    sbb_cols: List[str],
-    vvn_cols: List[str],
+    sbb_cols: Optional[List[str]],
+    vvn_cols: Optional[List[str]],
     perc_cols: List[str],
 ) -> pd.Series:
     """
     Leest de vegetatietypen van een vlak in en maakt er een lijst van VegTypeInfo objecten van
     Vlakken zonder percentage
     """
     # Validatie
-    if len(sbb_cols) != 0 and len(sbb_cols) != len(perc_cols):
+    if sbb_cols is not None and len(sbb_cols) != len(perc_cols):
         raise ValueError(
             f"De lengte van sbb_cols ({len(sbb_cols)}) moet 0 zijn of gelijk zijn aan de lengte van perc_col ({len(perc_cols)})"
         )
 
-    if len(vvn_cols) != 0 and len(vvn_cols) != len(perc_cols):
+    if vvn_cols is not None and len(vvn_cols) != len(perc_cols):
         raise ValueError(
             f"De lengte van vvn_cols ({len(vvn_cols)}) moet 0 zijn of gelijk zijn aan de lengte van perc_col ({len(perc_cols)})"
         )
 
-    assert len(sbb_cols) + len(vvn_cols) > 0, "Er moet een SBB of VvN kolom zijn"
+    assert sbb_cols or vvn_cols, "Er moet een SBB of VvN kolom zijn"
 
     # Inlezen
-    if len(sbb_cols) == 0:
+    if not sbb_cols:
         sbb_cols = [None] * len(perc_cols)
-    if len(vvn_cols) == 0:
+    if not vvn_cols:
         vvn_cols = [None] * len(perc_cols)
 
     def _row_to_vegtypeinfo_list(row: gpd.GeoSeries) -> List[VegTypeInfo]:
         vegtype_list = []
         for sbb_col, vvn_col, perc_col in zip(sbb_cols, vvn_cols, perc_cols):
             # Als er geen percentage is, willen we ook geen VegTypeInfo,
             # dus slaan we deze over
@@ -555,15 +561,15 @@
 
 def _single_to_multi(
     gdf: gpd.GeoDataFrame,
     SBB_col: Optional[str] = None,
     VvN_col: Optional[str] = None,
     split_char: Optional[str] = None,
     perc_col: Optional[str] = None,
-) -> Tuple[gpd.GeoDataFrame, List[str], List[str], List[str]]:
+) -> gpd.GeoDataFrame:
     """
     Converteert een "single" kolomformat dataframe naar een "multi" kolomformat dataframe
     De nieuwe "multi" format kolommen heten SBB1/2/3/..., VvN1/2/3/... en perc1/2/3/...
     """
     # Uitvinden hoe veel kolommen er moeten komen
     assert SBB_col or VvN_col, "Er moet een SBB of VvN kolom zijn"
     if perc_col:
@@ -603,39 +609,33 @@
                     new_col_prefix=col,
                 )
             )
             gdf = gdf.join(new_columns)
 
     # Kolomnamen moeten geupdated worden.
     if SBB_col:
-        SBB_out = [f"{SBB_col}{idx+1}" for idx in range(n_cols_needed)]
+        SBB_col = [f"{SBB_col}{idx+1}" for idx in range(n_cols_needed)]
         # Stel dat er max 3 VvN zijn en max 2 SBB, dan moet de SBB3 nog wel bestaan
-        for col in SBB_out:
+        for col in SBB_col:
             if col not in gdf.columns:
                 gdf[col] = None
-    else:
-        SBB_out = []
 
     if VvN_col:
-        VvN_out = [f"{VvN_col}{idx+1}" for idx in range(n_cols_needed)]
-        for col in VvN_out:
+        VvN_col = [f"{VvN_col}{idx+1}" for idx in range(n_cols_needed)]
+        for col in VvN_col:
             if col not in gdf.columns:
                 gdf[col] = None
-    else:
-        VvN_out = []
 
     if perc_col:
-        perc_out = [f"{perc_col}{idx+1}" for idx in range(n_cols_needed)]
-        for col in perc_out:
+        perc_col = [f"{perc_col}{idx+1}" for idx in range(n_cols_needed)]
+        for col in perc_col:
             if col not in gdf.columns:
                 gdf[col] = None
-    else:
-        perc_out = []
 
-    return gdf, SBB_out, VvN_out, perc_out
+    return gdf, SBB_col, VvN_col, perc_col
 
 
 class Kartering:
     def __init__(self, gdf: gpd.GeoDataFrame):
         self.gdf = gdf
 
         # Alle VegTypeInfo sorteren op percentage van hoog naar laag
@@ -745,93 +745,49 @@
 
         return cls(gdf)
 
     @classmethod
     def from_shapefile(
         cls,
         shape_path: Path,
-        *,
         vegtype_col_format: Literal["single", "multi"],
         sbb_of_vvn: Literal["VvN", "SBB", "beide"],
         ElmID_col: Optional[str] = None,
         datum_col: Optional[str] = None,
         opmerking_col: Optional[str] = None,
-        SBB_col: List[str],
-        VvN_col: List[str],
+        SBB_col: Optional[str] = None,
+        VvN_col: Optional[str] = None,
         split_char: Optional[str] = "+",
-        perc_col: List[str],
-        lok_vegtypen_col: List[str],
+        perc_col: Optional[str] = None,
+        lok_vegtypen_col: Optional[str] = None,
     ) -> Self:
         """
         Deze method wordt gebruikt om een Kartering te maken van een shapefile.
         Input:
         - shape_path: het pad naar de shapefile
         - ElmID_col: de kolomnaam van de ElementID in de Shapefile; uniek per vlak
         - vegtype_col_format: "single" als complexen in 1 kolom zitten of "multi" als er meerdere kolommen zijn
         - sbb_of_vvn: "VvN" als VvN de voorname vertaling is vanuit het lokale type, "SBB" voor SBB en "beide" als beide er zijn.
         - datum_col: kolomnaam van de datum als deze er is
         - opmerking_col: kolomnaam van de opmerking als deze er is
-        - VvN_col: kolomnaam van de VvN vegetatietypen als deze er is (bij single_col mag deze list maximaal lengte 1 hebben)
-        - SBB_col: kolomnaam van de SBB vegetatietypen als deze er is (bij single_col mag deze list maximaal lengte 1 hebben)
+        - VvN_col: kolomnaam van de VvN vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
+        - SBB_col: kolomnaam van de SBB vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
         - split_char: karakter waarop de vegetatietypen gesplitst moeten worden (voor complexen (bv "16aa2+15aa")) (wordt bij mutli_col gebruikt om de kolommen te scheiden)
-        - perc_col: kolomnaam van de percentage als deze er is (bij single_col mag deze list maximaal lengte 1 hebben))
-        - lok_vegtypen_col: kolomnaam van de lokale vegetatietypen als deze er zijn (bij single_col mag deze list maximaal lengte 1 hebben)
+        - perc_col: kolomnaam van de percentage als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))
+        - lok_vegtypen_col: kolomnaam van de lokale vegetatietypen als deze er zijn (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
         """
-        # CONTROLEREN VAN DE INPUT
-        if sbb_of_vvn == "VvN":
-            num_cols = len(VvN_col)
-            if len(VvN_col) == 0:
-                raise ValueError(
-                    "VvN_col moet worden opgegeven als sbb_of_vvn == 'VvN'"
-                )
-        elif sbb_of_vvn == "SBB":
-            num_cols = len(SBB_col)
-            if len(SBB_col) == 0:
-                raise ValueError(
-                    "SBB_col moet worden opgegeven als sbb_of_vvn == 'SBB'"
-                )
-        elif sbb_of_vvn == "beide":
-            num_cols = len(VvN_col)
-            if len(VvN_col) == 0 or len(SBB_col) == 0:
-                raise ValueError(
-                    "Zowel VvN_col als SBB_col moeten worden opgegeven als sbb_of_vvn == 'beide'"
-                )
-            if len(VvN_col) != len(SBB_col):
-                raise ValueError(
-                    "VvN_col en SBB_col moeten even lang zijn als sbb_of_vvn == 'beide'"
-                )
-        else:
-            raise ValueError("sbb_of_vvn moet ['VvN', 'SBB' of 'beide'] zijn")
 
-        if vegtype_col_format == "single":
-            if num_cols != 1:
-                raise ValueError(
-                    "Aantal kolommen moet 1 zijn bij vegtype_col_format == 'single'"
-                )
-        elif vegtype_col_format == "multi":
-            if num_cols == 0:
-                raise ValueError(
-                    "Aantal kolommen moet groter dan 0 zijn bij vegtype_col_format == 'multi'"
-                )
-
-        if len(perc_col) != num_cols and len(perc_col) != 0:
-            raise ValueError(
-                "Aantal kolommen moet gelijk zijn tussen perc_col en SBB_col/VvN_col"
-            )
-
-        if len(lok_vegtypen_col) != num_cols and len(lok_vegtypen_col) != 0:
-            raise ValueError(
-                "Aantal kolommen moet gelijk zijn tussen perc_col en SBB_col/VvN_col"
-            )
+        ###############
+        ##### Valideren, opschonen en aanvullen van de shapefile
+        ###############
 
-        # VALIDEREN, OPSCHONEN EN AANVULLEN VAN DE SHAPEFILE
         shapefile = gpd.read_file(shape_path)
 
         if ElmID_col and not shapefile[ElmID_col].is_unique:
-            logging.warn(
+            warnings.warn(
                 f"""De kolom {ElmID_col} bevat niet-unieke waarden in {shape_path}.
                 Eerste paar dubbele waarden:
                 {
                     shapefile[ElmID_col][shapefile[ElmID_col].duplicated()].head().to_list()
                 }
                 Er worden nieuwe waarden voor {ElmID_col} gemaakt en vanaf nu gebruikt.
                 """
@@ -844,81 +800,94 @@
             shapefile[ElmID_col] = range(len(shapefile))
 
         # Om niet bij splitten steeds "if split_char is not None:" te hoeven doen
         if split_char is None:
             split_char = "+"
 
         # Vastleggen lokale vegtypen voor in de output
-        if len(lok_vegtypen_col) > 0:
+        if lok_vegtypen_col is not None:
             shapefile["_LokVegTyp"] = shapefile.apply(
-                lambda row: ", ".join([str(row[col]) for col in lok_vegtypen_col]),
+                lambda row: ", ".join(
+                    [str(row[col]) for col in lok_vegtypen_col.split(split_char)]
+                ),
                 axis=1,
             )
         else:
             shapefile[
                 "_LokVegTyp"
             ] = "Geen kolommen opgegeven voor lokale vegetatietypen"
 
         # Selectie van de te bewaren kolommen
         cols = [
             col for col in [datum_col, opmerking_col] if col in shapefile.columns
         ] + [ElmID_col, "_LokVegTyp", "geometry"]
 
         # Uitvinden welke vegtype kolommen er mee moeten
-        cols += SBB_col + VvN_col + perc_col
+        if vegtype_col_format == "multi":
+            if SBB_col is not None:
+                SBB_col = SBB_col.split(split_char)
+                cols += SBB_col
+            if VvN_col is not None:
+                VvN_col = VvN_col.split(split_char)
+                cols += VvN_col
+            if perc_col is not None:
+                perc_col = perc_col.split(split_char)
+                cols += perc_col
+        else:
+            cols += [col for col in [VvN_col, SBB_col, perc_col] if col is not None]
         if not all(col in shapefile.columns for col in cols):
             raise ValueError(
                 f"Niet alle opgegeven kolommen ({cols}) gevonden in de shapefile kolommen ({shapefile.columns})"
             )
         gdf = shapefile[cols].copy()
 
         # Standardiseren van kolomnamen
-        # Als er geen datum of opmerking kolom is, dan maken we die en vullen we deze met None
-        if datum_col is None:
-            datum_col = "Datum"
-            gdf[datum_col] = None
-        if opmerking_col is None:
-            opmerking_col = "Opmerking"
-            gdf[opmerking_col] = None
-
         gdf = gdf.rename(
             columns={ElmID_col: "ElmID", opmerking_col: "Opmerking", datum_col: "Datum"}
         )
         ElmID_col = "ElmID"
         opmerking_col = "Opmerking"
         datum_col = "Datum"
 
         gdf = fix_crs(gdf, shape_path)
 
         if vegtype_col_format == "single":
             gdf, SBB_col, VvN_col, perc_col = _single_to_multi(
                 gdf=gdf,
-                SBB_col=None if len(SBB_col) == 0 else SBB_col[0],
-                VvN_col=None if len(VvN_col) == 0 else VvN_col[0],
+                SBB_col=SBB_col,
+                VvN_col=VvN_col,
                 split_char=split_char,
-                perc_col=None if len(perc_col) == 0 else perc_col[0],
+                perc_col=perc_col,
             )
             vegtype_col_format = "multi"
 
         # Opschonen
-        if len(SBB_col) > 0:
+        if SBB_col:
             gdf[SBB_col] = gdf[SBB_col].apply(_SBB.opschonen_series)
 
-        if len(VvN_col) > 0:
+        if VvN_col:
             gdf[VvN_col] = gdf[VvN_col].apply(_VvN.opschonen_series)
 
+        # Als er geen datum of opmerking kolom is, dan maken we die en vullen we deze met None
+        datum_col = "Datum" if datum_col is None else datum_col
+        opmerking_col = "Opmerking" if opmerking_col is None else opmerking_col
+        for col in [datum_col, opmerking_col]:
+            if col not in gdf.columns:
+                gdf[col] = None
+
         # Standardiseren van kolomnamen
+        gdf = gdf.rename(columns={datum_col: "Datum", opmerking_col: "Opmerking"})
         gdf["Opp"] = gdf["geometry"].area
         LokVrtNar_string = sbb_of_vvn if sbb_of_vvn != "beide" else "zowel SBB als VvN"
         gdf[
             "_LokVrtNar"
         ] = f"Lokale typologie is primair vertaald naar {LokVrtNar_string}"
 
         # Percentages invullen als die er niet zijn
-        if len(perc_col) == 0:
+        if perc_col is None:
             if vegtype_col_format == "multi":
                 perc_col = [
                     f"perc_{n}"
                     for n in range(
                         max([len(col) for col in [SBB_col, VvN_col] if col is not None])
                     )
                 ]
@@ -956,15 +925,15 @@
         # NOTE: Als dit te langzaam blijkt is een steekproef wss ook voldoende
         # NOTE NOTE: Als we zowel SBB en VvN uit de kartering hebben, willen we
         #            dan nog wwl doen voor de SBB zonder al meegegeven VvN?
         VvN_already_present = self.gdf["VegTypeInfo"].apply(
             lambda infos: any(len(info.VvN) > 0 for info in infos)
         )
         if VvN_already_present.any() and not override_existing_VvN:
-            logging.warn(
+            warnings.warn(
                 "Er zijn al VvN aanwezig in de kartering. De was-wordt lijst wordt niet toegepast."
             )
             return
 
         self.gdf["VegTypeInfo"] = self.gdf["VegTypeInfo"].apply(
             wwl.toevoegen_VvN_aan_List_VegTypeInfo
         )
@@ -981,60 +950,75 @@
 
         self.gdf["HabitatVoorstel"] = self.gdf["VegTypeInfo"].apply(
             lambda infos: [dt.find_habtypes(info) for info in infos]
             if len(infos) > 0
             else [[HabitatVoorstel.H0000_no_vegtype_present()]]
         )
 
-    def check_mitsen(self, fgr: FGR) -> None:
+    # NOTE: Moeten fgr/bodemkaart/lbk optional zijn?
+    def check_mitsen(self, fgr: FGR, bodemkaart: Bodemkaart, lbk: LBK) -> None:
         """
         Checkt of de mitsen in de habitatvoorstellen van de kartering wordt voldaan.
         """
         assert (
             "HabitatVoorstel" in self.gdf.columns
         ), "Er is geen kolom met HabitatVoorstel"
 
         # Deze dataframe wordt verrijkt met de info nodig om mitsen te checken.
         mits_info_df = gpd.GeoDataFrame(self.gdf.geometry)
 
         ### Bepaal waar meer informatie nodig is
-        # FGR
         fgr_needed = self.gdf["HabitatVoorstel"].apply(
             is_criteria_type_present, args=(FGRCriterium,)
         )
-        # Bodem
-        # etc
+        bodem_needed = self.gdf["HabitatVoorstel"].apply(
+            is_criteria_type_present, args=(BodemCriterium,)
+        )
+        lbk_needed = self.gdf["HabitatVoorstel"].apply(
+            is_criteria_type_present, args=(LBKCriterium,)
+        )
 
         ### Verrijken met de benodigde informatie
-        # FGR
-        mits_info_df["fgr"] = fgr.fgr_for_geometry(mits_info_df.loc[fgr_needed]).drop(
+        mits_info_df["fgr"] = fgr.for_geometry(mits_info_df.loc[fgr_needed]).drop(
+            columns="index_right"
+        )
+        mits_info_df["bodem"] = bodemkaart.for_geometry(
+            mits_info_df.loc[bodem_needed]
+        ).drop(columns="index_right")
+        mits_info_df["lbk"] = lbk.for_geometry(mits_info_df.loc[lbk_needed]).drop(
             columns="index_right"
         )
-        # Bodem
-        # etc
 
         ### Mitsen checken
         for idx, row in self.gdf.iterrows():
             mits_info_row = mits_info_df.loc[idx]
             for voorstellen in row.HabitatVoorstel:
                 for voorstel in voorstellen:
                     if voorstel.mits is None:
                         raise ValueError("Er is een habitatvoorstel zonder mits")
                     voorstel.mits.check(mits_info_row)
 
-    def bepaal_habitatkeuzes(self, fgr: FGR, max_iter: int = 20) -> None:
+    def bepaal_habitatkeuzes(
+        self, fgr: FGR, bodemkaart: Bodemkaart, lbk: LBK, max_iter: int = 20
+    ) -> None:
         """ """
+        assert isinstance(fgr, FGR), f"fgr moet een FGR object zijn, geen {type(fgr)}"
+        assert isinstance(
+            bodemkaart, Bodemkaart
+        ), f"bodemkaart moet een Bodemkaart object zijn, geen {type(bodemkaart)}"
+        assert isinstance(lbk, LBK), f"lbk moet een LBK object zijn, geen {type(lbk)}"
+
         # We starten alle HabitatKeuzes op None, en dan vullen we ze steeds verder in
         self.gdf["HabitatKeuze"] = self.gdf.VegTypeInfo.apply(
             lambda voorstellen_list: [None for sublist in voorstellen_list]
         )
         self.gdf["finished_on_iteration"] = 0
 
         ### Checken mitsen
-        self.check_mitsen(fgr)
+        self.check_mitsen(fgr, bodemkaart, lbk)
 
         ### Verkrijgen overlay gdf
         # Hier staat in welke vlakken er voor hoeveel procent aan welke andere vlakken grenzen
         # Als er geen vlakken met mozaiekregels zijn of als deze vlakken allemaal nergens aan grenzen is overlayed None
         overlayed = make_buffered_boundary_overlay_gdf(self.gdf)
 
         for i in range(max_iter):
@@ -1095,27 +1079,27 @@
 
             if (
                 n_keuzes_still_to_determine_pre == n_keuzes_still_to_determine_post
                 or n_keuzes_still_to_determine_post == 0
             ):
                 break
         else:
-            logging.warn(
+            warnings.warn(
                 f"Maximaal aantal iteraties ({max_iter}) bereikt voor het bepalen van de habitatkeuzes."
             )
 
         # Of we hebben overal een keuze, of we komen niet verder met nog meer iteraties,
         # of we hebben max_iter bereikt
 
         if n_keuzes_still_to_determine_post > 0:
             # NOTE
             # NOTE: @reviewer Moet dit een warning zijn vind je? Of gewoon een print?
             # NOTE: Het is iets wat niet alarmerend is maar wel nuttig om te weten.
             # NOTE
-            logging.warn(
+            warnings.warn(
                 f"Er zijn nog {n_keuzes_still_to_determine_post} habitatkeuzes die niet bepaald konden worden."
             )
 
         assert (
             self.gdf.HabitatKeuze.apply(lambda keuzes: keuzes.count(None)).sum() == 0
         ), "Er zijn nog habitatkeuzes die niet behandeld zijn en nog None zijn na bepaal_habitatkeuzes"
 
@@ -1240,9 +1224,16 @@
         """
         Slaat de kartering op in een shapefile
         """
         final = self.as_final_format()
         path.parent.mkdir(parents=True, exist_ok=True)
         final.to_file(path)
 
-    def __len__(self):
+    def get_geometry_mask(self) -> gpd.GeoDataFrame:
+        """
+        Geeft een gdf met alleen de geometrieen van de kartering,
+        bedoeld voor masking bij inladen grote gpkg's, zoals bodemkaart en LBK
+        """
+        return self.gdf[["geometry"]]
+
+    def __len__(self) -> int:
         return len(self.gdf)
```

### Comparing `veg2hab-0.2.2a1/veg2hab/waswordtlijst.py` & `veg2hab-0.2.3a0/veg2hab/waswordtlijst.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a1/PKG-INFO` & `veg2hab-0.2.3a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: veg2hab
-Version: 0.2.2a1
+Version: 0.2.3a0
 Summary: Package voor automatisch omzetten van vegetatiekarteringen naar habitatkaarten
 License: LGPLv3
 Author: Spheer.ai
 Author-email: info@spheer.ai
-Requires-Python: >=3.7.1,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: geopandas (>=0.10.0,<0.11.0)
-Requires-Dist: openpyxl (>=3.1.0,<4.0.0)
-Requires-Dist: pandas (>=1.3.0,<2.0.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: geopandas (>=0.10.0)
+Requires-Dist: openpyxl (>=3.0.0)
+Requires-Dist: pydantic (>=1.0,<2.0)
 Requires-Dist: pygeos (>=0.14,<0.15)
-Requires-Dist: pyodbc (>=4.0.1,<5.0.0)
+Requires-Dist: pyodbc (>=4.0.1)
 Requires-Dist: setuptools (<60.0.0)
 Requires-Dist: typing-extensions (==4.7.1)
-Requires-Dist: xlrd (>=2.0.1,<3.0.0)
+Requires-Dist: xlrd (>=2.0.1)
 Description-Content-Type: text/markdown
 
 # veg2hab
 
 - [veg2hab](#veg2hab)
   - [Introductie](#introductie)
   - [Installatie instructies](#installatie-instructies)
@@ -52,35 +51,35 @@
 
 veg2hab wordt gedistribueerd via PyPI, waar alle toekomstige versies aan toe worden gevoegd.
 
 ## Installatie instructies
 
 ### Installatie binnen ArcGIS Pro
 
-Gebruik van veg2hab is ontwikkeld voor en getest in ArcGIS Pro versie 3.0 en hoger.
-Installatie vanaf PyPI is veruit het eenvoudigst, en wordt hieronder omschreven:
+Gebruik van veg2hab is ontwikkeld voor en getest in ArcGIS Pro versie 3.0 en hoger. 
+Installatie vanaf PyPI is veruit het eenvoudigst, en wordt hieronder omschreven: 
 
  1. Open ArcGIS Pro
- 2. Maak een nieuwe python environment aan voor veg2hab (de default conda environment is read-only en niet geschikt om veg2hab in te installeren):
-    - Open de 'Package Manager'
+ 2. Maak een nieuwe python environment aan voor veg2hab (de default conda environment is read-only en niet geschikt om veg2hab in te installeren): 
+    - Open de 'Package Manager'  
         <img src="./images/package_manager.png" alt="package manager" width="400"/>
-    - Klik op het tandwiel naast 'Active Environment'
-    - Maak een nieuwe environment aan op een locatie naar keuze. Gebruik als 'Source' de default Environment.
-        <img src="./images/new_environment.png" alt="new python environment" width="400"/>
+    - Klik op het tandwiel naast 'Active Environment'  
+    - Maak een nieuwe environment aan op een locatie naar keuze. Gebruik als 'Source' de default Environment.  
+        <img src="./images/new_environment.png" alt="new python environment" width="400"/>  
         <img src="./images/environment_location.png" alt="location of new environment" width="400"/>
     - Selecteer de environment en druk op 'OK'.
  3. Download en installeer veg2hab:
-    - Klik op 'New notebook'
+    - Klik op 'New notebook'  
         <img src="./images/new_notebook.png" alt="new notebook" width="400"/>
-    - Download veg2hab met het commando `!pip install --upgrade veg2hab`
+    - Download veg2hab met het commando `!pip install --upgrade veg2hab`  
         <img src="./images/notebook_prompts.png" alt="prompts in notebook to install veg2hab" width="400"/>
     - Installeer veg2hab met het commando `import veg2hab`
  4. Installeer de veg2hab Python Toolbox:
     - Gebruik het commando `veg2hab.installatie_instructies()` om de locatie van de toolbox te vinden
-    - Ga naar 'Add Toolbox (file)' en voeg de toolbox toe vanaf de locatie
+    - Ga naar 'Add Toolbox (file)' en voeg de toolbox toe vanaf de locatie  
         <img src="./images/add_toolbox.png" alt="adding the veg2hab Python Toolbox" width="400"/>
 
 Als het goed is, wordt de veg2hab toolbox nu getoond in de Geoprocessing tab:
 
 <img src="./images/geoprocessing_tab.png" alt="geoprocessing tab" width="400"/>
 
 
@@ -95,31 +94,31 @@
 
 ### Gebruik in ArcGIS Pro
 
 De omzetting van veg2hab van vegetatiekarteringen naar habitattypekaarten gebeurt in tools in de veg2hab Python Toolbox. Om de omzetting te doen, dient de gebruiker eerst de betreffende vegetatiekarteringen in te laden als kaart in ArcGIS Pro.
 
 De omzettool komt in twee smaken:
 1. `digitale_standaard`, voor het omzetten van vegetatiekarteringen die de landelijke digitale standaard gebruiken, die bestaat uit een shapefile gecombineerd met een access database. De gebruiker voert in welke vegetatiekarteringen omgezet moet worden en waar de bijhorende access database te vinden is.
-2. `vector_bestand`, voor het omzetten van vegetatiekarteringen die alle benodigde informatie in de shapefile zelf bevatten. Omdat shapefiles geen standaard kolomnamen hebben, dient de gebruiker hier een handvol inputvelden in te vullen, bijvoorbeeld welke kolom de te gebruiken landelijke typologie bevat.
+2. `vector_bestand`, voor het omzetten van vegetatiekarteringen die alle benodigde informatie in de shapefile zelf bevatten. Omdat shapefiles geen standaard kolomnamen hebben, dient de gebruiker hier een handvol inputvelden in te vullen, bijvoorbeeld welke kolom de te gebruiken landelijke typologie bevat. 
 
 Let op:
 - Wanneer de gebruiker beschikt over een access database, raden wij aan de  `digitale_standaard` omzetting te gebruiken, ook als de shapefile alle informatie bevat. Hierbij is de kans op handmatige fouten kleiner.
-- Vegetatiekarteringen die omgezet worden met `vector_bestand` moeten beschikken over een landelijke typologie (SBB, VvN of rVvN).
+- Vegetatiekarteringen die omgezet worden met `vector_bestand` moeten beschikken over een landelijke typologie (SBB, VvN of rVvN). 
 
 
 ### Bronbestanden die veg2hab gebruikt
 
-veg2hab is afhankelijk van verschillende bronbestanden tijdens het omzetten van vegetatiekarteringen.
+veg2hab is afhankelijk van verschillende bronbestanden tijdens het omzetten van vegetatiekarteringen. 
 
-Sommige bestanden zijn landelijk beschikbaar. Deze bestanden worden automatisch mee geïnstalleerd met veg2hab en zijn niet aanpasbaar door de gebruiker:
+Sommige bestanden zijn landelijk beschikbaar. Deze bestanden worden automatisch mee geïnstalleerd met veg2hab en zijn niet aanpasbaar door de gebruiker: 
 
  - [WasWordtLijst](./data/5.%20Was-wordt-lijst-vegetatietypen-en-habitattypen-09-02-2021.xlsx) (versie 09-feb-2021): dit bestand wordt gebruikt om landelijke vegetatietypologieën in elkaar om te zetten
  - [DefinitieTabel](./data/definitietabel%20habitattypen%20(versie%2024%20maart%202009)_0.xls) (versie 24 maart 2009): dit is een samenvatting van de profieldocumenten
  - [Fysisch-Geografische Regio kaart](./data/bronbestanden/FGR.json) (versie 2013, [link naar origineel op Nationaal georegister](https://nationaalgeoregister.nl/geonetwork/srv/dut/catalog.search#/metadata/c8b5668f-c354-42f3-aafc-d15ae54cf170))
-
+  
 Let op: bij volgende versies komen er waarschijnlijk meer bronbestanden bij.
 
 
 
 ## Handleiding voor ontwikkelaars
 ### Lokale ontwikkeling
 Download de git repository:
@@ -148,15 +147,15 @@
 poetry run pytest tests/
 ```
 
 ### Nieuwe release
 1. Zorg ervoor dat de laatste bronbestanden in package_data staan met `poetry run python release.py create-package-data`.
 2. Maak een nieuwe versie met poetry (major, minor, patch): `poetry version {{rule}}`
 3. Pas de [\_\_init\_\_.py](veg2hab/__init__.py) __version__ variabele aan zodat deze overeen komt met de nieuw poetry version
-4. Pas [veg2hab.pyt](veg2hab/package_data/veg2hab.pyt) zodat de nieuwe version in SUPPORTED_VERSIONS staat. Heb je aanpassingen gedaan aan veg2hab.pyt sinds de laatste release, zorg er dan voor dat de `SUPPORTED_VERSIONS = [{{new_version}}]` wordt gezet.
+4. Pas [toolbox.pyt](veg2hab/package_data/toolbox.pyt) zodat de nieuwe version in SUPPORTED_VERSIONS staat. Heb je aanpassingen gedaan aan toolbox.pyt sinds de laatste release, zorg er dan voor dat de `SUPPORTED_VERSIONS = [{{new_version}}]` wordt gezet.
 5. Draai `python release.py check-versions` om te checken dat je geen fouten hebt gemaakt.
 6. Push nu eerst je nieuwe wijzigingen (mochten die er zijn), naar github. (`git add`, `git commit`, `git push`)
 7. Maak een nieuwe tag: `git tag v$(poetry version -s)`
 8. Push de tag naar git `git push origin tag v$(poetry version -s)`
 9. Github actions zal automatisch de nieuwe versie op PyPI zetten.
 
 
@@ -171,18 +170,18 @@
 
 **ElmID**: Een voor ieder vlak uniek ID. Deze kan vanuit de bronkartering komen, maar kan ook nieuw zijn gegenereerd. Dit gebeurt de als ElmID (of een ElmID equivalent zoals OBJECTID) in de bronkartering niet voor ieder vlak uniek is; als dit het geval is is hierover een warning gegeven.
 
 **_Samnvttng**: Weergave van hoeveel procent van het vlak bedekt is met welk habitattype. Dit is een combinatie van alle kolommen `Habtype{i}` en `Perc{i}`.
 
 **_LokVegTyp**: Het in de bronkartering opgegeven lokale vegetatietype, als er een lokaal vegetatietype kolom is opgegeven.
 
-**_LokVrtNar**: Of de oorspronkelijk opgegeven lokale vegetatietypen in de bronkartering primair is vertaald naar SBB, VvN of beide. Als er naar SBB is vertaald, zijn er bijbehorende VvN uit de waswordtlijst gehaald. Als er naar VvN of naar beide is vertaald, is dit niet gedaan.
+**_LokVrtNar**: Of de oorspronkelijk opgegeven lokale vegetatietypen in de bronkartering primair is vertaald naar SBB, VvN of beide. Als er naar SBB is vertaald, zijn er bijbehorende VvN uit de waswordtlijst gehaald. Als er naar VvN of naar beide is vertaald, is dit niet gedaan. 
 
 ### Complex-deel-specifieke kolommen
-**Habtype{i}**: Habitattype van het complex-deel. HXXXX hier betekend dat er menselijk oordeel nodig is over dit complex-deel.
+**Habtype{i}**: Habitattype van het complex-deel. HXXXX hier betekend dat er menselijk oordeel nodig is over dit complex-deel. 
 
 **Perc{i}**: Percentage van het gehele vlak wat door dit complex-deel wordt bedekt.
 
 **Opp{i}**: Oppervlakte van dit complex-deel in m2.
 
 **Kwal{i}**: Kwaliteit van dit complex-deel. Dit kan zijn G (goed), M (matig) of X (nvt).
```

