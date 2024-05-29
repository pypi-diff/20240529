# Comparing `tmp/tracebloc_package-0.5.31.tar.gz` & `tmp/tracebloc_package-0.5.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-0.5.31.tar", last modified: Wed Apr 17 05:27:51 2024, max compression
+gzip compressed data, was "tracebloc_package-0.5.50.tar", last modified: Wed May 29 07:37:07 2024, max compression
```

## Comparing `tracebloc_package-0.5.31.tar` & `tracebloc_package-0.5.50.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-04-17 05:27:51.843870 tracebloc_package-0.5.31/
--rw-r--r--   0 syedsaqlain   (501) staff       (20)     1048 2023-08-28 08:45:59.000000 tracebloc_package-0.5.31/LICENSE.txt
--rw-r--r--   0 syedsaqlain   (501) staff       (20)      570 2024-04-17 05:27:51.843937 tracebloc_package-0.5.31/PKG-INFO
--rw-r--r--   0 syedsaqlain   (501) staff       (20)      188 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/README.md
--rw-r--r--   0 syedsaqlain   (501) staff       (20)       78 2024-04-17 05:27:51.844350 tracebloc_package-0.5.31/setup.cfg
--rw-r--r--   0 syedsaqlain   (501) staff       (20)     1079 2024-04-17 05:20:16.000000 tracebloc_package-0.5.31/setup.py
-drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-04-17 05:27:51.842934 tracebloc_package-0.5.31/tracebloc_package/
--rw-r--r--   0 syedsaqlain   (501) staff       (20)      163 2024-04-17 05:12:58.000000 tracebloc_package-0.5.31/tracebloc_package/__init__.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)     5669 2023-08-28 08:45:59.000000 tracebloc_package-0.5.31/tracebloc_package/check_parameters.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)     6839 2024-04-17 05:12:58.000000 tracebloc_package-0.5.31/tracebloc_package/detection_utils.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)    14785 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/functional_checks.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)    63835 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)     7109 2023-11-10 07:00:05.000000 tracebloc_package-0.5.31/tracebloc_package/messages.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)    11380 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/pytorch_checks.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)     8085 2024-04-17 05:12:58.000000 tracebloc_package-0.5.31/tracebloc_package/tensorflow_checks.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)    15375 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/upload.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)    11057 2024-04-17 05:20:00.000000 tracebloc_package-0.5.31/tracebloc_package/user.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)    15093 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/utils.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)     3200 2023-08-28 08:45:59.000000 tracebloc_package-0.5.31/tracebloc_package/weights.py
--rw-r--r--   0 syedsaqlain   (501) staff       (20)     6669 2024-04-17 05:12:58.000000 tracebloc_package-0.5.31/tracebloc_package/yololoss.py
-drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-04-17 05:27:51.843761 tracebloc_package-0.5.31/tracebloc_package.egg-info/
--rw-r--r--   0 syedsaqlain   (501) staff       (20)      570 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/PKG-INFO
--rw-r--r--   0 syedsaqlain   (501) staff       (20)      711 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/SOURCES.txt
--rw-r--r--   0 syedsaqlain   (501) staff       (20)        1 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/dependency_links.txt
--rw-r--r--   0 syedsaqlain   (501) staff       (20)        1 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/not-zip-safe
--rw-r--r--   0 syedsaqlain   (501) staff       (20)      234 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/requires.txt
--rw-r--r--   0 syedsaqlain   (501) staff       (20)       18 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/top_level.txt
+drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-05-29 07:37:07.000607 tracebloc_package-0.5.50/
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     1048 2023-08-28 08:45:59.000000 tracebloc_package-0.5.50/LICENSE.txt
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     1393 2024-05-29 07:37:07.000706 tracebloc_package-0.5.50/PKG-INFO
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     1011 2024-04-28 21:39:51.000000 tracebloc_package-0.5.50/README.md
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)       78 2024-05-29 07:37:07.001062 tracebloc_package-0.5.50/setup.cfg
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     1088 2024-05-29 07:36:41.000000 tracebloc_package-0.5.50/setup.py
+drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-05-29 07:37:06.991337 tracebloc_package-0.5.50/tracebloc_package/
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      210 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/__init__.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    63959 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/linkModelDataSet.py
+drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-05-29 07:37:06.996801 tracebloc_package-0.5.50/tracebloc_package/task_checks/
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      127 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_checks/__init__.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     5669 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_checks/check_parameters.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    15022 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_checks/functional_checks.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    13263 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_checks/pytorch_checks.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     8098 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_checks/tensorflow_checks.py
+drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-05-29 07:37:07.000265 tracebloc_package-0.5.50/tracebloc_package/task_utils/
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      147 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_utils/__init__.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      615 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_utils/constants.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     1793 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_utils/keypoint_detection_utils.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     7109 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_utils/messages.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    13345 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_utils/object_detection_utils.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     8019 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/task_utils/utils.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    15329 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/upload.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    11227 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/user.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     3200 2024-05-29 07:27:45.000000 tracebloc_package-0.5.50/tracebloc_package/weights.py
+drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-05-29 07:37:06.994642 tracebloc_package-0.5.50/tracebloc_package.egg-info/
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     1393 2024-05-29 07:37:06.000000 tracebloc_package-0.5.50/tracebloc_package.egg-info/PKG-INFO
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      951 2024-05-29 07:37:06.000000 tracebloc_package-0.5.50/tracebloc_package.egg-info/SOURCES.txt
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)        1 2024-05-29 07:37:06.000000 tracebloc_package-0.5.50/tracebloc_package.egg-info/dependency_links.txt
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)        1 2024-05-29 07:37:06.000000 tracebloc_package-0.5.50/tracebloc_package.egg-info/not-zip-safe
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      234 2024-05-29 07:37:06.000000 tracebloc_package-0.5.50/tracebloc_package.egg-info/requires.txt
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)       18 2024-05-29 07:37:06.000000 tracebloc_package-0.5.50/tracebloc_package.egg-info/top_level.txt
```

### Comparing `tracebloc_package-0.5.31/LICENSE.txt` & `tracebloc_package-0.5.50/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.5.31/setup.py` & `tracebloc_package-0.5.50/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import setuptools
+from setuptools import setup, find_packages
 
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-setuptools.setup(
+setup(
     name="tracebloc_package",
-    version="0.5.31",
+    version="0.5.50",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package",
     license="MIT",
     python_requires=">=3",
-    packages=["tracebloc_package"],
+    packages=find_packages(),
     author="Tracebloc",
     author_email="lukas-wutke@tracebloc.io",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "requests==2.31.0",
         "termcolor==2.3.0",
@@ -27,11 +27,11 @@
         "dill==0.3.7",
         "silence_tensorflow==1.2.1",
         "torch==2.1.0",
         "torchvision==0.16.0",
         "torchlightning==0.0.0",
         "torchmetrics==1.2.0",
         "timm==0.9.10",
-        "transformers==4.35.2",
+        "transformers==4.36.0",
     ],
     zip_safe=False,
 )
