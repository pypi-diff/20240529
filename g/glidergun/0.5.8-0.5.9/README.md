# Comparing `tmp/glidergun-0.5.8.tar.gz` & `tmp/glidergun-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glidergun-0.5.8.tar", last modified: Fri May 17 23:19:32 2024, max compression
+gzip compressed data, was "glidergun-0.5.9.tar", last modified: Wed May 29 09:40:44 2024, max compression
```

## Comparing `glidergun-0.5.8.tar` & `glidergun-0.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 23:19:32.025385 glidergun-0.5.8/
--rw-rw-rw-   0        0        0     2832 2024-05-17 23:19:32.023386 glidergun-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 23:19:31.997198 glidergun-0.5.8/glidergun/
--rw-rw-rw-   0        0        0      438 2024-05-17 15:49:39.000000 glidergun-0.5.8/glidergun/__init__.py
--rw-rw-rw-   0        0        0    50082 2024-05-17 15:49:45.000000 glidergun-0.5.8/glidergun/_grid.py
--rw-rw-rw-   0        0        0     4140 2024-05-17 15:49:49.000000 glidergun-0.5.8/glidergun/_ipython.py
--rw-rw-rw-   0        0        0     1783 2024-05-17 15:49:52.000000 glidergun-0.5.8/glidergun/_literals.py
--rw-rw-rw-   0        0        0    10489 2024-05-17 23:15:02.000000 glidergun-0.5.8/glidergun/_stack.py
-drwxrwxrwx   0        0        0        0 2024-05-17 23:19:32.022374 glidergun-0.5.8/glidergun.egg-info/
--rw-rw-rw-   0        0        0     2832 2024-05-17 23:19:31.000000 glidergun-0.5.8/glidergun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-17 23:19:31.000000 glidergun-0.5.8/glidergun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 23:19:31.000000 glidergun-0.5.8/glidergun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-17 23:19:31.000000 glidergun-0.5.8/glidergun.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 23:19:31.000000 glidergun-0.5.8/glidergun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      746 2024-05-17 23:12:50.000000 glidergun-0.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 23:19:32.025385 glidergun-0.5.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 09:40:44.196843 glidergun-0.5.9/
+-rw-rw-rw-   0        0        0     2832 2024-05-29 09:40:44.195102 glidergun-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 09:40:44.164989 glidergun-0.5.9/glidergun/
+-rw-rw-rw-   0        0        0      438 2024-05-17 15:49:39.000000 glidergun-0.5.9/glidergun/__init__.py
+-rw-rw-rw-   0        0        0    50287 2024-05-29 09:33:40.000000 glidergun-0.5.9/glidergun/_grid.py
+-rw-rw-rw-   0        0        0     4140 2024-05-24 11:06:10.000000 glidergun-0.5.9/glidergun/_ipython.py
+-rw-rw-rw-   0        0        0     1783 2024-05-17 15:49:52.000000 glidergun-0.5.9/glidergun/_literals.py
+-rw-rw-rw-   0        0        0    10489 2024-05-17 23:15:02.000000 glidergun-0.5.9/glidergun/_stack.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:40:44.193112 glidergun-0.5.9/glidergun.egg-info/
+-rw-rw-rw-   0        0        0     2832 2024-05-29 09:40:44.000000 glidergun-0.5.9/glidergun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-29 09:40:44.000000 glidergun-0.5.9/glidergun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:40:44.000000 glidergun-0.5.9/glidergun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-29 09:40:44.000000 glidergun-0.5.9/glidergun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 09:40:44.000000 glidergun-0.5.9/glidergun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      746 2024-05-29 08:33:55.000000 glidergun-0.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:40:44.196843 glidergun-0.5.9/setup.cfg
```

### Comparing `glidergun-0.5.8/PKG-INFO` & `glidergun-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glidergun
-Version: 0.5.8
+Version: 0.5.9
 Summary: Map Algebra with NumPy
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/glidergun
 Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `glidergun-0.5.8/README.md` & `glidergun-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.8/glidergun/_grid.py` & `glidergun-0.5.9/glidergun/_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1248,15 +1248,15 @@
 def _create(data: ndarray, crs: CRS, transform: Affine):
     if data.dtype == "float64":
         data = np.asanyarray(data, dtype="float32")
     elif data.dtype == "int64":
         data = np.asanyarray(data, dtype="int32")
     elif data.dtype == "uint64":
         data = np.asanyarray(data, dtype="uint32")
-    return Grid(data, crs, transform)
+    return Grid(data, crs if crs else CRS.from_epsg(3857), transform)
 
 
 def _read(dataset, index):
     grid = _create(dataset.read(index), dataset.crs, dataset.transform)
     return grid if dataset.nodata is None else grid.set_nan(dataset.nodata)
 
 
@@ -1507,14 +1507,19 @@
         coord_array.append(p[:2])
         value_array.append(p[-1])
 
     coords = np.array(coord_array)
     values = np.array(value_array)
     x, y = coords.transpose(1, 0)
     xmin, ymin, xmax, ymax = x.min(), y.min(), x.max(), y.max()
+
+    x_buffer = (xmax - xmin) * 0.1
+    y_buffer = (ymax - ymin) * 0.1
+    xmin, ymin, xmax, ymax = xmin - x_buffer, ymin - y_buffer, xmax + x_buffer, ymax + y_buffer
+
     extent = Extent(xmin, ymin, xmax, ymax)
     grid = create(extent, epsg, cell_size)
     interp = interpolator_factory(coords, values)
     xs = np.linspace(xmin, xmax, grid.width)
     ys = np.linspace(ymax, ymin, grid.height)
     array = np.array([[x0, y0] for x0 in xs for y0 in ys])
     data = interp(array).reshape((grid.width, grid.height)).transpose(1, 0)
```

### Comparing `glidergun-0.5.8/glidergun/_ipython.py` & `glidergun-0.5.9/glidergun/_ipython.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.8/glidergun/_literals.py` & `glidergun-0.5.9/glidergun/_literals.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.8/glidergun/_stack.py` & `glidergun-0.5.9/glidergun/_stack.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.8/glidergun.egg-info/PKG-INFO` & `glidergun-0.5.9/glidergun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glidergun
-Version: 0.5.8
+Version: 0.5.9
 Summary: Map Algebra with NumPy
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/glidergun
 Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `glidergun-0.5.8/pyproject.toml` & `glidergun-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glidergun"
-version = "0.5.8"
+version = "0.5.9"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "Map Algebra with NumPy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

