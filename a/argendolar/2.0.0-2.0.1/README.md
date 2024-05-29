# Comparing `tmp/argendolar-2.0.0.tar.gz` & `tmp/argendolar-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argendolar-2.0.0.tar", last modified: Wed May 29 14:56:14 2024, max compression
+gzip compressed data, was "argendolar-2.0.1.tar", last modified: Wed May 29 15:09:47 2024, max compression
```

## Comparing `argendolar-2.0.0.tar` & `argendolar-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 14:56:14.917853 argendolar-2.0.0/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-2.0.0/LICENSE
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4634 2024-05-29 14:56:14.917602 argendolar-2.0.0/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492     3950 2024-05-28 15:34:50.000000 argendolar-2.0.0/README.md
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 14:56:14.915513 argendolar-2.0.0/argendolar/
--rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-2.0.0/argendolar/__init__.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492    11169 2024-05-29 14:52:59.000000 argendolar-2.0.0/argendolar/argendolar.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-2.0.0/argendolar/tipo_dolares.py
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 14:56:14.917251 argendolar-2.0.0/argendolar.egg-info/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4634 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/SOURCES.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/dependency_links.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/requires.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/top_level.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-29 14:56:14.917924 argendolar-2.0.0/setup.cfg
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-29 14:53:49.000000 argendolar-2.0.0/setup.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:09:47.811803 argendolar-2.0.1/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-2.0.1/LICENSE
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:09:47.811545 argendolar-2.0.1/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4783 2024-05-29 15:08:48.000000 argendolar-2.0.1/README.md
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:09:47.809629 argendolar-2.0.1/argendolar/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-2.0.1/argendolar/__init__.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492    11169 2024-05-29 14:52:59.000000 argendolar-2.0.1/argendolar/argendolar.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-2.0.1/argendolar/tipo_dolares.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:09:47.811112 argendolar-2.0.1/argendolar.egg-info/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/SOURCES.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/dependency_links.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/requires.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/top_level.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-29 15:09:47.811868 argendolar-2.0.1/setup.cfg
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-29 15:08:48.000000 argendolar-2.0.1/setup.py
```

### Comparing `argendolar-2.0.0/LICENSE` & `argendolar-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argendolar-2.0.0/PKG-INFO` & `argendolar-2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: argendolar
-Version: 2.0.0
-Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
-Home-page: https://github.com/Mgobeaalcoba/argendolar
-Author: Mariano Gobea Alcoba
-Author-email: gobeamariano@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: requests
-
 # Argendolar Package
 
 ## Description
 
 This package is used to get the exchange rate between the Argentine Peso and the US Dollar and other currencies (Euro, Real, Peso Chileno y Peso Uruguayo). For this, it uses the [Dolar API](https://dolarapi.com) and the [ArgentinaDatos API](https://argentinadatos.com/docs/) and then it converts the obtained data to a Pandas DataFrame for further analysis.
 
 ## Installation
@@ -42,28 +23,38 @@
 argendolar = Argendolar()
 ```
 
 ## Methods
 
 The `Argendolar` class has the following methods:
 
+- `api_status()`: Get the status of the API.
 - `get_dolar()`: Get all the dollars exchange rates: official, blue, mep, ccl, tarjeta, mayorista, etc. 
 - `get_oficial()`: Get the official dollar exchange rate.
 - `get_blue()`: Get the blue dollar exchange rate.
 - `get_mep()`: Get the MEP dollar exchange rate.
 - `get_ccl()`: Get the CCL dollar exchange rate.
 - `get_tarjeta()`: Get the dollar exchange rate for credit cards.
 - `get_mayorista()`: Get the dollar exchange rate for wholesale.
 - `get_cripo()`: Get the dollar exchange rate for cripto.
 - `get_euro()`: Get the euro exchange rate.
 - `get_real()`: Get the real exchange rate.
 - `get_chileno()`: Get the peso chileno exchange rate.
 - `get_uruguayo()`: Get the peso uruguayo exchange rate.
 - `get_dolar_historico()`: Get the historical dollar exchange rate for a specific date and Dollar Type (TipoDivisa.OFICIAL, TipoDivisa.BLUE, TipoDivisa.MEP, TipoDivisa.CCL, TipoDivisa.TARJETA, TipoDivisa.MAYORISTA, TipoDivisa.CRIPTO)
 - `get_dolar_historia_completa()`: Get the complete historical dollar exchange rate since 2011.
+- `get_inflacion_mensual_historica()`: Get the monthly historical inflation rate since 2000-01.
+- `get_inflacion_interanual_historica()`: Get the interannual historical inflation rate since 2000-01.
+- `get_indice_uva_historico()`: Get the historical UVA index since 2016-01.
+- `get_tasa_plazo_fijo_diaria_bancos()`: Get the daily fixed term rate for banks.
+- `get_tasa_promedio_plazo_fijo_historica()`: Get the historical average fixed term rate since 2000-01.
+
+All methods initially consult the state of the APIs (`api_status()`) to understand whether or not they can respond to the query. If the API is not active then they return an exception giving visibility to the API crash.
+
+All methods return the data in a Pandas DataFrame format for a quick and easy analysis or visualization.
 
 ## Examples
 
 Here are some examples of how to use the package:
 
 ```python
 from argendolar import Argendolar
@@ -126,8 +117,8 @@
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
 
 ## Contact
 
-If you have any questions or suggestions, you can contact me at [Mariano Gobea Alcoba](mailto:gobeamariano@gmail.com) or [Mariano Gobea Alcoba](https://www.linkedin.com/in/mariano-gobea-alcoba/).
+If you have any questions or suggestions, you can contact me at [Mariano Gobea Alcoba](mailto:gobeamariano@gmail.com) or [Mariano Gobea Alcoba](https://www.linkedin.com/in/mariano-gobea-alcoba/).
```

### Comparing `argendolar-2.0.0/argendolar/argendolar.py` & `argendolar-2.0.1/argendolar/argendolar.py`

 * *Files identical despite different names*

### Comparing `argendolar-2.0.0/argendolar.egg-info/PKG-INFO` & `argendolar-2.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 2.0.0
+Version: 2.0.1
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -42,28 +42,38 @@
 argendolar = Argendolar()
 ```
 
 ## Methods
 
 The `Argendolar` class has the following methods:
 
+- `api_status()`: Get the status of the API.
 - `get_dolar()`: Get all the dollars exchange rates: official, blue, mep, ccl, tarjeta, mayorista, etc. 
 - `get_oficial()`: Get the official dollar exchange rate.
 - `get_blue()`: Get the blue dollar exchange rate.
 - `get_mep()`: Get the MEP dollar exchange rate.
 - `get_ccl()`: Get the CCL dollar exchange rate.
 - `get_tarjeta()`: Get the dollar exchange rate for credit cards.
 - `get_mayorista()`: Get the dollar exchange rate for wholesale.
 - `get_cripo()`: Get the dollar exchange rate for cripto.
 - `get_euro()`: Get the euro exchange rate.
 - `get_real()`: Get the real exchange rate.
 - `get_chileno()`: Get the peso chileno exchange rate.
 - `get_uruguayo()`: Get the peso uruguayo exchange rate.
 - `get_dolar_historico()`: Get the historical dollar exchange rate for a specific date and Dollar Type (TipoDivisa.OFICIAL, TipoDivisa.BLUE, TipoDivisa.MEP, TipoDivisa.CCL, TipoDivisa.TARJETA, TipoDivisa.MAYORISTA, TipoDivisa.CRIPTO)
 - `get_dolar_historia_completa()`: Get the complete historical dollar exchange rate since 2011.
+- `get_inflacion_mensual_historica()`: Get the monthly historical inflation rate since 2000-01.
+- `get_inflacion_interanual_historica()`: Get the interannual historical inflation rate since 2000-01.
+- `get_indice_uva_historico()`: Get the historical UVA index since 2016-01.
+- `get_tasa_plazo_fijo_diaria_bancos()`: Get the daily fixed term rate for banks.
+- `get_tasa_promedio_plazo_fijo_historica()`: Get the historical average fixed term rate since 2000-01.
+
+All methods initially consult the state of the APIs (`api_status()`) to understand whether or not they can respond to the query. If the API is not active then they return an exception giving visibility to the API crash.
+
+All methods return the data in a Pandas DataFrame format for a quick and easy analysis or visualization.
 
 ## Examples
 
 Here are some examples of how to use the package:
 
 ```python
 from argendolar import Argendolar
```

### Comparing `argendolar-2.0.0/setup.py` & `argendolar-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='argendolar',
-    version='2.0.0',
+    version='2.0.1',
     packages=find_packages(),
     install_requires=['pandas', 'requests'],
     author='Mariano Gobea Alcoba',
     author_email='gobeamariano@gmail.com',
     description='A package to get the exchange rates of the different types of dollars and others currencies in Argentina.',
     long_description=long_description,  # Usa el contenido del README.md como descripción larga
     long_description_content_type="text/markdown",  # Especifica el tipo de contenido como markdown
```

