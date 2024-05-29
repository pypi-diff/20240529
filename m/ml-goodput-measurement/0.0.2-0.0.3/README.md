# Comparing `tmp/ml_goodput_measurement-0.0.2.tar.gz` & `tmp/ml_goodput_measurement-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_goodput_measurement-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ml_goodput_measurement-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ml_goodput_measurement-0.0.2.tar` & `ml_goodput_measurement-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     6034 2024-03-01 01:13:24.675128 ml_goodput_measurement-0.0.2/README.md
--rw-r--r--   0        0        0      625 2024-03-01 01:15:03.188440 ml_goodput_measurement-0.0.2/ml_goodput_measurement/__init__.py
--rw-r--r--   0        0        0    13480 2024-03-01 01:14:02.418693 ml_goodput_measurement-0.0.2/ml_goodput_measurement/src/goodput.py
--rw-r--r--   0        0        0     6550 2024-03-01 01:14:02.418693 ml_goodput_measurement-0.0.2/ml_goodput_measurement/tests/goodput_test.py
--rw-r--r--   0        0        0     1648 2024-03-01 02:05:42.728008 ml_goodput_measurement-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6688 1970-01-01 00:00:00.000000 ml_goodput_measurement-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     8287 2024-05-29 00:15:19.273651 ml_goodput_measurement-0.0.3/README.md
+-rw-r--r--   0        0        0      674 2024-05-29 00:16:46.516125 ml_goodput_measurement-0.0.3/ml_goodput_measurement/__init__.py
+-rw-r--r--   0        0        0    25546 2024-05-29 00:15:46.287656 ml_goodput_measurement-0.0.3/ml_goodput_measurement/src/goodput.py
+-rw-r--r--   0        0        0     4177 2024-05-29 00:17:12.882081 ml_goodput_measurement-0.0.3/ml_goodput_measurement/src/monitoring.py
+-rw-r--r--   0        0        0    37941 2024-05-29 00:15:46.287656 ml_goodput_measurement-0.0.3/ml_goodput_measurement/tests/goodput_test.py
+-rw-r--r--   0        0        0     1688 2024-05-29 00:15:33.930739 ml_goodput_measurement-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9010 1970-01-01 00:00:00.000000 ml_goodput_measurement-0.0.3/PKG-INFO
```

### Comparing `ml_goodput_measurement-0.0.2/README.md` & `ml_goodput_measurement-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -21,28 +21,44 @@
  necessary information and query a job's Goodput. It can be pip installed to
  import its modules, and retrieve information about a training job's overall
  productive Goodput. The package exposes API interfaces to log useful
  information from the user application and query Goodput for the job run, gain
  insight into the productivity of ML workloads and utilization of compute
  resources.
 
+ The package also exposes Goodput Monitoring APIs which allow asynchronous query
+ and export of the job's Goodput to Tensorboard with configurable upload interval.
+
 ## Components
 
 
- The ML Goodput Measurement library consists of two main components: 
- the `GoodputRecorder` and the `GoodputCalculator`. The `GoodputRecorder`
+ The ML Goodput Measurement library consists of the following main components: 
+
+  - `GoodputRecorder`
+
+  - `GoodputCalculator`
+  - `GoodputMonitor`
+
+
+ The `GoodputRecorder`
  exposes APIs to the client to export key timestamps while a training job makes
  progress, namely APIs that allow logging of productive step time and total job
  run time. The library will serialize and store this data in Google Cloud
- Logging. The `GoodputCalculator` exposes APIs to compute Goodput based on the
+ Logging.
+
+ The `GoodputCalculator` exposes APIs to compute Goodput based on the
  recorded data. Cloud Logging handles its internal operations asynchronously.
  The recommended way to compute Goodput is to run an analysis program separate
  from the training application, either on a CPU instance or on the users'
  development machine.
 
+ The `GoodputMonitor` exposes APIs to query and upload goodput data to
+ Tensorboard asynchronously. It does this by instantiating a `GoodputCaluclator`
+ under the hood.
+
 ## Installation
 
  To install the ML Goodput Measurement package, run the following command on TPU VM:
 
  ```bash
  pip install ml-goodput-measurement
  ```
@@ -70,17 +86,17 @@
  To use this package, import the `goodput` module:
 
 
  ```python
  from ml_goodput_measurement import goodput
  ```
 
-### Define the name of the Google Cloud Logging logger bucket
+### Define the name of the Google Cloud Logging logger.
 
