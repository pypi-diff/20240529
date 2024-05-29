# Comparing `tmp/flatpack-3.5.0.tar.gz` & `tmp/flatpack-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.5.0.tar", last modified: Mon May 27 12:31:55 2024, max compression
+gzip compressed data, was "flatpack-3.5.1.tar", last modified: Wed May 29 07:31:15 2024, max compression
```

## Comparing `flatpack-3.5.0.tar` & `flatpack-3.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-27 12:31:55.470226 flatpack-3.5.0/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.0/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5746 2024-05-27 12:31:55.469899 flatpack-3.5.0/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5025 2024-05-27 12:31:06.000000 flatpack-3.5.0/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-27 12:31:55.465823 flatpack-3.5.0/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.0/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.0/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.0/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.0/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-27 12:31:55.467786 flatpack-3.5.0/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.0/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.0/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.0/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.5.0/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-05-25 14:16:18.000000 flatpack-3.5.0/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    33644 2024-05-26 03:22:31.000000 flatpack-3.5.0/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-27 12:31:55.468734 flatpack-3.5.0/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.0/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.0/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.0/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.0/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.0/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.0/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.0/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-27 12:31:55.469457 flatpack-3.5.0/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5746 2024-05-27 12:31:55.000000 flatpack-3.5.0/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-27 12:31:55.000000 flatpack-3.5.0/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-27 12:31:55.000000 flatpack-3.5.0/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-27 12:31:55.000000 flatpack-3.5.0/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-27 12:31:55.000000 flatpack-3.5.0/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-27 12:31:55.000000 flatpack-3.5.0/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-27 12:31:55.470307 flatpack-3.5.0/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-27 12:20:54.000000 flatpack-3.5.0/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.781423 flatpack-3.5.1/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.1/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 07:31:15.781118 flatpack-3.5.1/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5019 2024-05-27 13:05:21.000000 flatpack-3.5.1/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.777463 flatpack-3.5.1/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.1/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.1/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.779296 flatpack-3.5.1/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.1/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.1/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.1/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.5.1/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-05-25 14:16:18.000000 flatpack-3.5.1/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    33779 2024-05-29 07:30:10.000000 flatpack-3.5.1/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.780298 flatpack-3.5.1/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.1/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.1/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.1/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.1/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 07:31:15.780676 flatpack-3.5.1/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-29 07:31:15.000000 flatpack-3.5.1/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-29 07:31:15.781509 flatpack-3.5.1/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-29 07:30:46.000000 flatpack-3.5.1/setup.py
```

### Comparing `flatpack-3.5.0/LICENSE` & `flatpack-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/PKG-INFO` & `flatpack-3.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.0
+Version: 3.5.1
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -66,19 +66,19 @@
 - **Major versions** (`X.0.0`): These signify significant changes or updates.
 - **Minor versions** (`3.X.0`): Introduce new features without breaking compatibility.
 - **Patch versions** (`3.0.X`): Address bug fixes and minor refinements.
 
 This move is not merely about [semantic versioning](https://semver.org/). It is a pledge for clear communication and
 trust with our users. We invite you to explore our new release strategy and appreciate your patience as we evolve.
 
-[Explore the Project on GitHub](https://github.com/romlingroup/flatpack-ai)
+[Explore the Project on GitHub](https://github.com/RomlinGroup/Flatpack)
 
 ## License
 
-This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
+This project is released under [Apache-2.0](https://github.com/RomlinGroup/Flatpack/blob/main/LICENSE).
 
 ## install_requires
 
 **DISCLAIMER:** This information is only a technical reference, not an endorsement or legal advice. Before using any software for commercial purposes, perform compatibility checks and seek legal advice. You are responsible for ensuring compliance with licensing requirements.
 
 Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).
```

### Comparing `flatpack-3.5.0/README.md` & `flatpack-3.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 - **Major versions** (`X.0.0`): These signify significant changes or updates.
 - **Minor versions** (`3.X.0`): Introduce new features without breaking compatibility.
 - **Patch versions** (`3.0.X`): Address bug fixes and minor refinements.
 
 This move is not merely about [semantic versioning](https://semver.org/). It is a pledge for clear communication and
 trust with our users. We invite you to explore our new release strategy and appreciate your patience as we evolve.
 
-[Explore the Project on GitHub](https://github.com/romlingroup/flatpack-ai)
+[Explore the Project on GitHub](https://github.com/RomlinGroup/Flatpack)
 
 ## License
 
-This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
+This project is released under [Apache-2.0](https://github.com/RomlinGroup/Flatpack/blob/main/LICENSE).
 
 ## install_requires
 
 **DISCLAIMER:** This information is only a technical reference, not an endorsement or legal advice. Before using any software for commercial purposes, perform compatibility checks and seek legal advice. You are responsible for ensuring compliance with licensing requirements.
 
 Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).
```

### Comparing `flatpack-3.5.0/flatpack/agent_manager.py` & `flatpack-3.5.1/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/flatpack/datasets.py` & `flatpack-3.5.1/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.5.1/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/flatpack/instructions.py` & `flatpack-3.5.1/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/flatpack/main.py` & `flatpack-3.5.1/flatpack/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,19 +340,24 @@
 def fpk_unbox(directory_name: str, session, local: bool = False):
     """Unbox a flatpack from GitHub or a local directory."""
     if not fpk_valid_directory_name(directory_name):
         print(f"❌ Invalid directory name: '{directory_name}'.")
         return
 
     flatpack_dir = Path.cwd() / directory_name
-    build_dir = flatpack_dir / "build"
 
-    if build_dir.exists():
-        print("❌ Error: Build directory already exists.")
+    if flatpack_dir.exists():
+        print("❌ Error: Flatpack directory already exists.")
         return
+    else:
+        build_dir = flatpack_dir / "build"
+
+        if build_dir.exists():
+            print("❌ Error: Build directory already exists.")
+            return
 
     flatpack_dir.mkdir(parents=True, exist_ok=True)
     build_dir.mkdir(parents=True, exist_ok=True)
 
     temp_toml_path = build_dir / 'temp_flatpack.toml'
     if local:
         toml_path = flatpack_dir / 'flatpack.toml'
```

### Comparing `flatpack-3.5.0/flatpack/modules/lstm.py` & `flatpack-3.5.1/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/flatpack/modules/rnn.py` & `flatpack-3.5.1/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/flatpack/parsers.py` & `flatpack-3.5.1/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/flatpack/vector_manager.py` & `flatpack-3.5.1/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/flatpack.egg-info/PKG-INFO` & `flatpack-3.5.1/flatpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.0
+Version: 3.5.1
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -66,19 +66,19 @@
 - **Major versions** (`X.0.0`): These signify significant changes or updates.
 - **Minor versions** (`3.X.0`): Introduce new features without breaking compatibility.
 - **Patch versions** (`3.0.X`): Address bug fixes and minor refinements.
 
 This move is not merely about [semantic versioning](https://semver.org/). It is a pledge for clear communication and
 trust with our users. We invite you to explore our new release strategy and appreciate your patience as we evolve.
 
-[Explore the Project on GitHub](https://github.com/romlingroup/flatpack-ai)
+[Explore the Project on GitHub](https://github.com/RomlinGroup/Flatpack)
 
 ## License
 
-This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
+This project is released under [Apache-2.0](https://github.com/RomlinGroup/Flatpack/blob/main/LICENSE).
 
 ## install_requires
 
 **DISCLAIMER:** This information is only a technical reference, not an endorsement or legal advice. Before using any software for commercial purposes, perform compatibility checks and seek legal advice. You are responsible for ensuring compliance with licensing requirements.
 
 Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).
```

### Comparing `flatpack-3.5.0/flatpack.egg-info/SOURCES.txt` & `flatpack-3.5.1/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.0/setup.py` & `flatpack-3.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.5.0",
+    version="3.5.1",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "fastapi==0.110.2",
         "hnswlib==0.8.0",
         "httpx==0.27.0",
```

