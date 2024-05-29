# Comparing `tmp/GridCalServer-5.1.10.tar.gz` & `tmp/GridCalServer-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCalServer-5.1.10.tar", last modified: Wed May 29 21:19:44 2024, max compression
+gzip compressed data, was "GridCalServer-5.1.9.tar", last modified: Wed May 29 20:40:00 2024, max compression
```

## Comparing `GridCalServer-5.1.10.tar` & `GridCalServer-5.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-rw-rw-   0        0        0     1587 2024-05-29 20:39:28.886291 GridCalServer-5.1.10/GridCalServer/connection_example.py
--rw-rw-rw-   0        0        0     4893 2024-05-29 20:39:28.887791 GridCalServer-5.1.10/GridCalServer/endpoints.py
--rw-rw-rw-   0        0        0    11941 2024-05-29 20:39:28.885291 GridCalServer-5.1.10/GridCalServer/LICENSE.txt
--rw-rw-rw-   0        0        0     1237 2024-05-29 20:39:28.887791 GridCalServer-5.1.10/GridCalServer/run.py
--rw-rw-rw-   0        0        0        0 2024-05-29 20:39:28.885792 GridCalServer-5.1.10/GridCalServer/__init__.py
--rw-rw-rw-   0        0        0     2891 2024-05-29 20:43:21.872285 GridCalServer-5.1.10/GridCalServer/__version__.py
--rw-rw-rw-   0        0        0    67646 2024-05-29 20:39:28.886791 GridCalServer-5.1.10/GridCalServer/data/GridCal_icon.ico
--rw-rw-rw-   0        0        0        0 2024-05-29 20:39:28.887291 GridCalServer-5.1.10/GridCalServer/data/__init__.py
--rw-rw-rw-   0        0        0     3991 2024-05-29 20:39:28.888292 GridCalServer-5.1.10/setup.py
--rw-rw-rw-   0        0        0     1072 2024-05-29 21:19:44.700336 GridCalServer-5.1.10/PKG-INFO
--rw-rw-rw-   0        0        0       40 2024-05-29 21:19:44.700336 GridCalServer-5.1.10/setup.cfg
+-rw-rw-rw-   0        0        0     1587 2024-05-29 20:39:28.886291 GridCalServer-5.1.9/GridCalServer/connection_example.py
+-rw-rw-rw-   0        0        0     4893 2024-05-29 20:39:28.887791 GridCalServer-5.1.9/GridCalServer/endpoints.py
+-rw-rw-rw-   0        0        0    11941 2024-05-29 20:39:28.885291 GridCalServer-5.1.9/GridCalServer/LICENSE.txt
+-rw-rw-rw-   0        0        0     1237 2024-05-29 20:39:28.887791 GridCalServer-5.1.9/GridCalServer/run.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:39:28.885792 GridCalServer-5.1.9/GridCalServer/__init__.py
+-rw-rw-rw-   0        0        0     2890 2024-05-29 20:39:28.885792 GridCalServer-5.1.9/GridCalServer/__version__.py
+-rw-rw-rw-   0        0        0    67646 2024-05-29 20:39:28.886791 GridCalServer-5.1.9/GridCalServer/data/GridCal_icon.ico
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:39:28.887291 GridCalServer-5.1.9/GridCalServer/data/__init__.py
+-rw-rw-rw-   0        0        0     3991 2024-05-29 20:39:28.888292 GridCalServer-5.1.9/setup.py
+-rw-rw-rw-   0        0        0     1071 2024-05-29 20:40:00.882621 GridCalServer-5.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2024-05-29 20:40:00.882621 GridCalServer-5.1.9/setup.cfg
```

### Comparing `GridCalServer-5.1.10/GridCalServer/connection_example.py` & `GridCalServer-5.1.9/GridCalServer/connection_example.py`

 * *Files identical despite different names*

### Comparing `GridCalServer-5.1.10/GridCalServer/endpoints.py` & `GridCalServer-5.1.9/GridCalServer/endpoints.py`

 * *Files identical despite different names*

### Comparing `GridCalServer-5.1.10/GridCalServer/LICENSE.txt` & `GridCalServer-5.1.9/GridCalServer/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCalServer-5.1.10/GridCalServer/run.py` & `GridCalServer-5.1.9/GridCalServer/run.py`

 * *Files identical despite different names*

### Comparing `GridCalServer-5.1.10/GridCalServer/__version__.py` & `GridCalServer-5.1.9/GridCalServer/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCalServer_VERSION__ = "5.1.10"
+__GridCalServer_VERSION__ = "5.1.9"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCalServer v" + str(__GridCalServer_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCalServer-5.1.10/GridCalServer/data/GridCal_icon.ico` & `GridCalServer-5.1.9/GridCalServer/data/GridCal_icon.ico`

 * *Files identical despite different names*

### Comparing `GridCalServer-5.1.10/setup.py` & `GridCalServer-5.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `GridCalServer-5.1.10/PKG-INFO` & `GridCalServer-5.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCalServer
-Version: 5.1.10
+Version: 5.1.9
 Summary: GridCal is a Power Systems simulation program intended for professional use and research
 Home-page: https://github.com/SanPen/GridCal
 Author: Santiago Peñate Vera et. Al.
 Author-email: santiago@gridcal.org
 License: LGPL
 Keywords: power systems planning
 Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
```

