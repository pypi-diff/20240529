# Comparing `tmp/taskara-0.1.93.tar.gz` & `tmp/taskara-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.93.tar", max compression
+gzip compressed data, was "taskara-0.1.95.tar", max compression
```

## Comparing `taskara-0.1.93.tar` & `taskara-0.1.95.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.93/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.93/README.md
--rw-r--r--   0        0        0     1171 2024-05-27 19:31:50.979325 taskara-0.1.93/pyproject.toml
--rw-r--r--   0        0        0       93 2024-05-23 21:05:47.914823 taskara-0.1.93/taskara/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.93/taskara/agent.py
--rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.93/taskara/auth/default.py
--rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.93/taskara/auth/key.py
--rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.93/taskara/auth/provider.py
--rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.93/taskara/auth/transport.py
--rw-r--r--   0        0        0    12065 2024-05-27 17:42:48.069524 taskara-0.1.93/taskara/benchmark.py
--rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.93/taskara/cli/main.py
--rw-r--r--   0        0        0      672 2024-05-23 03:23:29.445785 taskara-0.1.93/taskara/config.py
--rw-r--r--   0        0        0     2128 2024-05-23 03:34:03.414774 taskara-0.1.93/taskara/db/conn.py
--rw-r--r--   0        0        0     3504 2024-05-23 03:34:03.415046 taskara-0.1.93/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.93/taskara/env.py
--rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.93/taskara/metrics.py
--rw-r--r--   0        0        0    12137 2024-05-23 03:59:01.085005 taskara-0.1.93/taskara/runtime/base.py
--rw-r--r--   0        0        0    14316 2024-05-23 03:44:21.827171 taskara-0.1.93/taskara/runtime/docker.py
--rw-r--r--   0        0        0    30554 2024-05-23 03:34:03.415905 taskara-0.1.93/taskara/runtime/kube.py
--rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.93/taskara/runtime/load.py
--rw-r--r--   0        0        0    16258 2024-05-23 03:34:03.416381 taskara-0.1.93/taskara/runtime/process.py
--rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.93/taskara/server/app.py
--rw-r--r--   0        0        0     3514 2024-05-23 03:59:01.025899 taskara-0.1.93/taskara/server/models.py
--rw-r--r--   0        0        0     8554 2024-05-23 21:06:30.131717 taskara-0.1.93/taskara/server/router/tasks.py
--rw-r--r--   0        0        0    36653 2024-05-27 19:31:46.200442 taskara-0.1.93/taskara/task.py
--rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.93/taskara/util.py
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 taskara-0.1.93/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.95/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.95/README.md
+-rw-r--r--   0        0        0     1171 2024-05-28 21:17:06.610063 taskara-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0      349 2024-05-28 21:17:06.610377 taskara-0.1.95/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.95/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.95/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.95/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.95/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.95/taskara/auth/transport.py
+-rw-r--r--   0        0        0    17809 2024-05-28 21:17:06.610669 taskara-0.1.95/taskara/benchmark.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.95/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-23 03:23:29.445785 taskara-0.1.95/taskara/config.py
+-rw-r--r--   0        0        0     2129 2024-05-28 21:17:06.610948 taskara-0.1.95/taskara/db/conn.py
+-rw-r--r--   0        0        0     4040 2024-05-28 21:17:06.611322 taskara-0.1.95/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.95/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.95/taskara/metrics.py
+-rw-r--r--   0        0        0    12137 2024-05-23 03:59:01.085005 taskara-0.1.95/taskara/runtime/base.py
+-rw-r--r--   0        0        0    14316 2024-05-23 03:44:21.827171 taskara-0.1.95/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    30788 2024-05-28 21:17:06.611714 taskara-0.1.95/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.95/taskara/runtime/load.py
+-rw-r--r--   0        0        0    16258 2024-05-23 03:34:03.416381 taskara-0.1.95/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2340 2024-05-28 21:17:06.612057 taskara-0.1.95/taskara/server/app.py
+-rw-r--r--   0        0        0     3996 2024-05-28 21:17:06.612409 taskara-0.1.95/taskara/server/models.py
+-rw-r--r--   0        0        0     3703 2024-05-28 21:17:06.612655 taskara-0.1.95/taskara/server/router/benchmarks.py
+-rw-r--r--   0        0        0     8554 2024-05-23 21:06:30.131717 taskara-0.1.95/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    36760 2024-05-28 21:17:06.613249 taskara-0.1.95/taskara/task.py
+-rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.95/taskara/util.py
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 taskara-0.1.95/PKG-INFO
```

### Comparing `taskara-0.1.93/LICENSE` & `taskara-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/README.md` & `taskara-0.1.95/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/pyproject.toml` & `taskara-0.1.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskara"
-version = "0.1.93"
+version = "0.1.95"
 description = "Task management for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,15 +16,15 @@
 google-auth = {version = "^2.29.0", optional = true}
 google-cloud-container = {version = "^2.45.0", optional = true}
 namesgenerator = "^0.3"
 typer = {version = "^0.12.3", optional = true}
 tabulate = {version = "^0.9.0", optional = true}
 devicebay = "^0.1.25"
 shortuuid = "^1.0.13"
