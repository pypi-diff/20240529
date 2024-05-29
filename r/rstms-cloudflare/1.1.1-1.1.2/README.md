# Comparing `tmp/rstms_cloudflare-1.1.1.tar.gz` & `tmp/rstms_cloudflare-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_cloudflare-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_cloudflare-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_cloudflare-1.1.1.tar` & `rstms_cloudflare-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      383 2024-05-21 05:24:31.576371 rstms_cloudflare-1.1.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1344 2024-05-21 01:52:37.934629 rstms_cloudflare-1.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.1.1/LICENSE
--rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.1.1/Makefile
--rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.1.1/README.md
--rw-r--r--   0        0        0        6 2024-05-21 05:24:31.576371 rstms_cloudflare-1.1.1/VERSION
--rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.1/docs/Makefile
--rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.1/docs/cli.rst
--rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.1/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.1/docs/contributing.rst
--rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.1/docs/index.rst
--rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.1/docs/installation.rst
--rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.1/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.1.1/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.1/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.1.1/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-1.1.1/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.1/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.1/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.1/make/docs.mk
--rw-r--r--   0        0        0      668 2024-05-20 19:47:31.723566 rstms_cloudflare-1.1.1/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.1/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.1/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.1/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.1.1/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.1/make/version.mk
--rw-r--r--   0        0        0     1159 2024-05-21 05:24:31.576371 rstms_cloudflare-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.1/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-21 05:24:31.428372 rstms_cloudflare-1.1.1/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-21 05:24:31.480372 rstms_cloudflare-1.1.1/requirements-docs.txt
--rw-r--r--   0        0        0       19 2024-05-21 05:24:31.372373 rstms_cloudflare-1.1.1/requirements.txt
--rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.1.1/rstms_cloudflare/__init__.py
--rw-r--r--   0        0        0     6466 2024-05-21 05:23:31.861012 rstms_cloudflare-1.1.1/rstms_cloudflare/cli.py
--rw-r--r--   0        0        0     6182 2024-05-21 01:42:56.024690 rstms_cloudflare-1.1.1/rstms_cloudflare/cloudflare.py
--rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.1.1/rstms_cloudflare/exception_handler.py
--rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.1.1/rstms_cloudflare/shell.py
--rw-r--r--   0        0        0      127 2024-05-21 05:24:31.576371 rstms_cloudflare-1.1.1/rstms_cloudflare/version.py
--rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.1.1/tests/test_cli.py
--rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.1/tox.ini
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rstms_cloudflare-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      383 2024-05-29 03:53:20.104606 rstms_cloudflare-1.1.2/.bumpversion.cfg
+-rw-r--r--   0        0        0     1344 2024-05-21 01:52:37.934629 rstms_cloudflare-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.1.2/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.1.2/Makefile
+-rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.1.2/README.md
+-rw-r--r--   0        0        0        6 2024-05-29 03:53:20.104606 rstms_cloudflare-1.1.2/VERSION
+-rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.2/docs/Makefile
+-rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.2/docs/cli.rst
+-rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.2/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.2/docs/contributing.rst
+-rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.2/docs/index.rst
+-rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.2/docs/installation.rst
+-rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.2/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.1.2/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.2/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.1.2/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-1.1.2/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.2/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.2/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.2/make/docs.mk
+-rw-r--r--   0        0        0      668 2024-05-20 19:47:31.723566 rstms_cloudflare-1.1.2/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.2/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.2/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.2/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.1.2/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.2/make/version.mk
+-rw-r--r--   0        0        0     1159 2024-05-29 03:53:20.104606 rstms_cloudflare-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.2/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-29 03:53:19.956607 rstms_cloudflare-1.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-29 03:53:20.012607 rstms_cloudflare-1.1.2/requirements-docs.txt
+-rw-r--r--   0        0        0       19 2024-05-29 03:53:19.900608 rstms_cloudflare-1.1.2/requirements.txt
+-rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.1.2/rstms_cloudflare/__init__.py
+-rw-r--r--   0        0        0     6474 2024-05-29 03:01:48.275249 rstms_cloudflare-1.1.2/rstms_cloudflare/cli.py
+-rw-r--r--   0        0        0     6182 2024-05-21 01:42:56.024690 rstms_cloudflare-1.1.2/rstms_cloudflare/cloudflare.py
+-rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.1.2/rstms_cloudflare/exception_handler.py
+-rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.1.2/rstms_cloudflare/shell.py
+-rw-r--r--   0        0        0      127 2024-05-29 03:53:20.104606 rstms_cloudflare-1.1.2/rstms_cloudflare/version.py
+-rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.1.2/tests/test_cli.py
+-rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.2/tox.ini
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rstms_cloudflare-1.1.2/PKG-INFO
```

### Comparing `rstms_cloudflare-1.1.1/.gitignore` & `rstms_cloudflare-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/LICENSE` & `rstms_cloudflare-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/Makefile` & `rstms_cloudflare-1.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/README.md` & `rstms_cloudflare-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/docs/Makefile` & `rstms_cloudflare-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/docs/conf.py` & `rstms_cloudflare-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/docs/installation.rst` & `rstms_cloudflare-1.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/docs/make.bat` & `rstms_cloudflare-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/make/clean.mk` & `rstms_cloudflare-1.1.2/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/make/common.mk` & `rstms_cloudflare-1.1.2/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/make/docs.mk` & `rstms_cloudflare-1.1.2/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/make/lint.mk` & `rstms_cloudflare-1.1.2/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/make/publish.mk` & `rstms_cloudflare-1.1.2/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/make/release.mk` & `rstms_cloudflare-1.1.2/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/make/test.mk` & `rstms_cloudflare-1.1.2/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/make/version.mk` & `rstms_cloudflare-1.1.2/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/pyproject.toml` & `rstms_cloudflare-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-cloudflare"
-version = "1.1.1"
+version = "1.1.2"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_cloudflare"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_cloudflare-1.1.1/rstms_cloudflare/cli.py` & `rstms_cloudflare-1.1.2/rstms_cloudflare/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 @click.argument("content")
 @click.option("-t", "--ttl", default=60)
 @click.option("-p", "--priority", default=10)
 @click.pass_obj
 def add(api, domain, type, host, content, ttl, priority):
     """add a new record"""
 
-    if type in ["A", "CNAME", "TXT"]:
+    if type in ["A", "CNAME", "TXT", 'AAAA']:
         priority = None
     elif type == "MX":
         priority = priority or 0
     else:
         raise ValueError(f"Unsupported record type '{type}'")
 
     added = api.add_record(domain, type, host, content, ttl, priority)
```

### Comparing `rstms_cloudflare-1.1.1/rstms_cloudflare/cloudflare.py` & `rstms_cloudflare-1.1.2/rstms_cloudflare/cloudflare.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/rstms_cloudflare/exception_handler.py` & `rstms_cloudflare-1.1.2/rstms_cloudflare/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/rstms_cloudflare/shell.py` & `rstms_cloudflare-1.1.2/rstms_cloudflare/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/tests/test_cli.py` & `rstms_cloudflare-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.1/PKG-INFO` & `rstms_cloudflare-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-cloudflare
-Version: 1.1.1
+Version: 1.1.2
 Summary: Top-level package for rstms-cloudflare.
 Keywords: rstms_cloudflare
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

