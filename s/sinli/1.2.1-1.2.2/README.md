# Comparing `tmp/sinli-1.2.1.tar.gz` & `tmp/sinli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinli-1.2.1.tar", last modified: Sun May  5 14:14:53 2024, max compression
+gzip compressed data, was "sinli-1.2.2.tar", last modified: Wed May 29 17:13:14 2024, max compression
```

## Comparing `sinli-1.2.1.tar` & `sinli-1.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    34449 2024-05-05 14:14:42.000000 sinli-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    46338 2024-05-05 14:14:53.726207 sinli-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6041 2024-05-05 14:14:42.000000 sinli-1.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-05 14:14:42.000000 sinli-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 14:14:53.726207 sinli-1.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.722207 sinli-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.722207 sinli-1.2.1/src/sinli/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/common/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5851 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/common/encoded_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/devolu/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/devolu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2390 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/devolu/v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/envio/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/envio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/envio/v8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/factul/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/factul/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/factul/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/libros/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/libros/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/libros/v8.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/libros/v9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/mensaj/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/mensaj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/mensaj/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/pedido/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/pedido/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/pedido/v7.py
--rw-rw-rw-   0 root         (0) root         (0)     5490 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/document.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/line.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/subject.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46338 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-05 14:14:42.000000 sinli-1.2.1/tests/test_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.247000 sinli-1.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34449 2024-05-29 17:07:11.000000 sinli-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    46338 2024-05-29 17:13:14.247000 sinli-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6041 2024-05-29 17:07:11.000000 sinli-1.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-29 17:13:03.000000 sinli-1.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 17:13:14.247000 sinli-1.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.239000 sinli-1.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/common/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/common/encoded_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/doctype/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/doctype/devolu/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/devolu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2390 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/devolu/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/doctype/envio/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/envio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/envio/v8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/doctype/factul/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/factul/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/factul/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/doctype/libros/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/libros/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/libros/v8.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/libros/v9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/doctype/mensaj/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/mensaj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/mensaj/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/src/sinli/doctype/pedido/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/pedido/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/doctype/pedido/v7.py
+-rw-rw-rw-   0 root         (0) root         (0)     5490 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     8087 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/line.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-29 17:07:11.000000 sinli-1.2.2/src/sinli/subject.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.247000 sinli-1.2.2/src/sinli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46338 2024-05-29 17:13:14.000000 sinli-1.2.2/src/sinli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2024-05-29 17:13:14.000000 sinli-1.2.2/src/sinli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 17:13:14.000000 sinli-1.2.2/src/sinli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-29 17:13:14.000000 sinli-1.2.2/src/sinli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-29 17:13:14.000000 sinli-1.2.2/src/sinli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:13:14.243000 sinli-1.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-29 17:07:11.000000 sinli-1.2.2/tests/test_document.py
```

### Comparing `sinli-1.2.1/LICENSE` & `sinli-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/PKG-INFO` & `sinli-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.2.1
+Version: 1.2.2
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sinli-1.2.1/README.md` & `sinli-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/pyproject.toml` & `sinli-1.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sinli"
-version = "1.2.1"
+version = "1.2.2"
 dependencies = [
     "typing-extensions==4.3.0",
     "pycountry==22.3.5"
 ]
 authors = [
     {name = "Devcontrol", email = "devcontrol@zici.fr"},
 ]
```

### Comparing `sinli-1.2.1/src/sinli/common/encoded_values.py` & `sinli-1.2.2/src/sinli/common/encoded_values.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/doctype/__init__.py` & `sinli-1.2.2/src/sinli/doctype/__init__.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/doctype/devolu/v2.py` & `sinli-1.2.2/src/sinli/doctype/devolu/v2.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/doctype/envio/v8.py` & `sinli-1.2.2/src/sinli/doctype/envio/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/doctype/factul/v1.py` & `sinli-1.2.2/src/sinli/doctype/factul/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/doctype/libros/v8.py` & `sinli-1.2.2/src/sinli/doctype/libros/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/doctype/libros/v9.py` & `sinli-1.2.2/src/sinli/doctype/libros/v9.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/doctype/mensaj/v1.py` & `sinli-1.2.2/src/sinli/doctype/mensaj/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/doctype/pedido/v7.py` & `sinli-1.2.2/src/sinli/doctype/pedido/v7.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/document.py` & `sinli-1.2.2/src/sinli/document.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli/line.py` & `sinli-1.2.2/src/sinli/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             return value.alpha_2
         elif type(value) == cls.lang_class:
             return value.alpha_3
         elif type(value) == cls.currency_class:
             if vlen == 3:  return value.alpha_3
             #elif vlen == 1: return value # TODO understand P and E values
         elif isinstance(ftype, EncodedField):
-            if value == None:
+            if value == None or value == "":
                 return " "
             return value[0]
         else: # string, integer
             return str(value)
 
     @classmethod
     def pretify(cls, k, v) -> str:
```

### Comparing `sinli-1.2.1/src/sinli/subject.py` & `sinli-1.2.2/src/sinli/subject.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.1/src/sinli.egg-info/PKG-INFO` & `sinli-1.2.2/src/sinli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.2.1
+Version: 1.2.2
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sinli-1.2.1/src/sinli.egg-info/SOURCES.txt` & `sinli-1.2.2/src/sinli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