```

### Comparing `tracebloc_package-0.5.31/tracebloc_package/check_parameters.py` & `tracebloc_package-0.5.50/tracebloc_package/task_checks/check_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,18 @@
 
     # Get the optimizer class
     optimizer_class = optimizers[optimizer_name.lower()]
 
     try:
         # Create an instance of the optimizer class
         optimiser = optimizer_class(learning_rate=learning_rate_func)
-        # if Valid optimiser and Return the optimizer instance
+        # if Valid optimizer and Return the optimizer instance
         return True, None
     except Exception as e:
-        # if not a valid optimiser/learning rate and Return the optimizer instance
+        # if not a valid optimizer/learning rate and Return the optimizer instance
         return False, e
 
 
 def get_learning_rate(learning_rate_name, **kwargs):
     if learning_rate_name == "constant":
         lr = kwargs.pop("value", 0.01)
         return lr
```

### Comparing `tracebloc_package-0.5.31/tracebloc_package/functional_checks.py` & `tracebloc_package-0.5.50/tracebloc_package/task_checks/functional_checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import inspect
 import sys
 import dis
 import re
 import shutil
 from inspect import getmembers, isfunction, isclass
-from .utils import *
+from ..task_utils.utils import *
+from ..task_utils.constants import *
 
 
 # base class for checks on model file
 class CheckModel:
     MAX_MODEL_NAME_LENGTH = 64
     message = ""
     model = None
