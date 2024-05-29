# Comparing `tmp/mypy_boto3_glue-1.34.84.tar.gz` & `tmp/mypy_boto3_glue-1.34.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_glue-1.34.84.tar", last modified: Fri Apr 12 19:32:35 2024, max compression
+gzip compressed data, was "mypy_boto3_glue-1.34.88.tar", last modified: Fri Apr 19 19:32:14 2024, max compression
```

## Comparing `mypy_boto3_glue-1.34.84.tar` & `mypy_boto3_glue-1.34.88.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.941305 mypy_boto3_glue-1.34.84/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-12 19:32:35.937305 mypy_boto3_glue-1.34.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.937305 mypy_boto3_glue-1.34.84/mypy_boto3_glue/
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   145215 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   145212 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   238323 2024-04-12 19:32:06.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   238323 2024-04-12 19:32:04.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.937305 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:35.941305 mypy_boto3_glue-1.34.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.001938 mypy_boto3_glue-1.34.88/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 19:31:52.000000 mypy_boto3_glue-1.34.88/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-19 19:32:14.001938 mypy_boto3_glue-1.34.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-19 19:31:52.000000 mypy_boto3_glue-1.34.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.001938 mypy_boto3_glue-1.34.88/mypy_boto3_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-19 19:31:52.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-19 19:31:52.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-19 19:31:52.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145215 2024-04-19 19:31:54.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145212 2024-04-19 19:31:53.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-19 19:31:54.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-19 19:31:54.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-19 19:31:54.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-19 19:31:54.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:31:52.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   238349 2024-04-19 19:31:59.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238349 2024-04-19 19:31:57.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 19:31:52.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.001938 mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-19 19:32:13.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-19 19:32:13.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:32:13.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:32:13.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 19:32:13.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 19:32:13.000000 mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:32:14.001938 mypy_boto3_glue-1.34.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-19 19:31:52.000000 mypy_boto3_glue-1.34.88/setup.py
```

### Comparing `mypy_boto3_glue-1.34.84/LICENSE` & `mypy_boto3_glue-1.34.88/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/PKG-INFO` & `mypy_boto3_glue-1.34.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.34.84
-Summary: Type annotations for boto3.Glue 1.34.84 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.88
+Summary: Type annotations for boto3.Glue 1.34.88 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_glue-1.34.84/README.md` & `mypy_boto3_glue-1.34.88/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/__init__.py` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/__init__.pyi` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/__main__.py` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glue 1.34.84\n"
-        "Version:         1.34.84\n"
+        "Type annotations for boto3.Glue 1.34.88\n"
+        "Version:         1.34.88\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.84")
+    print("1.34.88")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/client.py` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/client.pyi` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/literals.py` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/literals.pyi` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/paginator.py` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/paginator.pyi` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/type_defs.py` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7309,14 +7309,15 @@
         "IsRegisteredWithLakeFormation": bool,
         "CellFilters": List[ColumnRowFilterTypeDef],
         "QueryAuthorizationId": str,
         "IsMultiDialectView": bool,
         "ResourceArn": str,
         "IsProtected": bool,
         "Permissions": List[PermissionType],
+        "RowFilter": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchTablesResponseTypeDef = TypedDict(
     "SearchTablesResponseTypeDef",
     {
         "NextToken": str,
```

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue/type_defs.pyi` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -7309,14 +7309,15 @@
         "IsRegisteredWithLakeFormation": bool,
         "CellFilters": List[ColumnRowFilterTypeDef],
         "QueryAuthorizationId": str,
         "IsMultiDialectView": bool,
         "ResourceArn": str,
         "IsProtected": bool,
         "Permissions": List[PermissionType],
+        "RowFilter": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchTablesResponseTypeDef = TypedDict(
     "SearchTablesResponseTypeDef",
     {
         "NextToken": str,
```

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/PKG-INFO` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.34.84
-Summary: Type annotations for boto3.Glue 1.34.84 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.88
+Summary: Type annotations for boto3.Glue 1.34.88 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/SOURCES.txt` & `mypy_boto3_glue-1.34.88/mypy_boto3_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_glue-1.34.84/setup.py` & `mypy_boto3_glue-1.34.88/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glue",
-    version="1.34.84",
+    version="1.34.88",
     packages=["mypy_boto3_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Glue 1.34.84 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Glue 1.34.88 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

