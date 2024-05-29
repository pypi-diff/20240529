# Comparing `tmp/morphdb_utils-0.2.0.tar.gz` & `tmp/morphdb_utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphdb_utils-0.2.0.tar", max compression
+gzip compressed data, was "morphdb_utils-0.2.1.tar", max compression
```

## Comparing `morphdb_utils-0.2.0.tar` & `morphdb_utils-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      139 2024-05-02 05:57:33.266613 morphdb_utils-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.0/morphdb_utils/__init__.py
--rw-r--r--   0        0        0     3525 2024-05-23 03:47:31.584379 morphdb_utils-0.2.0/morphdb_utils/annotations.py
--rw-r--r--   0        0        0    14463 2024-05-28 04:13:08.806521 morphdb_utils-0.2.0/morphdb_utils/api.py
--rw-r--r--   0        0        0      426 2024-05-02 05:57:33.264995 morphdb_utils-0.2.0/morphdb_utils/logging.py
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.0/morphdb_utils/py.typed
--rw-r--r--   0        0        0     1616 2024-05-02 05:57:33.265180 morphdb_utils-0.2.0/morphdb_utils/type.py
--rw-r--r--   0        0        0      803 2024-05-28 04:18:21.383600 morphdb_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 morphdb_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      396 2024-05-28 08:58:13.260511 morphdb_utils-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.1/morphdb_utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-05-28 08:55:19.780238 morphdb_utils-0.2.1/morphdb_utils/annotations.py
+-rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.1/morphdb_utils/api.py
+-rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.1/morphdb_utils/logging.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.1/morphdb_utils/py.typed
+-rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.1/morphdb_utils/type.py
+-rw-r--r--   0        0        0      824 2024-05-29 09:10:08.743606 morphdb_utils-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 morphdb_utils-0.2.1/PKG-INFO
```

### Comparing `morphdb_utils-0.2.0/morphdb_utils/annotations.py` & `morphdb_utils-0.2.1/morphdb_utils/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-import os
-import io
 import base64
+import io
+import os
 from typing import Literal
 
-import pandas as pd  # type: ignore
 import matplotlib.figure  # type: ignore
+import pandas as pd  # type: ignore
 import plotly  # type: ignore
-import plotly.io as pio # type: ignore
-
+import plotly.io as pio  # type: ignore
 
 # enum type: export format
 VISUALIZATION_FORMAT = Literal["png", "html"]
 
 
-def _get_html_from_mpl_image(fig: matplotlib.figure.Figure, format: VISUALIZATION_FORMAT = "html") -> str:
+def _get_html_from_mpl_image(
+    fig: matplotlib.figure.Figure, format: VISUALIZATION_FORMAT = "html"
+) -> str:
     buf = io.BytesIO()
     fig.savefig(buf, format="png")
     buf.seek(0)
     if format == "png":
         # return in base64 encoded png format
         return base64.b64encode(buf.read()).decode()
     elif format == "html":
-        return (
-            f'<img src="data:image/png;base64,{base64.b64encode(buf.read()).decode()}" />'
-        )
+        return f'<img src="data:image/png;base64,{base64.b64encode(buf.read()).decode()}" />'
 
 
 def _get_html_from_plotly_image(fig, format: VISUALIZATION_FORMAT = "html") -> str:
     if format == "png":
         pio.kaleido.scope.chromium_args += ("--single-process",)
         buf = io.BytesIO()
         fig.write_image(buf, format="png")
```

### Comparing `morphdb_utils-0.2.0/morphdb_utils/api.py` & `morphdb_utils-0.2.1/morphdb_utils/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 from __future__ import annotations
 
 import io
+import json
 import os
 import urllib.parse
-from morphdb_utils.type import LoadDataParams, RefResponse, SignedUrlResponse, SqlResultResponse
+from typing import Dict, Optional, Tuple
 
 import pandas as pd
 import requests
-from requests.exceptions import Timeout
 import urllib3
+from requests.exceptions import Timeout
 from urllib3.exceptions import InsecureRequestWarning
-from typing import Optional
+
+from morphdb_utils.type import (
+    LoadDataParams,
+    Protocol,
+    RefResponse,
+    SignedUrlResponse,
+    SqlResultResponse,
+)
 
 urllib3.disable_warnings(InsecureRequestWarning)
 
 
 class MorphApiError(Exception):
     pass
 
 
 def _handle_morph_response(response: requests.Response):
     if response.status_code != 200:
         raise MorphApiError(response.text)
     response_json = response.json()
