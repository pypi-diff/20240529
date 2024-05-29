# Comparing `tmp/lenscraft-1.0.4.tar.gz` & `tmp/lenscraft-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenscraft-1.0.4.tar", last modified: Tue Apr 30 14:42:07 2024, max compression
+gzip compressed data, was "lenscraft-1.1.0.tar", last modified: Wed May 29 13:32:11 2024, max compression
```

## Comparing `lenscraft-1.0.4.tar` & `lenscraft-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-23 18:41:25.000000 lenscraft-1.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-23 19:08:22.000000 lenscraft-1.0.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-23 18:41:25.000000 lenscraft-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1300 2024-04-30 14:42:07.294971 lenscraft-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-23 19:24:28.000000 lenscraft-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.290971 lenscraft-1.0.4/images/
--rw-rw-rw-   0 root         (0) root         (0)   776666 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/0.9858_1.1766.png
--rw-rw-rw-   0 root         (0) root         (0)   192094 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/334.png
--rw-rw-rw-   0 root         (0) root         (0)  4916278 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/Ring_9_9.png
--rw-rw-rw-   0 root         (0) root         (0)    15666 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/mask.png
--rw-rw-rw-   0 root         (0) root         (0)   755205 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/spacer_top__13.png
--rw-rw-rw-   0 root         (0) root         (0)   609893 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/spacer_top__14.png
--rw-rw-rw-   0 root         (0) root         (0)   750759 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/spacer_top__3.png
--rw-rw-rw-   0 root         (0) root         (0)   916168 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/spacer_top__9.png
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-23 19:08:22.000000 lenscraft-1.0.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-23 18:41:25.000000 lenscraft-1.0.4/requirments.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 14:42:07.294971 lenscraft-1.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.286971 lenscraft-1.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 19:00:28.000000 lenscraft-1.0.4/src/lenscraft/__main__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft/_version.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft/assets/
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/assets/CornerTemplate.png
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft/editor/
--rw-rw-rw-   0 root         (0) root         (0)     5370 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/editor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7721 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/gabor.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/image.py
--rw-rw-rw-   0 root         (0) root         (0)    17849 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft/texture/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/texture/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/texture/classify.py
--rw-rw-rw-   0 root         (0) root         (0)    14493 2024-04-30 14:38:40.000000 lenscraft-1.0.4/src/lenscraft/texture/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1300 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      877 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      126 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.653898 lenscraft-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3968 2024-05-29 13:24:23.000000 lenscraft-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-23 19:08:22.000000 lenscraft-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-23 18:41:25.000000 lenscraft-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-05-29 13:32:11.653898 lenscraft-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-23 19:24:28.000000 lenscraft-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.633897 lenscraft-1.1.0/images/
+-rw-rw-rw-   0 root         (0) root         (0)   776666 2024-04-23 18:41:25.000000 lenscraft-1.1.0/images/0.9858_1.1766.png
+-rw-rw-rw-   0 root         (0) root         (0)   192094 2024-04-23 18:41:25.000000 lenscraft-1.1.0/images/334.png
+-rw-rw-rw-   0 root         (0) root         (0)  4916278 2024-04-23 18:41:25.000000 lenscraft-1.1.0/images/Ring_9_9.png
+-rw-rw-rw-   0 root         (0) root         (0)    15666 2024-04-23 18:41:25.000000 lenscraft-1.1.0/images/mask.png
+-rw-rw-rw-   0 root         (0) root         (0)   755205 2024-04-23 18:41:25.000000 lenscraft-1.1.0/images/spacer_top__13.png
+-rw-rw-rw-   0 root         (0) root         (0)   609893 2024-04-23 18:41:25.000000 lenscraft-1.1.0/images/spacer_top__14.png
+-rw-rw-rw-   0 root         (0) root         (0)   750759 2024-04-23 18:41:25.000000 lenscraft-1.1.0/images/spacer_top__3.png
+-rw-rw-rw-   0 root         (0) root         (0)   916168 2024-04-23 18:41:25.000000 lenscraft-1.1.0/images/spacer_top__9.png
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-29 13:24:23.000000 lenscraft-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-05-29 13:24:23.000000 lenscraft-1.1.0/requirments.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 13:32:11.653898 lenscraft-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.597895 lenscraft-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.641898 lenscraft-1.1.0/src/lenscraft/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.1.0/src/lenscraft/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 19:00:28.000000 lenscraft-1.1.0/src/lenscraft/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-29 13:32:11.000000 lenscraft-1.1.0/src/lenscraft/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-23 18:41:25.000000 lenscraft-1.1.0/src/lenscraft/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.641898 lenscraft-1.1.0/src/lenscraft/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-23 18:41:25.000000 lenscraft-1.1.0/src/lenscraft/assets/CornerTemplate.png
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 18:41:25.000000 lenscraft-1.1.0/src/lenscraft/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.645898 lenscraft-1.1.0/src/lenscraft/editor/
+-rw-rw-rw-   0 root         (0) root         (0)     6320 2024-05-28 16:58:24.000000 lenscraft-1.1.0/src/lenscraft/editor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2024-05-29 13:24:23.000000 lenscraft-1.1.0/src/lenscraft/gabor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5774 2024-04-23 18:41:25.000000 lenscraft-1.1.0/src/lenscraft/image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.645898 lenscraft-1.1.0/src/lenscraft/node/
+-rw-rw-rw-   0 root         (0) root         (0)     3942 2024-05-29 13:24:23.000000 lenscraft-1.1.0/src/lenscraft/node/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2729 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     6571 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/editor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.649898 lenscraft-1.1.0/src/lenscraft/node/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/nodes/canny.py
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/nodes/img_library.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/nodes/minmax.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/nodes/show_feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/nodes/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     3143 2024-05-28 16:58:24.000000 lenscraft-1.1.0/src/lenscraft/node/nodes/texture.py
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/node/nodes/threshold.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.649898 lenscraft-1.1.0/src/lenscraft/texture/
+-rw-rw-rw-   0 root         (0) root         (0)      888 2024-05-28 16:58:24.000000 lenscraft-1.1.0/src/lenscraft/texture/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3349 2024-05-28 16:58:24.000000 lenscraft-1.1.0/src/lenscraft/texture/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    17507 2024-05-28 17:02:30.000000 lenscraft-1.1.0/src/lenscraft/texture/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-05-22 19:35:33.000000 lenscraft-1.1.0/src/lenscraft/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.653898 lenscraft-1.1.0/src/lenscraft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-05-29 13:32:11.000000 lenscraft-1.1.0/src/lenscraft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1267 2024-05-29 13:32:11.000000 lenscraft-1.1.0/src/lenscraft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 13:32:11.000000 lenscraft-1.1.0/src/lenscraft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-29 13:32:11.000000 lenscraft-1.1.0/src/lenscraft.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-29 13:32:11.000000 lenscraft-1.1.0/src/lenscraft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 13:32:11.000000 lenscraft-1.1.0/src/lenscraft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:32:11.649898 lenscraft-1.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.1.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2024-05-22 19:35:33.000000 lenscraft-1.1.0/tests/test_node_graph.py
```

### Comparing `lenscraft-1.0.4/.gitignore` & `lenscraft-1.1.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+/models
+
 .DS_Store
 .python-version
 
 _db/
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
+_version.py
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
```

### Comparing `lenscraft-1.0.4/LICENSE` & `lenscraft-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/PKG-INFO` & `lenscraft-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: lenscraft
-Version: 1.0.4
+Version: 1.1.0
 Summary: Application to quickly build machine vision pipelines with little or no code
 Author-email: Gudjon Einar Magnusson <gmagnusson@fraunhofer.org>
 Project-URL: Homepage, https://cma.fraunhofer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dearpygui==1.10.0
 Requires-Dist: numpy==1.26.4
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: pillow==10.2.0
-Requires-Dist: scikit-learn==1.4.1.post1
-Requires-Dist: scipy==1.12.0
 Requires-Dist: shapely==2.0.3
