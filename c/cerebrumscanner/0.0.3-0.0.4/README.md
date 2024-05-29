# Comparing `tmp/cerebrumscanner-0.0.3.tar.gz` & `tmp/cerebrumscanner-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner-0.0.3.tar", last modified: Wed May 29 14:31:38 2024, max compression
+gzip compressed data, was "cerebrumscanner-0.0.4.tar", last modified: Wed May 29 15:20:38 2024, max compression
```

## Comparing `cerebrumscanner-0.0.3.tar` & `cerebrumscanner-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 14:31:38.127573 cerebrumscanner-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-09-10 19:28:05.000000 cerebrumscanner-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       24 2024-05-27 12:55:40.000000 cerebrumscanner-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    45364 2024-05-29 14:31:38.125373 cerebrumscanner-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3382 2024-02-21 06:32:05.000000 cerebrumscanner-0.0.3/README.md
--rw-rw-rw-   0        0        0      230 2024-05-28 10:23:21.000000 cerebrumscanner-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 14:31:38.127573 cerebrumscanner-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-29 14:29:38.000000 cerebrumscanner-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 14:31:38.077151 cerebrumscanner-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 14:31:38.088184 cerebrumscanner-0.0.3/src/cerebrumscanner/
--rw-rw-rw-   0        0        0       84 2024-05-28 12:15:56.000000 cerebrumscanner-0.0.3/src/cerebrumscanner/__init__.py
--rw-rw-rw-   0        0        0     5874 2024-05-29 14:31:26.000000 cerebrumscanner-0.0.3/src/cerebrumscanner/database_manager.py
--rw-rw-rw-   0        0        0     1379 2024-05-28 12:11:53.000000 cerebrumscanner-0.0.3/src/cerebrumscanner/image_processor.py
-drwxrwxrwx   0        0        0        0 2024-05-29 14:31:38.122374 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/
--rw-rw-rw-   0        0        0    45364 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2024-05-29 14:31:38.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      192 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 15:20:38.362559 cerebrumscanner-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-09-10 19:28:05.000000 cerebrumscanner-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       24 2024-05-27 12:55:40.000000 cerebrumscanner-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    45584 2024-05-29 15:20:38.360574 cerebrumscanner-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3382 2024-02-21 06:32:05.000000 cerebrumscanner-0.0.4/README.md
+-rw-rw-rw-   0        0        0      450 2024-05-29 15:18:43.000000 cerebrumscanner-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 15:20:38.362559 cerebrumscanner-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-29 15:18:59.000000 cerebrumscanner-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:20:38.320501 cerebrumscanner-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 15:20:38.333014 cerebrumscanner-0.0.4/src/cerebrumscanner/
+-rw-rw-rw-   0        0        0       84 2024-05-28 12:15:56.000000 cerebrumscanner-0.0.4/src/cerebrumscanner/__init__.py
+-rw-rw-rw-   0        0        0     5874 2024-05-29 14:31:26.000000 cerebrumscanner-0.0.4/src/cerebrumscanner/database_manager.py
+-rw-rw-rw-   0        0        0     1379 2024-05-28 12:11:53.000000 cerebrumscanner-0.0.4/src/cerebrumscanner/image_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:20:38.358045 cerebrumscanner-0.0.4/src/cerebrumscanner.egg-info/
+-rw-rw-rw-   0        0        0    45584 2024-05-29 15:20:38.000000 cerebrumscanner-0.0.4/src/cerebrumscanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-05-29 15:20:38.000000 cerebrumscanner-0.0.4/src/cerebrumscanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 15:20:38.000000 cerebrumscanner-0.0.4/src/cerebrumscanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 15:20:38.000000 cerebrumscanner-0.0.4/src/cerebrumscanner.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      250 2024-05-29 15:20:38.000000 cerebrumscanner-0.0.4/src/cerebrumscanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-29 15:20:38.000000 cerebrumscanner-0.0.4/src/cerebrumscanner.egg-info/top_level.txt
```

### Comparing `cerebrumscanner-0.0.3/LICENSE` & `cerebrumscanner-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.3/PKG-INFO` & `cerebrumscanner-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -679,18 +679,18 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kivy
-Requires-Dist: kivy-deps.angle
-Requires-Dist: kivy-deps.gstreamer
-Requires-Dist: kivy-deps.glew
-Requires-Dist: kivy-deps.sdl2
+Requires-Dist: kivy-deps.angle; python_version >= "3.6" and sys_platform == "windows"
+Requires-Dist: kivy-deps.gstreamer; python_version >= "3.6" and sys_platform == "windows"
+Requires-Dist: kivy-deps.glew; python_version >= "3.6" and sys_platform == "windows"
+Requires-Dist: kivy-deps.sdl2; python_version >= "3.6" and sys_platform == "windows"
 Requires-Dist: kivymd==1.2.0
 Requires-Dist: tqdm
 Requires-Dist: bcrypt
 Requires-Dist: pydicom
 Requires-Dist: dcm2niix
 Requires-Dist: dicom2nifti
 Requires-Dist: SimpleITK
```

### Comparing `cerebrumscanner-0.0.3/README.md` & `cerebrumscanner-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.3/setup.py` & `cerebrumscanner-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ) as readme_file, open("requirements.txt", encoding="utf-8") as requirements_file:
     package_license = license_file.read()
     long_description = readme_file.read()
     install_requires = requirements_file.read().split("\n")[0:]
 
 setup(
     name="cerebrumscanner",
-    version="0.0.3",
+    version="0.0.4",
     url="https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner",
     license=package_license,
     author="Nekodu Technology",
     author_email="info@nekodu.com",
     description=(
         "Cerebrum Scanner Project"
     ),
```

### Comparing `cerebrumscanner-0.0.3/src/cerebrumscanner/database_manager.py` & `cerebrumscanner-0.0.4/src/cerebrumscanner/database_manager.py`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.3/src/cerebrumscanner/image_processor.py` & `cerebrumscanner-0.0.4/src/cerebrumscanner/image_processor.py`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/PKG-INFO` & `cerebrumscanner-0.0.4/src/cerebrumscanner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -679,18 +679,18 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kivy
-Requires-Dist: kivy-deps.angle
-Requires-Dist: kivy-deps.gstreamer
-Requires-Dist: kivy-deps.glew
-Requires-Dist: kivy-deps.sdl2
+Requires-Dist: kivy-deps.angle; python_version >= "3.6" and sys_platform == "windows"
+Requires-Dist: kivy-deps.gstreamer; python_version >= "3.6" and sys_platform == "windows"
+Requires-Dist: kivy-deps.glew; python_version >= "3.6" and sys_platform == "windows"
+Requires-Dist: kivy-deps.sdl2; python_version >= "3.6" and sys_platform == "windows"
 Requires-Dist: kivymd==1.2.0
 Requires-Dist: tqdm
 Requires-Dist: bcrypt
 Requires-Dist: pydicom
 Requires-Dist: dcm2niix
 Requires-Dist: dicom2nifti
 Requires-Dist: SimpleITK
```

