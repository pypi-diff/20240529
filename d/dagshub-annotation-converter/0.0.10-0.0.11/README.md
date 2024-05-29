# Comparing `tmp/dagshub_annotation_converter-0.0.10.tar.gz` & `tmp/dagshub_annotation_converter-0.0.11.tar.gz`

## Comparing `dagshub_annotation_converter-0.0.10.tar` & `dagshub_annotation_converter-0.0.11.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/ruff.toml
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/cli.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/importer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/exporters/__init__.py
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/exporters/dagshub_datasource.py
--rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/exporters/yolo.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/importers/__init__.py
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/importers/cvat.py
--rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/importers/dagshub_datasource.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/importers/yolo.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/util/__init__.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/util/path_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/ir/__init__.py
--rw-r--r--   0        0        0     9432 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/ir/annotation_ir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/abc.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/keypointlabels.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/polygonlabels.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/rectanglelabels.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/task.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/.gitignore
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/README.md
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/pyproject.toml
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/ruff.toml
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/cli.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/importer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/exporters/__init__.py
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/exporters/dagshub_datasource.py
+-rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/exporters/yolo.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/importers/__init__.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/importers/cvat.py
+-rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/importers/dagshub_datasource.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/importers/yolo.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/util/__init__.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/util/path_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/ir/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/ir/annotation_ir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/abc.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/keypointlabels.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/polygonlabels.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/rectanglelabels.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/task.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/.gitignore
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/README.md
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 dagshub_annotation_converter-0.0.11/PKG-INFO
```

### Comparing `dagshub_annotation_converter-0.0.10/.github/workflows/python-publish.yml` & `dagshub_annotation_converter-0.0.11/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/exporters/dagshub_datasource.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/exporters/dagshub_datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/exporters/yolo.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/exporters/yolo.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,53 +21,75 @@
 YoloAnnotationType = Literal["bbox", "segmentation", "pose"]
 
 logger = logging.getLogger(__name__)
 
 
 class YoloExporterStrategy:
     @abstractmethod
-    def get_yolo_yaml(self, project: AnnotationProject, data_dir: Path, image_dir_name: str) -> str:
+    def get_yolo_yaml(
+        self,
+        project: AnnotationProject,
+        data_dir: Path,
+        image_dir_name: str,
+        label_dir_name: str,
+        **kwargs,
+    ) -> str:
         """Gets the contents of the YOLO metadata yaml file"""
         ...
 
     @abstractmethod
-    def convert_file(self, project: AnnotationProject, f: AnnotatedFile) -> str:
+    def convert_file(self, project: AnnotationProject, f: AnnotatedFile, **kwargs) -> str:
         """Converts annotations for a single file into a yolo annotation and returns the content"""
         ...
 
-    def generate_generic_yaml_content(self, project: AnnotationProject, data_dir: Path, image_dir_name: str) -> dict:
-        train, val = self.determine_test_and_val_folders(data_dir, image_dir_name)
+    def generate_generic_yaml_content(
+        self,
+        project: AnnotationProject,
+        data_dir: Path,
+        image_dir_name: str,
+        label_dir_name: str,
+    ) -> dict:
+        train, val = self.determine_test_and_val_folders(data_dir, image_dir_name, label_dir_name)
         yaml_structure = {
             "path": str(data_dir.absolute()),
             "names": {cat.id: cat.name for cat in project.categories.categories},
             "nc": len(project.categories),
             "train": train,
             "val": val,
         }
         return yaml_structure
 
-    def determine_test_and_val_folders(self, data_dir: Path, image_dir_name: str) -> tuple[str, str]:
+    @staticmethod
+    def determine_test_and_val_folders(data_dir: Path, image_dir_name: str, label_dir_name: str) -> tuple[str, str]:
         """
         Tries to find test and val folder.
         Current logic:
-        1) Drill down in data_dir until an image directory is found
-        2) Then look at the subfolders of the image dir
+        1) Drill down in data_dir until a label directory is found
+        2) Then look at the subfolders of the label dir
             If there's 0/1/more than 2 dirs - make the data dir both the test and val dir
             If there are two dirs and one contains train/one contains val, the other gets assigned accordingly
 
         """
-        img_dir = None
+        label_dir = None
         for root, dirs, files in os.walk(data_dir):
