# Comparing `tmp/isponsorblocktv-2.0.6.tar.gz` & `tmp/isponsorblocktv-2.0.7.tar.gz`

## Comparing `isponsorblocktv-2.0.6.tar` & `isponsorblocktv-2.0.7.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.deepsource.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.dockerignore
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/Dockerfile
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/config.json.template
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/docker-compose.yml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/requirements.txt
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.github/workflows/build_docker_images.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.github/workflows/release_pypi.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.github/workflows/update_docker_readme.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/main.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/main_tui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/__main__.py
--rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/api_helpers.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/conditional_ttl_cache.py
--rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/config_setup.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/constants.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/dial_client.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/helpers.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/logging_helpers.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/macos_install.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/main.py
--rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/setup-wizard-style.tcss
--rw-r--r--   0        0        0    35402 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/setup_wizard.py
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/src/iSponsorBlockTV/ytlounge.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/LICENSE.md
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.deepsource.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.dockerignore
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/Dockerfile
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/config.json.template
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/docker-compose.yml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/requirements.txt
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/workflows/build_docker_images.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/workflows/update_docker_readme.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/main.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/main_tui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/__main__.py
+-rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/api_helpers.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/conditional_ttl_cache.py
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/config_setup.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/constants.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/dial_client.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/helpers.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/macos_install.py
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/main.py
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/setup-wizard-style.tcss
+-rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/setup_wizard.py
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/ytlounge.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/LICENSE.md
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/README.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/PKG-INFO
```

### Comparing `isponsorblocktv-2.0.6/.pre-commit-config.yaml` & `isponsorblocktv-2.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/Dockerfile` & `isponsorblocktv-2.0.7/Dockerfile`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 # syntax=docker/dockerfile:1
-FROM python:3.11-alpine3.19 as compiler
+FROM python:3.11-alpine3.19 as BASE
+
+FROM base as compiler
 
 WORKDIR /app
 
 COPY src .
 
 RUN python3 -m compileall -b -f . && \
     find . -name "*.py" -type f -delete
 
-FROM python:3.11-alpine3.19
+FROM base as DEP_INSTALLER
+
+COPY requirements.txt .
+
+RUN apk add --no-cache gcc musl-dev && \
+    pip install --upgrade pip wheel && \
+    pip install --user -r requirements.txt && \
+    pip uninstall -y pip wheel && \
+    apk del gcc musl-dev && \
+    python3 -m compileall -b -f /root/.local/lib/python3.11/site-packages && \
+    find /root/.local/lib/python3.11/site-packages -name "*.py" -type f -delete && \
+    find /root/.local/lib/python3.11/ -name "__pycache__" -type d -exec rm -rf {} +
+
+FROM base
 
 ENV PIP_NO_CACHE_DIR=off iSPBTV_docker=True iSPBTV_data_dir=data TERM=xterm-256color COLORTERM=truecolor
 
 COPY requirements.txt .
 
-RUN pip install --upgrade pip wheel && \
-    pip install -r requirements.txt && \
-    pip uninstall -y pip wheel && \
-    python3 -m compileall -b -f /usr/local/lib/python3.11/site-packages && \
-    find /usr/local/lib/python3.11/site-packages -name "*.py" -type f -delete && \
-    find /usr/local/lib/python3.11/ -name "__pycache__" -type d -exec rm -rf {} +
+COPY --from=dep_installer /root/.local /root/.local
 
 WORKDIR /app
 
 COPY --from=compiler /app .
 
 ENTRYPOINT ["python3", "-u", "main.pyc"]
```

### Comparing `isponsorblocktv-2.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `isponsorblocktv-2.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `isponsorblocktv-2.0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/.github/workflows/build_docker_images.yml` & `isponsorblocktv-2.0.7/.github/workflows/build_docker_images.yml`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,14 @@
           username: ${{ github.repository_owner }}
           password: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Build and push
         uses: docker/build-push-action@v4
         with:
           context: .
-          platforms: linux/amd64, linux/arm64
+          platforms: linux/amd64, linux/arm64, linux/arm/v7
           push: ${{ github.event_name != 'pull_request' }}
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
           cache-from: type=registry,ref=ghcr.io/dmunozv04/isponsorblocktv:buildcache
           # Only cache if it's not a pull request
           cache-to: ${{ github.event_name != 'pull_request' && 'type=registry,ref=ghcr.io/dmunozv04/isponsorblocktv:buildcache,mode=max' || '' }}
