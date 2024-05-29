# Comparing `tmp/appmesh-1.1.7-py3-none-any.whl.zip` & `tmp/appmesh-1.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16442 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-27 11:16 appmesh/__init__.py
--rw-r--r--  2.0 unx    59591 b- defN 24-May-27 11:16 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10832 b- defN 24-May-27 11:16 appmesh-1.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-27 11:16 appmesh-1.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-27 11:16 appmesh-1.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-27 11:16 appmesh-1.1.7.dist-info/RECORD
-6 files, 70989 bytes uncompressed, 15620 bytes compressed:  78.0%
+Zip file size: 16482 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-29 12:22 appmesh/__init__.py
+-rw-r--r--  2.0 unx    59591 b- defN 24-May-29 12:22 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10945 b- defN 24-May-29 12:22 appmesh-1.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 12:22 appmesh-1.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-29 12:22 appmesh-1.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-29 12:22 appmesh-1.1.8.dist-info/RECORD
+6 files, 71102 bytes uncompressed, 15660 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-1.1.7.dist-info/METADATA
+Filename: appmesh-1.1.8.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-1.1.7.dist-info/WHEEL
+Filename: appmesh-1.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-1.1.7.dist-info/top_level.txt
+Filename: appmesh-1.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-1.1.7.dist-info/RECORD
+Filename: appmesh-1.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `appmesh-1.1.7.dist-info/METADATA` & `appmesh-1.1.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 1.1.7
+Version: 1.1.8
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 ---|---
 Application management | 1. Manage independent applications and guard the process running, similar with systemd but more flexible (long/short running, periodic long running, cron schedule, customized day time and error handling control) and comprehensive monitoring (number of starts, return code, error message, health-check) for both native and docker application. <br> 2. Use SDK/CLI run application on a remote host with sync/async mode and fetch result to client. <br> 3. Full control of application lifecycle (cgroup for resource limitation, specific OS user for execution user). <br> 4. Interactive application start support specify input data by pipe and environment variables.<br> 5. All functionality provides by [CLI](https://app-mesh.readthedocs.io/en/latest/CLI.html), [REST](https://app-mesh.readthedocs.io/en/latest/Development.html#rest-apis), [SDK](https://github.com/laoshanxi/app-mesh/tree/main/src/sdk) and [WebGUI](https://github.com/laoshanxi/app-mesh-ui) interface.<br>
 Security |  ⚡️ [JWT authentication](https://app-mesh.readthedocs.io/en/latest/JWT.html) for CLI and REST interface <br> ⚡️ [LDAP support](https://app-mesh.readthedocs.io/en/latest/LDAP.html) <br> ⚡️ [Role based permission control](https://app-mesh.readthedocs.io/en/latest/USER_ROLE.html) <br> ⚡️ [Multi-factor authentication](https://app-mesh.readthedocs.io/en/latest/MFA.html)<br> SSL support (ECDH and secure ciphers) for REST http connection  <br> Multi-tenant support
 Cloud native | Schedule cloud level applications for running on multile hosts with resource size request.<br> ⚡️ [Prometheus Exporter (build-in)](https://app-mesh.readthedocs.io/en/latest/PROMETHEUS.html) <br> ⚡️ [Grafana SimpleJson datasource](https://app-mesh.readthedocs.io/en/latest/GrafanaDataSource.html) <br> ⚡️ [Grafana Loki](https://app-mesh.readthedocs.io/en/latest/Loki.html) <br>⚡️ [Dockerfile](https://github.com/laoshanxi/app-mesh/blob/main/Dockerfile)
 Micro service application | ⚡️ [Consul micro-service cluster management](https://app-mesh.readthedocs.io/en/latest/CONSUL.html)
 Extra Features | Collect host/app resource usage <br> Remote run shell commands <br> Download/Upload files interface <br> Hot-update support `systemctl reload appmesh` <br> Bash completion <br> Reverse proxy <br> [Web GUI](https://github.com/laoshanxi/app-mesh-ui)
 Platform support | X86_64 <br> ARM32 <br> ARM64
-SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/appmesh_client.html) <br> [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/appmesh_client.go) <br> Swagger `https://localhost:6060/swagger`
+SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/appmesh_client.html) <br> [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/appmesh_client.go) <br> Swagger [OpenAPI Specification](https://raw.githubusercontent.com/laoshanxi/app-mesh/main/src/daemon/rest/openapi.yaml) `https://localhost:6060/swagger` 
 
 ## Getting started
 
 The [Installation doc](https://app-mesh.readthedocs.io/en/latest/Install.html) introduces how
 to install App Mesh via docker-compose or native way and setup App Mesh cluster.
 
 ## Documentation
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 1.1.7 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 1.1.8 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
@@ -67,38 +67,40 @@
 Reverse proxy
 [Web GUI](https://github.com/laoshanxi/app-mesh-ui) Platform support | X86_64
 ARM32
 ARM64 SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/
 appmesh_client.html)
 [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/
 appmesh_client.go)
-Swagger `https://localhost:6060/swagger` ## Getting started The [Installation
-doc](https://app-mesh.readthedocs.io/en/latest/Install.html) introduces how to
-install App Mesh via docker-compose or native way and setup App Mesh cluster.
-## Documentation - [Read the Docs](https://app-mesh.readthedocs.io/) - [REST
-API](https://app-mesh.readthedocs.io/en/latest/Development.html#rest-apis) -
-[Command lines](https://app-mesh.readthedocs.io/en/latest/CLI.html) -
-[Security](https://app-mesh.readthedocs.io/en/latest/JWT.html) ## Comparison
-### Standalone mode | Feature | App Mesh | [Supervisor](http://supervisord.org/
-) | [crontab](https://crontab.guru/) | | ------------------------ | -------- |
-------------------------------------- | -------------------------------- | |
-Accuracy | Seconds | Seconds | Minutes | | Language | C++11 | Python | C | |
-Web GUI | â | â | | Command lines | â | â | â | | SDK | â | | |
-Cron schedule expression | â | | â | | Manage daemon process | | | â | |
-Manage docker app | â | | | Start check (avoid leak) | â | â | | Session
-login | | | | Manage stdout/stderr | â | â | | Health check | â | | |
-Rich control options | â | | | Authentication | â | â | | Multi-tenant |
-â | | â | ### Cluster mode | Feature | App Mesh | Kubernetes | | ----------
-------- | -------- | ---------- | | Easy deploy | â | | More features | | â
-| | Non-container app | â | | Service expose | â | â | | Scheduler | â
-| â | | Definition file | JSON | YAML | | GUI | â | â | | Virtual Network
-| | â | | Monitor tools | â | â | --- ### Component diagram ![block-
-diagram](https://github.com/laoshanxi/app-mesh/raw/main/docs/source/
-block_diagram.png) --- ## Success - [Build a powerful monitor system with
-Grafana/Prometheus/Loki](https://app-mesh.readthedocs.io/en/latest/success/
+Swagger [OpenAPI Specification](https://raw.githubusercontent.com/laoshanxi/
+app-mesh/main/src/daemon/rest/openapi.yaml) `https://localhost:6060/swagger` ##
+Getting started The [Installation doc](https://app-mesh.readthedocs.io/en/
+latest/Install.html) introduces how to install App Mesh via docker-compose or
+native way and setup App Mesh cluster. ## Documentation - [Read the Docs]
+(https://app-mesh.readthedocs.io/) - [REST API](https://app-
+mesh.readthedocs.io/en/latest/Development.html#rest-apis) - [Command lines]
+(https://app-mesh.readthedocs.io/en/latest/CLI.html) - [Security](https://app-
+mesh.readthedocs.io/en/latest/JWT.html) ## Comparison ### Standalone mode |
+Feature | App Mesh | [Supervisor](http://supervisord.org/) | [crontab](https://
+crontab.guru/) | | ------------------------ | -------- | ----------------------
+--------------- | -------------------------------- | | Accuracy | Seconds |
+Seconds | Minutes | | Language | C++11 | Python | C | | Web GUI | â | â | |
+Command lines | â | â | â | | SDK | â | | | Cron schedule expression |
+â | | â | | Manage daemon process | | | â | | Manage docker app | â | |
+| Start check (avoid leak) | â | â | | Session login | | | | Manage stdout/
+stderr | â | â | | Health check | â | | | Rich control options | â | |
+| Authentication | â | â | | Multi-tenant | â | | â | ### Cluster mode
+| Feature | App Mesh | Kubernetes | | ----------------- | -------- | ---------
+- | | Easy deploy | â | | More features | | â | | Non-container app | â |
+| Service expose | â | â | | Scheduler | â | â | | Definition file |
+JSON | YAML | | GUI | â | â | | Virtual Network | | â | | Monitor tools |
+â | â | --- ### Component diagram ![block-diagram](https://github.com/
+laoshanxi/app-mesh/raw/main/docs/source/block_diagram.png) --- ## Success -
+[Build a powerful monitor system with Grafana/Prometheus/Loki](https://app-
+mesh.readthedocs.io/en/latest/success/
 build_powerful_monitor_system_with_Grafana_Prometheus_Loki.html) - [Customize
 application start behavior](https://app-mesh.readthedocs.io/en/latest/success/
 customize_app_startup_behavior.html) - [Manage cluster-level microservice
 applications](https://app-mesh.readthedocs.io/en/latest/success/
 manage_cluster_level_microservice_applications.html) - [Open service broker
 support local PV for Kubernetes](https://app-mesh.readthedocs.io/en/latest/
 success/open_service_broker_support_local_pv_for_K8S.html) - [Promote native
```

