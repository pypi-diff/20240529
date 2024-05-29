# Comparing `tmp/ambient_edge_server-0.1.4.tar.gz` & `tmp/ambient_edge_server-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_edge_server-0.1.4.tar", last modified: Mon May 27 23:35:08 2024, max compression
+gzip compressed data, was "ambient_edge_server-0.2.0.tar", last modified: Wed May 29 06:25:05 2024, max compression
```

## Comparing `ambient_edge_server-0.1.4.tar` & `ambient_edge_server-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:35:08.033182 ambient_edge_server-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 23:35:08.033182 ambient_edge_server-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:35:08.029182 ambient_edge_server-0.1.4/ambient_edge_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:35:08.029182 ambient_edge_server-0.1.4/ambient_edge_server/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/event_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/event_handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/event_handlers/deploy_service_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/event_handlers/test_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:35:08.029182 ambient_edge_server-0.1.4/ambient_edge_server/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/routers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/routers/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/routers/ports.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:35:08.033182 ambient_edge_server-0.1.4/ambient_edge_server/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/services/authorization_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/services/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/services/handler_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/services/port_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/services/service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:35:08.033182 ambient_edge_server-0.1.4/ambient_edge_server/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/ambient_edge_server/utils/custom_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:35:08.029182 ambient_edge_server-0.1.4/ambient_edge_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 23:35:07.000000 ambient_edge_server-0.1.4/ambient_edge_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-27 23:35:07.000000 ambient_edge_server-0.1.4/ambient_edge_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:35:07.000000 ambient_edge_server-0.1.4/ambient_edge_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 23:35:07.000000 ambient_edge_server-0.1.4/ambient_edge_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 23:35:07.000000 ambient_edge_server-0.1.4/ambient_edge_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 23:35:07.000000 ambient_edge_server-0.1.4/ambient_edge_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 23:35:08.033182 ambient_edge_server-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-27 23:34:56.000000 ambient_edge_server-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.399260 ambient_edge_server-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 06:25:05.399260 ambient_edge_server-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.395260 ambient_edge_server-0.2.0/ambient_edge_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.395260 ambient_edge_server-0.2.0/ambient_edge_server/event_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/event_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/event_handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/event_handlers/deploy_service_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/event_handlers/test_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.395260 ambient_edge_server-0.2.0/ambient_edge_server/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/models/system_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.395260 ambient_edge_server-0.2.0/ambient_edge_server/repos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/repos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/repos/node_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/repos/system_daemon_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/repos/token_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.399260 ambient_edge_server-0.2.0/ambient_edge_server/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/routers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/routers/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/routers/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/routers/ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.399260 ambient_edge_server-0.2.0/ambient_edge_server/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/services/authorization_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/services/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/services/handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/services/port_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/services/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/services/system_daemon_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.399260 ambient_edge_server-0.2.0/ambient_edge_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/ambient_edge_server/utils/custom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:05.395260 ambient_edge_server-0.2.0/ambient_edge_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 06:25:05.000000 ambient_edge_server-0.2.0/ambient_edge_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-29 06:25:05.000000 ambient_edge_server-0.2.0/ambient_edge_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:25:05.000000 ambient_edge_server-0.2.0/ambient_edge_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-29 06:25:05.000000 ambient_edge_server-0.2.0/ambient_edge_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 06:25:05.000000 ambient_edge_server-0.2.0/ambient_edge_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 06:25:05.000000 ambient_edge_server-0.2.0/ambient_edge_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:25:05.399260 ambient_edge_server-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 06:24:56.000000 ambient_edge_server-0.2.0/setup.py
```

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/app.py` & `ambient_edge_server-0.2.0/ambient_edge_server/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from fastapi import FastAPI
 
-from ambient_edge_server.routers import auth, ping, ports
+from ambient_edge_server.routers import auth, daemon, ping, ports
 from ambient_edge_server.services.service_manager import svc_manager
 from ambient_edge_server.utils import logger
 
 app = FastAPI()
 
 
 async def startup():
@@ -14,11 +14,11 @@
         logger.info("Services initialized.")
     except Exception as e:
         logger.warning("Failed to initialize services: %s", e)
 
 
 app.add_event_handler("startup", startup)
 
-routers = [ping, ports, auth]
+routers = [ping, ports, auth, daemon]
 
 for router in routers:
     app.include_router(router.router)
```

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/event_handlers/base_handler.py` & `ambient_edge_server-0.2.0/ambient_edge_server/event_handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/event_handlers/deploy_service_handler.py` & `ambient_edge_server-0.2.0/ambient_edge_server/event_handlers/deploy_service_handler.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/event_handlers/test_handler.py` & `ambient_edge_server-0.2.0/ambient_edge_server/event_handlers/test_handler.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/routers/auth.py` & `ambient_edge_server-0.2.0/ambient_edge_server/routers/auth.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/routers/ping.py` & `ambient_edge_server-0.2.0/ambient_edge_server/routers/ping.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/routers/ports.py` & `ambient_edge_server-0.2.0/ambient_edge_server/routers/ports.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/services/authorization_service.py` & `ambient_edge_server-0.2.0/ambient_edge_server/services/authorization_service.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/services/event_service.py` & `ambient_edge_server-0.2.0/ambient_edge_server/services/event_service.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/services/handler_service.py` & `ambient_edge_server-0.2.0/ambient_edge_server/services/handler_service.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/services/port_service.py` & `ambient_edge_server-0.2.0/ambient_edge_server/services/port_service.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server/services/service_manager.py` & `ambient_edge_server-0.2.0/ambient_edge_server/services/service_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from ambient_event_bus_client import Client, ClientOptions
 from docker import DockerClient
 
 from ambient_edge_server.config import settings
 from ambient_edge_server.repos.node_repo import FileNodeRepo