-    if "error" in response_json and "subCode" in response_json and "message" in response_json:
+    if (
+        "error" in response_json
+        and "subCode" in response_json
+        and "message" in response_json
+    ):
         error_message = response_json["message"]
         if response_json["error"] == "internal_server_error":
-            error_message = "System internal server error occurred. Please try again later."
+            error_message = (
+                "System internal server error occurred. Please try again later."
+            )
         if response_json["error"] == "notebook_error":
             if response_json["subCode"] == 2:
                 error_message = "Reference cell not found. Please check the cell name and try again."
         if response_json["error"] == "storage_error":
             if response_json["subCode"] == 4:
                 error_message = "Could not find data in the reference cell. Please check if the reference cell was executed successfully and retrieved the result correctly, and try again."
         if response_json["error"] == "template_error":
@@ -40,26 +54,25 @@
                 error_message = "The auth token connecting external source has been expired. Please authorize the connector and try again."
         if response_json["error"] == "external_connection_error":
             if response_json["subCode"] == 1:
                 error_message = "The connector not found. Please check if the connector exists and try again."
         raise MorphApiError(error_message)
     return response_json
 
+
 def _read_configuration_from_env() -> dict[str, str]:
     config = {}
     if "MORPH_DATABASE_ID" in os.environ:
         config["database_id"] = os.environ["MORPH_DATABASE_ID"]
     if "MORPH_BASE_URL" in os.environ:
         config["base_url"] = os.environ["MORPH_BASE_URL"]
     if "MORPH_TEAM_SLUG" in os.environ:
         config["team_slug"] = os.environ["MORPH_TEAM_SLUG"]
-    if "MORPH_AUTHORIZATION" in os.environ:
-        config["authorization"] = os.environ["MORPH_AUTHORIZATION"]
-    if "MORPH_NOTEBOOK_ID" in os.environ:
-        config["notebook_id"] = os.environ["MORPH_NOTEBOOK_ID"]
+    if "MORPH_API_KEY" in os.environ:
+        config["api_key"] = os.environ["MORPH_API_KEY"]
 
     return config
 
 
 def _canonicalize_base_url(base_url: str) -> str:
     if base_url.startswith("http"):
         return base_url
@@ -123,209 +136,218 @@
         parsed_rows.append(parsed_row)
     return pd.DataFrame.from_dict(parsed_rows)
 
 
 def _convert_signed_url_response_to_dateframe(
     response: SignedUrlResponse,
 ) -> pd.DataFrame:
-    ext = response.url.split(".")[-1].split("?")[0]
+    ext = response.url.split("?")[0].split("/")[-1].split(".")[-1]
     r = requests.get(response.url)
 
     if ext == "csv":
         chunks = []
         for chunk in pd.read_csv(
             io.BytesIO(r.content),
             header=0,
             chunksize=1_000_000,
             encoding_errors="replace",
         ):
             chunks.append(chunk)
         df = pd.concat(chunks, axis=0)
     else:
         if ext.endswith(".xls"):
-            df = pd.read_excel(io.BytesIO(r.content), engine="xlrd", header=0, sheet_name=0)
+            df = pd.read_excel(
+                io.BytesIO(r.content), engine="xlrd", header=0, sheet_name=0
+            )
         else:
-            df = pd.read_excel(io.BytesIO(r.content), engine="openpyxl", header=0, sheet_name=0)
+            df = pd.read_excel(
+                io.BytesIO(r.content), engine="openpyxl", header=0, sheet_name=0
+            )
     return df
 
 
 def _load_file_data_impl(
-    cell_name: str,
     filename: str | None = None,
     timestamp: int | None = None,
     base_url: str | None = None,
     team_slug: str | None = None,
-    authorization: str | None = None,
-    notebook_id: str | None = None,
+    api_key: str | None = None,
 ) -> pd.DataFrame:
     config_from_env = _read_configuration_from_env()
     if base_url is None:
         base_url = config_from_env["base_url"]
     if team_slug is None:
         team_slug = config_from_env["team_slug"]
-    if authorization is None:
-        authorization = config_from_env["authorization"]
-    if notebook_id is None:
-        notebook_id = config_from_env["notebook_id"]
+    if api_key is None:
+        api_key = config_from_env["api_key"]
 
     headers = {
         "teamSlug": team_slug,
-        "Authorization": authorization,
+        "X-Api-Key": api_key,
     }
