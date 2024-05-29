# Comparing `tmp/streamlit_cognite_reveal-0.0.3.tar.gz` & `tmp/streamlit_cognite_reveal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_cognite_reveal-0.0.3.tar", last modified: Wed May 29 08:49:36 2024, max compression
+gzip compressed data, was "streamlit_cognite_reveal-0.0.4.tar", max compression
```

## Comparing `streamlit_cognite_reveal-0.0.3.tar` & `streamlit_cognite_reveal-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,17 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.470049 streamlit_cognite_reveal-0.0.3/
--rw-r--r--   0 kvakkefly   (501) staff       (20)    11357 2024-05-06 10:15:16.000000 streamlit_cognite_reveal-0.0.3/LICENSE
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2829 2024-05-29 08:49:36.469766 streamlit_cognite_reveal-0.0.3/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2139 2024-05-24 14:41:54.000000 streamlit_cognite_reveal-0.0.3/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.428444 streamlit_cognite_reveal-0.0.3/reveal/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1312 2024-05-26 10:33:19.000000 streamlit_cognite_reveal-0.0.3/reveal/RevealConfig.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)       33 2024-05-26 09:38:59.000000 streamlit_cognite_reveal-0.0.3/reveal/TestClass.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4444 2024-05-29 08:47:35.000000 streamlit_cognite_reveal-0.0.3/reveal/__init__.py
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.426128 streamlit_cognite_reveal-0.0.3/reveal/frontend/
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.429864 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1693 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/asset-manifest.json
--rw-r--r--   0 kvakkefly   (501) staff       (20)   197459 2024-05-29 08:48:44.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/bootstrap.min.css
--rw-r--r--   0 kvakkefly   (501) staff       (20)      553 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/index.html
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.426552 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.430546 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/css/
--rw-r--r--   0 kvakkefly   (501) staff       (20)   331112 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/css/main.c81cb3cf.css
--rw-r--r--   0 kvakkefly   (501) staff       (20)   461776 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/css/main.c81cb3cf.css.map
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.444735 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3941 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/114.e0ebff55.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3959 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/142.e332c9ad.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     5176 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/211.ee14119e.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3976 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/413.5c9588ac.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4033 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/463.ad8fb302.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3940 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/690.16ab8bc4.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4753 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/797.fb53d4d2.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4270 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/809.14863d52.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3589 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/82.2b5d6c2f.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3822 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/913.b1b6282c.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3882 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/974.691b1718.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)  5730621 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/main.aaf72a55.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     5906 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/main.aaf72a55.js.LICENSE.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20) 16432189 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/js/main.aaf72a55.js.map
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.467861 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/
--rw-r--r--   0 kvakkefly   (501) staff       (20)   106140 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)   104332 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)   105924 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)    98868 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)   105804 2024-05-29 08:49:20.000000 streamlit_cognite_reveal-0.0.3/reveal/frontend/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-05-29 08:49:36.470104 streamlit_cognite_reveal-0.0.3/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1146 2024-05-29 08:48:45.000000 streamlit_cognite_reveal-0.0.3/setup.py
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-05-29 08:49:36.469030 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2829 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1679 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-05-29 08:49:36.000000 streamlit_cognite_reveal-0.0.3/streamlit_cognite_reveal.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11357 2024-05-06 10:15:16.798098 streamlit_cognite_reveal-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1873 2024-05-29 08:54:42.726917 streamlit_cognite_reveal-0.0.4/README.md
+-rw-r--r--   0        0        0      662 2024-05-29 08:56:31.552331 streamlit_cognite_reveal-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       33 2024-05-26 09:38:59.177839 streamlit_cognite_reveal-0.0.4/reveal/TestClass.py
+-rw-r--r--   0        0        0     3744 2024-05-29 08:54:42.727945 streamlit_cognite_reveal-0.0.4/reveal/__init__.py
+-rw-r--r--   0        0        0      180 2024-05-06 10:15:16.798758 streamlit_cognite_reveal-0.0.4/reveal/frontend/.env
+-rw-r--r--   0        0        0       67 2024-05-06 10:15:16.798860 streamlit_cognite_reveal-0.0.4/reveal/frontend/.prettierrc
+-rw-r--r--   0        0        0      394 2024-05-06 10:15:16.798959 streamlit_cognite_reveal-0.0.4/reveal/frontend/config-overrides.js
+-rw-r--r--   0        0        0     1149 2024-05-29 08:54:42.728186 streamlit_cognite_reveal-0.0.4/reveal/frontend/package.json
+-rw-r--r--   0        0        0   197459 2024-05-06 10:15:16.799611 streamlit_cognite_reveal-0.0.4/reveal/frontend/public/bootstrap.min.css
+-rw-r--r--   0        0        0      894 2024-05-06 10:15:16.800119 streamlit_cognite_reveal-0.0.4/reveal/frontend/public/index.html
+-rw-r--r--   0        0        0     4285 2024-05-29 08:54:42.728473 streamlit_cognite_reveal-0.0.4/reveal/frontend/src/RevealComponent.tsx
+-rw-r--r--   0        0        0      229 2024-05-29 08:54:42.728634 streamlit_cognite_reveal-0.0.4/reveal/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2024-05-06 10:15:16.800473 streamlit_cognite_reveal-0.0.4/reveal/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2024-05-06 10:15:16.800574 streamlit_cognite_reveal-0.0.4/reveal/frontend/tsconfig.json
+-rw-r--r--   0        0        0   541336 2024-05-29 08:54:42.729986 streamlit_cognite_reveal-0.0.4/reveal/frontend/yarn.lock
+-rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 streamlit_cognite_reveal-0.0.4/PKG-INFO
```

### Comparing `streamlit_cognite_reveal-0.0.3/LICENSE` & `streamlit_cognite_reveal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_cognite_reveal-0.0.3/PKG-INFO` & `streamlit_cognite_reveal-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: streamlit-cognite-reveal
-Version: 0.0.3
-Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
-Home-page: 
-Author: Anders Hafreager
-Author-email: anders.hafreager@cognite.com
-Requires-Python: >=3.7
+Version: 0.0.4
+Summary: A component to render Cognite Reveal 3D viewer in Streamlit.
+License: Apache-2.0 license
+Author: Sagar Thalwar
+Author-email: sagar.thalwar@cognite.com
+Requires-Python: >=3.9
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: streamlit (>=0.63)
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: streamlit>=0.63
-Provides-Extra: devel
-Requires-Dist: wheel; extra == "devel"
-Requires-Dist: pytest==7.4.0; extra == "devel"
-Requires-Dist: playwright==1.39.0; extra == "devel"
-Requires-Dist: requests==2.31.0; extra == "devel"
-Requires-Dist: pytest-playwright-snapshot==1.0; extra == "devel"
-Requires-Dist: pytest-rerunfailures==12.0; extra == "devel"
 
 # Cognite 3D Reveal Streamlit
 
 This is a Streamlit library that can be used to show 3D models inside a Streamlit app. It works especially good when used inside Streamlit in Fusion, but can also be used in standalone Streamlit apps.
 
 ## How to install
 
