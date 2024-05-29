# Comparing `tmp/prjit-0.0.2.tar.gz` & `tmp/prjit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prjit-0.0.2.tar", last modified: Mon May 27 08:10:32 2024, max compression
+gzip compressed data, was "prjit-0.0.3.tar", last modified: Wed May 29 08:20:37 2024, max compression
```

## Comparing `prjit-0.0.2.tar` & `prjit-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-27 08:10:32.956447 prjit-0.0.2/
--rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-27 08:10:32.956248 prjit-0.0.2/PKG-INFO
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-27 08:10:32.953476 prjit-0.0.2/bin/
--rwxr-xr-x   0 archiba    (501) staff       (20)    17563 2024-05-27 07:31:05.000000 prjit-0.0.2/bin/prjit
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-27 08:10:32.956057 prjit-0.0.2/prjit.egg-info/
--rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-27 08:10:32.000000 prjit-0.0.2/prjit.egg-info/PKG-INFO
--rw-r--r--   0 archiba    (501) staff       (20)      261 2024-05-27 08:10:32.000000 prjit-0.0.2/prjit.egg-info/SOURCES.txt
--rw-r--r--   0 archiba    (501) staff       (20)        1 2024-05-27 08:10:32.000000 prjit-0.0.2/prjit.egg-info/dependency_links.txt
--rw-r--r--   0 archiba    (501) staff       (20)       75 2024-05-27 08:10:32.000000 prjit-0.0.2/prjit.egg-info/requires.txt
--rw-r--r--   0 archiba    (501) staff       (20)        9 2024-05-27 08:10:32.000000 prjit-0.0.2/prjit.egg-info/top_level.txt
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-27 08:10:32.955874 prjit-0.0.2/prjitter/
--rw-r--r--   0 archiba    (501) staff       (20)       22 2024-05-27 08:10:22.000000 prjit-0.0.2/prjitter/__init__.py
--rw-r--r--   0 archiba    (501) staff       (20)     1962 2024-05-27 07:05:22.000000 prjit-0.0.2/prjitter/bundles.py
--rw-r--r--   0 archiba    (501) staff       (20)     4335 2024-05-27 05:46:21.000000 prjit-0.0.2/prjitter/config.py
--rw-r--r--   0 archiba    (501) staff       (20)     3794 2024-05-27 07:27:41.000000 prjit-0.0.2/prjitter/state.py
--rw-r--r--   0 archiba    (501) staff       (20)     3958 2024-05-27 08:10:10.000000 prjit-0.0.2/prjitter/switcher.py
--rw-r--r--   0 archiba    (501) staff       (20)       38 2024-05-27 08:10:32.956486 prjit-0.0.2/setup.cfg
--rw-r--r--   0 archiba    (501) staff       (20)      609 2024-05-27 08:10:22.000000 prjit-0.0.2/setup.py
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:20:37.523127 prjit-0.0.3/
+-rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:20:37.522914 prjit-0.0.3/PKG-INFO
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:20:37.521162 prjit-0.0.3/bin/
+-rwxr-xr-x   0 archiba    (501) staff       (20)    18214 2024-05-29 08:19:19.000000 prjit-0.0.3/bin/prjit
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:20:37.522706 prjit-0.0.3/prjit.egg-info/
+-rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/PKG-INFO
+-rw-r--r--   0 archiba    (501) staff       (20)      261 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/SOURCES.txt
+-rw-r--r--   0 archiba    (501) staff       (20)        1 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/dependency_links.txt
+-rw-r--r--   0 archiba    (501) staff       (20)       75 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/requires.txt
+-rw-r--r--   0 archiba    (501) staff       (20)        9 2024-05-29 08:20:37.000000 prjit-0.0.3/prjit.egg-info/top_level.txt
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:20:37.522521 prjit-0.0.3/prjitter/
+-rw-r--r--   0 archiba    (501) staff       (20)       22 2024-05-29 08:19:51.000000 prjit-0.0.3/prjitter/__init__.py
+-rw-r--r--   0 archiba    (501) staff       (20)     1962 2024-05-27 07:05:22.000000 prjit-0.0.3/prjitter/bundles.py
+-rw-r--r--   0 archiba    (501) staff       (20)     4420 2024-05-29 08:14:35.000000 prjit-0.0.3/prjitter/config.py
+-rw-r--r--   0 archiba    (501) staff       (20)     3794 2024-05-27 07:27:41.000000 prjit-0.0.3/prjitter/state.py
+-rw-r--r--   0 archiba    (501) staff       (20)     3958 2024-05-27 08:10:10.000000 prjit-0.0.3/prjitter/switcher.py
+-rw-r--r--   0 archiba    (501) staff       (20)       38 2024-05-29 08:20:37.523164 prjit-0.0.3/setup.cfg
+-rw-r--r--   0 archiba    (501) staff       (20)      609 2024-05-29 08:20:35.000000 prjit-0.0.3/setup.py
```

### Comparing `prjit-0.0.2/bin/prjit` & `prjit-0.0.3/bin/prjit`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 import subprocess
+from datetime import datetime
 from pathlib import Path
 
 import inquirer
 import prompt_toolkit.completion
 import prompt_toolkit.document
 from fire import Fire
 
@@ -65,14 +66,15 @@
         default_project_config.dump(global_config)
         default_project_config.create_switch_root_path(global_config)
         print('Done initializing prjit')
 
     def switch(self, dry_run: bool = False):
         global_config = GlobalConfig.load_from_env()
         state = PrjitState.load_config(global_config)
+        old_project = state.current_project
         project_names = [project.project_name for project in state.project_configs]
         print('Switching into project...')
         questions = [
             inquirer.List("project_name",
                           message="Choose a project to switch into",
                           choices=project_names)
         ]
@@ -92,20 +94,25 @@
             for command in switch_commands:
                 print('Executing:', ' '.join(command))
                 if not dry_run:
                     subprocess.run(command)
             state.current_project = project_name
             state.bound_bundle_ids = []
             state.save_current()
+            switch_log_path = global_config.switch_log_path()
+            if old_project is None:
+                switch_log_path.open('a').write(f'Action:exit,ProjectName:{old_project},Time:{datetime.now().isoformat()}\n')
+            switch_log_path.open('a').write(f'Action:switch,ProjectName:{project_name},Time:{datetime.now().isoformat()}\n')
         else:
             print('Switching cancelled')
 
     def exit(self, dry_run: bool = False):
         global_config = GlobalConfig.load_from_env()
         state = PrjitState.load_config(global_config)
+        old_project = state.current_project
         switcher = PrjitSwitcher(state)
         switch_commands = switcher.plan_switch_out()
         print('Following commands will be executed:')
         for command in switch_commands:
             print(' '.join(command))
         questions = [
             inquirer.Confirm("confirm",
@@ -116,14 +123,16 @@
             for command in switch_commands:
                 print('Executing:', ' '.join(command))
                 if not dry_run:
                     subprocess.run(command)
             state.current_project = None
             state.bound_bundle_ids = []
             state.save_current()
+            switch_log_path = global_config.switch_log_path()
+            switch_log_path.open('a').write(f'Action:exit,ProjectName:{old_project},Time:{datetime.now().isoformat()}\n')
         else:
             print('Switching out cancelled')
 
     def project(self):
         global_config = GlobalConfig.load_from_env()
         state = PrjitState.load_config(global_config)
         print('You can manage projects here.')
```

