# Comparing `tmp/lit_ecology_classifier-0.1.tar.gz` & `tmp/lit_ecology_classifier-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lit_ecology_classifier-0.1.tar", last modified: Wed May 29 09:43:46 2024, max compression
+gzip compressed data, was "lit_ecology_classifier-0.2.tar", last modified: Wed May 29 12:57:30 2024, max compression
```

## Comparing `lit_ecology_classifier-0.1.tar` & `lit_ecology_classifier-0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/
--rw-r--r--   0 bkch     (29810) em09     (32012)     1068 2024-05-29 09:38:39.000000 lit_ecology_classifier-0.1/LICENSE
--rw-r--r--   0 bkch     (29810) em09     (32012)     3518 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/PKG-INFO
--rw-r--r--   0 bkch     (29810) em09     (32012)     2898 2024-05-29 09:43:06.000000 lit_ecology_classifier-0.1/README.md
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/
--rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/__init__.py
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/data/
--rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/data/__init__.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     8631 2024-05-29 08:00:08.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/data/datamodule.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     8457 2024-05-28 12:07:34.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/data/tardataset.py
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/helpers/
--rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/helpers/__init__.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     2652 2024-05-29 09:33:38.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/helpers/argparser.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     1145 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/helpers/calc_class_weights.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     8045 2024-05-29 07:04:21.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/helpers/helpers.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     3469 2024-05-29 08:00:08.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/main.py
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/models/
--rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/models/__init__.py
--rw-r--r--   0 bkch     (29810) em09     (32012)    11341 2024-05-29 09:29:55.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/models/model.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     2699 2024-05-28 12:48:04.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/models/setup_model.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     1817 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.1/lit_ecology_classifier/predict.py
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/
--rw-r--r--   0 bkch     (29810) em09     (32012)     3518 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/PKG-INFO
--rw-r--r--   0 bkch     (29810) em09     (32012)      836 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)        1 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)       76 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/entry_points.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)       69 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/requires.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)       23 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/top_level.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)       38 2024-05-29 09:43:46.000000 lit_ecology_classifier-0.1/setup.cfg
--rw-r--r--   0 bkch     (29810) em09     (32012)     1026 2024-05-29 09:37:46.000000 lit_ecology_classifier-0.1/setup.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/
+-rw-r--r--   0 bkch     (29810) em09     (32012)     1068 2024-05-29 12:20:15.000000 lit_ecology_classifier-0.2/LICENSE
+-rw-r--r--   0 bkch     (29810) em09     (32012)     3629 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/PKG-INFO
+-rw-r--r--   0 bkch     (29810) em09     (32012)     2969 2024-05-29 12:20:15.000000 lit_ecology_classifier-0.2/README.md
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/
+-rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/__init__.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/data/
+-rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/data/__init__.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     8631 2024-05-29 08:00:08.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/data/datamodule.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     8457 2024-05-28 12:07:34.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/data/tardataset.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/helpers/
+-rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/helpers/__init__.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     2652 2024-05-29 12:47:00.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/helpers/argparser.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     1145 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/helpers/calc_class_weights.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     8045 2024-05-29 07:04:21.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/helpers/helpers.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     3469 2024-05-29 08:00:08.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/main.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/models/
+-rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/models/__init__.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)    11407 2024-05-29 12:46:01.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/models/model.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     2665 2024-05-29 12:45:34.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/models/setup_model.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     1817 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2/lit_ecology_classifier/predict.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/
+-rw-r--r--   0 bkch     (29810) em09     (32012)     3629 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 bkch     (29810) em09     (32012)      836 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)        1 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)       76 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)       69 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/requires.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)       23 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/top_level.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)       38 2024-05-29 12:57:30.000000 lit_ecology_classifier-0.2/setup.cfg
+-rw-r--r--   0 bkch     (29810) em09     (32012)     1074 2024-05-29 12:57:16.000000 lit_ecology_classifier-0.2/setup.py
```

### Comparing `lit_ecology_classifier-0.1/LICENSE` & `lit_ecology_classifier-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/PKG-INFO` & `lit_ecology_classifier-0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: lit_ecology_classifier
-Version: 0.1
+Version: 0.2
 Summary: Image Classifier optimised for ecology use-cases
 Home-page: https://github.com/kaechb/lit_ecology_classifier
 Author: Benno Kaech
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
 Requires-Dist: lightning
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 
 # Lit Ecology Classifier
