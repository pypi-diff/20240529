# Comparing `tmp/plegui-1.1.2.tar.gz` & `tmp/plegui-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plegui-1.1.2.tar", last modified: Thu May 23 21:22:23 2024, max compression
+gzip compressed data, was "plegui-1.1.9.tar", last modified: Wed May 29 22:19:19 2024, max compression
```

## Comparing `plegui-1.1.2.tar` & `plegui-1.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 21:22:23.119540 plegui-1.1.2/
--rw-rw-rw-   0        0        0     1190 2024-05-23 21:22:23.104540 plegui-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      779 2024-05-23 21:22:00.000000 plegui-1.1.2/README.md
--rw-rw-rw-   0        0        0     1103 2024-05-15 20:32:47.000000 plegui-1.1.2/license
-drwxrwxrwx   0        0        0        0 2024-05-23 21:22:23.093541 plegui-1.1.2/plegui.egg-info/
--rw-rw-rw-   0        0        0     1190 2024-05-23 21:22:21.000000 plegui-1.1.2/plegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-23 21:22:22.000000 plegui-1.1.2/plegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 21:22:21.000000 plegui-1.1.2/plegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 21:22:21.000000 plegui-1.1.2/plegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 21:22:23.119540 plegui-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      725 2024-05-23 21:19:32.000000 plegui-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 22:19:19.449875 plegui-1.1.9/
+-rw-rw-rw-   0        0        0     1202 2024-05-29 22:19:19.449875 plegui-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      779 2024-05-23 21:22:00.000000 plegui-1.1.9/README.md
+-rw-rw-rw-   0        0        0     1103 2024-05-15 20:32:47.000000 plegui-1.1.9/license
+drwxrwxrwx   0        0        0        0 2024-05-29 22:19:19.449875 plegui-1.1.9/plegui.egg-info/
+-rw-rw-rw-   0        0        0     1202 2024-05-29 22:19:19.000000 plegui-1.1.9/plegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-05-29 22:19:19.000000 plegui-1.1.9/plegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 22:19:19.000000 plegui-1.1.9/plegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 22:19:19.000000 plegui-1.1.9/plegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 22:19:19.449875 plegui-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      737 2024-05-29 22:18:42.000000 plegui-1.1.9/setup.py
```

### Comparing `plegui-1.1.2/PKG-INFO` & `plegui-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: plegui
-Version: 1.1.2
-Summary: A library used to make GUIs and Messages boxes
+Version: 1.1.9
+Summary: A library used to make GUIs and Messages boxes and other..
 Author: PyGaps CEO
 Author-email: soqratiakram33@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `plegui-1.1.2/README.md` & `plegui-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `plegui-1.1.2/license` & `plegui-1.1.9/license`

 * *Files identical despite different names*

### Comparing `plegui-1.1.2/plegui.egg-info/PKG-INFO` & `plegui-1.1.9/plegui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: plegui
-Version: 1.1.2
-Summary: A library used to make GUIs and Messages boxes
+Version: 1.1.9
+Summary: A library used to make GUIs and Messages boxes and other..
 Author: PyGaps CEO
 Author-email: soqratiakram33@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `plegui-1.1.2/setup.py` & `plegui-1.1.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="plegui",
-    version="1.1.2",
-    description="A library used to make GUIs and Messages boxes",
+    version="1.1.9",
+    description="A library used to make GUIs and Messages boxes and other..",
     long_description=README,
     long_description_content_type="text/markdown",
     author="PyGaps CEO",
     author_email="soqratiakram33@gmail.com",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