### Comparing `prjit-0.0.2/prjitter/bundles.py` & `prjit-0.0.3/prjitter/bundles.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.2/prjitter/config.py` & `prjit-0.0.3/prjitter/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         prjit_root_dir = getenv("PRJIT_ROOT_DIR", str(default_prjit_root_dir_path.absolute()))
         prjit_root_dir_path = Path(prjit_root_dir).absolute()
         return cls(root_dir=str(prjit_root_dir_path))
 
     def root_path(self):
         return Path(self.root_dir)
 
+    def switch_log_path(self) -> Path:
+        return self.root_path / 'switch.log'
+
 
 class PrjitSwitchPath(BaseModel):
     name: str = Field(description="The name of the switch path")
     path: str = Field(description="The path of the switch path")
     is_directory: bool = Field(description="Whether the switch path is a directory", default=True)
 
     def __str__(self) -> str:
```

### Comparing `prjit-0.0.2/prjitter/state.py` & `prjit-0.0.3/prjitter/state.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.2/prjitter/switcher.py` & `prjit-0.0.3/prjitter/switcher.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.2/setup.py` & `prjit-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='prjit',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(include=['prjitter', 'prjitter.*']),
     url='https://github.com/archiba/prjit',
     license='',
     author='archiba',
     author_email='yuki-chiba@outlook.jp',
     description='Define a project workspace and switch files and applications',
     python_requirems='>=3.9',
```