```

### Comparing `isponsorblocktv-2.0.6/.github/workflows/release_pypi.yml` & `isponsorblocktv-2.0.7/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/.github/workflows/update_docker_readme.yml` & `isponsorblocktv-2.0.7/.github/workflows/update_docker_readme.yml`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/api_helpers.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/api_helpers.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/conditional_ttl_cache.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/conditional_ttl_cache.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/config_setup.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/config_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
 
 import aiohttp
 
 from . import api_helpers, ytlounge
 
 
-async def pair_device():
+async def pair_device(web_session):
     try:
-        lounge_controller = ytlounge.YtLoungeApi("iSponsorBlockTV")
+        lounge_controller = ytlounge.YtLoungeApi(
+            "iSponsorBlockTV", web_session=web_session
+        )
         pairing_code = input(
             "Enter pairing code (found in Settings - Link with TV code): "
         )
         pairing_code = int(
             pairing_code.replace("-", "").replace(" ", "")
         )  # remove dashes and spaces
         print("Pairing...")
@@ -29,14 +31,15 @@
         print(f"Failed to pair device: {e}")
         return
 
 
 def main(config, debug: bool) -> None:
     print("Welcome to the iSponsorBlockTV cli setup wizard")
     loop = asyncio.get_event_loop_policy().get_event_loop()
+    web_session = aiohttp.ClientSession()
     if debug:
         loop.set_debug(True)
     asyncio.set_event_loop(loop)
     if hasattr(config, "atvs"):
         print(
             "The atvs config option is deprecated and has stopped working. Please read"
             " this for more information on how to upgrade to V2:"
@@ -48,15 +51,15 @@
                 " with it present)? (y/n) "
             )
             == "y"
         ):
             del config["atvs"]
     devices = config.devices
     while not input(f"Paired with {len(devices)} Device(s). Add more? (y/n) ") == "n":
-        task = loop.create_task(pair_device())
+        task = loop.create_task(pair_device(web_session))
         loop.run_until_complete(task)
         device = task.result()
         if device:
             devices.append(device)
     config.devices = devices
 
     apikey = config.apikey
@@ -108,15 +111,14 @@
     ):
         if not apikey:
             print(
                 "WARNING: You need to specify an API key to use this function,"
                 " otherwise the program will fail to start.\nYou can add one by"
                 " re-running this setup wizard."
             )
-        web_session = aiohttp.ClientSession()
         api_helper = api_helpers.ApiHelper(config, web_session)
         while True:
             channel_info = {}
             channel = input('Enter a channel name or "/exit" to exit: ')
             if channel == "/exit":
                 break
 
@@ -148,20 +150,20 @@
             if choice == "6":
                 continue
 
             channel_info["id"] = results[int(choice)][0]
             channel_info["name"] = results[int(choice)][1]
             channel_whitelist.append(channel_info)
         # Close web session asynchronously
-        loop.run_until_complete(web_session.close())
 
     config.channel_whitelist = channel_whitelist
 
     config.skip_count_tracking = (
         not input(
             "Do you want to report skipped segments to sponsorblock. Only the segment"
             " UUID will be sent? (y/n) "
         )
         == "n"
     )
     print("Config finished")
     config.save()
+    loop.run_until_complete(web_session.close())
```

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/constants.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/constants.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/dial_client.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/dial_client.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/helpers.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/helpers.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/macos_install.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/macos_install.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/main.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import asyncio
 import logging
 import time
 from signal import SIGINT, SIGTERM, signal
 from typing import Optional
 
 import aiohttp
-import rich
 
-from . import api_helpers, logging_helpers, ytlounge
+from . import api_helpers, ytlounge
 
 
 class DeviceListener:
-    def __init__(self, api_helper, config, device, log_name_len, debug: bool):
+    def __init__(self, api_helper, config, device, debug: bool, web_session):
         self.task: Optional[asyncio.Task] = None
         self.api_helper = api_helper
         self.offset = device.offset
         self.name = device.name
         self.cancelled = False
         self.logger = logging.getLogger(f"iSponsorBlockTV-{device.screen_id}")
+        self.web_session = web_session
         if debug:
             self.logger.setLevel(logging.DEBUG)
         else:
             self.logger.setLevel(logging.INFO)
-        rh = logging_helpers.LogHandler(device.name, log_name_len, level=logging.DEBUG)
-        rh.add_filter_string(device.screen_id)
-        self.logger.addHandler(rh)
+        sh = logging.StreamHandler()
+        sh.setFormatter(
+            logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+        )
+        self.logger.addHandler(sh)
         self.logger.info(f"Starting device")
         self.lounge_controller = ytlounge.YtLoungeApi(
-            device.screen_id, config, api_helper, self.logger
+            device.screen_id, config, api_helper, self.logger, self.web_session
         )
 
     # Ensures that we have a valid auth token
     async def refresh_auth_loop(self):
         while True:
             await asyncio.sleep(60 * 60 * 24)  # Refresh every 24 hours
             try:
@@ -70,15 +72,15 @@
                     await lounge_controller.connect()
                 except:
                     pass
             self.logger.info(
                 "Connected to device %s (%s)", lounge_controller.screen_name, self.name
             )
             try:
-                # print("Subscribing to lounge")
+                self.logger.info("Subscribing to lounge")
                 sub = await lounge_controller.subscribe_monitored(self)
                 await sub
             except:
                 pass
 
     # Method called on playback state change
     async def __call__(self, state):
@@ -149,20 +151,20 @@
     devices = []  # Save the devices to close them later
     if debug:
         loop.set_debug(True)
     asyncio.set_event_loop(loop)
     tcp_connector = aiohttp.TCPConnector(ttl_dns_cache=300)
     web_session = aiohttp.ClientSession(loop=loop, connector=tcp_connector)
     api_helper = api_helpers.ApiHelper(config, web_session)
-    longest_name_len = len(list(sorted([i.name for i in config.devices]))[-1])
     for i in config.devices:
-        device = DeviceListener(api_helper, config, i, longest_name_len, debug)
+        device = DeviceListener(api_helper, config, i, debug, web_session)
         devices.append(device)
         tasks.append(loop.create_task(device.loop()))
         tasks.append(loop.create_task(device.refresh_auth_loop()))
     signal(SIGINT, lambda s, f: loop.stop())
     signal(SIGTERM, lambda s, f: loop.stop())
-    rich.reconfigure(color_system="standard")
     loop.run_forever()
     print("Cancelling tasks and exiting...")
     loop.run_until_complete(finish(devices))
     loop.run_until_complete(web_session.close())
+    loop.run_until_complete(tcp_connector.close())
+    loop.close()
```

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/setup-wizard-style.tcss` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/setup-wizard-style.tcss`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/setup_wizard.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/setup_wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
             self.query_one(".element-name").disabled = False
 
 
 class Device(Element):
     """A device element."""
 
     def process_values_from_data(self):
-        print("HIIII")
         print(self.element_data)
         if "name" in self.element_data and self.element_data["name"]:
             self.element_name = self.element_data["name"]
         else:
             self.element_name = (
                 "Unnamed device with id "
                 f"{self.element_data['screen_id'][:5]}..."
@@ -231,16 +230,16 @@
     """Screen with a dialog to add a device, either with a pairing code or with lan discovery."""
 
     BINDINGS = [("escape", "dismiss({})", "Return")]
 
     def __init__(self, config, **kwargs) -> None:
         super().__init__(**kwargs)
         self.config = config
-        web_session = aiohttp.ClientSession()
-        self.api_helper = api_helpers.ApiHelper(config, web_session)
+        self.web_session = aiohttp.ClientSession()
+        self.api_helper = api_helpers.ApiHelper(config, self.web_session)
         self.devices_discovered_dial = []
 
     def compose(self) -> ComposeResult:
         with Container(id="add-device-container"):
             yield Label("Add Device", classes="title")
             with Grid(id="add-device-switch-buttons"):
                 yield Button(
@@ -333,15 +332,17 @@
             not event.validation_result.is_valid
         )
 
     @on(Input.Submitted, "#pairing-code-input")
     @on(Button.Pressed, "#add-device-pin-add-button")
     async def handle_add_device_pin(self) -> None:
         self.query_one("#add-device-pin-add-button").disabled = True
-        lounge_controller = ytlounge.YtLoungeApi("iSponsorBlockTV")
+        lounge_controller = ytlounge.YtLoungeApi(
+            "iSponsorBlockTV", web_session=self.web_session
+        )
         pairing_code = self.query_one("#pairing-code-input").value
         pairing_code = int(
             pairing_code.replace("-", "").replace(" ", "")
         )  # remove dashes and spaces
         device_name = self.parent.query_one("#device-name-input").value
         paired = False
         try:
```

### Comparing `isponsorblocktv-2.0.6/src/iSponsorBlockTV/ytlounge.py` & `isponsorblocktv-2.0.7/src/iSponsorBlockTV/ytlounge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import asyncio
 import json
 
 import pyytlounge
+from aiohttp import ClientSession
 
 from .constants import youtube_client_blacklist
 
 create_task = asyncio.create_task
 
 
 class YtLoungeApi(pyytlounge.YtLoungeApi):
-    def __init__(self, screen_id, config=None, api_helper=None, logger=None):
+    def __init__(
+        self,
+        screen_id,
+        config=None,
+        api_helper=None,
+        logger=None,
+        web_session: ClientSession = None,
+    ):
         super().__init__("iSponsorBlockTV", logger=logger)
+        if web_session is not None:
+            self.session = web_session  # And use the one we passed
         self.auth.screen_id = screen_id
         self.auth.lounge_id_token = None
         self.api_helper = api_helper
         self.volume_state = {}
         self.subscribe_task = None
         self.subscribe_task_watchdog = None
         self.callback = None
