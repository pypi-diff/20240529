# Comparing `tmp/solar_registry-0.3.3.tar.gz` & `tmp/solar_registry-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.3.3.tar", last modified: Wed May 29 11:08:27 2024, max compression
+gzip compressed data, was "solar_registry-0.3.4.tar", last modified: Wed May 29 11:51:09 2024, max compression
```

## Comparing `solar_registry-0.3.3.tar` & `solar_registry-0.3.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11357 2024-05-29 11:08:03.916610 solar_registry-0.3.3/LICENSE
--rw-r--r--   0        0        0      682 2024-05-29 11:08:03.916610 solar_registry-0.3.3/README.md
--rw-r--r--   0        0        0     1240 2024-05-29 11:08:27.484861 solar_registry-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     2282 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     5891 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0      298 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/model/asset.py
--rw-r--r--   0        0        0     1009 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/model/legacy.py
--rw-r--r--   0        0        0     4538 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/py.typed
--rw-r--r--   0        0        0        0 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     5496 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/service/cos_sync.py
--rw-r--r--   0        0        0     3003 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2699 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      956 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     2069 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-29 11:08:03.920611 solar_registry-0.3.3/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0      383 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/test_cos_sync.py
--rw-r--r--   0        0        0     1512 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/test_merger.py
--rw-r--r--   0        0        0      503 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/test_pr_generator.py
--rw-r--r--   0        0        0     3842 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/test_testtool.py
--rw-r--r--   0        0        0      299 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/test_validator.py
--rw-r--r--   0        0        0      730 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/testdata/error_meta_files/error_yaml_with_loose.yaml
--rw-r--r--   0        0        0     1249 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/testdata/error_meta_files/error_yaml_with_strict.yaml
--rw-r--r--   0        0        0      774 2024-05-29 11:08:03.920611 solar_registry-0.3.3/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml
--rw-r--r--   0        0        0      763 2024-05-29 11:08:03.924610 solar_registry-0.3.3/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml
--rw-r--r--   0        0        0     1401 2024-05-29 11:08:03.924610 solar_registry-0.3.3/tests/testdata/legacy/testtool.yaml
--rw-r--r--   0        0        0     3074 2024-05-29 11:08:03.924610 solar_registry-0.3.3/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-29 11:08:03.924610 solar_registry-0.3.3/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     3090 2024-05-29 11:08:03.924610 solar_registry-0.3.3/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 11:50:43.567829 solar_registry-0.3.4/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-29 11:50:43.567829 solar_registry-0.3.4/README.md
+-rw-r--r--   0        0        0     1240 2024-05-29 11:51:09.067792 solar_registry-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     2282 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     5891 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/model/asset.py
+-rw-r--r--   0        0        0     1009 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/model/legacy.py
+-rw-r--r--   0        0        0     4713 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/py.typed
+-rw-r--r--   0        0        0        0 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     5496 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/service/cos_sync.py
+-rw-r--r--   0        0        0     3003 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2699 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      956 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     2069 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-29 11:50:43.567829 solar_registry-0.3.4/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:50:43.567829 solar_registry-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0      383 2024-05-29 11:50:43.567829 solar_registry-0.3.4/tests/test_cos_sync.py
+-rw-r--r--   0        0        0     1512 2024-05-29 11:50:43.567829 solar_registry-0.3.4/tests/test_merger.py
+-rw-r--r--   0        0        0      503 2024-05-29 11:50:43.567829 solar_registry-0.3.4/tests/test_pr_generator.py
+-rw-r--r--   0        0        0     3880 2024-05-29 11:50:43.567829 solar_registry-0.3.4/tests/test_testtool.py
+-rw-r--r--   0        0        0      299 2024-05-29 11:50:43.567829 solar_registry-0.3.4/tests/test_validator.py
+-rw-r--r--   0        0        0      730 2024-05-29 11:50:43.571829 solar_registry-0.3.4/tests/testdata/error_meta_files/error_yaml_with_loose.yaml
+-rw-r--r--   0        0        0     1249 2024-05-29 11:50:43.571829 solar_registry-0.3.4/tests/testdata/error_meta_files/error_yaml_with_strict.yaml
+-rw-r--r--   0        0        0      774 2024-05-29 11:50:43.571829 solar_registry-0.3.4/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml
+-rw-r--r--   0        0        0      763 2024-05-29 11:50:43.571829 solar_registry-0.3.4/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml
+-rw-r--r--   0        0        0     1418 2024-05-29 11:50:43.571829 solar_registry-0.3.4/tests/testdata/legacy/testtool.yaml
+-rw-r--r--   0        0        0     3074 2024-05-29 11:50:43.571829 solar_registry-0.3.4/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-29 11:50:43.571829 solar_registry-0.3.4/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     3090 2024-05-29 11:50:43.571829 solar_registry-0.3.4/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.3.4/PKG-INFO
```

### Comparing `solar_registry-0.3.3/LICENSE` & `solar_registry-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/README.md` & `solar_registry-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/pyproject.toml` & `solar_registry-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.3.3"
+version = "0.3.4"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.3.3/src/solar_registry/cli.py` & `solar_registry-0.3.4/src/solar_registry/cli.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.3.4/src/solar_registry/commands/meta_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/src/solar_registry/model/legacy.py` & `solar_registry-0.3.4/src/solar_registry/model/legacy.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/src/solar_registry/model/test_tool.py` & `solar_registry-0.3.4/src/solar_registry/model/test_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
     """
     测试工具模型定义
     """
 
     schema_version: float = Field(alias="schemaVersion")
     name: str = Field(pattern=r"^[a-zA-Z-0-9]+$")
