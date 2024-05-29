# Comparing `tmp/dt_extension_migrator-0.1.0.tar.gz` & `tmp/dt_extension_migrator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt_extension_migrator-0.1.0.tar", max compression
+gzip compressed data, was "dt_extension_migrator-0.1.1.tar", max compression
```

## Comparing `dt_extension_migrator-0.1.0.tar` & `dt_extension_migrator-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-24 16:54:43.631910 dt_extension_migrator-0.1.0/dt_extension_migrator/__init__.py
--rw-r--r--   0        0        0     8330 2024-05-24 17:34:46.545410 dt_extension_migrator-0.1.0/dt_extension_migrator/extension_apps/remote_unix.py
--rw-r--r--   0        0        0     1882 2024-05-24 17:12:32.055935 dt_extension_migrator-0.1.0/dt_extension_migrator/main.py
--rw-r--r--   0        0        0      467 2024-05-24 17:01:33.273598 dt_extension_migrator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      132 2024-05-24 17:00:30.549928 dt_extension_migrator-0.1.0/README.md
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 dt_extension_migrator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-24 16:54:43.631910 dt_extension_migrator-0.1.1/dt_extension_migrator/__init__.py
+-rw-r--r--   0        0        0    10649 2024-05-28 20:11:35.117069 dt_extension_migrator-0.1.1/dt_extension_migrator/extension_apps/__pycache__/generic_commands.cpython-312.pyc
+-rw-r--r--   0        0        0     9327 2024-05-28 20:16:59.047319 dt_extension_migrator-0.1.1/dt_extension_migrator/extension_apps/__pycache__/remote_unix.cpython-312.pyc
+-rw-r--r--   0        0        0    11173 2024-05-28 20:19:20.898262 dt_extension_migrator-0.1.1/dt_extension_migrator/extension_apps/generic_commands.py
+-rw-r--r--   0        0        0     9107 2024-05-28 20:19:29.036170 dt_extension_migrator-0.1.1/dt_extension_migrator/extension_apps/remote_unix.py
+-rw-r--r--   0        0        0     2178 2024-05-28 20:19:34.702241 dt_extension_migrator-0.1.1/dt_extension_migrator/main.py
+-rw-r--r--   0        0        0      467 2024-05-28 20:21:15.018130 dt_extension_migrator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2325 2024-05-28 17:45:18.854121 dt_extension_migrator-0.1.1/README.md
+-rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 dt_extension_migrator-0.1.1/PKG-INFO
```

### Comparing `dt_extension_migrator-0.1.0/dt_extension_migrator/extension_apps/remote_unix.py` & `dt_extension_migrator-0.1.1/dt_extension_migrator/extension_apps/remote_unix.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from rich import print
 
 import json
 from typing import Optional, List
 
 app = typer.Typer()
 
+EF1_EXTENSION_ID = "custom.remote.python.remote_agent"
+EF2_EXTENSION_ID = "com.dynatrace.extension.remote-unix"
+
 
 def build_authentication_from_ef1(ef1_config: dict):
     authentication = {"username": ef1_config.get("username")}
 
     password = ef1_config.get("password")
     ssh_key_contents = ef1_config.get("ssh_key_contents")
     ssh_key_file = ef1_config.get("ssh_key_file")
@@ -80,15 +83,17 @@
         "enabled": False,
         "description": description,
         "version": version,
         "featureSets": ["default"],
         "pythonRemote": {"endpoints": []},
     }
 
-    print(f"{len(ef1_configurations)} endpoints will attempt to be added to the monitoring configuration.")
+    print(
+        f"{len(ef1_configurations)} endpoints will attempt to be added to the monitoring configuration."
+    )
     for index, row in ef1_configurations.iterrows():
         enabled = row["enabled"]
         properties: dict = json.loads(row["properties"])
         endpoint_configuration = {
             "enabled": enabled,
             "hostname": properties.get("hostname"),
             "port": int(properties.get("port")),
@@ -154,73 +159,96 @@
                 )
 
         base_config["pythonRemote"]["endpoints"].append(endpoint_configuration)
 
     return base_config
 
 
-@app.command()
+@app.command(help="Pull EF1 remote unix configurations into a spreadsheet.")
 def pull(
     dt_url: Annotated[str, typer.Option(envvar="DT_URL")],
     dt_token: Annotated[str, typer.Option(envvar="DT_TOKEN")],
-    output_file: Optional[str] = None,
-    index: Optional[List[str]] = ["group"],
+    output_file: Optional[str] = None or f"{EF1_EXTENSION_ID}.xlsx",
+    index: Annotated[
+        Optional[List[str]],
+        typer.Option(
+            help="Specify what property to group sheets by. Can be specified multipl times."
+        ),
+    ] = ["group"],
 ):
     dt = Dynatrace(dt_url, dt_token)
-    configs = dt.extensions.list_instances(
-        extension_id="custom.remote.python.remote_agent"
-    )
+    configs = dt.extensions.list_instances(extension_id=EF1_EXTENSION_ID)
     full_configs = []
 
     for config in track(configs, description="Pulling EF1 configs"):
