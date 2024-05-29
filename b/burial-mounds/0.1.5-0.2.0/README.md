# Comparing `tmp/burial_mounds-0.1.5.tar.gz` & `tmp/burial_mounds-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burial_mounds-0.1.5.tar", max compression
+gzip compressed data, was "burial_mounds-0.2.0.tar", max compression
```

## Comparing `burial_mounds-0.1.5.tar` & `burial_mounds-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1071 2024-04-22 07:49:21.859560 burial_mounds-0.1.5/LICENSE
--rw-r--r--   0        0        0     6779 2024-05-20 12:05:23.784727 burial_mounds-0.1.5/README.md
--rw-r--r--   0        0        0       53 2024-05-07 09:39:10.646657 burial_mounds-0.1.5/burial_mounds/__init__.py
--rw-r--r--   0        0        0      124 2024-05-07 10:06:17.874263 burial_mounds-0.1.5/burial_mounds/__main__.py
--rw-r--r--   0        0        0       45 2024-05-07 09:18:28.665769 burial_mounds-0.1.5/burial_mounds/cli.py
--rw-r--r--   0        0        0     1752 2024-05-20 12:26:24.164470 burial_mounds-0.1.5/burial_mounds/finetune.py
--rw-r--r--   0        0        0     2157 2024-05-07 10:05:45.822170 burial_mounds-0.1.5/burial_mounds/hub.py
--rw-r--r--   0        0        0     7019 2024-05-20 09:21:03.038104 burial_mounds-0.1.5/burial_mounds/preprocess_mounds.py
--rw-r--r--   0        0        0     5890 2024-05-19 13:46:15.939729 burial_mounds-0.1.5/burial_mounds/preprocess_xview.py
--rw-r--r--   0        0        0     2566 2024-05-20 08:46:21.207877 burial_mounds-0.1.5/burial_mounds/utils.py
--rw-r--r--   0        0        0      514 2024-05-20 12:28:51.584900 burial_mounds-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7707 1970-01-01 00:00:00.000000 burial_mounds-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-22 07:49:21.859560 burial_mounds-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6779 2024-05-20 12:05:23.784727 burial_mounds-0.2.0/README.md
+-rw-r--r--   0        0        0       53 2024-05-07 09:39:10.646657 burial_mounds-0.2.0/burial_mounds/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-07 10:06:17.874263 burial_mounds-0.2.0/burial_mounds/__main__.py
+-rw-r--r--   0        0        0       45 2024-05-07 09:18:28.665769 burial_mounds-0.2.0/burial_mounds/cli.py
+-rw-r--r--   0        0        0     1752 2024-05-20 12:26:24.164470 burial_mounds-0.2.0/burial_mounds/finetune.py
+-rw-r--r--   0        0        0     2590 2024-05-29 08:18:26.821749 burial_mounds-0.2.0/burial_mounds/hub.py
+-rw-r--r--   0        0        0     2477 2024-05-29 08:23:47.854688 burial_mounds-0.2.0/burial_mounds/model.py
+-rw-r--r--   0        0        0     7779 2024-05-28 12:16:11.519182 burial_mounds-0.2.0/burial_mounds/preprocess_mounds.py
+-rw-r--r--   0        0        0     5890 2024-05-19 13:46:15.939729 burial_mounds-0.2.0/burial_mounds/preprocess_xview.py
+-rw-r--r--   0        0        0     2566 2024-05-20 08:46:21.207877 burial_mounds-0.2.0/burial_mounds/utils.py
+-rw-r--r--   0        0        0      514 2024-05-29 08:25:52.158737 burial_mounds-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7707 1970-01-01 00:00:00.000000 burial_mounds-0.2.0/PKG-INFO
```

### Comparing `burial_mounds-0.1.5/LICENSE` & `burial_mounds-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.5/README.md` & `burial_mounds-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.5/burial_mounds/finetune.py` & `burial_mounds-0.2.0/burial_mounds/finetune.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.5/burial_mounds/preprocess_mounds.py` & `burial_mounds-0.2.0/burial_mounds/preprocess_mounds.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,76 +56,97 @@
 
 def get_labels_in_window(
     polygons: Iterable[shapely.Polygon],
     window: Window,
     dataset,
     image_size: int,
     format: Literal["detect", "obb"] = "obb",
+    min_mound_size: int = 32,
 ) -> Iterable[list[str]]:
     """Yields YOLO label entries in a window in a dataset
     for each bounding polygons."""
     window_bounds = shapely.box(*dataset.window_bounds(window))
     # YOLO entries for window
     for polygon in polygons:
         if not polygon.intersects(window_bounds):
             continue
         polygon = polygon.intersection(window_bounds)
         try:
