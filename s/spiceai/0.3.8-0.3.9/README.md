# Comparing `tmp/spiceai-0.3.8.tar.gz` & `tmp/spiceai-0.3.9.tar.gz`

## Comparing `spiceai-0.3.8.tar` & `spiceai-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.8/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.8/scripts/mytoml.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.8/scripts/prompt.txt
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.8/scripts/run.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/errors.py
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/models.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/providers.py
--rw-r--r--   0        0        0    36631 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/spice.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/spice_message.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/utils.py
--rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/wrapped_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 spiceai-0.3.8/tests/conftest.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 spiceai-0.3.8/tests/test_spice.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.8/LICENSE
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.8/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.9/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.9/scripts/mytoml.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.9/scripts/prompt.txt
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.9/scripts/run.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.9/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.9/spice/errors.py
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.9/spice/models.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.9/spice/providers.py
+-rw-r--r--   0        0        0    36703 2020-02-02 00:00:00.000000 spiceai-0.3.9/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.9/spice/spice_message.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 spiceai-0.3.9/spice/utils.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.9/spice/wrapped_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 spiceai-0.3.9/tests/conftest.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 spiceai-0.3.9/tests/test_spice.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.9/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.9/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.9/PKG-INFO
```

### Comparing `spiceai-0.3.8/.github/workflows/ruff.yml` & `spiceai-0.3.9/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/scripts/run.py` & `spiceai-0.3.9/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/spice/errors.py` & `spiceai-0.3.9/spice/errors.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/spice/models.py` & `spiceai-0.3.9/spice/models.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/spice/providers.py` & `spiceai-0.3.9/spice/providers.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/spice/spice.py` & `spiceai-0.3.9/spice/spice.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
     def _log_response(self, response: SpiceResponse, name: Optional[str] = None):
         base_name = "spice" if name is None else name
 
         if self.logging_dir is not None:
             full_name = f"{base_name}_{self._cur_logged_names[base_name]}.json"
             self._cur_logged_names[base_name] += 1
             response_dict = dataclasses.asdict(response)
+            response_dict.pop("_result", "")  # May not be serializable
             response_json = json.dumps(response_dict, cls=MessagesEncoder)
 
             logging_dir = self.logging_dir / self._cur_run
             logging_dir.mkdir(exist_ok=True, parents=True)
             with (logging_dir / full_name).open("w") as file:
                 file.write(f"{response_json}\n")
         if self.logging_callback is not None:
```

### Comparing `spiceai-0.3.8/spice/spice_message.py` & `spiceai-0.3.9/spice/spice_message.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/spice/utils.py` & `spiceai-0.3.9/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/spice/wrapped_clients.py` & `spiceai-0.3.9/spice/wrapped_clients.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/tests/conftest.py` & `spiceai-0.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/tests/test_spice.py` & `spiceai-0.3.9/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/LICENSE` & `spiceai-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/README.md` & `spiceai-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.8/pyproject.toml` & `spiceai-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch]
 
 [tool.hatch.build.targets.wheel]
 packages=["spice"]
 
 [project]
 name = "spiceai"
-version = "0.3.8"
+version = "0.3.9"
 license = {text = "Apache-2.0"}
 description = "A Python library for building AI-powered applications."
 readme = "README.md"
 dependencies = [
     "python-dotenv",
     "openai",
     "anthropic",
```

### Comparing `spiceai-0.3.8/PKG-INFO` & `spiceai-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: httpx
 Requires-Dist: jinja2
 Requires-Dist: openai
```