-skillpacks = "^0.1.30"
+skillpacks = "^0.1.31"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 flake8 = "^7.0.0"
 black = "^24.2.0"
 pytest-env = "^1.1.3"
```

### Comparing `taskara-0.1.93/taskara/agent.py` & `taskara-0.1.95/taskara/agent.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/auth/key.py` & `taskara-0.1.95/taskara/auth/key.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/auth/provider.py` & `taskara-0.1.95/taskara/auth/provider.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/auth/transport.py` & `taskara-0.1.95/taskara/auth/transport.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/cli/main.py` & `taskara-0.1.95/taskara/cli/main.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/config.py` & `taskara-0.1.95/taskara/config.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/db/conn.py` & `taskara-0.1.95/taskara/db/conn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import logging
 import os
 import time
-import logging
 
-from sqlalchemy import create_engine, Engine
+from sqlalchemy import Engine, create_engine
 from sqlalchemy.orm import sessionmaker
 
-from .models import Base
 from taskara.config import AGENTSEA_DB_DIR, DB_NAME
 
+from .models import Base
+
 logger = logging.getLogger(__name__)
 
 DB_TYPE = os.environ.get("DB_TYPE", "sqlite")
 
 
 def get_pg_conn() -> Engine:
     # Helper function to get environment variable with fallback
```

### Comparing `taskara-0.1.93/taskara/db/models.py` & `taskara-0.1.95/taskara/db/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import time
-from sqlalchemy import Boolean, Column, String, Float, Integer, ForeignKey, Table
+
+from sqlalchemy import Boolean, Column, Float, ForeignKey, Integer, String, Table
 from sqlalchemy.orm import declarative_base, relationship
 
 Base = declarative_base()
 
 benchmark_task_association = Table(
     "benchmark_task_association",
     Base.metadata,
     Column("benchmark_id", String, ForeignKey("benchmarks.id"), primary_key=True),
     Column(
         "task_template_id", String, ForeignKey("task_templates.id"), primary_key=True
     ),
 )
 
+eval_task_association = Table(
+    "eval_task_association",
+    Base.metadata,
+    Column("eval_id", String, ForeignKey("evals.id"), primary_key=True),
+    Column("task_id", String, ForeignKey("tasks.id"), primary_key=True),
+)
+
 
 class TaskRecord(Base):
     __tablename__ = "tasks"
 
     id = Column(String, primary_key=True)
     owner_id = Column(String, nullable=True)
     description = Column(String, nullable=False)
@@ -66,15 +74,14 @@
 class BenchmarkRecord(Base):
     __tablename__ = "benchmarks"
 
     id = Column(String, primary_key=True)
     owner_id = Column(String, nullable=True)
     name = Column(String, unique=True, index=True)
     description = Column(String, nullable=False)
