# Comparing `tmp/beaker_gantry-1.0.1.tar.gz` & `tmp/beaker_gantry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaker_gantry-1.0.1.tar", last modified: Fri May 24 18:05:15 2024, max compression
+gzip compressed data, was "beaker_gantry-1.1.0.tar", last modified: Wed May 29 19:56:55 2024, max compression
```

## Comparing `beaker_gantry-1.0.1.tar` & `beaker_gantry-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:05:15.219862 beaker_gantry-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-24 18:05:15.219862 beaker_gantry-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:05:15.219862 beaker_gantry-1.0.1/beaker_gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-24 18:05:15.000000 beaker_gantry-1.0.1/beaker_gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-24 18:05:15.000000 beaker_gantry-1.0.1/beaker_gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:05:15.000000 beaker_gantry-1.0.1/beaker_gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 18:05:15.000000 beaker_gantry-1.0.1/beaker_gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 18:05:15.000000 beaker_gantry-1.0.1/beaker_gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 18:05:15.000000 beaker_gantry-1.0.1/beaker_gantry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:05:15.215862 beaker_gantry-1.0.1/gantry/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:05:15.219862 beaker_gantry-1.0.1/gantry/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/commands/follow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/commands/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/gantry/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-24 18:04:50.000000 beaker_gantry-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:05:15.219862 beaker_gantry-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/beaker_gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 19:56:55.000000 beaker_gantry-1.1.0/beaker_gantry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:55.958855 beaker_gantry-1.1.0/gantry/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/gantry/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/follow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/commands/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/gantry/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-29 19:56:35.000000 beaker_gantry-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:56:55.962855 beaker_gantry-1.1.0/setup.cfg
```

### Comparing `beaker_gantry-1.0.1/LICENSE` & `beaker_gantry-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.0.1/PKG-INFO` & `beaker_gantry-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-gantry
-Version: 1.0.1
+Version: 1.1.0
 Summary: Gantry streamlines running Python experiments in Beaker by managing containers and boilerplate for you
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Pete Walsh <petew@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `beaker_gantry-1.0.1/README.md` & `beaker_gantry-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.0.1/beaker_gantry.egg-info/PKG-INFO` & `beaker_gantry-1.1.0/beaker_gantry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-gantry
-Version: 1.0.1
+Version: 1.1.0
 Summary: Gantry streamlines running Python experiments in Beaker by managing containers and boilerplate for you
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Pete Walsh <petew@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `beaker_gantry-1.0.1/beaker_gantry.egg-info/SOURCES.txt` & `beaker_gantry-1.1.0/beaker_gantry.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 gantry/py.typed
 gantry/util.py
 gantry/version.py
 gantry/commands/__init__.py
 gantry/commands/cluster.py
 gantry/commands/config.py
 gantry/commands/follow.py
+gantry/commands/list.py
 gantry/commands/main.py
 gantry/commands/run.py
 gantry/commands/stop.py
```

### Comparing `beaker_gantry-1.0.1/gantry/commands/cluster.py` & `beaker_gantry-1.1.0/gantry/commands/cluster.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+from typing import List
+
 import click
-from beaker import Beaker
+from beaker import Beaker, Cluster, Node
 from rich import print
