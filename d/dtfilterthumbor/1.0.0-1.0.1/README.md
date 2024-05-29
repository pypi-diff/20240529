# Comparing `tmp/dtfilterthumbor-1.0.0.tar.gz` & `tmp/dtfilterthumbor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfilterthumbor-1.0.0.tar", last modified: Wed May 29 04:26:05 2024, max compression
+gzip compressed data, was "dtfilterthumbor-1.0.1.tar", last modified: Wed May 29 07:41:35 2024, max compression
```

## Comparing `dtfilterthumbor-1.0.0.tar` & `dtfilterthumbor-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 04:26:05.810181 dtfilterthumbor-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-29 04:26:05.810181 dtfilterthumbor-1.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      333 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 04:26:05.809181 dtfilterthumbor-1.0.0/dtfilterthumbor/
--rw-rw-r--   0 root         (0) root         (0)      322 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/dtfilterthumbor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7395 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/dtfilterthumbor/dtwatermark.py
--rw-rw-r--   0 root         (0) root         (0)     7416 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/dtfilterthumbor/dtwatermark2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 04:26:05.810181 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-29 04:26:05.000000 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      265 2024-05-29 04:26:05.000000 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 04:26:05.000000 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-29 04:26:05.000000 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 04:26:05.810181 dtfilterthumbor-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:41:35.771608 dtfilterthumbor-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-29 07:41:35.770608 dtfilterthumbor-1.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      333 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:41:35.768608 dtfilterthumbor-1.0.1/dtfilterthumbor/
+-rw-rw-r--   0 root         (0) root         (0)      322 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.1/dtfilterthumbor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7395 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.1/dtfilterthumbor/dtwatermark.py
+-rw-rw-r--   0 root         (0) root         (0)     7429 2024-05-29 07:40:38.000000 dtfilterthumbor-1.0.1/dtfilterthumbor/dtwatermark2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:41:35.770608 dtfilterthumbor-1.0.1/dtfilterthumbor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-29 07:41:35.000000 dtfilterthumbor-1.0.1/dtfilterthumbor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      265 2024-05-29 07:41:35.000000 dtfilterthumbor-1.0.1/dtfilterthumbor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 07:41:35.000000 dtfilterthumbor-1.0.1/dtfilterthumbor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-29 07:41:35.000000 dtfilterthumbor-1.0.1/dtfilterthumbor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 07:41:35.771608 dtfilterthumbor-1.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-29 07:40:38.000000 dtfilterthumbor-1.0.1/setup.py
```

### Comparing `dtfilterthumbor-1.0.0/PKG-INFO` & `dtfilterthumbor-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfilterthumbor
-Version: 1.0.0
+Version: 1.0.1
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `dtfilterthumbor-1.0.0/dtfilterthumbor/dtwatermark.py` & `dtfilterthumbor-1.0.1/dtfilterthumbor/dtwatermark.py`

 * *Files identical despite different names*

### Comparing `dtfilterthumbor-1.0.0/dtfilterthumbor/dtwatermark2.py` & `dtfilterthumbor-1.0.1/dtfilterthumbor/dtwatermark2.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             if image_size[1] * 1.0 / watermark_sz[1] < 2:
                 repeat_y = (
                     math.ceil(image_size[1] * 1.0 / watermark_sz[1]),
                     10,
                 )
                 space_y = 10
 
-        mos_y = 0;
+        print ("change mose y")
         if not mos_x and not mos_y:
             self.engine.paste(self.watermark_engine, (x, y), merge=True)
         elif mos_x and mos_y:
             if (repeat_x[0] * repeat_y[0]) > 100:
                 tmpRepeatX = min(6, repeat_x[0])
                 tmpRepeatY = min(6, repeat_y[0])
                 repeat_x = (
```

### Comparing `dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/PKG-INFO` & `dtfilterthumbor-1.0.1/dtfilterthumbor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfilterthumbor
-Version: 1.0.0
+Version: 1.0.1
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `dtfilterthumbor-1.0.0/setup.py` & `dtfilterthumbor-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="dtfilterthumbor",
-    version="1.0.0",
+    version="1.0.1",
     description="dan tri filter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="xuantrangk54",
     author_email="xuantrangk54@gmail.com",
     license="MIT",
```

