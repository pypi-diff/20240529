# Comparing `tmp/torch_model_manager-0.4.3.dev2.tar.gz` & `tmp/torch_model_manager-1.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.3.dev2.tar", last modified: Tue May 28 21:06:11 2024, max compression
+gzip compressed data, was "torch_model_manager-1.0.1.dev1.tar", last modified: Wed May 29 09:21:12 2024, max compression
```

## Comparing `torch_model_manager-0.4.3.dev2.tar` & `torch_model_manager-1.0.1.dev1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:06:11.818942 torch_model_manager-0.4.3.dev2/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 21:06:11.814942 torch_model_manager-0.4.3.dev2/PKG-INFO
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev2/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 21:06:11.818942 torch_model_manager-0.4.3.dev2/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 21:06:08.000000 torch_model_manager-0.4.3.dev2/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:06:11.798941 torch_model_manager-0.4.3.dev2/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:06:11.798941 torch_model_manager-0.4.3.dev2/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev2/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:06:11.802941 torch_model_manager-0.4.3.dev2/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev2/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev2/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:06:11.802941 torch_model_manager-0.4.3.dev2/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev2/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev2/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1627 2024-05-28 20:55:15.000000 torch_model_manager-0.4.3.dev2/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24171 2024-05-28 21:05:47.000000 torch_model_manager-0.4.3.dev2/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev2/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev2/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:06:11.810942 torch_model_manager-0.4.3.dev2/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 21:06:11.000000 torch_model_manager-0.4.3.dev2/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 21:06:11.000000 torch_model_manager-0.4.3.dev2/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 21:06:11.000000 torch_model_manager-0.4.3.dev2/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 21:06:11.000000 torch_model_manager-0.4.3.dev2/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 21:06:11.000000 torch_model_manager-0.4.3.dev2/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:06:11.806942 torch_model_manager-0.4.3.dev2/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev2/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev2/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:21:12.064753 torch_model_manager-1.0.1.dev1/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-29 09:21:12.064753 torch_model_manager-1.0.1.dev1/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev1/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-29 09:21:12.068753 torch_model_manager-1.0.1.dev1/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2243 2024-05-29 09:21:10.000000 torch_model_manager-1.0.1.dev1/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:21:12.064753 torch_model_manager-1.0.1.dev1/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:21:12.064753 torch_model_manager-1.0.1.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:21:12.064753 torch_model_manager-1.0.1.dev1/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:21:12.064753 torch_model_manager-1.0.1.dev1/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-1.0.1.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-1.0.1.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1729 2024-05-29 09:02:04.000000 torch_model_manager-1.0.1.dev1/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    24171 2024-05-29 08:15:42.000000 torch_model_manager-1.0.1.dev1/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-1.0.1.dev1/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-1.0.1.dev1/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:21:12.064753 torch_model_manager-1.0.1.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-29 09:21:12.000000 torch_model_manager-1.0.1.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-29 09:21:12.000000 torch_model_manager-1.0.1.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-29 09:21:12.000000 torch_model_manager-1.0.1.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      241 2024-05-29 09:21:12.000000 torch_model_manager-1.0.1.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-29 09:21:12.000000 torch_model_manager-1.0.1.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-29 09:21:12.064753 torch_model_manager-1.0.1.dev1/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-1.0.1.dev1/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-1.0.1.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.3.dev2/PKG-INFO` & `torch_model_manager-1.0.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.3.dev2
+Version: 1.0.1.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.3.dev2/README.md` & `torch_model_manager-1.0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.3.dev2/setup.py` & `torch_model_manager-1.0.1.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.3.dev2',
+    version='1.0.1.dev1',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.3.dev2/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-1.0.1.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.3.dev2/tests/test_utils/test_helpers.py` & `torch_model_manager-1.0.1.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.3.dev2/torch_model_manager/neptune_manager.py` & `torch_model_manager-1.0.1.dev1/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.3.dev2/torch_model_manager/notebook_manager.py` & `torch_model_manager-1.0.1.dev1/torch_model_manager/notebook_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import subprocess
     
-def clone_repo(project, user, branch = None, token=None, move_to_root=True, change_dir=None):
+def clone_repo(project, user, branch = None, token=None, move_to_root=True, delete_original = True, change_dir=None):
     """
     Clone a repository from a given URL to a given directory.
     """
     assert (move_to_root and not change_dir) or (not move_to_root and change_dir), "Only one of move_to_root and change_dir can be True"
+
     # Clone the repository
     if token is not None:
         github_url = f"https://{token}@github.com/{user}/{project}.git"
     else:
         github_url = f"https://github.com/{user}/{project}.git"
     
     # Clone the repository using variables
@@ -17,14 +18,18 @@
         os.system(f"git clone -b {branch} {github_url}")
     else:
         os.system(f"git clone {github_url}")
         
     
     if move_to_root:
         os.system(f"mv {project}/* .")
+        if delete_original:
+            os.system(f"rm -rf {project}")
+    
+
     
     if change_dir:
         os.chdir(project)
 
 def install_dependencies(requirements_file="requirements.txt", script_file="requirements.sh", compiler="bash"):
     """
     Install the requirements from the requirements.txt file.
```

### Comparing `torch_model_manager-0.4.3.dev2/torch_model_manager/segmentation_manager.py` & `torch_model_manager-1.0.1.dev1/torch_model_manager/segmentation_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.3.dev2/torch_model_manager/torch_model_manager.py` & `torch_model_manager-1.0.1.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.3.dev2/torch_model_manager/wandb_manager.py` & `torch_model_manager-1.0.1.dev1/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.3.dev2/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-1.0.1.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.3.dev2
+Version: 1.0.1.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.3.dev2/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-1.0.1.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.3.dev2/utils/helpers.py` & `torch_model_manager-1.0.1.dev1/utils/helpers.py`

 * *Files identical despite different names*

