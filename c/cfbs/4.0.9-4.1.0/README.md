# Comparing `tmp/cfbs-4.0.9.tar.gz` & `tmp/cfbs-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfbs-4.0.9.tar", last modified: Fri May  3 15:29:45 2024, max compression
+gzip compressed data, was "cfbs-4.1.0.tar", last modified: Wed May 29 11:56:51 2024, max compression
```

## Comparing `cfbs-4.0.9.tar` & `cfbs-4.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:45.281458 cfbs-4.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 15:29:37.000000 cfbs-4.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-05-03 15:29:45.281458 cfbs-4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-05-03 15:29:37.000000 cfbs-4.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:45.277458 cfbs-4.0.9/cfbs/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      288 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    18928 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/cfbs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/cfbs_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    40229 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/git_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/internal_file_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/pretty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21801 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:45.281458 cfbs-4.0.9/cfbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:29:45.281458 cfbs-4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-03 15:29:37.000000 cfbs-4.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:45.281458 cfbs-4.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_pretty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_validate_index_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_validate_mock_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_validate_mock_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:56:50.997216 cfbs-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 11:56:42.000000 cfbs-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-05-29 11:56:50.997216 cfbs-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-05-29 11:56:42.000000 cfbs-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:56:50.993216 cfbs-4.1.0/cfbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 11:56:50.000000 cfbs-4.1.0/cfbs/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      288 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19569 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/cfbs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/cfbs_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41321 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/git_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/internal_file_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21801 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 11:56:42.000000 cfbs-4.1.0/cfbs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:56:50.997216 cfbs-4.1.0/cfbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-05-29 11:56:50.000000 cfbs-4.1.0/cfbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-29 11:56:50.000000 cfbs-4.1.0/cfbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:56:50.000000 cfbs-4.1.0/cfbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-29 11:56:50.000000 cfbs-4.1.0/cfbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 11:56:50.000000 cfbs-4.1.0/cfbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:56:50.997216 cfbs-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-29 11:56:42.000000 cfbs-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:56:50.997216 cfbs-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 11:56:42.000000 cfbs-4.1.0/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-29 11:56:42.000000 cfbs-4.1.0/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-29 11:56:42.000000 cfbs-4.1.0/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-05-29 11:56:42.000000 cfbs-4.1.0/tests/test_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-29 11:56:42.000000 cfbs-4.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-29 11:56:42.000000 cfbs-4.1.0/tests/test_validate_index_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-29 11:56:42.000000 cfbs-4.1.0/tests/test_validate_mock_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-29 11:56:42.000000 cfbs-4.1.0/tests/test_validate_mock_input.py
```

### Comparing `cfbs-4.0.9/LICENSE` & `cfbs-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/PKG-INFO` & `cfbs-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfbs
-Version: 4.0.9
+Version: 4.1.0
 Summary: Tooling to build, manage and deploy CFEngine policy
 Home-page: https://github.com/cfengine/cfbs
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfbs-4.0.9/README.md` & `cfbs-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/args.py` & `cfbs-4.1.0/cfbs/args.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/build.py` & `cfbs-4.1.0/cfbs/build.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/cfbs_config.py` & `cfbs-4.1.0/cfbs/cfbs_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,38 +127,51 @@
         if "@" in url and (url.rindex("@") > url.rindex(".")):
             assert url.split("@")[-1] == url_commit
             url = url[0 : url.rindex("@")]
 
         remote_config = CFBSJson(path=config_path, url=url, url_commit=url_commit)
 
         provides = remote_config.get_provides()
+        add_all = True
         # URL specified in to_add, but no specific modules => let's add all (with a prompt)
         if len(to_add) == 0:
             modules = list(provides.values())
-            print("Found %d modules in '%s':" % (len(modules), url))
-            for m in modules:
-                print("  - " + m["name"])
             if not any(modules):
                 user_error("no modules available, nothing to do")
-            if not self.non_interactive:
+            print("Found %d modules in '%s':" % (len(modules), url))
+            for m in modules:
+                deps = m.get("dependencies", [])
+                deps = "" if not deps else " (Depends on: " + ", ".join(deps) + ")"
+                print("  - " + m["name"] + deps)
+            if len(modules) > 1 and not self.non_interactive:
                 answer = prompt_user(
                     non_interactive=self.non_interactive,
                     prompt="Do you want to add all %d of them?" % (len(modules)),
                     choices=YES_NO_CHOICES,
-                    default="no",
+                    default="yes",
                 )
                 if answer.lower() not in ("y", "yes"):
-                    return
+                    add_all = False
         else:
             missing = [k for k in to_add if k not in provides]
             if missing:
                 user_error("Missing modules: " + ", ".join(missing))
             modules = [provides[k] for k in to_add]
 