- Create a run-specific logger bucket where Cloud Logging entries can be written and read from.
+ Create a run-specific logger name where Cloud Logging entries can be written to and read from.
 
  For example:
 
  ```python
  goodput_logger_name = f'goodput_{config.run_name}'
  ```
 
@@ -175,7 +191,48 @@
 Finally, call the `get_job_goodput` API to retrieve Goodput for the entire job run.
 
 ```python
 total_goodput = goodput_calculator.get_job_goodput()
 print(f"Total job goodput: {total_goodput:.2f}%")
 ```
 
+### Monitor Goodput with `GoodputMonitor`
+
+In order to monitor the Goodput of a job run on Tensorboard, all you need to do
+is instantiate a `GoodputMonitor` object with the job's run name, cloud logger 
+name and Goodput monitoring configurations (as described below). Then call the 
+`start_goodput_uploader` API to asynchronously query and upload measured Goodput
+to the specified Tensorboard directory. 
+
+
+#### Create a `GoodputMonitor` object
+
+Create a `GoodputMonitor` object with the following parameters:
+
+ 1. `job_name`: The full run name of the job.
+ 2. `logger_name`: The name of the Cloud Logging logger object (created in the previous step).
+ 3. `tensorboard_dir`: The directory to write TensorBoard data to.
+ 4. `upload_interval`: The time interval at which to query and upload data to TensorBoard.
+ 5. `monitoring_enabled`: Whether or not monitoring is enabled. If the application is
+      interested in monitoring Goodput, it should set this value to True. Only one worker 
+      should enable monitoring.
+
+> **_NOTE:_** Please ensure that only **one** worker enables monitoring of Goodput.
+   In JAX, for example, the check could be `if jax.process_index() == 0`
+
+For example:
+
+```python
+goodput_logger_name = f'goodput_{config.run_name}' # You can choose your own logger name.
+goodput_monitoring_enabled = config.monitor_goodput and jax.process_index() == 0 # Check for configs whether or not the enable monitoring.
+
+goodput_monitor = goodput.GoodputMonitor(job_name=config.run_name, logger_name=logger_name, tensorboard_dir=config.tensorboard_dir, upload_interval=config.goodput_upload_interval_seconds, monitoring_enabled=goodput_monitoring_enabled)
+```
+
+#### Start asynchronous "query and upload" of Goodput
+
+Call the `start_goodput_uploader` API to spin off a thread which continuously queries and uploads Goodput.
+
+```python
+goodput_monitor.start_goodput_uploader()
+```
+
```

### Comparing `ml_goodput_measurement-0.0.2/ml_goodput_measurement/__init__.py` & `ml_goodput_measurement-0.0.3/ml_goodput_measurement/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
@@ -10,7 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ml_goodput_measurement.src import goodput
+from ml_goodput_measurement.src import monitoring
```

### Comparing `ml_goodput_measurement-0.0.2/pyproject.toml` & `ml_goodput_measurement-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [project]
 name = "ml_goodput_measurement"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Cloud TPU Team", email="cloud-tpu-eng@google.com" },
 ]
 description = "Package to retrieve Goodput of jobs running on Cloud TPU."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "Apache-2.0"}