-            if image_dir_name in dirs:
-                img_dir = Path(root) / image_dir_name
-        if img_dir is None:
-            raise RuntimeError(f'Could not find the image dir named "{image_dir_name}" in the data directory')
-        subdirs = [img_dir / p for p in os.listdir(img_dir)]
+            if label_dir_name in dirs:
+                label_dir = Path(root) / label_dir_name
+        if label_dir is None:
+            raise RuntimeError(f'Could not find the label dir named "{label_dir_name}" in the data directory')
+        subdirs = [label_dir / p for p in os.listdir(label_dir)]
         subdirs = [p for p in subdirs if p.is_dir()]
 
+        # Replace the label -> image
+        img_dir_parts = list(label_dir.parts)
+        for i, part in enumerate(reversed(label_dir.parts)):
+            if part == label_dir_name:
+                img_dir_parts[len(img_dir_parts) - i - 1] = image_dir_name
+                break
+
+        img_dir = Path(*img_dir_parts)
         img_dir_relative = img_dir.relative_to(data_dir)
 
         if len(subdirs) != 2:
             return str(img_dir_relative), str(img_dir_relative)
 
         p1 = subdirs[0]
         p2 = subdirs[1]
@@ -76,18 +98,20 @@
             return str(img_dir_relative / p1.name), str(img_dir_relative / p2.name)
         elif "val" in p1.name or "train" in p1.name:
             return str(img_dir_relative / p2.name), str(img_dir_relative / p1.name)
         return str(img_dir_relative), str(img_dir_relative)
 
 
 class BBoxExporterStrategy(YoloExporterStrategy):
-    def get_yolo_yaml(self, project: AnnotationProject, data_dir: Path, image_dir_name: str) -> str:
-        return yaml.dump(self.generate_generic_yaml_content(project, data_dir, image_dir_name))
+    def get_yolo_yaml(
+        self, project: AnnotationProject, data_dir: Path, image_dir_name: str, label_dir_name: str, **kwargs
+    ) -> str:
+        return yaml.dump(self.generate_generic_yaml_content(project, data_dir, image_dir_name, label_dir_name))
 
-    def convert_file(self, project: AnnotationProject, f: AnnotatedFile) -> str:
+    def convert_file(self, project: AnnotationProject, f: AnnotatedFile, **kwargs) -> str:
         wrong_annotation_counter = 0
         res = ""
         for ann in f.annotations:
             assert f.image_width is not None and f.image_height is not None
             ann = ann.normalized(f.image_width, f.image_height)
             if not isinstance(ann, BBoxAnnotation):
                 wrong_annotation_counter += 1
@@ -97,18 +121,25 @@
             res += f"{ann.category.id} {middle_x} {middle_y} {ann.width} {ann.height}\n"
         if wrong_annotation_counter != 0:
             logger.warning(f"Skipped {wrong_annotation_counter} non-bounding box annotation(s) for file {f.file}")
         return res
 
 
 class SegmentationExporterStrategy(YoloExporterStrategy):
-    def get_yolo_yaml(self, project: AnnotationProject, data_dir: Path, image_dir_name: str) -> str:
-        return yaml.dump(self.generate_generic_yaml_content(project, data_dir, image_dir_name))
+    def get_yolo_yaml(
+        self,
+        project: AnnotationProject,
+        data_dir: Path,
+        image_dir_name: str,
+        label_dir_name: str,
+        **kwargs,
+    ) -> str:
+        return yaml.dump(self.generate_generic_yaml_content(project, data_dir, image_dir_name, label_dir_name))
 
-    def convert_file(self, project: AnnotationProject, f: AnnotatedFile) -> str:
+    def convert_file(self, project: AnnotationProject, f: AnnotatedFile, **kwargs) -> str:
         wrong_annotation_counter = 0
         res = ""
         for ann in f.annotations:
             assert f.image_width is not None and f.image_height is not None
             ann = ann.normalized(f.image_width, f.image_height)
             if not isinstance(ann, SegmentationAnnotation):
                 wrong_annotation_counter += 1
@@ -118,25 +149,27 @@
             res += "\n"
         if wrong_annotation_counter != 0:
             logger.warning(f"Skipped {wrong_annotation_counter} non-segment annotation(s) for file {f.file}")
         return res
 
 
 class PoseExporterStrategy(YoloExporterStrategy):
