# Comparing `tmp/furiosa-serving-0.9.0rc3.tar.gz` & `tmp/furiosa_serving-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-serving-0.9.0rc3.tar", last modified: Fri Apr 14 21:26:03 2023, max compression
+gzip compressed data, was "furiosa_serving-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `furiosa-serving-0.9.0rc3.tar` & `furiosa_serving-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        0 2023-04-14 21:20:23.032568 furiosa-serving-0.9.0rc3/CONTRIBUTING.md
--rw-r--r--   0        0        0      378 2023-04-14 21:20:23.032568 furiosa-serving-0.9.0rc3/Makefile
--rw-r--r--   0        0        0    11731 2023-04-14 21:20:23.032568 furiosa-serving-0.9.0rc3/README.md
--rw-r--r--   0        0        0     2636 2023-04-14 21:20:23.032568 furiosa-serving-0.9.0rc3/examples/assets/images/1234567890.jpg
--rw-r--r--   0        0        0     1286 2023-04-14 21:20:23.032568 furiosa-serving-0.9.0rc3/examples/assets/images/6254.jpg
--rw-r--r--   0        0        0    92833 2023-04-14 21:20:23.032568 furiosa-serving-0.9.0rc3/examples/assets/images/car.jpg
--rw-r--r--   0        0        0    10484 2023-04-14 21:20:23.032568 furiosa-serving-0.9.0rc3/examples/assets/labels/ImageNetLabels.txt
--rw-r--r--   0        0        0    18136 2023-04-14 21:20:23.032568 furiosa-serving-0.9.0rc3/examples/assets/models/MNISTnet_uint8_quant_without_softmax.tflite
--rw-r--r--   0        0        0  4275408 2023-04-14 21:20:23.060568 furiosa-serving-0.9.0rc3/examples/assets/models/image_classification.onnx
--rw-r--r--   0        0        0     1042 2023-04-14 21:20:23.060568 furiosa-serving-0.9.0rc3/examples/image_classify.py
--rw-r--r--   0        0        0     2842 2023-04-14 21:20:23.060568 furiosa-serving-0.9.0rc3/examples/number_classify.py
--rw-r--r--   0        0        0      346 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/__init__.py
--rw-r--r--   0        0        0     5960 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/application.py
--rw-r--r--   0        0        0        0 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/apps/__init__.py
--rw-r--r--   0        0        0      539 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/apps/health.py
--rw-r--r--   0        0        0     1088 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/apps/model.py
--rw-r--r--   0        0        0     1018 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/apps/repository.py
--rw-r--r--   0        0        0       17 2023-04-14 21:22:32.047400 furiosa-serving-0.9.0rc3/furiosa/serving/git_version.txt
--rw-r--r--   0        0        0     8907 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/model.py
--rw-r--r--   0        0        0       96 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/processors/__init__.py
--rw-r--r--   0        0        0     2962 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/processors/base.py
--rw-r--r--   0        0        0     2349 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/processors/imagenet.py
--rw-r--r--   0        0        0        0 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/py.typed
--rw-r--r--   0        0        0     6388 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/furiosa/serving/telemetry.py
--rw-r--r--   0        0        0     2882 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0      692 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/tests/test_load_models.py
--rw-r--r--   0        0        0     1087 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/tests/test_processors.py
--rw-r--r--   0        0        0      582 2023-04-14 21:20:23.064568 furiosa-serving-0.9.0rc3/tests/test_subapp.py
--rw-r--r--   0        0        0    13488 1970-01-01 00:00:00.000000 furiosa-serving-0.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 05:34:31.576838 furiosa_serving-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      378 2023-05-24 05:34:31.576838 furiosa_serving-0.9.1/Makefile
+-rw-r--r--   0        0        0    11731 2023-05-24 05:34:31.576838 furiosa_serving-0.9.1/README.md
+-rw-r--r--   0        0        0     2636 2023-05-24 05:34:31.576838 furiosa_serving-0.9.1/examples/assets/images/1234567890.jpg
+-rw-r--r--   0        0        0     1286 2023-05-24 05:34:31.576838 furiosa_serving-0.9.1/examples/assets/images/6254.jpg
+-rw-r--r--   0        0        0    92833 2023-05-24 05:34:31.580838 furiosa_serving-0.9.1/examples/assets/images/car.jpg
+-rw-r--r--   0        0        0    10484 2023-05-24 05:34:31.580838 furiosa_serving-0.9.1/examples/assets/labels/ImageNetLabels.txt
+-rw-r--r--   0        0        0    18136 2023-05-24 05:34:31.580838 furiosa_serving-0.9.1/examples/assets/models/MNISTnet_uint8_quant_without_softmax.tflite
+-rw-r--r--   0        0        0  4275408 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/examples/assets/models/image_classification.onnx
+-rw-r--r--   0        0        0     1042 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/examples/image_classify.py
+-rw-r--r--   0        0        0     2842 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/examples/number_classify.py
+-rw-r--r--   0        0        0      346 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/__init__.py
+-rw-r--r--   0        0        0     5960 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/application.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/apps/__init__.py
+-rw-r--r--   0        0        0      539 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/apps/health.py
+-rw-r--r--   0        0        0     1088 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/apps/model.py
+-rw-r--r--   0        0        0     1018 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/apps/repository.py
+-rw-r--r--   0        0        0       14 2023-05-24 05:37:29.983641 furiosa_serving-0.9.1/furiosa/serving/git_version.txt
+-rw-r--r--   0        0        0     8907 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/model.py
+-rw-r--r--   0        0        0       96 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/processors/__init__.py
+-rw-r--r--   0        0        0     2962 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/processors/base.py
+-rw-r--r--   0        0        0     2349 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/processors/imagenet.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/py.typed
+-rw-r--r--   0        0        0     6388 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/furiosa/serving/telemetry.py
+-rw-r--r--   0        0        0     2878 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      692 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/tests/test_load_models.py
+-rw-r--r--   0        0        0     1087 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/tests/test_processors.py
+-rw-r--r--   0        0        0      582 2023-05-24 05:34:31.612838 furiosa_serving-0.9.1/tests/test_subapp.py
+-rw-r--r--   0        0        0    13485 1970-01-01 00:00:00.000000 furiosa_serving-0.9.1/PKG-INFO
```

### Comparing `furiosa-serving-0.9.0rc3/README.md` & `furiosa_serving-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/examples/assets/images/1234567890.jpg` & `furiosa_serving-0.9.1/examples/assets/images/1234567890.jpg`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/examples/assets/images/6254.jpg` & `furiosa_serving-0.9.1/examples/assets/images/6254.jpg`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/examples/assets/images/car.jpg` & `furiosa_serving-0.9.1/examples/assets/images/car.jpg`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/examples/assets/labels/ImageNetLabels.txt` & `furiosa_serving-0.9.1/examples/assets/labels/ImageNetLabels.txt`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/examples/assets/models/MNISTnet_uint8_quant_without_softmax.tflite` & `furiosa_serving-0.9.1/examples/assets/models/MNISTnet_uint8_quant_without_softmax.tflite`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/examples/assets/models/image_classification.onnx` & `furiosa_serving-0.9.1/examples/assets/models/image_classification.onnx`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/examples/image_classify.py` & `furiosa_serving-0.9.1/examples/image_classify.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/examples/number_classify.py` & `furiosa_serving-0.9.1/examples/number_classify.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/furiosa/serving/application.py` & `furiosa_serving-0.9.1/furiosa/serving/application.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/furiosa/serving/apps/health.py` & `furiosa_serving-0.9.1/furiosa/serving/apps/health.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/furiosa/serving/apps/model.py` & `furiosa_serving-0.9.1/furiosa/serving/apps/model.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/furiosa/serving/apps/repository.py` & `furiosa_serving-0.9.1/furiosa/serving/apps/repository.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/furiosa/serving/model.py` & `furiosa_serving-0.9.1/furiosa/serving/model.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/furiosa/serving/processors/base.py` & `furiosa_serving-0.9.1/furiosa/serving/processors/base.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/furiosa/serving/processors/imagenet.py` & `furiosa_serving-0.9.1/furiosa/serving/processors/imagenet.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/furiosa/serving/telemetry.py` & `furiosa_serving-0.9.1/furiosa/serving/telemetry.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/pyproject.toml` & `furiosa_serving-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-serving"
-version = "0.9.0.rc3"
+version = "0.9.1"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Environment :: Web Environment",
```

### Comparing `furiosa-serving-0.9.0rc3/tests/test_load_models.py` & `furiosa_serving-0.9.1/tests/test_load_models.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/tests/test_processors.py` & `furiosa_serving-0.9.1/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/tests/test_subapp.py` & `furiosa_serving-0.9.1/tests/test_subapp.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.9.0rc3/PKG-INFO` & `furiosa_serving-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-serving
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: Furiosa serving framework, easy to use inference server.
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

