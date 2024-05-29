# Comparing `tmp/clarifai-datautils-0.0.2.tar.gz` & `tmp/clarifai-datautils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-datautils-0.0.2.tar", last modified: Tue Mar 19 15:50:22 2024, max compression
+gzip compressed data, was "clarifai-datautils-0.0.3.tar", last modified: Wed May 29 13:50:35 2024, max compression
```

## Comparing `clarifai-datautils-0.0.2.tar` & `clarifai-datautils-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:22.106311 clarifai-datautils-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-19 15:50:22.106311 clarifai-datautils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:22.102311 clarifai-datautils-0.0.2/clarifai_datautils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:22.102311 clarifai-datautils-0.0.2/clarifai_datautils/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/constants/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:22.102311 clarifai-datautils-0.0.2/clarifai_datautils/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:22.106311 clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:50:22.102311 clarifai-datautils-0.0.2/clarifai_datautils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-19 15:50:22.000000 clarifai-datautils-0.0.2/clarifai_datautils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-19 15:50:22.000000 clarifai-datautils-0.0.2/clarifai_datautils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:50:22.000000 clarifai-datautils-0.0.2/clarifai_datautils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-19 15:50:22.000000 clarifai-datautils-0.0.2/clarifai_datautils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-19 15:50:22.000000 clarifai-datautils-0.0.2/clarifai_datautils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 15:50:22.106311 clarifai-datautils-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-19 15:50:11.000000 clarifai-datautils-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.223583 clarifai-datautils-0.0.3/clarifai_datautils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/clarifai_datautils/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/base/features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/clarifai_datautils/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/constants/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/constants/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/constants/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/clarifai_datautils/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/clarifai_datautils/image/annotation_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/image/annotation_conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/image/annotation_conversion/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/image/annotation_conversion/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/image/annotation_conversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/clarifai_datautils/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/clarifai_datautils/text/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/text/pipeline/PDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/text/pipeline/Text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/text/pipeline/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/text/pipeline/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/text/pipeline/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/clarifai_datautils/text/pipeline/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:35.223583 clarifai-datautils-0.0.3/clarifai_datautils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-29 13:50:35.000000 clarifai-datautils-0.0.3/clarifai_datautils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-29 13:50:35.000000 clarifai-datautils-0.0.3/clarifai_datautils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:50:35.000000 clarifai-datautils-0.0.3/clarifai_datautils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 13:50:35.000000 clarifai-datautils-0.0.3/clarifai_datautils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 13:50:35.000000 clarifai-datautils-0.0.3/clarifai_datautils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:50:35.227583 clarifai-datautils-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 13:50:27.000000 clarifai-datautils-0.0.3/setup.py
```

### Comparing `clarifai-datautils-0.0.2/LICENSE` & `clarifai-datautils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-datautils-0.0.2/PKG-INFO` & `clarifai-datautils-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: clarifai-datautils
-Version: 0.0.2
-Summary: Clarifai Data Utils
-Home-page: https://github.com/Clarifai/clarifai-python-datautils
-Author: Clarifai
-Author-email: support@clarifai.com
-License: Apache 2.0
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Clarifai logo](docs/logo.png)
 
 # Clarifai Python Data Utils
 
 
 [![Discord](https://img.shields.io/discord/1145701543228735582)](https://discord.gg/M32V7a7a)
 [![codecov](https://img.shields.io/pypi/dm/clarifai)](https://pypi.org/project/clarifai-datautils)
@@ -34,14 +13,15 @@
 ---
 ## Table Of Contents
 
 * **[Installation](#installation)**
 * **[Getting Started](#getting-started)**
 * **[Features](#features)**
   * [Image Utils](#image-utils)
+  * [Data Ingestion Pipeline](#ingestion-pipeline)
 * **[Usage](#usage)**
 * **[Examples](#more-examples)**
 
 
 ## Installation
 
 
@@ -75,15 +55,17 @@
 ## Features
 
 ### Image Utils
 - #### Annotation Loader
   - Load various annotated image datasets and export to clarifai Platform
   - Convert from one annotation format to other supported annotation formats
 
-
+### Data Ingestion Pipeline
+  - Easy to use pipelines to load data from files and ingest into clarifai platfrom.
+  - Load text files(pdf, doc, etc..) , transform, chunk and upload to the Clarifai Platform
 
 ## Usage
 ### Image Annotation Loader
 ```python
 from clarifai_datautils import ImageAnnotations
 #import from folder
 coco_dataset = ImageAnnotations.import_from(path='folder_path',format= 'coco_detection')
@@ -98,10 +80,34 @@
 coco_dataset.get_info()
 
 
 #exporting to other formats
 coco_dataset.export_to('voc_detection')
 ```
 
+
+### Data Ingestion Pipelines
+```python
+from clarifai_datautils.text import Pipeline, PDFPartition
+from clarifai_datautils.text.pipeline.cleaners import Clean_extra_whitespace
+
+# Define the pipeline
+pipeline = Pipeline(
+    name='pipeline-1',
+    transformations=[
+        PDFPartition(chunking_strategy = "by_title",max_characters = 1024),
+        Clean_extra_whitespace()
+    ]
+)
+
+
+# Using SDK to upload
+from clarifai.client import Dataset
+dataset = Dataset(dataset_url)
+dataset.upload_dataset(pipeline.run(files = file_path, loader = True))
+
+```
+
+
 ## More Examples
 
 See many more code examples in this [repo](https://github.com/Clarifai/examples).
```

### Comparing `clarifai-datautils-0.0.2/clarifai_datautils/constants/annotations.py` & `clarifai-datautils-0.0.3/clarifai_datautils/constants/annotations.py`

 * *Files identical despite different names*

### Comparing `clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/annotations.py` & `clarifai-datautils-0.0.3/clarifai_datautils/image/annotation_conversion/annotations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Any, Dict
 
 from datumaro.components.dataset import Dataset
 from datumaro.components.errors import (DatasetError, DatasetImportError, DatasetNotFoundError,
                                         MultipleFormatsMatchError)
 
+from clarifai_datautils.base import ClarifaiDataLoader
 from clarifai_datautils.constants.annotations import (IMAGE_ANNOTATION_FORMATS,
                                                       IMAGE_ANNOTATION_FORMATS_TO_TASKS,
                                                       IMAGE_FORMAT_MAP)
+from clarifai_datautils.constants.base import DATASET_UPLOAD_TASKS
 from clarifai_datautils.errors import AnnotationsDatasetError, AnnotationsFormatError
-from clarifai_datautils.image.annotation_conversion.base import ClarifaiDataLoader
 from clarifai_datautils.image.annotation_conversion.loaders import (ClassificationDataLoader,
                                                                     DetectionDataLoader,
                                                                     SegmentationDataLoader)
 from clarifai_datautils.image.annotation_conversion.utils import Clarifai_to_Datumaro
 
 
 class ImageAnnotations():
@@ -161,19 +162,19 @@
         A ClarifaiDataloader object.
 
     Example:
         >>> from clarifai_datautils import ImageAnnotations
         >>> format = ImageAnnotations.import_from(path=folder_path, format = 'coco_detection')
         >>> clarifai_dataset_loader = format.dataloader
     """
-    if self.task == 'visual_classification':
+    if self.task == DATASET_UPLOAD_TASKS.VISUAL_CLASSIFICATION:
       return ClassificationDataLoader(self._dataset)
-    elif self.task == 'visual_detection':
+    elif self.task == DATASET_UPLOAD_TASKS.VISUAL_DETECTION:
       return DetectionDataLoader(self._dataset)
-    elif self.task == 'visual_segmentation':
+    elif self.task == DATASET_UPLOAD_TASKS.VISUAL_SEGMENTATION:
       return SegmentationDataLoader(self._dataset)
 
   def __str__(self) -> str:
     separator = "\t"
     return (f"Dataset\n"
             f"\tsize={len(self._dataset._data)}\n"
             f"\tsource_path={self._dataset._source_path}\n"
```

### Comparing `clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/base.py` & `clarifai-datautils-0.0.3/clarifai_datautils/base/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import TypeVar, Union
 
-from .features import (VisualClassificationFeatures, VisualDetectionFeatures,
-                       VisualSegmentationFeatures)
+from clarifai_datautils.constants.base import DATASET_UPLOAD_TASKS
 
-DATASET_UPLOAD_TASKS = ["visual_classification", "visual_detection", "visual_segmentation"]
+from .features import (TextFeatures, VisualClassificationFeatures, VisualDetectionFeatures,
+                       VisualSegmentationFeatures)
 
 OutputFeaturesType = TypeVar(
     'OutputFeaturesType',
-    bound=Union[VisualClassificationFeatures, VisualDetectionFeatures, VisualSegmentationFeatures])
+    bound=Union[VisualClassificationFeatures, VisualDetectionFeatures, VisualSegmentationFeatures,
+                TextFeatures])
 
 
 class ClarifaiDataLoader:
   """Clarifai data loader base class."""
 
   def __init__(self) -> None:
     pass
```

### Comparing `clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/features.py` & `clarifai-datautils-0.0.3/clarifai_datautils/base/features.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,31 +8,44 @@
   """Image classification datasets preprocessing output features."""
   image_path: str
   labels: List[Union[str, int]]  # List[str or int] to cater for multi-class tasks
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
   metadata: Optional[dict] = None
   image_bytes: Optional[bytes] = None
+  label_ids: Optional[List[str]] = None
 
 
 @dataclass
 class VisualDetectionFeatures:
   """Image Detection datasets preprocessing output features."""
   image_path: str
   labels: List[Union[str, int]]
   bboxes: List[List[float]]
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
   metadata: Optional[dict] = None
   image_bytes: Optional[bytes] = None
+  label_ids: Optional[List[str]] = None
 
 
 @dataclass
 class VisualSegmentationFeatures:
   """Image Segmentation datasets preprocessing output features."""
   image_path: str
   labels: List[Union[str, int]]
   polygons: List[List[List[float]]]
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
   metadata: Optional[dict] = None
   image_bytes: Optional[bytes] = None
+  label_ids: Optional[List[str]] = None
+
+
+@dataclass
+class TextFeatures:
+  """Text classification datasets preprocessing output features."""
+  text: str
+  labels: List[Union[str, int]]  # List[str or int] to cater for multi-class tasks
+  id: Optional[int] = None  # text_id
+  metadata: Optional[dict] = None
+  label_ids: Optional[List[str]] = None
```

### Comparing `clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/loaders.py` & `clarifai-datautils-0.0.3/clarifai_datautils/image/annotation_conversion/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import re
 
 import cv2
 import datumaro.plugins.transforms as transforms
 import numpy as np
 from datumaro.components.annotation import AnnotationType
 from datumaro.components.media import ImageFromNumpy
+from clarifai_datautils.constants.base import DATASET_UPLOAD_TASKS
 
-from .base import ClarifaiDataLoader
-from .features import (VisualClassificationFeatures, VisualDetectionFeatures,
-                       VisualSegmentationFeatures)
+from ...base import ClarifaiDataLoader
+from ...base.features import (VisualClassificationFeatures, VisualDetectionFeatures,
+                              VisualSegmentationFeatures)
 
 delimiters = [",", "|", ";", "/", "\\", ":", " "]
 
 
 class ClassificationDataLoader(ClarifaiDataLoader):
   """Annotation's Classificatoin Dataset object."""
 
@@ -31,15 +32,15 @@
     }
     label_map = annotation_object.categories()[AnnotationType.label]._indices
     self.label_map = dict([(value, key)
                            for key, value in label_map.items()])  #swapped key and value
 
   @property
   def task(self):
-    return "visual_classification"
+    return DATASET_UPLOAD_TASKS.VISUAL_CLASSIFICATION
 
   def __getitem__(self, index: int):
     dataset_item = self.annotation_object.get(
         id=self.map_ids[index]['id'], subset=self.map_ids[index]['subset'])
 
     image_path = dataset_item.media.path if type(dataset_item.media) != ImageFromNumpy else None
     # Some datasets have images stored as bytes instead of paths
@@ -86,15 +87,15 @@
     }
     label_map = annotation_object.categories()[AnnotationType.label]._indices
     self.label_map = dict([(value, key)
                            for key, value in label_map.items()])  #swapped key and value
 
   @property
   def task(self):
-    return "visual_detection"
+    return DATASET_UPLOAD_TASKS.VISUAL_DETECTION
 
   def __getitem__(self, index: int):
     dataset_item = self.annotation_object.get(
         id=self.map_ids[index]['id'], subset=self.map_ids[index]['subset'])
 
     image_path = dataset_item.media.path
     image_bytes = dataset_item.media.bytes
@@ -166,15 +167,15 @@
     }
     label_map = annotation_object.categories()[AnnotationType.label]._indices
     self.label_map = dict([(value, key)
                            for key, value in label_map.items()])  #swapped key and value
 
   @property
   def task(self):
-    return "visual_segmentation"
+    return DATASET_UPLOAD_TASKS.VISUAL_SEGMENTATION
 
   def __getitem__(self, index: int):
     dataset_item = self.annotation_object.get(
         id=self.map_ids[index]['id'], subset=self.map_ids[index]['subset'])
 
     image_path = dataset_item.media.path
     image_bytes = dataset_item.media.bytes
```

### Comparing `clarifai-datautils-0.0.2/clarifai_datautils/image/annotation_conversion/utils.py` & `clarifai-datautils-0.0.3/clarifai_datautils/image/annotation_conversion/utils.py`

 * *Files identical despite different names*

### Comparing `clarifai-datautils-0.0.2/clarifai_datautils.egg-info/PKG-INFO` & `clarifai-datautils-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai-datautils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Clarifai Data Utils
 Home-page: https://github.com/Clarifai/clarifai-python-datautils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,15 @@
 ---
 ## Table Of Contents
 
 * **[Installation](#installation)**
 * **[Getting Started](#getting-started)**
 * **[Features](#features)**
   * [Image Utils](#image-utils)
+  * [Data Ingestion Pipeline](#ingestion-pipeline)
 * **[Usage](#usage)**
 * **[Examples](#more-examples)**
 
 
 ## Installation
 
 
@@ -75,15 +76,17 @@
 ## Features
 
 ### Image Utils
 - #### Annotation Loader
   - Load various annotated image datasets and export to clarifai Platform
   - Convert from one annotation format to other supported annotation formats
 
-
+### Data Ingestion Pipeline
+  - Easy to use pipelines to load data from files and ingest into clarifai platfrom.
+  - Load text files(pdf, doc, etc..) , transform, chunk and upload to the Clarifai Platform
 
 ## Usage
 ### Image Annotation Loader
 ```python
 from clarifai_datautils import ImageAnnotations
 #import from folder
 coco_dataset = ImageAnnotations.import_from(path='folder_path',format= 'coco_detection')
@@ -98,10 +101,34 @@
 coco_dataset.get_info()
 
 
 #exporting to other formats
 coco_dataset.export_to('voc_detection')
 ```
 
+
+### Data Ingestion Pipelines
+```python
+from clarifai_datautils.text import Pipeline, PDFPartition
+from clarifai_datautils.text.pipeline.cleaners import Clean_extra_whitespace
+
+# Define the pipeline
+pipeline = Pipeline(
+    name='pipeline-1',
+    transformations=[
+        PDFPartition(chunking_strategy = "by_title",max_characters = 1024),
+        Clean_extra_whitespace()
+    ]
+)
+
+
+# Using SDK to upload
+from clarifai.client import Dataset
+dataset = Dataset(dataset_url)
+dataset.upload_dataset(pipeline.run(files = file_path, loader = True))
+
+```
+
+
 ## More Examples
 
 See many more code examples in this [repo](https://github.com/Clarifai/examples).
```

### Comparing `clarifai-datautils-0.0.2/clarifai_datautils.egg-info/SOURCES.txt` & `clarifai-datautils-0.0.3/clarifai_datautils.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,24 @@
 clarifai_datautils/__init__.py
 clarifai_datautils/errors.py
 clarifai_datautils.egg-info/PKG-INFO
 clarifai_datautils.egg-info/SOURCES.txt
 clarifai_datautils.egg-info/dependency_links.txt
 clarifai_datautils.egg-info/requires.txt
 clarifai_datautils.egg-info/top_level.txt
+clarifai_datautils/base/__init__.py
+clarifai_datautils/base/features.py
 clarifai_datautils/constants/annotations.py
+clarifai_datautils/constants/base.py
+clarifai_datautils/constants/pipeline.py
 clarifai_datautils/image/__init__.py
 clarifai_datautils/image/annotation_conversion/__init__.py
 clarifai_datautils/image/annotation_conversion/annotations.py
-clarifai_datautils/image/annotation_conversion/base.py
-clarifai_datautils/image/annotation_conversion/features.py
 clarifai_datautils/image/annotation_conversion/loaders.py
-clarifai_datautils/image/annotation_conversion/utils.py
+clarifai_datautils/image/annotation_conversion/utils.py
+clarifai_datautils/text/__init__.py
+clarifai_datautils/text/pipeline/PDF.py
+clarifai_datautils/text/pipeline/Text.py
+clarifai_datautils/text/pipeline/base.py
+clarifai_datautils/text/pipeline/cleaners.py
+clarifai_datautils/text/pipeline/extractors.py
+clarifai_datautils/text/pipeline/loaders.py
```

### Comparing `clarifai-datautils-0.0.2/setup.py` & `clarifai-datautils-0.0.3/setup.py`

 * *Files identical despite different names*