+    legacy_name: str = Field("", alias="legacyName")
     description: str = Field(min_length=10, max_length=1000)
 
     # x.x.x 格式版本
     version: str = Field(pattern=r"^(\d+\.\d+\.\d+|stable)$")
     lang: Literal["python", "golang", "javascript", "java"]
     base_image: str = Field(alias="defaultBaseImage")
     lang_type: Literal["COMPILED", "INTERPRETED"] = Field(alias="langType")
@@ -114,14 +115,17 @@
                     raise ValueError("gitPkgUrl must be set")
                 if not self.version_file:
                     raise ValueError("versionFile must be set")
                 if not self.index_file:
                     raise ValueError("indexFile must be set")
                 if not self.scaffold_repo:
                     raise ValueError("scaffoldRepo must be set")
+            else:
+                if not self.legacy_name:
+                    raise ValueError("legacyName must be set")
 
             if not self.name_zh:
                 raise ValueError("name_zh must be set")
 
         return self
```

### Comparing `solar_registry-0.3.3/src/solar_registry/service/cos_sync.py` & `solar_registry-0.3.4/src/solar_registry/service/cos_sync.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/src/solar_registry/service/generator.py` & `solar_registry-0.3.4/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/src/solar_registry/service/pr_generator.py` & `solar_registry-0.3.4/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/src/solar_registry/service/testtool.py` & `solar_registry-0.3.4/src/solar_registry/service/testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/src/solar_registry/service/validator.py` & `solar_registry-0.3.4/src/solar_registry/service/validator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/src/solar_registry/util/file.py` & `solar_registry-0.3.4/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/tests/test_merger.py` & `solar_registry-0.3.4/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/tests/test_testtool.py` & `solar_registry-0.3.4/tests/test_testtool.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     assert param1.value == "初始化命令"
     assert param1.desc == "加载/执行用例前的初始化命令"
     assert param1.default == "# place your extra init command here"
     assert param1.lang == "bash"
     assert param1.input_widget == ParamWidget.Code
 
     assert tool.legacy_spec
+    assert tool.legacy_name == "qt4s"
     assert tool.legacy_spec.report_type == "junit"
     assert tool.legacy_spec.maintainers == ["aa", "bb"]
     assert tool.legacy_spec.testcase_runner.cli == "test"
     assert tool.legacy_spec.testcase_loader.cli == "test"
     assert tool.legacy_spec.testcase_analyzer.cli == "test"
     assert tool.legacy_spec.scaffolding_tool.cli == "test"
     assert tool.legacy_spec.node_setup.cli == "test"
```

### Comparing `solar_registry-0.3.3/tests/testdata/error_meta_files/error_yaml_with_loose.yaml` & `solar_registry-0.3.4/tests/testdata/error_meta_files/error_yaml_with_loose.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/tests/testdata/error_meta_files/error_yaml_with_strict.yaml` & `solar_registry-0.3.4/tests/testdata/error_meta_files/error_yaml_with_strict.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml` & `solar_registry-0.3.4/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml` & `solar_registry-0.3.4/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/tests/testdata/legacy/testtool.yaml` & `solar_registry-0.3.4/tests/testdata/legacy/testtool.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 schemaVersion: 1.0
 name: qt4s
+legacyName: qt4s
 nameZh: qt4s自动化测试
 lang: python
 langType: "INTERPRETED"
 description: qt4s自动化测试工具
 version: '0.1.6'
 defaultBaseImage: python:3.10 # 用户在 TestContainer 配置中未指定 baseImage 时的默认镜像
 indexFile: https://opentestsolar.github.io/testtool-registry/testtools/stable.index.json
```

### Comparing `solar_registry-0.3.3/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.3.4/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.3.4/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.3.4/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.3/PKG-INFO` & `solar_registry-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.3.3
+Version: 0.3.4
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

