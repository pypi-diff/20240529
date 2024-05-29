# Comparing `tmp/pyannote-onnx-0.0.4.tar.gz` & `tmp/pyannote-onnx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyannote-onnx-0.0.4.tar", last modified: Thu Apr 25 15:35:33 2024, max compression
+gzip compressed data, was "pyannote-onnx-0.0.5.tar", last modified: Wed May 29 05:45:01 2024, max compression
```

## Comparing `pyannote-onnx-0.0.4.tar` & `pyannote-onnx-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:35:33.367649 pyannote-onnx-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 15:35:33.367649 pyannote-onnx-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:35:33.359649 pyannote-onnx-0.0.4/pyannote_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/inference_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/pyannote_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/segmentation-3.0.onnx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:35:33.367649 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:35:33.367649 pyannote-onnx-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:45:01.976285 pyannote-onnx-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 05:45:01.976285 pyannote-onnx-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:45:01.968285 pyannote-onnx-0.0.5/pyannote_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/pyannote_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx/segmentation-3.0.onnx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:45:01.976285 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/pyannote_onnx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 05:45:01.976285 pyannote-onnx-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 05:45:01.000000 pyannote-onnx-0.0.5/setup.py
```

### Comparing `pyannote-onnx-0.0.4/LICENSE` & `pyannote-onnx-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.4/PKG-INFO` & `pyannote-onnx-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyannote-onnx-0.0.4/README.md` & `pyannote-onnx-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.4/pyannote_onnx/__init__.py` & `pyannote-onnx-0.0.5/pyannote_onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.4/pyannote_onnx/cli.py` & `pyannote-onnx-0.0.5/pyannote_onnx/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
+import librosa
 import matplotlib.pyplot as plt
 import numpy as np
-import soundfile as sf
 
 from pyannote_onnx import PyannoteONNX
 
 
 @click.command()
 @click.argument("wav_path", type=click.Path(exists=True, file_okay=True))
 @click.option("--plot/--no-plot", default=False, help="Plot the vad probabilities")
@@ -36,15 +36,15 @@
 
     num_speakers = vad.get_num_speakers(
         wav_path, threshold=0.5, min_speech_duration_ms=100
     )
     print(num_speakers)
 
     if plot:
-        wav, sr = sf.read(wav_path, dtype="float32")
+        wav, sr = librosa.load(wav_path, sr=vad.sample_rate)
         x1 = np.arange(0, len(wav)) / sr
         outputs = [output for output in vad(wav)]
         x2 = [(i * 270 + 721) / sr for i in range(0, len(outputs))]
 
         plt.plot(x1, wav)
         plt.plot(x2, outputs)
         plt.show()
```

### Comparing `pyannote-onnx-0.0.4/pyannote_onnx/inference_session.py` & `pyannote-onnx-0.0.5/pyannote_onnx/inference_session.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.4/pyannote_onnx/pyannote_onnx.py` & `pyannote-onnx-0.0.5/pyannote_onnx/pyannote_onnx.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from itertools import permutations
 from pathlib import Path
 from typing import Union
 
 import librosa
 import numpy as np
 import soundfile as sf
+from tqdm import tqdm
 
 from .inference_session import PickableInferenceSession
 
 
 class PyannoteONNX:
     def __init__(self):
         # segmentation-3.0 classes:
@@ -90,20 +91,27 @@
             np.abs(np.sum(np.array(perms)[:, : x.shape[0], :] - x, axis=1)), axis=1
         )
         return perms[np.argmin(diffs)]
 
     def __call__(self, x, step=5.0, return_chunk=False):
         step = int(step * self.sample_rate)
         # step: [0.5 * duration, 0.9 * duration]
-        step = max(min(step, 0.9 * self.duration // 10), self.duration // 2)
+        step = max(min(step, 0.9 * self.duration), self.duration // 2)
         # overlap: [0.1 * duration, 0.5 * duration]
         overlap = self.sample2frame(self.duration - step)
         overlap_chunk = np.zeros((overlap, self.num_classes))
         windows = list(self.sliding_window(x, self.duration, step))
+        progress_bar = tqdm(
+            total=len(windows),
+            desc="Pyannote processing",
+            unit="frames",
+            bar_format="{l_bar}{bar}{r_bar} | {percentage:.2f}%",
+        )
         for idx, (window_size, window) in enumerate(windows):
+            progress_bar.update(1)
             ort_outs = np.exp(
                 self.session.run(None, {"input": window[None, None, :]})[0][0]
             )
             # https://herve.niderb.fr/fastpages/2022/10/23/One-speaker-segmentation-model-to-rule-them-all
             # reorder the speakers and aggregate
             ort_outs = np.concatenate(
                 (
@@ -147,17 +155,17 @@
             segment["end"] = int(segment["end"] * step)
 
         segment["start"] = max(segment["start"] - speech_pad_samples, 0)
         segment["end"] = min(segment["end"] + speech_pad_samples, len(wav))
         if save_path:
             wav = wav[segment["start"] : segment["end"]]
             if flat_layout:
-                sf.write(str(save_path) + f"_{idx:04d}.wav", wav, sample_rate)
+                sf.write(str(save_path) + f"_{idx:05d}.wav", wav, sample_rate)
             else:
-                sf.write(str(Path(save_path) / f"{idx:04d}.wav"), wav, sample_rate)
+                sf.write(str(Path(save_path) / f"{idx:05d}.wav"), wav, sample_rate)
         if return_seconds:
             segment["start"] = round(segment["start"] / sample_rate, 3)
             segment["end"] = round(segment["end"] / sample_rate, 3)
         return segment
 
     def get_speech_timestamps(
         self,
@@ -223,20 +231,21 @@
             sample_rate=sample_rate,
             save_path=save_path,
             flat_layout=flat_layout,
             speech_pad_samples=speech_pad_samples,
             return_seconds=return_seconds,
         )
 
+        dur_ms = len(wav) * 1000 / sr
         if len(wav.shape) > 1:
             raise ValueError(
                 "More than one dimension in audio."
                 "Are you trying to process audio with 2 channels?"
             )
-        if sr / len(wav) > 31.25:
+        if dur_ms < 32:
             raise ValueError("Input audio is too short.")
 
         min_speech_samples = sr * min_speech_duration_ms // 1000
         max_speech_samples = sr * max_speech_duration_s - 2 * speech_pad_samples
         min_silence_samples = sr * min_silence_duration_ms // 1000
         min_silence_samples_at_max_speech = sr * 98 // 1000
```

### Comparing `pyannote-onnx-0.0.4/pyannote_onnx/segmentation-3.0.onnx` & `pyannote-onnx-0.0.5/pyannote_onnx/segmentation-3.0.onnx`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.4/pyannote_onnx.egg-info/PKG-INFO` & `pyannote-onnx-0.0.5/pyannote_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyannote-onnx-0.0.4/setup.py` & `pyannote-onnx-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 from setuptools import setup, find_packages
 
 
 with open("requirements.txt", encoding="utf8") as f:
     requirements = f.readlines()
 
 setup(
```

