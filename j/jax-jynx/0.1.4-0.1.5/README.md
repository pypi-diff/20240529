# Comparing `tmp/jax_jynx-0.1.4.tar.gz` & `tmp/jax_jynx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_jynx-0.1.4.tar", max compression
+gzip compressed data, was "jax_jynx-0.1.5.tar", max compression
```

## Comparing `jax_jynx-0.1.4.tar` & `jax_jynx-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1078 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/LICENSE
--rw-r--r--   0        0        0     4048 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/README.md
--rw-r--r--   0        0        0      384 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/__init__.py
--rw-r--r--   0        0        0     5425 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/callbacks.py
--rw-r--r--   0        0        0     3603 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/fit.py
--rw-r--r--   0        0        0     1755 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/__init__.py
--rw-r--r--   0        0        0    21152 2024-04-18 13:25:50.893671 jax_jynx-0.1.4/jynx/layers/containers.py
--rw-r--r--   0        0        0     2059 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/factory.py
--rw-r--r--   0        0        0    12781 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/linear.py
--rw-r--r--   0        0        0     6896 2024-04-18 13:48:03.591997 jax_jynx-0.1.4/jynx/layers/misc.py
--rw-r--r--   0        0        0     2785 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/module.py
--rw-r--r--   0        0        0     4614 2024-05-28 13:37:39.495061 jax_jynx-0.1.4/jynx/layers/nets.py
--rw-r--r--   0        0        0     8084 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/rnn.py
--rw-r--r--   0        0        0     3922 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/static.py
--rw-r--r--   0        0        0    22219 2024-04-18 13:49:43.470562 jax_jynx-0.1.4/jynx/layers/transformer.py
--rw-r--r--   0        0        0     4849 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/pytree.py
--rw-r--r--   0        0        0     1141 2024-05-28 13:35:33.484894 jax_jynx-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 jax_jynx-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4048 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/README.md
+-rw-r--r--   0        0        0      384 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/__init__.py
+-rw-r--r--   0        0        0     5554 2024-05-29 11:49:23.292837 jax_jynx-0.1.5/jynx/callbacks.py
+-rw-r--r--   0        0        0     3603 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/fit.py
+-rw-r--r--   0        0        0     1755 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/layers/__init__.py
+-rw-r--r--   0        0        0    21152 2024-04-18 13:25:50.893671 jax_jynx-0.1.5/jynx/layers/containers.py
+-rw-r--r--   0        0        0     2059 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/layers/factory.py
+-rw-r--r--   0        0        0    12781 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/layers/linear.py
+-rw-r--r--   0        0        0     6896 2024-04-18 13:48:03.591997 jax_jynx-0.1.5/jynx/layers/misc.py
+-rw-r--r--   0        0        0     2785 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/layers/module.py
+-rw-r--r--   0        0        0     4614 2024-05-29 11:46:35.010773 jax_jynx-0.1.5/jynx/layers/nets.py
+-rw-r--r--   0        0        0     8084 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/layers/rnn.py
+-rw-r--r--   0        0        0     3922 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/layers/static.py
+-rw-r--r--   0        0        0    22219 2024-04-18 13:49:43.470562 jax_jynx-0.1.5/jynx/layers/transformer.py
+-rw-r--r--   0        0        0     4849 2024-04-18 13:22:10.769575 jax_jynx-0.1.5/jynx/pytree.py
+-rw-r--r--   0        0        0     1141 2024-05-29 11:51:02.023704 jax_jynx-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 jax_jynx-0.1.5/PKG-INFO
```

### Comparing `jax_jynx-0.1.4/LICENSE` & `jax_jynx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/README.md` & `jax_jynx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/callbacks.py` & `jax_jynx-0.1.5/jynx/callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import typing as tp
 from dataclasses import dataclass
 from pathlib import Path
 
 import numpy as np
 
-type Logs = tp.Dict[str, tp.Any]
+type Logs = dict[str, tp.Any]
 type TrainState = tp.Any
 
 
 def StopIfDryRun(dry_run: bool) -> tp.Callable[..., None]:
     def fun(*args):
         del args
         if dry_run:
-            raise StopIteration()
+            raise StopIteration
 
     return fun
 
 
 class _Monitor:
     def __init__(self, name: str, mode: tp.Literal["min", "max"] = "min"):
         from numpy import inf
@@ -43,22 +43,22 @@
 
     def __call__(self, state: TrainState, logs: Logs):
         step, value = logs["step"], logs[self.monitor.name]
         if self.monitor.is_better(value):
             self.monitor.best = value
             self.last_improvement = step
         if step - self.last_improvement >= self.steps_without_improvement:
-            raise StopIteration()
+            raise StopIteration
 
 
 class CheckPoint:
     def __init__(
         self,
-        path: tp.Union[Path, str],
-        monitor: tp.Optional[str] = None,
+        path: Path | str,
+        monitor: str | None = None,
         mode: tp.Literal["min", "max"] = "min",
     ):
         from os import makedirs
         from os.path import exists
 
         self.path = Path(path)
         self.monitor = _Monitor(monitor, mode) if monitor is not None else None
@@ -81,45 +81,45 @@
                 {
                     "state": state,
                     "logs": logs,
                 },
                 stream,
             )
 
