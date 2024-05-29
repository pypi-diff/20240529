# Comparing `tmp/aempsconn-1.0.0.tar.gz` & `tmp/aempsconn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aempsconn-1.0.0.tar", max compression
+gzip compressed data, was "aempsconn-1.0.1.tar", max compression
```

## Comparing `aempsconn-1.0.0.tar` & `aempsconn-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1063 2024-05-20 18:41:47.580822 aempsconn-1.0.0/LICENSE
--rw-r--r--   0        0        0     2109 2024-05-20 18:41:47.580822 aempsconn-1.0.0/README.md
--rw-r--r--   0        0        0      599 2024-05-20 18:41:47.580822 aempsconn-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1387 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/aemps.py
--rw-r--r--   0        0        0      250 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/__init__.py
--rw-r--r--   0        0        0     2652 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/maestras.py
--rw-r--r--   0        0        0     1049 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/medicamento.py
--rw-r--r--   0        0        0     6457 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/medicamentos.py
--rw-r--r--   0        0        0     3111 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/presentaciones.py
--rw-r--r--   0        0        0     2253 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/vmpp.py
--rw-r--r--   0        0        0      180 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/modules/__init__.py
--rw-r--r--   0        0        0      633 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/modules/medicamento.py
--rw-r--r--   0        0        0      643 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/modules/medicamentos.py
--rw-r--r--   0        0        0      664 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/modules/presentaciones.py
--rw-r--r--   0        0        0      627 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/modules/vmpp.py
--rw-r--r--   0        0        0       60 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/__init__.py
--rw-r--r--   0        0        0      155 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/atc.py
--rw-r--r--   0        0        0      223 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/descripcion_clinica.py
--rw-r--r--   0        0        0      560 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/documento.py
--rw-r--r--   0        0        0      250 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/documento_material.py
--rw-r--r--   0        0        0     1238 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/estado.py
--rw-r--r--   0        0        0      199 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/excipiente.py
--rw-r--r--   0        0        0      281 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/foto.py
--rw-r--r--   0        0        0      168 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/item.py
--rw-r--r--   0        0        0      345 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/material.py
--rw-r--r--   0        0        0     1248 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/medicamento.py
--rw-r--r--   0        0        0      464 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/nota.py
--rw-r--r--   0        0        0      601 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/presentacion.py
--rw-r--r--   0        0        0      218 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/principio_activo.py
--rw-r--r--   0        0        0      269 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/problema_suministro.py
--rw-r--r--   0        0        0      789 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/registro_cambios.py
--rw-r--r--   0        0        0      183 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/seccion.py
--rw-r--r--   0        0        0       48 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/__init__.py
--rw-r--r--   0        0        0      829 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/constants.py
--rw-r--r--   0        0        0      135 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/filter/__init__.py
--rw-r--r--   0        0        0      984 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/filter/base_operator.py
--rw-r--r--   0        0        0      576 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/filter/filter.py
--rw-r--r--   0        0        0      389 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/filter/operator.py
--rw-r--r--   0        0        0      753 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/hof.py
--rw-r--r--   0        0        0       95 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/module/__init__.py
--rw-r--r--   0        0        0     1454 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/module/base_module.py
--rw-r--r--   0        0        0     5157 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/request_handler.py
--rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 aempsconn-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-29 17:32:23.104887 aempsconn-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2109 2024-05-29 17:32:23.104887 aempsconn-1.0.1/README.md
+-rw-r--r--   0        0        0      599 2024-05-29 17:32:23.108887 aempsconn-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1387 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/aemps.py
+-rw-r--r--   0        0        0      250 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/filter/__init__.py
+-rw-r--r--   0        0        0     2652 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/filter/maestras.py
+-rw-r--r--   0        0        0     1049 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/filter/medicamento.py
+-rw-r--r--   0        0        0     6457 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/filter/medicamentos.py
+-rw-r--r--   0        0        0     3111 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/filter/presentaciones.py
+-rw-r--r--   0        0        0     2253 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/filter/vmpp.py
+-rw-r--r--   0        0        0      180 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/modules/__init__.py
+-rw-r--r--   0        0        0      633 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/modules/medicamento.py
+-rw-r--r--   0        0        0      643 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/modules/medicamentos.py
+-rw-r--r--   0        0        0      664 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/modules/presentaciones.py
+-rw-r--r--   0        0        0      627 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/modules/vmpp.py
+-rw-r--r--   0        0        0       60 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/__init__.py
+-rw-r--r--   0        0        0      155 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/atc.py
+-rw-r--r--   0        0        0      223 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/descripcion_clinica.py
+-rw-r--r--   0        0        0      560 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/documento.py
+-rw-r--r--   0        0        0      250 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/documento_material.py
+-rw-r--r--   0        0        0     1245 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/estado.py
+-rw-r--r--   0        0        0      199 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/excipiente.py
+-rw-r--r--   0        0        0      281 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/foto.py
+-rw-r--r--   0        0        0      168 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/item.py
+-rw-r--r--   0        0        0      345 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/material.py
+-rw-r--r--   0        0        0     1248 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/medicamento.py
+-rw-r--r--   0        0        0      464 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/nota.py
+-rw-r--r--   0        0        0      601 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/presentacion.py
+-rw-r--r--   0        0        0      218 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/principio_activo.py
+-rw-r--r--   0        0        0      269 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/problema_suministro.py
+-rw-r--r--   0        0        0      789 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/registro_cambios.py
+-rw-r--r--   0        0        0      183 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/objects/seccion.py
+-rw-r--r--   0        0        0       48 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/__init__.py
+-rw-r--r--   0        0        0      829 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/constants.py
+-rw-r--r--   0        0        0      135 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/filter/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/filter/base_operator.py
+-rw-r--r--   0        0        0      576 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/filter/filter.py
+-rw-r--r--   0        0        0      389 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/filter/operator.py
+-rw-r--r--   0        0        0      753 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/hof.py
+-rw-r--r--   0        0        0       95 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/module/__init__.py
+-rw-r--r--   0        0        0     1454 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/module/base_module.py
+-rw-r--r--   0        0        0     5157 2024-05-29 17:32:23.108887 aempsconn-1.0.1/src/aempsconn/utils/request_handler.py
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 aempsconn-1.0.1/PKG-INFO
```

### Comparing `aempsconn-1.0.0/LICENSE` & `aempsconn-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/README.md` & `aempsconn-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/pyproject.toml` & `aempsconn-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "aempsconn"
-version = "1.0.0"
+version = "1.0.1"
 description = "Library designed for interacting with the CIMA API (AEMPS)"
 license = "MIT"
 authors = ["fqlenos <fqlenos@protonmail.com>"]
 maintainers = ["fqlenos <fqlenos@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/fqlenos/aempsconn"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = "2.7.1"
-requests = "2.31.0"
+pydantic = "2.7.2"
+requests = "2.32.3"
 urllib3 = "2.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "3.7.1"
 pydoclint = "0.4.1"
 flake8 = "7.0.0"
```

### Comparing `aempsconn-1.0.0/src/aempsconn/aemps.py` & `aempsconn-1.0.1/src/aempsconn/aemps.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/filter/maestras.py` & `aempsconn-1.0.1/src/aempsconn/filter/maestras.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/filter/medicamento.py` & `aempsconn-1.0.1/src/aempsconn/filter/medicamento.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/filter/medicamentos.py` & `aempsconn-1.0.1/src/aempsconn/filter/medicamentos.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/filter/presentaciones.py` & `aempsconn-1.0.1/src/aempsconn/filter/presentaciones.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/filter/vmpp.py` & `aempsconn-1.0.1/src/aempsconn/filter/vmpp.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/modules/medicamento.py` & `aempsconn-1.0.1/src/aempsconn/modules/medicamento.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/modules/medicamentos.py` & `aempsconn-1.0.1/src/aempsconn/modules/medicamentos.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/modules/presentaciones.py` & `aempsconn-1.0.1/src/aempsconn/modules/presentaciones.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/modules/vmpp.py` & `aempsconn-1.0.1/src/aempsconn/modules/vmpp.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/objects/documento.py` & `aempsconn-1.0.1/src/aempsconn/objects/documento.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/objects/estado.py` & `aempsconn-1.0.1/src/aempsconn/objects/estado.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         if v is None:
             return None
 
         try:
             if isinstance(v, int):
                 try:
-                    return datetime.fromtimestamp(v)
+                    return datetime.fromtimestamp(v / 1000)
 
                 except (OSError, ValueError):
                     return None
 
             elif isinstance(v, str):
                 try:
                     return datetime.fromisoformat(v)
```

### Comparing `aempsconn-1.0.0/src/aempsconn/objects/medicamento.py` & `aempsconn-1.0.1/src/aempsconn/objects/medicamento.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/objects/presentacion.py` & `aempsconn-1.0.1/src/aempsconn/objects/presentacion.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/objects/registro_cambios.py` & `aempsconn-1.0.1/src/aempsconn/objects/registro_cambios.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/utils/constants.py` & `aempsconn-1.0.1/src/aempsconn/utils/constants.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/utils/filter/base_operator.py` & `aempsconn-1.0.1/src/aempsconn/utils/filter/base_operator.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/utils/filter/filter.py` & `aempsconn-1.0.1/src/aempsconn/utils/filter/filter.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/utils/hof.py` & `aempsconn-1.0.1/src/aempsconn/utils/hof.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/utils/module/base_module.py` & `aempsconn-1.0.1/src/aempsconn/utils/module/base_module.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/src/aempsconn/utils/request_handler.py` & `aempsconn-1.0.1/src/aempsconn/utils/request_handler.py`

 * *Files identical despite different names*

### Comparing `aempsconn-1.0.0/PKG-INFO` & `aempsconn-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: aempsconn
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library designed for interacting with the CIMA API (AEMPS)
 Home-page: https://github.com/fqlenos/aempsconn
 License: MIT
 Author: fqlenos
 Author-email: fqlenos@protonmail.com
 Maintainer: fqlenos
 Maintainer-email: fqlenos@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic (==2.7.1)
-Requires-Dist: requests (==2.31.0)
+Requires-Dist: pydantic (==2.7.2)
+Requires-Dist: requests (==2.32.3)
 Requires-Dist: urllib3 (==2.2.1)
 Project-URL: Repository, https://github.com/fqlenos/aempsconn
 Description-Content-Type: text/markdown
 
 # AEMPSconn
 Library designed for interacting with the CIMA REST API ([AEMPS](https://cima.aemps.es/cima/publico/home.html)).
 More information related to the official REST API can be found [here](https://cima.aemps.es/cima/resources/docs/CIMA_REST_API.pdf).
```

