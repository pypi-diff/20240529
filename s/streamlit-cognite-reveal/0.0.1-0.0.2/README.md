# Comparing `tmp/streamlit_cognite_reveal-0.0.1.tar.gz` & `tmp/streamlit_cognite_reveal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_cognite_reveal-0.0.1.tar", last modified: Wed May 29 08:44:07 2024, max compression
+gzip compressed data, was "streamlit_cognite_reveal-0.0.2.tar", last modified: Wed May 29 08:47:51 2024, max compression
```

## Comparing `streamlit_cognite_reveal-0.0.1.tar` & `streamlit_cognite_reveal-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:44:07.028189 streamlit_cognite_reveal-0.0.1/
--rw-r--r--   0 kvakkefly   (501) staff       (20)    11357 2024-05-06 10:15:16.000000 streamlit_cognite_reveal-0.0.1/LICENSE
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2811 2024-05-29 08:44:07.027913 streamlit_cognite_reveal-0.0.1/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2139 2024-05-24 14:41:54.000000 streamlit_cognite_reveal-0.0.1/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:44:07.026209 streamlit_cognite_reveal-0.0.1/reveal/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1312 2024-05-26 10:33:19.000000 streamlit_cognite_reveal-0.0.1/reveal/RevealConfig.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)       33 2024-05-26 09:38:59.000000 streamlit_cognite_reveal-0.0.1/reveal/TestClass.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4429 2024-05-27 08:53:53.000000 streamlit_cognite_reveal-0.0.1/reveal/__init__.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-05-29 08:44:07.028245 streamlit_cognite_reveal-0.0.1/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1128 2024-05-29 08:43:47.000000 streamlit_cognite_reveal-0.0.1/setup.py
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:44:07.027249 streamlit_cognite_reveal-0.0.1/streamlit_cognite_reveal.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2811 2024-05-29 08:44:07.000000 streamlit_cognite_reveal-0.0.1/streamlit_cognite_reveal.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      327 2024-05-29 08:44:07.000000 streamlit_cognite_reveal-0.0.1/streamlit_cognite_reveal.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-05-29 08:44:07.000000 streamlit_cognite_reveal-0.0.1/streamlit_cognite_reveal.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-05-29 08:44:07.000000 streamlit_cognite_reveal-0.0.1/streamlit_cognite_reveal.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-05-29 08:44:07.000000 streamlit_cognite_reveal-0.0.1/streamlit_cognite_reveal.egg-info/top_level.txt
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:47:51.444079 streamlit_cognite_reveal-0.0.2/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)    11357 2024-05-06 10:15:16.000000 streamlit_cognite_reveal-0.0.2/LICENSE
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2829 2024-05-29 08:47:51.443840 streamlit_cognite_reveal-0.0.2/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2139 2024-05-24 14:41:54.000000 streamlit_cognite_reveal-0.0.2/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:47:51.442232 streamlit_cognite_reveal-0.0.2/reveal/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1312 2024-05-26 10:33:19.000000 streamlit_cognite_reveal-0.0.2/reveal/RevealConfig.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       33 2024-05-26 09:38:59.000000 streamlit_cognite_reveal-0.0.2/reveal/TestClass.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4444 2024-05-29 08:47:35.000000 streamlit_cognite_reveal-0.0.2/reveal/__init__.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-05-29 08:47:51.444132 streamlit_cognite_reveal-0.0.2/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1146 2024-05-29 08:47:24.000000 streamlit_cognite_reveal-0.0.2/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:47:51.443221 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2829 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      327 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-05-29 08:47:51.000000 streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/top_level.txt
```

### Comparing `streamlit_cognite_reveal-0.0.1/LICENSE` & `streamlit_cognite_reveal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_cognite_reveal-0.0.1/PKG-INFO` & `streamlit_cognite_reveal-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: streamlit-cognite-reveal
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
-Author: John Smith
-Author-email: john@example.com
+Author: Anders Hafreager
+Author-email: anders.hafreager@cognite.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
 Requires-Dist: pytest==7.4.0; extra == "devel"
```

### Comparing `streamlit_cognite_reveal-0.0.1/README.md` & `streamlit_cognite_reveal-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_cognite_reveal-0.0.1/reveal/RevealConfig.py` & `streamlit_cognite_reveal-0.0.2/reveal/RevealConfig.py`

 * *Files identical despite different names*

### Comparing `streamlit_cognite_reveal-0.0.1/reveal/__init__.py` & `streamlit_cognite_reveal-0.0.2/reveal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .RevealConfig import RevealConfig
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
 _RELEASE = bool(os.getenv('RELEASE', False))
-
+_RELEASE = True
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
 
 # It's worth noting that this call to `declare_component` is the
```

### Comparing `streamlit_cognite_reveal-0.0.1/setup.py` & `streamlit_cognite_reveal-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-cognite-reveal",
-    version="0.0.1",
-    author="John Smith",
-    author_email="john@example.com",
+    version="0.0.2",
+    author="Anders Hafreager",
+    author_email="anders.hafreager@cognite.com",
     description="Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
     package_data={'': ['frontend/build/**/*']},
     include_package_data=True,
```

### Comparing `streamlit_cognite_reveal-0.0.1/streamlit_cognite_reveal.egg-info/PKG-INFO` & `streamlit_cognite_reveal-0.0.2/streamlit_cognite_reveal.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: streamlit-cognite-reveal
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
-Author: John Smith
-Author-email: john@example.com
+Author: Anders Hafreager
+Author-email: anders.hafreager@cognite.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
 Requires-Dist: pytest==7.4.0; extra == "devel"
```

