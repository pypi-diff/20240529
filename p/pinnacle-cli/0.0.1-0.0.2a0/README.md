# Comparing `tmp/pinnacle_cli-0.0.1.tar.gz` & `tmp/pinnacle_cli-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinnacle_cli-0.0.1.tar", max compression
+gzip compressed data, was "pinnacle_cli-0.0.2a0.tar", max compression
```

## Comparing `pinnacle_cli-0.0.1.tar` & `pinnacle_cli-0.0.2a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2600 2024-05-29 17:20:05.770602 pinnacle_cli-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-29 17:20:05.770697 pinnacle_cli-0.0.1/pinnacle_cli/__init__.py
--rw-r--r--   0        0        0      185 2024-05-29 17:20:05.771088 pinnacle_cli-0.0.1/pinnacle_cli/constants.py
--rw-r--r--   0        0        0     1660 2024-05-29 17:20:05.771365 pinnacle_cli-0.0.1/pinnacle_cli/dev.py
--rw-r--r--   0        0        0      603 2024-05-29 17:20:05.771620 pinnacle_cli-0.0.1/pinnacle_cli/main.py
--rw-r--r--   0        0        0      431 2024-05-29 17:20:05.772982 pinnacle_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 pinnacle_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2600 2024-05-29 17:32:40.661734 pinnacle_cli-0.0.2a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 17:32:40.661832 pinnacle_cli-0.0.2a0/pinnacle_cli/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-29 17:32:40.662008 pinnacle_cli-0.0.2a0/pinnacle_cli/constants.py
+-rw-r--r--   0        0        0     1689 2024-05-29 17:33:08.817555 pinnacle_cli-0.0.2a0/pinnacle_cli/dev.py
+-rw-r--r--   0        0        0      603 2024-05-29 17:32:40.662280 pinnacle_cli-0.0.2a0/pinnacle_cli/main.py
+-rw-r--r--   0        0        0      433 2024-05-29 17:35:05.561252 pinnacle_cli-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 pinnacle_cli-0.0.2a0/PKG-INFO
```

### Comparing `pinnacle_cli-0.0.1/README.md` & `pinnacle_cli-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `pinnacle_cli-0.0.1/pinnacle_cli/dev.py` & `pinnacle_cli-0.0.2a0/pinnacle_cli/dev.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 for filename in os.listdir(DIRECTORY):
     if filename.endswith(".py"):
         module_name = os.path.splitext(filename)[0]
         module_parent = (
             DIRECTORY[2:] if DIRECTORY.startswith("./") else DIRECTORY
         ).replace("/", ".")
-        importlib.import_module(f"{module_parent}.{module_name}")
+        importlib.import_module(f"{module_parent + "" if module_parent else ""}{module_name}")
 
 origins = ["*"]
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
```

### Comparing `pinnacle_cli-0.0.1/pinnacle_cli/main.py` & `pinnacle_cli-0.0.2a0/pinnacle_cli/main.py`

 * *Files identical despite different names*

### Comparing `pinnacle_cli-0.0.1/PKG-INFO` & `pinnacle_cli-0.0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinnacle-cli
-Version: 0.0.1
+Version: 0.0.2a0
 Summary: 
 Author: Ivan Zhang
 Author-email: ivanzhangofficial@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

