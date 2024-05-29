# Comparing `tmp/metrit-0.0.4.tar.gz` & `tmp/metrit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrit-0.0.4.tar", last modified: Wed May 29 09:56:11 2024, max compression
+gzip compressed data, was "metrit-0.0.8.tar", last modified: Wed May 29 15:05:55 2024, max compression
```

## Comparing `metrit-0.0.4.tar` & `metrit-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:56:11.479851 metrit-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 09:56:06.000000 metrit-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 09:56:11.479851 metrit-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-29 09:56:06.000000 metrit-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:56:11.479851 metrit-0.0.4/metrit/
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/Monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/StatCollector.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/Stats.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:56:11.479851 metrit-0.0.4/metrit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:56:11.479851 metrit-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 09:56:08.000000 metrit-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:56:11.479851 metrit-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_StatsCollector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_metrit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_metrit_deactivated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_metrit_with_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.336684 metrit-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.332684 metrit-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.332684 metrit-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-29 15:05:49.000000 metrit-0.0.8/.github/workflows/push_to_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-29 15:05:49.000000 metrit-0.0.8/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-29 15:05:49.000000 metrit-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 15:05:49.000000 metrit-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-29 15:05:49.000000 metrit-0.0.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-05-29 15:05:55.336684 metrit-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 15:05:49.000000 metrit-0.0.8/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    26374 2024-05-29 15:05:49.000000 metrit-0.0.8/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-29 15:05:49.000000 metrit-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.332684 metrit-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-29 15:05:49.000000 metrit-0.0.8/examples/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.336684 metrit-0.0.8/metrit/
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/Monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/StatCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/Stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 15:05:49.000000 metrit-0.0.8/metrit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.336684 metrit-0.0.8/metrit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 15:05:55.000000 metrit-0.0.8/metrit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-29 15:05:49.000000 metrit-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:05:55.336684 metrit-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:55.336684 metrit-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_StatsCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_metrit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_metrit_deactivated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_metrit_with_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 15:05:49.000000 metrit-0.0.8/tests/test_utils.py
```

### Comparing `metrit-0.0.4/LICENSE` & `metrit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/PKG-INFO` & `metrit-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,35 @@
 Metadata-Version: 2.1
 Name: metrit
-Version: 0.0.4
+Version: 0.0.8
 Summary: A dead simple resources monitoring decorator
-Home-page: https://github.com/mcrespoae/metrit
-Author: mcrespoae
-Author-email: info@mariocrespo.es
-Keywords: metrit
+Author-email: Mario Crespo <info@mariocrespo.es>
+License: MIT License
+        
+        Copyright (c) 2024 Mario Crespo
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Repository, https://github.com/mcrespoae/metrit
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `metrit-0.0.4/README.md` & `metrit-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/metrit/Monitoring.py` & `metrit-0.0.8/metrit/Monitoring.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/metrit/StatCollector.py` & `metrit-0.0.8/metrit/StatCollector.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/metrit/Stats.py` & `metrit-0.0.8/metrit/Stats.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/metrit/core.py` & `metrit-0.0.8/metrit/core.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/metrit/utils.py` & `metrit-0.0.8/metrit/utils.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/metrit.egg-info/PKG-INFO` & `metrit-0.0.8/metrit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,35 @@
 Metadata-Version: 2.1
 Name: metrit
-Version: 0.0.4
+Version: 0.0.8
 Summary: A dead simple resources monitoring decorator
-Home-page: https://github.com/mcrespoae/metrit
-Author: mcrespoae
-Author-email: info@mariocrespo.es
-Keywords: metrit
+Author-email: Mario Crespo <info@mariocrespo.es>
+License: MIT License
+        
+        Copyright (c) 2024 Mario Crespo
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Repository, https://github.com/mcrespoae/metrit
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `metrit-0.0.4/tests/test_StatsCollector.py` & `metrit-0.0.8/tests/test_StatsCollector.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/tests/test_metrit.py` & `metrit-0.0.8/tests/test_metrit.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/tests/test_metrit_deactivated.py` & `metrit-0.0.8/tests/test_metrit_deactivated.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/tests/test_metrit_with_args.py` & `metrit-0.0.8/tests/test_metrit_with_args.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.4/tests/test_utils.py` & `metrit-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