-    owner_id = Column(String, nullable=True)
     public = Column(Boolean, default=False)
     tags = Column(String, nullable=True)
     labels = Column(String, nullable=True)
     created = Column(Float, default=time.time)
 
     task_templates = relationship(
         "TaskTemplateRecord",
@@ -84,14 +91,24 @@
 
 
 class EvalRecord(Base):
     __tablename__ = "evals"
 
     id = Column(String, primary_key=True)
     owner_id = Column(String, nullable=True)
+    benchmark_id = Column(String, ForeignKey("benchmarks.id"))
+    assigned_to = Column(String, nullable=True)
+    assigned_type = Column(String, nullable=True)
+    created = Column(Float, default=time.time)
+
+    benchmark = relationship("BenchmarkRecord")
+    tasks = relationship(
+        "TaskRecord",
+        secondary=eval_task_association,
+    )
 
 
 class TrackerRecord(Base):
     __tablename__ = "trackers"
 
     id = Column(String, primary_key=True)
     name = Column(String, unique=True, index=True)
```

### Comparing `taskara-0.1.93/taskara/metrics.py` & `taskara-0.1.95/taskara/metrics.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/runtime/base.py` & `taskara-0.1.95/taskara/runtime/base.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/runtime/docker.py` & `taskara-0.1.95/taskara/runtime/docker.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/runtime/kube.py` & `taskara-0.1.95/taskara/runtime/kube.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-from typing import List, Optional, Tuple, Type, Union, Iterator, Dict
-import os
+import atexit
+import base64
 import json
-import urllib.error
-import urllib.parse
-import urllib.request
-from tenacity import retry, stop_after_attempt, wait_fixed
+import logging
+import os
+import signal
 import socket
-import base64
 import subprocess
-import atexit
-import signal
 import sys
-import logging
+import urllib.error
+import urllib.parse
+import urllib.request
+from math import log
+from typing import Dict, Iterator, List, Optional, Tuple, Type, Union
 
-from kubernetes import client, config
-from google.oauth2 import service_account
-from google.cloud import container_v1
 from google.auth.transport.requests import Request
-from kubernetes.client.rest import ApiException
-from kubernetes.stream import portforward
+from google.cloud import container_v1
+from google.oauth2 import service_account
+from kubernetes import client, config
 from kubernetes.client import Configuration
 from kubernetes.client.api import core_v1_api
+from kubernetes.client.rest import ApiException
+from kubernetes.stream import portforward
 from namesgenerator import get_random_name
-from tenacity import retry
 from pydantic import BaseModel
+from tenacity import retry, stop_after_attempt, wait_fixed
 
-from taskara.server.models import V1Task
+from taskara.server.models import (
+    V1ResourceLimits,
+    V1ResourceRequests,
+    V1Task,
+    V1Tracker,
+)
 from taskara.util import find_open_port
-from .base import TrackerRuntime, Tracker
-from taskara.server.models import V1Tracker, V1ResourceLimits, V1ResourceRequests
+
+from .base import Tracker, TrackerRuntime
 
 logger = logging.getLogger(__name__)
 
 
 class GKEOpts(BaseModel):
     cluster_name: str
     region: str
@@ -91,15 +96,15 @@
         Parameters:
             name (str): The base name of the secret, usually related to the pod name.
             env_vars (dict): A dictionary containing the environment variables as key-value pairs.
 
         Returns:
             client.V1Secret: The created Kubernetes Secret object.
         """
-        print("creating secret with envs: ", env_vars)
+        logger.debug(f"creating secret with envs: {env_vars}")
         secret = client.V1Secret(
             api_version="v1",
             kind="Secret",
             metadata=client.V1ObjectMeta(
                 name=name,
                 namespace=self.namespace,
                 # This ensures that the secret is deleted when the pod is deleted.
@@ -108,18 +113,18 @@
             string_data=env_vars,
             type="Opaque",
         )
         try:
             self.core_api.create_namespaced_secret(
                 namespace=self.namespace, body=secret
             )
-            print(f"Secret created: {name}")
+            logger.debug(f"Secret created: {name}")
             return secret
         except ApiException as e:
-            print(f"Failed to create secret: {e}")
+            logger.error(f"Failed to create secret: {e}")
             raise
 
     def create(
         self,
         image: str,
         name: Optional[str] = None,
         resource_requests: V1ResourceRequests = V1ResourceRequests(),
@@ -132,15 +137,15 @@
             name = get_random_name("-")
             if not name:
                 raise ValueError("Could not generate a random name")
 
         secret = None
         if env_vars:
             # Create a secret for the environment variables
-            print("creating secret...")
+            logger.debug("creating secret...")
             secret: Optional[client.V1Secret] = self.create_secret(name, env_vars)
             env_from = [
                 client.V1EnvFromSource(
                     secret_ref=client.V1SecretEnvSource(name=secret.metadata.name)  # type: ignore
                 )
             ]
         else:
@@ -150,15 +155,15 @@
         resources = client.V1ResourceRequirements(
             requests={"memory": resource_requests.memory, "cpu": resource_requests.cpu},
             limits={"memory": resource_limits.memory, "cpu": resource_limits.cpu},
         )
         if resource_requests.gpu:
             raise ValueError("GPU resource requests are not supported")
 
-        print("\nusing resources: ", resources.__dict__)
+        logger.debug(f"using resources: {resources.__dict__}")
 
         # Container configuration
         container = client.V1Container(
             name=name,
             image=image,
             ports=[client.V1ContainerPort(container_port=9070)],
             resources=resources,
@@ -193,19 +198,19 @@
             spec=pod_spec,
         )
 
         try:
             created_pod: client.V1Pod = self.core_api.create_namespaced_pod(  # type: ignore
                 namespace=self.namespace, body=pod
             )
-            print(f"Pod created with name='{name}'")
+            logger.debug(f"Pod created with name='{name}'")
             # print("created pod: ", created_pod.__dict__)
             # Update secret's owner reference UID to newly created pod's UID
             if secret:
-                print("updating secret refs...")
+                logger.debug("updating secret refs...")
                 if not secret.metadata:
                     raise ValueError("expected secret metadata to be set")
                 if not created_pod.metadata:
                     raise ValueError("expected pod metadata to be set")
                 secret.metadata.owner_references = [
                     client.V1OwnerReference(
                         api_version="v1",
@@ -213,17 +218,17 @@
                         name=name,
                         uid=created_pod.metadata.uid,  # This should be set dynamically after pod creation
                     )
                 ]
                 self.core_api.patch_namespaced_secret(
                     name=secret.metadata.name, namespace=self.namespace, body=secret  # type: ignore
                 )
-                print("secret refs updated")
+                logger.debug("secret refs updated")
         except ApiException as e:
-            print(f"Exception when creating pod: {e}")
+            logger.error(f"Exception when creating pod: {e}")
             raise
 
         self.wait_pod_ready(name)
         self.wait_for_http_200(name)
 
     @classmethod
     def connect_config_type(cls) -> Type[KubeConnectConfig]:
@@ -254,31 +259,31 @@
         gke_service = container_v1.ClusterManagerClient(credentials=credentials)
         project_id = service_account_info.get("project_id")
         if not project_id or not opts.cluster_name or not opts.region:
             raise ValueError(
                 "Missing project_id, cluster_name, or region in credentials or metadata"
             )
 
-        print("\nK8s getting cluster...")
+        logger.debug("K8s getting cluster...")
         cluster_request = container_v1.GetClusterRequest(
             name=f"projects/{project_id}/locations/{opts.region}/clusters/{opts.cluster_name}"
         )
         cluster = gke_service.get_cluster(request=cluster_request)
 
         # Configure Kubernetes client
-        print("\nK8s getting token...")
+        logger.debug("K8s getting token...")
         ca_cert = base64.b64decode(cluster.master_auth.cluster_ca_certificate)
         try:
-            print("\nK8s refreshing token...")
+            logger.debug("K8s refreshing token...")
             credentials.refresh(Request())
         except Exception as e:
-            print("\nK8s token refresh failed: ", e)
+            logger.debug(f"K8s token refresh failed: {e}")
             raise e
         access_token = credentials.token
-        print("\nK8s got token: ", access_token)
+        logger.debug(f"K8s got token: {access_token}")
 
         cluster_name = opts.cluster_name
 
         kubeconfig = {
             "apiVersion": "v1",
             "kind": "Config",
             "clusters": [
@@ -310,15 +315,15 @@
                     },
                 }
             ],
         }
 
         config.load_kube_config_from_dict(config_dict=kubeconfig)
         v1_client = client.CoreV1Api()
-        print("\nK8s returning client...")
+        logger.debug("K8s returning client...")
 
         return v1_client, project_id, cluster_name
 
     @retry(stop=stop_after_attempt(200), wait=wait_fixed(2))
     def wait_for_http_200(self, name: str, path: str = "/", port: int = 9070):
         """
         Waits for an HTTP 200 response from the specified path on the given pod.
@@ -327,26 +332,26 @@
             name (str): The name of the pod.
             path (str): The path to query. Defaults to root '/'.
             port (int): The port on which the pod service is exposed. Defaults to 9070.
 
         Raises:
             RuntimeError: If the response is not 200 after the specified retries.
         """
-        print(
+        logger.debug(
             f"Checking HTTP 200 readiness for pod {name} on path {path} and port: {port}"
         )
         status_code, response_text = self.call(
             name=name, path=path, method="GET", port=port
         )
         if status_code != 200:
             print(f"Received status code {status_code}, retrying...")
             raise Exception(
                 f"Pod {name} at path {path} is not ready. Status code: {status_code}"
             )
-        print(f"Pod {name} at path {path} responded with: ", response_text)
+        logger.debug(f"Pod {name} at path {path} responded with: {response_text}")
         print(f"Pod {name} at path {path} is ready with status 200.")
 
     @retry(stop=stop_after_attempt(200), wait=wait_fixed(2))
     def wait_pod_ready(self, name: str) -> bool:
         """
         Checks if the specified pod is ready to serve requests.
 
@@ -363,15 +368,15 @@
                 for condition in conditions:
                     if condition.type == "Ready" and condition.status == "True":
                         print("pod is ready!")
                         return True
             print("pod is not ready yet...")
             raise Exception(f"Pod {name} is not ready")
         except ApiException as e:
-            print(f"Failed to read pod status for '{name}': {e}")
+            logger.error(f"Failed to read pod status for '{name}': {e}")
             raise
 
     @retry(stop=stop_after_attempt(15))
     def call(
         self,
         name: str,
         path: str,
@@ -496,30 +501,30 @@
             if data:
                 # Convert data to JSON string and set the request body
                 request.add_header("Content-Type", "application/json")
                 if headers:
                     for k, v in headers.items():
                         request.add_header(k, v)
                 request.data = json.dumps(data).encode("utf-8")
-            print(f"Request Data: {request.data}")
+            logger.debug(f"Request Data: {request.data}")
 
         # Send the request and handle the response
         try:
             response = urllib.request.urlopen(request)
             status_code = response.code
             response_text = response.read().decode("utf-8")
-            print(f"Status Code: {status_code}")
+            logger.debug(f"Status Code: {status_code}")
 
             # Parse the JSON response and return a dictionary
             return status_code, response_text
         except urllib.error.HTTPError as e:
             status_code = e.code
             error_message = e.read().decode("utf-8")
-            print(f"Error: {status_code}")
-            print(error_message)
+            logger.debug(f"Error: {status_code}")
+            logger.debug(error_message)
 
             raise SystemError(
                 f"Error making http request kubernetes pod {status_code}: {error_message}"
             )
         finally:
             try:
                 if response:  # type: ignore
@@ -603,15 +608,15 @@
                 name=name,
                 namespace=self.namespace,
                 follow=follow,
                 pretty="true",
                 _preload_content=False,  # Important to return a generator when following
             )
         except ApiException as e:
-            print(f"Failed to get logs for pod '{name}': {e}")
+            logger.error(f"Failed to get logs for pod '{name}': {e}")
             raise
 
     def list(
         self,
         owner_id: Optional[str] = None,
         source: bool = False,
     ) -> List[Tracker]:
@@ -625,15 +630,15 @@
                 for pod in pods.items:
                     name = pod.metadata.name
 
                     instances.append(
                         Tracker(name=name, runtime=self, status="running", port=9070)
                     )
             except ApiException as e:
-                print(f"Failed to list pods: {e}")
+                logger.error(f"Failed to list pods: {e}")
                 raise
 
         else:
             instances = Tracker.find(owner_id=owner_id, runtime_name=self.name())
 
         return instances
 
@@ -646,15 +651,15 @@
         if source:
             try:
                 pod = self.core_api.read_namespaced_pod(
                     name=name, namespace=self.namespace
                 )
                 return Tracker(name=name, runtime=self, status="running", port=9070)
             except ApiException as e:
-                print(f"Failed to get pod '{name}': {e}")
+                logger.error(f"Failed to get pod '{name}': {e}")
                 raise
 
         else:
             instances = Tracker.find(
                 name=name, owner_id=owner_id, runtime_name=self.name()
             )
             if not instances:
@@ -670,17 +675,17 @@
             # Delete the pod
             self.core_api.delete_namespaced_pod(
                 name=name,
                 namespace="default",
                 body=client.V1DeleteOptions(grace_period_seconds=5),
             )
             self.core_api.delete_namespaced_secret(name=name, namespace=self.namespace)
-            print(f"Successfully deleted pod: {name}")
+            logger.debug(f"Successfully deleted pod: {name}")
         except ApiException as e:
-            print(f"Failed to delete pod '{name}': {e}")
+            logger.error(f"Failed to delete pod '{name}': {e}")
             raise
 
     def clean(
         self,
         owner_id: Optional[str] = None,
     ) -> None:
         pods = self.core_api.list_namespaced_pod(
@@ -689,29 +694,29 @@
         for pod in pods.items:
             try:
                 self.core_api.delete_namespaced_pod(
                     name=pod.metadata.name,
                     namespace="default",
                     body=client.V1DeleteOptions(grace_period_seconds=5),
                 )
-                print(f"Deleted pod: {pod.metadata.name}")
+                logger.debug(f"Deleted pod: {pod.metadata.name}")
             except ApiException as e:
-                print(f"Failed to delete pod '{pod.metadata.name}': {e}")
+                logger.error(f"Failed to delete pod '{pod.metadata.name}': {e}")
 
     def run(
         self,
         name: str,
         env_vars: Optional[dict] = None,
         owner_id: Optional[str] = None,
         labels: Optional[Dict[str, str]] = None,
         resource_requests: V1ResourceRequests = V1ResourceRequests(),
         resource_limits: V1ResourceLimits = V1ResourceLimits(),
         auth_enabled: bool = True,
     ) -> Tracker:
-        print("creating task server...")
+        logger.debug("creating task server...")
         if not self.img:
             raise ValueError("img not found")
 
         requests = V1ResourceRequests()
         limits = V1ResourceLimits()
         self.create(
             image=self.img,
@@ -738,21 +743,23 @@
 
         try:
             log_lines = self.logs(name=server_name, follow=True)
             for line in log_lines:
                 print(line.decode("utf-8"))  # type: ignore
         except KeyboardInterrupt:
             # This block will be executed if SIGINT is caught
-            print(f"Interrupt received, stopping logs and deleting pod '{server_name}'")
+            logger.error(
+                f"Interrupt received, stopping logs and deleting pod '{server_name}'"
+            )
             self.delete(server_name)
         except ApiException as e:
-            print(f"Failed to follow logs for pod '{server_name}': {e}")
+            logger.error(f"Failed to follow logs for pod '{server_name}': {e}")
             raise
         except Exception as e:
-            print(f"An error occurred while fetching logs: {e}")
+            logger.error(f"An error occurred while fetching logs: {e}")
             raise
 
     def _signal_handler(self, server_name: str):
         def handle_signal(signum, frame):
             print(
                 f"Signal {signum} received, stopping and deleting pod '{server_name}'"
             )
```

### Comparing `taskara-0.1.93/taskara/runtime/load.py` & `taskara-0.1.95/taskara/runtime/load.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/runtime/process.py` & `taskara-0.1.95/taskara/runtime/process.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/server/app.py` & `taskara-0.1.95/taskara/server/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging.config
-from contextlib import asynccontextmanager
 import os
+from contextlib import asynccontextmanager
 
 from fastapi import FastAPI, Request, status
-from fastapi.middleware.cors import CORSMiddleware
 from fastapi.exceptions import RequestValidationError
+from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse
 
+from .router.benchmarks import router as benchmarks_router
 from .router.tasks import router as tasks_router
 
 logging.config.fileConfig("logging.conf", disable_existing_loggers=False)
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
@@ -55,14 +56,15 @@
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 app.include_router(tasks_router)
+app.include_router(benchmarks_router)
 
 
 @app.get("/")
 async def root():
     return {"message": "tasks4lyfe"}
```

### Comparing `taskara-0.1.93/taskara/server/models.py` & `taskara-0.1.95/taskara/server/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Optional, List, Dict, Any
-import shortuuid
 import time
+from typing import Any, Dict, List, Optional
 
-from threadmem.server.models import V1RoleThread
-from pydantic import BaseModel, Field
-from devicebay.models import V1Device
+import shortuuid
 from devicebay import V1Device, V1DeviceType
+from devicebay.models import V1Device
 from mllm import V1Prompt
+from pydantic import BaseModel, Field
+from threadmem.server.models import V1RoleThread
 
 
 class V1TaskUpdate(BaseModel):
     status: Optional[str] = None
     description: Optional[str] = None
     max_steps: Optional[int] = None
     error: Optional[str] = None
@@ -136,10 +136,33 @@
 
 class V1Benchmark(BaseModel):
     id: str
     name: str
     description: str
     tasks: List[V1TaskTemplate]
     owner_id: Optional[str]
-    tags: List[str]
-    labels: Dict[str, str]
+    tags: List[str] = []
+    labels: Dict[str, str] = {}
     created: float
+    public: bool = False
+
+
+class V1BenchmarkEval(BaseModel):
+    assigned_to: str | None = None
+    assigned_type: str | None = None
+
+
+class V1Benchmarks(BaseModel):
+    benchmarks: List[V1Benchmark]
+
+
+class V1Eval(BaseModel):
+    id: Optional[str] = None
+    benchmark: V1Benchmark
+    tasks: List[V1Task]
+    assigned_to: Optional[str] = None
+    assigned_type: Optional[str] = None
+    owner_id: Optional[str] = None
+
+
+class V1Evals(BaseModel):
+    evals: List[V1Eval]
```

### Comparing `taskara-0.1.93/taskara/server/router/tasks.py` & `taskara-0.1.95/taskara/server/router/tasks.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/taskara/task.py` & `taskara-0.1.95/taskara/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,20 @@
                 )
                 v1episode = V1Episode.model_validate(episode_data)
                 return Episode.from_v1(v1episode)
 
             except Exception as e:
                 logger.error(f"failed to get prompts from remote: {e}")
                 raise
-
+        
+        if not id:
+            ep = Episode()
+            ep.save()
+            return ep
+        
         episodes = Episode.find(id=id)
         if not episodes:
             raise ValueError(f"Episode by id '{id}' not found")
         return episodes[0]
 
     def record_action(
         self,
```

### Comparing `taskara-0.1.93/taskara/util.py` & `taskara-0.1.95/taskara/util.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.93/PKG-INFO` & `taskara-0.1.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.93
+Version: 0.1.95
 Summary: Task management for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: docker (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: google-auth (>=2.29.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: google-cloud-container (>=2.45.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: namesgenerator (>=0.3,<0.4)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: shortuuid (>=1.0.13,<2.0.0)
-Requires-Dist: skillpacks (>=0.1.30,<0.2.0)
+Requires-Dist: skillpacks (>=0.1.31,<0.2.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "cli" or extra == "all"
 Requires-Dist: threadmem (>=0.2.26,<0.3.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0) ; extra == "cli" or extra == "all"
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: taskara Version: 0.1.93 Summary: Task management
+Metadata-Version: 2.1 Name: taskara Version: 0.1.95 Summary: Task management
 for AI agents License: MIT Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: cli Provides-
 Extra: runtime Requires-Dist: devicebay (>=0.1.25,<0.2.0) Requires-Dist: docker
 (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all" Requires-Dist: google-
 auth (>=2.29.0,<3.0.0) ; extra == "runtime" or extra == "all" Requires-Dist:
 google-cloud-container (>=2.45.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0) ; extra == "runtime" or extra ==
 "all" Requires-Dist: namesgenerator (>=0.3,<0.4) Requires-Dist: pydantic
 (>=2.6.4,<3.0.0) Requires-Dist: shortuuid (>=1.0.13,<2.0.0) Requires-Dist:
-skillpacks (>=0.1.30,<0.2.0) Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
+skillpacks (>=0.1.31,<0.2.0) Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "cli" or extra == "all"
 Requires-Dist: threadmem (>=0.2.26,<0.3.0) Requires-Dist: typer
 (>=0.12.3,<0.13.0) ; extra == "cli" or extra == "all" Description-Content-Type:
 text/markdown
                              ************ TTaasskkaarraa ************
                         Task management for AI agents
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
```