-            bbox = get_bounding_box(polygon=polygon, window=window, dataset=dataset)
-            bbox = convert_bbox(
-                bbox,
-                width=image_size,
-                height=image_size,
-                format=format,
+            x_min, y_min, x_max, y_max = get_bounding_box(
+                polygon=polygon, window=window, dataset=dataset
             )
-            yield ["0"] + [f"{coord:.6f}" for coord in bbox]
+            if ((x_max - x_min) > min_mound_size) and (
+                (y_max - y_min) > min_mound_size
+            ):
+                bbox = convert_bbox(
+                    [x_min, y_min, x_max, y_max],
+                    width=image_size,
+                    height=image_size,
+                    format=format,
+                )
+                yield ["0"] + [f"{coord:.6f}" for coord in bbox]
         except WindowError as e:
             print(f"WARNING: Couldn't add feature on window, {e}")
 
 
 @cli.command(
     "preprocess_mounds",
     data_dir=Arg("--data_dir", "-d", help="Data where mounds data is located."),
     out_dir=Arg(
         "--out_dir", "-o", help="Data where mounds YOLO dataset should be saved."
     ),
     image_size=Arg(
         "--image_size", "-s", help="Size of the square shaped images to produce."
     ),
     format=Arg("--format", "-f", help="Format of the dataset {'detect' or 'obb'}"),
+    min_mound_size=Arg(
+        "--min_mound_size",
+        "-m",
+        help="Minimal width and length of a mound to be labelled.",
+    ),
+    joint=Arg(
+        "--joint",
+        "-j",
+        help="Indicates whether the joint image should be used, or the separate images.",
+    ),
 )
 def preprocess_mounds(
     data_dir: str = "data/TRAP_Data",
     out_dir: str = "data/mounds",
     image_size: int = 1024,
     format: Literal["obb", "detect"] = "obb",
+    min_mound_size: int = 10,
+    joint: bool = False,
 ):
     """Preprocesses the mounds dataset.
     Creates square images with annotations, corrects satellite color
     channels and produces train and test splits."""
     print(
         f"""
     Preprocessing burial mounds dataset with following parameters:
       - directory: {data_dir}
       - window size: {image_size} x {image_size}
       - format: {format}
+      - minimum mound size: {min_mound_size}
+      - joint: {joint}
     """
     )
     data_path = Path(data_dir)
     print("Loading bounding boxes")
     boxes = gpd.read_file(data_path.joinpath("Kaz_mndbbox.geojson"))
     boxes = boxes.set_crs(epsg=32635, allow_override=True)
     out_path = Path(out_dir)
     out_path.mkdir(exist_ok=True, parents=True)
 
-    files = {
-        "east": data_path.joinpath("East/kaz_e_fuse.img"),
-        "west": data_path.joinpath("West/kaz_w_fuse.img"),
-        # "joint": data_path.joinpath("kaz_fuse.img"),
-    }
+    files = dict()
+    if joint:
+        files["joint"] = data_path.joinpath("kaz_fuse.img")
+    else:
+        files["east"] = data_path.joinpath("East/kaz_e_fuse.img")
+        files["west"] = data_path.joinpath("West/kaz_w_fuse.img")
     images_path = out_path.joinpath("images")
     images_path.mkdir(exist_ok=True)
     labels_path = out_path.joinpath("labels")
     labels_path.mkdir(exist_ok=True)
     annotated_path = out_path.joinpath("annotated")
     annotated_path.mkdir(exist_ok=True)
     print("Deleting previous images.")
@@ -145,14 +166,15 @@
                 window_entries: list[list[str]] = list(
                     get_labels_in_window(
                         boxes.geometry,
                         window=window,
                         dataset=dataset,
                         image_size=image_size,
                         format=format,
+                        min_mound_size=min_mound_size,
                     )
                 )
                 # Go to next window if there are no mounds in it
                 if not window_entries:
                     continue
                 image = np.stack([dataset.read(ch, window=window) for ch in (1, 2, 3)])
                 # Only appending image if it is large enough
```

### Comparing `burial_mounds-0.1.5/burial_mounds/preprocess_xview.py` & `burial_mounds-0.2.0/burial_mounds/preprocess_xview.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.5/burial_mounds/utils.py` & `burial_mounds-0.2.0/burial_mounds/utils.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.5/pyproject.toml` & `burial_mounds-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burial-mounds"
-version = "0.1.5"
+version = "0.2.0"
 description = "Recognizing burial mounds with YOLO"
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `burial_mounds-0.1.5/PKG-INFO` & `burial_mounds-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burial-mounds
-Version: 0.1.5
+Version: 0.2.0
 Summary: Recognizing burial mounds with YOLO
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

