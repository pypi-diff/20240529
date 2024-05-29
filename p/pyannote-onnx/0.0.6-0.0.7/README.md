# Comparing `tmp/pyannote-onnx-0.0.6.tar.gz` & `tmp/pyannote-onnx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyannote-onnx-0.0.6.tar", last modified: Wed May 29 09:09:08 2024, max compression
+gzip compressed data, was "pyannote-onnx-0.0.7.tar", last modified: Wed May 29 13:27:53 2024, max compression
```

## Comparing `pyannote-onnx-0.0.6.tar` & `pyannote-onnx-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:09:08.906635 pyannote-onnx-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 09:09:08.906635 pyannote-onnx-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:09:08.898635 pyannote-onnx-0.0.6/pyannote_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/inference_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/pyannote_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx/segmentation-3.0.onnx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:09:08.906635 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/pyannote_onnx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:09:08.906635 pyannote-onnx-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 09:09:08.000000 pyannote-onnx-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:27:53.742340 pyannote-onnx-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 13:27:53.742340 pyannote-onnx-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:27:53.734341 pyannote-onnx-0.0.7/pyannote_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/pyannote_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/segmentation-3.0.onnx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:27:53.742340 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:27:53.742340 pyannote-onnx-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/setup.py
```

### Comparing `pyannote-onnx-0.0.6/LICENSE` & `pyannote-onnx-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.6/PKG-INFO` & `pyannote-onnx-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyannote-onnx-0.0.6/README.md` & `pyannote-onnx-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.6/pyannote_onnx/__init__.py` & `pyannote-onnx-0.0.7/pyannote_onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.6/pyannote_onnx/cli.py` & `pyannote-onnx-0.0.7/pyannote_onnx/cli.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.6/pyannote_onnx/inference_session.py` & `pyannote-onnx-0.0.7/pyannote_onnx/inference_session.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.6/pyannote_onnx/pyannote_onnx.py` & `pyannote-onnx-0.0.7/pyannote_onnx/pyannote_onnx.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         #   7. {spk2, spk3}
         # only keep the first 4 classes
         #   1. {speech}
         #   2. {spk1}
         #   3. {spk2}
         #   4. {spk3}
         self.num_classes = 4
-        self.sample_rate = 16000
-        self.duration = 10 * self.sample_rate
+        self.vad_sr = 16000
+        self.duration = 10 * self.vad_sr
         onnx_model = f"{os.path.dirname(__file__)}/segmentation-3.0.onnx"
         self.session = PickableInferenceSession(onnx_model)
 
     @staticmethod
     def sample2frame(x):
         # Conv1d & MaxPool1d & SincNet:
         #   * https://pytorch.org/docs/stable/generated/torch.nn.Conv1d.html
@@ -89,15 +89,15 @@
         perms = [np.array(perm).T for perm in permutations(y.T)]
         diffs = np.sum(
             np.abs(np.sum(np.array(perms)[:, : x.shape[0], :] - x, axis=1)), axis=1
         )
         return perms[np.argmin(diffs)]
 
     def __call__(self, x, step=5.0, return_chunk=False):
-        step = int(step * self.sample_rate)
+        step = int(step * self.vad_sr)
         # step: [0.5 * duration, 0.9 * duration]
         step = max(min(step, 0.9 * self.duration), self.duration // 2)
         # overlap: [0.1 * duration, 0.5 * duration]
         overlap = self.sample2frame(self.duration - step)
         overlap_chunk = np.zeros((overlap, self.num_classes))
         windows = list(self.sliding_window(x, self.duration, step))
         progress_bar = tqdm(
@@ -145,22 +145,17 @@
         wav,
         sample_rate,
         save_path,
         flat_layout,
         speech_pad_samples,
         return_seconds,
     ):
-        step = sample_rate / self.sample_rate
-        if step != 1.0:
-            segment["start"] = int(segment["start"] * step)
-            segment["end"] = int(segment["end"] * step)
-
         segment["start"] = max(segment["start"] - speech_pad_samples, 0)
         segment["end"] = min(segment["end"] + speech_pad_samples, len(wav))
-        if save_path:
+        if save_path is not None:
             wav = wav[segment["start"] : segment["end"]]
             if flat_layout:
                 sf.write(str(save_path) + f"_{idx:05d}.wav", wav, sample_rate)
             else:
                 sf.write(str(Path(save_path) / f"{idx:05d}.wav"), wav, sample_rate)
         if return_seconds:
             segment["start"] = round(segment["start"] / sample_rate, 3)
@@ -171,16 +166,16 @@
         self,
         wav_path: Union[str, Path],
         save_path: Union[str, Path] = None,
         flat_layout: bool = True,
         threshold: float = 0.5,
         min_speech_duration_ms: int = 250,
         max_speech_duration_s: float = float("inf"),
-        min_silence_duration_ms: int = 100,
-        speech_pad_ms: int = 30,
+        min_silence_duration_ms: int = 200,
+        speech_pad_ms: int = 100,
         return_seconds: bool = False,
     ):
         """
         Splitting long audios into speech chunks using Pyannote ONNX
 
         Parameters
         ----------
@@ -198,75 +193,74 @@
             Final speech chunks shorter min_speech_duration_ms are thrown out
         max_speech_duration_s: int (default - inf)
             Maximum duration of speech chunks in seconds
             Chunks longer than max_speech_duration_s will be split at the timestamp
             of the last silence that lasts more than 98ms (if any), to prevent
             agressive cutting. Otherwise, they will be split aggressively just
             before max_speech_duration_s.
-        min_silence_duration_ms: int (default - 100 milliseconds)
+        min_silence_duration_ms: int (default - 200 milliseconds)
             In the end of each speech chunk wait for min_silence_duration_ms before
             separating it.
-        speech_pad_ms: int (default - 30 milliseconds)
+        speech_pad_ms: int (default - 100 milliseconds)
             Final speech chunks are padded by speech_pad_ms each side
         return_seconds: bool (default - False)
             whether return timestamps in seconds (default - samples)
 
         Returns
         ----------
         speeches: list of dicts
             list containing ends and beginnings of speech chunks (samples or seconds
             based on return_seconds)
         """