@@ -63,61 +73,61 @@
             # Unmute when the video starts playing
             if self.mute_ads and data["state"] == "1":
                 create_task(self.mute(False, override=True))
         elif event_type == "nowPlaying":
             data = args[0]
             # Unmute when the video starts playing
             if self.mute_ads and data.get("state", "0") == "1":
-                # print("Ad has ended, unmuting")
+                self.logger.info("Ad has ended, unmuting")
                 create_task(self.mute(False, override=True))
         elif event_type == "onAdStateChange":
             data = args[0]
             if data["adState"] == "0":  # Ad is not playing
-                # print("Ad has ended, unmuting")
+                self.logger.info("Ad has ended, unmuting")
                 create_task(self.mute(False, override=True))
             elif (
                 self.skip_ads and data["isSkipEnabled"] == "true"
             ):  # YouTube uses strings for booleans
-                self._logger.info("Ad can be skipped, skipping")
+                self.logger.info("Ad can be skipped, skipping")
                 create_task(self.skip_ad())
                 create_task(self.mute(False, override=True))
             elif (
                 self.mute_ads
             ):  # Seen multiple other adStates, assuming they are all ads
-                self._logger.info("Ad has started, muting")
+                self.logger.info("Ad has started, muting")
                 create_task(self.mute(True, override=True))
         # Manages volume, useful since YouTube wants to know the volume when unmuting (even if they already have it)
         elif event_type == "onVolumeChanged":
             self.volume_state = args[0]
             pass
         # Gets segments for the next video before it starts playing
         elif event_type == "autoplayUpNext":
             if len(args) > 0 and (
                 vid_id := args[0]["videoId"]
             ):  # if video id is not empty
-                print(f"Getting segments for next video: {vid_id}")
+                self.logger.info(f"Getting segments for next video: {vid_id}")
                 create_task(self.api_helper.get_segments(vid_id))
 
         # #Used to know if an ad is skippable or not
         elif event_type == "adPlaying":
             data = args[0]
             # Gets segments for the next video (after the ad) before it starts playing
             if vid_id := data["contentVideoId"]:
-                self._logger.info(f"Getting segments for next video: {vid_id}")
+                self.logger.info(f"Getting segments for next video: {vid_id}")
                 create_task(self.api_helper.get_segments(vid_id))
             elif (
                 self.skip_ads and data["isSkipEnabled"] == "true"
             ):  # YouTube uses strings for booleans
-                self._logger.info("Ad can be skipped, skipping")
+                self.logger.info("Ad can be skipped, skipping")
                 create_task(self.skip_ad())
                 create_task(self.mute(False, override=True))
             elif (
                 self.mute_ads
             ):  # Seen multiple other adStates, assuming they are all ads
-                self._logger.info("Ad has started, muting")
+                self.logger.info("Ad has started, muting")
                 create_task(self.mute(True, override=True))
 
         elif event_type == "loungeStatus":
             data = args[0]
             devices = json.loads(data["devices"])
             for device in devices:
                 if device["type"] == "LOUNGE_SCREEN":
```

### Comparing `isponsorblocktv-2.0.6/.gitignore` & `isponsorblocktv-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/LICENSE.md` & `isponsorblocktv-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/README.md` & `isponsorblocktv-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.6/pyproject.toml` & `isponsorblocktv-2.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iSponsorBlockTV"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
     {"name" = "dmunozv04"}
 ]
 description = "SponsorBlock client for all YouTube TV clients"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `isponsorblocktv-2.0.6/PKG-INFO` & `isponsorblocktv-2.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: iSponsorBlockTV
-Version: 2.0.6
+Version: 2.0.7
 Summary: SponsorBlock client for all YouTube TV clients
 Project-URL: Homepage, https://github.com/dmunozv04/iSponsorBlockTV
 Project-URL: Bug Tracker, https://github.com/dmunozv04/iSponsorBlockTV/issues
 Author: dmunozv04
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.7
-Requires-Dist: aiohttp==3.9.0
+Requires-Dist: aiohttp==3.9.5
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: argparse==1.4.0
 Requires-Dist: async-cache==1.1.1
-Requires-Dist: pyytlounge==1.6.3
-Requires-Dist: rich==13.6.0
+Requires-Dist: pyytlounge==2.0.0
+Requires-Dist: rich==13.7.1
 Requires-Dist: ssdp==1.3.0
 Requires-Dist: textual-slider==0.1.1
-Requires-Dist: textual==0.40.0
+Requires-Dist: textual==0.58.0
 Requires-Dist: xmltodict==0.13.0
 Description-Content-Type: text/markdown
 
 # iSponsorBlockTV
 Skip sponsor segments in YouTube videos playing on a YouTube TV device (see below for compatibility details).
 
 This project is written in asynchronous python and should be pretty quick.
```

