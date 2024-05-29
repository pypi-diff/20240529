# Comparing `tmp/flatpack-3.5.1.tar.gz` & `tmp/flatpack-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.5.1.tar", last modified: Wed May 29 07:31:15 2024, max compression
+gzip compressed data, was "flatpack-3.5.2.tar", last modified: Wed May 29 14:33:54 2024, max compression
```

## Comparing `flatpack-3.5.1.tar` & `flatpack-3.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.781423 flatpack-3.5.1/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.1/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 07:31:15.781118 flatpack-3.5.1/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5019 2024-05-27 13:05:21.000000 flatpack-3.5.1/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.777463 flatpack-3.5.1/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.1/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.1/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.779296 flatpack-3.5.1/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.1/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.1/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.1/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.5.1/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-05-25 14:16:18.000000 flatpack-3.5.1/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    33779 2024-05-29 07:30:10.000000 flatpack-3.5.1/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.780298 flatpack-3.5.1/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.1/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.1/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.1/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.780676 flatpack-3.5.1/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-29 07:31:15.781509 flatpack-3.5.1/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-29 07:30:46.000000 flatpack-3.5.1/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.933303 flatpack-3.5.2/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.2/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 14:33:54.933009 flatpack-3.5.2/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5019 2024-05-27 13:05:21.000000 flatpack-3.5.2/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.930396 flatpack-3.5.2/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.2/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.2/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.931798 flatpack-3.5.2/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.2/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.2/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.2/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.5.2/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-05-25 14:16:18.000000 flatpack-3.5.2/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    36256 2024-05-29 14:32:57.000000 flatpack-3.5.2/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.932324 flatpack-3.5.2/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.2/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.2/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.2/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.932593 flatpack-3.5.2/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-29 14:33:54.933373 flatpack-3.5.2/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-29 13:36:26.000000 flatpack-3.5.2/setup.py
```

### Comparing `flatpack-3.5.1/LICENSE` & `flatpack-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/PKG-INFO` & `flatpack-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.1
+Version: 3.5.2
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.5.1/README.md` & `flatpack-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack/agent_manager.py` & `flatpack-3.5.2/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack/datasets.py` & `flatpack-3.5.2/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.5.2/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack/instructions.py` & `flatpack-3.5.2/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack/main.py` & `flatpack-3.5.2/flatpack/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 import atexit
 import httpx
 import ngrok
 import os
 import re
 import requests
 import shlex
+import shutil
 import stat
 import subprocess
 import sys
 import toml
 import uvicorn
 
 from .agent_manager import AgentManager
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.staticfiles import StaticFiles
 from huggingface_hub import snapshot_download
 from importlib.metadata import version
+from io import BytesIO
 from .parsers import parse_toml_to_venv_script
 from pathlib import Path
 from .session_manager import SessionManager
 from typing import List, Optional, Union
 from .vector_manager import VectorManager
+from zipfile import ZipFile
 
 HOME_DIR = Path.home()
 
 BASE_URL = "https://raw.githubusercontent.com/romlingroup/flatpack/main/warehouse"
 CONFIG_FILE_PATH = HOME_DIR / ".fpk_config.toml"
 GITHUB_REPO_URL = "https://api.github.com/repos/romlingroup/flatpack"
 KEY_FILE_PATH = HOME_DIR / ".fpk_encryption_key"
@@ -113,14 +116,55 @@
         "red": "\033[91m",
         "white": "\033[97m",
         "yellow": "\033[93m"
     }
     return colors[color] + text + colors["default"]
 
 
