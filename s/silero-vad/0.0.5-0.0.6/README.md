# Comparing `tmp/silero-vad-0.0.5.tar.gz` & `tmp/silero-vad-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silero-vad-0.0.5.tar", last modified: Tue May 28 03:21:33 2024, max compression
+gzip compressed data, was "silero-vad-0.0.6.tar", last modified: Wed May 29 08:25:15 2024, max compression
```

## Comparing `silero-vad-0.0.5.tar` & `silero-vad-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:21:33.566980 silero-vad-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 03:21:33.000000 silero-vad-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 03:21:33.000000 silero-vad-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-28 03:21:33.566980 silero-vad-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 03:21:33.000000 silero-vad-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 03:21:33.000000 silero-vad-0.0.5/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 03:21:33.000000 silero-vad-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 03:21:33.566980 silero-vad-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-28 03:21:33.000000 silero-vad-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:21:33.566980 silero-vad-0.0.5/silero_vad/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/frame_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/inference_session.py
--rw-r--r--   0 runner    (1001) docker     (127)  1807522 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/silero_vad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:21:33.566980 silero-vad-0.0.5/silero_vad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:25:15.334678 silero-vad-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 08:25:14.000000 silero-vad-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 08:25:14.000000 silero-vad-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-29 08:25:15.330678 silero-vad-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 08:25:14.000000 silero-vad-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 08:25:14.000000 silero-vad-0.0.6/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 08:25:14.000000 silero-vad-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:25:15.334678 silero-vad-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-29 08:25:14.000000 silero-vad-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:25:15.330678 silero-vad-0.0.6/silero_vad/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-29 08:25:14.000000 silero-vad-0.0.6/silero_vad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-29 08:25:14.000000 silero-vad-0.0.6/silero_vad/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-29 08:25:14.000000 silero-vad-0.0.6/silero_vad/frame_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 08:25:14.000000 silero-vad-0.0.6/silero_vad/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1807522 2024-05-29 08:25:14.000000 silero-vad-0.0.6/silero_vad/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-05-29 08:25:14.000000 silero-vad-0.0.6/silero_vad/silero_vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-29 08:25:14.000000 silero-vad-0.0.6/silero_vad/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:25:15.330678 silero-vad-0.0.6/silero_vad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-29 08:25:15.000000 silero-vad-0.0.6/silero_vad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-29 08:25:15.000000 silero-vad-0.0.6/silero_vad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:25:15.000000 silero-vad-0.0.6/silero_vad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 08:25:15.000000 silero-vad-0.0.6/silero_vad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 08:25:15.000000 silero-vad-0.0.6/silero_vad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 08:25:15.000000 silero-vad-0.0.6/silero_vad.egg-info/top_level.txt
```

### Comparing `silero-vad-0.0.5/LICENSE` & `silero-vad-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.5/PKG-INFO` & `silero-vad-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-vad
-Version: 0.0.5
+Version: 0.0.6
 Summary: Silero VAD
 Home-page: https://github.com/pengzhendong/silero-vad
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `silero-vad-0.0.5/setup.py` & `silero-vad-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.5/silero_vad/__init__.py` & `silero-vad-0.0.6/silero_vad/__init__.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.5/silero_vad/cli.py` & `silero-vad-0.0.6/silero_vad/cli.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.5/silero_vad/frame_queue.py` & `silero-vad-0.0.6/silero_vad/frame_queue.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.5/silero_vad/inference_session.py` & `silero-vad-0.0.6/silero_vad/inference_session.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.5/silero_vad/silero_vad.onnx` & `silero-vad-0.0.6/silero_vad/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.5/silero_vad/silero_vad.py` & `silero-vad-0.0.6/silero_vad/silero_vad.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,38 @@
 from .inference_session import PickableInferenceSession
 from .utils import get_energy
 
 
 class SileroVAD:
     def __init__(self, onnx_model=f"{os.path.dirname(__file__)}/silero_vad.onnx"):
         self.session = PickableInferenceSession(onnx_model)
-        self.reset_states()
         self.sample_rates = [8000, 16000]
+        self.reset_states()
+
+    @staticmethod
+    def init_states():
+        h = np.zeros((2, 1, 64)).astype(np.float32)
+        c = np.zeros((2, 1, 64)).astype(np.float32)
+        return h, c
 
     def reset_states(self):
-        self._h = np.zeros((2, 1, 64)).astype(np.float32)
-        self._c = np.zeros((2, 1, 64)).astype(np.float32)
+        self._h, self._c = self.init_states()
 
-    def __call__(self, x, sr: int):
+    def __call__(self, x, sr, h=None, c=None):
+        use_external_state = h is not None and c is not None
         ort_inputs = {
             "input": x[np.newaxis, :],
-            "h": self._h,
-            "c": self._c,
+            "h": h if use_external_state else self._h,
+            "c": c if use_external_state else self._c,
             "sr": np.array(sr, dtype=np.int64),
         }
-        ort_outs = self.session.run(None, ort_inputs)
-        out, self._h, self._c = ort_outs
+        out, h, c = self.session.run(None, ort_inputs)
+        if use_external_state:
+            return out, h, c
+        self._h, self._c = h, c
         return out
 
     @staticmethod
     def process_segment(
         idx,
         segment,
         wav,
@@ -173,28 +181,28 @@
 
         speech_pad_samples = speech_pad_ms * vad_sr // 1000
         min_silence_samples_at_max_speech = 98 * vad_sr // 1000
         min_speech_samples = min_speech_duration_ms * vad_sr // 1000
         min_silence_samples = min_silence_duration_ms * vad_sr // 1000
         max_speech_duration_samples = max_speech_duration_s * vad_sr
         max_speech_samples = max_speech_duration_samples - 2 * speech_pad_samples
-        self.reset_states()
+        h, c = self.init_states()
 
         idx = 0
         current_speech = {}
         neg_threshold = threshold - 0.15
         triggered = False
         # to save potential segment end (and tolerate some silence)
         temp_end = 0
         # to save potential segment limits in case of maximum segment size reached
         prev_end = 0
         next_start = 0
         for frame_start, frame_end, frame in queue.add_chunk(wav, True):
             progress_bar.update(1)
-            speech_prob = self(frame, vad_sr)
+            speech_prob, h, c = self(frame, vad_sr, h, c)
             # current frame is speech
             if speech_prob >= threshold:
                 if temp_end > 0 and next_start < prev_end:
                     next_start = frame_end
                 temp_end = 0
                 if not triggered:
                     triggered = True
```

### Comparing `silero-vad-0.0.5/silero_vad/utils.py` & `silero-vad-0.0.6/silero_vad/utils.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.5/silero_vad.egg-info/PKG-INFO` & `silero-vad-0.0.6/silero_vad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-vad
-Version: 0.0.5
+Version: 0.0.6
 Summary: Silero VAD
 Home-page: https://github.com/pengzhendong/silero-vad
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