-    def load(self) -> tp.Tuple[TrainState, Logs]:
+    def load(self) -> tuple[TrainState, Logs]:
         import cloudpickle as pickle
 
         with self.path.open("rb") as stream:
             obj = pickle.load(stream)
 
         return obj["state"], obj["logs"]
 
 
 class Logger:
-    def __init__(self, metrics: tp.Optional[tp.Sequence[str]] = None):
+    def __init__(self, metrics: tp.Sequence[str] | None = None):
         self.metrics = metrics
 
     def __call__(self, state: TrainState, logs: Logs):
         if self.metrics is not None:
             metrics = self.metrics
         else:
             metrics = [k for k in logs.keys() if k != "step"]
 
         for m in metrics:
             self.log(m, logs[m], logs["step"])
 
     def log_hparams(self, hparams: Logs):
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def log(self, metric_name: str, value: tp.Any, step: int):
         ...
 
 
 class TensorBoardLogger(Logger):
-    def __init__(self, log_dir: str, metrics: tp.Optional[tp.Sequence[str]] = None):
+    def __init__(self, log_dir: str, metrics: tp.Sequence[str] | None = None):
         super().__init__(metrics)
         from tensorboardX import SummaryWriter
 
         self.writer = SummaryWriter(log_dir)
 
     def log_hparams(self, hparams, metrics={}):
         self.writer.add_hparams(hparams, metrics)
@@ -140,15 +140,15 @@
         mlflow.log_metric(metric_name, value, step)
 
 
 class ConsoleLogger(Logger):
     def __init__(
         self,
         name: str = __name__,
-        metrics: tp.Optional[tp.Sequence[str]] = None,
+        metrics: tp.Sequence[str] | None = None,
     ):
         super().__init__(metrics)
         import logging
 
         self.logger = logging.getLogger(name)
         self.logger.addHandler(logging.StreamHandler())
         self.logger.setLevel(logging.INFO)
@@ -159,33 +159,37 @@
     def log(self, metric_name, value, step):
         self.logger.info("Step [%s], %s = %s", step, metric_name, value)
 
 
 @dataclass(frozen=True)
 class BatchMetric[B, T]:
     compute_on_batch: tp.Callable[[TrainState, B], T]
-    aggregate: tp.Callable[[tp.List[T]], T] = np.mean  # type: ignore
+    aggregate: tp.Callable[[list[T]], T] = np.mean  # type: ignore
 
 
-type Metric[B, T] = tp.Union[BatchMetric[B, T], tp.Callable[[TrainState], T]]
+type Metric[B, T] = BatchMetric[B, T] | tp.Callable[[TrainState], T]
 
 
 class ComputeMetrics[B]:
     def __init__(
         self,
         data_iter: tp.Iterable[B],
         metrics: tp.Mapping[str, Metric[B, tp.Any]],
+        max_batches: int | None = None,
     ):
         self.data_iter = data_iter
         self.metrics = metrics
+        self.max_batches = max_batches
 
     def __call__(self, state: TrainState, logs: Logs):
         metrics: dict = {name: [] for name in self.metrics.keys()}
 
-        for batch in self.data_iter:
+        for i, batch in enumerate(self.data_iter):
+            if self.max_batches is not None and i >= self.max_batches:
+                break
             for name, metric in self.metrics.items():
                 if isinstance(metric, BatchMetric):
                     metrics[name].append(metric.compute_on_batch(state, batch))
 
         for name, metric in self.metrics.items():
             if isinstance(metric, BatchMetric):
                 logs[name] = metric.aggregate(metrics[name])
```

### Comparing `jax_jynx-0.1.4/jynx/fit.py` & `jax_jynx-0.1.5/jynx/fit.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/__init__.py` & `jax_jynx-0.1.5/jynx/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/containers.py` & `jax_jynx-0.1.5/jynx/layers/containers.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/factory.py` & `jax_jynx-0.1.5/jynx/layers/factory.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/linear.py` & `jax_jynx-0.1.5/jynx/layers/linear.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/misc.py` & `jax_jynx-0.1.5/jynx/layers/misc.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/module.py` & `jax_jynx-0.1.5/jynx/layers/module.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/nets.py` & `jax_jynx-0.1.5/jynx/layers/nets.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/rnn.py` & `jax_jynx-0.1.5/jynx/layers/rnn.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/static.py` & `jax_jynx-0.1.5/jynx/layers/static.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/layers/transformer.py` & `jax_jynx-0.1.5/jynx/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/jynx/pytree.py` & `jax_jynx-0.1.5/jynx/pytree.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.4/pyproject.toml` & `jax_jynx-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jax-jynx"
-version = "0.1.4"
+version = "0.1.5"
 description = "A neural network library using jax"
 authors = ["Scott Cameron"]
 readme = "README.md"
 packages = [
   { include = "jynx" }
 ]
```

### Comparing `jax_jynx-0.1.4/PKG-INFO` & `jax_jynx-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: jax-jynx
-Version: 0.1.4
+Version: 0.1.5
 Summary: A neural network library using jax
 Author: Scott Cameron
 Requires-Python: >=3.12
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jax (>=0.4.24)
 Requires-Dist: jaxlib (>=0.4.24)
 Requires-Dist: optax (>=0.1.9)
 Description-Content-Type: text/markdown
 
 # Jynx
```

