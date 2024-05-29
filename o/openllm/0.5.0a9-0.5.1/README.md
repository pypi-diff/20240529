# Comparing `tmp/openllm-0.5.0a9.tar.gz` & `tmp/openllm-0.5.1.tar.gz`

## Comparing `openllm-0.5.0a9.tar` & `openllm-0.5.1.tar`

### file list

```diff
@@ -1,78 +1,58 @@
--rw-r--r--   0        0        0    42925 2020-02-02 00:00:00.000000 openllm-0.5.0a9/CHANGELOG.md
--rw-r--r--   0        0        0    40681 2020-02-02 00:00:00.000000 openllm-0.5.0a9/README.md
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.0a9/pyoxidizer.bzl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_service_vars.pyi
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/Dockerfile.j2
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/__init__.pyi
--rw-r--r--   0        0        0    19189 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/_entrypoint.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/_helpers.py
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/_llm.py
--rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/_service.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/_service_vars.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/_openllm_tiny/bentofile.yaml
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/__init__.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/__init__.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/__main__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_deprecated.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_generation.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_generation.pyi
--rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_llm.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_llm.pyi
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_quantisation.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_quantisation.pyi
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_runners.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_runners.pyi
--rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_strategies.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_strategies.pyi
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/_version.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/client.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/client.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/py.typed
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/utils.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/utils.pyi
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/bundle/__init__.pyi
--rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/bundle/_package.pyi
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/entrypoints/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/entrypoints/__init__.pyi
--rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/entrypoints/_openapi.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/entrypoints/_openapi.pyi
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/entrypoints/hf.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/entrypoints/hf.pyi
--rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/entrypoints/openai.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/entrypoints/openai.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/__init__.pyi
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/_helpers.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/ggml/__init__.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/transformers/__init__.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/transformers/_helpers.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/transformers/weights.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm/serialisation/vllm/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/__init__.py
--rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/_factory.py
--rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/_sdk.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/termui.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/extension/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/extension/dive_bentos.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/extension/get_containerfile.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/extension/get_prompt.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/extension/list_bentos.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/extension/list_models.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/extension/playground.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/playground/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/playground/__init__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/playground/_meta.yml
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/playground/features.py
--rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 openllm-0.5.0a9/src/openllm_cli/playground/opt_tuned.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.0a9/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.0a9/LICENSE.md
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 openllm-0.5.0a9/pyproject.toml
--rw-r--r--   0        0        0    47179 2020-02-02 00:00:00.000000 openllm-0.5.0a9/PKG-INFO
+-rw-r--r--   0        0        0    44371 2020-02-02 00:00:00.000000 openllm-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0    36563 2020-02-02 00:00:00.000000 openllm-0.5.1/README.md
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.1/pyoxidizer.bzl
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_service_vars.pyi
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/Dockerfile.j2
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/__init__.pyi
+-rw-r--r--   0        0        0    22767 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/_entrypoint.py
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/_helpers.py
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/_llm.py
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/_service.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/_service_vars.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/_termui.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/bentofile.yaml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/service.md
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 openllm-0.5.1/src/_openllm_tiny/setup.sh
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/__init__.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/__init__.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/__main__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_deprecated.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_generation.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_generation.pyi
+-rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_llm.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_llm.pyi
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_quantisation.pyi
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_runners.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_runners.pyi
+-rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_strategies.pyi
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/_version.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/client.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/client.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/py.typed
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/utils.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/utils.pyi
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/bundle/__init__.pyi
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/bundle/_package.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/__init__.pyi
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/_helpers.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/ggml/__init__.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/transformers/__init__.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/transformers/_helpers.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/transformers/weights.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm/serialisation/vllm/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm_cli/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm_cli/entrypoint.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 openllm-0.5.1/src/openllm_cli/termui.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.1/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 openllm-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    42926 2020-02-02 00:00:00.000000 openllm-0.5.1/PKG-INFO
```