-    def get_yolo_yaml(self, project: AnnotationProject, data_dir: Path, image_dir_name: str) -> str:
-        yaml_dict = self.generate_generic_yaml_content(project, data_dir, image_dir_name)
+    def get_yolo_yaml(
+        self, project: AnnotationProject, data_dir: Path, image_dir_name: str, label_dir_name: str, **kwargs
+    ) -> str:
+        yaml_dict = self.generate_generic_yaml_content(project, data_dir, image_dir_name, label_dir_name)
         if len(project.pose_config.pose_points) == 0:
             project.regenerate_pose_points()
 
         max_points = project.pose_config.bind_pose_points_to_max()
 
-        yaml_dict["kpt_shape"] = [max_points, 3]
+        yaml_dict["kpt_shape"] = [max_points, kwargs.get("keypoint_dim", 3)]
         return yaml.dump(yaml_dict)
 
-    def convert_file(self, project: AnnotationProject, f: AnnotatedFile):
+    def convert_file(self, project: AnnotationProject, f: AnnotatedFile, **kwargs):
         # For pose: validate that the amount of points is equal across all annotations, otherwise don't import
         # Need poses to be consistent
         wrong_annotation_counter = 0
         res = ""
         for ann in f.annotations:
             assert f.image_width is not None and f.image_height is not None
             ann = ann.normalized(f.image_width, f.image_height)
@@ -148,35 +181,58 @@
             res += f"{ann.category.id} {middle_x} {middle_y} {ann.width} {ann.height} "
             points = ann.points
             # Fill out the remaining until we hit the max
             category_n_points = project.pose_config.pose_points.get(ann.category, len(points))
             if len(points) < category_n_points:
                 delta = category_n_points - len(points)
                 points.extend([KeyPoint(x=0.0, y=0.0, is_visible=False)] * delta)
-            res += " ".join([f"{p.x} {p.y} {1 if p.is_visible or p.is_visible is None else 0}" for p in points])
+            points_output = ""
+            for p in points:
+                points_output += f" {p.x} {p.y} "
+                if kwargs.get("keypoint_dim", 3) == 3:
+                    points_output += "1 " if p.is_visible or p.is_visible is None else "0 "
+                points_output = points_output.strip()
+            res += points_output
+            res += "\n"
         if wrong_annotation_counter != 0:
             logger.warning(f"Skipped {wrong_annotation_counter} non-pose annotation(s) for file {f.file}")
         return res
 
 
 class YoloExporter:
     def __init__(
         self,
         data_dir: Union[str, PathLike],
         annotation_type: YoloAnnotationType,
         image_dir_name: str = "images",
         label_dir_name: str = "labels",
         label_extension: str = ".txt",
         meta_file: Union[str, PathLike] = "annotations.yaml",
+        overwrite_existing_meta_file: bool = True,
+        pose_keypoint_dim: Literal[2, 3] = 3,
     ):
+        """
+        Export annotations to YOLO format
+        :param data_dir: path to the directory where to store the labels
+        :param annotation_type: Type of annotations to export. Either bbox, segmentation, or pose
+        :param image_dir_name: Name of the image directory. Default is images
+        :param label_dir_name: Name of the label directory. Default is labels
+        :param label_extension: Extension to use on the label files. Default is .txt
+        :param meta_file: Path of the YOLO .yaml file that will be written
+        :param overwrite_existing_meta_file: If this is set to True, existing meta file wouldn't be overwritten.
+            Be cautious, this might cause category mismatches, if the data has changed!
+        :param pose_keypoint_dim: For pose annotations - dimensions of a keypoint. Either 2 or 3, 3 by default
+        """
         self.data_dir = Path(data_dir)
         self.image_dir_name = image_dir_name
         self.label_dir_name = label_dir_name
         self.meta_file = meta_file
         self.label_extension = label_extension
+        self.overwrite_existing_meta_file = overwrite_existing_meta_file
+        self.pose_keypoint_dim = pose_keypoint_dim
         if not self.label_extension.startswith("."):
             self.label_extension = "." + self.label_extension
 
         self.strategy = self.determine_export_strategy(annotation_type)
 
     @staticmethod
     def determine_export_strategy(annotation_type: YoloAnnotationType) -> YoloExporterStrategy:
@@ -191,26 +247,39 @@
             raise ValueError(
                 f"Unknown yolo annotation type: {annotation_type}. Allowed types are: {YoloAnnotationType}"
             )
 
     def export(self, project: AnnotationProject):
         # Write the annotations
         for annotated in project.files:
-            converted = self.strategy.convert_file(project, annotated)
+            converted = self.strategy.convert_file(project, annotated, keypoint_dim=self.pose_keypoint_dim)
             if not converted:
                 logger.warning(f"No annotations of fitting type found for file {annotated.file}")
                 continue
             annotation_file_path = yolo_img_path_to_label_path(
                 Path(annotated.file), self.image_dir_name, self.label_dir_name, self.label_extension
             )
             annotation_file_path = self.data_dir / annotation_file_path
             annotation_file_path.parent.mkdir(parents=True, exist_ok=True)
             annotation_file_path.write_text(converted)
 
         # Write the metadata file
-        Path(self.meta_file).parent.mkdir(parents=True, exist_ok=True)
-        with open(self.meta_file, "w") as f:
-            dt_now = datetime.datetime.now()
-            f.write(
-                f"# This YOLO dataset was autogenerated by DagsHub annotation converter on {dt_now.isoformat()}\n\n"
-            )
-            f.write(self.strategy.get_yolo_yaml(project, self.data_dir, self.image_dir_name))
+        meta_file_path = Path(self.meta_file)
+        meta_file_path.parent.mkdir(parents=True, exist_ok=True)
+        if meta_file_path.exists() and not self.overwrite_existing_meta_file:
+            logger.warning(f"Not overwriting existing YOLO config {self.meta_file}")
+        else:
+            with open(self.meta_file, "w") as f:
+                dt_now = datetime.datetime.now()
+                f.write(
+                    f"# This YOLO dataset was autogenerated by DagsHub annotation converter on {dt_now.isoformat()}\n\n"
+                )
+                f.write(
+                    self.strategy.get_yolo_yaml(
+                        project,
+                        self.data_dir,
+                        self.image_dir_name,
+                        self.label_dir_name,
+                        keypoint_dim=self.pose_keypoint_dim,
+                    )
+                )
+                logger.warning(f"Written out the YOLO config to {self.meta_file}")
```

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/importers/cvat.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/importers/cvat.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/importers/dagshub_datasource.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/importers/dagshub_datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/importers/yolo.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/importers/yolo.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/image/util/__init__.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/image/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/ir/annotation_ir.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/ir/annotation_ir.py`

 * *Files 3% similar despite different names*

```diff
@@ -276,14 +276,20 @@
         return max_val
 
 
 class YoloImportConfig(BaseModel):
     keypoint_shape: Literal[2, 3] = 2
 
 
+class YoloExportConfig(BaseModel):
+    keypoint_dim: Literal[2, 3] = 3  # Export with 3 dimensions by default
+    rewrite_yaml: bool = True
+    """Whether to rewrite the YAML file or not if it already exists"""
+
+
 class ImportConfig(BaseModel):
     yolo: YoloImportConfig = YoloImportConfig()
 
 
 class AnnotationProject(BaseModel):
     categories: Categories = Categories()
     files: List[AnnotatedFile] = []
```

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/abc.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/abc.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/keypointlabels.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/keypointlabels.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/polygonlabels.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/polygonlabels.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/rectanglelabels.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/rectanglelabels.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/dagshub_annotation_converter/schema/label_studio/task.py` & `dagshub_annotation_converter-0.0.11/dagshub_annotation_converter/schema/label_studio/task.py`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/README.md` & `dagshub_annotation_converter-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/pyproject.toml` & `dagshub_annotation_converter-0.0.11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagshub_annotation_converter-0.0.10/PKG-INFO` & `dagshub_annotation_converter-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dagshub-annotation-converter
-Version: 0.0.10
+Version: 0.0.11
 Summary: Annotation converter between different formats
 Project-URL: Documentation, https://github.com/dagshub/dagshub-annotation-converter#readme
 Project-URL: Issues, https://github.com/dagshub/dagshub-annotation-converter/issues
 Project-URL: Source, https://github.com/dagshub/dagshub-annotation-converter
 Author-email: Kirill Bolashev <kirill@dagshub.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