+from rich.progress import Progress
+from rich.table import Table
 
 from .main import CLICK_COMMAND_DEFAULTS, CLICK_GROUP_DEFAULTS, main
 
 
 @main.group(**CLICK_GROUP_DEFAULTS)
 def cluster():
     """
@@ -21,73 +25,84 @@
 def list_clusters(cloud: bool = False):
     """
     List available clusters.
 
     By default only on-premise clusters are displayed.
     """
     beaker = Beaker.from_env(session=True)
-    clusters = [c for c in beaker.cluster.list() if c.is_cloud == cloud]
+
+    table = Table(title="Clusters", show_lines=True)
+    table.add_column("Cluster", justify="left", no_wrap=True)
+    table.add_column("Nodes")
+
+    def cluster_info(cluster: Cluster) -> str:
+        info = f"{icon} [b magenta]{cluster.full_name}[/], {len(nodes)} nodes"
+        if (limits := cluster.node_spec) is not None:
+            info += f"\nCPUs: {limits.cpu_count}\n"
+            info += f"GPUs: {limits.gpu_count or 0} {'x' if limits.gpu_type else ''} {limits.gpu_type or ''}"
+        return info
+
+    def node_info(nodes: List[Node]) -> str:
+        return "\n".join(
+            f"[i cyan]{node.hostname}[/] - "
+            f"CPUs: {node.limits.cpu_count}, "
+            f"GPUs: {node.limits.gpu_count or 0} {'x' if node.limits.gpu_type else ''} {node.limits.gpu_type or ''}"
+            for node in nodes
+        )
+
+    with Progress(transient=True) as progress:
+        task = progress.add_task("Collecting clusters...", start=False, total=None)
+        clusters = [c for c in beaker.cluster.list() if c.is_cloud == cloud]
+        progress.update(task, completed=True)
+
     for cluster in clusters:
         icon = "☁️" if cluster.is_cloud else "🏠"
         nodes = sorted(beaker.cluster.nodes(cluster), key=lambda node: node.hostname)
-        print(f"{icon} [b magenta]{cluster.full_name}[/], {len(nodes)} nodes")
-        for node in nodes:
-            print(
-                f"   [i cyan]{node.hostname}[/] - "
-                f"CPUs: {node.limits.cpu_count}, "
-                f"GPUs: {node.limits.gpu_count or 0} {'x' if node.limits.gpu_type else ''} {node.limits.gpu_type or ''}"
-            )
-        if cluster.node_spec is not None:
-            limits = cluster.node_spec
-            print(
-                f"  CPUs: {limits.cpu_count}, "
-                f"GPUs: {limits.gpu_count or 0} {'x' if limits.gpu_type else ''} {limits.gpu_type or ''}"
-            )
+        table.add_row(
+            cluster_info(cluster),
+            node_info(nodes),
+        )
+
+    print(table)
 
 
 @cluster.command(name="util", **CLICK_COMMAND_DEFAULTS)
-@click.argument("cluster", nargs=1, required=True, type=str)
-def cluster_util(cluster: str):
+@click.argument("cluster_name", nargs=1, required=True, type=str)
+def cluster_util(cluster_name: str):
     """
     Get the current status and utilization for a cluster.
     """
     beaker = Beaker.from_env(session=True)
-    cluster_util = beaker.cluster.utilization(cluster)
-    cluster = cluster_util.cluster
-    icon = "☁️" if cluster.is_cloud else "🏠"
-    print(
-        f"{icon} [b magenta]{cluster.full_name}[/]\n\n"
-        f"running jobs: {cluster_util.running_jobs} ({cluster_util.running_preemptible_jobs} preemptible)\n"
-        f"queued jobs: {cluster_util.queued_jobs}"
-    )
-    if cluster_util.nodes:
-        print("nodes:")
-    for node in sorted(cluster_util.nodes, key=lambda n: n.hostname):
-        print(
-            f"  [i cyan]{node.hostname}[/] - {node.running_jobs} jobs ({node.running_preemptible_jobs} preemptible)\n"
-            f"    CPUs free: [{'green' if node.free.cpu_count else 'red'}]"
-            f"{node.free.cpu_count} / {node.limits.cpu_count}[/]\n"
-            f"    GPUs free: [{'green' if node.free.gpu_count else 'red'}]"
-            f"{node.free.gpu_count or 0} / {node.limits.gpu_count}[/] {node.free.gpu_type or ''}\n"
-        )
-
 
-@cluster.command(name="allow-preemptible", **CLICK_COMMAND_DEFAULTS)
-@click.argument("cluster", nargs=1, required=True, type=str)
-def cluster_allow_preemptible(cluster: str):
-    """
-    Allow preemptible jobs on the cluster.
-    """
-    beaker = Beaker.from_env(session=True)
-    beaker.cluster.update(cluster, allow_preemptible=True)
-    print("[green]\N{check mark} Preemptible jobs allowed[/]")
+    with Progress(transient=True) as progress:
+        task = progress.add_task("Pulling cluster data...", start=False, total=None)
+        cluster_util = beaker.cluster.utilization(cluster_name)
+        cluster = cluster_util.cluster
+        icon = "☁️" if cluster.is_cloud else "🏠"
+        progress.update(task, completed=True)
 
+    table = Table(
+        title=(
+            f"{icon} [b magenta]{cluster.full_name}[/]\n"
+            f"[i u blue]{beaker.cluster.url(cluster)}[/]\n"
+            f"running jobs: {cluster_util.running_jobs} ({cluster_util.running_preemptible_jobs} preemptible)\n"
+            f"queued jobs: {cluster_util.queued_jobs}"
+        ),
+        show_lines=True,
+    )
+    table.add_column("Node", justify="left", no_wrap=True)
+    table.add_column("Jobs")
+    table.add_column("Utilization")
+
+    for node_util in sorted(cluster_util.nodes, key=lambda n: n.hostname):
+        table.add_row(
+            f"[i cyan]{node_util.hostname}[/]",
+            f"{node_util.running_jobs} jobs ({node_util.running_preemptible_jobs} preemptible)",
+            "[red]\N{ballot x} cordoned[/]"
+            if node_util.cordoned
+            else f"CPUs free: [{'green' if node_util.free.cpu_count else 'red'}]"
+            f"{node_util.free.cpu_count} / {node_util.limits.cpu_count}[/]\n"
+            f"GPUs free: [{'green' if node_util.free.gpu_count else 'red'}]"
+            f"{node_util.free.gpu_count or 0} / {node_util.limits.gpu_count}[/] {node_util.free.gpu_type or ''}",
+        )
 
-@cluster.command(name="disallow-preemptible", **CLICK_COMMAND_DEFAULTS)
-@click.argument("cluster", nargs=1, required=True, type=str)
-def cluster_disallow_preemptible(cluster: str):
-    """
-    Disallow preemptible jobs on the cluster.
-    """
-    beaker = Beaker.from_env(session=True)
-    beaker.cluster.update(cluster, allow_preemptible=False)
-    print("[yellow]\N{ballot x} Preemptible jobs disallowed[/]")
+    print(table)
```

### Comparing `beaker_gantry-1.0.1/gantry/commands/config.py` & `beaker_gantry-1.1.0/gantry/commands/config.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.0.1/gantry/commands/main.py` & `beaker_gantry-1.1.0/gantry/commands/main.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.0.1/gantry/commands/run.py` & `beaker_gantry-1.1.0/gantry/commands/run.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.0.1/gantry/entrypoint.sh` & `beaker_gantry-1.1.0/gantry/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.0.1/gantry/util.py` & `beaker_gantry-1.1.0/gantry/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tempfile
 import time
 from datetime import datetime
+from enum import Enum
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Optional, Tuple, Union, cast
 
 import requests
 import rich
 from beaker import (
     Beaker,
@@ -26,14 +27,19 @@
 from .exceptions import *
 from .version import VERSION
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
 
+class StrEnum(str, Enum):
+    def __str__(self) -> str:
+        return self.value
+
+
 def unique_name() -> str:
     import uuid
 
     import petname
 
     return cast(str, petname.generate()) + "-" + str(uuid.uuid4())[:7]
 
@@ -120,15 +126,15 @@
     stream_logs = exit_code is None
     if stream_logs:
         print()
         rich.get_console().rule("Logs")
 
     last_timestamp: Optional[str] = None
     since: Optional[Union[str, datetime]] = datetime.utcnow()
-    while stream_logs and exit_code is None:
+    while stream_logs and exit_code is None and not job.is_finalized:
         job = beaker.experiment.tasks(experiment.id)[0].latest_job  # type: ignore
         assert job is not None
         exit_code = job.status.exit_code
         last_timestamp = display_logs(
             beaker.job.logs(job, quiet=True, since=since),
             ignore_timestamp=last_timestamp,
         )
@@ -142,16 +148,17 @@
         print()
 
     return job
 
 
 def display_results(beaker: Beaker, experiment: Experiment, job: Job):
     exit_code = job.status.exit_code
-    assert exit_code is not None
-    if exit_code > 0:
+    if exit_code is None:
+        raise ExperimentFailedError("Experiment failed")
+    elif exit_code > 0:
         raise ExperimentFailedError(f"Experiment exited with non-zero code ({exit_code})")
     assert job.execution is not None
     assert job.status.started is not None
     assert job.status.exited is not None
     result_dataset = None
     if job.result is not None and job.result.beaker is not None:
         result_dataset = job.result.beaker
```

### Comparing `beaker_gantry-1.0.1/pyproject.toml` & `beaker_gantry-1.1.0/pyproject.toml`

 * *Files identical despite different names*

