# Comparing `tmp/albucore-0.0.4.tar.gz` & `tmp/albucore-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albucore-0.0.4.tar", last modified: Sat May 18 00:36:35 2024, max compression
+gzip compressed data, was "albucore-0.0.5.tar", last modified: Wed May 29 02:06:01 2024, max compression
```

## Comparing `albucore-0.0.4.tar` & `albucore-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:36:35.343985 albucore-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-18 00:36:26.000000 albucore-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-18 00:36:35.343985 albucore-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 00:36:26.000000 albucore-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:36:35.339985 albucore-0.0.4/albucore/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 00:36:26.000000 albucore-0.0.4/albucore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-18 00:36:26.000000 albucore-0.0.4/albucore/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-18 00:36:26.000000 albucore-0.0.4/albucore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:36:35.343985 albucore-0.0.4/albucore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-18 00:36:26.000000 albucore-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:36:35.343985 albucore-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-18 00:36:26.000000 albucore-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:36:35.343985 albucore-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-05-18 00:36:26.000000 albucore-0.0.4/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-18 00:36:26.000000 albucore-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-29 02:06:01.606849 albucore-0.0.5/
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1075 2024-05-14 02:01:45.000000 albucore-0.0.5/LICENSE
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3059 2024-05-29 02:06:01.606586 albucore-0.0.5/PKG-INFO
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1349 2024-05-29 02:05:51.000000 albucore-0.0.5/README.md
+drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-29 02:06:01.604238 albucore-0.0.5/albucore/
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       48 2024-05-29 02:05:51.000000 albucore-0.0.5/albucore/__init__.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     4768 2024-05-29 02:05:51.000000 albucore-0.0.5/albucore/functions.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     5998 2024-05-29 02:05:51.000000 albucore-0.0.5/albucore/utils.py
+drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-29 02:06:01.606266 albucore-0.0.5/albucore.egg-info/
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3059 2024-05-29 02:06:01.000000 albucore-0.0.5/albucore.egg-info/PKG-INFO
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      353 2024-05-29 02:06:01.000000 albucore-0.0.5/albucore.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-05-29 02:06:01.000000 albucore-0.0.5/albucore.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-05-15 02:11:09.000000 albucore-0.0.5/albucore.egg-info/not-zip-safe
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       60 2024-05-29 02:06:01.000000 albucore-0.0.5/albucore.egg-info/requires.txt
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        9 2024-05-29 02:06:01.000000 albucore-0.0.5/albucore.egg-info/top_level.txt
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2611 2024-05-16 02:10:17.000000 albucore-0.0.5/pyproject.toml
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       38 2024-05-29 02:06:01.606898 albucore-0.0.5/setup.cfg
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3671 2024-05-28 22:32:30.000000 albucore-0.0.5/setup.py
+drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-29 02:06:01.605927 albucore-0.0.5/tests/
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     7068 2024-05-29 02:05:51.000000 albucore-0.0.5/tests/test_add.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    10449 2024-05-29 02:05:51.000000 albucore-0.0.5/tests/test_multiply.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2143 2024-05-29 02:05:51.000000 albucore-0.0.5/tests/test_utils.py
```

### Comparing `albucore-0.0.4/LICENSE` & `albucore-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `albucore-0.0.4/PKG-INFO` & `albucore-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albucore
-Version: 0.0.4
+Version: 0.0.5
 Summary: A high-performance image processing library designed to optimize and extend the Albumentations library with specialized functions for advanced image transformations. Perfect for developers working in computer vision who require efficient and scalable image augmentation.
 Home-page: https://github.com/albumentations-team/albucore
 Author: Vladimir I. Iglovikov
 License: MIT
 Keywords: Image Processing,Computer Vision,Image Augmentation,Albumentations,Optimization,Machine Learning,Deep Learning,Python Imaging,Data Augmentation,Performance,Efficiency,High-Performance,CV,OpenCV,Automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -66,28 +66,12 @@
 # Multiply by a vector
 multiplier = [1.5, 1.2, 0.9]  # Different multiplier for each channel
 multiplied_image = multiply(img, multiplier)
 ```
 
 ## Benchmarks
 