-
+Documentation: https://lit-ecology-classifier.readthedocs.io/en/latest/
 Lit Ecology Classifier is a machine learning project designed for image classification tasks. It leverages PyTorch Lightning for streamlined training and evaluation processes.
 
 ## Features
 
 - Easy configuration and setup
 - Utilizes PyTorch Lightning for robust training and evaluation
 - Supports training on multiple GPUs
```

### Comparing `lit_ecology_classifier-0.1/README.md` & `lit_ecology_classifier-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Lit Ecology Classifier
-
+Documentation: https://lit-ecology-classifier.readthedocs.io/en/latest/
 Lit Ecology Classifier is a machine learning project designed for image classification tasks. It leverages PyTorch Lightning for streamlined training and evaluation processes.
 
 ## Features
 
 - Easy configuration and setup
 - Utilizes PyTorch Lightning for robust training and evaluation
 - Supports training on multiple GPUs
```

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/data/datamodule.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/data/tardataset.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/data/tardataset.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/helpers/argparser.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/helpers/argparser.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/helpers/calc_class_weights.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/helpers/calc_class_weights.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/helpers/helpers.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/main.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/main.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/models/model.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,17 +207,17 @@
 
         if self.hparams.use_wandb:
             self.logger.log_image(key=f"score_distributions", images=[fig_score], step=self.current_epoch)
             self.logger.log_image(key="confusion_matrix", images=[fig], step=self.current_epoch)
             self.logger.log_image(key="confusion_matrix_norm", images=[fig2], step=self.current_epoch)
         else:
             logging.info(f"Saving confusion matrix and score distributions to {self.hparams.train_outpath}")
-            fig.savefig(f"{self.hparams.train_outpath}/confusion_matrix_test_set.png")
-            fig2.savefig(f"{self.hparams.train_outpath}/confusion_matrix_normalized_test_set.png")
-            fig_score.savefig(f"{self.hparams.train_outpath}/score_distributions_epoch_test_set.png")
+            fig.savefig(f"{self.hparams.train_outpath}/{self.logger.log_dir}/confusion_matrix_test_set.png")
+            fig2.savefig(f"{self.hparams.train_outpath}/{self.logger.log_dir}/confusion_matrix_normalized_test_set.png")
+            fig_score.savefig(f"{self.hparams.train_outpath}/{self.logger.log_dir}/score_distributions_epoch_test_set.png")
         plt.close(fig)
         plt.close(fig2)
         plt.close(fig_score)
 
     def on_predict_start(self) -> None:
         """
         Hook for the start of the inference phase.
```

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/models/setup_model.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/models/setup_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import numpy as np
 import timm
 import torch
 from safetensors.torch import load_file
 
-def setup_model( finetune, num_classes,checkpoint_path="checkpoints/beitv2_base_patch16_224.in1k_ft_in22k_in1k.safetensors", **kwargs):
+def setup_model( finetune, num_classes,checkpoint_path="checkpoints/backbone.safetensors", **kwargs):
     """
     Set up and return the specified model architecture.
 
     Args:
         architecture (str): The model architecture to use.
         main_param_path (str): Path to the directory containing main parameters.
         ensemble (bool): Whether to use model ensembling.
```

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier/predict.py` & `lit_ecology_classifier-0.2/lit_ecology_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/PKG-INFO` & `lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: lit_ecology_classifier
-Version: 0.1
+Version: 0.2
 Summary: Image Classifier optimised for ecology use-cases
 Home-page: https://github.com/kaechb/lit_ecology_classifier
 Author: Benno Kaech
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
 Requires-Dist: lightning
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 
 # Lit Ecology Classifier
-
+Documentation: https://lit-ecology-classifier.readthedocs.io/en/latest/
 Lit Ecology Classifier is a machine learning project designed for image classification tasks. It leverages PyTorch Lightning for streamlined training and evaluation processes.
 
 ## Features
 
 - Easy configuration and setup
 - Utilizes PyTorch Lightning for robust training and evaluation
 - Supports training on multiple GPUs
```

### Comparing `lit_ecology_classifier-0.1/lit_ecology_classifier.egg-info/SOURCES.txt` & `lit_ecology_classifier-0.2/lit_ecology_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.1/setup.py` & `lit_ecology_classifier-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
 
 
+
 with open("README.md", "r", encoding="utf-8") as fh:
-        long_description = fh.read()
+    long_description = fh.read()
 
 setup(
     name='lit_ecology_classifier',
-    version='0.1',
-    long_description=long_description,
+    version='0.2',
     description='Image Classifier optimised for ecology use-cases',
     packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     install_requires=[
         'torch',
         'torchvision',
         'torchaudio ',
         'lightning',
         'numpy',
         'scipy',
```