+Requires-Dist: keras==3.3.3
 
 # Lenscraft
 
 This application allows users to create and tweak a custom computer vision pipeline for micro-assembly
 
 ## How to run
 Install the package from pypi
```

### Comparing `lenscraft-1.0.4/README.md` & `lenscraft-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/images/0.9858_1.1766.png` & `lenscraft-1.1.0/images/0.9858_1.1766.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/images/334.png` & `lenscraft-1.1.0/images/334.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/images/Ring_9_9.png` & `lenscraft-1.1.0/images/Ring_9_9.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/images/mask.png` & `lenscraft-1.1.0/images/mask.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/images/spacer_top__13.png` & `lenscraft-1.1.0/images/spacer_top__13.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/images/spacer_top__14.png` & `lenscraft-1.1.0/images/spacer_top__14.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/images/spacer_top__3.png` & `lenscraft-1.1.0/images/spacer_top__3.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/images/spacer_top__9.png` & `lenscraft-1.1.0/images/spacer_top__9.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/pyproject.toml` & `lenscraft-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "dearpygui==1.10.0",
     "numpy==1.26.4",
     "opencv-python==4.9.0.80",
     "pillow==10.2.0",
-    "scikit-learn==1.4.1.post1",
-    "scipy==1.12.0",
-    "shapely==2.0.3"
+    "shapely==2.0.3",
+    "keras==3.3.3"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `lenscraft-1.0.4/src/lenscraft/assets/CornerTemplate.png` & `lenscraft-1.1.0/src/lenscraft/assets/CornerTemplate.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/src/lenscraft/editor/__init__.py` & `lenscraft-1.1.0/src/lenscraft/editor/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import dearpygui.dearpygui as dpg
 import json
 
 from lenscraft.image import ImageLibrary
-from lenscraft.nodes import NodeEditor
+from lenscraft.node.editor import Graph, NodeEditor
+from lenscraft.node.nodes.img_library import ImageLibraryNode
 from lenscraft.texture import TextureModelLibrary
 from lenscraft.texture.tool import TextureClassifierTool
 
+
 def print_me(sender):
     print(f"Menu Item: {sender}")
 
 
 class EditorWindow:
-    def __init__(self, image_library: ImageLibrary, texture_library: TextureModelLibrary):
+    def __init__(
+        self, image_library: ImageLibrary, texture_library: TextureModelLibrary
+    ):
         self.image_library = image_library
         self.texture_library = texture_library
         self.texture_tool = TextureClassifierTool(image_library, texture_library)
+        self.node_editor = NodeEditor(self.image_library, self.texture_library)
 
     def load_project_callback(self, caller, app_data):
         print(f"Load project {app_data}")
         project_file_path = app_data["file_path_name"]
         self.load_project(file_path=project_file_path)
 
     def load_project(self, file_path="project.json"):
@@ -26,50 +31,61 @@
         try:
             with open(file_path, "r") as file:
                 project = json.load(file)
                 print(project)
                 for path in project["images"]:
                     self.image_library.load(path)
 
+                graph = Graph().load(project["graph"], self.node_editor)
+                self.node_editor.set_graph(graph)
+
             self.update_images()
 
         except FileNotFoundError:
             print(f"No saved image selection found at '{file_path}'")
 
-
     def save_project_callback(self, caller, app_data):
         print(f"Save project {app_data}")
         project_file_path = app_data["file_path_name"]
         self.save_project(project_file_path)
 
+    def clear_node_editor(self):
+        self.node_editor.clear()
+        graph = self.create_default_graph()
+        self.node_editor.set_graph(graph)
+
     def save_project(self, project_file_path):
         try:
+            graph = self.node_editor.graph.to_json()
+
             with open(project_file_path, "w") as file:
                 image_paths = [img.path for img in self.image_library.images]
-                json.dump({"images": image_paths}, file)
+                json.dump({"images": image_paths, "graph": graph}, file)
 
         except Exception as ex:
             print(ex)
 
-
     def load_images(self, sender, app_data):
         for name, path in app_data["selections"].items():
             print(f"Load image {path}")  # Use print for demonstration
             self.image_library.load(path)
 
         self.update_images()
 
-
     def update_images(self):
         dpg.delete_item("image_row", children_only=True)  # Clear existing images
 
         with dpg.group(parent="image_row", horizontal=True):
             for image in self.image_library.images:
                 image.show_in_context()
 
+    def create_default_graph(self):
+        graph = Graph()
+        graph.add_node(ImageLibraryNode(self.node_editor))
+        return graph
 
     def add_to_context(self):
         # Create a window that fills the viewport and cannot be moved or closed
         with dpg.window(
             tag="primary",
             no_move=True,
             no_close=True,
@@ -116,23 +132,27 @@
                 callback=self.load_project_callback,
                 id="load_project_dialog",
                 width=700,
                 height=400,
             ):
                 dpg.add_file_extension(".json", color=(0, 255, 255, 255))
 
-            editor = NodeEditor(self.image_library, self.texture_library)
             with dpg.child_window(label="Node Editor", width=-1):
-                editor.add_to_context()
+                self.node_editor.add_to_context()
+                # Create default graph
+                graph = self.create_default_graph()
+                self.node_editor.set_graph(graph)
 
             self.texture_tool.add_to_context()
 
+
 def run_gui():
     image_library = ImageLibrary()
     texture_library = TextureModelLibrary()
+    texture_library.find_models_in_directory("./models")
     editor = EditorWindow(image_library, texture_library)
 
     dpg.create_context()
 
     # Create a viewport
     viewport_width = 1024
     viewport_height = 800
@@ -142,25 +162,30 @@
 
     with dpg.viewport_menu_bar():
         with dpg.menu(label="File"):
             dpg.add_menu_item(
                 label="Add Images", callback=lambda: dpg.show_item("file_dialog_id")
             )
             dpg.add_menu_item(
-                label="Load Project", callback=lambda: dpg.show_item("load_project_dialog")
+                label="Load Project",
+                callback=lambda: dpg.show_item("load_project_dialog"),
             )
             dpg.add_menu_item(
-                label="Save Project", callback=lambda: dpg.show_item("save_project_dialog")
+                label="Save Project",
+                callback=lambda: dpg.show_item("save_project_dialog"),
+            )
+            dpg.add_menu_item(
+                label="Clear",
+                callback=editor.clear_node_editor,
             )
 
         dpg.add_menu_item(label="Help", callback=print_me)
 
     editor.add_to_context()
 
-
     dpg.setup_dearpygui()
     dpg.show_viewport()
     dpg.set_primary_window("primary", True)
 
     dpg.start_dearpygui()
 
-    dpg.destroy_context()
+    dpg.destroy_context()
```

