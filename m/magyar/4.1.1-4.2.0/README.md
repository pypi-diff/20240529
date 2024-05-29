# Comparing `tmp/magyar-4.1.1.tar.gz` & `tmp/magyar-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-4.1.1.tar", last modified: Wed May 29 20:13:36 2024, max compression
+gzip compressed data, was "magyar-4.2.0.tar", last modified: Wed May 29 20:40:20 2024, max compression
```

## Comparing `magyar-4.1.1.tar` & `magyar-4.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-29 20:13:36.590805 magyar-4.1.1/
--rw-r--r--   0 bela      (1000) bela      (1000)     7763 2024-05-29 20:13:36.590805 magyar-4.1.1/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     7347 2024-05-26 09:02:28.000000 magyar-4.1.1/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-29 20:13:36.590805 magyar-4.1.1/magyar.egg-info/
--rw-r--r--   0 bela      (1000) bela      (1000)     7763 2024-05-29 20:13:36.000000 magyar-4.1.1/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-29 20:13:36.000000 magyar-4.1.1/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-29 20:13:36.000000 magyar-4.1.1/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-29 20:13:36.000000 magyar-4.1.1/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)  3496747 2024-05-29 20:13:15.000000 magyar-4.1.1/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-29 20:13:36.590805 magyar-4.1.1/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      633 2024-05-29 20:13:15.000000 magyar-4.1.1/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-29 20:40:20.163390 magyar-4.2.0/
+-rw-r--r--   0 bela      (1000) bela      (1000)     8242 2024-05-29 20:40:20.162390 magyar-4.2.0/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     7789 2024-05-29 20:38:06.000000 magyar-4.2.0/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-29 20:40:20.161390 magyar-4.2.0/magyar.egg-info/
+-rw-r--r--   0 bela      (1000) bela      (1000)     8242 2024-05-29 20:40:20.000000 magyar-4.2.0/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-29 20:40:20.000000 magyar-4.2.0/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-29 20:40:20.000000 magyar-4.2.0/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-29 20:40:20.000000 magyar-4.2.0/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)  3496747 2024-05-29 20:13:15.000000 magyar-4.2.0/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-29 20:40:20.163390 magyar-4.2.0/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      670 2024-05-29 20:38:06.000000 magyar-4.2.0/setup.py
```

### Comparing `magyar-4.1.1/PKG-INFO` & `magyar-4.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: magyar
-Version: 4.1.1
-Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP
-Home-page: https://github.com/kobanya/nevek
-Author: Nagy Béla
-Author-email: nagy.belabudapest@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # magyar
 
 
 ## Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
 1. Magyar vezetéknevek   =  magyar.**vezeteknev**
@@ -199,15 +187,35 @@
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
         "kerulet": None,
         "kozterulet": None,
         "terulet_jellege": None
     },]  <BR><BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/irsz.png)
+<BR><BR>
+**Határon túli települések magyar nevei, magyar és a ma hivatalos nyelven**
+<BR><BR>
+magyar.hatarontuli 
+<BR><BR>
+
+Adatstruktúra : hatarontuli= [ {
+    "Abafája": {
+        "mai_hivatalos_nev": "Apalina",
+        "orszag": "RO"
+    },
+    "Abafalva": {
+        "mai_hivatalos_nev": "Abovce",
+        "orszag": "SK"
+    }]
+
+<BR><BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/hatarontuli_nev.png)
+
+
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható.
+Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-4.1.1/README.md` & `magyar-4.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: magyar
+Version: 4.2.0
+Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP, Határon túli magyar települések
+Home-page: https://github.com/kobanya/nevek
+Author: Nagy Béla
+Author-email: nagy.belabudapest@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # magyar
 
 
 ## Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
 1. Magyar vezetéknevek   =  magyar.**vezeteknev**
@@ -187,15 +199,35 @@
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
         "kerulet": None,
         "kozterulet": None,
         "terulet_jellege": None
     },]  <BR><BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/irsz.png)
+<BR><BR>
+**Határon túli települések magyar nevei, magyar és a ma hivatalos nyelven**
+<BR><BR>
+magyar.hatarontuli 
+<BR><BR>
+
+Adatstruktúra : hatarontuli= [ {
+    "Abafája": {
+        "mai_hivatalos_nev": "Apalina",
+        "orszag": "RO"
+    },
+    "Abafalva": {
+        "mai_hivatalos_nev": "Abovce",
+        "orszag": "SK"
+    }]
+
+<BR><BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/hatarontuli_nev.png)
+
+
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható.
+Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-4.1.1/magyar.egg-info/PKG-INFO` & `magyar-4.2.0/magyar.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.1.1
-Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP
+Version: 4.2.0
+Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP, Határon túli magyar települések
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -199,14 +199,34 @@
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
         "kerulet": None,
         "kozterulet": None,
         "terulet_jellege": None
     },]  <BR><BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/irsz.png)
+<BR><BR>
+**Határon túli települések magyar nevei, magyar és a ma hivatalos nyelven**
+<BR><BR>
+magyar.hatarontuli 
+<BR><BR>
+
+Adatstruktúra : hatarontuli= [ {
+    "Abafája": {
+        "mai_hivatalos_nev": "Apalina",
+        "orszag": "RO"
+    },
+    "Abafalva": {
+        "mai_hivatalos_nev": "Abovce",
+        "orszag": "SK"
+    }]
+
+<BR><BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/hatarontuli_nev.png)
+
+
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.1.1/magyar.py` & `magyar-4.2.0/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-4.1.1/setup.py` & `magyar-4.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="4.1.1",
+    version="4.2.0",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
-    description="Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP",
+    description="Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP, Határon túli magyar települések",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

