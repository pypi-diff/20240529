# Comparing `tmp/rxd-0.0.8.tar.gz` & `tmp/rxd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxd-0.0.8.tar", last modified: Mon May 27 00:49:43 2024, max compression
+gzip compressed data, was "rxd-0.0.9.tar", last modified: Mon May 27 01:23:01 2024, max compression
```

## Comparing `rxd-0.0.8.tar` & `rxd-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:49:43.405976 rxd-0.0.8/
--rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-27 00:49:43.405582 rxd-0.0.8/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:51:53.000000 rxd-0.0.8/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:49:43.400494 rxd-0.0.8/rxd/
--rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:58:36.000000 rxd-0.0.8/rxd/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)     5910 2024-05-27 00:48:42.000000 rxd-0.0.8/rxd/app_manager.py
--rwxr-xr-x   0 huy        (501) staff       (20)      410 2024-05-25 23:57:42.000000 rxd-0.0.8/rxd/ask.py
--rw-r--r--   0 huy        (501) staff       (20)      939 2024-05-26 23:27:05.000000 rxd-0.0.8/rxd/cmd.py
--rw-r--r--   0 huy        (501) staff       (20)     1815 2024-05-26 20:22:11.000000 rxd-0.0.8/rxd/cmd_app.py
--rw-r--r--   0 huy        (501) staff       (20)     1148 2024-05-26 20:16:36.000000 rxd-0.0.8/rxd/cmd_responder.py
--rw-r--r--   0 huy        (501) staff       (20)      358 2024-05-25 12:54:20.000000 rxd-0.0.8/rxd/cmd_setup.py
--rw-r--r--   0 huy        (501) staff       (20)      111 2024-05-26 20:17:01.000000 rxd-0.0.8/rxd/cmd_worker_daemon.py
--rw-r--r--   0 huy        (501) staff       (20)     2794 2024-05-25 22:31:16.000000 rxd-0.0.8/rxd/codex.py
--rw-r--r--   0 huy        (501) staff       (20)      143 2024-05-26 16:11:09.000000 rxd-0.0.8/rxd/messages.py
--rw-r--r--   0 huy        (501) staff       (20)      113 2024-05-25 23:36:37.000000 rxd-0.0.8/rxd/worker.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:49:43.404914 rxd-0.0.8/rxd.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-27 00:49:43.000000 rxd-0.0.8/rxd.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      386 2024-05-27 00:49:43.000000 rxd-0.0.8/rxd.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-27 00:49:43.000000 rxd-0.0.8/rxd.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-27 00:49:43.000000 rxd-0.0.8/rxd.egg-info/entry_points.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 05:12:36.000000 rxd-0.0.8/rxd.egg-info/not-zip-safe
--rw-r--r--   0 huy        (501) staff       (20)       12 2024-05-27 00:49:43.000000 rxd-0.0.8/rxd.egg-info/requires.txt
--rw-r--r--   0 huy        (501) staff       (20)        4 2024-05-27 00:49:43.000000 rxd-0.0.8/rxd.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-27 00:49:43.406127 rxd-0.0.8/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)      788 2024-05-27 00:49:35.000000 rxd-0.0.8/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 01:23:01.875035 rxd-0.0.9/
+-rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-27 01:23:01.874643 rxd-0.0.9/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:51:53.000000 rxd-0.0.9/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 01:23:01.869789 rxd-0.0.9/rxd/
+-rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:58:36.000000 rxd-0.0.9/rxd/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)     5857 2024-05-27 01:22:40.000000 rxd-0.0.9/rxd/app_manager.py
+-rwxr-xr-x   0 huy        (501) staff       (20)      410 2024-05-25 23:57:42.000000 rxd-0.0.9/rxd/ask.py
+-rw-r--r--   0 huy        (501) staff       (20)      939 2024-05-26 23:27:05.000000 rxd-0.0.9/rxd/cmd.py
+-rw-r--r--   0 huy        (501) staff       (20)     1815 2024-05-26 20:22:11.000000 rxd-0.0.9/rxd/cmd_app.py
+-rw-r--r--   0 huy        (501) staff       (20)     1148 2024-05-26 20:16:36.000000 rxd-0.0.9/rxd/cmd_responder.py
+-rw-r--r--   0 huy        (501) staff       (20)      358 2024-05-25 12:54:20.000000 rxd-0.0.9/rxd/cmd_setup.py
+-rw-r--r--   0 huy        (501) staff       (20)      111 2024-05-26 20:17:01.000000 rxd-0.0.9/rxd/cmd_worker_daemon.py
+-rw-r--r--   0 huy        (501) staff       (20)     2794 2024-05-25 22:31:16.000000 rxd-0.0.9/rxd/codex.py
+-rw-r--r--   0 huy        (501) staff       (20)      143 2024-05-26 16:11:09.000000 rxd-0.0.9/rxd/messages.py
+-rw-r--r--   0 huy        (501) staff       (20)      113 2024-05-25 23:36:37.000000 rxd-0.0.9/rxd/worker.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 01:23:01.873965 rxd-0.0.9/rxd.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-27 01:23:01.000000 rxd-0.0.9/rxd.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      386 2024-05-27 01:23:01.000000 rxd-0.0.9/rxd.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-27 01:23:01.000000 rxd-0.0.9/rxd.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-27 01:23:01.000000 rxd-0.0.9/rxd.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 05:12:36.000000 rxd-0.0.9/rxd.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (501) staff       (20)       12 2024-05-27 01:23:01.000000 rxd-0.0.9/rxd.egg-info/requires.txt
+-rw-r--r--   0 huy        (501) staff       (20)        4 2024-05-27 01:23:01.000000 rxd-0.0.9/rxd.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-27 01:23:01.875187 rxd-0.0.9/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)      788 2024-05-27 01:22:55.000000 rxd-0.0.9/setup.py
```

### Comparing `rxd-0.0.8/rxd/app_manager.py` & `rxd-0.0.9/rxd/app_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             After=network.target
             StartLimitIntervalSec=30
             StartLimitBurst=5
 
             [Service]
             Type=forking
             User={user}
