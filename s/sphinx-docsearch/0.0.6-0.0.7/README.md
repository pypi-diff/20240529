# Comparing `tmp/sphinx_docsearch-0.0.6.tar.gz` & `tmp/sphinx_docsearch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_docsearch-0.0.6.tar", max compression
+gzip compressed data, was "sphinx_docsearch-0.0.7.tar", max compression
```

## Comparing `sphinx_docsearch-0.0.6.tar` & `sphinx_docsearch-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1064 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/LICENSE
--rw-r--r--   0        0        0     1621 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/README.md
--rw-r--r--   0        0        0     1928 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4819 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/py.typed
--rw-r--r--   0        0        0      130 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/alabaster-docsearch-custom.css
--rw-r--r--   0        0        0    13762 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/docsearch.css
--rw-r--r--   0        0        0   127820 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/docsearch.js
--rw-r--r--   0        0        0      648 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/docsearch_config.js_t
--rw-r--r--   0        0        0     1782 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/furo-docsearch-custom.css
--rw-r--r--   0        0        0      220 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/pydata-docsearch-custom.css
--rw-r--r--   0        0        0      167 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/rtd-docsearch-custom.css
--rw-r--r--   0        0        0      117 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/templates/searchbox.html
--rw-r--r--   0        0        0      117 2024-05-28 06:48:06.050317 sphinx_docsearch-0.0.6/src/sphinx_docsearch/templates/sidebar/search.html
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 sphinx_docsearch-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-29 07:31:28.957350 sphinx_docsearch-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1621 2024-05-29 07:31:28.957350 sphinx_docsearch-0.0.7/README.md
+-rw-r--r--   0        0        0     1928 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4819 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/py.typed
+-rw-r--r--   0        0        0      130 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/alabaster-docsearch-custom.css
+-rw-r--r--   0        0        0    13762 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/docsearch.css
+-rw-r--r--   0        0        0   127820 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/docsearch.js
+-rw-r--r--   0        0        0      648 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/docsearch_config.js_t
+-rw-r--r--   0        0        0     1782 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/furo-docsearch-custom.css
+-rw-r--r--   0        0        0      401 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/pydata-docsearch-custom.css
+-rw-r--r--   0        0        0      167 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/rtd-docsearch-custom.css
+-rw-r--r--   0        0        0      117 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/templates/searchbox.html
+-rw-r--r--   0        0        0      117 2024-05-29 07:31:28.961350 sphinx_docsearch-0.0.7/src/sphinx_docsearch/templates/sidebar/search.html
+-rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 sphinx_docsearch-0.0.7/PKG-INFO
```

### Comparing `sphinx_docsearch-0.0.6/LICENSE` & `sphinx_docsearch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.6/README.md` & `sphinx_docsearch-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.6/pyproject.toml` & `sphinx_docsearch-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-docsearch"
-version = "0.0.6"
+version = "0.0.7"
 description = "A Sphinx extension for replacing the built-in search with Algolia DocSearch"
 authors = ["Algolia <support@algolia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "sphinx_docsearch", from = "src"}
 ]
```

### Comparing `sphinx_docsearch-0.0.6/src/sphinx_docsearch/__init__.py` & `sphinx_docsearch-0.0.7/src/sphinx_docsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/docsearch.css` & `sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/docsearch.css`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/docsearch.js` & `sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/docsearch.js`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/docsearch_config.js_t` & `sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/docsearch_config.js_t`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.6/src/sphinx_docsearch/static/furo-docsearch-custom.css` & `sphinx_docsearch-0.0.7/src/sphinx_docsearch/static/furo-docsearch-custom.css`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.6/PKG-INFO` & `sphinx_docsearch-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-docsearch
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Sphinx extension for replacing the built-in search with Algolia DocSearch
 License: MIT
 Author: Algolia
 Author-email: support@algolia.com
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
```