-        wav, sr = librosa.load(wav_path, sr=self.sample_rate)
+        sr = sf.info(wav_path).samplerate
         speech_pad_samples = sr * speech_pad_ms // 1000
+        min_speech_samples = sr * min_speech_duration_ms // 1000
+        max_speech_samples = sr * max_speech_duration_s - 2 * speech_pad_samples
+        min_silence_samples = sr * min_silence_duration_ms // 1000
+        min_silence_samples_at_max_speech = sr * 98 // 1000
 
-        sample_rate = sf.info(wav_path).samplerate
-        if sample_rate == self.sample_rate:
+        wav, _ = librosa.load(wav_path, sr=self.vad_sr)
+        if sr == self.vad_sr:
             original_wav = wav
         else:
             # load the wav with original sample rate for saving
             original_wav, _ = sf.read(wav_path)
         fn = partial(
             self.process_segment,
             wav=original_wav,
-            sample_rate=sample_rate,
+            sample_rate=sr,
             save_path=save_path,
             flat_layout=flat_layout,
             speech_pad_samples=speech_pad_samples,
             return_seconds=return_seconds,
         )
 
-        dur_ms = len(wav) * 1000 / sr
+        dur_ms = len(wav) * 1000 / self.vad_sr
         if len(wav.shape) > 1:
             raise ValueError(
                 "More than one dimension in audio."
                 "Are you trying to process audio with 2 channels?"
             )
         if dur_ms < 32:
             raise ValueError("Input audio is too short.")
 
-        min_speech_samples = sr * min_speech_duration_ms // 1000
-        max_speech_samples = sr * max_speech_duration_s - 2 * speech_pad_samples
-        min_silence_samples = sr * min_silence_duration_ms // 1000
-        min_silence_samples_at_max_speech = sr * 98 // 1000
-
         current_speech = {}
         neg_threshold = threshold - 0.15
         triggered = False
         # to save potential segment end (and tolerate some silence)
         temp_end = 0
         # to save potential segment limits in case of maximum segment size reached
         prev_end = 0
         next_start = 0
 
         idx = 0
-        current_samples = 721
+        current_samples = 721 * sr / self.vad_sr
         for outupt in self(wav):
             speech_prob = outupt[0]
-            current_samples += 270
+            current_samples += 270 * sr / self.vad_sr
             # current frame is speech
             if speech_prob >= threshold:
                 if temp_end > 0 and next_start < prev_end:
                     next_start = current_samples
                 temp_end = 0
                 if not triggered:
                     triggered = True
@@ -319,15 +313,15 @@
                         idx += 1
                     current_speech = {}
                     prev_end = 0
                     next_start = 0
                     temp_end = 0
                     triggered = False
 
-        num_samples = len(wav)
+        num_samples = len(original_wav)
         # deal with the last speech segment
         if (
             current_speech
             and num_samples - current_speech["start"] > min_speech_samples
         ):
             current_speech["end"] = num_samples
             yield fn(idx, current_speech)
@@ -337,25 +331,22 @@
         wav: Union[str, Path, np.ndarray],
         threshold: float = 0.5,
         min_speech_duration_ms: float = 100,
     ):
         """
         Get the max number of speakers
         """
-        if isinstance(wav, np.ndarray):
-            sr = self.sample_rate
-        else:
-            wav, sr = librosa.load(wav, sr=self.sample_rate)
+        wav, _ = librosa.load(wav, sr=self.vad_sr)
 
         if len(wav.shape) > 1:
             raise ValueError(
                 "More than one dimension in audio."
                 "Are you trying to process audio with 2 channels?"
             )
-        if sr / len(wav) > 31.25:
+        if self.vad_sr / len(wav) > 31.25:
             raise ValueError("Input audio is too short.")
 
         outputs = np.array(list(self(wav)))[:, 1 : self.num_classes]
         speech_frames = np.sum(outputs > threshold, axis=0)
-        speech_duration_ms = self.frame2sample(speech_frames) * 1000 / sr
+        speech_duration_ms = self.frame2sample(speech_frames) * 1000 / self.vad_sr
         num_speakers = np.sum(speech_duration_ms > min_speech_duration_ms)
         return num_speakers
```

### Comparing `pyannote-onnx-0.0.6/pyannote_onnx/segmentation-3.0.onnx` & `pyannote-onnx-0.0.7/pyannote_onnx/segmentation-3.0.onnx`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.6/pyannote_onnx.egg-info/PKG-INFO` & `pyannote-onnx-0.0.7/pyannote_onnx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyannote-onnx-0.0.6/setup.py` & `pyannote-onnx-0.0.7/setup.py`

 * *Files identical despite different names*