+def fpk_create(flatpack_name, repo_url="https://github.com/RomlinGroup/template"):
+    if not re.match(r'^[a-z0-9-]+$', flatpack_name):
+        raise ValueError("Error: Invalid name format. Only lowercase letters, numbers, and hyphens are allowed.")
+
+    flatpack_name = flatpack_name.lower().replace(' ', '-')
+
+    current_dir = os.getcwd()
+    template_dir = fpk_download_and_extract_template(repo_url, current_dir)
+
+    flatpack_dir = os.path.join(current_dir, flatpack_name)
+    os.makedirs(flatpack_dir, exist_ok=True)
+
+    for item in os.listdir(template_dir):
+        s = os.path.join(template_dir, item)
+        d = os.path.join(flatpack_dir, item)
+        if os.path.isdir(s):
+            shutil.copytree(s, d, dirs_exist_ok=True)
+        else:
+            shutil.copy2(s, d)
+
+    files_to_edit = [
+        (os.path.join(flatpack_dir, "README.md"), r"# template", f"# {flatpack_name}"),
+        (os.path.join(flatpack_dir, "flatpack.toml"), r"{{model_name}}", flatpack_name),
+        (os.path.join(flatpack_dir, "build.sh"), r"export DEFAULT_REPO_NAME=template",
+         f"export DEFAULT_REPO_NAME={flatpack_name}"),
+        (os.path.join(flatpack_dir, "build.sh"), r"export FLATPACK_NAME=template",
+         f"export FLATPACK_NAME={flatpack_name}")
+    ]
+
+    for file_path, pattern, replacement in files_to_edit:
+        with open(file_path, 'r') as file:
+            filedata = file.read()
+
+        newdata = re.sub(pattern, replacement, filedata)
+
+        with open(file_path, 'w') as file:
+            file.write(newdata)
+
+    print(f"Contents of template copied to {flatpack_name}.")
+
+
 def fpk_display_disclaimer(directory_name: str, local: bool):
     """Display a disclaimer message with details about a specific flatpack.
 
     Args:
         directory_name (str): Name of the flatpack directory.
     """
     disclaimer_template = """
@@ -158,14 +202,21 @@
         please_note_colored = fpk_colorize(please_note_content, "yellow")
     else:
         please_note_colored = ""
 
     print(disclaimer_template.format(please_note=please_note_colored))
 
 
+def fpk_download_and_extract_template(repo_url, dest_dir):
+    response = requests.get(f"{repo_url}/archive/refs/heads/main.zip")
+    with ZipFile(BytesIO(response.content)) as zip_ref:
+        zip_ref.extractall(dest_dir)
+    return os.path.join(dest_dir, "template-main")
+
+
 def fpk_fetch_flatpack_toml_from_dir(directory_name: str, session: httpx.Client) -> Optional[str]:
     """Fetch the flatpack TOML configuration from a specific directory.
     Args:
         directory_name (str): Name of the flatpack directory.
         session (httpx.Client): HTTP client session for making requests.
     Returns:
         Optional[str]: The TOML content if found, otherwise None.
@@ -341,15 +392,15 @@
     """Unbox a flatpack from GitHub or a local directory."""
     if not fpk_valid_directory_name(directory_name):
         print(f"❌ Invalid directory name: '{directory_name}'.")
         return
 
     flatpack_dir = Path.cwd() / directory_name
 
-    if flatpack_dir.exists():
+    if flatpack_dir.exists() and not local:
         print("❌ Error: Flatpack directory already exists.")
         return
     else:
         build_dir = flatpack_dir / "build"
 
         if build_dir.exists():
             print("❌ Error: Build directory already exists.")
@@ -450,14 +501,19 @@
     parser_set_api.add_argument('api_key', type=str, help='API key to set')
     parser_set_api.set_defaults(func=lambda args, session: fpk_cli_handle_set_api_key(args, session))
 
     # Get API key
     parser_get_api = api_key_subparsers.add_parser('get', help='Get the current API key')
     parser_get_api.set_defaults(func=lambda args, session: fpk_cli_handle_get_api_key(args, session))
 
+    # Create flatpack
+    parser_create = subparsers.add_parser('create', help='Create a new flatpack.')
+    parser_create.add_argument('input', nargs='?', default=None, help='The name of the flatpack to create.')
+    parser_create.set_defaults(func=lambda args, session: fpk_cli_handle_create(args, session))
+
     # Unbox commands
     parser_unbox = subparsers.add_parser('unbox', help='Unbox a flatpack from GitHub or a local directory.')
     parser_unbox.add_argument('input', nargs='?', default=None, help='The name of the flatpack to unbox.')
     parser_unbox.add_argument('--local', action='store_true', help='Unbox from a local directory instead of GitHub.')
     parser_unbox.set_defaults(func=lambda args, session: fpk_cli_handle_unbox(args, session))
 
     # Build commands
@@ -558,14 +614,23 @@
 
 
 def fpk_cli_handle_build(args, session):
     directory_name = args.directory
     fpk_build(directory_name)
 
 
+def fpk_cli_handle_create(args, session):
+    if not args.input:
+        print("❌ Please specify a name for the new flatpack.")
+        return
+
+    flatpack_name = args.input
+    fpk_create(flatpack_name)
+
+
 def create_venv(venv_dir):
     subprocess.run(["python3", "-m", "venv", venv_dir], check=True)
 
 
 def fpk_cli_handle_compress(args, session: httpx.Client):
     model_id = args.model_id
     token = args.token
```

### Comparing `flatpack-3.5.1/flatpack/modules/lstm.py` & `flatpack-3.5.2/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack/modules/rnn.py` & `flatpack-3.5.2/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack/parsers.py` & `flatpack-3.5.2/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack/vector_manager.py` & `flatpack-3.5.2/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/flatpack.egg-info/PKG-INFO` & `flatpack-3.5.2/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.1
+Version: 3.5.2
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.5.1/flatpack.egg-info/SOURCES.txt` & `flatpack-3.5.2/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.1/setup.py` & `flatpack-3.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.5.1",
+    version="3.5.2",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "fastapi==0.110.2",
         "hnswlib==0.8.0",
         "httpx==0.27.0",
```

