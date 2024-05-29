# Comparing `tmp/cto_cli-0.2.0.tar.gz` & `tmp/cto_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cto_cli-0.2.0.tar", max compression
+gzip compressed data, was "cto_cli-0.3.0.tar", max compression
```

## Comparing `cto_cli-0.2.0.tar` & `cto_cli-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-05-03 11:11:03.634479 cto_cli-0.2.0/LICENSE
--rw-r--r--   0        0        0      233 2024-05-03 11:11:03.634479 cto_cli-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/api/__init__.py
--rw-r--r--   0        0        0     7715 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/api/connector.py
--rw-r--r--   0        0        0        0 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/commands/__init__.py
--rw-r--r--   0        0        0     3273 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/commands/config.py
--rw-r--r--   0        0        0     2047 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/commands/users.py
--rw-r--r--   0        0        0        0 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/__init__.py
--rw-r--r--   0        0        0      451 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/commands.py
--rw-r--r--   0        0        0     6279 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/files.py
--rw-r--r--   0        0        0     7277 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/operations.py
--rw-r--r--   0        0        0     3068 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/settings.py
--rw-r--r--   0        0        0     1832 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/validators.py
--rw-r--r--   0        0        0     3778 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/main.py
--rw-r--r--   0        0        0      652 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/main.py
--rw-r--r--   0        0        0      213 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/utils/errors.py
--rw-r--r--   0        0        0     1580 2024-05-03 11:11:04.342481 cto_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 cto_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 09:42:10.999284 cto_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0      233 2024-05-29 09:42:10.999284 cto_cli-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/api/__init__.py
+-rw-r--r--   0        0        0     8748 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/api/connector.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/commands/__init__.py
+-rw-r--r--   0        0        0     4043 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/commands/config.py
+-rw-r--r--   0        0        0     2046 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/commands/users.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/__init__.py
+-rw-r--r--   0        0        0      451 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/commands.py
+-rw-r--r--   0        0        0     7333 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/files.py
+-rw-r--r--   0        0        0     7384 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/operations.py
+-rw-r--r--   0        0        0     3266 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/settings.py
+-rw-r--r--   0        0        0     1832 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/validators.py
+-rw-r--r--   0        0        0     3779 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/main.py
+-rw-r--r--   0        0        0      652 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/main.py
+-rw-r--r--   0        0        0      213 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/utils/errors.py
+-rw-r--r--   0        0        0     1580 2024-05-29 09:42:11.931291 cto_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 cto_cli-0.3.0/PKG-INFO
```

### Comparing `cto_cli-0.2.0/LICENSE` & `cto_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cto_cli-0.2.0/cto_cli/ecs/api/connector.py` & `cto_cli-0.3.0/cto_cli/ecs/api/connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,23 @@
         self._url = url
 
         if load_settings:
             self._set_api_details()
 
     @staticmethod
     def _handle_error_response(error: requests.exceptions.HTTPError):
+        if error.response.status_code == 422:
+            try:
+                error = [detail['msg'] for detail in error.response.json()['detail']]
+            except Exception:
+                pass
+            else:
+                if len(error) == 1:
+                    error = error[0]
+                print_error(error, exit=True)
         try:
             print_error(f'{error.response.json()["detail"]}', exit=True)
         except Exception:
             print_error(f'{error.response.text}', exit=True)
 
     def _handle_response(self, response: requests.Response) -> None:
         try:
@@ -60,15 +69,15 @@
     def _print_response(response: requests.Response) -> None:
         if response.headers['content-type'] == 'application/json':
             response_json = response.json()
             print_json(data=response_json)
         elif response.headers['content-type'] == 'application/yaml':
             print(Syntax(response.text, 'yaml'))
         else:
-            print(response.text)
+            print(Syntax(response.text, 'text'))
 
     def _make_request(
         self,
         method: str,
         url: str,
         headers: dict | None = None,
         json: dict | None = None,
@@ -169,22 +178,25 @@
     def get_config_hashes(self) -> dict[str, Any]:
         response = self._make_request('get', 'config/hashes')
         self._handle_response(response)
 
         return response.json()
 
     def push_config_changes(
-        self, file_with_changes: BytesIO, deleted_files: list[str], commit_hash: str
+        self, file_with_changes: BytesIO, deleted_files: list[str], commit_hash: str, tag: str | None = None
     ) -> None | dict:
         response = self._make_request(
             'post',
             'config',
             headers={'commit-hash': commit_hash},
             files={'file': file_with_changes},
-            data={'deleted_files': deleted_files},
+            data={
+                'deleted_files': deleted_files,
+                **({'tag': tag} if tag else {}),
+            },
         )
 
         self._handle_response(response)
 
         response_json = response.json()
         print_json(data=response_json)
 
@@ -192,33 +204,47 @@
 
     def build_config(
         self,
         path: str | Path,
         strategy_name: str | None = None,
         recursive: bool = False,
         show_secrets: bool = False,
+        config_id: str | None = None,
+        detect_drift: bool = False,
         format: str | None = None,
         filter: str | None = None,
     ):
         response = self._make_request(
             'post',
             'config/build',
             json={
                 'path': path,
                 'recursive': recursive,
                 **({'show_secrets': show_secrets} if show_secrets else {}),
                 **({'strategy_name': strategy_name} if strategy_name else {}),
                 **({'format': format} if format else {}),
                 **({'filter': filter} if filter else {}),
+                **({'config_id': config_id} if config_id else {}),
+                **({'detect_drift': detect_drift} if detect_drift else {}),
             },
         )
 
         self._handle_response(response)
         self._print_response(response)
 
+    def generate_schema(self, path: str | Path, strategy_name: str, write: bool = False):
+        response = self._make_request(
+            'post',
+            'config/generate_schema',
+            json={'path': path, 'strategy_name': strategy_name, 'write': write},
+        )
+
+        self._handle_response(response)
+        self._print_response(response)
+
     def decrypt_file(
         self,
         path: str | Path,
     ):
         response = self._make_request(
             'post',
             'config/decrypt',
```

### Comparing `cto_cli-0.2.0/cto_cli/ecs/commands/config.py` & `cto_cli-0.3.0/cto_cli/ecs/commands/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 from cto_cli.ecs.local.settings import (
     validate_workdir_in_ecs_repo_path,
     get_ecs_path,
 )
 from cto_cli.ecs.local.validators import check_versions_compatibility
 from cto_cli.utils.errors import print_error
+from rich.progress import Progress, SpinnerColumn, TextColumn
 
 app = typer.Typer(callback=check_versions_compatibility)
 
 
 def pull_remote_repo(
     api_connector: APIConnector, show_status: bool = True, update_type: HashTypeUpdate = HashTypeUpdate.CURRENT
 ) -> None:
@@ -47,22 +48,22 @@
 @validate_workdir_in_ecs_repo_path
 def pull() -> None:
     pull_remote_repo(APIConnector())
 
 
 @app.command(name='push')
 @validate_workdir_in_ecs_repo_path
-def push() -> None:
+def push(tag: Annotated[str, typer.Option()] = None) -> None:
     api_connector = APIConnector()
 
     repo_hashes = api_connector.get_config_hashes()
     if is_repo_update_needed(repo_hashes):
         print_error('[red]Repo is not up-to-date, run [b]cto ecs config pull[/b] to update[/red]', exit=True)
 
-    server_modified_files = handle_config_push(api_connector)
+    server_modified_files = handle_config_push(api_connector, tag)
     pull_remote_repo(api_connector, show_status=False, update_type=HashTypeUpdate.BOTH)
     if server_modified_files:
         update_server_modified_files(server_modified_files)
 
 
 def validate_strategy_name(value: str):
     if value is None or len(value) < 2:
@@ -72,35 +73,52 @@
 
 @app.command(name='build')
 def build(
     path: Annotated[str, typer.Option()],
     strategy_name: Annotated[str, typer.Option()] = None,
     format: Annotated[str, typer.Option()] = None,
     filter: Annotated[str, typer.Option(help='filter result using JMESPath')] = None,
+    config_id: Annotated[str, typer.Option()] = None,
+    detect_drift: bool = False,
     recursive: bool = False,
     show_secrets: bool = False,
 ) -> None:
     if strategy_name:
         validate_strategy_name(strategy_name)
 
     APIConnector().build_config(
         path=path,
         strategy_name=strategy_name,
         format=format,
         filter=filter,
         recursive=recursive,
         show_secrets=show_secrets,
+        config_id=config_id,
+        detect_drift=detect_drift,
     )
 
 
 @app.command(name='decrypt')
 def decrypt(path: Annotated[str, typer.Option()]) -> None:
     APIConnector().decrypt_file(path)
 
 
+@app.command(name='generate-schema')
+def generate_schema(
+    path: Annotated[str, typer.Option()], strategy_name: Annotated[str, typer.Option()], write: bool = False
+) -> None:
+    with Progress(
+        SpinnerColumn(),
+        TextColumn('[progress.description]{task.description}'),
+        transient=True,
+    ) as progress:
+        progress.add_task(description='AI is generating schema for you...', total=None)
+        APIConnector().generate_schema(path=path, strategy_name=strategy_name, write=write)
+
+
 @app.command(name='status')
 @validate_workdir_in_ecs_repo_path
 def status() -> None:
     modified_files = FilesHandler().modified_files
 
     if not modified_files.has_changes():
         print('[green]No modified files[/green]')
```

### Comparing `cto_cli-0.2.0/cto_cli/ecs/commands/users.py` & `cto_cli-0.3.0/cto_cli/ecs/commands/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from enum import Enum
 
 if sys.version_info < (3, 11):
     from typing_extensions import Annotated
 else:
     from typing import Annotated
 
-
 import typer
 from rich.prompt import Confirm
 
 from cto_cli.ecs.api.connector import APIConnector
 from cto_cli.ecs.local.settings import get_current_working_dir_relative_path_to_ecs_repo
 from cto_cli.ecs.local.validators import check_versions_compatibility
```

### Comparing `cto_cli-0.2.0/cto_cli/ecs/local/files.py` & `cto_cli-0.3.0/cto_cli/ecs/local/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 import base64
 import io
 import json
+import yaml
+from yaml import YAMLError
 import os
 import shutil
 import zipfile
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Sequence, Any
 
 from cto_cli.ecs.local.commands import run_command
 from cto_cli.ecs.local.settings import get_repo_path, get_hashes_path
 from cto_cli.utils.errors import print_error
 
 EXCLUDED_PATHS = ['*.idea/*', '*.git/*', '*.vscode/*']
+EXTENSIONS_TO_VALIDATE = ['.json', '.yaml', '.yml']
 
 
 class HashTypeUpdate:
     CURRENT = 'current'
     BOTH = 'both'
 
 
@@ -168,7 +171,30 @@
         except zipfile.BadZipFile:
             with open(remote_zip_path, 'rb') as file:
                 data = file.read()
                 decoded_data = base64.b64decode(data)
 
                 with zipfile.ZipFile(io.BytesIO(decoded_data), 'r') as zip_file:
                     zip_file.extractall(path=extract_path)
+
+    @staticmethod
+    def validate_files(file_paths: list[str]):
+        invalid_files = []
+
+        for file_path in file_paths:
+            for extension_to_validate in EXTENSIONS_TO_VALIDATE:
+                if file_path.endswith(extension_to_validate):
+                    with open(file_path) as f:
+                        try:
+                            content = yaml.safe_load(f)
+                        except YAMLError:
+                            invalid_files.append(file_path)
+
+                        if not isinstance(content, (dict, list)):
+                            print_error(
+                                f'Validation failed for file: [b]{file_path}[/b] ECS supports only JSONs|YAMLs that are an array '
+                                f'or an object',
+                                exit=True,
+                            )
+
+        if invalid_files:
+            print_error(f'These files contain errors: {invalid_files}', exit=True)
```

### Comparing `cto_cli-0.2.0/cto_cli/ecs/local/operations.py` & `cto_cli-0.3.0/cto_cli/ecs/local/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,24 +138,26 @@
     if stash:
         run_command(f'git stash apply {stash} && git stash drop {stash}')
 
         if commit:
             run_command('git commit -a -m "changes before push"')
 
 
-def handle_config_push(api_connector: APIConnector) -> Optional[list[str]]:
+def handle_config_push(api_connector: APIConnector, tag: str | None = None) -> Optional[list[str]]:
     _restore_and_delete_stash()
 
     commit_hash = FilesHandler.get_stored_remote_hashes()['current']['repo_hash']
     modified_files = FilesHandler().modified_files
 
     if not modified_files.has_changes():
         print('[yellow]There is nothing to be pushed[/yellow]')
         sys.exit(0)
 
+    FilesHandler.validate_files(modified_files.get_added_or_updated_paths())
+
     show_modified_local_files(modified_files)
 
     if modified_files.modified_only_locally:
         full_path_files = [
             str(get_repo_path() / modified_file) for modified_file in modified_files.modified_only_locally
         ]
         run_command(f'git stash push -m {STASH_NAME} -- {" ".join(full_path_files)}')
@@ -184,15 +186,15 @@
         _merge_remote_branch()
 
     _restore_and_delete_stash(commit=True)
     zipped_local_changes = FilesHandler.zip_paths(
         modified_files.get_added_or_updated_paths(), root_path=get_repo_path()
     )
 
-    response = api_connector.push_config_changes(zipped_local_changes, modified_files.deleted, commit_hash)
+    response = api_connector.push_config_changes(zipped_local_changes, modified_files.deleted, commit_hash, tag)
 
     if response and (skipped_files := response.get('skipped_files')):
         skipped_files_json = json.dumps(skipped_files, indent=4)
         delete_files = Confirm.ask(
             f"These paths were skipped on ecs push as you haven't been authed against them: "
             f'[yellow]{skipped_files_json}[/yellow]\n Do you want to [red]delete[/red] them?'
         )
```

### Comparing `cto_cli-0.2.0/cto_cli/ecs/local/settings.py` & `cto_cli-0.3.0/cto_cli/ecs/local/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-import sys
 import os
 import json
 from dataclasses import dataclass
 from functools import wraps
 from pathlib import Path
 from cto_cli.utils.errors import print_error
+from json.decoder import JSONDecodeError
 
 CTO_DIR = Path.home() / '.cto'
 ECS_SETTINGS_LOCATION = CTO_DIR / 'ecs_settings.json'
 
 
 class SettingsNotFound(Exception):
     pass
@@ -30,29 +30,32 @@
     @classmethod
     def load_from_env(cls) -> ECSSettings:
         try:
             return cls(
                 url=os.environ['ECS_URL'],
                 token=os.environ['ECS_TOKEN'],
                 ecs_path=os.environ['ECS_LOCAL_PATH'],
-                saas_token=os.getenv('ECS_SAAS_TOKEN')
+                saas_token=os.getenv('ECS_SAAS_TOKEN'),
             )
         except KeyError:
             raise EnvSettingsNotFound
 
 
 def load_ecs_settings() -> ECSSettings:
     try:
         return ECSSettings.load_from_env()
     except EnvSettingsNotFound:
         pass
 
     try:
         with open(ECS_SETTINGS_LOCATION, 'r') as f:
-            return ECSSettings(**json.load(f))
+            try:
+                return ECSSettings(**json.load(f))
+            except JSONDecodeError:
+                print_error('Your ECS settings file is corrupted', exit=True)
     except FileNotFoundError:
         raise SettingsNotFound
 
 
 def get_ecs_path() -> Path:
     try:
         return Path(load_ecs_settings().ecs_path)
@@ -83,15 +86,17 @@
     get_repo_path().mkdir(parents=True, exist_ok=True)
 
 
 def store_settings(url: str, token: str, saas_token: None | str = None) -> None:
     CTO_DIR.mkdir(parents=True, exist_ok=True)
 
     with open(ECS_SETTINGS_LOCATION, 'w') as f:
-        f.write(json.dumps({'token': token, 'url': url, 'saas_token': saas_token, 'ecs_path': str(WORKING_DIR)}))
+        f.write(
+            json.dumps({'token': token, 'url': url, 'saas_token': saas_token, 'ecs_path': str(WORKING_DIR)}, indent=4)
+        )
 
 
 def _validate_workdir_in_ecs_repo_path():
     ecs_repo_path = get_repo_path()
 
     try:
         WORKING_DIR.relative_to(Path(ecs_repo_path))
```

### Comparing `cto_cli-0.2.0/cto_cli/ecs/local/validators.py` & `cto_cli-0.3.0/cto_cli/ecs/local/validators.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.2.0/cto_cli/ecs/main.py` & `cto_cli-0.3.0/cto_cli/ecs/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     saas_token = None
 
     saas = typer.confirm(
         'If you\'re using ECS Cloud type Y, if you\'re using your own on-prem ECS server, type N', abort=False
     )
     if saas:
         saas_token = typer.prompt(
-            "What's your ECS SaaS token?", default=settings.saas_token if settings and settings.saas_token else None
+            "What's your ECS Cloud token?", default=settings.saas_token if settings and settings.saas_token else None
         )
         api_url = 'https://api.enterpriseconfigurationservice.com'
         api_connector = APIConnector(
             load_settings=False, url=api_url, headers={'Authorization': 'very_first_user', 'x-saas-token': saas_token}
         )
     else:
         api_url = typer.prompt("What's the API url?", default=settings.url if settings else None)
```

### Comparing `cto_cli-0.2.0/cto_cli/main.py` & `cto_cli-0.3.0/cto_cli/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.2.0/pyproject.toml` & `cto_cli-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cto-cli"
-version = "0.2.0"
+version = "0.3.0"
 description = "The CTO cli"
 authors = ["CTO <support@cloudtechnologyoffice.com>"]
 readme = "README.md"
 homepage = "https://doc.cloudtechnologyoffice.com/ecs/latest"
 repository = "https://github.com/Cloud-Technology-Office/cto-cli"
 license = "Apache-2.0"
```

### Comparing `cto_cli-0.2.0/PKG-INFO` & `cto_cli-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cto-cli
-Version: 0.2.0
+Version: 0.3.0
 Summary: The CTO cli
 Home-page: https://doc.cloudtechnologyoffice.com/ecs/latest
 License: Apache-2.0
 Author: CTO
 Author-email: support@cloudtechnologyoffice.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

