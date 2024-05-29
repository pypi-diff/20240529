# Comparing `tmp/pyannote-onnx-0.0.5.tar.gz` & `tmp/pyannote-onnx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyannote-onnx-0.0.5.tar", last modified: Wed May 29 05:45:01 2024, max compression
+gzip compressed data, was "pyannote-onnx-0.0.6.tar", last modified: Wed May 29 09:09:08 2024, max compression
```

## Comparing `pyannote-onnx-0.0.5.tar` & `pyannote-onnx-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:45:01.976285 pyannote-onnx-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 05:45:01.976285 pyannote-onnx-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:45:01.968285 pyannote-onnx-0.0.5/pyannote_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/inference_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/pyannote_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/segmentation-3.0.onnx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:45:01.976285 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 05:45:01.976285 pyannote-onnx-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:09:08.906635 pyannote-onnx-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 09:09:08.906635 pyannote-onnx-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:09:08.898635 pyannote-onnx-0.0.6/pyannote_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/pyannote_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/segmentation-3.0.onnx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:09:08.906635 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:09:08.906635 pyannote-onnx-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/setup.py
```

### Comparing `pyannote-onnx-0.0.5/LICENSE` & `pyannote-onnx-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.5/PKG-INFO` & `pyannote-onnx-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyannote-onnx-0.0.5/README.md` & `pyannote-onnx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.5/pyannote_onnx/__init__.py` & `pyannote-onnx-0.0.6/pyannote_onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.5/pyannote_onnx/cli.py` & `pyannote-onnx-0.0.6/pyannote_onnx/cli.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.5/pyannote_onnx/inference_session.py` & `pyannote-onnx-0.0.6/pyannote_onnx/inference_session.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.5/pyannote_onnx/pyannote_onnx.py` & `pyannote-onnx-0.0.6/pyannote_onnx/pyannote_onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,22 +330,26 @@
             and num_samples - current_speech["start"] > min_speech_samples
         ):
             current_speech["end"] = num_samples
             yield fn(idx, current_speech)
 
     def get_num_speakers(
         self,
-        wav_path: Union[str, Path],
+        wav: Union[str, Path, np.ndarray],
         threshold: float = 0.5,
         min_speech_duration_ms: float = 100,
     ):
         """
         Get the max number of speakers
         """
-        wav, sr = librosa.load(wav_path, sr=self.sample_rate)
+        if isinstance(wav, np.ndarray):
+            sr = self.sample_rate
+        else:
+            wav, sr = librosa.load(wav, sr=self.sample_rate)
+
         if len(wav.shape) > 1:
             raise ValueError(
                 "More than one dimension in audio."
                 "Are you trying to process audio with 2 channels?"
             )
         if sr / len(wav) > 31.25:
             raise ValueError("Input audio is too short.")
```

### Comparing `pyannote-onnx-0.0.5/pyannote_onnx/segmentation-3.0.onnx` & `pyannote-onnx-0.0.6/pyannote_onnx/segmentation-3.0.onnx`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.5/pyannote_onnx.egg-info/PKG-INFO` & `pyannote-onnx-0.0.6/pyannote_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyannote-onnx-0.0.5/setup.py` & `pyannote-onnx-0.0.6/setup.py`

 * *Files identical despite different names*

