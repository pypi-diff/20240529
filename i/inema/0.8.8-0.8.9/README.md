# Comparing `tmp/inema-0.8.8.tar.gz` & `tmp/inema-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inema-0.8.8.tar", last modified: Sat May 27 11:21:10 2023, max compression
+gzip compressed data, was "inema-0.8.9.tar", last modified: Sat Dec 30 22:31:49 2023, max compression
```

## Comparing `inema-0.8.8.tar` & `inema-0.8.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-05-27 11:21:10.667201 inema-0.8.8/
--rw-r--r--   0 gms       (1000) gms       (1000)     7651 2023-05-19 17:49:22.000000 inema-0.8.8/LICENSE
--rw-r--r--   0 gms       (1000) gms       (1000)     2551 2023-05-27 11:21:10.667201 inema-0.8.8/PKG-INFO
--rw-r--r--   0 gms       (1000) gms       (1000)     1962 2021-03-13 09:37:23.000000 inema-0.8.8/README.rst
-drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-05-27 11:21:10.666201 inema-0.8.8/inema/
--rw-r--r--   0 gms       (1000) gms       (1000)      158 2021-03-13 09:37:23.000000 inema-0.8.8/inema/__init__.py
-drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-05-27 11:21:10.667201 inema-0.8.8/inema/data/
--rw-r--r--   0 gms       (1000) gms       (1000)    60237 2020-12-05 11:52:42.000000 inema-0.8.8/inema/data/formats.json
--rw-r--r--   0 gms       (1000) gms       (1000)    10382 2023-05-19 17:51:32.000000 inema-0.8.8/inema/data/products-2023-07-01.json
--rw-r--r--   0 gms       (1000) gms       (1000)     8113 2023-01-01 17:57:14.000000 inema-0.8.8/inema/data/products.json
--rwxr-xr-x   0 gms       (1000) gms       (1000)    13755 2023-05-19 17:49:22.000000 inema-0.8.8/inema/frank.py
--rw-r--r--   0 gms       (1000) gms       (1000)    10070 2023-05-19 17:49:22.000000 inema-0.8.8/inema/inema.py
--rw-r--r--   0 gms       (1000) gms       (1000)      901 2023-05-19 17:49:22.000000 inema-0.8.8/inema/utils.py
--rw-r--r--   0 gms       (1000) gms       (1000)    13183 2023-05-19 17:49:22.000000 inema-0.8.8/inema/wpint.py
-drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-05-27 11:21:10.666201 inema-0.8.8/inema.egg-info/
--rw-r--r--   0 gms       (1000) gms       (1000)     2551 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/PKG-INFO
--rw-r--r--   0 gms       (1000) gms       (1000)      376 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/SOURCES.txt
--rw-r--r--   0 gms       (1000) gms       (1000)        1 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/dependency_links.txt
--rw-r--r--   0 gms       (1000) gms       (1000)       43 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/entry_points.txt
--rw-r--r--   0 gms       (1000) gms       (1000)       29 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/requires.txt
--rw-r--r--   0 gms       (1000) gms       (1000)        6 2023-05-27 11:21:10.000000 inema-0.8.8/inema.egg-info/top_level.txt
--rw-r--r--   0 gms       (1000) gms       (1000)       92 2023-05-27 11:21:10.667201 inema-0.8.8/setup.cfg
--rw-r--r--   0 gms       (1000) gms       (1000)     1224 2023-05-19 17:55:56.000000 inema-0.8.8/setup.py
+drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-12-30 22:31:49.691167 inema-0.8.9/
+-rw-r--r--   0 gms       (1000) gms       (1000)     7651 2023-05-19 17:49:22.000000 inema-0.8.9/LICENSE
+-rw-r--r--   0 gms       (1000) gms       (1000)     2551 2023-12-30 22:31:49.691167 inema-0.8.9/PKG-INFO
+-rw-r--r--   0 gms       (1000) gms       (1000)     1962 2021-03-13 09:37:23.000000 inema-0.8.9/README.rst
+drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-12-30 22:31:49.691167 inema-0.8.9/inema/
+-rw-r--r--   0 gms       (1000) gms       (1000)      158 2021-03-13 09:37:23.000000 inema-0.8.9/inema/__init__.py
+drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-12-30 22:31:49.691167 inema-0.8.9/inema/data/
+-rw-r--r--   0 gms       (1000) gms       (1000)    60237 2020-12-05 11:52:42.000000 inema-0.8.9/inema/data/formats.json
+-rw-r--r--   0 gms       (1000) gms       (1000)    10383 2023-12-30 22:08:33.000000 inema-0.8.9/inema/data/products-2024-01-01.json
+-rw-r--r--   0 gms       (1000) gms       (1000)    10382 2023-05-19 17:51:32.000000 inema-0.8.9/inema/data/products.json
+-rwxr-xr-x   0 gms       (1000) gms       (1000)    13755 2023-05-19 17:49:22.000000 inema-0.8.9/inema/frank.py
+-rw-r--r--   0 gms       (1000) gms       (1000)    10070 2023-05-19 17:49:22.000000 inema-0.8.9/inema/inema.py
+-rw-r--r--   0 gms       (1000) gms       (1000)      901 2023-05-19 17:49:22.000000 inema-0.8.9/inema/utils.py
+-rw-r--r--   0 gms       (1000) gms       (1000)    13183 2023-05-19 17:49:22.000000 inema-0.8.9/inema/wpint.py
+drwxr-xr-x   0 gms       (1000) gms       (1000)        0 2023-12-30 22:31:49.691167 inema-0.8.9/inema.egg-info/
+-rw-r--r--   0 gms       (1000) gms       (1000)     2551 2023-12-30 22:31:49.000000 inema-0.8.9/inema.egg-info/PKG-INFO
+-rw-r--r--   0 gms       (1000) gms       (1000)      376 2023-12-30 22:31:49.000000 inema-0.8.9/inema.egg-info/SOURCES.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)        1 2023-12-30 22:31:49.000000 inema-0.8.9/inema.egg-info/dependency_links.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)       43 2023-12-30 22:31:49.000000 inema-0.8.9/inema.egg-info/entry_points.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)       29 2023-12-30 22:31:49.000000 inema-0.8.9/inema.egg-info/requires.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)        6 2023-12-30 22:31:49.000000 inema-0.8.9/inema.egg-info/top_level.txt
+-rw-r--r--   0 gms       (1000) gms       (1000)       92 2023-12-30 22:31:49.691167 inema-0.8.9/setup.cfg
+-rw-r--r--   0 gms       (1000) gms       (1000)     1224 2023-12-30 22:11:03.000000 inema-0.8.9/setup.py
```

### Comparing `inema-0.8.8/LICENSE` & `inema-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inema-0.8.8/PKG-INFO` & `inema-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inema
-Version: 0.8.8
+Version: 0.8.9
 Summary: A Python interface to the Deutsche Post Internetmarke and Warenpost International Online Franking
 Home-page: https://git.sysmocom.de/odoo/python-inema/
 Author: Harald Welte
 Author-email: hwelte@sysmocom.de
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `inema-0.8.8/README.rst` & `inema-0.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `inema-0.8.8/inema/data/formats.json` & `inema-0.8.9/inema/data/formats.json`

 * *Files identical despite different names*

### Comparing `inema-0.8.8/inema/data/products-2023-07-01.json` & `inema-0.8.9/inema/data/products.json`

 * *Files identical despite different names*

### Comparing `inema-0.8.8/inema/data/products.json` & `inema-0.8.9/inema/data/products-2024-01-01.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8012295081967213%*

 * *Differences: {"'1008'": "OrderedDict([('cost_price', '5.7'), ('international', False), ('max_weight', '20'), "*

 * *           "('name', 'Standardbrief Integral + EINSCHREIBEN + RÜCKSCHEIN')])",*

 * * "'1010'": "OrderedDict([('cost_price', '7.9'), ('international', False), ('max_weight', '20'), "*

 * *           "('name', 'Standardbrief Integral + EINSCHREIBEN + EIGENHÄNDIG + RÜCKSCHEIN')])",*

 * * "'1018'": "OrderedDict([('cost_price', '5.85'), ('international', False), ('max_weight', '50'), "*

 * *           "('name', 'Kompaktbrief Integral + […]*

```diff
@@ -37,26 +37,38 @@
     },
     "10071": {
         "cost_price": "7",
         "international": true,
         "max_weight": "1000",
         "name": "Maxibrief Intern. bis 1.000g GK"
     },
+    "1008": {
+        "cost_price": "5.7",
+        "international": false,
+        "max_weight": "20",
+        "name": "Standardbrief Integral + EINSCHREIBEN + R\u00dcCKSCHEIN"
+    },
     "1009": {
         "cost_price": "5.70",
         "international": false,
         "max_weight": "20",
         "name": "Standardbrief Integral + EINSCHREIBEN + EIGENH\u00c4NDIG"
     },
     "10091": {
         "cost_price": "17",
         "international": true,
         "max_weight": "2000",
         "name": "Maxibrief Intern. bis 2.000g GK"
     },
+    "1010": {
+        "cost_price": "7.9",
+        "international": false,
+        "max_weight": "20",
+        "name": "Standardbrief Integral + EINSCHREIBEN + EIGENH\u00c4NDIG + R\u00dcCKSCHEIN"
+    },
     "1012": {
         "cost_price": "3.35",
         "international": false,
         "max_weight": "50",
         "name": "Kompaktbrief Integral + EINSCHREIBEN EINWURF"
     },
     "10162": {
@@ -73,20 +85,32 @@
     },
     "1017": {
         "cost_price": "3.65",
         "international": false,
         "max_weight": "50",
         "name": "Kompaktbrief Integral + EINSCHREIBEN"
     },
+    "1018": {
+        "cost_price": "5.85",
+        "international": false,
+        "max_weight": "50",
+        "name": "Kompaktbrief Integral + EINSCHREIBEN + R\u00dcCKSCHEIN"
+    },
     "1019": {
         "cost_price": "5.85",
         "international": false,
         "max_weight": "50",
         "name": "Kompaktbrief Integral + EINSCHREIBEN + EIGENH\u00c4NDIG"
     },
+    "1020": {
+        "cost_price": "8.05",
+        "international": false,
+        "max_weight": "50",
+        "name": "Kompaktbrief Integral + EINSCHREIBEN + EIGENH\u00c4NDIG + R\u00dcCKSCHEIN"
+    },
     "10201": {
         "cost_price": "0.95",
         "international": true,
         "max_weight": "15",
         "name": "Postkarte Intern. GK"
     },
     "1022": {
@@ -97,74 +121,122 @@
     },
     "1027": {
         "cost_price": "4.25",
         "international": false,
         "max_weight": "500",
         "name": "Gro\u00dfbrief Integral + EINSCHREIBEN"
     },
+    "1028": {
+        "cost_price": "6.45",
+        "international": false,
+        "max_weight": "500",
+        "name": "Gro\u00dfbrief Integral + EINSCHREIBEN + R\u00dcCKSCHEIN"
+    },
     "1029": {
         "cost_price": "6.45",
         "international": false,
         "max_weight": "500",
         "name": "Gro\u00dfbrief Integral + EINSCHREIBEN + EIGENH\u00c4NDIG"
     },
+    "1030": {
+        "cost_price": "8.65",
+        "international": false,
+        "max_weight": "500",
+        "name": "Gro\u00dfbrief Integral + EINSCHREIBEN + EIGENH\u00c4NDIG + R\u00dcCKSCHEIN"
+    },
     "1032": {
         "cost_price": "5.10",
         "international": false,
         "max_weight": "1000",
         "name": "Maxibrief Integral + EINSCHREIBEN EINWURF"
     },
     "1037": {
         "cost_price": "5.40",
         "international": false,
         "max_weight": "1000",
         "name": "Maxibrief Integral + EINSCHREIBEN"
     },
+    "1038": {
+        "cost_price": "7.6",
+        "international": false,
+        "max_weight": "1000",
+        "name": "Maxibrief Integral + EINSCHREIBEN + R\u00dcCKSCHEIN"
+    },
     "1039": {
         "cost_price": "7.60",
         "international": false,
         "max_weight": "1000",
         "name": "Maxibrief Integral + EINSCHREIBEN + EIGENH\u00c4NDIG"
     },
+    "1040": {
+        "cost_price": "9.8",
+        "international": false,
+        "max_weight": "1000",
+        "name": "Maxibrief Integral + EINSCHREIBEN + EIGENH\u00c4NDIG + R\u00dcCKSCHEIN"
+    },
     "1042": {
         "cost_price": "7.30",
         "international": false,
         "max_weight": "2000",
         "name": "Maxibrief Integral + Zusatzentgelt MBf + EINSCHREIBEN EINWURF"
     },
     "1047": {
         "cost_price": "7.60",
         "international": false,
         "max_weight": "2000",
         "name": "Maxibrief Integral + Zusatzentgelt MBf + EINSCHREIBEN"
     },
+    "1048": {
+        "cost_price": "9.8",
+        "international": false,
+        "max_weight": "2000",
+        "name": "Maxibrief Integral + Zusatzentgelt MBf + EINSCHREIBEN + R\u00dcCKSCHEIN"
+    },
     "1049": {
         "cost_price": "9.80",
         "international": false,
         "max_weight": "2000",
         "name": "Maxibrief Integral + Zusatzentgelt MBf + EINSCHREIBEN + EIGENH\u00c4NDIG"
     },
+    "1050": {
+        "cost_price": "12",
+        "international": false,
+        "max_weight": "2000",
+        "name": "Maxibrief Integral + Zusatzentgelt MBf + EINSCHREIBEN + EIGENH\u00c4NDIG + R\u00dcCKSCHEIN"
+    },
     "1052": {
         "cost_price": "3.05",
         "international": false,
         "max_weight": "15",
         "name": "Postkarte Integral + EINSCHREIBEN EINWURF"
     },
     "1057": {
         "cost_price": "3.35",
         "international": false,
         "max_weight": "15",
         "name": "Postkarte Integral + EINSCHREIBEN"
     },
+    "1058": {
+        "cost_price": "5.55",
+        "international": false,
+        "max_weight": "",
+        "name": "Postkarte Integral + EINSCHREIBEN + R\u00dcCKSCHEIN"
+    },
     "1059": {
         "cost_price": "5.55",
         "international": false,
         "max_weight": "15",
         "name": "Postkarte Integral + EINSCHREIBEN + EIGENH\u00c4NDIG"
     },
+    "1060": {
+        "cost_price": "7.75",
+        "international": false,
+        "max_weight": "",
+        "name": "Postkarte Integral + EINSCHREIBEN + EIGENH\u00c4NDIG + R\u00dcCKSCHEIN"
+    },
     "11": {
         "cost_price": "1.00",
         "international": false,
         "max_weight": "50",
         "name": "Kompaktbrief"
     },
     "11006": {
@@ -242,21 +314,21 @@
     "21": {
         "cost_price": "1.60",
         "international": false,
         "max_weight": "500",
         "name": "Gro\u00dfbrief"
     },
     "282": {
-        "cost_price": "1.95",
+        "cost_price": "2.25",
         "international": false,
         "max_weight": "500",
         "name": "B\u00fccher- und Warensendung 500"
     },
     "290": {
-        "cost_price": "2.25",
+        "cost_price": "2.55",
         "international": false,
         "max_weight": "1000",
         "name": "B\u00fccher- und Warensendung 1000"
     },
     "31": {
         "cost_price": "2.75",
         "international": false,
```

### Comparing `inema-0.8.8/inema/frank.py` & `inema-0.8.9/inema/frank.py`

 * *Files identical despite different names*

### Comparing `inema-0.8.8/inema/inema.py` & `inema-0.8.9/inema/inema.py`

 * *Files identical despite different names*

### Comparing `inema-0.8.8/inema/utils.py` & `inema-0.8.9/inema/utils.py`

 * *Files identical despite different names*

### Comparing `inema-0.8.8/inema/wpint.py` & `inema-0.8.9/inema/wpint.py`

 * *Files identical despite different names*

### Comparing `inema-0.8.8/inema.egg-info/PKG-INFO` & `inema-0.8.9/inema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inema
-Version: 0.8.8
+Version: 0.8.9
 Summary: A Python interface to the Deutsche Post Internetmarke and Warenpost International Online Franking
 Home-page: https://git.sysmocom.de/odoo/python-inema/
 Author: Harald Welte
 Author-email: hwelte@sysmocom.de
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `inema-0.8.8/setup.py` & `inema-0.8.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,24 +4,24 @@
         'zeep >= 0.12.0',
         'pytz',
         'setuptools' # i.e. provides pkg_resources
 ]
 
 setup(
         name='inema',
-        version='0.8.8',
+        version='0.8.9',
         description='A Python interface to the Deutsche Post Internetmarke and Warenpost International Online Franking',
         long_description=open('README.rst').read(),
         author='Harald Welte',
         author_email='hwelte@sysmocom.de',
         url='https://git.sysmocom.de/odoo/python-inema/',
         packages=['inema'],
         install_requires=install_requires,
         package_data={'inema': ['data/products.json',
-                                'data/products-2023-07-01.json',
+                                'data/products-2024-01-01.json',
                                 'data/formats.json']},
         license='LGPLv3',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
             'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3',
```