-            ExecStart=/usr/bin/screen -dmS rxd-app-{screen_name} {python_path} -m rxd.cmd app run {self.name}
+            ExecStart={python_path} -m rxd.cmd app run {self.name}
             Restart=always
             RestartSec=5
 
             [Install]
             WantedBy=default.target
             """
         systemd_service_file = textwrap.dedent(systemd_service_file)
@@ -178,20 +178,20 @@
         print(f'Writing {self.systemd_services_definition_path}')
         with open(self.systemd_services_definition_path, "w") as fh:
             fh.write(systemd_service_file)
 
         if Path('/etc/systemd/system').exists():
             if not systemd_service_install_path.exists():
 
-                print("Symlinking %s -> %s" %
+                print("Moving %s -> %s" %
                       (self.systemd_services_definition_path,
                        systemd_service_install_path))
                 print("We need sudo permissions to do so")
                 sp.check_call(
-                    ["sudo", "ln", "-s",
+                    ["sudo", "mv",
                      self.systemd_services_definition_path,
                      systemd_service_install_path])
         else:
             print("Systemd does not exist")
 
     def __repr__(self):
         return "Application(name=%s, repo=%s)" % (self.name, self.repo)
```

### Comparing `rxd-0.0.8/rxd/cmd.py` & `rxd-0.0.9/rxd/cmd.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.8/rxd/cmd_app.py` & `rxd-0.0.9/rxd/cmd_app.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.8/rxd/cmd_responder.py` & `rxd-0.0.9/rxd/cmd_responder.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.8/rxd/codex.py` & `rxd-0.0.9/rxd/codex.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.8/setup.py` & `rxd-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='rxd',
-      version='0.0.8',
+      version='0.0.9',
       description='A reactive application manager',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Huy Nguyen',
       author_email='121183+huyng@users.noreply.github.com',
       packages=['rxd'],
       entry_points={
```

