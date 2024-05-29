# Comparing `tmp/prjit-0.0.3.tar.gz` & `tmp/prjit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prjit-0.0.3.tar", last modified: Wed May 29 08:20:37 2024, max compression
+gzip compressed data, was "prjit-0.0.4.tar", last modified: Wed May 29 08:22:27 2024, max compression
```

## Comparing `prjit-0.0.3.tar` & `prjit-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:20:37.523127 prjit-0.0.3/
--rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:20:37.522914 prjit-0.0.3/PKG-INFO
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:20:37.521162 prjit-0.0.3/bin/
--rwxr-xr-x   0 archiba    (501) staff       (20)    18214 2024-05-29 08:19:19.000000 prjit-0.0.3/bin/prjit
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:20:37.522706 prjit-0.0.3/prjit.egg-info/
--rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/PKG-INFO
--rw-r--r--   0 archiba    (501) staff       (20)      261 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/SOURCES.txt
--rw-r--r--   0 archiba    (501) staff       (20)        1 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/dependency_links.txt
--rw-r--r--   0 archiba    (501) staff       (20)       75 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/requires.txt
--rw-r--r--   0 archiba    (501) staff       (20)        9 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/top_level.txt
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:20:37.522521 prjit-0.0.3/prjitter/
--rw-r--r--   0 archiba    (501) staff       (20)       22 2024-05-29 08:19:51.000000 prjit-0.0.3/prjitter/__init__.py
--rw-r--r--   0 archiba    (501) staff       (20)     1962 2024-05-27 07:05:22.000000 prjit-0.0.3/prjitter/bundles.py
--rw-r--r--   0 archiba    (501) staff       (20)     4420 2024-05-29 08:14:35.000000 prjit-0.0.3/prjitter/config.py
--rw-r--r--   0 archiba    (501) staff       (20)     3794 2024-05-27 07:27:41.000000 prjit-0.0.3/prjitter/state.py
--rw-r--r--   0 archiba    (501) staff       (20)     3958 2024-05-27 08:10:10.000000 prjit-0.0.3/prjitter/switcher.py
--rw-r--r--   0 archiba    (501) staff       (20)       38 2024-05-29 08:20:37.523164 prjit-0.0.3/setup.cfg
--rw-r--r--   0 archiba    (501) staff       (20)      609 2024-05-29 08:20:35.000000 prjit-0.0.3/setup.py
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:22:27.202182 prjit-0.0.4/
+-rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:22:27.201989 prjit-0.0.4/PKG-INFO
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:22:27.200244 prjit-0.0.4/bin/
+-rwxr-xr-x   0 archiba    (501) staff       (20)    18214 2024-05-29 08:19:19.000000 prjit-0.0.4/bin/prjit
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:22:27.201781 prjit-0.0.4/prjit.egg-info/
+-rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/PKG-INFO
+-rw-r--r--   0 archiba    (501) staff       (20)      261 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/SOURCES.txt
+-rw-r--r--   0 archiba    (501) staff       (20)        1 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/dependency_links.txt
+-rw-r--r--   0 archiba    (501) staff       (20)       75 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/requires.txt
+-rw-r--r--   0 archiba    (501) staff       (20)        9 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/top_level.txt
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:22:27.201595 prjit-0.0.4/prjitter/
+-rw-r--r--   0 archiba    (501) staff       (20)       22 2024-05-29 08:22:20.000000 prjit-0.0.4/prjitter/__init__.py
+-rw-r--r--   0 archiba    (501) staff       (20)     1962 2024-05-27 07:05:22.000000 prjit-0.0.4/prjitter/bundles.py
+-rw-r--r--   0 archiba    (501) staff       (20)     4422 2024-05-29 08:22:15.000000 prjit-0.0.4/prjitter/config.py
+-rw-r--r--   0 archiba    (501) staff       (20)     3794 2024-05-27 07:27:41.000000 prjit-0.0.4/prjitter/state.py
+-rw-r--r--   0 archiba    (501) staff       (20)     3958 2024-05-27 08:10:10.000000 prjit-0.0.4/prjitter/switcher.py
+-rw-r--r--   0 archiba    (501) staff       (20)       38 2024-05-29 08:22:27.202219 prjit-0.0.4/setup.cfg
+-rw-r--r--   0 archiba    (501) staff       (20)      609 2024-05-29 08:22:23.000000 prjit-0.0.4/setup.py
```

### Comparing `prjit-0.0.3/bin/prjit` & `prjit-0.0.4/bin/prjit`

 * *Files identical despite different names*

### Comparing `prjit-0.0.3/prjitter/bundles.py` & `prjit-0.0.4/prjitter/bundles.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.3/prjitter/config.py` & `prjit-0.0.4/prjitter/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         prjit_root_dir_path = Path(prjit_root_dir).absolute()
         return cls(root_dir=str(prjit_root_dir_path))
 
     def root_path(self):
         return Path(self.root_dir)
 
     def switch_log_path(self) -> Path:
-        return self.root_path / 'switch.log'
+        return self.root_path() / 'switch.log'
 
 
 class PrjitSwitchPath(BaseModel):
     name: str = Field(description="The name of the switch path")
     path: str = Field(description="The path of the switch path")
     is_directory: bool = Field(description="Whether the switch path is a directory", default=True)
```

### Comparing `prjit-0.0.3/prjitter/state.py` & `prjit-0.0.4/prjitter/state.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.3/prjitter/switcher.py` & `prjit-0.0.4/prjitter/switcher.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.3/setup.py` & `prjit-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='prjit',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(include=['prjitter', 'prjitter.*']),
     url='https://github.com/archiba/prjit',
     license='',
     author='archiba',
     author_email='yuki-chiba@outlook.jp',
     description='Define a project workspace and switch files and applications',
     python_requirems='>=3.9',
```

