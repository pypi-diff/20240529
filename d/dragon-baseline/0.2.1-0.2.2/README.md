# Comparing `tmp/dragon_baseline-0.2.1.tar.gz` & `tmp/dragon_baseline-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragon_baseline-0.2.1.tar", last modified: Wed May  8 12:37:53 2024, max compression
+gzip compressed data, was "dragon_baseline-0.2.2.tar", last modified: Wed May 29 08:30:03 2024, max compression
```

## Comparing `dragon_baseline-0.2.1.tar` & `dragon_baseline-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.329367 dragon_baseline-0.2.1/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2023-10-10 15:36:12.000000 dragon_baseline-0.2.1/LICENSE
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1428 2024-05-08 12:37:53.329284 dragon_baseline-0.2.1/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)      136 2024-05-08 11:38:49.000000 dragon_baseline-0.2.1/README.md
--rw-r--r--   0 joeranbosma   (501) staff       (20)      504 2023-11-02 16:39:08.000000 dragon_baseline-0.2.1/pyproject.toml
--rw-r--r--   0 joeranbosma   (501) staff       (20)      879 2024-05-08 12:37:53.329818 dragon_baseline-0.2.1/setup.cfg
--rw-r--r--   0 joeranbosma   (501) staff       (20)      736 2024-05-08 11:41:02.000000 dragon_baseline-0.2.1/setup.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.321778 dragon_baseline-0.2.1/src/
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.325708 dragon_baseline-0.2.1/src/dragon_baseline/
--rw-r--r--   0 joeranbosma   (501) staff       (20)       85 2023-11-13 10:46:15.000000 dragon_baseline-0.2.1/src/dragon_baseline/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1346 2024-03-05 15:10:45.000000 dragon_baseline-0.2.1/src/dragon_baseline/__main__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.328268 dragon_baseline-0.2.1/src/dragon_baseline/architectures/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-11-13 10:43:50.000000 dragon_baseline-0.2.1/src/dragon_baseline/architectures/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     6028 2024-05-08 12:32:22.000000 dragon_baseline-0.2.1/src/dragon_baseline/architectures/clf_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7565 2024-05-08 12:32:27.000000 dragon_baseline-0.2.1/src/dragon_baseline/architectures/ner_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5823 2024-05-08 12:32:09.000000 dragon_baseline-0.2.1/src/dragon_baseline/architectures/reg_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    32960 2024-05-08 12:33:21.000000 dragon_baseline-0.2.1/src/dragon_baseline/main.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    18567 2024-03-05 15:10:45.000000 dragon_baseline-0.2.1/src/dragon_baseline/nlp_algorithm.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    34016 2023-11-02 16:39:08.000000 dragon_baseline-0.2.1/src/dragon_baseline/run_classification.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    35990 2023-11-02 16:39:08.000000 dragon_baseline-0.2.1/src/dragon_baseline/run_classification_multi_label.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    29174 2024-05-08 11:34:55.000000 dragon_baseline-0.2.1/src/dragon_baseline/run_ner.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.328470 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1428 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)      765 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/SOURCES.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/dependency_links.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-11-13 11:58:50.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/not-zip-safe
--rw-r--r--   0 joeranbosma   (501) staff       (20)      177 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/requires.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)       16 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/top_level.txt
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-29 08:30:03.366521 dragon_baseline-0.2.2/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2023-10-10 15:36:12.000000 dragon_baseline-0.2.2/LICENSE
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     6917 2024-05-29 08:30:03.366442 dragon_baseline-0.2.2/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5625 2024-05-29 07:51:12.000000 dragon_baseline-0.2.2/README.md
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      504 2023-11-02 16:39:08.000000 dragon_baseline-0.2.2/pyproject.toml
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      879 2024-05-29 08:30:03.366826 dragon_baseline-0.2.2/setup.cfg
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      736 2024-05-29 08:26:31.000000 dragon_baseline-0.2.2/setup.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-29 08:30:03.361364 dragon_baseline-0.2.2/src/
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-29 08:30:03.363733 dragon_baseline-0.2.2/src/dragon_baseline/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       85 2023-11-13 10:46:15.000000 dragon_baseline-0.2.2/src/dragon_baseline/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1346 2024-03-05 15:10:45.000000 dragon_baseline-0.2.2/src/dragon_baseline/__main__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-29 08:30:03.365446 dragon_baseline-0.2.2/src/dragon_baseline/architectures/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-11-13 10:43:50.000000 dragon_baseline-0.2.2/src/dragon_baseline/architectures/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     6028 2024-05-29 08:26:31.000000 dragon_baseline-0.2.2/src/dragon_baseline/architectures/clf_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7565 2024-05-29 08:26:31.000000 dragon_baseline-0.2.2/src/dragon_baseline/architectures/ner_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5823 2024-05-29 08:26:31.000000 dragon_baseline-0.2.2/src/dragon_baseline/architectures/reg_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    32900 2024-05-29 08:26:31.000000 dragon_baseline-0.2.2/src/dragon_baseline/main.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    18567 2024-03-05 15:10:45.000000 dragon_baseline-0.2.2/src/dragon_baseline/nlp_algorithm.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    34016 2023-11-02 16:39:08.000000 dragon_baseline-0.2.2/src/dragon_baseline/run_classification.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    35990 2023-11-02 16:39:08.000000 dragon_baseline-0.2.2/src/dragon_baseline/run_classification_multi_label.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    29174 2024-05-29 08:26:31.000000 dragon_baseline-0.2.2/src/dragon_baseline/run_ner.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-29 08:30:03.365700 dragon_baseline-0.2.2/src/dragon_baseline.egg-info/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     6917 2024-05-29 08:30:03.000000 dragon_baseline-0.2.2/src/dragon_baseline.egg-info/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      765 2024-05-29 08:30:03.000000 dragon_baseline-0.2.2/src/dragon_baseline.egg-info/SOURCES.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2024-05-29 08:30:03.000000 dragon_baseline-0.2.2/src/dragon_baseline.egg-info/dependency_links.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-11-13 11:58:50.000000 dragon_baseline-0.2.2/src/dragon_baseline.egg-info/not-zip-safe
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      177 2024-05-29 08:30:03.000000 dragon_baseline-0.2.2/src/dragon_baseline.egg-info/requires.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       16 2024-05-29 08:30:03.000000 dragon_baseline-0.2.2/src/dragon_baseline.egg-info/top_level.txt
```

### Comparing `dragon_baseline-0.2.1/LICENSE` & `dragon_baseline-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/setup.cfg` & `dragon_baseline-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/setup.py` & `dragon_baseline-0.2.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 if __name__ == "__main__":
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
-        version="0.2.1",
+        version="0.2.2",
         author_email="Joeran.Bosma@radboudumc.nl",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/DIAGNijmegen/dragon_baseline",
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/dragon_baseline/issues"
         },