+from ambient_edge_server.repos.system_daemon_repo import LinuxSystemDaemonRepo
 from ambient_edge_server.repos.token_repo import EncryptedTokenRepository
 from ambient_edge_server.services import (
     authorization_service,
     event_service,
     handler_service,
     port_service,
 )
+from ambient_edge_server.services.system_daemon_service import LinuxDaemonService
 from ambient_edge_server.utils import logger
 
 
 class ServiceManager:
     def __init__(self):
+        if settings.platform == "linux":
+            self._system_daemon_repo = LinuxSystemDaemonRepo()
+            self._system_daemon_service = LinuxDaemonService(self._system_daemon_repo)
+        else:
+            logger.fatal("Platform not supported")
+            raise NotImplementedError("Platform not supported")
         self._port_service = port_service.PortService()
         self._token_repo = EncryptedTokenRepository()
         self._node_repo = FileNodeRepo()
         self._authorization_service = authorization_service.AuthorizationService(
             token_repo=self._token_repo, node_repo=self._node_repo
         )
 
@@ -58,9 +66,12 @@
 
     def get_authorization_service(self):
         return self._authorization_service
 
     def get_event_service(self):
         return self._event_service
 
+    def get_system_daemon_service(self):
+        return self._system_daemon_service
+
 
 svc_manager = ServiceManager()
```

### Comparing `ambient_edge_server-0.1.4/ambient_edge_server.egg-info/SOURCES.txt` & `ambient_edge_server-0.2.0/ambient_edge_server.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,19 +9,28 @@
 ambient_edge_server.egg-info/entry_points.txt
 ambient_edge_server.egg-info/requires.txt
 ambient_edge_server.egg-info/top_level.txt
 ambient_edge_server/event_handlers/__init__.py
 ambient_edge_server/event_handlers/base_handler.py
 ambient_edge_server/event_handlers/deploy_service_handler.py
 ambient_edge_server/event_handlers/test_handler.py
+ambient_edge_server/models/__init__.py
+ambient_edge_server/models/api.py
+ambient_edge_server/models/system_service.py
+ambient_edge_server/repos/__init__.py
+ambient_edge_server/repos/node_repo.py
+ambient_edge_server/repos/system_daemon_repo.py
+ambient_edge_server/repos/token_repo.py
 ambient_edge_server/routers/__init__.py
 ambient_edge_server/routers/auth.py
+ambient_edge_server/routers/daemon.py
 ambient_edge_server/routers/ping.py
 ambient_edge_server/routers/ports.py
 ambient_edge_server/services/__init__.py
 ambient_edge_server/services/authorization_service.py
 ambient_edge_server/services/event_service.py
 ambient_edge_server/services/handler_service.py
 ambient_edge_server/services/port_service.py
 ambient_edge_server/services/service_manager.py
+ambient_edge_server/services/system_daemon_service.py
 ambient_edge_server/utils/__init__.py
 ambient_edge_server/utils/custom_logger.py
```

### Comparing `ambient_edge_server-0.1.4/setup.py` & `ambient_edge_server-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 from setuptools import setup, find_packages
 
 PACKAGE_NAME = 'ambient_edge_server'
-VERSION = '0.1.4'
+VERSION = '0.2.0'
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     packages=find_packages(),
     install_requires=[
         'fastapi==0.111.0',
```