### Comparing `lenscraft-1.0.4/src/lenscraft/image.py` & `lenscraft-1.1.0/src/lenscraft/image.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.4/src/lenscraft/texture/__init__.py` & `lenscraft-1.1.0/src/lenscraft/texture/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+import os
 from typing import List
 import logging
+import glob
 
 
 class TextureModelLibrary:
     def __init__(self):
         self.models: List[str] = []
         self._on_update_callbacks = []
 
+    def find_models_in_directory(self, path):
+        model_files = glob.glob("*.keras", root_dir=path)
+        for file in model_files:
+            self.models.append(os.path.join(path, file))
+        self._trigger_on_update()
+
     def add_model(self, path):
         self.models.append(path)
         self._trigger_on_update()
 
     def on_update(self, callback):
         """Register callback that will be called if the list of images changes"""
         self._on_update_callbacks.append(callback)
```

### Comparing `lenscraft-1.0.4/src/lenscraft/texture/classify.py` & `lenscraft-1.1.0/src/lenscraft/texture/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,112 @@
-import pickle
+import os
 import numpy as np
-from sklearn.model_selection import train_test_split
-from sklearn.svm import SVC
-from sklearn.metrics import accuracy_score, classification_report
+import tensorflow as tf
+import keras
+from keras.api.layers import Dense, Input
+from keras.api.callbacks import Callback
 