@@ -19,24 +19,25 @@
     main_class = ""
     input_shape = ""
     output_classes = ""
     image_size = 224
     batch_size = 16
     framework = ""
     model_type = ""
-    category = CLASSIFICATION
+    category = IMAGE_CLASSIFICATION
     notallowed = ["__MACOSX", "__pycache__"]
     input_shape_patt = re.compile("(^input_shape\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     out_classes_patt = re.compile("(^output_classes\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     main_method_patt = re.compile("(^main_method\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     main_class_patt = re.compile("(^main_class\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     framework_patt = re.compile("(^framework\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     image_size_patt = re.compile("(^image_size\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     batch_size_patt = re.compile("(^batch_size\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     model_type_patt = re.compile("(^model_type\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
+    category_type_patt = re.compile("(^category\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
 
     def __init__(
         self, progress_bar, model_name=None, model_path=None
     ):  # pragma: no cover
         self.model_name = model_name
         self.model_path = model_path
         self.progress_bar = progress_bar
@@ -66,14 +67,15 @@
             filedata = tmp_fp.read()
             if TORCH_HUB_PATTERN in filedata:
                 self.file_not_allowed = True
 
         common_pattern_dict = {
             self.framework_patt: "framework",
             self.model_type_patt: "model_type",
+            self.category_type_patt: "category",
             self.out_classes_patt: "output_classes",
             self.input_shape_patt: "input_shape",
             self.main_method_patt: "main_method",
             self.main_class_patt: "main_class",
             self.image_size_patt: "image_size",
             self.batch_size_patt: "batch_size",
         }
@@ -100,20 +102,21 @@
                             main_file = True
 
                     remove_lines.append(linenum)
                     break
 
         if main_file:
             if self.framework == "":
-                print("Framework parameter missing from file")
-                return False, [], []
-            self.category = CLASSIFICATION if self.model_type == "" else DETECTION
-            if self.category == DETECTION and self.output_classes == "":
-                print("Output classes parameter missing from file")
-                return False, [], []
+                raise Exception("Framework parameter missing from file")
+            if self.category == "":
+                raise Exception("Category parameter missing from file")
+            if self.output_classes == "":
+                raise Exception("Output classes parameter missing from file")
+            if self.image_size == "" and self.input_shape is not None:
+                self.image_size = self.input_shape[1]
 
         return main_file, remove_lines, filedata.split("\n")
 
     def replace_vars(self, code):
         if re.search(
             f"[^a-zA-Z_\-0-9]{self.input_shape}[^a-zA-Z_\-0-9]", code
         ) or re.search(f"{self.input_shape}[^a-zA-Z_\-0-9]", code):
```

### Comparing `tracebloc_package-0.5.31/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-0.5.50/tracebloc_package/linkModelDataSet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import inspect
 import requests, json
-import dill
-import base64
 from termcolor import colored
-from tracebloc_package import check_parameters
-from .utils import *
-from .functional_checks import CheckModel
-from .tensorflow_checks import TensorflowChecks
-from .pytorch_checks import TorchChecks
-import torch.nn as nn
+from .task_checks import check_parameters
+from .task_utils.utils import *
+from .task_checks.tensorflow_checks import TensorflowChecks
+from .task_checks.pytorch_checks import TorchChecks
 
 
 class LinkModelDataSet:
     """
     creating a training plan and assign data set
     parameters: modelId, datasetId, token
 
@@ -34,15 +30,15 @@
         image_size,
         batchsize,
         model_path,
         url="",
         environment="production",
         framework=TENSORFLOW_FRAMEWORK,
         model_type="",
-        category=CLASSIFICATION,
+        category=IMAGE_CLASSIFICATION,
         loss=None,
     ):
         self.__framework = framework
         self.__url = url
         self.__token = token
         self.__earlystopCallback = {}
         self.__reducelrCallback = {}
@@ -95,15 +91,15 @@
         self.__rescale = "None"
         self.__validation_split = self.__default_validation_split()
         self.__shuffle = True
         self.__layers_non_trainable = ""
         self.__metrics = str(["accuracy"])
         self.__objective = ""
         self.__name = "None"
-        self.__modelType = model_type
+        self.__model_type = model_type
         self.__category = category
         self.__upperboundTime = 0
         self.__weights = weights
         self.__images_per_class = json.dumps(self.__class_names)
         self.__eligibility_passed = True
         self.__error_method = []
         self.__reform_model = False
@@ -158,15 +154,15 @@
         self.__rescale = "None"
         self.__validation_split = self.__default_validation_split()
         self.__shuffle = True
         self.__layers_non_trainable = ""
         self.__metrics = str(["accuracy"])
         self.__objective = ""
         self.__name = "None"
-        self.__modelType = "None"
+        self.__model_type = "None"
         self.__category = "Classification"
         self.__upperboundTime = 0
         self.__images_per_edge = self.__total_images
         self.__images_per_class = json.dumps(self.__class_names)
         self.__eligibility_passed = True
         self.__reform_model = False
         print("Training Plan Parameters reset")
@@ -681,15 +677,15 @@
                         self.__print_error(error_msg)
                 elif lossFunction[TYPE] == CUSTOM:
                     if os.path.exists(os.path.join(self.tmp_path, "loss.py")):
                         try:
                             model_checks = TensorflowChecks(
                                 model=self.__model,
                                 model_name=self.__modelName,
-                                model_type=self.__modelType,
+                                model_type=self.__model_type,
                                 category=self.__category,
                                 classes=self.__num_classes,
                                 progress_bar=None,
                                 message="",
                                 tmp_path=self.tmp_path,
                             )
                             model_checks.small_training_loop(
@@ -728,15 +724,15 @@
                     self.__print_error(error_msg)
             elif lossFunction[TYPE] == CUSTOM:
                 if os.path.exists(os.path.join(self.tmp_path, "loss.py")):
                     try:
                         model_checks = TorchChecks(
                             model=self.__model,
                             model_name=self.__modelName,
-                            model_type=self.__modelType,
+                            model_type=self.__model_type,
                             category=self.__category,
                             progress_bar=None,
                             message="",
                             image_size=self.__image_shape,
                             batch_size=self.__batchSize,
                             classes=self.__num_classes,
                             tmp_path=self.tmp_path,
@@ -1051,15 +1047,15 @@
 
     def channel_shift_range(self, channel_shift_range: float):
         """
         Float. Range for random channel shifts.
         example: trainingObject.channel_shift_range(0.4)
         default: 0.0
         """
-        if self.__framework == PYTORCH_FRAMEWORK and self.__image_type is not "rgb":
+        if self.__framework == PYTORCH_FRAMEWORK and self.__image_type != "rgb":
             error_msg = "channel_shift_range:You can not set channel_shift_range if image type is not rgb\n"
             self.__print_error(error_msg)
         elif type(channel_shift_range) == float:
             self.__channel_shift_range = channel_shift_range
             self.__remove_error_method()
         else:
             error_msg = (
@@ -1304,60 +1300,60 @@
     #     try:
     #         d.index(dtype.lower())
     #         self.__dtype = dtype.lower()
     #     except:
     #         print(f"Please provide supported fill modes: {d}\n\n")
     #
     # def metrics(self,metrics:list):
-    # 	'''
-    # 	List of strings.
-    # 	List of metrics to be evaluated by the model
-    # 	during training and testing.
-    # 	example: setMetrics(['accuracy','mse'])
-    # 	default: ['accuracy']
-    # 	'''
-    # 	if type(metrics)== list and all(isinstance(sub, str) for sub in metrics):
-    # 		metrics = str(metrics)
-    # 		self.__metrics = metrics
-    # 	else:
-    # 		print("Provide values as list of strings")
-    #
-    # 	def __display_time(self,seconds, granularity=5):
-    # 		intervals = (
-    # 		('weeks', 604800),  # 60 * 60 * 24 * 7
-    # 		('days', 86400),    # 60 * 60 * 24
-    # 		('hours', 3600),    # 60 * 60
-    # 		('minutes', 60),
-    # 		('seconds', 1),)
-    # 		result = []
-    #
-    # 		for name, count in intervals:
-    # 			value = seconds // count
-    # 			if value:
-    # 				seconds -= value * count
-    # 				if value == 1:
-    # 					name = name.rstrip('s')
-    # 				result.append("{} {}".format(value, name))
-    # 		return ', '.join(result[:granularity])
-    #
-    # 	def getEstimate(self):
-    #
-    # 		header = {'Authorization' : f"Token {self.__token}"}
-    # 		re = requests.post(f"{self.__url}flops/",headers= header,data={'datasetId':self.__datasetId,
-    # 			'batchSize':self.__batchSize,'noOfEpochs':self.__epochs,'modelName':self.__modelName})
-    # # 		print(re.status_code)
-    # 		if re.status_code == 200:
-    #
-    # 			body_unicode = re.content.decode('utf-8')
-    # 			content = int(json.loads(body_unicode))
-    # 			self.__upperboundTime = content
-    # 			cycleTime = content * self.__cycles
-    # 			display = self.__display_time(cycleTime)
+    #   '''
+    #   List of strings.
+    #   List of metrics to be evaluated by the model
+    #   during training and testing.
+    #   example: setMetrics(['accuracy','mse'])
+    #   default: ['accuracy']
+    #   '''
+    #   if type(metrics)== list and all(isinstance(sub, str) for sub in metrics):
+    #       metrics = str(metrics)
+    #       self.__metrics = metrics
+    #   else:
+    #       print("Provide values as list of strings")
+    #
+    #   def __display_time(self,seconds, granularity=5):
+    #       intervals = (
+    #       ('weeks', 604800),  # 60 * 60 * 24 * 7
+    #       ('days', 86400),    # 60 * 60 * 24
+    #       ('hours', 3600),    # 60 * 60
+    #       ('minutes', 60),
+    #       ('seconds', 1),)
+    #       result = []
+    #
+    #       for name, count in intervals:
+    #           value = seconds // count
+    #           if value:
+    #               seconds -= value * count
+    #               if value == 1:
+    #                   name = name.rstrip('s')
+    #               result.append("{} {}".format(value, name))
+    #       return ', '.join(result[:granularity])
+    #
+    #   def getEstimate(self):
+    #
+    #       header = {'Authorization' : f"Token {self.__token}"}
+    #       re = requests.post(f"{self.__url}flops/",headers= header,data={'datasetId':self.__datasetId,
+    #           'batchSize':self.__batchSize,'noOfEpochs':self.__epochs,'modelName':self.__modelName})
+    # #         print(re.status_code)
+    #       if re.status_code == 200:
+    #
+    #           body_unicode = re.content.decode('utf-8')
+    #           content = int(json.loads(body_unicode))
+    #           self.__upperboundTime = content
+    #           cycleTime = content * self.__cycles
+    #           display = self.__display_time(cycleTime)
     #
-    # 			print(f"It will take around {display} to complete {self.__cycles} cycles for given training plan.")
+    #           print(f"It will take around {display} to complete {self.__cycles} cycles for given training plan.")
 
     def __checkTrainingPlan(self):
         # call API to compare current training plan for duplication
         header = {"Authorization": f"Token {self.__token}"}
         data = {"parameters": json.dumps(self.__getParameters())}
         # print(data,"\n\n")
         re = requests.post(
@@ -1439,14 +1435,15 @@
                 if self._environment != "production":
                     print(re.content, "\n")
                 text = colored(
                     "Error:Experiment creation Failed. Please ensure you have entered correct parameters.",
                     "red",
                 )
                 print(text, "\n")
+            self.resetTrainingPlan()
 
     def __getParameters(self):
         parameters = {
             "message": "training",
             "datasetId": self.__datasetId,
             "epochs": self.__epochs,
             "cycles": self.__cycles,
@@ -1475,16 +1472,15 @@
             "rescale": self.__rescale,
             "validation_split": self.__validation_split,
             "shuffle": self.__shuffle,
             "layersFreeze": self.__layers_non_trainable,
             "metrics": self.__metrics,
             "objective": self.__objective,
             "name": self.__name,
-            "modelType": self.__modelType,
-            "model_type": self.__modelType,
+            "model_type": self.__model_type,
             "category": self.__category,
             "upperboundTime": self.__upperboundTime,
             "callbacks": self.__callbacks,
             "pre_trained_weights": self.__weights,
             "subdataset": self.__subdataset,
             "images_per_edge": json.dumps(self.__images_per_edge),
             "images_per_class": self.__images_per_class,
```

### Comparing `tracebloc_package-0.5.31/tracebloc_package/messages.py` & `tracebloc_package-0.5.50/tracebloc_package/task_utils/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.5.31/tracebloc_package/pytorch_checks.py` & `tracebloc_package-0.5.50/tracebloc_package/task_checks/pytorch_checks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import os.path
-
-import torch
-from torch.utils.data import DataLoader
 from collections import OrderedDict
 import torch.optim as optim
 import torch.nn as nn
-from .detection_utils import *
-from .utils import *
+from ..task_utils.utils import *
+from torch.utils.data import DataLoader
 
 
 class TorchChecks:
     def __init__(self, **kwargs):
         validate_kwargs(
             kwargs,
             {
@@ -69,31 +66,47 @@
             # Define the number of fake images and other properties
             # Create fake image data
             train_dataset = dummy_dataset_pytorch(
                 image_size=self.image_size,
                 num_classes=self.classes,
                 category=self.category,
                 model_type=self.model_type,
-                tmp_path=self.tmp_path,
-            )
-
-            train_loader = DataLoader(
-                train_dataset, batch_size=self.batch_size, shuffle=True
             )
 
-            # train_loader, classes = mock_torch_data(self.tmp_path)
             if self.criterion is not None:
                 self.get_loss_function(custom_loss)
 
-            if self.category == CLASSIFICATION:
+            if self.category == IMAGE_CLASSIFICATION:
+                train_loader = DataLoader(
+                    train_dataset, batch_size=self.batch_size, shuffle=True
+                )
                 self.classification_training(train_loader)
-            elif self.model_type == YOLO:
-                self.yolo_training(train_loader)
-            elif self.model_type == RCNN:
-                self.rcnn_training(train_loader)
+            elif self.category == OBJECT_DETECTION:
+                if self.model_type == YOLO:
+                    train_loader = DataLoader(
+                        train_dataset, batch_size=self.batch_size, shuffle=True
+                    )
+                    self.yolo_training(train_loader)
+                elif self.model_type == RCNN:
+                    train_loader = DataLoader(
+                        train_dataset, batch_size=self.batch_size, shuffle=True, collate_fn=self.collate_fn
+                    )
+                    self.rcnn_training(train_loader)
+                else:
+                    raise Exception("Unsupported model")
+            elif self.category == KEYPOINT_DETECTION:
+                if self.model_type == RCNN:
+                    train_loader = DataLoader(
+                        train_dataset, batch_size=self.batch_size, shuffle=True, collate_fn=self.collate_fn
+                    )
+                else:
+                    train_loader = DataLoader(
+                        train_dataset, batch_size=self.batch_size, shuffle=True
+                    )
+                self.keypoint_training(train_loader)
             else:
                 # Raise an exception for unsupported models
                 raise Exception("Unsupported model")
 
             # dump weights from trained model will be used in averaging check
             get_model_parameters(
                     model=self.model,
@@ -178,32 +191,33 @@
             del params_dict
             del state_dict
             del parameters
         except Exception as e:
             raise
 
     def get_loss_function(self, custom_loss=False):
-        if self.category == CLASSIFICATION:
-            self.criterion = nn.CrossEntropyLoss()
-        if custom_loss or self.category == DETECTION:
+        if custom_loss or self.category == OBJECT_DETECTION:
             try:
                 import sys
 
                 sys.path.append(self.tmp_path)
                 if os.path.exists(os.path.join(self.tmp_path, "loss.py")):
                     from loss import Custom_loss
 
-                    self.criterion = Custom_loss
-                    self.loss = self.criterion
+                    self.loss = self.criterion = Custom_loss
                 else:
                     raise Exception(
                         "loss.py file missing in the zip.\n Please refer docs for more information."
                     )
             except Exception as e:
                 raise e
+        elif self.model_type == KEYPOINT_DETECTION:
+            self.criterion = nn.MSELoss(reduction='sum')
+        else:
+            self.criterion = nn.CrossEntropyLoss()
         self.progress_bar.update(1)
 
     def yolo_training(self, train_loader):
         total_correct = 0
         total_samples = 0
         for epoch in range(1):  # loop over the dataset multiple times
             running_loss = 0.0
@@ -245,14 +259,44 @@
                 loss = self.criterion(outputs, labels)
                 loss.backward()
                 optimizer.step()
 
                 # print statistics
                 running_loss += loss.item()
 
+    def keypoint_training(self, train_loader):
+        optimizer = optim.SGD(self.model.parameters(), lr=0.001, momentum=0.9)
+
+        try:
+
+            total_loss = 0
+            num_batches = 0
+            self.model.train()
+
+            for i, data in enumerate(train_loader, 0):
+                optimizer.zero_grad()
+                images, targets = data
+                if self.model_type == RCNN:
+                    loss_dict = self.model(images, targets)
+
+                    losses = sum(loss for loss in loss_dict.values())
+                    total_loss += losses.item()
+                    num_batches += 1
+                else:
+                    keypoints_targets = targets['keypoints']  # Shape: (batch_size, num_keypoints, 3)
+
+                    outputs = self.model(images)
+                    losses = self.criterion(outputs, keypoints_targets)
+
+                losses.backward()
+                optimizer.step()
+
+        except Exception as e:
+            raise e
+
     def rcnn_training(self, train_loader):
         for epoch in range(1):  # loop over the dataset multiple times
             running_loss = 0.0
             for i, data in enumerate(train_loader, 0):
                 # get the inputs; data is a list of [inputs, labels]
                 images, targets = data
                 targets = torch.tensor(targets, dtype=torch.long)
```

### Comparing `tracebloc_package-0.5.31/tracebloc_package/tensorflow_checks.py` & `tracebloc_package-0.5.50/tracebloc_package/task_checks/tensorflow_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from silence_tensorflow import silence_tensorflow
+from ..task_utils.utils import *
 
 silence_tensorflow()
-from .utils import *
+
 
 
 class TensorflowChecks:
     def __init__(self, **kwargs):
         validate_kwargs(
             kwargs,
             {
```

### Comparing `tracebloc_package-0.5.31/tracebloc_package/upload.py` & `tracebloc_package-0.5.50/tracebloc_package/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-import pickletools
 import shutil
 import sys
-import torch
-import requests, json, pickle
-from importlib.machinery import SourceFileLoader
+import requests, json
 from termcolor import colored
-import os
 import rich
 from tqdm import tqdm
-from .utils import *
-from .functional_checks import CheckModel
-from .tensorflow_checks import TensorflowChecks
-from .pytorch_checks import TorchChecks
+from .task_utils.utils import *
+from .task_checks.functional_checks import CheckModel
+from .task_checks.tensorflow_checks import TensorflowChecks
+from .task_checks.pytorch_checks import TorchChecks
 
 # hide warnings from tensorflow
 import warnings
 
 warnings.filterwarnings("ignore")
 
 
@@ -32,15 +28,15 @@
         self.model_check_class = None
         self.progress_bar = None
         self.progress_bar_2 = None
         self.__modelname = ""
         self.__model_path = ""
         self.__weights_path = ""
         self.__framework = TENSORFLOW_FRAMEWORK
-        self.__category = CLASSIFICATION
+        self.__category = IMAGE_CLASSIFICATION
         self.__model_type = ""
         self.__image_size = 224
         self.__batch_size = 16
         self.__classes = 0
         self.__ext = ".py"
         self.model = None
         self.loss = None
```

### Comparing `tracebloc_package-0.5.31/tracebloc_package/user.py` & `tracebloc_package-0.5.50/tracebloc_package/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # import useful libraries
-import getpass
 import requests
 import json
-import getpass, os
+import getpass
 from .upload import Model
 from .linkModelDataSet import LinkModelDataSet
 from termcolor import colored
 import rich
-from .utils import *
+from .task_utils.utils import *
 
 
 class User:
     """
     Parameters: username, password
 
     ***
     Please provide a valid username and password
     Call getToken method on Login to get new token for provided
     username and password
     """
 
-    def __init__(self, environment="production"):
+    def __init__(self, environment="production", username=None, password=None):
         self.__environment = environment
         self.__url = self.env_url(self.__environment)
         if self.__url is None:
             text = colored(
                 "\nThe class does not take any arguments. Just run: user = User()",
                 "red",
             )
             print(text, "\n")
             return
-        self.__username = input("Enter your email address : ")
-        self.__password = getpass.getpass("Enter your password : ")
+        self.__username = username
+        if not self.__username:
+            self.__username = input("Enter your email address : ")
+        self.__password = password
+        if not self.__password:
+            self.__password = getpass.getpass("Enter your password : ")
         self.__token = self.login()
         self.__ext = ".py"
         self.__image_size = 224
         self.__batch_size = 16
         self.__model_path = ""
         self.__framework = TENSORFLOW_FRAMEWORK
-        self.__category = CLASSIFICATION
+        self.__category = IMAGE_CLASSIFICATION
         self.__model_type = ""
         self.__modelId = ""
         self.__modelName = ""
         self.__weights = False
         self.__model = None
         self.__loss = None
```

### Comparing `tracebloc_package-0.5.31/tracebloc_package/weights.py` & `tracebloc_package-0.5.50/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.5.31/tracebloc_package.egg-info/SOURCES.txt` & `tracebloc_package-0.5.50/tracebloc_package.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 tracebloc_package/__init__.py
-tracebloc_package/check_parameters.py
-tracebloc_package/detection_utils.py
-tracebloc_package/functional_checks.py
 tracebloc_package/linkModelDataSet.py
-tracebloc_package/messages.py
-tracebloc_package/pytorch_checks.py
-tracebloc_package/tensorflow_checks.py
 tracebloc_package/upload.py
 tracebloc_package/user.py
-tracebloc_package/utils.py
 tracebloc_package/weights.py
-tracebloc_package/yololoss.py
 tracebloc_package.egg-info/PKG-INFO
 tracebloc_package.egg-info/SOURCES.txt
 tracebloc_package.egg-info/dependency_links.txt
 tracebloc_package.egg-info/not-zip-safe
 tracebloc_package.egg-info/requires.txt
-tracebloc_package.egg-info/top_level.txt
+tracebloc_package.egg-info/top_level.txt
+tracebloc_package/task_checks/__init__.py
+tracebloc_package/task_checks/check_parameters.py
+tracebloc_package/task_checks/functional_checks.py
+tracebloc_package/task_checks/pytorch_checks.py
+tracebloc_package/task_checks/tensorflow_checks.py
+tracebloc_package/task_utils/__init__.py
+tracebloc_package/task_utils/constants.py
+tracebloc_package/task_utils/keypoint_detection_utils.py
+tracebloc_package/task_utils/messages.py
+tracebloc_package/task_utils/object_detection_utils.py
+tracebloc_package/task_utils/utils.py
```

