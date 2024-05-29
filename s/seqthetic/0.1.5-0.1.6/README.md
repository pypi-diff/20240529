# Comparing `tmp/seqthetic-0.1.5.tar.gz` & `tmp/seqthetic-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqthetic-0.1.5.tar", max compression
+gzip compressed data, was "seqthetic-0.1.6.tar", max compression
```

## Comparing `seqthetic-0.1.5.tar` & `seqthetic-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      741 2024-05-23 06:57:29.435818 seqthetic-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    12058 2024-05-14 07:00:49.209241 seqthetic-0.1.5/readme.md
--rw-r--r--   0        0        0      216 2024-05-23 06:48:22.854947 seqthetic-0.1.5/seqthetic/__init__.py
--rw-r--r--   0        0        0     2934 2024-05-23 06:44:17.166835 seqthetic-0.1.5/seqthetic/dataset.py
--rw-r--r--   0        0        0      562 2024-05-14 04:17:11.407174 seqthetic-0.1.5/seqthetic/dependencies/__init__.py
--rw-r--r--   0        0        0      883 2024-05-14 03:57:53.546887 seqthetic-0.1.5/seqthetic/dependencies/adapter.py
--rw-r--r--   0        0        0     1795 2024-05-14 04:32:16.874428 seqthetic-0.1.5/seqthetic/dependencies/base.py
--rw-r--r--   0        0        0     2538 2024-05-23 06:55:56.027722 seqthetic-0.1.5/seqthetic/dependencies/fbm.py
--rw-r--r--   0        0        0     1882 2024-05-07 07:27:35.421846 seqthetic-0.1.5/seqthetic/dependencies/function.py
--rw-r--r--   0        0        0     1500 2024-05-07 07:27:35.425272 seqthetic-0.1.5/seqthetic/dependencies/random.py
--rw-r--r--   0        0        0     2798 2024-05-07 07:27:35.369313 seqthetic-0.1.5/seqthetic/mapping.py
--rw-r--r--   0        0        0     1305 2024-05-08 11:53:41.162062 seqthetic-0.1.5/seqthetic/range.py
--rw-r--r--   0        0        0     1246 2024-05-15 02:19:29.918718 seqthetic-0.1.5/seqthetic/seed.py
--rw-r--r--   0        0        0     4075 2024-05-09 06:40:31.603486 seqthetic-0.1.5/seqthetic/spec_variation.py
--rw-r--r--   0        0        0     5704 2024-05-15 02:55:53.636248 seqthetic-0.1.5/seqthetic/synthesis_spec.py
--rw-r--r--   0        0        0     3647 2024-05-15 02:51:58.490011 seqthetic-0.1.5/seqthetic/synthesizer.py
--rw-r--r--   0        0        0     1349 2024-05-09 06:38:18.422069 seqthetic-0.1.5/seqthetic/utils.py
--rw-r--r--   0        0        0        0 2024-05-07 12:03:34.624527 seqthetic-0.1.5/seqthetic/vary/__init__.py
--rw-r--r--   0        0        0      709 2024-05-09 04:33:48.215716 seqthetic-0.1.5/seqthetic/vary/compose_ops.py
--rw-r--r--   0        0        0     1475 2024-05-07 16:38:49.316467 seqthetic-0.1.5/seqthetic/vary/compute_ops.py
--rw-r--r--   0        0        0     1232 2024-05-08 12:19:45.887199 seqthetic-0.1.5/seqthetic/vary/domain_ops.py
--rw-r--r--   0        0        0     5426 2024-05-14 04:32:16.874428 seqthetic-0.1.5/seqthetic/vary/transform.py
--rw-r--r--   0        0        0      954 2024-05-08 03:02:01.961163 seqthetic-0.1.5/seqthetic/vary/variation.py
--rw-r--r--   0        0        0     4102 2024-05-14 04:41:06.866213 seqthetic-0.1.5/seqthetic/vary/variator.py
--rw-r--r--   0        0        0     4526 2024-05-15 03:27:39.863802 seqthetic-0.1.5/seqthetic/vocabulary.py
--rw-r--r--   0        0        0    12500 1970-01-01 00:00:00.000000 seqthetic-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      833 2024-05-29 15:23:35.155801 seqthetic-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    12090 2024-05-29 02:46:09.325438 seqthetic-0.1.6/README.md
+-rw-r--r--   0        0        0      216 2024-05-23 06:48:22.854947 seqthetic-0.1.6/seqthetic/__init__.py
+-rw-r--r--   0        0        0     3010 2024-05-29 02:51:18.694141 seqthetic-0.1.6/seqthetic/dataset.py
+-rw-r--r--   0        0        0      562 2024-05-14 04:17:11.407174 seqthetic-0.1.6/seqthetic/dependencies/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-14 03:57:53.546887 seqthetic-0.1.6/seqthetic/dependencies/adapter.py
+-rw-r--r--   0        0        0     1828 2024-05-29 08:30:20.211236 seqthetic-0.1.6/seqthetic/dependencies/base.py
+-rw-r--r--   0        0        0     5148 2024-05-29 08:35:28.974698 seqthetic-0.1.6/seqthetic/dependencies/fbm.py
+-rw-r--r--   0        0        0     1902 2024-05-29 02:56:30.039379 seqthetic-0.1.6/seqthetic/dependencies/function.py
+-rw-r--r--   0        0        0     1500 2024-05-07 07:27:35.425272 seqthetic-0.1.6/seqthetic/dependencies/random.py
+-rw-r--r--   0        0        0     4752 2024-05-29 14:55:15.076762 seqthetic-0.1.6/seqthetic/mapping.py
+-rw-r--r--   0        0        0     1466 2024-05-29 08:17:43.186910 seqthetic-0.1.6/seqthetic/range.py
+-rw-r--r--   0        0        0     1246 2024-05-15 02:19:29.918718 seqthetic-0.1.6/seqthetic/seed.py
+-rw-r--r--   0        0        0     4075 2024-05-09 06:40:31.603486 seqthetic-0.1.6/seqthetic/spec_variation.py
+-rw-r--r--   0        0        0     5724 2024-05-29 02:46:09.329805 seqthetic-0.1.6/seqthetic/synthesis_spec.py
+-rw-r--r--   0        0        0     7171 2024-05-29 15:22:46.630251 seqthetic-0.1.6/seqthetic/synthesizer.py
+-rw-r--r--   0        0        0     1349 2024-05-09 06:38:18.422069 seqthetic-0.1.6/seqthetic/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 12:03:34.624527 seqthetic-0.1.6/seqthetic/vary/__init__.py
+-rw-r--r--   0        0        0      709 2024-05-09 04:33:48.215716 seqthetic-0.1.6/seqthetic/vary/compose_ops.py
+-rw-r--r--   0        0        0     1475 2024-05-07 16:38:49.316467 seqthetic-0.1.6/seqthetic/vary/compute_ops.py
+-rw-r--r--   0        0        0     1232 2024-05-08 12:19:45.887199 seqthetic-0.1.6/seqthetic/vary/domain_ops.py
+-rw-r--r--   0        0        0     5426 2024-05-14 04:32:16.874428 seqthetic-0.1.6/seqthetic/vary/transform.py
+-rw-r--r--   0        0        0      954 2024-05-08 03:02:01.961163 seqthetic-0.1.6/seqthetic/vary/variation.py
+-rw-r--r--   0        0        0     4102 2024-05-14 04:41:06.866213 seqthetic-0.1.6/seqthetic/vary/variator.py
+-rw-r--r--   0        0        0     4526 2024-05-15 03:27:39.863802 seqthetic-0.1.6/seqthetic/vocabulary.py
+-rw-r--r--   0        0        0    12700 1970-01-01 00:00:00.000000 seqthetic-0.1.6/PKG-INFO
```

### Comparing `seqthetic-0.1.5/pyproject.toml` & `seqthetic-0.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqthetic"
-version = "0.1.5"
+version = "0.1.6"
 description = "Creates sequence data for pretraining and benchmarking sequence models"
 authors = ["Shom <shaomi_lin@126.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
@@ -16,14 +16,18 @@
 numpy = "^1.26.4"
 pydantic = "^2.7.0"
 nanoid = "^2.0.0"
 stochastic = "^0.7.0"
 jupyter = "^1.0.0"
 plotly = "^5.21.0"
 flake8 = "^7.0.0"
+more-itertools = "^10.2.0"
+dill = "^0.3.8"
+joblib = "^1.4.2"
+joblib-progress = "^1.0.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 isort = "^5.13.2"
 devtools = "^0.12.2"
 snakeviz = "^2.2.0"
```

### Comparing `seqthetic-0.1.5/readme.md` & `seqthetic-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 Features:
 1. **Diversity**: Supports generating data following various patterns including fractional Brownian Motion(fbm), [LIME](https://arxiv.org/pdf/2101.06223)(TODO), [TILT](https://arxiv.org/abs/2004.14601)(TODO) and [synthetic pretraining tasks](https://arxiv.org/abs/2206.10139) etc.
 2. **Spec-Driven**: Everything about the dataset is described by a spec, which helps with documenting each ablation and high-level manipulation. 
 3. **Reproducibility**: Processes involving randomness have their seeds recorded in the spec file. This means you can transfer the dataset by only 
 
 ## Installation 
 
+```
+pip install -e .
+
+```
 ## Usage
 
 ### Generation
 To generate a synthetic dataset, just write a spec and use synthesizer to make the dataset. For details on spec, please see [Concepts](#concepts):
 ```python
 # write the spec 
 spec = SynthesisSpec(...)
@@ -222,8 +226,8 @@
     - [ ] loglinear
     - [ ] corpus vocab
     - [ ] domain vocab 
     - [ ] **evolution**
 - [ ] mapping
     - [ ] **multiple**
     - [ ] **clip**
-- dataloader related?
+- dataloader related?
```

### Comparing `seqthetic-0.1.5/seqthetic/dataset.py` & `seqthetic-0.1.6/seqthetic/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,18 @@
     def __init__(self, spec: SynthesisSpec, df: pd.DataFrame):
         self.spec = spec
         self.df = df
 
     def save(self, path: str, format="csv"):
         if format == "csv":
             spec_path = self.spec.save(path)
-            save_name = self.spec.id
+            save_name = self.spec.name or self.spec.id
 
             dataset_path = Path(path) / f"{save_name}.csv"
+            print(f"Save the dataset to {dataset_path}")
             self.df["metadata"] = self.df["metadata"].apply(json.dumps)
             self.df.to_csv(dataset_path, index=False)
             return SavePath(spec_path=spec_path, dataset_path=str(dataset_path))
         else:
             raise NotImplementedError("Only csv format is supported")
 
     def view_dependencies(self, n=1):
```

### Comparing `seqthetic-0.1.5/seqthetic/dependencies/__init__.py` & `seqthetic-0.1.6/seqthetic/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/dependencies/adapter.py` & `seqthetic-0.1.6/seqthetic/dependencies/adapter.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/dependencies/base.py` & `seqthetic-0.1.6/seqthetic/dependencies/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,31 @@
     dependencies: List[np.ndarray]
     metadata: List[dict]
 
 
 class BaseDependency(BaseModel, ABC):
     generator: str = ""
     # fields in metadata field in dataset
-    metadata_schema: List[str] = Field(default_factory=list, exclude=True)
+    metadata_schema: List[str] = Field(
+        default_factory=lambda: ["sequence_length"], exclude=True
+    )
     base_seed_schema: List[str] = Field(
         default_factory=lambda: ["sequence_length"], exclude=True
     )
     custom_seed_schema: List[str] = Field(default_factory=list, exclude=True)
     sequence_length: FlexibleRange
     seed: Seed = Field(default_factory=Seed, exclude=True)
 
     @property
     def seed_schema(self) -> list[str]:
         return self.base_seed_schema + self.custom_seed_schema
 
     def init_seed(self):
         self.seed = Seed(seed_schema=self.seed_schema)
-        
+
     @model_validator(mode="after")
     def must_rewrite_generator(self):
         if not self.generator:
             raise ValueError("Please fill generator with proper value")
         return self
 
     @model_validator(mode="after")
@@ -50,8 +52,8 @@
 
     @abstractmethod
     def make_dependency(self, num_sequence: int) -> DependencyResult:
         pass
 
 
 def SchemaList(fields: list[str]):
-    return Field(default_factory=lambda: fields.copy(), exclude=True)
+    return Field(default_factory=lambda: fields.copy(), exclude=True)
```

### Comparing `seqthetic-0.1.5/seqthetic/dependencies/fbm.py` & `seqthetic-0.1.6/seqthetic/dependencies/function.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,49 @@
 from typing import List
 
+import numpy as np
 from pydantic import Field
-from stochastic.processes.continuous import FractionalBrownianMotion
 
-from seqthetic.dependencies.base import BaseDependency, DependencyResult, SchemaList
+from seqthetic.dependencies.base import (BaseDependency, DependencyResult,
+                                         SchemaList)
 from seqthetic.range import FlexibleRange
 from seqthetic.utils import make_digitizer
 
 
-class FBMDependency(BaseDependency):
-    """
-    Dependency from discretized fractional brownian motion(fBm).
-
-    Attributes:
-        hurst: Hurst exponent for the fbm
-        discretize_ratio: ratio for discretizing: binning into round(length * binning_ratio) bins. range (0, 1]
-        sequence_vocab_size: size of the vocabulary for each sequence
-    """
-
-    generator: str = "fbm"
-
-    hurst: FlexibleRange = Field(..., gt=0, lt=1)
-    discretize_ratio: FlexibleRange = Field(..., gt=0, le=1)
-    metadata_schema: List[str] = SchemaList(["hurst", "discretize_ratio"])
-
-    custom_seed_schema: List[str] = SchemaList(
-        ["hurst", "discretize_ratio", "dependency"]
-    )
-
-    def make_dependency(self, num_sequence: int):
-        # prepare random generators
-        rngs = {}
-        for field in ["hurst", "sequence_length", "discretize_ratio", "dependency"]:
-            rngs[field] = self.seed.get_rng(field)
-
-        dep_rngs = self.seed.get_rng("dependency", num_sequence, return_list=True)
-
-        # sample parameters
-        hursts = rngs["hurst"].uniform(self.hurst.min, self.hurst.max, num_sequence)
-        if self.sequence_length.constant:
-            lengths = [int(self.sequence_length.min)] * num_sequence
-        else:
-            lengths = rngs["sequence_length"].integers(
-                self.sequence_length.min, self.sequence_length.max, num_sequence
-            )
-        binning_ratios = rngs["discretize_ratio"].uniform(
+class FunctionDependency(BaseDependency):
+    """Dependency from a function"""
+
+    generator: str = "function"
+
+    function: str
+
+    # python code for the function, for example "func = lambda x: np.sin(x)", please use numpy function recommended
+    # please name the function as "func"
+    discretize_ratio: FlexibleRange = Field(..., gt=0, le=1)  # ratio for binning
+    metadata_schema: List[str] = SchemaList(["sequence_length", "discretize_ratio"])
+    custom_seed_schema: List[str] = SchemaList(["discretize_ratio"])
+
+    def make_function_dependency(self, num_sequence: int):
+        length_rng = self.seed.get_rng("sequence_length")
+        binning_ratio_rng = self.seed.get_rng("discretize_ratio")
+        lengths = length_rng.integers(
+            self.sequence_length.min, self.sequence_length.max, num_sequence
+        )
+        env = {}
+        exec(self.function, {"np": np}, env)
+        func = env["func"]
+        binning_ratios = binning_ratio_rng.uniform(
             self.discretize_ratio.min, self.discretize_ratio.max, num_sequence
         )
+        
+        dependencies_raw = [func(np.arange(length)) for length in lengths]
+        
         # make digitizer
         digitizers = [make_digitizer(ratio) for ratio in binning_ratios]
-        # make fbms
-        fbms = [
-            FractionalBrownianMotion(hurst, rng=rng)
-            for hurst, rng in zip(hursts, dep_rngs)
+        dependencies = [
+            list(digitize(dr)) for dr, digitize in (dependencies_raw, digitizers)
         ]
-        deps_raw = [fbm.sample(length - 1) for length, fbm in zip(lengths, fbms)]
-        dependencies = [digitize(dr) for dr, digitize in zip(deps_raw, digitizers)]
         metadata = [
-            {"hurst": h, "sequence_length": l, "discretize_ratio": b}
-            for h, l, b in zip(hursts, lengths, binning_ratios)
+            {"sequence_length": l, "binning_ratio": b}
+            for l, b in zip(lengths, binning_ratios)
         ]
-        return DependencyResult(dependencies, metadata)
+        return DependencyResult(dependencies, metadata)
```

### Comparing `seqthetic-0.1.5/seqthetic/dependencies/random.py` & `seqthetic-0.1.6/seqthetic/dependencies/random.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/mapping.py` & `seqthetic-0.1.6/seqthetic/mapping.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,115 @@
 from typing import Callable, Dict, List, Literal, Tuple
 
+from tqdm import tqdm
 import numpy as np
 from pydantic import BaseModel, Field
 
 from seqthetic.seed import Seed
 from seqthetic.vocabulary import VocabProb
+from joblib_progress import joblib_progress
+from joblib import Parallel, delayed
+from more_itertools import chunked
 
 Mapping = Dict[int, Tuple[List[int], List[float]]]
 
 
 class MappingSpec(BaseModel):
     """Mapping dependency to word"""
 
     sample_by: Literal["frequency", "random"] = "frequency"
     map_by: Literal["frequency", "random"] = "frequency"
     # whether to split dependency and generate multiple sequences
     # e.g. 1 means no split
     # 2 means 1 dependency split in half and mapped to 2 sequences
-    # 
+    #
     # todo
     split_dependency_ratio: int = Field(default=1, ge=1)
     # how many sequence are generated from the same dependency with different vocabulary
     # e.g. 1 means no duplication, 2 means 1 dependency mapped to 2 sequences with different vocabulary
     # todo
     duplicate_dependency_ratio: int = Field(default=1, ge=1)
+
     @staticmethod
     def make_dep_freq(dependency: np.ndarray) -> np.ndarray:
         # 定义结构体的数据类型
         dtype = [("dep", int), ("freq", int)]
 
         # 统计每个元素的出现频率
         unique_deps, counts = np.unique(dependency, return_counts=True)
 
         # 创建结构体数组
         structured_array = np.array(list(zip(unique_deps, counts)), dtype=dtype)
 
         # 按频率降序排列
         sorted_array = np.sort(structured_array, order="freq")[::-1]
 
-        return sorted_array
+        return sorted_array["dep"]
+
+    @staticmethod
+    def map_one_to_sequence(
+        dependency: np.ndarray,
+        unique_dep: np.ndarray,
+        sampled_vocab: np.ndarray,
+    ):
+        # consider moving mapping to prepare_params
+        mapping = {d: v for d, v in zip(unique_dep, sampled_vocab)}
+        seq = np.array([mapping[d] for d in dependency])
+        return seq
+
+    def prepare_params(
+        self,
+        dependencies: list[np.ndarray],
+        vocab: VocabProb,
+        sample_rngs: list[np.random.Generator],
+        n_jobs: int,
+        unique_dep_str: str,
+        sample_str: str,
+    ):
+        sample_by = self.sample_by == "frequency"
+        map_by = self.map_by == "frequency"
+        with joblib_progress(
+            unique_dep_str, total=len(dependencies)
+        ):
+            unique_deps = list(
+                Parallel(n_jobs=n_jobs)(
+                    delayed(self.make_dep_freq)(dependency)
+                    for dependency in dependencies
+                )
+            )
+        # sampled vocabs is much smaller than vocabs
+        dep_vocab_nums = [len(dep_freq) for dep_freq in unique_deps]
+        with joblib_progress(
+            sample_str, total=len(dependencies)
+        ):
+            sampled_vocabs = list(
+                Parallel(n_jobs=n_jobs)(
+                    delayed(vocab.sample_vocab)(
+                        dep_vocab_num,
+                        rng,
+                        sample_by_frequency=sample_by,
+                        sort_by_frequency=map_by,
+                    )
+                    for dep_vocab_num, rng in zip(dep_vocab_nums, sample_rngs)
+                )
+            )
+
+        return unique_deps, sampled_vocabs
 
     def map_to_sequence(
         self, dependencies: list[np.ndarray], vocab: VocabProb, vocab_seed: Seed
     ) -> list[list[int]]:
         num_dependency = len(dependencies)
 
         sample_rngs = vocab_seed.get_rng("sample", num_dependency, return_list=True)
 
-        dep_freqs = [self.make_dep_freq(dependency) for dependency in dependencies]
+        dep_freqs = [
+            self.make_dep_freq(dependency)
+            for dependency in tqdm(dependencies, desc="Dependency to vocab mapping.")
+        ]
         #
         # one to one mapping from dependency to vocab, on condition that it's used for sequence
         dep_vocab_nums = [len(dep_freq) for dep_freq in dep_freqs]
 
         sample_by = self.sample_by == "frequency"
         map_by = self.map_by == "frequency"
```

### Comparing `seqthetic-0.1.5/seqthetic/range.py` & `seqthetic-0.1.6/seqthetic/range.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from abc import ABC
 from typing import Annotated
 
-from pydantic import (AfterValidator, BaseModel, PlainSerializer,
-                      computed_field, model_validator)
+from pydantic import (
+    AfterValidator,
+    BaseModel,
+    PlainSerializer,
+    computed_field,
+    model_validator,
+)
 
 
 class Range(BaseModel, ABC):
     min: float
     max: float
 
     @computed_field
@@ -19,14 +24,20 @@
         if self.min <= 0 or self.max <= 0:
             raise ValueError("value should be positive")
         elif self.min > self.max:
             raise ValueError("min should be less than max")
 
         return self
 
+    def __str__(self):
+        if self.constant:
+            return f"{self.min}"
+        else:
+            return f"Range({self.min}, {self.max})"
+
 
 FlexibleRangeInput = float | int | Range
 
 
 def convert_single_number(v: FlexibleRangeInput):
     if isinstance(v, int) or isinstance(v, float):
         if v <= 0:
```

### Comparing `seqthetic-0.1.5/seqthetic/seed.py` & `seqthetic-0.1.6/seqthetic/seed.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/spec_variation.py` & `seqthetic-0.1.6/seqthetic/spec_variation.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/synthesis_spec.py` & `seqthetic-0.1.6/seqthetic/synthesis_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,19 +132,20 @@
             if seq_len.constant:
                 domain.num_sequence = int(
                     domain.num_token // domain.dependency.sequence_length.min
                 )
             # todo: for not constant length sequence
         return self
 
-    def save(self, path_str: str = "./", name: str | None = None):
+    def save(self, path: str = "./"):
         """save the dataset spec to a json file"""
         spec_json = self.model_dump_json(indent=4)
-        name = name or self.id
-        path = Path(path_str) / f"{name}.synspec.json"
+        name = self.name or self.id
+        path = Path(path) / f"{name}.synspec.json"
+        print(f"Save the spec file to {path}")
         with open(path, "w") as f:
             f.write(spec_json)
         return str(path)
 
     @classmethod
     def load(cls, path: str = ""):
         with open(path, "r") as f:
```

### Comparing `seqthetic-0.1.5/seqthetic/utils.py` & `seqthetic-0.1.6/seqthetic/utils.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/vary/compose_ops.py` & `seqthetic-0.1.6/seqthetic/vary/compose_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/vary/compute_ops.py` & `seqthetic-0.1.6/seqthetic/vary/compute_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/vary/domain_ops.py` & `seqthetic-0.1.6/seqthetic/vary/domain_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/vary/transform.py` & `seqthetic-0.1.6/seqthetic/vary/transform.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/vary/variation.py` & `seqthetic-0.1.6/seqthetic/vary/variation.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/vary/variator.py` & `seqthetic-0.1.6/seqthetic/vary/variator.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/seqthetic/vocabulary.py` & `seqthetic-0.1.6/seqthetic/vocabulary.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.5/PKG-INFO` & `seqthetic-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: seqthetic
-Version: 0.1.5
+Version: 0.1.6
 Summary: Creates sequence data for pretraining and benchmarking sequence models
 Author: Shom
 Author-email: shaomi_lin@126.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: flake8 (>=7.0.0,<8.0.0)
+Requires-Dist: joblib (>=1.4.2,<2.0.0)
+Requires-Dist: joblib-progress (>=1.0.5,<2.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: more-itertools (>=10.2.0,<11.0.0)
 Requires-Dist: nanoid (>=2.0.0,<3.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: plotly (>=5.21.0,<6.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: stochastic (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
@@ -24,14 +28,18 @@
 Features:
 1. **Diversity**: Supports generating data following various patterns including fractional Brownian Motion(fbm), [LIME](https://arxiv.org/pdf/2101.06223)(TODO), [TILT](https://arxiv.org/abs/2004.14601)(TODO) and [synthetic pretraining tasks](https://arxiv.org/abs/2206.10139) etc.
 2. **Spec-Driven**: Everything about the dataset is described by a spec, which helps with documenting each ablation and high-level manipulation. 
 3. **Reproducibility**: Processes involving randomness have their seeds recorded in the spec file. This means you can transfer the dataset by only 
 
 ## Installation 
 
+```
+pip install -e .
+
+```
 ## Usage
 
 ### Generation
 To generate a synthetic dataset, just write a spec and use synthesizer to make the dataset. For details on spec, please see [Concepts](#concepts):
 ```python
 # write the spec 
 spec = SynthesisSpec(...)
@@ -242,7 +250,8 @@
     - [ ] corpus vocab
     - [ ] domain vocab 
     - [ ] **evolution**
 - [ ] mapping
     - [ ] **multiple**
     - [ ] **clip**
 - dataloader related?
+
```

