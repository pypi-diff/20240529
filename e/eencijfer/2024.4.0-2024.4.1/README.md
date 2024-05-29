# Comparing `tmp/eencijfer-2024.4.0.tar.gz` & `tmp/eencijfer-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eencijfer-2024.4.0.tar", max compression
+gzip compressed data, was "eencijfer-2024.4.1.tar", max compression
```

## Comparing `eencijfer-2024.4.0.tar` & `eencijfer-2024.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1069 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/LICENSE
--rw-r--r--   0        0        0      925 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/README.md
--rw-r--r--   0        0        0     1808 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/__init__.py
--rw-r--r--   0        0        0       43 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/__init__.py
--rw-r--r--   0        0        0    11868 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/cohorten.py
--rw-r--r--   0        0        0     1891 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/eencijfer.py
--rw-r--r--   0        0        0     3174 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/eindexamencijfers.py
--rw-r--r--   0        0        0        0 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/__init__py
--rw-r--r--   0        0        0     2159 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv
--rw-r--r--   0        0        0     1639 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/diploma.py
--rw-r--r--   0        0        0       53 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/local_data.py
--rw-r--r--   0        0        0     7712 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/opleiding.py
--rw-r--r--   0        0        0     1455 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/assets/transformations/postcodes.py
--rw-r--r--   0        0        0     1756 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/assets/transformations/prestatieafspraken.py
--rw-r--r--   0        0        0     7437 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/assets/transformations/vooropleiding.py
--rw-r--r--   0        0        0     5221 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/cli.py
--rw-r--r--   0        0        0       61 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/__init__.py
--rw-r--r--   0        0        0     2712 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/column_converters.py
--rw-r--r--   0        0        0    10854 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/eencijfer.py
--rw-r--r--   0        0        0      710 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Croho.csv
--rw-r--r--   0        0        0      716 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Croho_vest.csv
--rw-r--r--   0        0        0      136 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_actuele_instelling.csv
--rw-r--r--   0        0        0      349 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_brinnummer.csv
--rw-r--r--   0        0        0      527 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv
--rw-r--r--   0        0        0      128 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_ho-inst.csv
--rw-r--r--   0        0        0      284 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_ho_ISCED.csv
--rw-r--r--   0        0        0      126 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_isat.csv
--rw-r--r--   0        0        0      213 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_land_naar_herkomstindikking.csv
--rw-r--r--   0        0        0      264 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_landcode.csv
--rw-r--r--   0        0        0      282 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_nationaliteitscode.csv
--rw-r--r--   0        0        0      191 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_postcodecijfers_2023.csv
--rw-r--r--   0        0        0      191 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_postcodecijfers_2024.csv
--rw-r--r--   0        0        0      249 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vakcode.csv
--rw-r--r--   0        0        0      237 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vestnr_ho.csv
--rw-r--r--   0        0        0      237 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vestnr_ho_compleet.csv
--rw-r--r--   0        0        0      213 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vooropl.csv
--rw-r--r--   0        0        0      140 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vopl.csv
--rw-r--r--   0        0        0     6244 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/EV____24.csv
--rw-r--r--   0        0        0     1058 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/VAKHAVW_____.csv
--rw-r--r--   0        0        0     6596 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/pii.py
--rw-r--r--   0        0        0       28 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/io/__init__.py
--rw-r--r--   0        0        0     2777 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/io/db.py
--rw-r--r--   0        0        0     3915 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/io/files.py
--rw-r--r--   0        0        0     2232 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/settings.py
--rw-r--r--   0        0        0       33 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/__init__.py
--rw-r--r--   0        0        0     4054 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/detect_eencijfer_files.py
--rw-r--r--   0        0        0     2624 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/init.py
--rw-r--r--   0        0        0      991 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/local_data.py
--rw-r--r--   0        0        0     1944 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/qa.py
--rw-r--r--   0        0        0     2525 2024-04-18 19:42:47.086748 eencijfer-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-18 19:42:47.086748 eencijfer-2024.4.0/tests/__init__.py
--rw-r--r--   0        0        0      450 2024-04-18 19:42:47.086748 eencijfer-2024.4.0/tests/test_cli.py
--rw-r--r--   0        0        0      541 2024-04-18 19:42:47.086748 eencijfer-2024.4.0/tests/test_eencijfer.py
--rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 eencijfer-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-29 09:54:31.035344 eencijfer-2024.4.1/LICENSE
+-rw-r--r--   0        0        0      925 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/README.md
+-rw-r--r--   0        0        0     1808 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/__init__.py
+-rw-r--r--   0        0        0    11868 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/cohorten.py
+-rw-r--r--   0        0        0     1891 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/eencijfer.py
+-rw-r--r--   0        0        0     3174 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/eindexamencijfers.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/transformations/__init__py
+-rw-r--r--   0        0        0     2159 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv
+-rw-r--r--   0        0        0     1639 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/transformations/diploma.py
+-rw-r--r--   0        0        0       53 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/transformations/local_data.py
+-rw-r--r--   0        0        0     7712 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/transformations/opleiding.py
+-rw-r--r--   0        0        0     1455 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/transformations/postcodes.py
+-rw-r--r--   0        0        0     1756 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/transformations/prestatieafspraken.py
+-rw-r--r--   0        0        0     7437 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/assets/transformations/vooropleiding.py
+-rw-r--r--   0        0        0     5221 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/cli.py
+-rw-r--r--   0        0        0       61 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/__init__.py
+-rw-r--r--   0        0        0     2712 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/column_converters.py
+-rw-r--r--   0        0        0    10854 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/eencijfer.py
+-rw-r--r--   0        0        0      703 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Croho.csv
+-rw-r--r--   0        0        0      706 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Croho_vest.csv
+-rw-r--r--   0        0        0      136 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_actuele_instelling.csv
+-rw-r--r--   0        0        0      349 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_brinnummer.csv
+-rw-r--r--   0        0        0      527 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv
+-rw-r--r--   0        0        0      128 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_ho-inst.csv
+-rw-r--r--   0        0        0      284 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_ho_ISCED.csv
+-rw-r--r--   0        0        0      126 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_isat.csv
+-rw-r--r--   0        0        0      213 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_land_naar_herkomstindikking.csv
+-rw-r--r--   0        0        0      264 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_landcode.csv
+-rw-r--r--   0        0        0      282 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_nationaliteitscode.csv
+-rw-r--r--   0        0        0      191 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_postcodecijfers_2023.csv
+-rw-r--r--   0        0        0      191 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_postcodecijfers_2024.csv
+-rw-r--r--   0        0        0      249 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_vakcode.csv
+-rw-r--r--   0        0        0      237 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_vestnr_ho.csv
+-rw-r--r--   0        0        0      237 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_vestnr_ho_compleet.csv
+-rw-r--r--   0        0        0      213 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_vooropl.csv
+-rw-r--r--   0        0        0      140 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_vopl.csv
+-rw-r--r--   0        0        0     6235 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/EV____24.csv
+-rw-r--r--   0        0        0     1058 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/import_definitions/VAKHAVW_____.csv
+-rw-r--r--   0        0        0     7003 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/convert/pii.py
+-rw-r--r--   0        0        0       28 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/io/__init__.py
+-rw-r--r--   0        0        0     2777 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/io/db.py
+-rw-r--r--   0        0        0     3915 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/io/files.py
+-rw-r--r--   0        0        0     2232 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/settings.py
+-rw-r--r--   0        0        0       33 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/utils/__init__.py
+-rw-r--r--   0        0        0     4054 2024-05-29 09:54:31.039344 eencijfer-2024.4.1/eencijfer/utils/detect_eencijfer_files.py
+-rw-r--r--   0        0        0     2624 2024-05-29 09:54:31.043344 eencijfer-2024.4.1/eencijfer/utils/init.py
+-rw-r--r--   0        0        0      991 2024-05-29 09:54:31.043344 eencijfer-2024.4.1/eencijfer/utils/local_data.py
+-rw-r--r--   0        0        0     1944 2024-05-29 09:54:31.043344 eencijfer-2024.4.1/eencijfer/utils/qa.py
+-rw-r--r--   0        0        0     2526 2024-05-29 09:54:31.043344 eencijfer-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-29 09:54:31.043344 eencijfer-2024.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      450 2024-05-29 09:54:31.043344 eencijfer-2024.4.1/tests/test_cli.py
+-rw-r--r--   0        0        0      541 2024-05-29 09:54:31.043344 eencijfer-2024.4.1/tests/test_eencijfer.py
+-rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 eencijfer-2024.4.1/PKG-INFO
```

### Comparing `eencijfer-2024.4.0/LICENSE` & `eencijfer-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/README.md` & `eencijfer-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/__init__.py` & `eencijfer-2024.4.1/eencijfer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for eencijfer."""
 
 __author__ = """Bram Enning"""
 __email__ = 'bramenning@gmail.com'
-__version__ = '2024.4.0'
+__version__ = '2024.4.1'
 __app_name__ = 'eencijfer'
 
 import logging
 import shutil
 from importlib import import_module
 from pathlib import Path
```

### Comparing `eencijfer-2024.4.0/eencijfer/assets/cohorten.py` & `eencijfer-2024.4.1/eencijfer/assets/cohorten.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/assets/eencijfer.py` & `eencijfer-2024.4.1/eencijfer/assets/eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/assets/eindexamencijfers.py` & `eencijfer-2024.4.1/eencijfer/assets/eindexamencijfers.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv` & `eencijfer-2024.4.1/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/assets/transformations/diploma.py` & `eencijfer-2024.4.1/eencijfer/assets/transformations/diploma.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/assets/transformations/opleiding.py` & `eencijfer-2024.4.1/eencijfer/assets/transformations/opleiding.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/assets/transformations/postcodes.py` & `eencijfer-2024.4.1/eencijfer/assets/transformations/postcodes.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/assets/transformations/prestatieafspraken.py` & `eencijfer-2024.4.1/eencijfer/assets/transformations/prestatieafspraken.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/assets/transformations/vooropleiding.py` & `eencijfer-2024.4.1/eencijfer/assets/transformations/vooropleiding.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/cli.py` & `eencijfer-2024.4.1/eencijfer/cli.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/convert/column_converters.py` & `eencijfer-2024.4.1/eencijfer/convert/column_converters.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/convert/eencijfer.py` & `eencijfer-2024.4.1/eencijfer/convert/eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/convert/import_definitions/Croho.csv` & `eencijfer-2024.4.1/eencijfer/convert/import_definitions/Croho.csv`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Label,StartingPosition,NumberOfPositions,Converter
-AdministratienummerOWI,1,4,convert_to_object
+Instellingscode,1,4,convert_to_object
 Opleidingscode,5,5,convert_to_object
 ActueleInstellingInclBesturenfusies,10,4,convert_to_object
 ActueleInstellingExclBesturenfusies,14,4,convert_to_object
 OpleidingActueelEquivalent,18,5,convert_to_object
 OpleidingHistorischEquivalent,23,5,convert_to_object
 CrohoOnderdeelActueleOpleiding,28,1,convert_to_object
 CrohoSubonderdeelActueleOpleiding,29,2,convert_to_object
```

### Comparing `eencijfer-2024.4.0/eencijfer/convert/import_definitions/Croho_vest.csv` & `eencijfer-2024.4.1/eencijfer/convert/import_definitions/Croho_vest.csv`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Label,StartingPosition,NumberOfPositions,Converter
-AdministratienummerOWI,1,4,convert_to_object
+Instellingscode,1,4,convert_to_object
 Opleidingscode,5,5,convert_to_object
-VestigingsnummerOWI,10,2,convert_to_object
+Vestigingsnummer,10,2,convert_to_object
 ActueleInstelling,12,4,convert_to_object
 ActueleVestiging,16,2,convert_to_object
 OpleidingActueelEquivalent,18,5,convert_to_object
 OpleidingHistorischEquivalent,23,5,convert_to_object
 CrohoOnderdeelActueleOpleiding,28,1,convert_to_object
 CrohoSubonderdeelActueleOpleiding,29,2,convert_to_object
 SoortHogerOnderwijs,31,3,convert_to_object
```

### Comparing `eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv` & `eencijfer-2024.4.1/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/convert/import_definitions/EV____24.csv` & `eencijfer-2024.4.1/eencijfer/convert/import_definitions/EV____24.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Label,StartingPosition,NumberOfPositions,Converter
 PersoonsgebondenNummer,1,12,convert_to_object
 Inschrijvingsjaar,13,4,convert_to_int64
-AdministratienummerOwiInstelling,17,4,convert_to_object
+Instellingscode,17,4,convert_to_object
 ActueleInstelling,21,4,convert_to_object
 Opleidingscode,25,5,convert_to_int64
 Opleidingsvorm,30,1,convert_opleidingsvorm
 Opleidingsfase,31,1,convert_to_object
 MaandVanaf,32,2,convert_to_int64
-BeeindigingCode,34,1,convert_to_int64
+BeeindigingsCode,34,1,convert_to_int64
 MaandTot,35,2,convert_to_int64
 ExamenresultaatCode,37,1,convert_to_int64
 MaandExamenresultaat,38,2,convert_to_int64
-BekostigingCode,40,1,convert_to_object
+BekostigingsCode,40,1,convert_to_object
 EersteJaarAanDezeInstelling,41,4,convert_to_int64
 Inschrijvingsvorm,45,1,convert_to_object
 SoortHogerOnderwijs,46,3,convert_to_object
 OpleidingActueelEquivalent,49,5,convert_to_object
 OpleidingHistorischEquivalent,54,5,convert_to_object
 CrohoOnderdeelActueleOpleiding,59,1,convert_to_object
 CrohoSubonderdeelActueleOpleiding,60,2,convert_to_object
@@ -27,15 +27,15 @@
 SoortInschrijvingTypeHoBinnenSoortHo,68,1,convert_to_object
 SoortInschrijvingOpleidingActueelEquivalent,69,1,convert_to_object
 SoortInschrijvingActueleInstelling,70,1,convert_to_object
 SoortInschrijvingActueleOpleidingInstelling,71,1,convert_to_object
 VerblijfsjaarHogerOnderwijs,72,2,convert_to_int64
 VerblijfsjaarSoortHo,74,2,convert_to_int64
 VerblijfsjaarTypeHoBinnenSoortHo,76,2,convert_to_int64
-IndicatieEerstejaarsOplActueelEquivalent,78,1,convert_to_int64
+IndicatieEerstejaarsOpleidingActueelEquivalent,78,1,convert_to_int64
 IndicatieEerstejaarsActueleInstelling,79,1,convert_to_int64
 IndicatieEerstejaarsActueleOplInstelling,80,1,convert_to_int64
 EersteJaarInHetHogerOnderwijs,81,4,convert_to_int64
 EersteJaarAanDezeSoortHogerOnderwijs,85,4,convert_to_int64
 EersteJaarAanDezeOpleidingInstelling,89,4,convert_to_int64
 Diplomajaar,93,4,convert_to_int_zero_to_nan
 OpleidingsfaseActueelVanHetDiploma,97,1,convert_to_object
```

### Comparing `eencijfer-2024.4.0/eencijfer/convert/import_definitions/VAKHAVW_____.csv` & `eencijfer-2024.4.1/eencijfer/convert/import_definitions/VAKHAVW_____.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/convert/pii.py` & `eencijfer-2024.4.1/eencijfer/convert/pii.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Tools for removing PII."""
 
 import logging
