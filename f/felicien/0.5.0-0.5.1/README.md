# Comparing `tmp/felicien-0.5.0.tar.gz` & `tmp/felicien-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felicien-0.5.0.tar", max compression
+gzip compressed data, was "felicien-0.5.1.tar", max compression
```

## Comparing `felicien-0.5.0.tar` & `felicien-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-05-26 15:49:47.210403 felicien-0.5.0/LICENSE
--rw-r--r--   0        0        0     2599 2024-05-26 15:49:47.210403 felicien-0.5.0/README.md
--rw-r--r--   0        0        0      142 2024-05-26 15:49:47.216403 felicien-0.5.0/felicien/__init__.py
--rw-r--r--   0        0        0     6505 2024-05-26 15:49:47.216403 felicien-0.5.0/felicien/feliconnector.py
--rw-r--r--   0        0        0    12839 2024-05-26 15:49:47.216403 felicien-0.5.0/felicien/felits.py
--rw-r--r--   0        0        0     1067 2024-05-26 15:49:47.217403 felicien-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 felicien-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-28 13:20:00.022959 felicien-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2599 2024-05-28 13:20:00.023959 felicien-0.5.1/README.md
+-rw-r--r--   0        0        0      142 2024-05-28 13:20:00.028959 felicien-0.5.1/felicien/__init__.py
+-rw-r--r--   0        0        0     6505 2024-05-28 13:20:00.029959 felicien-0.5.1/felicien/feliconnector.py
+-rw-r--r--   0        0        0    13044 2024-05-28 13:20:00.029959 felicien-0.5.1/felicien/felits.py
+-rw-r--r--   0        0        0     1067 2024-05-28 13:20:00.030959 felicien-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 felicien-0.5.1/PKG-INFO
```

### Comparing `felicien-0.5.0/LICENSE` & `felicien-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `felicien-0.5.0/README.md` & `felicien-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `felicien-0.5.0/felicien/feliconnector.py` & `felicien-0.5.1/felicien/feliconnector.py`

 * *Files identical despite different names*

### Comparing `felicien-0.5.0/felicien/felits.py` & `felicien-0.5.1/felicien/felits.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,35 +350,41 @@
 
         Returns:
             pd.Series: the extract of the timeserie
 
         Raises:
             ValueError if the position argument is not "first" or "last"
         """
+        # case of series with maximum 2 points
+        if self.size <= 2:
+            return self.data
+
         # create an array stating if two points are separated by
         # exactly 1 frequency
         segments = self.data.index.diff() == self.frequency  # type: ignore
 
-        # estimate the size of the longest segment
+        # estimate the size of the longest segment matching the frequency
         longest_length = max(
-            len(list(y)) for (_, y) in itertools.groupby(segments)
+            len(list(y)) if is_freq else 0
+            for (is_freq, y) in itertools.groupby(segments)
         )
 
         # finding the position of the longest segment (first or last)
         start_position = 0
         cursor = 0
         for is_freq, segment in itertools.groupby(segments):
+            local_segment = list(segment)
             # case where the frequency matches and the length of
             # the segment is the longest
-            if is_freq and len(list(segment)) == longest_length:
+            if is_freq and len(local_segment) == longest_length:
                 start_position = cursor
 
                 # in case we found the first longest segment
                 if position == "first":
                     break
 
             # move current cursor along the serie
-            cursor += len(list(segment))
+            cursor += len(local_segment)
 
         return self.data.iloc[
             start_position - 1 : start_position + longest_length  # noqa E203
         ]
```

### Comparing `felicien-0.5.0/pyproject.toml` & `felicien-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "felicien"
-version = "0.5.0"
+version = "0.5.1"
 description = "Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB."
 authors = ["Julien Andrieux <chilladx@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "felicien" },
 ]
```

### Comparing `felicien-0.5.0/PKG-INFO` & `felicien-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felicien
-Version: 0.5.0
+Version: 0.5.1
 Summary: Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB.
 License: MIT
 Author: Julien Andrieux
 Author-email: chilladx@pm.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