```

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/__main__.py` & `dragon_baseline-0.2.2/src/dragon_baseline/__main__.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/architectures/__init__.py` & `dragon_baseline-0.2.2/src/dragon_baseline/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/architectures/clf_multi_head.py` & `dragon_baseline-0.2.2/src/dragon_baseline/architectures/clf_multi_head.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/architectures/ner_multi_head.py` & `dragon_baseline-0.2.2/src/dragon_baseline/architectures/ner_multi_head.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/architectures/reg_multi_head.py` & `dragon_baseline-0.2.2/src/dragon_baseline/architectures/reg_multi_head.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/main.py` & `dragon_baseline-0.2.2/src/dragon_baseline/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import re
 import subprocess
 from pathlib import Path
-from typing import List
+from typing import List, Union
 
 import numpy as np
 import pandas as pd
 import torch
 from scipy.special import expit, softmax
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import StandardScaler
@@ -171,28 +171,28 @@
         # select a random subset of samples without an entity
         df = pd.concat([df[mask], df[~mask].sample(n=mask.sum(), random_state=seed)], ignore_index=True)
 
     return df
 
 
 class DragonBaseline(NLPAlgorithm):
-    def __init__(self, input_path: Path = Path("/input"), output_path: Path = Path("/output"), workdir: Path = Path("/opt/app"), models_dir: Path = Path("/opt/app/models"), **kwargs):
+    def __init__(self, input_path: Path = Path("/input"), output_path: Path = Path("/output"), workdir: Path = Path("/opt/app"), model_name: Union[str, Path] = "distilbert-base-multilingual-cased", **kwargs):
         """
         Baseline implementation for the DRAGON Challenge (https://dragon.grand-challenge.org/).
         This baseline uses the HuggingFace Transformers library (https://huggingface.co/transformers/).
 
         The baseline must implement the following methods:
         - `preprocess`: preprocess the data
         - `train`: train the model
         - `predict`: predict the labels for the test data
         """
         super().__init__(input_path=input_path, output_path=output_path, **kwargs)
 
         # default training settings
-        self.model_name = models_dir / "distilbert-base-multilingual-cased"
+        self.model_name = model_name
         self.per_device_train_batch_size = 4
         self.gradient_accumulation_steps = 2
         self.gradient_checkpointing = False
         self.max_seq_length = 512
         self.learning_rate = 3e-5
         self.num_train_epochs = 5
         self.warmup_ratio = 0.1
@@ -669,9 +669,8 @@
         "Task108_Example_sl_ner-fold0",
         "Task109_Example_ml_ner-fold0",
     ]:
         DragonBaseline(
             input_path=Path(f"test-input/{job_name}"),
             output_path=Path(f"test-output/{job_name}"),
             workdir=Path(f"test-workdir/{job_name}"),
-            models_dir=Path(f"test-workdir/models"),
         ).process()
```

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/nlp_algorithm.py` & `dragon_baseline-0.2.2/src/dragon_baseline/nlp_algorithm.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/run_classification.py` & `dragon_baseline-0.2.2/src/dragon_baseline/run_classification.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/run_classification_multi_label.py` & `dragon_baseline-0.2.2/src/dragon_baseline/run_classification_multi_label.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline/run_ner.py` & `dragon_baseline-0.2.2/src/dragon_baseline/run_ner.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.1/src/dragon_baseline.egg-info/SOURCES.txt` & `dragon_baseline-0.2.2/src/dragon_baseline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

