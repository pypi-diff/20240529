# Comparing `tmp/kframe-0.5.0rc3.tar.gz` & `tmp/kframe-0.5.0rc5.tar.gz`

## Comparing `kframe-0.5.0rc3.tar` & `kframe-0.5.0rc5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/.tool-versions
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/CHANGELOG.md
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/.github/workflows/main_release.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/__about__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/api/__init__.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/api/apitools.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/collections/__init__.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/collections/collections.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/config/configattr.py
--rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/model/__init__.py
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/src/kframe/model/managedb.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/tests/__init__.py
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/tests/test_config.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/tests/test_secretattr.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/.gitignore
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/LICENSE.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/README.md
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/pyproject.toml
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 kframe-0.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/.tool-versions
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/CHANGELOG.md
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/__about__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/api/__init__.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/api/apitools.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/collections/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/collections/collections.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/model/__init__.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/src/kframe/model/managedb.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/tests/__init__.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/tests/test_config.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/tests/test_secretattr.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/.gitignore
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/LICENSE.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/README.md
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 kframe-0.5.0rc5/PKG-INFO
```

### Comparing `kframe-0.5.0rc3/CHANGELOG.md` & `kframe-0.5.0rc5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v0.5.0rc4 (2024-05-29)
+
+### Feat
+
+- Add DictObject class for accessing dictionary values as attributes
+
 ## v0.5.0rc2 (2024-05-23)
 
 ### Feat
 
 - Add custom collections package
 
 ## v0.5.0a1 (2024-05-22)
```

### Comparing `kframe-0.5.0rc3/.github/workflows/main_ci.yml` & `kframe-0.5.0rc5/.github/workflows/main_ci.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/.github/workflows/main_pre_release.yml` & `kframe-0.5.0rc5/.github/workflows/main_pre_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/.github/workflows/main_release.yml` & `kframe-0.5.0rc5/.github/workflows/main_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/src/kframe/api/apitools.py` & `kframe-0.5.0rc5/src/kframe/api/apitools.py`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/src/kframe/config/configattr.py` & `kframe-0.5.0rc5/src/kframe/config/configattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/src/kframe/config/configentity.py` & `kframe-0.5.0rc5/src/kframe/config/configentity.py`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/src/kframe/model/managedb.py` & `kframe-0.5.0rc5/src/kframe/model/managedb.py`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/tests/test_config.py` & `kframe-0.5.0rc5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/tests/test_secretattr.py` & `kframe-0.5.0rc5/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/LICENSE.txt` & `kframe-0.5.0rc5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/README.md` & `kframe-0.5.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `kframe-0.5.0rc3/pyproject.toml` & `kframe-0.5.0rc5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.5.0rc3"
+version = "0.5.0rc5"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
```

### Comparing `kframe-0.5.0rc3/PKG-INFO` & `kframe-0.5.0rc5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.5.0rc3
+Version: 0.5.0rc5
 Summary: Kaeus development framework
 Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
 Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
 Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
```

