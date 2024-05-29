# Comparing `tmp/rshf-0.0.4.tar.gz` & `tmp/rshf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rshf-0.0.4.tar", last modified: Sun May 26 18:28:04 2024, max compression
+gzip compressed data, was "rshf-0.0.5.tar", last modified: Wed May 29 16:51:28 2024, max compression
```

## Comparing `rshf-0.0.4.tar` & `rshf-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.351825 rshf-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 18:28:00.000000 rshf-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-26 18:28:04.351825 rshf-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-26 18:28:00.000000 rshf-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-26 18:28:00.000000 rshf-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-26 18:28:00.000000 rshf-0.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.335825 rshf-0.0.4/rshf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.339825 rshf-0.0.4/rshf/croma/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/croma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/croma/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.339825 rshf-0.0.4/rshf/geoclap/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/geoclap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.339825 rshf-0.0.4/rshf/geoclip/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/geoclip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/geoclip/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.339825 rshf-0.0.4/rshf/prithvi/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/prithvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13682 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/prithvi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.339825 rshf-0.0.4/rshf/rvsa/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/rvsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15196 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/rvsa/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.339825 rshf-0.0.4/rshf/satclip/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satclip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satclip/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satclip/spherical_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satclip/spherical_harmonics_closed_form.py
--rw-r--r--   0 runner    (1001) docker     (127)  7765721 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satclip/spherical_harmonics_ylm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.347825 rshf-0.0.4/rshf/satmae/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satmae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satmae/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.351825 rshf-0.0.4/rshf/satmaepp/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satmaepp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/satmaepp/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.351825 rshf-0.0.4/rshf/scalemae/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/scalemae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-26 18:28:00.000000 rshf-0.0.4/rshf/scalemae/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:28:04.351825 rshf-0.0.4/rshf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-26 18:28:04.000000 rshf-0.0.4/rshf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-26 18:28:04.000000 rshf-0.0.4/rshf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:28:04.000000 rshf-0.0.4/rshf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:28:04.000000 rshf-0.0.4/rshf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-26 18:28:04.000000 rshf-0.0.4/rshf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 18:28:04.000000 rshf-0.0.4/rshf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-26 18:28:04.351825 rshf-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.136285 rshf-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 16:51:23.000000 rshf-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 16:51:28.136285 rshf-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 16:51:23.000000 rshf-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 16:51:23.000000 rshf-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-29 16:51:23.000000 rshf-0.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/bioclip/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/bioclip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/bioclip/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/clip/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/clip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/croma/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/croma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/croma/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/geoclap/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/geoclap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/geoclip/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/geoclip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/geoclip/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/presto/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/presto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24910 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/presto/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/prithvi/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/prithvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13682 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/prithvi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.120285 rshf-0.0.5/rshf/remoteclip/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/remoteclip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/remoteclip/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.124285 rshf-0.0.5/rshf/rvsa/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/rvsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15196 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/rvsa/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.124285 rshf-0.0.5/rshf/satclip/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satclip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satclip/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satclip/spherical_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satclip/spherical_harmonics_closed_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)  7765721 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satclip/spherical_harmonics_ylm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.132285 rshf-0.0.5/rshf/satmae/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satmae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28993 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satmae/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.132285 rshf-0.0.5/rshf/satmaepp/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satmaepp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/satmaepp/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.132285 rshf-0.0.5/rshf/scalemae/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/scalemae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/scalemae/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.132285 rshf-0.0.5/rshf/sinr/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/sinr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-29 16:51:23.000000 rshf-0.0.5/rshf/sinr/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:51:28.136285 rshf-0.0.5/rshf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 16:51:28.000000 rshf-0.0.5/rshf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-29 16:51:28.000000 rshf-0.0.5/rshf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:51:28.000000 rshf-0.0.5/rshf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:51:27.000000 rshf-0.0.5/rshf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-29 16:51:28.000000 rshf-0.0.5/rshf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 16:51:28.000000 rshf-0.0.5/rshf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-29 16:51:28.136285 rshf-0.0.5/setup.cfg
```

### Comparing `rshf-0.0.4/LICENSE` & `rshf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/PKG-INFO` & `rshf-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rshf
-Version: 0.0.4
+Version: 0.0.5
 Summary: RS pretrained models in huggingface style
 Home-page: https://github.com/mvrl/rshf
 Author: Srikumar Sastry
 Author-email: s.sastry@wustl.edu
 Keywords: Remote Sensing,Huggingface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,14 +14,15 @@
 License-File: LICENSE
 Requires-Dist: torch==2.3.0
 Requires-Dist: timm==1.0.3
 Requires-Dist: numpy==1.26.4
 Requires-Dist: huggingface_hub==0.23.1
 Requires-Dist: einops==0.8.0
 Requires-Dist: transformers==4.41.1