### Comparing `openllm-0.5.0a9/CHANGELOG.md` & `openllm-0.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,55 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.5.1](https://github.com/bentoml/openllm/tree/v0.5.1)
+No significant changes.
+
+
+## [0.5.0](https://github.com/bentoml/openllm/tree/v0.5.0)
+No significant changes.
+
+
+## [0.5.0-alpha.15](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.15)
+
+### Backwards-incompatible Changes
+
+- Now, OpenLLM is compatible with BentoML 1.2 and above architecture.
+
+  Additionally, `openllm` CLI will only offer `start` and `build` to simplify the workflow.
+
+  OpenLLM will also now require vllm by default, and CPU support is currently turning off. We will look into supporting CPU in later version as our main focus is on accelerator.
+
+  Python API is also considered deprecated and internal only. If you are using this in your old service, make sure to set `IMPLEMENTATION=deprecated` as environment variable to avoid breaking changes. We recommend users to upgrade to BentoML 1.2.
+  [#996](https://github.com/bentoml/openllm/issues/996)
+
+## [0.5.0-alpha.14](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.14)
+No significant changes.
+
+
+## [0.5.0-alpha.13](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.13)
+No significant changes.
+
+
+## [0.5.0-alpha.12](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.12)
+No significant changes.
+
+
+## [0.5.0-alpha.11](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.11)
+No significant changes.
+
+
+## [0.5.0-alpha.10](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.10)
+No significant changes.
+
+
 ## [0.5.0-alpha.9](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.9)
 No significant changes.
 
 
 ## [0.5.0-alpha.8](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.8)
 No significant changes.
```

### Comparing `openllm-0.5.0a9/README.md` & `openllm-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,18 @@
     </a>
 </div>
 
 ## 📖 Introduction
 
 OpenLLM helps developers **run any open-source LLMs**, such as Llama 2 and Mistral, as **OpenAI-compatible API endpoints**, locally and in the cloud, optimized for serving throughput and production deployment.
 
-
 - 🚂 Support a wide range of open-source LLMs including LLMs fine-tuned with your own data
 - ⛓️ OpenAI compatible API endpoints for seamless transition from your LLM app to open-source LLMs
 - 🔥 State-of-the-art serving and inference performance
-- 🎯 Simplified cloud deployment via [BentoML](www.bentoml.com)
-
+- 🎯 Simplified cloud deployment via [BentoML](https://www.bentoml.com)
 
 <!-- hatch-fancy-pypi-readme intro stop -->
 
 ![Gif showing OpenLLM Intro](/.github/assets/output.gif)
 
 <br/>
 
@@ -42,132 +40,65 @@
 
 For starter, we provide two ways to quickly try out OpenLLM:
 
 ### Jupyter Notebooks
 
 Try this [OpenLLM tutorial in Google Colab: Serving Llama 2 with OpenLLM](https://colab.research.google.com/github/bentoml/OpenLLM/blob/main/examples/llama2.ipynb).
 
-### Docker
-
-We provide a docker container that helps you start running OpenLLM:
-
-```bash
-docker run --rm -it -p 3000:3000 ghcr.io/bentoml/openllm start facebook/opt-1.3b --backend pt
-```
-
-> [!NOTE]
-> Given you have access to GPUs and have setup [nvidia-docker](https://github.com/NVIDIA/nvidia-container-toolkit),  you can additionally pass in `--gpus`
-> to use GPU for faster inference and optimization
->```bash
-> docker run --rm --gpus all -p 3000:3000 -it ghcr.io/bentoml/openllm start HuggingFaceH4/zephyr-7b-beta --backend vllm
-> ```
-
-
 ## 🏃 Get started
 
 The following provides instructions for how to get started with OpenLLM locally.
 
 ### Prerequisites
 
-You have installed Python 3.8 (or later) and `pip`. We highly recommend using a [Virtual Environment](https://docs.python.org/3/library/venv.html) to prevent package conflicts.
+You have installed Python 3.9 (or later) and `pip`. We highly recommend using a [Virtual Environment](https://docs.python.org/3/library/venv.html) to prevent package conflicts.
 
 ### Install OpenLLM
 
 Install OpenLLM by using `pip` as follows:
 
 ```bash
 pip install openllm
 ```
 
 To verify the installation, run:
 
 ```bash
 $ openllm -h
-
-Usage: openllm [OPTIONS] COMMAND [ARGS]...
-
-   ██████╗ ██████╗ ███████╗███╗   ██╗██╗     ██╗     ███╗   ███╗
-  ██╔═══██╗██╔══██╗██╔════╝████╗  ██║██║     ██║     ████╗ ████║
-  ██║   ██║██████╔╝█████╗  ██╔██╗ ██║██║     ██║     ██╔████╔██║
-  ██║   ██║██╔═══╝ ██╔══╝  ██║╚██╗██║██║     ██║     ██║╚██╔╝██║
-  ╚██████╔╝██║     ███████╗██║ ╚████║███████╗███████╗██║ ╚═╝ ██║
-   ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝╚═╝     ╚═╝.
-
-  An open platform for operating large language models in production.
-  Fine-tune, serve, deploy, and monitor any LLMs with ease.
-
-Options:
-  -v, --version  Show the version and exit.
-  -h, --help     Show this message and exit.
-
-Commands:
-  build       Package a given models into a BentoLLM.
-  import      Setup LLM interactively.
-  models      List all supported models.
-  prune       Remove all saved models, (and optionally bentos) built with OpenLLM locally.
-  query       Query a LLM interactively, from a terminal.
-  start       Start a LLMServer for any supported LLM.
-
-Extensions:
-  build-base-container  Base image builder for BentoLLM.
-  dive-bentos           Dive into a BentoLLM.
-  get-containerfile     Return Containerfile of any given Bento.
-  get-prompt            Get the default prompt used by OpenLLM.
-  list-bentos           List available bentos built by OpenLLM.
-  list-models           This is equivalent to openllm models...
-  playground            OpenLLM Playground.
 ```
 
 ### Start a LLM server
 
-OpenLLM allows you to quickly spin up an LLM server using `openllm start`. For example, to start a [phi-2](https://huggingface.co/microsoft/phi-2) server, run the following:
+OpenLLM allows you to quickly spin up an LLM server using `openllm start`. For example, to start a [Llama 3 8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B) server, run the following:
 
 ```bash
-TRUST_REMOTE_CODE=True openllm start microsoft/phi-2
+openllm start meta-llama/Meta-Llama-3-8B
 ```
 
-This starts the server at [http://0.0.0.0:3000/](http://0.0.0.0:3000/). OpenLLM downloads the model to the BentoML local Model Store if it has not been registered before. To view your local models, run `bentoml models list`.
-
 To interact with the server, you can visit the web UI at [http://0.0.0.0:3000/](http://0.0.0.0:3000/) or send a request using `curl`. You can also use OpenLLM’s built-in Python client to interact with the server:
 
 ```python
 import openllm
 
-client = openllm.client.HTTPClient('http://localhost:3000')
-client.query('Explain to me the difference between "further" and "farther"')
-```
-
-Alternatively, use the `openllm query` command to query the model:
-
-```bash
-export OPENLLM_ENDPOINT=http://localhost:3000
-openllm query 'Explain to me the difference between "further" and "farther"'
+client = openllm.HTTPClient('http://localhost:3000')
+client.generate('Explain to me the difference between "further" and "farther"')
 ```
 
 OpenLLM seamlessly supports many models and their variants. You can specify different variants of the model to be served. For example:
 
 ```bash
 openllm start <model_id> --<options>
 ```
 
 > [!NOTE]
 > OpenLLM supports specifying fine-tuning weights and quantized weights
 > for any of the supported models as long as they can be loaded with the model
 > architecture. Use the `openllm models` command to see the complete list of supported
 > models, their architectures, and their variants.
 
-> [!IMPORTANT]
-> If you are testing OpenLLM on CPU, you might want to pass in `DTYPE=float32`. By default,
-> OpenLLM will set model `dtype` to `bfloat16` for the best performance.
-> ```bash
-> DTYPE=float32 openllm start microsoft/phi-2
-> ```
-> This will also applies to older GPUs. If your GPUs doesn't support `bfloat16`, then you also
-> want to set `DTYPE=float16`.
-
 ## 🧩 Supported models
 
 OpenLLM currently supports the following models. By default, OpenLLM doesn't include dependencies to run all models. The extra model-specific dependencies can be installed with the instructions below.
 
 <!-- update-readme.py: start -->
 <details>
 
@@ -740,15 +671,15 @@
 > pip install "openllm[phi]"
 > ```
 
 
 Run the following command to quickly spin up a Phi server:
 
 ```bash
-TRUST_REMOTE_CODE=True openllm start microsoft/phi-2
+TRUST_REMOTE_CODE=True openllm start microsoft/Phi-3-mini-4k-instruct
 ```
 In a different terminal, run the following command to interact with the server:
 
 ```bash
 export OPENLLM_ENDPOINT=http://localhost:3000
 openllm query 'What are large language models?'
 ```
@@ -759,16 +690,20 @@
 
 
 ### Supported models
 
 You can specify any of the following Phi models via `openllm start`:
 
 
-- [microsoft/phi-2](https://huggingface.co/microsoft/phi-2)
-- [microsoft/phi-1_5](https://huggingface.co/microsoft/phi-1_5)
+- [microsoft/Phi-3-mini-4k-instruct](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)
+- [microsoft/Phi-3-mini-128k-instruct](https://huggingface.co/microsoft/Phi-3-mini-128k-instruct)
+- [microsoft/Phi-3-small-8k-instruct](https://huggingface.co/microsoft/Phi-3-small-8k-instruct)
+- [microsoft/Phi-3-small-128k-instruct](https://huggingface.co/microsoft/Phi-3-small-128k-instruct)
+- [microsoft/Phi-3-medium-4k-instruct](https://huggingface.co/microsoft/Phi-3-medium-4k-instruct)
+- [microsoft/Phi-3-medium-128k-instruct](https://huggingface.co/microsoft/Phi-3-medium-128k-instruct)
 
 </details>
 
 <details>
 
 <summary>Qwen</summary>
 
@@ -1089,15 +1024,14 @@
 ```bash
 openllm build facebook/opt-6.7b --adapter-id ./path/to/adapter_id --build-ctx .
 ```
 
 > [!IMPORTANT]
 > Fine-tuning support is still experimental and currently only works with PyTorch backend. vLLM support is coming soon.
 
-
 ## ⚙️ Integrations
 
 OpenLLM is not just a standalone product; it's a building block designed to
 integrate with other powerful tools easily. We currently offer integration with
 [OpenAI's Compatible Endpoints](https://platform.openai.com/docs/api-reference/completions/object),
 [LlamaIndex](https://www.llamaindex.ai/),
 [LangChain](https://github.com/hwchase17/langchain), and
@@ -1107,30 +1041,27 @@
 
 OpenLLM Server can be used as a drop-in replacement for OpenAI's API. Simply
 specify the base_url to `llm-endpoint/v1` and you are good to go:
 
 ```python
 import openai
 
-client = openai.OpenAI(
-  base_url='http://localhost:3000/v1', api_key='na'
-)  # Here the server is running on localhost:3000
+client = openai.OpenAI(base_url='http://localhost:3000/v1', api_key='na')  # Here the server is running on 0.0.0.0:3000
 
-completions = client.completions.create(
+completions = client.chat.completions.create(
   prompt='Write me a tag line for an ice cream shop.', model=model, max_tokens=64, stream=stream
 )
 ```
 
 The compatible endpoints supports `/completions`, `/chat/completions`, and `/models`
 
 > [!NOTE]
 > You can find out OpenAI example clients under the
 > [examples](https://github.com/bentoml/OpenLLM/tree/main/examples) folder.
 
-
 ### [LlamaIndex](https://docs.llamaindex.ai/en/stable/examples/llm/openllm/)
 
 To start a local LLM with `llama_index`, simply use `llama_index.llms.openllm.OpenLLM`:
 
 ```python
 import asyncio
 from llama_index.llms.openllm import OpenLLM
@@ -1164,32 +1095,14 @@
 ```python
 from langchain.llms import OpenLLM
 
 llm = OpenLLM(server_url='http://44.23.123.1:3000', server_type='http')
 llm('What is the difference between a duck and a goose? And why there are so many Goose in Canada?')
 ```
 
-### Transformers Agents
-
-OpenLLM seamlessly integrates with
-[Transformers Agents](https://huggingface.co/docs/transformers/transformers_agents).
-
-> [!WARNING]
-> The Transformers Agent is still at an experimental stage. It is
-> recommended to install OpenLLM with `pip install -r nightly-requirements.txt`
-> to get the latest API update for HuggingFace agent.
-
-```python
-import transformers
-
-agent = transformers.HfAgent('http://localhost:3000/hf/agent')  # URL that runs the OpenLLM server
-
-agent.run('Is the following `text` positive or negative?', text="I don't like how this models is generate inputs")
-```
-
 <!-- hatch-fancy-pypi-readme interim stop -->
 
 ![Gif showing Agent integration](/.github/assets/agent.gif)
 
 <br/>
 
 <!-- hatch-fancy-pypi-readme meta start -->
@@ -1272,34 +1185,14 @@
 capabilities or have any questions, don't hesitate to reach out in our
 [discord channel](https://l.bentoml.com/join-openllm-discord).
 
 Checkout our
 [Developer Guide](https://github.com/bentoml/OpenLLM/blob/main/DEVELOPMENT.md)
 if you wish to contribute to OpenLLM's codebase.
 
-## 🍇 Telemetry
-
-OpenLLM collects usage data to enhance user experience and improve the product.
-We only report OpenLLM's internal API calls and ensure maximum privacy by
-excluding sensitive information. We will never collect user code, model data, or
-stack traces. For usage tracking, check out the
-[code](https://github.com/bentoml/OpenLLM/blob/main/openllm-core/src/openllm_core/utils/analytics.py).
-
-You can opt out of usage tracking by using the `--do-not-track` CLI option:
-
-```bash
-openllm [command] --do-not-track
-```
-
-Or by setting the environment variable `OPENLLM_DO_NOT_TRACK=True`:
-
-```bash
-export OPENLLM_DO_NOT_TRACK=True
-```
-
 ## 📔 Citation
 
 If you use OpenLLM in your research, we provide a [citation](./CITATION.cff) to
 use:
 
 ```bibtex
 @software{Pham_OpenLLM_Operating_LLMs_2023,
```

#### html2text {}

```diff
@@ -4,119 +4,74 @@
                               _[_T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_]
 ## ð Introduction OpenLLM helps developers **run any open-source LLMs**,
 such as Llama 2 and Mistral, as **OpenAI-compatible API endpoints**, locally
 and in the cloud, optimized for serving throughput and production deployment. -
 ð Support a wide range of open-source LLMs including LLMs fine-tuned with
 your own data - âï¸ OpenAI compatible API endpoints for seamless transition
 from your LLM app to open-source LLMs - ð¥ State-of-the-art serving and
-inference performance - ð¯ Simplified cloud deployment via [BentoML]
-(www.bentoml.com) ![Gif showing OpenLLM Intro](/.github/assets/output.gif)
+inference performance - ð¯ Simplified cloud deployment via [BentoML](https://
+www.bentoml.com) ![Gif showing OpenLLM Intro](/.github/assets/output.gif)
 ## ð¾ TL/DR For starter, we provide two ways to quickly try out OpenLLM: ###
 Jupyter Notebooks Try this [OpenLLM tutorial in Google Colab: Serving Llama 2
 with OpenLLM](https://colab.research.google.com/github/bentoml/OpenLLM/blob/
-main/examples/llama2.ipynb). ### Docker We provide a docker container that
-helps you start running OpenLLM: ```bash docker run --rm -it -p 3000:3000
-ghcr.io/bentoml/openllm start facebook/opt-1.3b --backend pt ``` > [!NOTE] >
-Given you have access to GPUs and have setup [nvidia-docker](https://
-github.com/NVIDIA/nvidia-container-toolkit), you can additionally pass in `--
-gpus` > to use GPU for faster inference and optimization >```bash > docker run
---rm --gpus all -p 3000:3000 -it ghcr.io/bentoml/openllm start HuggingFaceH4/
-zephyr-7b-beta --backend vllm > ``` ## ð Get started The following provides
+main/examples/llama2.ipynb). ## ð Get started The following provides
 instructions for how to get started with OpenLLM locally. ### Prerequisites You
-have installed Python 3.8 (or later) andÂ `pip`. We highly recommend using a
+have installed Python 3.9 (or later) andÂ `pip`. We highly recommend using a
 [Virtual Environment](https://docs.python.org/3/library/venv.html) to prevent
 package conflicts. ### Install OpenLLM Install OpenLLM by using `pip` as
 follows: ```bash pip install openllm ``` To verify the installation, run:
-```bash $ openllm -h Usage: openllm [OPTIONS] COMMAND [ARGS]...
-âââââââ âââââââ
-ââââââââââââ ââââââ âââ ââââ
-ââââ
-ââââââââââââââââââââââââââââââ
-ââââââ âââ âââââ âââââ âââ
-âââââââââââââââââ ââââââ
-ââââââ âââ âââââââââââ âââ
-ââââââââââ ââââââ
-âââââââââââââ âââ
-âââââââââââ ââââââââââââ
-âââââââââââ
-âââââââââââââââââââââââââ
-âââ âââ âââââââ âââ
-âââââââââââ
-ââââââââââââââââââââââââ
-âââ. An open platform for operating large language models in production.
-Fine-tune, serve, deploy, and monitor any LLMs with ease. Options: -v, --
-version Show the version and exit. -h, --help Show this message and exit.
-Commands: build Package a given models into a BentoLLM. import Setup LLM
-interactively. models List all supported models. prune Remove all saved models,
-(and optionally bentos) built with OpenLLM locally. query Query a LLM
-interactively, from a terminal. start Start a LLMServer for any supported LLM.
-Extensions: build-base-container Base image builder for BentoLLM. dive-bentos
-Dive into a BentoLLM. get-containerfile Return Containerfile of any given
-Bento. get-prompt Get the default prompt used by OpenLLM. list-bentos List
-available bentos built by OpenLLM. list-models This is equivalent to openllm
-models... playground OpenLLM Playground. ``` ### Start a LLM server OpenLLM
-allows you to quickly spin up an LLM server using `openllm start`. For example,
-to start aÂ [phi-2](https://huggingface.co/microsoft/phi-2)Â server, run the
-following: ```bash TRUST_REMOTE_CODE=True openllm start microsoft/phi-2 ```
-This starts the server atÂ [http://0.0.0.0:3000/](http://0.0.0.0:3000/).
-OpenLLM downloads the model to the BentoML local Model Store if it has not been
-registered before. To view your local models, run `bentoml models list`. To
-interact with the server, you can visit the web UI atÂ [http://0.0.0.0:3000/]
-(http://0.0.0.0:3000/) or send a request usingÂ `curl`. You can also use
-OpenLLMâs built-in Python client to interact with the server: ```python
-import openllm client = openllm.client.HTTPClient('http://localhost:3000')
-client.query('Explain to me the difference between "further" and "farther"')
-``` Alternatively, use theÂ `openllm query`Â command to query the model:
-```bash export OPENLLM_ENDPOINT=http://localhost:3000 openllm query 'Explain to
-me the difference between "further" and "farther"' ``` OpenLLM seamlessly
+```bash $ openllm -h ``` ### Start a LLM server OpenLLM allows you to quickly
+spin up an LLM server using `openllm start`. For example, to start aÂ [Llama 3
+8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B)Â server, run the
+following: ```bash openllm start meta-llama/Meta-Llama-3-8B ``` To interact
+with the server, you can visit the web UI atÂ [http://0.0.0.0:3000/](http://
+0.0.0.0:3000/) or send a request usingÂ `curl`. You can also use OpenLLMâs
+built-in Python client to interact with the server: ```python import openllm
+client = openllm.HTTPClient('http://localhost:3000') client.generate('Explain
+to me the difference between "further" and "farther"') ``` OpenLLM seamlessly
 supports many models and their variants. You can specify different variants of
 the model to be served. For example: ```bash openllm start -- ``` > [!NOTE] >
 OpenLLM supports specifying fine-tuning weights and quantized weights > for any
 of the supported models as long as they can be loaded with the model >
 architecture. Use theÂ `openllm models`Â command to see the complete list of
-supported > models, their architectures, and their variants. > [!IMPORTANT] >
-If you are testing OpenLLM on CPU, you might want to pass in `DTYPE=float32`.
-By default, > OpenLLM will set model `dtype` to `bfloat16` for the best
-performance. > ```bash > DTYPE=float32 openllm start microsoft/phi-2 > ``` >
-This will also applies to older GPUs. If your GPUs doesn't support `bfloat16`,
-then you also > want to set `DTYPE=float16`. ## ð§© Supported models OpenLLM
-currently supports the following models. By default, OpenLLM doesn't include
-dependencies to run all models. The extra model-specific dependencies can be
-installed with the instructions below. Baichuan ### Quickstart > **Note:**
-Baichuan requires to install with: > ```bash > pip install "openllm[baichuan]"
-> ``` Run the following command to quickly spin up a Baichuan server: ```bash
-TRUST_REMOTE_CODE=True openllm start baichuan-inc/baichuan-7b ``` In a
-different terminal, run the following command to interact with the server:
-```bash export OPENLLM_ENDPOINT=http://localhost:3000 openllm query 'What are
-large language models?' ``` > **Note:** Any Baichuan variants can be deployed
-with OpenLLM. Visit the [HuggingFace Model Hub](https://huggingface.co/
-models?sort=trending&search=baichuan) to see more Baichuan-compatible models.
-### Supported models You can specify any of the following Baichuan models via
-`openllm start`: - [baichuan-inc/baichuan2-7b-base](https://huggingface.co/
-baichuan-inc/baichuan2-7b-base) - [baichuan-inc/baichuan2-7b-chat](https://
-huggingface.co/baichuan-inc/baichuan2-7b-chat) - [baichuan-inc/baichuan2-13b-
-base](https://huggingface.co/baichuan-inc/baichuan2-13b-base) - [baichuan-inc/
-baichuan2-13b-chat](https://huggingface.co/baichuan-inc/baichuan2-13b-chat)
-ChatGLM ### Quickstart > **Note:** ChatGLM requires to install with: > ```bash
-> pip install "openllm[chatglm]" > ``` Run the following command to quickly
-spin up a ChatGLM server: ```bash TRUST_REMOTE_CODE=True openllm start thudm/
-chatglm-6b ``` In a different terminal, run the following command to interact
+supported > models, their architectures, and their variants. ## ð§© Supported
+models OpenLLM currently supports the following models. By default, OpenLLM
+doesn't include dependencies to run all models. The extra model-specific
+dependencies can be installed with the instructions below. Baichuan ###
+Quickstart > **Note:** Baichuan requires to install with: > ```bash > pip
+install "openllm[baichuan]" > ``` Run the following command to quickly spin up
+a Baichuan server: ```bash TRUST_REMOTE_CODE=True openllm start baichuan-inc/
+baichuan-7b ``` In a different terminal, run the following command to interact
 with the server: ```bash export OPENLLM_ENDPOINT=http://localhost:3000 openllm
-query 'What are large language models?' ``` > **Note:** Any ChatGLM variants
+query 'What are large language models?' ``` > **Note:** Any Baichuan variants
 can be deployed with OpenLLM. Visit the [HuggingFace Model Hub](https://
-huggingface.co/models?sort=trending&search=chatglm) to see more ChatGLM-
+huggingface.co/models?sort=trending&search=baichuan) to see more Baichuan-
 compatible models. ### Supported models You can specify any of the following
-ChatGLM models via `openllm start`: - [thudm/chatglm-6b](https://
-huggingface.co/thudm/chatglm-6b) - [thudm/chatglm-6b-int8](https://
-huggingface.co/thudm/chatglm-6b-int8) - [thudm/chatglm-6b-int4](https://
-huggingface.co/thudm/chatglm-6b-int4) - [thudm/chatglm2-6b](https://
-huggingface.co/thudm/chatglm2-6b) - [thudm/chatglm2-6b-int4](https://
-huggingface.co/thudm/chatglm2-6b-int4) - [thudm/chatglm3-6b](https://
-huggingface.co/thudm/chatglm3-6b) Dbrx ### Quickstart > **Note:** Dbrx requires
-to install with: > ```bash > pip install "openllm[dbrx]" > ``` Run the
+Baichuan models via `openllm start`: - [baichuan-inc/baichuan2-7b-base](https:/
+/huggingface.co/baichuan-inc/baichuan2-7b-base) - [baichuan-inc/baichuan2-7b-
+chat](https://huggingface.co/baichuan-inc/baichuan2-7b-chat) - [baichuan-inc/
+baichuan2-13b-base](https://huggingface.co/baichuan-inc/baichuan2-13b-base) -
+[baichuan-inc/baichuan2-13b-chat](https://huggingface.co/baichuan-inc/
+baichuan2-13b-chat) ChatGLM ### Quickstart > **Note:** ChatGLM requires to
+install with: > ```bash > pip install "openllm[chatglm]" > ``` Run the
+following command to quickly spin up a ChatGLM server: ```bash
+TRUST_REMOTE_CODE=True openllm start thudm/chatglm-6b ``` In a different
+terminal, run the following command to interact with the server: ```bash export
+OPENLLM_ENDPOINT=http://localhost:3000 openllm query 'What are large language
+models?' ``` > **Note:** Any ChatGLM variants can be deployed with OpenLLM.
+Visit the [HuggingFace Model Hub](https://huggingface.co/
+models?sort=trending&search=chatglm) to see more ChatGLM-compatible models. ###
+Supported models You can specify any of the following ChatGLM models via
+`openllm start`: - [thudm/chatglm-6b](https://huggingface.co/thudm/chatglm-6b)
+- [thudm/chatglm-6b-int8](https://huggingface.co/thudm/chatglm-6b-int8) -
+[thudm/chatglm-6b-int4](https://huggingface.co/thudm/chatglm-6b-int4) - [thudm/
+chatglm2-6b](https://huggingface.co/thudm/chatglm2-6b) - [thudm/chatglm2-6b-
+int4](https://huggingface.co/thudm/chatglm2-6b-int4) - [thudm/chatglm3-6b]
+(https://huggingface.co/thudm/chatglm3-6b) Dbrx ### Quickstart > **Note:** Dbrx
+requires to install with: > ```bash > pip install "openllm[dbrx]" > ``` Run the
 following command to quickly spin up a Dbrx server: ```bash
 TRUST_REMOTE_CODE=True openllm start databricks/dbrx-instruct ``` In a
 different terminal, run the following command to interact with the server:
 ```bash export OPENLLM_ENDPOINT=http://localhost:3000 openllm query 'What are
 large language models?' ``` > **Note:** Any Dbrx variants can be deployed with
 OpenLLM. Visit the [HuggingFace Model Hub](https://huggingface.co/
 models?sort=trending&search=dbrx) to see more Dbrx-compatible models. ###
@@ -262,35 +217,41 @@
 start`: - [facebook/opt-125m](https://huggingface.co/facebook/opt-125m) -
 [facebook/opt-350m](https://huggingface.co/facebook/opt-350m) - [facebook/opt-
 1.3b](https://huggingface.co/facebook/opt-1.3b) - [facebook/opt-2.7b](https://
 huggingface.co/facebook/opt-2.7b) - [facebook/opt-6.7b](https://huggingface.co/
 facebook/opt-6.7b) - [facebook/opt-66b](https://huggingface.co/facebook/opt-
 66b) Phi ### Quickstart > **Note:** Phi requires to install with: > ```bash >
 pip install "openllm[phi]" > ``` Run the following command to quickly spin up a
-Phi server: ```bash TRUST_REMOTE_CODE=True openllm start microsoft/phi-2 ``` In
-a different terminal, run the following command to interact with the server:
-```bash export OPENLLM_ENDPOINT=http://localhost:3000 openllm query 'What are
-large language models?' ``` > **Note:** Any Phi variants can be deployed with
-OpenLLM. Visit the [HuggingFace Model Hub](https://huggingface.co/
-models?sort=trending&search=phi) to see more Phi-compatible models. ###
-Supported models You can specify any of the following Phi models via `openllm
-start`: - [microsoft/phi-2](https://huggingface.co/microsoft/phi-2) -
-[microsoft/phi-1_5](https://huggingface.co/microsoft/phi-1_5) Qwen ###
-Quickstart > **Note:** Qwen requires to install with: > ```bash > pip install
-"openllm[qwen]" > ``` Run the following command to quickly spin up a Qwen
-server: ```bash TRUST_REMOTE_CODE=True openllm start qwen/Qwen-7B-Chat ``` In a
-different terminal, run the following command to interact with the server:
-```bash export OPENLLM_ENDPOINT=http://localhost:3000 openllm query 'What are
-large language models?' ``` > **Note:** Any Qwen variants can be deployed with
-OpenLLM. Visit the [HuggingFace Model Hub](https://huggingface.co/
-models?sort=trending&search=qwen) to see more Qwen-compatible models. ###
-Supported models You can specify any of the following Qwen models via `openllm
-start`: - [qwen/Qwen-7B-Chat](https://huggingface.co/qwen/Qwen-7B-Chat) -
-[qwen/Qwen-7B-Chat-Int8](https://huggingface.co/qwen/Qwen-7B-Chat-Int8) -
-[qwen/Qwen-7B-Chat-Int4](https://huggingface.co/qwen/Qwen-7B-Chat-Int4) -
+Phi server: ```bash TRUST_REMOTE_CODE=True openllm start microsoft/Phi-3-mini-
+4k-instruct ``` In a different terminal, run the following command to interact
+with the server: ```bash export OPENLLM_ENDPOINT=http://localhost:3000 openllm
+query 'What are large language models?' ``` > **Note:** Any Phi variants can be
+deployed with OpenLLM. Visit the [HuggingFace Model Hub](https://
+huggingface.co/models?sort=trending&search=phi) to see more Phi-compatible
+models. ### Supported models You can specify any of the following Phi models
+via `openllm start`: - [microsoft/Phi-3-mini-4k-instruct](https://
+huggingface.co/microsoft/Phi-3-mini-4k-instruct) - [microsoft/Phi-3-mini-128k-
+instruct](https://huggingface.co/microsoft/Phi-3-mini-128k-instruct) -
+[microsoft/Phi-3-small-8k-instruct](https://huggingface.co/microsoft/Phi-3-
+small-8k-instruct) - [microsoft/Phi-3-small-128k-instruct](https://
+huggingface.co/microsoft/Phi-3-small-128k-instruct) - [microsoft/Phi-3-medium-
+4k-instruct](https://huggingface.co/microsoft/Phi-3-medium-4k-instruct) -
+[microsoft/Phi-3-medium-128k-instruct](https://huggingface.co/microsoft/Phi-3-
+medium-128k-instruct) Qwen ### Quickstart > **Note:** Qwen requires to install
+with: > ```bash > pip install "openllm[qwen]" > ``` Run the following command
+to quickly spin up a Qwen server: ```bash TRUST_REMOTE_CODE=True openllm start
+qwen/Qwen-7B-Chat ``` In a different terminal, run the following command to
+interact with the server: ```bash export OPENLLM_ENDPOINT=http://localhost:3000
+openllm query 'What are large language models?' ``` > **Note:** Any Qwen
+variants can be deployed with OpenLLM. Visit the [HuggingFace Model Hub](https:
+//huggingface.co/models?sort=trending&search=qwen) to see more Qwen-compatible
+models. ### Supported models You can specify any of the following Qwen models
+via `openllm start`: - [qwen/Qwen-7B-Chat](https://huggingface.co/qwen/Qwen-7B-
+Chat) - [qwen/Qwen-7B-Chat-Int8](https://huggingface.co/qwen/Qwen-7B-Chat-Int8)
+- [qwen/Qwen-7B-Chat-Int4](https://huggingface.co/qwen/Qwen-7B-Chat-Int4) -
 [qwen/Qwen-14B-Chat](https://huggingface.co/qwen/Qwen-14B-Chat) - [qwen/Qwen-
 14B-Chat-Int8](https://huggingface.co/qwen/Qwen-14B-Chat-Int8) - [qwen/Qwen-
 14B-Chat-Int4](https://huggingface.co/qwen/Qwen-14B-Chat-Int4) StableLM ###
 Quickstart > **Note:** StableLM requires to install with: > ```bash > pip
 install "openllm[stablelm]" > ``` Run the following command to quickly spin up
 a StableLM server: ```bash TRUST_REMOTE_CODE=True openllm start stabilityai/
 stablelm-tuned-alpha-3b ``` In a different terminal, run the following command
@@ -417,17 +378,17 @@
 designed to integrate with other powerful tools easily. We currently offer
 integration with [OpenAI's Compatible Endpoints](https://platform.openai.com/
 docs/api-reference/completions/object), [LlamaIndex](https://www.llamaindex.ai/
 ), [LangChain](https://github.com/hwchase17/langchain), and [Transformers
 Agents](https://huggingface.co/docs/transformers/transformers_agents). ###
 OpenAI Compatible Endpoints OpenLLM Server can be used as a drop-in replacement
 for OpenAI's API. Simply specify the base_url to `llm-endpoint/v1` and you are
-good to go: ```python import openai client = openai.OpenAI( base_url='http://
-localhost:3000/v1', api_key='na' ) # Here the server is running on localhost:
-3000 completions = client.completions.create( prompt='Write me a tag line for
+good to go: ```python import openai client = openai.OpenAI(base_url='http://
+localhost:3000/v1', api_key='na') # Here the server is running on 0.0.0.0:3000
+completions = client.chat.completions.create( prompt='Write me a tag line for
 an ice cream shop.', model=model, max_tokens=64, stream=stream ) ``` The
 compatible endpoints supports `/completions`, `/chat/completions`, and `/
 models` > [!NOTE] > You can find out OpenAI example clients under the >
 [examples](https://github.com/bentoml/OpenLLM/tree/main/examples) folder. ###
 [LlamaIndex](https://docs.llamaindex.ai/en/stable/examples/llm/openllm/) To
 start a local LLM with `llama_index`, simply use
 `llama_index.llms.openllm.OpenLLM`: ```python import asyncio from
@@ -439,24 +400,16 @@
 `llama_index.llms.openllm.OpenLLMAPI`: ```python from llama_index.llms.openllm
 import OpenLLMAPI ``` > [!NOTE] > All synchronous and asynchronous API from
 `llama_index.llms.LLM` are supported. ### [LangChain](https://
 python.langchain.com/docs/integrations/llms/openllm/) Spin up an OpenLLM
 server, and connect to it by specifying its URL: ```python from langchain.llms
 import OpenLLM llm = OpenLLM(server_url='http://44.23.123.1:3000',
 server_type='http') llm('What is the difference between a duck and a goose? And
-why there are so many Goose in Canada?') ``` ### Transformers Agents OpenLLM
-seamlessly integrates with [Transformers Agents](https://huggingface.co/docs/
-transformers/transformers_agents). > [!WARNING] > The Transformers Agent is
-still at an experimental stage. It is > recommended to install OpenLLM with
-`pip install -r nightly-requirements.txt` > to get the latest API update for
-HuggingFace agent. ```python import transformers agent = transformers.HfAgent
-('http://localhost:3000/hf/agent') # URL that runs the OpenLLM server agent.run
-('Is the following `text` positive or negative?', text="I don't like how this
-models is generate inputs") ``` ![Gif showing Agent integration](/.github/
-assets/agent.gif)
+why there are so many Goose in Canada?') ``` ![Gif showing Agent integration]
+(/.github/assets/agent.gif)
 ## ð Deploying models to production There are several ways to deploy your
 LLMs: ### ð³ Docker container 1. **Building a Bento**: With OpenLLM, you can
 easily build a Bento for a specific model, like `mistralai/Mistral-7B-Instruct-
 v0.1`, using the `build` command.: ```bash openllm build mistralai/Mistral-7B-
 Instruct-v0.1 ``` A [Bento](https://docs.bentoml.com/en/latest/concepts/
 bento.html#what-is-a-bento), in BentoML, is the unit of distribution. It
 packages your program's source code, models, files, artefacts, and
@@ -481,22 +434,14 @@
 is actively maintained by the BentoML team. Feel free to reach out and join us
 in our pursuit to make LLMs more accessible and easy to use ð [Join our
 Slack community!](https://l.bentoml.com/join-slack) ## ð Contributing We
 welcome contributions! If you're interested in enhancing OpenLLM's capabilities
 or have any questions, don't hesitate to reach out in our [discord channel]
 (https://l.bentoml.com/join-openllm-discord). Checkout our [Developer Guide]
 (https://github.com/bentoml/OpenLLM/blob/main/DEVELOPMENT.md) if you wish to
-contribute to OpenLLM's codebase. ## ð Telemetry OpenLLM collects usage data
-to enhance user experience and improve the product. We only report OpenLLM's
-internal API calls and ensure maximum privacy by excluding sensitive
-information. We will never collect user code, model data, or stack traces. For
-usage tracking, check out the [code](https://github.com/bentoml/OpenLLM/blob/
-main/openllm-core/src/openllm_core/utils/analytics.py). You can opt out of
-usage tracking by using the `--do-not-track` CLI option: ```bash openllm
-[command] --do-not-track ``` Or by setting the environment variable
-`OPENLLM_DO_NOT_TRACK=True`: ```bash export OPENLLM_DO_NOT_TRACK=True ``` ##
-ð Citation If you use OpenLLM in your research, we provide a [citation](./
-CITATION.cff) to use: ```bibtex @software{Pham_OpenLLM_Operating_LLMs_2023,
-author = {Pham, Aaron and Yang, Chaoyu and Sheng, Sean and Zhao, Shenyang and
-Lee, Sauyon and Jiang, Bo and Dong, Fog and Guan, Xipeng and Ming, Frost},
-license = {Apache-2.0}, month = jun, title = {{OpenLLM: Operating LLMs in
-production}}, url = {https://github.com/bentoml/OpenLLM}, year = {2023} } ```
+contribute to OpenLLM's codebase. ## ð Citation If you use OpenLLM in your
+research, we provide a [citation](./CITATION.cff) to use: ```bibtex @software
+{Pham_OpenLLM_Operating_LLMs_2023, author = {Pham, Aaron and Yang, Chaoyu and
+Sheng, Sean and Zhao, Shenyang and Lee, Sauyon and Jiang, Bo and Dong, Fog and
+Guan, Xipeng and Ming, Frost}, license = {Apache-2.0}, month = jun, title = {
+{OpenLLM: Operating LLMs in production}}, url = {https://github.com/bentoml/
+OpenLLM}, year = {2023} } ```
```

### Comparing `openllm-0.5.0a9/pyoxidizer.bzl` & `openllm-0.5.1/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/_openllm_tiny/__init__.pyi` & `openllm-0.5.1/src/_openllm_tiny/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/_openllm_tiny/_helpers.py` & `openllm-0.5.1/src/_openllm_tiny/_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,17 @@
   ChatCompletionResponse,
   Delta,
   ErrorResponse,
   NotSupportedError,
   LogProbs,
   UsageInfo,
 )
+from openllm_core._typing_compat import LiteralSerialisation
 from starlette.requests import Request
-from huggingface_hub import scan_cache_dir
+from huggingface_hub import HfApi
 
 if t.TYPE_CHECKING:
   import bentoml
   from vllm import RequestOutput
 
 
 logger = logging.getLogger(__name__)
@@ -324,18 +325,27 @@
 
 
 # NOTE: Check for following supported mapping from here:
 # python -c "from openllm_core._typing_compat import get_type_hints, get_literal_args; from _bentoml_sdk.service.config import ResourceSchema; print(get_literal_args(get_type_hints(ResourceSchema)['gpu_type']))"
 RECOMMENDED_MAPPING = {'nvidia-l4': 24e9, 'nvidia-a10g': 24e9, 'nvidia-tesla-a100': 40e9, 'nvidia-a100-80gb': 80e9}
 
 
-def recommended_instance_type(model_id: str, bentomodel: bentoml.Model | None = None):
+def recommended_instance_type(
+  model_id: str, bentomodel: bentoml.Model | None = None, serialisation: LiteralSerialisation = 'safetensors'
+):
+  extensions = 'safetensors' if serialisation == 'safetensors' else 'pt'
+  api = HfApi()
+
   if bentomodel is not None:
     size = sum(f.stat().st_size for f in pathlib.Path(resolve_filepath(model_id)).glob('**/*') if f.is_file())
   else:
-    info = next(filter(lambda repo: repo.repo_id == model_id, scan_cache_dir().repos))
-    size = info.size_on_disk
+    size = sum(
+      i.size
+      for i in api.get_paths_info(
+        model_id, list(filter(lambda x: x.endswith(f'.{extensions}'), api.list_repo_files(model_id)))
+      )
+    )
 
   # find the first occurence of the gpu_type in the recommended mapping such that "size" should be less than or equal to 70% of the recommended size
   for gpu, max_size in RECOMMENDED_MAPPING.items():
     if size <= max_size * 0.7:
       return gpu
```

### Comparing `openllm-0.5.0a9/src/_openllm_tiny/_llm.py` & `openllm-0.5.1/src/_openllm_tiny/_llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     try:
       async for generations in self._model.generate(
         prompt,
         sampling_params=SamplingParams(**{
           k: config.__getitem__(k) for k in set(inspect.signature(SamplingParams).parameters.keys())
         }),
         request_id=request_id,
-        prompt_token_ids=prompt_token_ids,
+        prompt_token_ids=prompt_token_ids if prompt_token_ids else None,
       ):
         yield generations
     except Exception as err:
       raise RuntimeError(f'Failed to start generation task: {err}') from err
 
   async def generate(
     self,
@@ -196,30 +196,18 @@
     **attrs: t.Any,
   ) -> GenerationOutput:
     if stop is not None:
       attrs.update({'stop': stop})
     if stop_token_ids is not None:
       attrs.update({'stop_token_ids': stop_token_ids})
     config = self.config.model_construct_env(**attrs)
-    texts, token_ids = [[]] * config['n'], [[]] * config['n']
     async for result in self.generate_iterator(
       prompt,
       prompt_token_ids=prompt_token_ids,
       request_id=request_id,
       adapter_name=adapter_name,
       **config.model_dump(),
     ):
-      for output in result.outputs:
-        texts[output.index].append(output.text)
-        token_ids[output.index].extend(output.token_ids)
+      pass
     if (final_result := result) is None:
       raise RuntimeError('No result is returned.')
-    converted = GenerationOutput.from_vllm(final_result)
-    return converted.model_copy(
-      update=dict(
-        prompt=prompt,
-        outputs=[
-          output.model_copy(update=dict(text=''.join(texts[output.index]), token_ids=token_ids[output.index]))
-          for output in converted.outputs
-        ],
-      )
-    )
+    return GenerationOutput.from_vllm(final_result).model_copy(update=dict(prompt=prompt))
```

### Comparing `openllm-0.5.0a9/src/_openllm_tiny/_service.py` & `openllm-0.5.1/src/_openllm_tiny/_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,43 +20,47 @@
 
 try:
   bentomodel = bentoml.models.get(svars.model_id.lower())
   model_id = bentomodel.path
 except Exception:
   bentomodel = None
   model_id = svars.model_id
-LLMConfig = core.AutoConfig.for_model(svars.model_name)
+LLMConfig = core.AutoConfig.from_id(model_id, trust_remote_code=svars.trust_remote_code)
 GenerationInput = core.GenerationInput.from_config(LLMConfig)
 ChatMessages = [
   MessageParam(
     role='system',
     content='You are acting as Ernest Hemmingway. All of your response will follow his and his writing style ONLY.',
   ),
-  MessageParam(role='user', content='Write an essay about Nietzsche and absurdism.'),
+  MessageParam(role='user', content='Write an essay on absurdism and its impact in the 20th century.'),
 ]
 
 app_v1 = FastAPI(
   debug=True,
   version=importlib.metadata.version('openllm'),
   title='OpenAI',
   description='OpenAI Compatible API support',
   contact={'name': 'BentoML Team', 'email': 'contact@bentoml.com'},
 )
 
+if core.utils.get_debug_mode():
+  logger.info('service_config: %s', svars.services_config)
+
 
 @bentoml.mount_asgi_app(app_v1, path='/v1')
 @bentoml.service(name=f"llm-{LLMConfig['start_name']}-service", **svars.services_config)
 class LLMService:
   bentomodel = bentomodel
 
   def __init__(self):
     self.llm = openllm.LLM.from_model(
       model_id,
       dtype=svars.dtype,
       bentomodel=bentomodel,
+      revision=svars.revision,
       serialisation=svars.serialisation,
       quantise=svars.quantise,
       llm_config=LLMConfig,
       trust_remote_code=svars.trust_remote_code,
       max_model_len=svars.max_model_len,
       gpu_memory_utilization=svars.gpu_memory_utilization,
     )
@@ -66,40 +70,50 @@
   async def generate_v1(
     self,
     prompt: str = pydantic.Field(default='What is the meaning of life?', description='Given prompt to generate from'),
     prompt_token_ids: t.Optional[t.List[int]] = None,
     stop: t.Optional[t.List[str]] = None,
     stop_token_ids: t.Optional[t.List[int]] = None,
     request_id: t.Optional[str] = None,
-    llm_config: t.Dict[str, t.Any] = pydantic.Field(default=LLMConfig, description='LLM Config'),
+    llm_config: t.Dict[str, t.Any] = pydantic.Field(default=LLMConfig.model_dump(), description='LLM Config'),
   ) -> core.GenerationOutput:
-    llm_config.update(stop=stop, stop_token_ids=stop_token_ids)
+    if stop:
+      llm_config.update(stop=stop)
+    if stop_token_ids:
+      llm_config.update(stop_token_ids=stop_token_ids)
+
     return await self.llm.generate(
       prompt=prompt, prompt_token_ids=prompt_token_ids, request_id=request_id, **llm_config
     )
 
   @core.utils.api(route='/v1/generate_stream')
   async def generate_stream_v1(
     self,
     prompt: str = pydantic.Field(default='What is the meaning of life?', description='Given prompt to generate from'),
     prompt_token_ids: t.Optional[t.List[int]] = None,
     stop: t.Optional[t.List[str]] = None,
     stop_token_ids: t.Optional[t.List[int]] = None,
     request_id: t.Optional[str] = None,
-    llm_config: t.Dict[str, t.Any] = pydantic.Field(default=LLMConfig, description='LLM Config'),
+    llm_config: t.Dict[str, t.Any] = pydantic.Field(default=LLMConfig.model_dump(), description='LLM Config'),
   ) -> t.AsyncGenerator[str, None]:
-    llm_config.update(stop=stop, stop_token_ids=stop_token_ids)
+    if stop:
+      llm_config.update(stop=stop)
+    if stop_token_ids:
+      llm_config.update(stop_token_ids=stop_token_ids)
 
     _config = LLMConfig.model_construct_env(**core.utils.dict_filter_none(llm_config))
     previous_texts = [''] * _config['n']
     previous_num_tokens = [0] * _config['n']
     finish_reason_sent = [False] * _config['n']
 
     async for generations in self.llm.generate_iterator(
-      prompt=prompt, prompt_token_ids=prompt_token_ids, request_id=request_id, **llm_config
+      prompt=prompt,
+      prompt_token_ids=prompt_token_ids,
+      request_id=request_id,
+      **core.utils.dict_filter_none(llm_config),
     ):
       for output in generations.outputs:
         i = output.index
         if finish_reason_sent[i]:
           continue
         delta_token_ids = output.token_ids[previous_num_tokens[i] :]
         delta_text = output.text[len(previous_texts[i]) :]
```

### Comparing `openllm-0.5.0a9/src/_openllm_tiny/_service_vars.py` & `openllm-0.5.1/src/_openllm_tiny/_service_vars.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import orjson, openllm_core.utils as coreutils
 from openllm_core._typing_compat import LiteralSerialisation, LiteralQuantise
 from _openllm_tiny._llm import Dtype
 
 (
   model_id,
-  model_name,
+  revision,
   quantise,
   serialisation,
   dtype,
   trust_remote_code,
   max_model_len,
   gpu_memory_utilization,
   services_config,
 ) = (
   coreutils.getenv('model_id', var=['MODEL_ID'], return_type=str),
-  coreutils.getenv('model_name', return_type=str),
+  orjson.loads(coreutils.getenv('revision', return_type=str)),
   coreutils.getenv('quantize', var=['QUANTISE'], return_type=LiteralQuantise),
   coreutils.getenv('serialization', default='safetensors', var=['SERIALISATION'], return_type=LiteralSerialisation),
   coreutils.getenv('dtype', default='auto', var=['TORCH_DTYPE'], return_type=Dtype),
   coreutils.check_bool_env('TRUST_REMOTE_CODE', False),
   orjson.loads(coreutils.getenv('max_model_len', default=orjson.dumps(None))),
   orjson.loads(coreutils.getenv('gpu_memory_utilization', default=orjson.dumps(0.9), var=['GPU_MEMORY_UTILISATION'])),
   orjson.loads(coreutils.getenv('services_config', orjson.dumps({}))),
```

### Comparing `openllm-0.5.0a9/src/openllm/__init__.py` & `openllm-0.5.1/src/openllm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,46 +23,43 @@
 __lazy = utils.LazyModule(  # NOTE: update this to sys.modules[__name__] once mypy_extensions can recognize __spec__
   __name__,
   globals()['__file__'],
   {
     'exceptions': [],
     'client': ['HTTPClient', 'AsyncHTTPClient'],
     'bundle': [],
-    'testing': [],
     'utils': ['api'],
-    'entrypoints': ['mount_entrypoints'],
     'serialisation': ['ggml', 'transformers', 'vllm'],
     '_llm': ['LLM'],
     '_deprecated': ['Runner'],
     '_runners': ['runner'],
-    '_quantisation': ['infer_quantisation_config'],
     '_strategies': ['CascadingResourceStrategy', 'get_resource'],
   },
   extra_objects={'COMPILED': COMPILED},
 )
 __all__, __dir__ = __lazy.__all__, __lazy.__dir__
 
 _BREAKING_INTERNAL = ['_service', '_service_vars']
 _NEW_IMPL = ['LLM', *_BREAKING_INTERNAL]
 
-if (_BENTOML_VERSION := utils.pkg.pkg_version_info('bentoml')) > (1, 2):
+if utils.pkg.pkg_version_info('bentoml') > (1, 2):
   import _openllm_tiny as _tiny
 else:
   _tiny = None
 
 
 def __getattr__(name: str) -> _t.Any:
   if name in _NEW_IMPL:
     if utils.getenv('IMPLEMENTATION', default='new_impl') == 'deprecated' or _tiny is None:
       if name in _BREAKING_INTERNAL:
         raise ImportError(
           f'"{name}" is an internal implementation and considered breaking with older OpenLLM. Please migrate your code if you depend on this.'
         )
       _warnings.warn(
-        f'"{name}" is considered deprecated implementation and will be removed in the future. Make sure to upgrade to OpenLLM 0.5.x',
+        f'"{name}" is considered deprecated implementation and could be breaking. See https://github.com/bentoml/OpenLLM for more information on upgrading instruction.',
         DeprecationWarning,
         stacklevel=3,
       )
       return __lazy.__getattr__(name)
     else:
       return getattr(_tiny, name)
   else:
```

### Comparing `openllm-0.5.0a9/src/openllm/__init__.pyi` & `openllm-0.5.1/src/openllm/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 from . import (
   bundle as bundle,
   client as client,
   exceptions as exceptions,
   serialisation as serialisation,
   utils as utils,
-  entrypoints as entrypoints,
 )
 from .serialisation import ggml as ggml, transformers as transformers, vllm as vllm
 from ._deprecated import Runner as Runner
 from ._runners import runner as runner
 from ._quantisation import infer_quantisation_config as infer_quantisation_config
 from ._strategies import CascadingResourceStrategy as CascadingResourceStrategy, get_resource as get_resource
 from _openllm_tiny import LLM as LLM
```

### Comparing `openllm-0.5.0a9/src/openllm/_deprecated.py` & `openllm-0.5.1/src/openllm/_deprecated.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_generation.py` & `openllm-0.5.1/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_llm.py` & `openllm-0.5.1/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_llm.pyi` & `openllm-0.5.1/src/openllm/_llm.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_quantisation.py` & `openllm-0.5.1/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_quantisation.pyi` & `openllm-0.5.1/src/openllm/_quantisation.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_runners.py` & `openllm-0.5.1/src/openllm/_runners.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_runners.pyi` & `openllm-0.5.1/src/openllm/_runners.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_strategies.py` & `openllm-0.5.1/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/_strategies.pyi` & `openllm-0.5.1/src/openllm/_strategies.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/utils.py` & `openllm-0.5.1/src/openllm/utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/utils.pyi` & `openllm-0.5.1/src/openllm/utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/bundle/__init__.py` & `openllm-0.5.1/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/bundle/__init__.pyi` & `openllm-0.5.1/src/openllm/bundle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/bundle/_package.py` & `openllm-0.5.1/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/bundle/_package.pyi` & `openllm-0.5.1/src/openllm/bundle/_package.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/serialisation/__init__.py` & `openllm-0.5.1/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/serialisation/__init__.pyi` & `openllm-0.5.1/src/openllm/serialisation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/serialisation/_helpers.py` & `openllm-0.5.1/src/openllm/serialisation/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/serialisation/transformers/__init__.py` & `openllm-0.5.1/src/openllm/serialisation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/serialisation/transformers/_helpers.py` & `openllm-0.5.1/src/openllm/serialisation/transformers/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/serialisation/transformers/weights.py` & `openllm-0.5.1/src/openllm/serialisation/transformers/weights.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm/serialisation/vllm/__init__.py` & `openllm-0.5.1/src/openllm/serialisation/vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/src/openllm_cli/termui.py` & `openllm-0.5.1/src/_openllm_tiny/_termui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 from __future__ import annotations
-import enum
-import functools
-import logging
-import os
-import typing as t
-
-import click
-import inflection
-import orjson
-
+import enum, functools, logging, os, typing as t
+import click, inflection, orjson
 from openllm_core._typing_compat import DictStrAny, TypedDict
 from openllm_core.utils import get_debug_mode
 
 logger = logging.getLogger('openllm')
 
 
 class Level(enum.IntEnum):
```

### Comparing `openllm-0.5.0a9/.gitignore` & `openllm-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/LICENSE.md` & `openllm-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a9/pyproject.toml` & `openllm-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -34,18 +34,18 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "bentoml[io]>=1.2",
+    "bentoml[io]>=1.2.16",
     "transformers[torch,tokenizers]>=4.36.0",
-    "openllm-client>=0.5.0-alpha.9",
-    "openllm-core>=0.5.0-alpha.9",
+    "openllm-client>=0.5.1",
+    "openllm-core>=0.5.1",
     "safetensors",
     "vllm>=0.4.2",
     "optimum>=1.12.0",
     "accelerate",
     "ghapi",
     "einops",
     "sentencepiece",
@@ -108,15 +108,15 @@
 full = [
     "openllm[agents,awq,baichuan,chatglm,dbrx,dolly-v2,falcon,fine-tune,flan-t5,gemma,ggml,gpt-neox,gptq,grpc,llama,mistral,mixtral,mpt,openai,opt,phi,playground,qwen,stablelm,starcoder,vllm,yi]",
 ]
 gemma = ["xformers"]
 ggml = ["ctransformers"]
 gpt-neox = ["xformers"]
 gptq = ["auto-gptq[triton]>=0.4.2"]
-grpc = ["bentoml[grpc]>=1.2"]
+grpc = ["bentoml[grpc]>=1.2.16"]
 llama = ["xformers"]
 mistral = ["xformers"]
 mixtral = ["xformers"]
 mpt = ["triton"]
 openai = ["openai[datalib]>=1", "tiktoken", "fastapi"]
 opt = ["triton"]
 phi = ["triton"]
@@ -146,53 +146,14 @@
 [tool.hatch.metadata]
 allow-direct-references = true
 [tool.hatch.build.targets.wheel]
 only-include = ["src/openllm", "src/openllm_cli", "src/_openllm_tiny"]
 sources = ["src"]
 [tool.hatch.build.targets.sdist]
 exclude = ["/.git_archival.txt", "tests", "/.python-version-default"]
-[tool.hatch.build.targets.wheel.hooks.mypyc]
-dependencies = [
-    "hatch-mypyc==0.16.0",
-    "mypy==1.7.0",
-    # avoid https://github.com/pallets/click/issues/2558
-    "click==8.1.3",
-    "bentoml==1.1.9",
-    "transformers>=4.32.1",
-    "pandas-stubs",
-    "types-psutil",
-    "types-tabulate",
-    "types-PyYAML",
-    "types-protobuf",
-]
-enable-by-default = false
-exclude = ["src/_openllm_tiny/_service.py", "src/openllm/utils/__init__.py"]
-include = [
-    "src/openllm/__init__.py",
-    "src/openllm/_quantisation.py",
-    "src/openllm/_generation.py",
-    "src/openllm/exceptions.py",
-    "src/openllm/testing.py",
-    "src/openllm/utils",
-]
-# NOTE: This is consistent with pyproject.toml
-mypy-args = [
-    "--strict",
-    # this is because all transient library doesn't have types
-    "--follow-imports=skip",
-    "--allow-subclassing-any",
-    "--check-untyped-defs",
-    "--ignore-missing-imports",
-    "--no-warn-return-any",
-    "--warn-unreachable",
-    "--no-warn-no-return",
-    "--no-warn-unused-ignores",
-]
-options = { verbose = true, strip_asserts = true, debug_level = "2", opt_level = "3", include_runtime_files = true }
-require-runtime-dependencies = true
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 # PyPI doesn't support the <picture> tag.
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
 <p align="center">
   <a href="https://github.com/bentoml/openllm">
```

### Comparing `openllm-0.5.0a9/PKG-INFO` & `openllm-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.5.0a9
+Version: 0.5.1
 Summary: OpenLLM: Run any open-source LLMs, such as Llama 2, Mistral, as OpenAI compatible API endpoint in the cloud.
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://discord.gg/openllm
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -35,23 +35,23 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: accelerate
-Requires-Dist: bentoml[io]>=1.2
+Requires-Dist: bentoml[io]>=1.2.16
 Requires-Dist: bitsandbytes<0.42
 Requires-Dist: build[virtualenv]<1
 Requires-Dist: click>=8.1.3
 Requires-Dist: cuda-python; platform_system != 'Darwin'
 Requires-Dist: einops
 Requires-Dist: ghapi
-Requires-Dist: openllm-client>=0.5.0-alpha.9
-Requires-Dist: openllm-core>=0.5.0-alpha.9
+Requires-Dist: openllm-client>=0.5.1
+Requires-Dist: openllm-core>=0.5.1
 Requires-Dist: optimum>=1.12.0
 Requires-Dist: safetensors
 Requires-Dist: scipy
 Requires-Dist: sentencepiece
 Requires-Dist: transformers[tokenizers,torch]>=4.36.0
 Requires-Dist: vllm>=0.4.2
 Provides-Extra: agents
@@ -86,15 +86,15 @@
 Provides-Extra: ggml
 Requires-Dist: ctransformers; extra == 'ggml'
 Provides-Extra: gpt-neox
 Requires-Dist: xformers; extra == 'gpt-neox'
 Provides-Extra: gptq
 Requires-Dist: auto-gptq[triton]>=0.4.2; extra == 'gptq'
 Provides-Extra: grpc
-Requires-Dist: bentoml[grpc]>=1.2; extra == 'grpc'
+Requires-Dist: bentoml[grpc]>=1.2.16; extra == 'grpc'
 Provides-Extra: llama
 Requires-Dist: xformers; extra == 'llama'
 Provides-Extra: mistral
 Requires-Dist: xformers; extra == 'mistral'
 Provides-Extra: mixtral
 Requires-Dist: xformers; extra == 'mixtral'
 Provides-Extra: mpt
@@ -151,151 +151,82 @@
     </a>
 </div>
 
 ## 📖 Introduction
 
 OpenLLM helps developers **run any open-source LLMs**, such as Llama 2 and Mistral, as **OpenAI-compatible API endpoints**, locally and in the cloud, optimized for serving throughput and production deployment.
 
-
 - 🚂 Support a wide range of open-source LLMs including LLMs fine-tuned with your own data
 - ⛓️ OpenAI compatible API endpoints for seamless transition from your LLM app to open-source LLMs
 - 🔥 State-of-the-art serving and inference performance
-- 🎯 Simplified cloud deployment via [BentoML](www.bentoml.com)
-
+- 🎯 Simplified cloud deployment via [BentoML](https://www.bentoml.com)
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/bentoml/openllm/main/.github/assets/output.gif" alt="Gif showing OpenLLM Intro" />
 </p>
 
 ## 💾 TL/DR
 
 For starter, we provide two ways to quickly try out OpenLLM:
 
 ### Jupyter Notebooks
 
 Try this [OpenLLM tutorial in Google Colab: Serving Llama 2 with OpenLLM](https://colab.research.google.com/github/bentoml/OpenLLM/blob/main/examples/llama2.ipynb).
 
-### Docker
-
-We provide a docker container that helps you start running OpenLLM:
-
-```bash
-docker run --rm -it -p 3000:3000 ghcr.io/bentoml/openllm start facebook/opt-1.3b --backend pt
-```
-
-> [!NOTE]
-> Given you have access to GPUs and have setup [nvidia-docker](https://github.com/NVIDIA/nvidia-container-toolkit),  you can additionally pass in `--gpus`
-> to use GPU for faster inference and optimization
->```bash
-> docker run --rm --gpus all -p 3000:3000 -it ghcr.io/bentoml/openllm start HuggingFaceH4/zephyr-7b-beta --backend vllm
-> ```
-
-
 ## 🏃 Get started
 
 The following provides instructions for how to get started with OpenLLM locally.
 
 ### Prerequisites
 
-You have installed Python 3.8 (or later) and `pip`. We highly recommend using a [Virtual Environment](https://docs.python.org/3/library/venv.html) to prevent package conflicts.
+You have installed Python 3.9 (or later) and `pip`. We highly recommend using a [Virtual Environment](https://docs.python.org/3/library/venv.html) to prevent package conflicts.
 
 ### Install OpenLLM
 
 Install OpenLLM by using `pip` as follows:
 
 ```bash
 pip install openllm
 ```
 
 To verify the installation, run:
 
 ```bash
 $ openllm -h
-
-Usage: openllm [OPTIONS] COMMAND [ARGS]...
-
-   ██████╗ ██████╗ ███████╗███╗   ██╗██╗     ██╗     ███╗   ███╗
-  ██╔═══██╗██╔══██╗██╔════╝████╗  ██║██║     ██║     ████╗ ████║
-  ██║   ██║██████╔╝█████╗  ██╔██╗ ██║██║     ██║     ██╔████╔██║
-  ██║   ██║██╔═══╝ ██╔══╝  ██║╚██╗██║██║     ██║     ██║╚██╔╝██║
-  ╚██████╔╝██║     ███████╗██║ ╚████║███████╗███████╗██║ ╚═╝ ██║
-   ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝╚═╝     ╚═╝.
-
-  An open platform for operating large language models in production.
-  Fine-tune, serve, deploy, and monitor any LLMs with ease.
-
-Options:
-  -v, --version  Show the version and exit.
-  -h, --help     Show this message and exit.
-
-Commands:
-  build       Package a given models into a BentoLLM.
-  import      Setup LLM interactively.
-  models      List all supported models.
-  prune       Remove all saved models, (and optionally bentos) built with OpenLLM locally.
-  query       Query a LLM interactively, from a terminal.
-  start       Start a LLMServer for any supported LLM.
-
-Extensions:
-  build-base-container  Base image builder for BentoLLM.
-  dive-bentos           Dive into a BentoLLM.
-  get-containerfile     Return Containerfile of any given Bento.
-  get-prompt            Get the default prompt used by OpenLLM.
-  list-bentos           List available bentos built by OpenLLM.
-  list-models           This is equivalent to openllm models...
-  playground            OpenLLM Playground.
 ```
 
 ### Start a LLM server
 
-OpenLLM allows you to quickly spin up an LLM server using `openllm start`. For example, to start a [phi-2](https://huggingface.co/microsoft/phi-2) server, run the following:
+OpenLLM allows you to quickly spin up an LLM server using `openllm start`. For example, to start a [Llama 3 8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B) server, run the following:
 
 ```bash
-TRUST_REMOTE_CODE=True openllm start microsoft/phi-2
+openllm start meta-llama/Meta-Llama-3-8B
 ```
 
-This starts the server at [http://0.0.0.0:3000/](http://0.0.0.0:3000/). OpenLLM downloads the model to the BentoML local Model Store if it has not been registered before. To view your local models, run `bentoml models list`.
-
 To interact with the server, you can visit the web UI at [http://0.0.0.0:3000/](http://0.0.0.0:3000/) or send a request using `curl`. You can also use OpenLLM’s built-in Python client to interact with the server:
 
 ```python
 import openllm
 
-client = openllm.client.HTTPClient('http://localhost:3000')
-client.query('Explain to me the difference between "further" and "farther"')
-```
-
-Alternatively, use the `openllm query` command to query the model:
-
-```bash
-export OPENLLM_ENDPOINT=http://localhost:3000
-openllm query 'Explain to me the difference between "further" and "farther"'
+client = openllm.HTTPClient('http://localhost:3000')
+client.generate('Explain to me the difference between "further" and "farther"')
 ```
 
 OpenLLM seamlessly supports many models and their variants. You can specify different variants of the model to be served. For example:
 
 ```bash
 openllm start <model_id> --<options>
 ```
 
 > [!NOTE]
 > OpenLLM supports specifying fine-tuning weights and quantized weights
 > for any of the supported models as long as they can be loaded with the model
 > architecture. Use the `openllm models` command to see the complete list of supported
 > models, their architectures, and their variants.
 
-> [!IMPORTANT]
-> If you are testing OpenLLM on CPU, you might want to pass in `DTYPE=float32`. By default,
-> OpenLLM will set model `dtype` to `bfloat16` for the best performance.
-> ```bash
-> DTYPE=float32 openllm start microsoft/phi-2
-> ```
-> This will also applies to older GPUs. If your GPUs doesn't support `bfloat16`, then you also
-> want to set `DTYPE=float16`.
-
 ## 🧩 Supported models
 
 OpenLLM currently supports the following models. By default, OpenLLM doesn't include dependencies to run all models. The extra model-specific dependencies can be installed with the instructions below.
 
 <!-- update-readme.py: start -->
 <details>
 
@@ -868,15 +799,15 @@
 > pip install "openllm[phi]"
 > ```
 
 
 Run the following command to quickly spin up a Phi server:
 
 ```bash
-TRUST_REMOTE_CODE=True openllm start microsoft/phi-2
+TRUST_REMOTE_CODE=True openllm start microsoft/Phi-3-mini-4k-instruct
 ```
 In a different terminal, run the following command to interact with the server:
 
 ```bash
 export OPENLLM_ENDPOINT=http://localhost:3000
 openllm query 'What are large language models?'
 ```
@@ -887,16 +818,20 @@
 
 
 ### Supported models
 
 You can specify any of the following Phi models via `openllm start`:
 
 
-- [microsoft/phi-2](https://huggingface.co/microsoft/phi-2)
-- [microsoft/phi-1_5](https://huggingface.co/microsoft/phi-1_5)
+- [microsoft/Phi-3-mini-4k-instruct](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)
+- [microsoft/Phi-3-mini-128k-instruct](https://huggingface.co/microsoft/Phi-3-mini-128k-instruct)
+- [microsoft/Phi-3-small-8k-instruct](https://huggingface.co/microsoft/Phi-3-small-8k-instruct)
+- [microsoft/Phi-3-small-128k-instruct](https://huggingface.co/microsoft/Phi-3-small-128k-instruct)
+- [microsoft/Phi-3-medium-4k-instruct](https://huggingface.co/microsoft/Phi-3-medium-4k-instruct)
+- [microsoft/Phi-3-medium-128k-instruct](https://huggingface.co/microsoft/Phi-3-medium-128k-instruct)
 
 </details>
 
 <details>
 
 <summary>Qwen</summary>
 
@@ -1217,15 +1152,14 @@
 ```bash
 openllm build facebook/opt-6.7b --adapter-id ./path/to/adapter_id --build-ctx .
 ```
 
 > [!IMPORTANT]
 > Fine-tuning support is still experimental and currently only works with PyTorch backend. vLLM support is coming soon.
 
-
 ## ⚙️ Integrations
 
 OpenLLM is not just a standalone product; it's a building block designed to
 integrate with other powerful tools easily. We currently offer integration with
 [OpenAI's Compatible Endpoints](https://platform.openai.com/docs/api-reference/completions/object),
 [LlamaIndex](https://www.llamaindex.ai/),
 [LangChain](https://github.com/hwchase17/langchain), and
@@ -1235,30 +1169,27 @@
 
 OpenLLM Server can be used as a drop-in replacement for OpenAI's API. Simply
 specify the base_url to `llm-endpoint/v1` and you are good to go:
 
 ```python
 import openai
 
-client = openai.OpenAI(
-  base_url='http://localhost:3000/v1', api_key='na'
-)  # Here the server is running on localhost:3000
+client = openai.OpenAI(base_url='http://localhost:3000/v1', api_key='na')  # Here the server is running on 0.0.0.0:3000
 
-completions = client.completions.create(
+completions = client.chat.completions.create(
   prompt='Write me a tag line for an ice cream shop.', model=model, max_tokens=64, stream=stream
 )
 ```
 
 The compatible endpoints supports `/completions`, `/chat/completions`, and `/models`
 
 > [!NOTE]
 > You can find out OpenAI example clients under the
 > [examples](https://github.com/bentoml/OpenLLM/tree/main/examples) folder.
 
-
 ### [LlamaIndex](https://docs.llamaindex.ai/en/stable/examples/llm/openllm/)
 
 To start a local LLM with `llama_index`, simply use `llama_index.llms.openllm.OpenLLM`:
 
 ```python
 import asyncio
 from llama_index.llms.openllm import OpenLLM
@@ -1292,32 +1223,14 @@
 ```python
 from langchain.llms import OpenLLM
 
 llm = OpenLLM(server_url='http://44.23.123.1:3000', server_type='http')
 llm('What is the difference between a duck and a goose? And why there are so many Goose in Canada?')
 ```
 
-### Transformers Agents
-
-OpenLLM seamlessly integrates with
-[Transformers Agents](https://huggingface.co/docs/transformers/transformers_agents).
-
-> [!WARNING]
-> The Transformers Agent is still at an experimental stage. It is
-> recommended to install OpenLLM with `pip install -r nightly-requirements.txt`
-> to get the latest API update for HuggingFace agent.
-
-```python
-import transformers
-
-agent = transformers.HfAgent('http://localhost:3000/hf/agent')  # URL that runs the OpenLLM server
-
-agent.run('Is the following `text` positive or negative?', text="I don't like how this models is generate inputs")
-```
-
 <p align="center">
   <img src="https://raw.githubusercontent.com/bentoml/openllm/main/.github/assets/agent.gif" alt="Gif showing Agent integration" />
 </p>
 
 ## 🚀 Deploying models to production
 
 There are several ways to deploy your LLMs:
@@ -1396,34 +1309,14 @@
 capabilities or have any questions, don't hesitate to reach out in our
 [discord channel](https://l.bentoml.com/join-openllm-discord).
 
 Checkout our
 [Developer Guide](https://github.com/bentoml/OpenLLM/blob/main/DEVELOPMENT.md)
 if you wish to contribute to OpenLLM's codebase.
 
-## 🍇 Telemetry
-
-OpenLLM collects usage data to enhance user experience and improve the product.
-We only report OpenLLM's internal API calls and ensure maximum privacy by
-excluding sensitive information. We will never collect user code, model data, or
-stack traces. For usage tracking, check out the
-[code](https://github.com/bentoml/OpenLLM/blob/main/openllm-core/src/openllm_core/utils/analytics.py).
-
-You can opt out of usage tracking by using the `--do-not-track` CLI option:
-
-```bash
-openllm [command] --do-not-track
-```
-
-Or by setting the environment variable `OPENLLM_DO_NOT_TRACK=True`:
-
-```bash
-export OPENLLM_DO_NOT_TRACK=True
-```
-
 ## 📔 Citation
 
 If you use OpenLLM in your research, we provide a [citation](./CITATION.cff) to
 use:
 
 ```bibtex
 @software{Pham_OpenLLM_Operating_LLMs_2023,
@@ -1436,26 +1329,20 @@
 }
 ```
 
 ## Release Information
 
 ### Backwards-incompatible Changes
 
-- ### openllm-core
-
-  Bump `attrs` to `23.2.0`
-
-  Added experimental helpers `.pydantic_model()` functions to convert current attrs-based class to its compatible pydantic class.
-
-  ### openllm
+- Now, OpenLLM is compatible with BentoML 1.2 and above architecture.
 
-  Updated OpenLLM architecture to new 1.2 BentoML.
+  Additionally, `openllm` CLI will only offer `start` and `build` to simplify the workflow.
 
-  `openllm.Runner` remains the old Runnable implementation. Therefore, if you still depends on the old architecture, make sure to use `openllm.Runner` instead of `llm.runner`.
+  OpenLLM will also now require vllm by default, and CPU support is currently turning off. We will look into supporting CPU in later version as our main focus is on accelerator.
 
-  `llm.runner` will now become an `bentoml.depends()` singleton, therefore, to avoid breaking change, make sure to set `OPENLLM_RUNNER_BEHAVIOUR=deprecated` in your environment variable. This is the default behaviour. To opt-in the new architecture, set `OPENLLM_RUNNER_BEHAVIOUR=new_impl`
-  [#821](https://github.com/bentoml/openllm/issues/821)
+  Python API is also considered deprecated and internal only. If you are using this in your old service, make sure to set `IMPLEMENTATION=deprecated` as environment variable to avoid breaking changes. We recommend users to upgrade to BentoML 1.2.
+  [#996](https://github.com/bentoml/openllm/issues/996)
 
 
 ---
 
 [Click me for full changelog](https://github.com/bentoml/openllm/blob/main/CHANGELOG.md)
```