-class RedBlue:
+TEXTURE_MODEL_DIR = "models"
+TRAIN_RATIO = 0.8
+
+
+def standardize(data):
+    mean = tf.reduce_mean(data, axis=0)
+    stddev = tf.math.reduce_std(data, axis=0)
+    return (data - mean) / stddev
+
+
+class ModelBuilder:
     def __init__(self):
         self.red = None
         self.blue = None
-        self.model = SVC(kernel="rbf")
 
     def add_red(self, features):
         if self.red is None:
             self.red = features
         else:
             self.red = np.vstack((self.red, features))
 
     def add_blue(self, features):
         if self.blue is None:
             self.blue = features
         else:
             self.blue = np.vstack((self.blue, features))
 
     def save(self, name):
-        model_path = f"models/{name}.pkl"
-        with open(model_path, "wb") as file:
-            pickle.dump(self.model, file)
+        os.makedirs(TEXTURE_MODEL_DIR, exist_ok=True)
+        model_path = os.path.join(TEXTURE_MODEL_DIR, f"{name}.keras")
+        model = ClassificationModel(self.model)
+        model.save(model_path)
 
         return model_path
+    
+    def _build_model(self, input_shape):
+        model = keras.Sequential()
+        model.add(Input(input_shape))
+        model.add(Dense(60, activation="relu"))
+        model.add(Dense(10, activation="relu"))
+        model.add(Dense(1, activation="sigmoid"))
 
