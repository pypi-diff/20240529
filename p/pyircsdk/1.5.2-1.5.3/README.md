# Comparing `tmp/pyircsdk-1.5.2.tar.gz` & `tmp/pyircsdk-1.5.3.tar.gz`

## Comparing `pyircsdk-1.5.2.tar` & `pyircsdk-1.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/__about__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/__init__.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/command.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/message.py
--rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/pyircsdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/event/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/event/event.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/__about__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/__init__.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/command.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/message.py
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/pyircsdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/event/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/event/event.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/PKG-INFO
```

### Comparing `pyircsdk-1.5.2/pyircsdk/command.py` & `pyircsdk-1.5.3/pyircsdk/command.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.2/pyircsdk/message.py` & `pyircsdk-1.5.3/pyircsdk/message.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.2/pyircsdk/pyircsdk.py` & `pyircsdk-1.5.3/pyircsdk/pyircsdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
                 # print('---')
 
                 # handle ping
                 if command == 'PING':
                     print('PING', trailing)
                     self.sendRaw('PONG ' + trailing + '\r\n')
                 # find End of /MOTD command
-                if command == '376':
+                if command == '376' or command == '422':
                     self.event.emit('connected', 'End of /MOTD command.')
 
                 # # find To connect type /QUOTE PONG
                 # if data.find('To connect type /QUOTE PONG') != -1:
                 #     print(data.split(':')[1])
                 #     self.sendRaw('QUOTE PONG ' + data.split(':')[1] + '\r\n')
```

### Comparing `pyircsdk-1.5.2/pyircsdk/event/event.py` & `pyircsdk-1.5.3/pyircsdk/event/event.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.2/.gitignore` & `pyircsdk-1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.2/LICENSE` & `pyircsdk-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.2/README.md` & `pyircsdk-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.2/pyproject.toml` & `pyircsdk-1.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pyircsdk"
 authors = [
   { name="Bludot", email="admin@floretos.com" },
 ]
-version = "1.5.2"
+version = "1.5.3"
 description = "pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyircsdk-1.5.2/PKG-INFO` & `pyircsdk-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyircsdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages.
 Project-URL: Homepage, https://github.com/bludot/pyircsdk
 Project-URL: Issues, https://github.com/bludot/pyircsdk/issues
 Author-email: Bludot <admin@floretos.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

