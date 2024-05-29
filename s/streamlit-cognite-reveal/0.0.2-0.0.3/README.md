# Comparing `tmp/streamlit_cognite_reveal-0.0.2.tar.gz` & `tmp/streamlit_cognite_reveal-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_cognite_reveal-0.0.2.tar", last modified: Wed May 29 08:47:51 2024, max compression
+gzip compressed data, was "streamlit_cognite_reveal-0.0.3.tar", last modified: Wed May 29 08:49:36 2024, max compression
```

## Comparing `streamlit_cognite_reveal-0.0.2.tar` & `streamlit_cognite_reveal-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,46 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:47:51.444079 streamlit_cognite_reveal-0.0.2/
--rw-r--r--   0 kvakkefly   (501) staff       (20)    11357 2024-05-06 10:15:16.000000 streamlit_cognite_reveal-0.0.2/LICENSE
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2829 2024-05-29 08:47:51.443840 streamlit_cognite_reveal-0.0.2/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2139 2024-05-24 14:41:54.000000 streamlit_cognite_reveal-0.0.2/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:47:51.442232 streamlit_cognite_reveal-0.0.2/reveal/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1312 2024-05-26 10:33:19.000000 streamlit_cognite_reveal-0.0.2/reveal/RevealConfig.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)       33 2024-05-26 09:38:59.000000 streamlit_cognite_reveal-0.0.2/reveal/TestClass.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4444 2024-05-29 08:47:35.000000 streamlit_cognite_reveal-0.0.2/reveal/__init__.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-05-29 08:47:51.444132 streamlit_cognite_reveal-0.0.2/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1146 2024-05-29 08:47:24.000000 streamlit_cognite_reveal-0.0.2/setup.py
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:47:51.443221 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2829 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      327 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/top_level.txt
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.470049 streamlit_cognite_reveal-0.0.3/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)    11357 2024-05-06 10:15:16.000000 streamlit_cognite_reveal-0.0.3/LICENSE
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2829 2024-05-29 08:49:36.469766 streamlit_cognite_reveal-0.0.3/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2139 2024-05-24 14:41:54.000000 streamlit_cognite_reveal-0.0.3/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.428444 streamlit_cognite_reveal-0.0.3/reveal/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1312 2024-05-26 10:33:19.000000 streamlit_cognite_reveal-0.0.3/reveal/RevealConfig.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       33 2024-05-26 09:38:59.000000 streamlit_cognite_reveal-0.0.3/reveal/TestClass.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4444 2024-05-29 08:47:35.000000 streamlit_cognite_reveal-0.0.3/reveal/__init__.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.426128 streamlit_cognite_reveal-0.0.3/reveal/frontend/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.429864 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1693 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/asset-manifest.json
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   197459 2024-05-29 08:48:44.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/bootstrap.min.css
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      553 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/index.html
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.426552 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.430546 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/css/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   331112 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/css/main.c81cb3cf.css
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   461776 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/css/main.c81cb3cf.css.map
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.444735 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3941 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/114.e0ebff55.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3959 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/142.e332c9ad.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     5176 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/211.ee14119e.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3976 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/413.5c9588ac.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4033 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/463.ad8fb302.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3940 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/690.16ab8bc4.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4753 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/797.fb53d4d2.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4270 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/809.14863d52.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3589 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/82.2b5d6c2f.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3822 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/913.b1b6282c.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3882 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/974.691b1718.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)  5730621 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/main.aaf72a55.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     5906 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/main.aaf72a55.js.LICENSE.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20) 16432189 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/main.aaf72a55.js.map
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.467861 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   106140 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   104332 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   105924 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)    98868 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   105804 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-05-29 08:49:36.470104 streamlit_cognite_reveal-0.0.3/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1146 2024-05-29 08:48:45.000000 streamlit_cognite_reveal-0.0.3/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.469030 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2829 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1679 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/top_level.txt
```

### Comparing `streamlit_cognite_reveal-0.0.2/LICENSE` & `streamlit_cognite_reveal-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_cognite_reveal-0.0.2/PKG-INFO` & `streamlit_cognite_reveal-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cognite-reveal
-Version: 0.0.2
+Version: 0.0.3
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
 Author: Anders Hafreager
 Author-email: anders.hafreager@cognite.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit_cognite_reveal-0.0.2/README.md` & `streamlit_cognite_reveal-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_cognite_reveal-0.0.2/reveal/RevealConfig.py` & `streamlit_cognite_reveal-0.0.3/reveal/RevealConfig.py`

 * *Files identical despite different names*

### Comparing `streamlit_cognite_reveal-0.0.2/reveal/__init__.py` & `streamlit_cognite_reveal-0.0.3/reveal/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_cognite_reveal-0.0.2/setup.py` & `streamlit_cognite_reveal-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-cognite-reveal",
-    version="0.0.2",
+    version="0.0.3",
     author="Anders Hafreager",
     author_email="anders.hafreager@cognite.com",
     description="Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/PKG-INFO` & `streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cognite-reveal
-Version: 0.0.2
+Version: 0.0.3
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
 Author: Anders Hafreager
 Author-email: anders.hafreager@cognite.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