-    url_sql = urllib.parse.urljoin(
+
+    split_url = urllib.parse.urlsplit(base_url)
+    request_url = urllib.parse.urljoin(
         _canonicalize_base_url(base_url),
-        f"/canvas-file-history/{cell_name}/url/sign",
+        f"{split_url.path}/resource/morph-storage/download-url",
     )
 
     query_params = {}
-    if notebook_id is not None:
-        query_params["notebookId"] = notebook_id
     if filename is not None:
         query_params["filename"] = filename
     if timestamp is not None:
         query_params["timestamp"] = timestamp
-    url_sql += f"?{urllib.parse.urlencode(query_params)}"
+    request_url += f"?{urllib.parse.urlencode(query_params)}"
 
     try:
-        response = requests.get(url_sql, headers=headers)
+        response = requests.get(request_url, headers=headers)
     except Timeout:
-        raise MorphApiError(f"Process Timeout while executing load_data")
+        raise MorphApiError("Process Timeout while executing load_data")
     except Exception as e:
         raise MorphApiError(f"{e}")
 
     response_body = _handle_morph_response(response)
+
     try:
-        structured_response_body = SignedUrlResponse(url=response_body["url"])
+        structured_response_body = SignedUrlResponse(
+            url=response_body["preSignedDownloadUrl"]
+        )
         df = _convert_signed_url_response_to_dateframe(structured_response_body)
         return df
     except Exception as e:
         raise MorphApiError(f"load_data error: {e}")
 
 
 def _execute_sql_impl(
     sql: str,
     connection_slug: str | None = None,
     database_id: str | None = None,
     base_url: str | None = None,
     team_slug: str | None = None,
-    authorization: str | None = None,
-    notebook_id: str | None = None,
+    api_key: str | None = None,
 ) -> pd.DataFrame:
     config_from_env = _read_configuration_from_env()
     if database_id is None:
         database_id = config_from_env["database_id"]
     if base_url is None:
         base_url = config_from_env["base_url"]
     if team_slug is None:
         team_slug = config_from_env["team_slug"]
-    if authorization is None:
-        authorization = config_from_env["authorization"]
-    if notebook_id is None:
-        notebook_id = config_from_env["notebook_id"]
+    if api_key is None:
+        api_key = config_from_env["api_key"]
 
     headers = {
         "teamSlug": team_slug,
-        "Authorization": authorization,
+        "X-Api-Key": api_key,
     }
 
+    split_url = urllib.parse.urlsplit(base_url)
     url_sql = urllib.parse.urljoin(
         _canonicalize_base_url(base_url),
-        f"/{database_id}/sql/python",
+        f"{split_url.path}/{database_id}/sql/python",
     )
 
-    request = {
-        "sql": sql
-    }
+    request = {"sql": sql}
     if connection_slug is not None:
         request["connectionSlug"] = connection_slug
 
     try:
         response = requests.post(url_sql, headers=headers, json=request, verify=True)
     except Timeout:
-        raise MorphApiError(f"Process Timeout whlie executing SQL")
+        raise MorphApiError("Process Timeout while executing SQL")
     except Exception as e:
         raise MorphApiError(f"SQL error: {e}")
 
     response_body = _handle_morph_response(response)
     try:
         structured_response_body = SqlResultResponse(
             headers=response_body["headers"], rows=response_body["rows"]
         )
         df = _convert_sql_engine_response(structured_response_body)
         return df
     except Exception as e:
         raise MorphApiError(f"{e}")
 
 
+def _find_canvas_json(start_dir: str) -> Optional[Tuple[str, Dict]]:
+    current_dir = start_dir
 
-def ref(
-    reference: str,
-    base_url: str | None = None,
-    team_slug: str | None = None,
-    authorization: str | None = None,
-    notebook_id: str | None = None
-) -> RefResponse:
-    config_from_env = _read_configuration_from_env()
-    if base_url is None:
-        base_url = config_from_env["base_url"]
-    if team_slug is None:
-        team_slug = config_from_env["team_slug"]
-    if authorization is None:
-        authorization = config_from_env["authorization"]
-    if notebook_id is None:
-        notebook_id = config_from_env["notebook_id"]
-
-    headers = {
-        "teamSlug": team_slug,
-        "Authorization": authorization,
-    }
-
-    url_sql = urllib.parse.urljoin(
-        _canonicalize_base_url(base_url),
-        f"/canvas/{notebook_id}/cell-name/{reference}",
+    while True:
+        canvas_json_path = os.path.join(current_dir, "canvas.json")
+        if os.path.isfile(canvas_json_path):
+            with open(canvas_json_path, "r") as f:
+                canvas_data = json.load(f)
+            return canvas_json_path, canvas_data
+
+        # ルートディレクトリに到達したらループを終了
+        parent_dir = os.path.dirname(current_dir)
+        if current_dir == parent_dir:
+            break
+
+        current_dir = parent_dir
+
+    return None
+
+
+def ref(reference: str) -> RefResponse:
+    # canvas.jsonを検索・パースする
+    current_dir = os.getcwd()
+    canvas_json = _find_canvas_json(current_dir)
+    if canvas_json is None:
+        raise MorphApiError("canvas.json not found")
+    canvas_json_path, canvas_json_data = canvas_json
+
+    # 当該リファレンスファイルの情報を取得
+    canvas_cell_conf = next(
+        (cell for cell in canvas_json_data["cells"] if cell["filename"] == reference),
+        None,
     )
-    try:
-        response = requests.get(url_sql, headers=headers)
-    except Timeout:
-        raise MorphApiError(f"Process Timeout while executing ref")
-    except Exception as e:
-        raise MorphApiError(f"ref error: {e}")
+    if canvas_cell_conf is None:
+        raise MorphApiError(f"Cell with filename {reference} not found")
 
-    response_body = _handle_morph_response(response)
-    structured_response_body = RefResponse(
-        cell_id=response_body["cellId"],
-        cell_name=response_body["cellName"],
-        cell_type=response_body["cellType"],
-        code=response_body["code"],
-        connection_type=response_body["connectionType"],
-        connection_slug=response_body["connectionSlug"],
-    )
+    # 当該リファレンスファイルの内容を取得
+    ref_code = None
+    if not canvas_cell_conf["filename"].startswith(Protocol.S3.value):
+        ref_file_path = os.path.join(
+            os.path.dirname(canvas_json_path), canvas_cell_conf["filename"]
+        )
+        with open(ref_file_path, "r") as f:
+            ref_code = f.read()
 
-    return structured_response_body
+    return RefResponse(
+        cell_type=canvas_cell_conf["cellType"],
+        filename=canvas_cell_conf["filename"],
+        settings=canvas_cell_conf["settings"],
+        description=canvas_cell_conf["description"],
+        code=ref_code,
+        parent_cells=canvas_cell_conf["parentCells"],
+        connection_type=canvas_cell_conf["connectionType"],
+        connection_slug=canvas_cell_conf["connectionSlug"],
+    )
 
 
 def execute_sql(*args, **kwargs) -> pd.DataFrame:
     if args and isinstance(args[0], RefResponse):
         if args[0].cell_type != "sql":
-            raise MorphApiError(f"Cell {args[0].cell_name} is not a SQL cell")
+            raise MorphApiError(f"Cell {args[0].filename} is not a SQL cell")
         ref_dict = {
             "sql": args[0].code,
             "connection_slug": args[0].connection_slug,
         }
         return _execute_sql_impl(**ref_dict, **kwargs)
     else:
         return _execute_sql_impl(*args, **kwargs)
 
 
 def load_file_data(*args, **kwargs) -> pd.DataFrame:
     if args and isinstance(args[0], RefResponse):
         if args[0].cell_type != "readonlySheet":
             raise MorphApiError(f"Cell {args[0].cell_name} is not a Sheet cell")
         ref_dict = {
-            "cell_name": args[0].cell_name,
+            "filename": args[0].filename,
         }
         return _load_file_data_impl(**ref_dict, **kwargs)
     else:
         return _load_file_data_impl(*args, **kwargs)
 
 
 def load_data(*args: LoadDataParams, **kwargs) -> pd.DataFrame:
@@ -334,15 +356,15 @@
             ref_dict = {
                 "sql": args[0].code,
                 "connection_slug": args[0].connection_slug,
             }
             return _execute_sql_impl(**ref_dict, **kwargs)
         elif args[0].cell_type == "readonlySheet" or args[0].cell_type == "python":
             ref_dict = {
-                "cell_name": args[0].cell_name,
+                "filename": args[0].filename,
             }
             return _load_file_data_impl(**ref_dict, **kwargs)
         else:
             raise MorphApiError(f"Cell {args[0].cell_name} is not a valid cell type")
     elif "type" in args[0]:
         if args[0]["type"] == "sql":
             omitted_args = {k: v for k, v in args[0].items() if k != "type"}
@@ -359,53 +381,52 @@
 def generate_report(
     refs: list[RefResponse],
     prompt: Optional[str] = None,
     language: Optional[str] = None,
     database_id: str | None = None,
     base_url: str | None = None,
     team_slug: str | None = None,
-    authorization: str | None = None,
-    notebook_id: str | None = None,
+    api_key: str | None = None,
 ) -> str:
     config_from_env = _read_configuration_from_env()
     if database_id is None:
         database_id = config_from_env["database_id"]
     if base_url is None:
         base_url = config_from_env["base_url"]
     if team_slug is None:
         team_slug = config_from_env["team_slug"]
-    if authorization is None:
-        authorization = config_from_env["authorization"]
-    if notebook_id is None:
-        notebook_id = config_from_env["notebook_id"]
+    if api_key is None:
+        api_key = config_from_env["api_key"]
 
     for ref in refs:
         if ref.cell_type != "python":
             raise MorphApiError(f"Cell {ref.cell_name} is not a Python cell")
         elif "@report" in ref.code:
-            raise MorphApiError(f"Cell {ref.cell_name}(report cell) is not allowed to be used in report generation.")
+            raise MorphApiError(
+                f"Cell {ref.cell_name}(report cell) is not allowed to be used in report generation."
+            )
 
     headers = {
         "teamSlug": team_slug,
-        "Authorization": authorization,
+        "X-Api-Key": api_key,
     }
 
     url = urllib.parse.urljoin(
         _canonicalize_base_url(base_url),
-        f"/agent/chat/report",
+        "/agent/chat/report",
     )
 
     request = {
         "cellIds": [ref.cell_id for ref in refs],
         "prompt": prompt,
         "language": language,
     }
 
     try:
         response = requests.post(url, headers=headers, json=request, verify=True)
     except Timeout:
-        raise MorphApiError(f"Process Timeout while executing generate_report")
+        raise MorphApiError("Process Timeout while executing generate_report")
     except Exception as e:
         raise MorphApiError(f"generate_report error: {e}")
 
     response_body = _handle_morph_response(response)
-    return response_body["report"]
+    return response_body["report"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `morphdb_utils-0.2.0/morphdb_utils/type.py` & `morphdb_utils-0.2.1/morphdb_utils/type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict, List, TypedDict, Optional, Literal, Union
+from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
+
+
+class Protocol(Enum):
+    FILE = "file://"
+    S3 = "morph-storage://"
 
 
 class NullValue(Enum):
     NULL_VALUE = 0
 
 
 class ListValue(TypedDict):
@@ -34,49 +39,51 @@
 @dataclass
 class SignedUrlResponse:
     url: str
 
 
 @dataclass
 class RefResponse:
-    cell_id: str
-    cell_name: str
-    code: str
     cell_type: str
+    filename: str
+    settings: Dict[str, int]
+    description: Optional[str]
+    code: Optional[str]
+    parent_cells: List[str]
     connection_type: Optional[str]
     connection_slug: Optional[str]
 
 
 class SheetCellParams(TypedDict):
-    type: Literal['sheet']
+    type: Literal["sheet"]
     cell_name: str
     filename: Optional[str]
     timestamp: Optional[int]
     base_url: Optional[str]
     team_slug: Optional[str]
     authorization: Optional[str]
     notebook_id: Optional[str]
 
 
 class SqlCellParams(TypedDict):
-    type: Literal['sql']
+    type: Literal["sql"]
     sql: str
     connection_slug: Optional[str]
     database_id: Optional[str]
     base_url: Optional[str]
     team_slug: Optional[str]
     authorization: Optional[str]
     notebook_id: Optional[str]
 
 
 class PythonCellParams(TypedDict):
-    type: Literal['python']
+    type: Literal["python"]
     cell_name: str
     filename: Optional[str]
     timestamp: Optional[int]
     base_url: Optional[str]
     team_slug: Optional[str]
     authorization: Optional[str]
-    notebook_id: Optional[str]    
+    notebook_id: Optional[str]
 
 
-LoadDataParams = Union[RefResponse, SheetCellParams, SqlCellParams]
+LoadDataParams = Union[RefResponse, SheetCellParams, SqlCellParams]
```

### Comparing `morphdb_utils-0.2.0/pyproject.toml` & `morphdb_utils-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "morphdb-utils"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["shibatanaoto <naoto.shibata510@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "1.5.3"
 requests = "2.31.0"
 xlrd = "2.0.1"
 matplotlib = "3.5.2"
 plotly = "5.21.0"
 kaleido = "0.2.1"
+openpyxl = "^3.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 types-requests = "^2.28.11.13"
 pytest = "^7.4.4"
 black = "^24.1.0"
@@ -34,8 +35,8 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
 pub-test = "poetry publish -r testpypi --build"
-pub = "poetry publish --build"
+pub = "poetry publish --build"
```