-    def train(self):
+        return model
+
+    def train(self, callback=None):
         # Combine the feature vectors
         X = np.vstack((self.red, self.blue))
-
         # Create labels (0 for the first set, 1 for the second set)
         y = np.array([0] * len(self.red) + [1] * len(self.blue))
 
-        X_train, X_test, y_train, y_test = train_test_split(
-            X, y, test_size=0.1, random_state=42
-        )
-
-        print("Train:", X_train.shape)
-
-
-        # Train the SVM model
-        self.model.fit(X_train, y_train)
-
-        # Predict labels for the test set
-        y_pred = self.model.predict(X_test)
+        total_samples = X.shape[0]
+        train_samples = int(total_samples * TRAIN_RATIO)
 
-        # Calculate the accuracy
-        accuracy = accuracy_score(y_test, y_pred)
-        print(f"Accuracy: {accuracy:.2f}")
+        # Shuffle the data
+        indices = tf.range(start=0, limit=total_samples, dtype=tf.int32)
+        shuffled_indices = tf.random.shuffle(indices)
 
-        # Detailed classification report
-        print(classification_report(y_test, y_pred))
+        X = tf.gather(X, shuffled_indices).numpy()
+        y = tf.gather(y, shuffled_indices).numpy()
 
-        # feature_map = features.all()
-        # # Predict the class for each pixel's feature vector
-        # predictions = model.predict(feature_map)
+        # Split the data
+        X_train, X_test = X[:train_samples], X[train_samples:]
+        y_train, y_test = y[:train_samples], y[train_samples:]
 
-        # # Reshape the predictions back to the original image shape
-        # # Assume `original_image_shape` is a tuple with the shape of the original image (height, width)
-        # (w, h) = features.flat_shape()
-        # classification_image = predictions.reshape((h, w))
+        X_train = standardize(X_train)
+        X_test = standardize(X_test)
 
-        # # For visualization, scale the classification image to full 8-bit range if it's binary
-        # # This step is optional and depends on how you want to visualize the result
-        # classification_image_scaled = (classification_image * 255).astype(np.uint8)
+        self.model = self._build_model(input_shape=(X_train.shape[1],))
 
-        # # Save or display the classification image
-        # cv2.imwrite('classification_image.png', classification_image_scaled)
-        # dpg.set_value(mask_id, mask_to_data(classification_image))
-
-        print("Done")
-        return self.model
-
-        # # To load the model
-        # with open('svc_model.pkl', 'rb') as file:
-        #     model = pickle.load(file)
+        # Compile the model
+        self.model.compile(
+            optimizer="adam", loss="binary_crossentropy", metrics=["accuracy"]
+        )
 
+        # Train the model
+        callbacks = []
+        if callback is not None:
+            callbacks.append(callback)
+        self.model.fit(X_train, y_train, epochs=50, batch_size=32, validation_split=0.2, callbacks=callbacks, verbose=False)
+
+        # Evaluate the model
+        loss, accuracy = self.model.evaluate(X_test, y_test, callbacks=callbacks, verbose=False)
+        print(f"Test accuracy: {accuracy}")
+
+        classification_model = ClassificationModel(self.model)
+        classification_model.save("keras_mlp_model.keras")
+        
+        return classification_model
+
+class ClassificationModel:
+    def __init__(self, model: keras.Sequential):
+        self.model = model
+
+    def save(self, path):
+        self.model.save(path)
+
+    def predict(self, X):
+        y = self.model.predict(standardize(X), batch_size=10000)
+
+        return y
+
+    @staticmethod
+    def load(path):
+        model = keras.models.load_model(path)
+        return ClassificationModel(model)
```

### Comparing `lenscraft-1.0.4/src/lenscraft/texture/tool.py` & `lenscraft-1.1.0/src/lenscraft/texture/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,209 @@
 import time
 from typing import List, Optional
 import dearpygui.dearpygui as dpg
 import numpy as np
 import shapely
 from shapely.affinity import scale, translate
-import cv2
+from keras.api.callbacks import Callback
 
 from lenscraft.image import Image, ImageLibrary
 from lenscraft.texture import TextureModelLibrary
-from lenscraft.texture.classify import RedBlue
 from lenscraft.gabor import Gabor
+from lenscraft.texture.model import ModelBuilder
+
 
 def arr_to_data(arr):
     auxImg = np.asfarray(arr, dtype="f")
     auxImg = auxImg.ravel()
     auxImg = np.true_divide(auxImg, 255.0)
     return auxImg
 