-### Benchmark Results for 1000 Images of `float32` Type (256, 256, 1)
-
-|                  | albucore     | opencv           | numpy            |
-| ---------------- | ------------ | ---------------- | ---------------- |
-| MultiplyConstant | 12925 ± 1237 | 10963 ± 1053     | **14040 ± 2063** |
-| MultiplyVector   | 3832 ± 512   | **10824 ± 1005** | 8986 ± 511       |
-
-### Benchmark Results for 1000 Images of `uint8` Type (256, 256, 1)
-
-|                  | albucore         | opencv      | numpy      |
-| ---------------- | ---------------- | ----------- | ---------- |
-| MultiplyConstant | **24131 ± 1129** | 11622 ± 175 | 6969 ± 643 |
-| MultiplyVector   | **24279 ± 908**  | 11756 ± 152 | 6936 ± 408 |
-
-Albucore provides significant performance improvements for image processing tasks. Here are some benchmark results comparing Albucore with OpenCV and Numpy:
-
-For more detailed benchmark results, including other configurations and data types, refer to the [Benchmark](benchmark/results/) in the repository.
+For detailed benchmark results, including other configurations and data types, refer to the [Benchmark](benchmark/results/) in the repository.
 
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `albucore-0.0.4/README.md` & `albucore-0.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -34,28 +34,12 @@
 # Multiply by a vector
 multiplier = [1.5, 1.2, 0.9]  # Different multiplier for each channel
 multiplied_image = multiply(img, multiplier)
 ```
 
 ## Benchmarks
 
-### Benchmark Results for 1000 Images of `float32` Type (256, 256, 1)
-
-|                  | albucore     | opencv           | numpy            |
-| ---------------- | ------------ | ---------------- | ---------------- |
-| MultiplyConstant | 12925 ± 1237 | 10963 ± 1053     | **14040 ± 2063** |
-| MultiplyVector   | 3832 ± 512   | **10824 ± 1005** | 8986 ± 511       |
-
-### Benchmark Results for 1000 Images of `uint8` Type (256, 256, 1)
-
-|                  | albucore         | opencv      | numpy      |
-| ---------------- | ---------------- | ----------- | ---------- |
-| MultiplyConstant | **24131 ± 1129** | 11622 ± 175 | 6969 ± 643 |
-| MultiplyVector   | **24279 ± 908**  | 11756 ± 152 | 6936 ± 408 |
-
-Albucore provides significant performance improvements for image processing tasks. Here are some benchmark results comparing Albucore with OpenCV and Numpy:
-
-For more detailed benchmark results, including other configurations and data types, refer to the [Benchmark](benchmark/results/) in the repository.
+For detailed benchmark results, including other configurations and data types, refer to the [Benchmark](benchmark/results/) in the repository.
 
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `albucore-0.0.4/albucore/utils.py` & `albucore-0.0.5/albucore/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import wraps
-from typing import Any, Callable, Union
+from typing import Any, Callable, Sequence, Union
 
 import cv2
 import numpy as np
 from typing_extensions import Concatenate, ParamSpec
 
 NUM_RGB_CHANNELS = 3
 MONO_CHANNEL_DIMENSIONS = 2
@@ -149,7 +149,34 @@
 
     @wraps(func)
     def wrapped_function(img: np.ndarray, *args: P.args, **kwargs: P.kwargs) -> np.ndarray:
         img = np.require(img, requirements=["C_CONTIGUOUS"])
         return func(img, *args, **kwargs)
 
     return wrapped_function
+
+
+def convert_value(value: Union[Sequence[float], np.ndarray, float], num_channels: int) -> Union[float, np.ndarray]:
+    """Convert a multiplier to a float / int or a numpy array.
+
+    If num_channels is 1 or the length of the multiplier less than num_channels, the multiplier is converted to a float.
+    If length of the multiplier is greater than num_channels, multiplier is truncated to num_channels.
+    """
+    if isinstance(value, (int, float)):
+        return value
+    if (
+        # Case 1: num_channels is 1 and multiplier is a list or tuple
+        (num_channels == 1 and (isinstance(value, Sequence) or (isinstance(value, np.ndarray) and value.ndim == 1)))
+        or
+        # Case 2: multiplier length is 1, regardless of num_channels
+        (isinstance(value, (Sequence, np.ndarray)) and len(value) == 1)
+        # Case 3: num_channels more then length of multiplier
+        or (num_channels > 1 and len(value) < num_channels)
+    ):
+        # Convert to a float
+        return float(value[0])
+
+    if isinstance(value, Sequence):
+        return np.array(value[:num_channels], dtype=np.float64)
+    if value.ndim == 1 and value.shape[0] > num_channels:
+        value = value[:num_channels]
+    return value
```

