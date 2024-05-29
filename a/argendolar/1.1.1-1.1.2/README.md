# Comparing `tmp/argendolar-1.1.1.tar.gz` & `tmp/argendolar-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argendolar-1.1.1.tar", last modified: Tue May 28 15:09:44 2024, max compression
+gzip compressed data, was "argendolar-1.1.2.tar", last modified: Tue May 28 16:03:05 2024, max compression
```

## Comparing `argendolar-1.1.1.tar` & `argendolar-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 15:09:44.893748 argendolar-1.1.1/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-1.1.1/LICENSE
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4620 2024-05-28 15:09:44.893494 argendolar-1.1.1/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492     3936 2024-05-28 13:44:59.000000 argendolar-1.1.1/README.md
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 15:09:44.891331 argendolar-1.1.1/argendolar/
--rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-1.1.1/argendolar/__init__.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492     6351 2024-05-28 14:58:58.000000 argendolar-1.1.1/argendolar/argendolar.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-1.1.1/argendolar/tipo_dolares.py
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 15:09:44.893121 argendolar-1.1.1/argendolar.egg-info/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4620 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/SOURCES.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/dependency_links.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/requires.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/top_level.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-28 15:09:44.893810 argendolar-1.1.1/setup.cfg
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-28 15:09:41.000000 argendolar-1.1.1/setup.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 16:03:05.084296 argendolar-1.1.2/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-1.1.2/LICENSE
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4634 2024-05-28 16:03:05.084045 argendolar-1.1.2/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     3950 2024-05-28 15:34:50.000000 argendolar-1.1.2/README.md
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 16:03:05.082071 argendolar-1.1.2/argendolar/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-1.1.2/argendolar/__init__.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     6351 2024-05-28 14:58:58.000000 argendolar-1.1.2/argendolar/argendolar.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-1.1.2/argendolar/tipo_dolares.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 16:03:05.083696 argendolar-1.1.2/argendolar.egg-info/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4634 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/SOURCES.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/dependency_links.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/requires.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/top_level.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-28 16:03:05.084353 argendolar-1.1.2/setup.cfg
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-28 16:02:50.000000 argendolar-1.1.2/setup.py
```

### Comparing `argendolar-1.1.1/LICENSE` & `argendolar-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argendolar-1.1.1/PKG-INFO` & `argendolar-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 ```
 
 ## Usage
 
 To use the package, you can import the `Argendolar` class and create an instance of it. 
  
 ```python
-from argendolar import Argendolar
+from argendolar import Argendolar, TipoDivisas
 
 # Create an instance of Argendolar
 argendolar = Argendolar()
 ```
 
 ## Methods
 
@@ -101,15 +101,15 @@
 # Get the peso chileno exchange rate
 chileno = argendolar.get_chileno()
 
 # Get the peso uruguayo exchange rate
 uruguayo = argendolar.get_uruguayo()
 
 # Get the historical dollar exchange rate for a specific date
-historico = argendolar.get_dolar_historico(tipo: TipoDivisa.MEP, fecha='2022-01-01')
+historico = argendolar.get_dolar_historico(tipo: TipoDivisas.MEP, fecha='2022-01-01')
 
 # Get the complete historical dollar exchange rate since 2011
 historia_completa = argendolar.get_dolar_historia_completa()
 ```
 
 ## Contributing
```

### Comparing `argendolar-1.1.1/README.md` & `argendolar-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ```
 
 ## Usage
 
 To use the package, you can import the `Argendolar` class and create an instance of it. 
  
 ```python
-from argendolar import Argendolar
+from argendolar import Argendolar, TipoDivisas
 
 # Create an instance of Argendolar
 argendolar = Argendolar()
 ```
 
 ## Methods
 
@@ -82,15 +82,15 @@
 # Get the peso chileno exchange rate
 chileno = argendolar.get_chileno()
 
 # Get the peso uruguayo exchange rate
 uruguayo = argendolar.get_uruguayo()
 
 # Get the historical dollar exchange rate for a specific date
-historico = argendolar.get_dolar_historico(tipo: TipoDivisa.MEP, fecha='2022-01-01')
+historico = argendolar.get_dolar_historico(tipo: TipoDivisas.MEP, fecha='2022-01-01')
 
 # Get the complete historical dollar exchange rate since 2011
 historia_completa = argendolar.get_dolar_historia_completa()
 ```
 
 ## Contributing
```

### Comparing `argendolar-1.1.1/argendolar/argendolar.py` & `argendolar-1.1.2/argendolar/argendolar.py`

 * *Files identical despite different names*

### Comparing `argendolar-1.1.1/argendolar.egg-info/PKG-INFO` & `argendolar-1.1.2/argendolar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 ```
 
 ## Usage
 
 To use the package, you can import the `Argendolar` class and create an instance of it. 
  
 ```python
-from argendolar import Argendolar
+from argendolar import Argendolar, TipoDivisas
 
 # Create an instance of Argendolar
 argendolar = Argendolar()
 ```
 
 ## Methods
 
@@ -101,15 +101,15 @@
 # Get the peso chileno exchange rate
 chileno = argendolar.get_chileno()
 
 # Get the peso uruguayo exchange rate
 uruguayo = argendolar.get_uruguayo()
 
 # Get the historical dollar exchange rate for a specific date
-historico = argendolar.get_dolar_historico(tipo: TipoDivisa.MEP, fecha='2022-01-01')
+historico = argendolar.get_dolar_historico(tipo: TipoDivisas.MEP, fecha='2022-01-01')
 
 # Get the complete historical dollar exchange rate since 2011
 historia_completa = argendolar.get_dolar_historia_completa()
 ```
 
 ## Contributing
```

### Comparing `argendolar-1.1.1/setup.py` & `argendolar-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='argendolar',
-    version='1.1.1',
+    version='1.1.2',
     packages=find_packages(),
     install_requires=['pandas', 'requests'],
     author='Mariano Gobea Alcoba',
     author_email='gobeamariano@gmail.com',
     description='A package to get the exchange rates of the different types of dollars and others currencies in Argentina.',
     long_description=long_description,  # Usa el contenido del README.md como descripción larga
     long_description_content_type="text/markdown",  # Especifica el tipo de contenido como markdown
```