+
 def mask_to_data(mask):
     # Convert binary mask to an RGBA image where RGB channels follow the mask
     # and the alpha channel is set to 127 for 50% opacity
     rgba_image = np.zeros(
         (mask.shape[0], mask.shape[1], 4), dtype=np.float32
     )  # Create a 4-channel image
     rgba_image[:, :, :3] = mask[:, :, None] * 255  # Set RGB channels
     rgba_image[:, :, 3] = 128  # Set alpha channel to 50% opacity
 
     # Flatten the image and normalize to [0, 1]
     texture_data = rgba_image.ravel() / 255.0
 
     return texture_data
 
+
 class ImageTab:
     def __init__(self, tab, image: Image, canvas):
         self.tab_id = tab
         self.image = image
         self.canvas_id = canvas
         self.mask_texture_id = None
         self.mask = None
 
     def canvas_origin(self):
         (x, y) = dpg.get_item_pos(self.canvas_id)
-        return (x+9, y+32)
-    
+        return (x + 9, y + 32)
+
     def clear(self):
         if self.mask:
             dpg.delete_item(self.mask)
             self.mask = None
 
     def add_mask(self, mask):
         h, w = mask.shape[:2]
         if self.mask_texture_id is None:
             with dpg.texture_registry():
-                self.mask_texture_id = dpg.add_dynamic_texture(h, w, default_value=mask_to_data(mask))
+                self.mask_texture_id = dpg.add_dynamic_texture(
+                    h, w, default_value=mask_to_data(mask)
+                )
         else:
             dpg.set_value(self.mask_texture_id, mask_to_data(mask))
 
         w, h = dpg.get_item_rect_size(self.canvas_id)
-        self.mask = dpg.draw_image(self.mask_texture_id, (0,0), (w,h), parent=self.canvas_id)
+        self.mask = dpg.draw_image(
+            self.mask_texture_id, (0, 0), (w, h), parent=self.canvas_id
+        )
 
     def polygon_to_image_space(self, screen_polygon):
         (width, height) = dpg.get_item_rect_size(self.canvas_id)
         offset_x, offset_y = self.canvas_origin()
 
         scale_x = self.image.width / width
         scale_y = self.image.height / height
 
-        scaled_polygon = scale(screen_polygon, xfact=scale_x, yfact=scale_y, origin=(0, 0))
+        scaled_polygon = scale(
+            screen_polygon, xfact=scale_x, yfact=scale_y, origin=(0, 0)
+        )
         translated_polygon = translate(scaled_polygon, xoff=offset_x, yoff=offset_y)
 
         return translated_polygon
 
+
+class TrainingProgressWindow(Callback):
+    def __init__(self):
+        self.id = "training_progress_popup"
+        self.is_complete = False
+
+    def on_epoch_end(self, epoch, logs=None):
+        progress = epoch / 50.0
+        dpg.set_value(self.progress_bar, progress)
+
+    def on_train_end(self, logs=None):
+        self.is_complete = True
+        self.enable_close_button()
+
+    def on_predict_end(self, logs=None):
+        print("on_predict_end", logs)
+
+    def on_test_end(self, logs=None):
+        if self.is_complete:
+            dpg.set_value(
+                self.message, f"Training Complete. Test Accuracy: {logs['accuracy']}"
+            )
+            dpg.show_item(self.message)
+
+    def show(self, parent="TextureToolWindow"):
+        # Get the size of the parent window
+        parent_width = dpg.get_item_width(parent)
+        parent_height = dpg.get_item_height(parent)
+
+        # Define the size of the popup window
+        popup_width = 400
+        popup_height = 150
+
+        # Calculate the center position
+        pos_x = (parent_width - popup_width) // 2
+        pos_y = (parent_height - popup_height) // 2
+
+        # Set the position and show the popup
+        dpg.configure_item(
+            self.id,
+            pos=(pos_x, pos_y),
+            width=popup_width,
+            height=popup_height,
+            show=True,
+        )
+
+    def hide(self):
+        dpg.hide_item(self.id)
+
+    def add_to_context(self):
+        with dpg.window(
+            label="Progress Popup", modal=True, show=False, tag=self.id, no_close=True
+        ):
+            dpg.add_text("Training a texture classifier. This may take a minute")
+            self.progress_bar = dpg.add_progress_bar(
+                label="Progress", default_value=0.0, width=-1, tag="progress_bar"
+            )
+
+            self.message = dpg.add_text("", show=False)
+            self.ok_btn = dpg.add_button(
+                label="OK", callback=self._on_ok_btn, show=False
+            )
+
+    def enable_close_button(self):
+        dpg.show_item(self.ok_btn)
+
+    def _on_ok_btn(self, sender):
+        self.hide()
+
+
 class TextureClassifierTool:
