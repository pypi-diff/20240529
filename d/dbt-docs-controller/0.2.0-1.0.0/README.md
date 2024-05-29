# Comparing `tmp/dbt_docs_controller-0.2.0.tar.gz` & `tmp/dbt_docs_controller-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_docs_controller-0.2.0.tar", last modified: Wed May 29 17:34:25 2024, max compression
+gzip compressed data, was "dbt_docs_controller-1.0.0.tar", last modified: Wed May 29 17:47:26 2024, max compression
```

## Comparing `dbt_docs_controller-0.2.0.tar` & `dbt_docs_controller-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 17:34:25.760547 dbt_docs_controller-0.2.0/
--rw-rw-rw-   0        0        0     1067 2024-05-29 04:49:27.000000 dbt_docs_controller-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       62 2024-05-29 09:49:47.000000 dbt_docs_controller-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2271 2024-05-29 17:34:25.753448 dbt_docs_controller-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1680 2024-05-29 04:49:41.000000 dbt_docs_controller-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 17:34:25.676012 dbt_docs_controller-0.2.0/SRC/
--rw-rw-rw-   0        0        0      266 2024-05-29 17:03:08.000000 dbt_docs_controller-0.2.0/SRC/__init__.py
--rw-rw-rw-   0        0        0     1342 2024-05-29 17:29:33.000000 dbt_docs_controller-0.2.0/SRC/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:34:25.699117 dbt_docs_controller-0.2.0/SRC/__pycache__/
--rw-rw-rw-   0        0        0      437 2024-05-29 12:17:50.000000 dbt_docs_controller-0.2.0/SRC/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     8101 2024-05-29 10:06:13.000000 dbt_docs_controller-0.2.0/SRC/__pycache__/doc_controller.cpython-311.pyc
--rw-rw-rw-   0        0        0     8217 2024-05-29 12:19:24.000000 dbt_docs_controller-0.2.0/SRC/__pycache__/main.cpython-311.pyc
--rw-rw-rw-   0        0        0     5837 2024-05-29 17:34:16.000000 dbt_docs_controller-0.2.0/SRC/main.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:34:25.751058 dbt_docs_controller-0.2.0/dbt_docs_controller.egg-info/
--rw-rw-rw-   0        0        0     2271 2024-05-29 17:34:24.000000 dbt_docs_controller-0.2.0/dbt_docs_controller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-05-29 17:34:25.000000 dbt_docs_controller-0.2.0/dbt_docs_controller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 17:34:24.000000 dbt_docs_controller-0.2.0/dbt_docs_controller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-29 17:34:24.000000 dbt_docs_controller-0.2.0/dbt_docs_controller.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-05-29 17:34:24.000000 dbt_docs_controller-0.2.0/dbt_docs_controller.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 17:34:25.761149 dbt_docs_controller-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1976 2024-05-29 17:05:41.000000 dbt_docs_controller-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:47:26.514400 dbt_docs_controller-1.0.0/
+-rw-rw-rw-   0        0        0     1067 2024-05-29 04:49:27.000000 dbt_docs_controller-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       62 2024-05-29 09:49:47.000000 dbt_docs_controller-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2271 2024-05-29 17:47:26.510072 dbt_docs_controller-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1680 2024-05-29 04:49:41.000000 dbt_docs_controller-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 17:47:26.430856 dbt_docs_controller-1.0.0/SRC/
+-rw-rw-rw-   0        0        0      266 2024-05-29 17:03:08.000000 dbt_docs_controller-1.0.0/SRC/__init__.py
+-rw-rw-rw-   0        0        0     1342 2024-05-29 17:29:33.000000 dbt_docs_controller-1.0.0/SRC/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:47:26.451907 dbt_docs_controller-1.0.0/SRC/__pycache__/
+-rw-rw-rw-   0        0        0      437 2024-05-29 12:17:50.000000 dbt_docs_controller-1.0.0/SRC/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8101 2024-05-29 10:06:13.000000 dbt_docs_controller-1.0.0/SRC/__pycache__/doc_controller.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8217 2024-05-29 12:19:24.000000 dbt_docs_controller-1.0.0/SRC/__pycache__/main.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5841 2024-05-29 17:40:45.000000 dbt_docs_controller-1.0.0/SRC/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:47:26.504090 dbt_docs_controller-1.0.0/dbt_docs_controller.egg-info/
+-rw-rw-rw-   0        0        0     2271 2024-05-29 17:47:25.000000 dbt_docs_controller-1.0.0/dbt_docs_controller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-05-29 17:47:26.000000 dbt_docs_controller-1.0.0/dbt_docs_controller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:47:25.000000 dbt_docs_controller-1.0.0/dbt_docs_controller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-29 17:47:25.000000 dbt_docs_controller-1.0.0/dbt_docs_controller.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-05-29 17:47:25.000000 dbt_docs_controller-1.0.0/dbt_docs_controller.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:47:26.516223 dbt_docs_controller-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1976 2024-05-29 17:40:54.000000 dbt_docs_controller-1.0.0/setup.py
```

### Comparing `dbt_docs_controller-0.2.0/LICENSE.txt` & `dbt_docs_controller-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt_docs_controller-0.2.0/PKG-INFO` & `dbt_docs_controller-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-docs-controller
-Version: 0.2.0
+Version: 1.0.0
 Summary: dbt-docs-controller streamlines dbt documentation by generating only the relevant models, sources, and components for concise, targeted user information.
 Home-page: https://github.com/Govarthanans8/dbt-docs-controller/tree/main
 Author: Govarthanan S
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dbt_docs_controller-0.2.0/README.md` & `dbt_docs_controller-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_docs_controller-0.2.0/SRC/__main__.py` & `dbt_docs_controller-1.0.0/SRC/__main__.py`

 * *Files identical despite different names*

### Comparing `dbt_docs_controller-0.2.0/SRC/__pycache__/doc_controller.cpython-311.pyc` & `dbt_docs_controller-1.0.0/SRC/__pycache__/doc_controller.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dbt_docs_controller-0.2.0/SRC/__pycache__/main.cpython-311.pyc` & `dbt_docs_controller-1.0.0/SRC/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dbt_docs_controller-0.2.0/SRC/main.py` & `dbt_docs_controller-1.0.0/SRC/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     for package in sorted(packages):
         print(f"macro.{package}")
 
 # Main function to handle models, sources, and macros
 def main(models, sources, macros, actions):
     # Load the manifest.json file
     print("Main Function Execution Begins...")