@@ -47,52 +45,42 @@
 ```
 
 ## Local development
 
 It's recommended to add a clean environment. You need `pip` and `node`.
 
 Clone repo
-`git clone https://github.com/cognitedata/streamlit-cognite-reveal.git`
+`git clone https://github.com/cognitedata/hackathon-reveal-streamlit.git`
 
 Install Python packages
 `pip install streamlit`
-`pip install cognite-sdk`
 
 Install NPM packages and start server
 
 ```
-cd reveal/frontend
+cd cognite/streamlit/reveal/frontend
 yarn
 HTTPS=true yarn start
 ```
 
 Then open https://localhost:3001/ to accept bad certificate.
 
 Open repo folder in another terminal. Install this package as development package
 `pip install -e .`
 
 Extract a token from Fusion, and start with
 
-`COGNITE_TOKEN="TOKEN" streamlit run examples/demo.py`
+`COGNITE_TOKEN="TOKEN" streamlit run examples/example.py`
 
 ### Local development in fusion stlite
 
 Make sure you have set (reveal/**init**.py:8)[reveal/__init__.py:8] to `_RELEASE = True`.
 
 Step 1) Build front end component with `cd reveal/frontend && yarn && yarn build`
 Step 2) Build streamlit component with `python -m build` (hint: `pip install build`)
 Step 3) Start local server `python server.py`
 
 Open Fusion, create a Streamlit app and add the following the installed package
 `http://localhost:8000/dist/reveal_streamlit_component-0.0.1-py3-none-any.whl`
 
 It will then load successfully inside Stlite.
 
-## Building a release version
-
-In order to build a packaged release version, follow steps:
-
-Set the 'RELEASE' environment variable to indicate to build system that
-you are building a release version:
-`export RELEASE=1`
-
-<TODO> steps to actually build the package
```

### Comparing `streamlit_cognite_reveal-0.0.3/README.md` & `streamlit_cognite_reveal-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -28,52 +28,41 @@
 ```
 
 ## Local development
 
 It's recommended to add a clean environment. You need `pip` and `node`.
 
 Clone repo
-`git clone https://github.com/cognitedata/streamlit-cognite-reveal.git`
+`git clone https://github.com/cognitedata/hackathon-reveal-streamlit.git`
 
 Install Python packages
 `pip install streamlit`
-`pip install cognite-sdk`
 
 Install NPM packages and start server
 
 ```
-cd reveal/frontend
+cd cognite/streamlit/reveal/frontend
 yarn
 HTTPS=true yarn start
 ```
 
 Then open https://localhost:3001/ to accept bad certificate.
 
 Open repo folder in another terminal. Install this package as development package
 `pip install -e .`
 
 Extract a token from Fusion, and start with
 
-`COGNITE_TOKEN="TOKEN" streamlit run examples/demo.py`
+`COGNITE_TOKEN="TOKEN" streamlit run examples/example.py`
 
 ### Local development in fusion stlite
 
 Make sure you have set (reveal/**init**.py:8)[reveal/__init__.py:8] to `_RELEASE = True`.
 
 Step 1) Build front end component with `cd reveal/frontend && yarn && yarn build`
 Step 2) Build streamlit component with `python -m build` (hint: `pip install build`)
 Step 3) Start local server `python server.py`
 
 Open Fusion, create a Streamlit app and add the following the installed package
 `http://localhost:8000/dist/reveal_streamlit_component-0.0.1-py3-none-any.whl`
 
 It will then load successfully inside Stlite.
-
-## Building a release version
-
-In order to build a packaged release version, follow steps:
-
-Set the 'RELEASE' environment variable to indicate to build system that
-you are building a release version:
-`export RELEASE=1`
-
-<TODO> steps to actually build the package
```

### Comparing `streamlit_cognite_reveal-0.0.3/reveal/__init__.py` & `streamlit_cognite_reveal-0.0.4/reveal/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 import os
-import warnings
-import dataclasses
 import streamlit.components.v1 as components
-from .RevealConfig import RevealConfig
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = bool(os.getenv('RELEASE', False))
-_RELEASE = True
+_RELEASE = False
+
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
 
 # It's worth noting that this call to `declare_component` is the
 # *only thing* you need to do to create the binding between Streamlit and
 # your component frontend. Everything else we do in this file is simply a
 # best practice.
 
 if not _RELEASE:
-    warnings.warn("WARNING: Running in development mode.")
     reveal_func = components.declare_component(
         # We give the component a simple, descriptive name ("my_component"
         # does not fit this bill, so please choose something better for your
         # own component :)
         "reveal",
         # Pass `url` here to tell Streamlit that the component will be served
         # by the local dev server that you run via `npm run start`.
         # (This is useful while your component is in development.)
-        url="https://localhost:3010/",
+        url="https://localhost:3001/",
     )
 else:
     # When we're distributing a production version of the component, we'll
     # replace the `url` param with `path`, and point it to the component's
     # build directory:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
-    build_dir = os.path.join(parent_dir, "frontend", "build")
+    build_dir = os.path.join(parent_dir, "frontend/build")
     reveal_func = components.declare_component("reveal", path=build_dir)
 
-def reveal(client, scene_external_id: str, scene_space: str, config: RevealConfig = None, key=None):
+
+def reveal(client, scene_external_id, scene_space, selected_asset_ids=[], key=None):
     """Create a new instance of Reveal.
 
     Parameters
     ----------
     client: CogniteClient
         The CogniteClient to use
     scene_external_id: string
         External id of the 3D scene
+    selected_asset_ids: int[]
+        List of IDs of assets to select
+
     scene_space: string
         Space id of the 3D scene
-    config: RevealConfig
-        Instance of a RevealConfig dataclass
     key: str or None
         An optional key that uniquely identifies this component. If this is
         None, and the component's arguments are changed, the component will
         be re-mounted in the Streamlit frontend and lose its current state.
 
     Returns
     -------
@@ -76,26 +74,19 @@
     client_config = {
         # TODO replace this with a callback that refeshes token
         # Also; can we get rid of the Bearer evilness?
         "token": client.config.credentials.authorization_header()[1].replace("Bearer ", ""),
         "project": client.config.project,
         "baseUrl": client.config.base_url
     }
-    clipping_plane_arguments = []
-    for clipping_plane in config.clipping_planes:
-        # We only send a list of four numbers, normal + distance
-        clipping_plane_arguments.append([*clipping_plane.normal, clipping_plane.distance])
     component_value = reveal_func(
         client_config=client_config, 
         scene_external_id=scene_external_id, 
-        selected_asset_ids=config.selected_asset_ids,
-        clipping_planes=clipping_plane_arguments,
+        selected_asset_ids=selected_asset_ids,
         scene_space=scene_space, 
-        default_node_appearance=config.default_node_appearance.value,
-        styled_node_collections=[dataclasses.asdict(styled_node_collection) for styled_node_collection in config.styled_node_collections],
         key=key, 
-        default={}
+        default=0
     )
 
     # We could modify the value returned from the component if we wanted.
     # There's no need to do this in our simple example - but it's an option.
     return component_value
```

### Comparing `streamlit_cognite_reveal-0.0.3/reveal/frontend/build/bootstrap.min.css` & `streamlit_cognite_reveal-0.0.4/reveal/frontend/public/bootstrap.min.css`

 * *Files identical despite different names*