-    def __init__(self, image_library: ImageLibrary, texture_library: TextureModelLibrary):
+    def __init__(
+        self, image_library: ImageLibrary, texture_library: TextureModelLibrary
+    ):
         self.id = "TextureToolWindow"  # dpg.generate_uuid()
         self.image_library = image_library
         self.texture_library = texture_library
         self.image_library.on_update(self._on_image_added)
         self.borders: List[TextureBorder] = []
         self.current_model = None
         self.model_name = "my-texture"
+        self.training_window = TrainingProgressWindow()
 
         self._current_tab_id = None
         self._tabs = {}
         self._masks = {}
 
     def load_image(self):
         pass
 
-    def do_train(self):
-        redblue = RedBlue()
+    def do_train_nn(self):
+        model_builder = ModelBuilder()
         gabor = Gabor()
         feature_tab_map = {}
+        self.training_window.show()
+
+        # Gather training data
         for border in self.borders:
             if border.tab.tab_id in feature_tab_map:
                 features = feature_tab_map[border.tab.tab_id]
             else:
                 features = gabor.load_features(border.tab.image.path)
                 feature_tab_map[border.tab.tab_id] = features
-            
+
             inside, outside = border.extract_features(features)
-            redblue.add_blue(inside)
-            redblue.add_red(outside)
+            model_builder.add_blue(inside)
+            model_builder.add_red(outside)
 
-        model = redblue.train()
+        # Train model
+        model = model_builder.train(callback=self.training_window)
 
+        # Run prediction on sample image
         features = feature_tab_map[border.tab.tab_id]
         fv = features.all()
         result = model.predict(fv).reshape(features.flat_shape())
-        #result = (result * 255).astype(np.uint8)
-        cv2.imwrite('classification_image.png', result)
         self.current_tab().add_mask(result)
-        self.current_model = redblue
+        self.current_model = model_builder
+
+        dpg.show_item("group_save_model")
+        dpg.hide_item("group_create_model")
 
     def _on_tab_switch(self, sender, app_data):
         self._current_tab_id = app_data
 
     def _on_model_name_change(self, sender, app_data):
         self.model_name = app_data
 
@@ -132,15 +220,15 @@
                 with dpg.drawlist(width=w, height=h) as canvas:
                     image.draw_image(width=w)
                 self._tabs[tab] = ImageTab(tab, image, canvas)
 
     def _on_mouse_click(self):
         if not dpg.is_item_visible(self.id):
             return
-        
+
         current_tab = self.current_tab()
         if not current_tab:
             return
         canvas = self._tabs[current_tab.tab_id].canvas_id
         if not dpg.is_item_hovered(canvas):
             return
 
@@ -180,30 +268,32 @@
         self.borders = []
         self._update_border_list()
 
     def save_model(self):
         if self.current_model is None:
             print("No model to save")
             return
-        
+
         new_path = self.current_model.save(self.model_name)
         self.texture_library.add_model(new_path)
 
+        dpg.hide_item(self.id)
+
     def start_new_border(self):
         canvas = self.current_tab().canvas_id
         start = self.mouse_image_coordinates()
         print("Start:", start)
         new_line = TextureBorder(self.current_tab(), start)
         self.borders.append(new_line)
         self._update_border_list()
 
     def current_tab(self) -> Optional[ImageTab]:
         if self._current_tab_id is None:
             return None
-        
+
         return self._tabs[self._current_tab_id]
 
     def current_canvas(self):
         return self.current_tab().canvas_id
 
     def _update_border_list(self):
         # Clear the list
@@ -212,14 +302,19 @@
         # Re-Render the list
         for i, border in enumerate(self.borders):
             with dpg.child_window(height=70, autosize_x=True, parent="border_list"):
                 with dpg.group(horizontal=True):
                     dpg.add_button(label="X", width=20, height=50)
                     dpg.add_text(f"Border {i}")
 
