# Comparing `tmp/torch_model_manager-1.0.1.dev2.tar.gz` & `tmp/torch_model_manager-1.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-1.0.1.dev2.tar", last modified: Wed May 29 09:37:50 2024, max compression
+gzip compressed data, was "torch_model_manager-1.0.1.dev3.tar", last modified: Wed May 29 09:40:58 2024, max compression
```

## Comparing `torch_model_manager-1.0.1.dev2.tar` & `torch_model_manager-1.0.1.dev3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:37:50.534091 torch_model_manager-1.0.1.dev2/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-29 09:37:50.534091 torch_model_manager-1.0.1.dev2/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev2/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-29 09:37:50.534091 torch_model_manager-1.0.1.dev2/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2243 2024-05-29 09:37:48.000000 torch_model_manager-1.0.1.dev2/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:37:50.530091 torch_model_manager-1.0.1.dev2/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:37:50.530091 torch_model_manager-1.0.1.dev2/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev2/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:37:50.530091 torch_model_manager-1.0.1.dev2/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev2/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev2/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:37:50.530091 torch_model_manager-1.0.1.dev2/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-1.0.1.dev2/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-1.0.1.dev2/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1707 2024-05-29 09:37:35.000000 torch_model_manager-1.0.1.dev2/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    24171 2024-05-29 08:15:42.000000 torch_model_manager-1.0.1.dev2/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-1.0.1.dev2/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-1.0.1.dev2/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:37:50.534091 torch_model_manager-1.0.1.dev2/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-29 09:37:50.000000 torch_model_manager-1.0.1.dev2/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-29 09:37:50.000000 torch_model_manager-1.0.1.dev2/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-29 09:37:50.000000 torch_model_manager-1.0.1.dev2/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      241 2024-05-29 09:37:50.000000 torch_model_manager-1.0.1.dev2/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-29 09:37:50.000000 torch_model_manager-1.0.1.dev2/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:37:50.534091 torch_model_manager-1.0.1.dev2/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev2/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-1.0.1.dev2/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:40:58.180503 torch_model_manager-1.0.1.dev3/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-29 09:40:58.180503 torch_model_manager-1.0.1.dev3/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev3/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-29 09:40:58.180503 torch_model_manager-1.0.1.dev3/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2243 2024-05-29 09:40:56.000000 torch_model_manager-1.0.1.dev3/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:40:58.176503 torch_model_manager-1.0.1.dev3/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:40:58.176503 torch_model_manager-1.0.1.dev3/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev3/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:40:58.176503 torch_model_manager-1.0.1.dev3/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev3/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev3/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:40:58.176503 torch_model_manager-1.0.1.dev3/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-1.0.1.dev3/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-1.0.1.dev3/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1725 2024-05-29 09:40:49.000000 torch_model_manager-1.0.1.dev3/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    24171 2024-05-29 08:15:42.000000 torch_model_manager-1.0.1.dev3/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-1.0.1.dev3/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-1.0.1.dev3/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:40:58.180503 torch_model_manager-1.0.1.dev3/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-29 09:40:58.000000 torch_model_manager-1.0.1.dev3/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-29 09:40:58.000000 torch_model_manager-1.0.1.dev3/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-29 09:40:58.000000 torch_model_manager-1.0.1.dev3/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      241 2024-05-29 09:40:58.000000 torch_model_manager-1.0.1.dev3/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-29 09:40:58.000000 torch_model_manager-1.0.1.dev3/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:40:58.176503 torch_model_manager-1.0.1.dev3/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev3/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-1.0.1.dev3/utils/helpers.py
```

### Comparing `torch_model_manager-1.0.1.dev2/PKG-INFO` & `torch_model_manager-1.0.1.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 1.0.1.dev2
+Version: 1.0.1.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-1.0.1.dev2/README.md` & `torch_model_manager-1.0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-1.0.1.dev2/setup.py` & `torch_model_manager-1.0.1.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='1.0.1.dev2',
+    version='1.0.1.dev3',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-1.0.1.dev2/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-1.0.1.dev3/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-1.0.1.dev2/tests/test_utils/test_helpers.py` & `torch_model_manager-1.0.1.dev3/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-1.0.1.dev2/torch_model_manager/neptune_manager.py` & `torch_model_manager-1.0.1.dev3/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-1.0.1.dev2/torch_model_manager/notebook_manager.py` & `torch_model_manager-1.0.1.dev3/torch_model_manager/notebook_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,10 +45,10 @@
         
 def execute_command(*args):
     """
     Execute a command with given executable and arguments.
     """
     # Construct the command
     command = " ".join(list(args))
-
+    print(command)
     # Execute the command using subprocess
     os.system(command)
```

### Comparing `torch_model_manager-1.0.1.dev2/torch_model_manager/segmentation_manager.py` & `torch_model_manager-1.0.1.dev3/torch_model_manager/segmentation_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-1.0.1.dev2/torch_model_manager/torch_model_manager.py` & `torch_model_manager-1.0.1.dev3/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-1.0.1.dev2/torch_model_manager/wandb_manager.py` & `torch_model_manager-1.0.1.dev3/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-1.0.1.dev2/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-1.0.1.dev3/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 1.0.1.dev2
+Version: 1.0.1.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-1.0.1.dev2/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-1.0.1.dev3/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-1.0.1.dev2/utils/helpers.py` & `torch_model_manager-1.0.1.dev3/utils/helpers.py`

 * *Files identical despite different names*

