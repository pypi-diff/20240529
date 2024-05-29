# Comparing `tmp/maskalib-0.2.tar.gz` & `tmp/maskalib-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maskalib-0.2.tar", last modified: Sun May 26 02:19:13 2024, max compression
+gzip compressed data, was "maskalib-0.5.tar", last modified: Wed May 29 01:05:30 2024, max compression
```

## Comparing `maskalib-0.2.tar` & `maskalib-0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 02:19:13.234923 maskalib-0.2/
--rw-rw-rw-   0        0        0     1112 2024-05-26 02:19:13.233923 maskalib-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2024-05-26 02:18:53.000000 maskalib-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 02:19:13.228887 maskalib-0.2/maskalib/
--rw-rw-rw-   0        0        0     8267 2024-05-26 01:56:04.000000 maskalib-0.2/maskalib/MaskaAI.py
--rw-rw-rw-   0        0        0     8107 2024-05-26 02:00:23.000000 maskalib-0.2/maskalib/MaskaAIPremium.py
--rw-rw-rw-   0        0        0       97 2024-05-26 02:00:31.000000 maskalib-0.2/maskalib/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-26 01:47:52.000000 maskalib-0.2/maskalib/main.py
-drwxrwxrwx   0        0        0        0 2024-05-26 02:19:13.232917 maskalib-0.2/maskalib.egg-info/
--rw-rw-rw-   0        0        0     1112 2024-05-26 02:19:13.000000 maskalib-0.2/maskalib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-26 02:19:13.000000 maskalib-0.2/maskalib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 02:19:13.000000 maskalib-0.2/maskalib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-26 02:19:13.000000 maskalib-0.2/maskalib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 02:19:13.234923 maskalib-0.2/setup.cfg
--rw-rw-rw-   0        0        0      373 2024-05-26 02:13:14.000000 maskalib-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:30.060000 maskalib-0.5/
+-rw-rw-rw-   0        0        0     1112 2024-05-29 01:05:32.000000 maskalib-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-26 02:18:54.000000 maskalib-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:30.090000 maskalib-0.5/maskalib/
+-rw-rw-rw-   0        0        0     8267 2024-05-26 01:56:06.000000 maskalib-0.5/maskalib/MaskaAI.py
+-rw-rw-rw-   0        0        0     8107 2024-05-26 02:00:24.000000 maskalib-0.5/maskalib/MaskaAIPremium.py
+-rw-rw-rw-   0        0        0      135 2024-05-29 00:21:54.000000 maskalib-0.5/maskalib/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-26 01:47:54.000000 maskalib-0.5/maskalib/main.py
+-rw-rw-rw-   0        0        0     6468 2024-05-29 01:04:42.000000 maskalib-0.5/maskalib/ps99invest.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:30.120000 maskalib-0.5/maskalib.egg-info/
+-rw-rw-rw-   0        0        0     1112 2024-05-29 01:05:30.000000 maskalib-0.5/maskalib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-29 01:05:30.000000 maskalib-0.5/maskalib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 01:05:30.000000 maskalib-0.5/maskalib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 01:05:30.000000 maskalib-0.5/maskalib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 01:05:32.000000 maskalib-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      373 2024-05-29 01:05:10.000000 maskalib-0.5/setup.py
```

### Comparing `maskalib-0.2/PKG-INFO` & `maskalib-0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: maskalib
-Version: 0.2
-Description-Content-Type: text/markdown
-
 # Maskalib
 
 Maskalib is a Python library for [describe the purpose of your library].
 
 ## Installation
 
 You can install Maskalib using pip:
@@ -42,8 +37,8 @@
 x = MaskaAI(MODEL, YourAINAME,  MESSAGETOASK, APIKEY)
 print(x[0]) #Status
 print(x[1]) #Title
 print(x[2]) #Response
 
 ```
 
-# Go to Maska.ai to know more :D
+# Go to Maska.ai to know more :D
```

### Comparing `maskalib-0.2/README.md` & `maskalib-0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: maskalib
+Version: 0.5
+Description-Content-Type: text/markdown
+
 # Maskalib
 
 Maskalib is a Python library for [describe the purpose of your library].
 
 ## Installation
 
 You can install Maskalib using pip:
@@ -37,8 +42,8 @@
 x = MaskaAI(MODEL, YourAINAME,  MESSAGETOASK, APIKEY)
 print(x[0]) #Status
 print(x[1]) #Title
 print(x[2]) #Response
 
 ```
 
-# Go to Maska.ai to know more :D
+# Go to Maska.ai to know more :D
```

### Comparing `maskalib-0.2/maskalib/MaskaAI.py` & `maskalib-0.5/maskalib/MaskaAI.py`

 * *Files identical despite different names*

### Comparing `maskalib-0.2/maskalib/MaskaAIPremium.py` & `maskalib-0.5/maskalib/MaskaAIPremium.py`

 * *Files identical despite different names*

### Comparing `maskalib-0.2/maskalib.egg-info/PKG-INFO` & `maskalib-0.5/maskalib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maskalib
-Version: 0.2
+Version: 0.5
 Description-Content-Type: text/markdown
 
 # Maskalib
 
 Maskalib is a Python library for [describe the purpose of your library].
 
 ## Installation
```