+        if len(self.borders) > 0:
+            dpg.show_item("group_create_model")
+        else:
+            dpg.hide_item("group_create_model")
+
     def add_to_context(self):
         # Create a window that fills the viewport and cannot be moved or closed
         with dpg.window(
             tag=self.id,
             label="TextureClassifierTool",
             no_collapse=True,
             show=False,
@@ -250,29 +345,40 @@
                                 "Draw one or more texture boundaries on your images to train a texture classifier",
                                 wrap=150,
                             )
 
                     with dpg.child_window(border=False, tag="border_list", height=-100):
                         pass
 
-                    dpg.add_button(
-                        label="Train", height=25, width=-1, callback=self.do_train
-                    )
+                    with dpg.group(tag="group_create_model", show=False):
+                        dpg.add_button(
+                            label="Train",
+                            height=25,
+                            width=-1,
+                            callback=self.do_train_nn,
+                        )
                     dpg.add_button(
                         label="Reset", height=25, width=-1, callback=self.clear
                     )
-                    dpg.add_input_text(label="Name", default_value=self.model_name, callback=self._on_model_name_change)
-                    dpg.add_button(
-                        label="Save", height=25, width=-1, callback=self.save_model
-                    )
+                    with dpg.group(tag="group_save_model", show=False):
+                        dpg.add_input_text(
+                            label="Name",
+                            default_value=self.model_name,
+                            callback=self._on_model_name_change,
+                        )
+                        dpg.add_button(
+                            label="Save", height=25, width=-1, callback=self.save_model
+                        )
 
         with dpg.handler_registry():
             dpg.add_mouse_release_handler(callback=self._on_mouse_click)
             dpg.add_mouse_move_handler(callback=self._on_mouse_move)
 
+        self.training_window.add_to_context()
+
 
 class TextureBorder:
     def __init__(self, tab: ImageTab, start=None, end=None, width=10):
         self.tab = tab
         self.start = np.array(start) if start else None
         self.end = np.array(end) if end else None
         self.done = False
@@ -315,19 +421,19 @@
             dpg.delete_item(self.inside_polygon_id)
 
     def draw(self):
         dt = time.time() - self._last_draw
         if dt < 0.05:
             # Prevent drawing too fast
             return
-        
+
         if np.array_equal(self.start, self.end):
             # Dont draw unless there is some distance between start and end
             return
-        
+
         self.draw_line()
         self.draw_rectangles()
         self._last_draw = time.time()
 
     def draw_line(self):
         if self.line_id and dpg.does_item_exist(self.line_id):
             dpg.delete_item(self.line_id)
```

### Comparing `lenscraft-1.0.4/src/lenscraft/utils.py` & `lenscraft-1.1.0/src/lenscraft/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 import threading
+import nanoid
+
+ID_ALPHABET = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+ID_SIZE = 6
 
 def debounce(wait):
     """ Decorator that will postpone a function's
         execution until after `wait` seconds
         have elapsed since the last time it was invoked. """
     def decorator(fn):
         def debounced(*args, **kwargs):
@@ -12,8 +16,15 @@
             if hasattr(debounced, '_timer'):
                 debounced._timer.cancel()
             
             debounced._timer = threading.Timer(wait, call_it)
             debounced._timer.start()
         
         return debounced
-    return decorator
+    return decorator
+
+def uid() -> str:
+    """Returns a string that is likely to be unique.
+    Works well if you are generating hundreds or maybe thousands of ids.
+    If you need millions of ids, do something else
+    """
+    return nanoid.generate(ID_ALPHABET, 6)
```

### Comparing `lenscraft-1.0.4/src/lenscraft.egg-info/PKG-INFO` & `lenscraft-1.1.0/src/lenscraft.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: lenscraft
-Version: 1.0.4
+Version: 1.1.0
 Summary: Application to quickly build machine vision pipelines with little or no code
 Author-email: Gudjon Einar Magnusson <gmagnusson@fraunhofer.org>
 Project-URL: Homepage, https://cma.fraunhofer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dearpygui==1.10.0
 Requires-Dist: numpy==1.26.4
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: pillow==10.2.0
-Requires-Dist: scikit-learn==1.4.1.post1
-Requires-Dist: scipy==1.12.0
 Requires-Dist: shapely==2.0.3
+Requires-Dist: keras==3.3.3
 
 # Lenscraft
 
 This application allows users to create and tweak a custom computer vision pipeline for micro-assembly
 
 ## How to run
 Install the package from pypi
```