### Comparing `albucore-0.0.4/albucore.egg-info/PKG-INFO` & `albucore-0.0.5/albucore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albucore
-Version: 0.0.4
+Version: 0.0.5
 Summary: A high-performance image processing library designed to optimize and extend the Albumentations library with specialized functions for advanced image transformations. Perfect for developers working in computer vision who require efficient and scalable image augmentation.
 Home-page: https://github.com/albumentations-team/albucore
 Author: Vladimir I. Iglovikov
 License: MIT
 Keywords: Image Processing,Computer Vision,Image Augmentation,Albumentations,Optimization,Machine Learning,Deep Learning,Python Imaging,Data Augmentation,Performance,Efficiency,High-Performance,CV,OpenCV,Automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -66,28 +66,12 @@
 # Multiply by a vector
 multiplier = [1.5, 1.2, 0.9]  # Different multiplier for each channel
 multiplied_image = multiply(img, multiplier)
 ```
 
 ## Benchmarks
 
-### Benchmark Results for 1000 Images of `float32` Type (256, 256, 1)
-
-|                  | albucore     | opencv           | numpy            |
-| ---------------- | ------------ | ---------------- | ---------------- |
-| MultiplyConstant | 12925 ± 1237 | 10963 ± 1053     | **14040 ± 2063** |
-| MultiplyVector   | 3832 ± 512   | **10824 ± 1005** | 8986 ± 511       |
-
-### Benchmark Results for 1000 Images of `uint8` Type (256, 256, 1)
-
-|                  | albucore         | opencv      | numpy      |
-| ---------------- | ---------------- | ----------- | ---------- |
-| MultiplyConstant | **24131 ± 1129** | 11622 ± 175 | 6969 ± 643 |
-| MultiplyVector   | **24279 ± 908**  | 11756 ± 152 | 6936 ± 408 |
-
-Albucore provides significant performance improvements for image processing tasks. Here are some benchmark results comparing Albucore with OpenCV and Numpy:
-
-For more detailed benchmark results, including other configurations and data types, refer to the [Benchmark](benchmark/results/) in the repository.
+For detailed benchmark results, including other configurations and data types, refer to the [Benchmark](benchmark/results/) in the repository.
 
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `albucore-0.0.4/pyproject.toml` & `albucore-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `albucore-0.0.4/setup.py` & `albucore-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `albucore-0.0.4/tests/test_functions.py` & `albucore-0.0.5/tests/test_multiply.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,21 @@
-from typing import Sequence
 import pytest
 import numpy as np
 
 
 from albucore.utils import MAX_OPENCV_WORKING_CHANNELS, clip
 
 from albucore import (
     multiply_with_lut,
     multiply_with_numpy,
     multiply_with_opencv,
     multiply,
-    convert_multiplier,
+    convert_value,
 )
 
-@pytest.mark.parametrize(
-    "multiplier, num_channels, expected",
-    [
-        ((1.5), 1, 1.5),
-        (np.array([1.5]), 3, 1.5),
-        ([1.5], 2, 1.5),
-        ([1.5, 2.5], 1, 1.5),
-        ([1.5, 2.5, 0.5], 2, np.array([1.5, 2.5, 0.5], dtype=np.float32)),
-        ((1.5), 2, 1.5),
-    ]
-)
-def test_convert_multiplier(multiplier, num_channels, expected):
-    result = convert_multiplier(multiplier, num_channels)
-    if isinstance(expected, np.ndarray):
-        assert np.array_equal(result, expected)
-    else:
-         assert result == expected
 
 @pytest.mark.parametrize(
     "img, multiplier, expected_output",
     [
         # Test case 1: Multiplier as a float, image of type uint8
         (
             np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]], dtype=np.uint8),
@@ -152,38 +134,26 @@
         ),
         # Test case 2: Multiplier as a vector, image of type uint8
         (
             np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]], dtype=np.uint8),
             np.array([0.5, 1.5, 2.0], dtype=np.float32),
             np.array([[[0, 3, 6], [2, 7, 12]], [[3, 12, 18], [5, 16, 24]]], dtype=np.uint8),
         ),
-        # Test case 3: Multiplier as an array, image of type uint8
-        (
-            np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]], dtype=np.uint8),
-            np.array([[[1, 0.5, 0.25], [0.5, 1, 1.5]], [[1.5, 2, 0.5], [0.25, 0.75, 1]]], dtype=np.float32),
-            np.array([[[1, 1, 0], [2, 5, 9]], [[10, 16, 4], [2, 8, 12]]], dtype=np.uint8),
-        ),
         # Clipping effect test for uint8
         (
             np.array([[[100, 150, 200], [250, 255, 100]], [[50, 75, 125], [175, 200, 225]]], dtype=np.uint8),
             2.0,
             np.array([[[200, 255, 255], [255, 255, 200]], [[100, 150, 250], [255, 255, 255]]], dtype=np.uint8),
         ),
         # New test case 7: Multiplier as a vector, image of type uint8 with 4 channels
         (
             np.array([[[1, 2, 3, 4], [5, 6, 7, 8]], [[9, 10, 11, 12], [13, 14, 15, 16]]], dtype=np.uint8),
             np.array([0.5, 1.5, 2.0, 2.5], dtype=np.float32),
             np.array([[[0, 3, 6, 10], [2, 9, 14, 20]], [[4, 15, 22, 30], [6, 21, 30, 40]]], dtype=np.uint8),
         ),