-        config = config.get_full_configuration("custom.remote.python.remote_agent")
+        config = config.get_full_configuration(EF1_EXTENSION_ID)
         full_config = config.json()
         properties = full_config.get("properties", {})
         for key in properties:
             if key in index or key == "username":
                 full_config.update({key: properties[key]})
         full_config["properties"] = json.dumps(properties)
         full_configs.append(full_config)
 
     writer = pd.ExcelWriter(
-        output_file or f"custom.remote.python.remote_agent-export.xlsx",
+        output_file,
         engine="xlsxwriter",
     )
     df = pd.DataFrame(full_configs)
     df_grouped = df.groupby(index)
     for key, group in df_grouped:
         key = [subgroup for subgroup in key if subgroup]
         group.to_excel(
             writer, sheet_name="-".join(key) or "Default", index=False, header=True
         )
     writer.close()
+    print(f"Exported configurations available in '{output_file}'")
 
 
 @app.command()
 def push(
     dt_url: Annotated[str, typer.Option(envvar="DT_URL")],
     dt_token: Annotated[str, typer.Option(envvar="DT_TOKEN")],
-    input_file: Annotated[str, typer.Option()],
-    sheet: Annotated[str, typer.Option()],
+    input_file: Annotated[
+        str,
+        typer.Option(
+            help="The location of a previously pulled/exported list of EF1 endpoints"
+        ),
+    ],
+    sheet: Annotated[
+        str,
+        typer.Option(
+            help="The name of a sheet in a previously pulled/exported list of EF1 endpoints"
+        ),
+    ],
     ag_group: Annotated[str, typer.Option()],
-    version: Annotated[str, typer.Option()],
+    version: Annotated[
+        str,
+        typer.Option(
+            help="The version of the EF2 extension you would look to create this configuration for"
+        ),
+    ],
     skip_endpoint_auth: Annotated[bool, typer.Option()] = False,
     enabled: Annotated[bool, typer.Option()] = False,
 ):
     xls = pd.ExcelFile(input_file)
     df = pd.read_excel(xls, sheet)
 
     config = build_ef2_config_from_ef1(version, sheet, False, df)
 
     dt = Dynatrace(dt_url, dt_token, print_bodies=False)
     config = MonitoringConfigurationDto(ag_group, config)
     try:
-        result = dt.extensions_v2.post_monitoring_configurations("custom:remote-unix", [config])[0]
+        result = dt.extensions_v2.post_monitoring_configurations(
+            EF2_EXTENSION_ID, [config]
+        )[0]
         print(f"Configs created successfully. Response: {result['code']}")
         base_url = dt_url if not dt_url.endswith("/") else dt_url[:-1]
-        print(f"Link to monitoring configuration: {base_url}/ui/hub/ext/listing/registered/custom:remote-unix/{result['objectId']}/read")
+        print(
+            f"Link to monitoring configuration: {base_url}/ui/hub/ext/listing/registered/{EF2_EXTENSION_ID}/{result['objectId']}/read"
+        )
     except Exception as e:
         print(f"[bold red]{e}[/bold red]")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `dt_extension_migrator-0.1.0/dt_extension_migrator/main.py` & `dt_extension_migrator-0.1.1/dt_extension_migrator/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+import dt_extension_migrator.extension_apps.generic_commands
 import typer
 from typing_extensions import Annotated
 from dynatrace import Dynatrace
 import pandas
+from rich import print
 
 from typing import Optional
 import json
 
 import dt_extension_migrator.extension_apps.remote_unix
 
 app = typer.Typer()
 app.add_typer(dt_extension_migrator.extension_apps.remote_unix.app, name="remote-unix")
+app.add_typer(
+    dt_extension_migrator.extension_apps.generic_commands.app, name="generic-commands"
+)
 
 SUPPORTED_EF1_EXTENSION_MAPPINGS = {
-    "custom.remote.python.remote_agent": "com.dynatrace.extension.remote-unix"
+    "custom.remote.python.remote_agent": "com.dynatrace.extension.remote-unix",
+    "custom.remote.python.generic_linux_commands": "custom:generic-commands",
 }
 
 
 @app.command()
-def export__generic_configs(
+def export_generic_configs(
     dt_url: Annotated[str, typer.Option(envvar="DT_URL")],
     dt_token: Annotated[str, typer.Option(envvar="DT_TOKEN")],
     extension_id: Annotated[str, typer.Option()],
     output_file: Optional[str] = None,
     index: Optional[str] = "group",
 ):
     dt = Dynatrace(dt_url, dt_token)
@@ -30,28 +36,27 @@
     for config in configs:
         config = config.get_full_configuration(extension_id)
         full_config = config.json()
         properties = full_config.get("properties", {})
         for key in properties:
             if (key in index) or (key == "username"):
                 full_config.update({key: properties[key]})
-        full_config['properties'] = json.dumps(properties)
+        full_config["properties"] = json.dumps(properties)
         full_configs.append(full_config)
 
     writer = pandas.ExcelWriter(
         output_file or f"{extension_id}-export.xlsx", engine="xlsxwriter"
     )
     df = pandas.DataFrame(full_configs)
     df_grouped = df.groupby(index)
     for key, group in df_grouped:
         group.to_excel(writer, sheet_name=key or "Default", index=False, header=True)
     writer.close()
 
     if extension_id not in SUPPORTED_EF1_EXTENSION_MAPPINGS:
         print(
-            f"WARNING - {extension_id} is not an extension currently supported for migration!!!"
+            f"[bold yellow]WARNING - {extension_id} is not an extension currently supported for migrationl.[/bold yellow]"
         )
 
 
-
 if __name__ == "__main__":
     app()
```

