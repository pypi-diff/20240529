# Comparing `tmp/llm_ollama-0.4.0.tar.gz` & `tmp/llm_ollama-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_ollama-0.4.0.tar", last modified: Wed May 22 07:11:44 2024, max compression
+gzip compressed data, was "llm_ollama-0.4.1.tar", last modified: Wed May 29 20:00:43 2024, max compression
```

## Comparing `llm_ollama-0.4.0.tar` & `llm_ollama-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:11:44.575372 llm_ollama-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-22 07:11:44.575372 llm_ollama-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:11:44.571372 llm_ollama-0.4.0/llm_ollama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/llm_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:11:44.575372 llm_ollama-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:11:44.571372 llm_ollama-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/tests/test_ollama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:00:43.663555 llm_ollama-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 20:00:39.000000 llm_ollama-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-29 20:00:43.663555 llm_ollama-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-29 20:00:39.000000 llm_ollama-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:00:43.663555 llm_ollama-0.4.1/llm_ollama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-29 20:00:43.000000 llm_ollama-0.4.1/llm_ollama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 20:00:43.000000 llm_ollama-0.4.1/llm_ollama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:00:43.000000 llm_ollama-0.4.1/llm_ollama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 20:00:43.000000 llm_ollama-0.4.1/llm_ollama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:00:43.000000 llm_ollama-0.4.1/llm_ollama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 20:00:43.000000 llm_ollama-0.4.1/llm_ollama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-29 20:00:39.000000 llm_ollama-0.4.1/llm_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-29 20:00:39.000000 llm_ollama-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:00:43.663555 llm_ollama-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:00:43.663555 llm_ollama-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-29 20:00:39.000000 llm_ollama-0.4.1/tests/test_ollama.py
```

### Comparing `llm_ollama-0.4.0/LICENSE` & `llm_ollama-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_ollama-0.4.0/PKG-INFO` & `llm_ollama-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-ollama
-Version: 0.4.0
+Version: 0.4.1
 Summary: LLM plugin providing access to local Ollama models
 Author: Sergey Alexandrov
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/taketwo/llm-ollama
 Project-URL: Changelog, https://github.com/taketwo/llm-ollama/releases
 Project-URL: Issues, https://github.com/taketwo/llm-ollama/issues
 Project-URL: CI, https://github.com/taketwo/llm-ollama/actions
```

### Comparing `llm_ollama-0.4.0/README.md` & `llm_ollama-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `llm_ollama-0.4.0/llm_ollama.egg-info/PKG-INFO` & `llm_ollama-0.4.1/llm_ollama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-ollama
-Version: 0.4.0
+Version: 0.4.1
 Summary: LLM plugin providing access to local Ollama models
 Author: Sergey Alexandrov
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/taketwo/llm-ollama
 Project-URL: Changelog, https://github.com/taketwo/llm-ollama/releases
 Project-URL: Issues, https://github.com/taketwo/llm-ollama/issues
 Project-URL: CI, https://github.com/taketwo/llm-ollama/actions
```

### Comparing `llm_ollama-0.4.0/llm_ollama.py` & `llm_ollama-0.4.1/llm_ollama.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,22 @@
     @cli.group(name="ollama")
     def ollama_group():
         "Commands for working with models hosted on Ollama"
 
     @ollama_group.command(name="list-models")
     def list_models():
         """List models that are available locally on Ollama server."""
-        for model in ollama.list()["models"]:
+        for model in _get_ollama_models():
             click.echo(model["name"])
 
 
 @llm.hookimpl
 def register_models(register):
     models = defaultdict(list)
-    for model in ollama.list()["models"]:
+    for model in _get_ollama_models():
         models[model["digest"]].append(model["name"])
         if model["name"].endswith(":latest"):
             models[model["digest"]].append(model["name"][: -len(":latest")])
     for names in models.values():
         name, aliases = _pick_primary_name(names)
         register(Ollama(name), aliases=aliases)
 
@@ -174,19 +174,36 @@
     names : list[str]
         A non-empty list of model names.
 
     Returns
     -------
     tuple[str, list[str, ...]]
         The primary model name and a list with the secondary names.
+
     """
     if len(names) == 1:
         return names[0], ()
     sorted_names = sorted(
         names,
         key=lambda name: (
             ":" not in name,
             name.endswith(":latest"),
             name,
         ),
     )
     return sorted_names[0], tuple(sorted_names[1:])
+
+
+def _get_ollama_models():
+    """Get a list of models available on Ollama.
+
+    Returns
+    -------
+    list[dict]
+        A list of models available on Ollama. If the Ollama server is down, an empty
+        list is returned.
+
+    """
+    try:
+        return ollama.list()["models"]
+    except:
+        return []
```

### Comparing `llm_ollama-0.4.0/pyproject.toml` & `llm_ollama-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-ollama"
-version = "0.4.0"
+version = "0.4.1"
 description = "LLM plugin providing access to local Ollama models"
 readme = "README.md"
 authors = [{ name = "Sergey Alexandrov" }]
 license = { text = "Apache-2.0" }
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 dependencies = ["llm", "ollama", "pydantic>=2"]
 requires-python = ">=3.8"
```

### Comparing `llm_ollama-0.4.0/tests/test_ollama.py` & `llm_ollama-0.4.1/tests/test_ollama.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from unittest.mock import patch
 
+from httpx import ConnectError
+
 from llm import get_models_with_aliases
 from llm.plugins import pm
 
 from llm_ollama import Ollama
 
 
 def test_plugin_is_installed():
@@ -43,7 +45,13 @@
         [m for m in get_models_with_aliases() if isinstance(m.model, Ollama)],
         key=lambda m: m.model.model_id,
     )
     assert len(registered_ollama_models) == len(expected)
     for model, (name, aliases) in zip(registered_ollama_models, expected):
         assert model.model.model_id == name
         assert model.aliases == aliases
+
+
+@patch("llm_ollama.ollama.list")
+def test_registered_models_when_ollama_is_down(mock_ollama_list):
+    mock_ollama_list.side_effect = ConnectError("[Errno 111] Connection refused")
+    assert not any(isinstance(m.model, Ollama) for m in get_models_with_aliases())
```

