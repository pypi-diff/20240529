# Comparing `tmp/astro_test_package-0.0.1.tar.gz` & `tmp/astro_test_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_test_package-0.0.1.tar", last modified: Wed May 29 12:17:01 2024, max compression
+gzip compressed data, was "astro_test_package-0.0.2.tar", last modified: Wed May 29 12:49:30 2024, max compression
```

## Comparing `astro_test_package-0.0.1.tar` & `astro_test_package-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:17:01.957193 astro_test_package-0.0.1/
--rw-rw-rw-   0        0        0     1078 2024-05-29 12:12:46.000000 astro_test_package-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1791 2024-05-29 12:17:01.954722 astro_test_package-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1304 2024-05-22 10:42:42.000000 astro_test_package-0.0.1/README.md
--rw-rw-rw-   0        0        0      429 2024-05-29 11:58:14.000000 astro_test_package-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 12:17:01.957690 astro_test_package-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 12:17:01.876315 astro_test_package-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 12:17:01.916927 astro_test_package-0.0.1/src/astro_test_package/
--rw-rw-rw-   0        0        0       47 2024-05-08 12:55:37.000000 astro_test_package-0.0.1/src/astro_test_package/__init__.py
--rw-rw-rw-   0        0        0      123 2024-05-08 12:36:52.000000 astro_test_package-0.0.1/src/astro_test_package/astro_analyzer.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:17:01.952772 astro_test_package-0.0.1/src/astro_test_package.egg-info/
--rw-rw-rw-   0        0        0     1791 2024-05-29 12:17:01.000000 astro_test_package-0.0.1/src/astro_test_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-29 12:17:01.000000 astro_test_package-0.0.1/src/astro_test_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:17:01.000000 astro_test_package-0.0.1/src/astro_test_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-29 12:17:01.000000 astro_test_package-0.0.1/src/astro_test_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 12:49:30.453425 astro_test_package-0.0.2/
+-rw-rw-rw-   0        0        0     1078 2024-05-29 12:12:46.000000 astro_test_package-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1823 2024-05-29 12:49:30.453425 astro_test_package-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1304 2024-05-22 10:42:42.000000 astro_test_package-0.0.2/README.md
+-rw-rw-rw-   0        0        0      476 2024-05-29 12:48:58.000000 astro_test_package-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:49:30.455096 astro_test_package-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 12:49:30.410445 astro_test_package-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 12:49:30.417691 astro_test_package-0.0.2/src/astro_test_package/
+-rw-rw-rw-   0        0        0       47 2024-05-08 12:55:37.000000 astro_test_package-0.0.2/src/astro_test_package/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-05-08 12:36:52.000000 astro_test_package-0.0.2/src/astro_test_package/astro_analyzer.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:49:30.448373 astro_test_package-0.0.2/src/astro_test_package.egg-info/
+-rw-rw-rw-   0        0        0     1823 2024-05-29 12:49:30.000000 astro_test_package-0.0.2/src/astro_test_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-29 12:49:30.000000 astro_test_package-0.0.2/src/astro_test_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:49:30.000000 astro_test_package-0.0.2/src/astro_test_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-29 12:49:30.000000 astro_test_package-0.0.2/src/astro_test_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-29 12:49:30.000000 astro_test_package-0.0.2/src/astro_test_package.egg-info/top_level.txt
```

### Comparing `astro_test_package-0.0.1/LICENSE` & `astro_test_package-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_test_package-0.0.1/PKG-INFO` & `astro_test_package-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: astro_test_package
-Version: 0.0.1
+Version: 0.0.2
 Summary: Astro test package
 Author-email: Mikhail Krivonosov <mike_live@mail.ru>
 Project-URL: Homepage, https://github.com/mike-live/astro-test-package
 Project-URL: Issues, https://github.com/mike-live/astro-test-package/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: opencv-python>4
 
 ### Astro test package
 
 ### Markdown
 .md : m = mark, d = down
 
 Rendering of markdown file `Shift-Ctrl-V`
```

### Comparing `astro_test_package-0.0.1/README.md` & `astro_test_package-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `astro_test_package-0.0.1/src/astro_test_package.egg-info/PKG-INFO` & `astro_test_package-0.0.2/src/astro_test_package.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: astro_test_package
-Version: 0.0.1
+Version: 0.0.2
 Summary: Astro test package
 Author-email: Mikhail Krivonosov <mike_live@mail.ru>
 Project-URL: Homepage, https://github.com/mike-live/astro-test-package
 Project-URL: Issues, https://github.com/mike-live/astro-test-package/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: opencv-python>4
 
 ### Astro test package
 
 ### Markdown
 .md : m = mark, d = down
 
 Rendering of markdown file `Shift-Ctrl-V`
```

