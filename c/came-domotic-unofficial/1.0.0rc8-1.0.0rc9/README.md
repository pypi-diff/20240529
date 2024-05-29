# Comparing `tmp/came_domotic_unofficial-1.0.0rc8.tar.gz` & `tmp/came_domotic_unofficial-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "came_domotic_unofficial-1.0.0rc8.tar", max compression
+gzip compressed data, was "came_domotic_unofficial-1.0.0rc9.tar", max compression
```

## Comparing `came_domotic_unofficial-1.0.0rc8.tar` & `came_domotic_unofficial-1.0.0rc9.tar`

### file list

```diff
@@ -1,19 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-28 23:50:01.862023 came_domotic_unofficial-1.0.0rc8/LICENSE
--rw-r--r--   0        0        0     5155 2024-04-28 23:50:01.862023 came_domotic_unofficial-1.0.0rc8/README.rst
--rw-r--r--   0        0        0     1633 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/__init__.py
--rw-r--r--   0        0        0     9212 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/auth.py
--rw-r--r--   0        0        0     4893 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/came_domotic_api.py
--rw-r--r--   0        0        0     1771 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/errors.py
--rw-r--r--   0        0        0     6343 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models.py
--rw-r--r--   0        0        0     1333 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/came_entity.py
--rw-r--r--   0        0        0     8532 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/digital_input.py
--rw-r--r--   0        0        0     2768 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/enums.py
--rw-r--r--   0        0        0     2002 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/exceptions.py
--rw-r--r--   0        0        0     3589 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/feature.py
--rw-r--r--   0        0        0     1587 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/helpers.py
--rw-r--r--   0        0        0     5930 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/light.py
--rw-r--r--   0        0        0     6451 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/opening.py
--rw-r--r--   0        0        0     6912 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/scenario.py
--rw-r--r--   0        0        0     2856 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/pyproject.toml
--rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 came_domotic_unofficial-1.0.0rc8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-29 00:08:26.081056 came_domotic_unofficial-1.0.0rc9/LICENSE
+-rw-r--r--   0        0        0     5155 2024-04-29 00:08:26.081056 came_domotic_unofficial-1.0.0rc9/README.rst
+-rw-r--r--   0        0        0     1633 2024-04-29 00:08:26.081056 came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/__init__.py
+-rw-r--r--   0        0        0     9212 2024-04-29 00:08:26.081056 came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/auth.py
+-rw-r--r--   0        0        0     4893 2024-04-29 00:08:26.081056 came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/came_domotic_api.py
+-rw-r--r--   0        0        0     1771 2024-04-29 00:08:26.081056 came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/errors.py
+-rw-r--r--   0        0        0     6343 2024-04-29 00:08:26.081056 came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/models.py
+-rw-r--r--   0        0        0     2856 2024-04-29 00:08:26.085056 came_domotic_unofficial-1.0.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 came_domotic_unofficial-1.0.0rc9/PKG-INFO
```

### Comparing `came_domotic_unofficial-1.0.0rc8/LICENSE` & `came_domotic_unofficial-1.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc8/README.rst` & `came_domotic_unofficial-1.0.0rc9/README.rst`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/__init__.py` & `came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/__init__.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/auth.py` & `came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/auth.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/came_domotic_api.py` & `came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/came_domotic_api.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/errors.py` & `came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/errors.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models.py` & `came_domotic_unofficial-1.0.0rc9/came_domotic_unofficial/models.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc8/pyproject.toml` & `came_domotic_unofficial-1.0.0rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
 [tool.poetry]
 name = "came_domotic_unofficial"
-version = "1.0.0rc8"
+version = "1.0.0rc9"
 description = "Python library to interact with a CAME ETI/Domo domotic server."
 license = "Apache-2.0"
 authors = ["camedomotic-unofficial <camedomotic-unofficial@gmail.com>"]
 maintainers = ["camedomotic-unofficial <camedomotic-unofficial@gmail.com>"]
 readme = "README.rst"
 
 homepage = "https://github.com/camedomotic-unofficial/came_domotic_unofficial"
```

### Comparing `came_domotic_unofficial-1.0.0rc8/PKG-INFO` & `came_domotic_unofficial-1.0.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: came_domotic_unofficial
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Python library to interact with a CAME ETI/Domo domotic server.
 Home-page: https://github.com/camedomotic-unofficial/came_domotic_unofficial
 License: Apache-2.0
 Keywords: CAME,ETI/Domo,domotic,home automation,home assistant,home-assistant
 Author: camedomotic-unofficial
 Author-email: camedomotic-unofficial@gmail.com
 Maintainer: camedomotic-unofficial
```