-import sys
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from eencijfer.io.files import ExportFormat, _save_to_file
 from eencijfer.utils.detect_eencijfer_files import _get_eencijfer_datafile, _get_eindexamen_datafile
@@ -141,45 +140,55 @@
     Returns:
         None: Overwrite files to eencijfer_dir.
     """
 
     logger.debug('Replacing pgns and removing pii.')
 
     eencijfer_fname = _get_eencijfer_datafile(eencijfer_dir)
-    if eencijfer_fname is None:
-        logger.warning("No eencijfer-file found. So no PII to remove.")
-        sys.exit(0)
+    vakken_fname = _get_eindexamen_datafile(eencijfer_dir)
 
-    eencijfer_fpath = Path(eencijfer_dir / eencijfer_fname).with_suffix('.parquet')
-    eencijfer = pd.read_parquet(eencijfer_fpath)
+    # at least on of the files should be present.
+    if eencijfer_fname is None and vakken_fname is None:
+        raise Exception("No eencijfer-file or eindexamens found. So no PII to remove or local_id to add.")
+
+    if eencijfer_fname is not None:
+        eencijfer_fpath = Path(eencijfer_dir / eencijfer_fname).with_suffix('.parquet')
+        eencijfer = pd.read_parquet(eencijfer_fpath)
 
-    vakken_fname = _get_eindexamen_datafile(eencijfer_dir)
-    if vakken_fname is None:
-        raise Exception("No eindexamen-file found.")
+        if add_local_id:
+            logger.info('Adding local_id to eencijfer and vakken.')
+            eencijfer = _add_local_id(eencijfer)
 
-    vakken_fpath = Path(eencijfer_dir / vakken_fname).with_suffix('.parquet')
-    vakken = pd.read_parquet(vakken_fpath)
+    if vakken_fname is not None:
+        vakken_fpath = Path(eencijfer_dir / vakken_fname).with_suffix('.parquet')
+        vakken = pd.read_parquet(vakken_fpath)
 
-    if add_local_id:
-        logger.info('Adding local_id to eencijfer and vakken.')
-        eencijfer = _add_local_id(eencijfer)
-        vakken = _add_local_id(vakken)
+        if add_local_id:
+            logger.info('Adding local_id to eindexamenvakken.')
+            vakken = _add_local_id(vakken)
 
     if remove_pii:
         if add_local_id:
             logger.warning('Not removing local_id! Data still contains PII.')
-        logger.info('Creating table with pseudo-ids...')
-        koppeltabel = _create_pgn_pseudo_id_table(eencijfer)
-        logger.info(f'...removing pgn from {eencijfer_fpath}')
-        eencijfer = _replace_pgn_with_pseudo_id(eencijfer, koppeltabel)
-        eencijfer = _empty_id_fields(eencijfer)
-
-        logger.info(f'...removing pgn from {vakken_fpath}')
-        vakken = _replace_pgn_with_pseudo_id(vakken, koppeltabel)
-        vakken = _empty_id_fields(vakken)
 
-    logger.info(f"Overwriting {eencijfer_fname} to {eencijfer_dir}")
-    _save_to_file(eencijfer, fname=eencijfer_fname, dir=eencijfer_dir, export_format=ExportFormat.parquet)
+        logger.info('Creating table with pseudo-ids...')
+        if eencijfer_fname:
+            koppeltabel = _create_pgn_pseudo_id_table(eencijfer)
+        else:
+            koppeltabel = _create_pgn_pseudo_id_table(vakken)
+
+        if eencijfer_fname:
+            logger.info(f'...removing pgn from {eencijfer_fpath}')
+            eencijfer = _replace_pgn_with_pseudo_id(eencijfer, koppeltabel)
+            eencijfer = _empty_id_fields(eencijfer)
+
+            logger.info(f"Overwriting {eencijfer_fname} to {eencijfer_dir}")
+            _save_to_file(eencijfer, fname=eencijfer_fname, dir=eencijfer_dir, export_format=ExportFormat.parquet)
+
+        if vakken_fname:
+            logger.info(f'...removing pgn from {vakken_fpath}')
+            vakken = _replace_pgn_with_pseudo_id(vakken, koppeltabel)
+            vakken = _empty_id_fields(vakken)
+            logger.info(f"Saving {vakken_fname} to {eencijfer_dir}")
+            _save_to_file(vakken, fname=vakken_fname, dir=eencijfer_dir, export_format=ExportFormat.parquet)
 
-    logger.info(f"Saving {vakken_fname} to {eencijfer_dir}")
-    _save_to_file(vakken, fname=vakken_fname, dir=eencijfer_dir, export_format=ExportFormat.parquet)
     return None
```

### Comparing `eencijfer-2024.4.0/eencijfer/io/db.py` & `eencijfer-2024.4.1/eencijfer/io/db.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/io/files.py` & `eencijfer-2024.4.1/eencijfer/io/files.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/settings.py` & `eencijfer-2024.4.1/eencijfer/settings.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/utils/detect_eencijfer_files.py` & `eencijfer-2024.4.1/eencijfer/utils/detect_eencijfer_files.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/utils/init.py` & `eencijfer-2024.4.1/eencijfer/utils/init.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/utils/local_data.py` & `eencijfer-2024.4.1/eencijfer/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/eencijfer/utils/qa.py` & `eencijfer-2024.4.1/eencijfer/utils/qa.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/pyproject.toml` & `eencijfer-2024.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "eencijfer"
-version = "2024.4.0"
+version = "2024.4.1"
 homepage = "https://github.com/enningb/eencijfer"
 description = "ETL-tool for Dutch eencijfer."
 authors = ["Bram Enning <bramenning@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -87,15 +87,15 @@
 #skip_glob = docs/conf.py
 
 
 [tool.mypy]
 disable_error_code = ["attr-defined"]
 
 [tool.bumpversion]
-current_version = "2024.4.0"
+current_version = "2024.4.1"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>post)\\d+\\.dev\\d+)?"
 message = "Version updated from {current_version} to {new_version}"
@@ -111,14 +111,15 @@
 
 
 
 
 
 
 
+
 
 
 
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `eencijfer-2024.4.0/tests/test_eencijfer.py` & `eencijfer-2024.4.1/tests/test_eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.4.0/PKG-INFO` & `eencijfer-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eencijfer
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: ETL-tool for Dutch eencijfer.
 Home-page: https://github.com/enningb/eencijfer
 License: MIT
 Author: Bram Enning
 Author-email: bramenning@gmail.com
 Requires-Python: >=3.9.0,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