@@ -28,15 +28,18 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 keywords = []
 
 # pip dependencies installed with `pip install -e .`
 dependencies = [
-  "google-cloud-logging>=3.5.0"
+  "google-cloud-logging>=3.5.0",
+  "numpy",
+  "scipy",
+  "tensorboard",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/google/cloud_tpu_goodput"
 "Bug Tracker" = "https://github.com/google/cloud_tpu_goodput/issues"
 
 [build-system]
```

### Comparing `ml_goodput_measurement-0.0.2/PKG-INFO` & `ml_goodput_measurement-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: ml_goodput_measurement
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to retrieve Goodput of jobs running on Cloud TPU.
 Keywords: 
 Author-email: Cloud TPU Team <cloud-tpu-eng@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-cloud-logging>=3.5.0
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: tensorboard
 Project-URL: Bug Tracker, https://github.com/google/cloud_tpu_goodput/issues
 Project-URL: Homepage, https://github.com/google/cloud_tpu_goodput
 
 <!--
  Copyright 2023 Google LLC
 
  Licensed under the Apache License, Version 2.0 (the "License");
@@ -37,28 +40,44 @@
  necessary information and query a job's Goodput. It can be pip installed to
  import its modules, and retrieve information about a training job's overall
  productive Goodput. The package exposes API interfaces to log useful
  information from the user application and query Goodput for the job run, gain
  insight into the productivity of ML workloads and utilization of compute
  resources.
 
+ The package also exposes Goodput Monitoring APIs which allow asynchronous query
+ and export of the job's Goodput to Tensorboard with configurable upload interval.
+
 ## Components
 
 
- The ML Goodput Measurement library consists of two main components: 
- the `GoodputRecorder` and the `GoodputCalculator`. The `GoodputRecorder`
+ The ML Goodput Measurement library consists of the following main components: 
+
+  - `GoodputRecorder`
+
+  - `GoodputCalculator`
+  - `GoodputMonitor`
+
+
+ The `GoodputRecorder`
  exposes APIs to the client to export key timestamps while a training job makes
  progress, namely APIs that allow logging of productive step time and total job
  run time. The library will serialize and store this data in Google Cloud
- Logging. The `GoodputCalculator` exposes APIs to compute Goodput based on the
+ Logging.
+
+ The `GoodputCalculator` exposes APIs to compute Goodput based on the
  recorded data. Cloud Logging handles its internal operations asynchronously.
  The recommended way to compute Goodput is to run an analysis program separate
  from the training application, either on a CPU instance or on the users'
  development machine.
 
+ The `GoodputMonitor` exposes APIs to query and upload goodput data to
+ Tensorboard asynchronously. It does this by instantiating a `GoodputCaluclator`
+ under the hood.
+
 ## Installation
 
  To install the ML Goodput Measurement package, run the following command on TPU VM:
 
  ```bash
  pip install ml-goodput-measurement
  ```
@@ -86,17 +105,17 @@
  To use this package, import the `goodput` module:
 
 
  ```python
  from ml_goodput_measurement import goodput
  ```
 
-### Define the name of the Google Cloud Logging logger bucket
+### Define the name of the Google Cloud Logging logger.
 
- Create a run-specific logger bucket where Cloud Logging entries can be written and read from.
+ Create a run-specific logger name where Cloud Logging entries can be written to and read from.
 
  For example:
 
  ```python
  goodput_logger_name = f'goodput_{config.run_name}'
  ```
 
@@ -191,8 +210,49 @@
 Finally, call the `get_job_goodput` API to retrieve Goodput for the entire job run.
 
 ```python
 total_goodput = goodput_calculator.get_job_goodput()
 print(f"Total job goodput: {total_goodput:.2f}%")
 ```
 
+### Monitor Goodput with `GoodputMonitor`
+
+In order to monitor the Goodput of a job run on Tensorboard, all you need to do
+is instantiate a `GoodputMonitor` object with the job's run name, cloud logger 
+name and Goodput monitoring configurations (as described below). Then call the 
+`start_goodput_uploader` API to asynchronously query and upload measured Goodput
+to the specified Tensorboard directory. 
+
+
+#### Create a `GoodputMonitor` object
+
+Create a `GoodputMonitor` object with the following parameters:
+
+ 1. `job_name`: The full run name of the job.
+ 2. `logger_name`: The name of the Cloud Logging logger object (created in the previous step).
+ 3. `tensorboard_dir`: The directory to write TensorBoard data to.
+ 4. `upload_interval`: The time interval at which to query and upload data to TensorBoard.
+ 5. `monitoring_enabled`: Whether or not monitoring is enabled. If the application is
+      interested in monitoring Goodput, it should set this value to True. Only one worker 
+      should enable monitoring.
+
+> **_NOTE:_** Please ensure that only **one** worker enables monitoring of Goodput.
+   In JAX, for example, the check could be `if jax.process_index() == 0`
+
+For example:
+
+```python
+goodput_logger_name = f'goodput_{config.run_name}' # You can choose your own logger name.
+goodput_monitoring_enabled = config.monitor_goodput and jax.process_index() == 0 # Check for configs whether or not the enable monitoring.
+
+goodput_monitor = goodput.GoodputMonitor(job_name=config.run_name, logger_name=logger_name, tensorboard_dir=config.tensorboard_dir, upload_interval=config.goodput_upload_interval_seconds, monitoring_enabled=goodput_monitoring_enabled)
+```
+
+#### Start asynchronous "query and upload" of Goodput
+
+Call the `start_goodput_uploader` API to spin off a thread which continuously queries and uploads Goodput.
+
+```python
+goodput_monitor.start_goodput_uploader()
+```
+
```