-        # New test case 8: Multiplier as a vector, image of type float32 with 4 channels
-        (
-            np.array([[[0.1, 0.2, 0.3, 0.4], [0.5, 0.6, 0.7, 0.8]], [[0.9, 1.0, 1.1, 1.2], [1.3, 1.4, 1.5, 1.6]]], dtype=np.float32),
-            np.array([0.5, 1.5, 2.0, 2.5], dtype=np.float32),
-            np.array([[[0.05, 0.3, 0.6, 1.0], [0.25, 0.9, 1.0, 1.0]], [[0.45, 1.0, 1.0, 1.0], [0.65, 1.0, 1.0, 1.0]]], dtype=np.float32),
-        ),
         # Test case 1: Multiplier as a float, image of type uint8, shape (height, width)
         (
             np.array([[1, 2, 3], [4, 5, 6]], dtype=np.uint8),
             2.0,
             np.array([[2, 4, 6], [8, 10, 12]], dtype=np.uint8),
         ),
         # Test case 2: Multiplier as a float, image of type uint8, shape (height, width, 1)
@@ -191,49 +161,57 @@
             np.array([[[1], [2]], [[3], [4]]], dtype=np.uint8),
             2.0,
             np.array([[[2], [4]], [[6], [8]]], dtype=np.uint8),
         ),
     ],
 )
 def test_multiply_with_lut(img, multiplier, expected_output):
-    result_lut = multiply_with_numpy(img, multiplier)
+    result_lut = multiply_with_lut(img, multiplier)
     assert np.allclose(result_lut, expected_output, atol=1e-6)
 
 
 np.random.seed(0)
+
+
 @pytest.mark.parametrize("img_dtype", [np.uint8, np.float32])
 @pytest.mark.parametrize("num_channels", [1, 3, 5])
-@pytest.mark.parametrize("multiplier", [1.5, [1.5], (1.5), np.array([2.0, 1.0, 0.5, 1.5, 1.1], np.float32)])
+@pytest.mark.parametrize(
+    "multiplier",
+    [
+        1.5,
+        [1.5],
+        (1.5),
+        np.array([2.0, 1.0, 0.5, 1.5, 1.1], np.float32),
+        np.array([2.0, 1.0, 0.5, 1.5, 1.1, 2.0], np.float32),
+    ]
+)
 @pytest.mark.parametrize("is_contiguous", [True, False])
 def test_multiply(img_dtype, num_channels, multiplier, is_contiguous):
-    height, width = 2, 2
+    height, width = 9, 11
+
     if is_contiguous:
         if img_dtype == np.uint8:
             img = np.random.randint(0, 256, size=(height, width, num_channels), dtype=img_dtype)
         else:
             img = np.random.rand(height, width, num_channels).astype(img_dtype)
     else:
         if img_dtype == np.uint8:
             img = np.random.randint(0, 256, size=(num_channels, height, width), dtype=img_dtype).transpose(1, 2, 0)
         else:
             img = np.random.rand(num_channels, height, width).astype(img_dtype).transpose(1, 2, 0)
 
-
     original_image = img.copy()
 
-    if not isinstance(multiplier, float):
-        multiplier = multiplier[:num_channels]
-
-    processed_multiplier = convert_multiplier(multiplier, num_channels)
+    processed_multiplier = convert_value(multiplier, num_channels)
 
     result = multiply(img, multiplier)
 
     assert np.array_equal(img, original_image), "Input image was modified"
 
-    result_numpy = multiply_with_numpy(img, multiplier)
+    result_numpy = multiply_with_numpy(img, processed_multiplier)
 
     assert np.array_equal(img, original_image), "Input image was modified"
 
     assert np.allclose(result, result_numpy, atol=1e-6)
 
     if num_channels <= MAX_OPENCV_WORKING_CHANNELS and img.dtype == np.uint8:
         result_lut = clip(multiply_with_lut(img, processed_multiplier), img.dtype)
```