+Requires-Dist: open_clip_torch==2.24.0
 
 # rshf
 ### Remote sensing pretrained models easy loading using huggingface -- PyTorch (for fast benchmarking)
 
 ### Installation:
 ```bash
 pip install rshf
```

### Comparing `rshf-0.0.4/README.md` & `rshf-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/croma/model.py` & `rshf-0.0.5/rshf/croma/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/geoclip/model.py` & `rshf-0.0.5/rshf/geoclip/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/prithvi/model.py` & `rshf-0.0.5/rshf/prithvi/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/rvsa/model.py` & `rshf-0.0.5/rshf/rvsa/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/satclip/model.py` & `rshf-0.0.5/rshf/satclip/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/satclip/spherical_harmonics.py` & `rshf-0.0.5/rshf/satclip/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/satclip/spherical_harmonics_closed_form.py` & `rshf-0.0.5/rshf/satclip/spherical_harmonics_closed_form.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/satclip/spherical_harmonics_ylm.py` & `rshf-0.0.5/rshf/satclip/spherical_harmonics_ylm.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/satmaepp/model.py` & `rshf-0.0.5/rshf/satmaepp/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf/scalemae/model.py` & `rshf-0.0.5/rshf/scalemae/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.4/rshf.egg-info/PKG-INFO` & `rshf-0.0.5/rshf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rshf
-Version: 0.0.4
+Version: 0.0.5
 Summary: RS pretrained models in huggingface style
 Home-page: https://github.com/mvrl/rshf
 Author: Srikumar Sastry
 Author-email: s.sastry@wustl.edu
 Keywords: Remote Sensing,Huggingface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,14 +14,15 @@
 License-File: LICENSE
 Requires-Dist: torch==2.3.0
 Requires-Dist: timm==1.0.3
 Requires-Dist: numpy==1.26.4
 Requires-Dist: huggingface_hub==0.23.1
 Requires-Dist: einops==0.8.0
 Requires-Dist: transformers==4.41.1
+Requires-Dist: open_clip_torch==2.24.0
 
 # rshf
 ### Remote sensing pretrained models easy loading using huggingface -- PyTorch (for fast benchmarking)
 
 ### Installation:
 ```bash
 pip install rshf
```

### Comparing `rshf-0.0.4/rshf.egg-info/SOURCES.txt` & `rshf-0.0.5/rshf.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -6,27 +6,36 @@
 rshf/__init__.py
 rshf.egg-info/PKG-INFO
 rshf.egg-info/SOURCES.txt
 rshf.egg-info/dependency_links.txt
 rshf.egg-info/not-zip-safe
 rshf.egg-info/requires.txt
 rshf.egg-info/top_level.txt
+rshf/bioclip/__init__.py
+rshf/bioclip/model.py
+rshf/clip/__init__.py
 rshf/croma/__init__.py
 rshf/croma/model.py
 rshf/geoclap/__init__.py
 rshf/geoclip/__init__.py
 rshf/geoclip/model.py
+rshf/presto/__init__.py
+rshf/presto/model.py
 rshf/prithvi/__init__.py
 rshf/prithvi/model.py
+rshf/remoteclip/__init__.py
+rshf/remoteclip/model.py
 rshf/rvsa/__init__.py
 rshf/rvsa/model.py
 rshf/satclip/__init__.py
 rshf/satclip/model.py
 rshf/satclip/spherical_harmonics.py
 rshf/satclip/spherical_harmonics_closed_form.py
 rshf/satclip/spherical_harmonics_ylm.py
 rshf/satmae/__init__.py
 rshf/satmae/model.py
 rshf/satmaepp/__init__.py
 rshf/satmaepp/model.py
 rshf/scalemae/__init__.py
-rshf/scalemae/model.py
+rshf/scalemae/model.py
+rshf/sinr/__init__.py
+rshf/sinr/model.py
```

### Comparing `rshf-0.0.4/setup.cfg` & `rshf-0.0.5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rshf
-version = 0.0.4
+version = 0.0.5
 author = Srikumar Sastry
 author_email = s.sastry@wustl.edu
 description = RS pretrained models in huggingface style
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mvrl/rshf
 keywords = Remote Sensing, Huggingface
```

