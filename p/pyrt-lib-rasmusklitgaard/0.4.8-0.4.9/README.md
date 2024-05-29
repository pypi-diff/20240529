# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.4.8.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.8.tar", last modified: Fri May 17 11:34:12 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.9.tar", last modified: Fri May 17 11:52:02 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.4.8.tar` & `pyrt_lib_rasmusklitgaard-0.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:34:12.114088 pyrt_lib_rasmusklitgaard-0.4.8/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.8/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 11:34:12.114088 pyrt_lib_rasmusklitgaard-0.4.8/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.8/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-17 11:34:04.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:34:12.110088 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11650 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/parameter_parser.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    33769 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/pyrt_database.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/resample.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:34:12.114088 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-17 11:34:12.114088 pyrt_lib_rasmusklitgaard-0.4.8/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:52:02.171676 pyrt_lib_rasmusklitgaard-0.4.9/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.9/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 11:52:02.171676 pyrt_lib_rasmusklitgaard-0.4.9/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.9/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-17 11:51:55.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:52:02.167676 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-17 11:51:59.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11650 2024-05-17 11:51:59.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-17 11:51:59.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-17 11:51:59.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/parameter_parser.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    33855 2024-05-17 11:51:59.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-17 11:51:59.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/pyrt_database.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-17 11:51:59.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/resample.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-17 11:51:59.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:52:02.171676 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 11:52:02.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-17 11:52:02.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-17 11:52:02.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-17 11:52:02.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-17 11:52:02.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-17 11:52:02.000000 pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-17 11:52:02.171676 pyrt_lib_rasmusklitgaard-0.4.9/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/LICENSE` & `pyrt_lib_rasmusklitgaard-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.8
+Version: 0.4.9
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/README.md` & `pyrt_lib_rasmusklitgaard-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.4.8"
+version = "0.4.9"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/parameter_parser.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 				self.wanted_structures = ["ctv", "bladder", "bladder wall", "rectum", "rectal wall", "Bladder Wall", "Rectal Wall", "Rectum", "Bladder", "CTV", "Rectal_Wall", "Bladder_Wall"]
 			self.actual_structure_names = self.get_actual_structure_names(self.wanted_structures , *args, **kwargs)
 			if self.actual_structure_names == None:
 				raise ValueError("No structures names set for patient {}".format(self.patient_id))
 		except AttributeError as e:
 			print("Attribute error for patient when setting structures: {}".format(self.patient_id))
 			print(str(e))
+			raise ValueError("No structures names set for patient {}".format(self.patient_id))
 		t7=time.time()
 
 		self.set_structure_indices()
 		t8=time.time()
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/pyrt_database.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/pyrt_database.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/resample.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/resample.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.8
+Version: 0.4.9
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.4.9/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