-    with open('/manifest.json', 'r') as file:
+    with open('../manifest.json', 'r') as file:
         manifest = json.load(file)
 
     # Handle model-related actions
     if 'model' in actions:
         if 'true-all' in models:
             true_docs(manifest)
         elif 'false-all' in models:
@@ -138,15 +138,15 @@
         elif 'list' in macros:
             list_macros(manifest)
             return
         else:
             update_docs_for_macros(manifest, macros)
 
     # Save the updated manifest.json file
-    with open('/manifest.json', 'w') as file:
+    with open('../manifest.json', 'w') as file:
         json.dump(manifest, file, indent=4)
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Manage docs, sources, and macros in manifest.json.")
     parser.add_argument('actions', metavar='A', type=str, nargs='+',
                         help='Specify "model" to update model docs, "source" to update sources, or "macro" to update macros.')
     parser.add_argument('--model', metavar='M', type=str, nargs='*',
```

### Comparing `dbt_docs_controller-0.2.0/dbt_docs_controller.egg-info/PKG-INFO` & `dbt_docs_controller-1.0.0/dbt_docs_controller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-docs-controller
-Version: 0.2.0
+Version: 1.0.0
 Summary: dbt-docs-controller streamlines dbt documentation by generating only the relevant models, sources, and components for concise, targeted user information.
 Home-page: https://github.com/Govarthanans8/dbt-docs-controller/tree/main
 Author: Govarthanan S
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dbt_docs_controller-0.2.0/setup.py` & `dbt_docs_controller-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import codecs
 
 with codecs.open('README.md', 'r', 'utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dbt-docs-controller',
-    version='0.2.0',
+    version='1.0.0',
     packages=find_packages(),
     package_dir={},
     entry_points={
         'console_scripts': [
             'dbt-docs-controller=SRC.__main__:main_wrapper',
         ],
     },
```

