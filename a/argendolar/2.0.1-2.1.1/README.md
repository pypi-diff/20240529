# Comparing `tmp/argendolar-2.0.1.tar.gz` & `tmp/argendolar-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argendolar-2.0.1.tar", last modified: Wed May 29 15:09:47 2024, max compression
+gzip compressed data, was "argendolar-2.1.1.tar", last modified: Wed May 29 15:24:00 2024, max compression
```

## Comparing `argendolar-2.0.1.tar` & `argendolar-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:09:47.811803 argendolar-2.0.1/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-2.0.1/LICENSE
--rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:09:47.811545 argendolar-2.0.1/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4783 2024-05-29 15:08:48.000000 argendolar-2.0.1/README.md
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:09:47.809629 argendolar-2.0.1/argendolar/
--rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-2.0.1/argendolar/__init__.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492    11169 2024-05-29 14:52:59.000000 argendolar-2.0.1/argendolar/argendolar.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-2.0.1/argendolar/tipo_dolares.py
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:09:47.811112 argendolar-2.0.1/argendolar.egg-info/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/SOURCES.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/dependency_links.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/requires.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-29 15:09:47.000000 argendolar-2.0.1/argendolar.egg-info/top_level.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-29 15:09:47.811868 argendolar-2.0.1/setup.cfg
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-29 15:08:48.000000 argendolar-2.0.1/setup.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:24:00.636310 argendolar-2.1.1/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-2.1.1/LICENSE
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:24:00.636018 argendolar-2.1.1/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4783 2024-05-29 15:08:48.000000 argendolar-2.1.1/README.md
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:24:00.632864 argendolar-2.1.1/argendolar/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-2.1.1/argendolar/__init__.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492    11171 2024-05-29 15:22:32.000000 argendolar-2.1.1/argendolar/argendolar.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-2.1.1/argendolar/tipo_dolares.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 15:24:00.635554 argendolar-2.1.1/argendolar.egg-info/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     5467 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/SOURCES.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/dependency_links.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/requires.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-29 15:24:00.000000 argendolar-2.1.1/argendolar.egg-info/top_level.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-29 15:24:00.636382 argendolar-2.1.1/setup.cfg
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-29 15:22:49.000000 argendolar-2.1.1/setup.py
```

### Comparing `argendolar-2.0.1/LICENSE` & `argendolar-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argendolar-2.0.1/PKG-INFO` & `argendolar-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 2.0.1
+Version: 2.1.1
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `argendolar-2.0.1/README.md` & `argendolar-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `argendolar-2.0.1/argendolar/argendolar.py` & `argendolar-2.1.1/argendolar/argendolar.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         """
         Check the status of the API.
         :return: True if the API is online, False otherwise.
         """
         url = f"{self.base_url}/v1/estado"
         response = requests.get(url)
         data = response.json()
-        if data["estado"] == "Correcto":
+        if data["estado"] == "Disponible":
             return True
         else:
             return False
 
     def get_dolar(self) -> pd.DataFrame:
         """
         Get all the dollars exchange rates:
```

### Comparing `argendolar-2.0.1/argendolar.egg-info/PKG-INFO` & `argendolar-2.1.1/argendolar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 2.0.1
+Version: 2.1.1
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `argendolar-2.0.1/setup.py` & `argendolar-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='argendolar',
-    version='2.0.1',
+    version='2.1.1',
     packages=find_packages(),
     install_requires=['pandas', 'requests'],
     author='Mariano Gobea Alcoba',
     author_email='gobeamariano@gmail.com',
     description='A package to get the exchange rates of the different types of dollars and others currencies in Argentina.',
     long_description=long_description,  # Usa el contenido del README.md como descripción larga
     long_description_content_type="text/markdown",  # Especifica el tipo de contenido como markdown
```