-        for module in modules:
+        for i, module in enumerate(modules, start=1):
+            if not add_all:
+                answer = prompt_user(
+                    non_interactive=self.non_interactive,
+                    prompt="(%d/%d) Do you want to add '%s'?"
+                    % (i, len(modules), module["name"]),
+                    choices=YES_NO_CHOICES,
+                    default="yes",
+                )
+                if answer.lower() not in ("y", "yes"):
+                    continue
             self.add_with_dependencies(module, remote_config)
 
     @staticmethod
     def _convert_added_by(added_by, to_add):
         # Convert string -> list:
         if type(added_by) is str:
             added_by = [added_by] * len(to_add)
```

### Comparing `cfbs-4.0.9/cfbs/cfbs_json.py` & `cfbs-4.1.0/cfbs/cfbs_json.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/commands.py` & `cfbs-4.1.0/cfbs/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import os
 import re
 import copy
 import logging as log
 import json
 import sys
+import functools
 from collections import OrderedDict
 from cfbs.args import get_args
 
 from cfbs.utils import (
     cfbs_dir,
     cfbs_filename,
     is_cfbs_repo,
@@ -235,53 +236,55 @@
     The CFBSConfig instance was initally created in main(). Back then
     cfbs.json did not exist, thus the instance is empty. Ensure it is reloaded
     now that the JSON exists.
     """
     CFBSConfig.reload()
 
     branch = None
-    to_add = ""
+    to_add = []
     if masterfiles is None:
         if prompt_user(
             non_interactive,
             "Do you wish to build on top of the default policy set, masterfiles? (Recommended)",
             choices=YES_NO_CHOICES,
             default="yes",
         ) in ("yes", "y"):
-            to_add = "masterfiles"
+            to_add = ["masterfiles"]
         else:
-            to_add = prompt_user(
-                non_interactive,
-                "Specify policy set to use instead (empty to skip)",
-                default="",
-            )
+            to_add = [
+                prompt_user(
+                    non_interactive,
+                    "Specify policy set to use instead (empty to skip)",
+                    default="",
+                )
+            ]
     elif re.match(r"[0-9]+(\.[0-9]+){2}(\-[0-9]+)?", masterfiles):
         log.debug("--masterfiles=%s appears to be a version number" % masterfiles)
-        to_add = "masterfiles@%s" % masterfiles
+        to_add = ["masterfiles@%s" % masterfiles]
     elif masterfiles != "no":
         """This appears to be a branch. Thus we'll add masterfiles normally
         and try to do the necessary modifications needed afterwards. I.e.
         changing the 'repo' attribute to be 'url' and changing the commit to
         be the current HEAD of the upstream branch."""
 
         log.debug("--masterfiles=%s appears to be a branch" % masterfiles)
         branch = masterfiles
-        to_add = "masterfiles"
+        to_add = ["masterfiles"]
 
     if branch is not None:
         remote = "https://github.com/cfengine/masterfiles"
         commit = ls_remote(remote, branch)
         if commit is None:
             user_error(
                 "Failed to find branch or tag %s at remote %s" % (branch, remote)
             )
         log.debug("Current commit for masterfiles branch %s is %s" % (branch, commit))
-        to_add = "%s@%s" % (remote, commit)
+        to_add = ["%s@%s" % (remote, commit), "masterfiles"]
     if to_add:
-        ret = add_command([to_add])
+        ret = add_command(to_add, added_by="cfbs init")
         if ret != 0:
             return ret
 
     return 0
 
 
 @cfbs_command("status")
@@ -379,23 +382,53 @@
     config.warn_about_unknown_keys()
     if not "build" in config:
         user_error(
             'Cannot remove any modules because the "build" key is missing from cfbs.json'
         )
     modules = config["build"]
 
+    def _get_dependents(dependency) -> list:
+        if len(modules) < 2:
+            return []
+
+        def reduce_dependencies(a, b):
+            result_b = [b["name"]] if dependency in b.get("dependencies", []) else []
+            if type(a) is list:
+                return a + result_b
+            else:
+                return (
+                    [a["name"]] if dependency in a.get("dependencies", []) else []
+                ) + result_b
+
+        return functools.reduce(reduce_dependencies, modules)
+
     def _get_module_by_name(name) -> dict:
         if not name.startswith("./") and name.endswith(".cf") and os.path.exists(name):
             name = "./" + name
 
         for module in modules:
             if module["name"] == name:
                 return module
         return None
 
+    def _remove_module_user_prompt(module):
+        dependents = _get_dependents(module["name"])
+        return prompt_user(
+            config.non_interactive,
+            "Do you wish to remove '%s'?" % module["name"]
+            + (
+                " (The module is a dependency of the following module%s: %s)"
+                % ("s" if len(dependents) > 1 else "", ", ".join(dependents))
+                if dependents
+                else ""
+            ),
+            choices=YES_NO_CHOICES,
+            default="yes",
+        )
+
     def _get_modules_by_url(name) -> list:
         r = []
         for module in modules:
             if "url" in module and module["url"] == name:
                 r.append(module)
         return r
 
@@ -404,32 +437,29 @@
     files = []
     for name in to_remove:
         if name.startswith(("https://", "ssh://", "git://")):
             matches = _get_modules_by_url(name)
             if not matches:
                 user_error("Could not find module with URL '%s'" % name)
             for module in matches:
-                answer = prompt_user(
-                    config.non_interactive,
-                    "Do you wish to remove '%s'?" % module["name"],
-                    choices=YES_NO_CHOICES,
-                    default="yes",
-                )
+                answer = _remove_module_user_prompt(module)
                 if answer.lower() in ("yes", "y"):
                     print("Removing module '%s'" % module["name"])
                     modules.remove(module)
                     msg += "\n - Removed module '%s'" % module["name"]
                     num_removed += 1
         else:
             module = _get_module_by_name(name)
             if module:
-                print("Removing module '%s'" % name)
-                modules.remove(module)
-                msg += "\n - Removed module '%s'" % module["name"]
-                num_removed += 1
+                answer = _remove_module_user_prompt(module)
+                if answer.lower() in ("yes", "y"):
+                    print("Removing module '%s'" % name)
+                    modules.remove(module)
+                    msg += "\n - Removed module '%s'" % module["name"]
+                    num_removed += 1
             else:
                 print("Module '%s' not found" % name)
         input_path = os.path.join(".", name, "input.json")
         if os.path.isfile(input_path) and prompt_user(
             config.non_interactive,
             "Module '%s' has input data '%s'. Do you want to remove it?"
             % (name, input_path),
```

### Comparing `cfbs-4.0.9/cfbs/git.py` & `cfbs-4.1.0/cfbs/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Should be fairly reusable, not depending on other parts
 of the CFBS codebase.
 
 See git_magic.py for more git related code.
 """
 
 import os
+import itertools
 import tempfile
 from subprocess import check_call, check_output, run, PIPE, DEVNULL, CalledProcessError
 
 
 class CFBSGitError(Exception):
     pass
 
@@ -185,15 +186,20 @@
         result = run(["git", "status", "-s", "-u"], check=True, stdout=PIPE)
         if "all" in scope:
             if len(result.stdout) > 0:
                 should_commit = True
         else:
             lines = result.stdout.decode("utf-8").split("\n")
             changes = [line.strip().split(" ")[1] for line in lines if line]
-            should_commit = any(i in changes for i in scope)
+            should_commit = any(
+                map(
+                    lambda x: os.path.samefile(*x),
+                    list(itertools.product(changes, scope)),
+                )
+            )
         if not should_commit:
             print("No changes to commit")
         return should_commit
     except CalledProcessError as cpe:
         raise CFBSGitError(
             "Failed to run 'git status -s -u' to check for changes."
         ) from cpe
```

### Comparing `cfbs-4.0.9/cfbs/git_magic.py` & `cfbs-4.1.0/cfbs/git_magic.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/index.py` & `cfbs-4.1.0/cfbs/index.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/internal_file_management.py` & `cfbs-4.1.0/cfbs/internal_file_management.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/main.py` & `cfbs-4.1.0/cfbs/main.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/module.py` & `cfbs-4.1.0/cfbs/module.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/pretty.py` & `cfbs-4.1.0/cfbs/pretty.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/prompts.py` & `cfbs-4.1.0/cfbs/prompts.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/utils.py` & `cfbs-4.1.0/cfbs/utils.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs/validate.py` & `cfbs-4.1.0/cfbs/validate.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/cfbs.egg-info/PKG-INFO` & `cfbs-4.1.0/cfbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfbs
-Version: 4.0.9
+Version: 4.1.0
 Summary: Tooling to build, manage and deploy CFEngine policy
 Home-page: https://github.com/cfengine/cfbs
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfbs-4.0.9/cfbs.egg-info/SOURCES.txt` & `cfbs-4.1.0/cfbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/setup.py` & `cfbs-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/tests/test_input.py` & `cfbs-4.1.0/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/tests/test_module.py` & `cfbs-4.1.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/tests/test_pretty.py` & `cfbs-4.1.0/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/tests/test_utils.py` & `cfbs-4.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/tests/test_validate_index_alias.py` & `cfbs-4.1.0/tests/test_validate_index_alias.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/tests/test_validate_mock_index.py` & `cfbs-4.1.0/tests/test_validate_mock_index.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.9/tests/test_validate_mock_input.py` & `cfbs-4.1.0/tests/test_validate_mock_input.py`

 * *Files identical despite different names*

