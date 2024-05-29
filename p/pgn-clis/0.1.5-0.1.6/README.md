# Comparing `tmp/pgn_clis-0.1.5.tar.gz` & `tmp/pgn_clis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgn_clis-0.1.5.tar", last modified: Wed May 29 15:59:26 2024, max compression
+gzip compressed data, was "pgn_clis-0.1.6.tar", last modified: Wed May 29 16:01:40 2024, max compression
```

## Comparing `pgn_clis-0.1.5.tar` & `pgn_clis-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:59:26.233228 pgn_clis-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 15:59:26.233228 pgn_clis-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-05-29 07:07:00.000000 pgn_clis-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      813 2024-05-29 15:59:22.000000 pgn_clis-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 15:59:26.233228 pgn_clis-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:59:26.213228 pgn_clis-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:59:26.213228 pgn_clis-0.1.5/src/pgn_clis/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-29 07:07:00.000000 pgn_clis-0.1.5/src/pgn_clis/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:59:26.223228 pgn_clis-0.1.5/src/pgn_clis/lib/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:42.000000 pgn_clis-0.1.5/src/pgn_clis/lib/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 07:13:23.000000 pgn_clis-0.1.5/src/pgn_clis/lib/clean.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-05-29 09:00:48.000000 pgn_clis-0.1.5/src/pgn_clis/lib/download.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1939 2024-05-29 15:59:10.000000 pgn_clis-0.1.5/src/pgn_clis/lib/random_samples.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-05-29 07:53:22.000000 pgn_clis-0.1.5/src/pgn_clis/lib/sans2ucis.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-05-29 08:19:20.000000 pgn_clis-0.1.5/src/pgn_clis/lib/style_sans.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:59:26.223228 pgn_clis-0.1.5/src/pgn_clis/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:52.000000 pgn_clis-0.1.5/src/pgn_clis/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      243 2024-05-29 07:14:41.000000 pgn_clis-0.1.5/src/pgn_clis/scripts/clean.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-29 08:12:42.000000 pgn_clis-0.1.5/src/pgn_clis/scripts/download.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1510 2024-05-29 15:56:54.000000 pgn_clis-0.1.5/src/pgn_clis/scripts/random_samples.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-29 07:53:46.000000 pgn_clis-0.1.5/src/pgn_clis/scripts/sans2ucis.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      526 2024-05-29 08:19:54.000000 pgn_clis-0.1.5/src/pgn_clis/scripts/style_sans.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:59:26.233228 pgn_clis-0.1.5/src/pgn_clis.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 15:59:26.000000 pgn_clis-0.1.5/src/pgn_clis.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      651 2024-05-29 15:59:26.000000 pgn_clis-0.1.5/src/pgn_clis.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 15:59:26.000000 pgn_clis-0.1.5/src/pgn_clis.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-05-29 15:59:26.000000 pgn_clis-0.1.5/src/pgn_clis.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-29 15:59:26.000000 pgn_clis-0.1.5/src/pgn_clis.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-29 15:59:26.000000 pgn_clis-0.1.5/src/pgn_clis.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:01:40.404329 pgn_clis-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 16:01:40.404329 pgn_clis-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-05-29 07:07:00.000000 pgn_clis-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      813 2024-05-29 16:01:38.000000 pgn_clis-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 16:01:40.404329 pgn_clis-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:01:40.394329 pgn_clis-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:01:40.404329 pgn_clis-0.1.6/src/pgn_clis/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-29 07:07:00.000000 pgn_clis-0.1.6/src/pgn_clis/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:01:40.404329 pgn_clis-0.1.6/src/pgn_clis/lib/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:42.000000 pgn_clis-0.1.6/src/pgn_clis/lib/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 07:13:23.000000 pgn_clis-0.1.6/src/pgn_clis/lib/clean.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-05-29 09:00:48.000000 pgn_clis-0.1.6/src/pgn_clis/lib/download.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2197 2024-05-29 16:01:30.000000 pgn_clis-0.1.6/src/pgn_clis/lib/random_samples.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-05-29 07:53:22.000000 pgn_clis-0.1.6/src/pgn_clis/lib/sans2ucis.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-05-29 08:19:20.000000 pgn_clis-0.1.6/src/pgn_clis/lib/style_sans.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:01:40.404329 pgn_clis-0.1.6/src/pgn_clis/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:52.000000 pgn_clis-0.1.6/src/pgn_clis/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      243 2024-05-29 07:14:41.000000 pgn_clis-0.1.6/src/pgn_clis/scripts/clean.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-29 08:12:42.000000 pgn_clis-0.1.6/src/pgn_clis/scripts/download.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1402 2024-05-29 16:01:16.000000 pgn_clis-0.1.6/src/pgn_clis/scripts/random_samples.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-29 07:53:46.000000 pgn_clis-0.1.6/src/pgn_clis/scripts/sans2ucis.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      526 2024-05-29 08:19:54.000000 pgn_clis-0.1.6/src/pgn_clis/scripts/style_sans.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:01:40.404329 pgn_clis-0.1.6/src/pgn_clis.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 16:01:40.000000 pgn_clis-0.1.6/src/pgn_clis.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      651 2024-05-29 16:01:40.000000 pgn_clis-0.1.6/src/pgn_clis.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 16:01:40.000000 pgn_clis-0.1.6/src/pgn_clis.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-05-29 16:01:40.000000 pgn_clis-0.1.6/src/pgn_clis.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-29 16:01:40.000000 pgn_clis-0.1.6/src/pgn_clis.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-29 16:01:40.000000 pgn_clis-0.1.6/src/pgn_clis.egg-info/top_level.txt
```

### Comparing `pgn_clis-0.1.5/pyproject.toml` & `pgn_clis-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pgn-clis"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "package_description"
 dependencies = [
   "chess-utils", "chess-notation", "fs-tools"
 ]
```

### Comparing `pgn_clis-0.1.5/src/pgn_clis/lib/random_samples.py` & `pgn_clis-0.1.6/src/pgn_clis/lib/random_samples.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,21 @@
   num_samples: int, max_len: int = 150,
   seed: int | None = None, logstream: TextIO | None = None,
   num_procs: int | None = None
 ):
   num_procs = num_procs or os.cpu_count() or 1
   proc_samples = num_samples // num_procs
 
+  if logstream:
+    print(f'Generating {num_samples} samples...', file=logstream)
+    print(f'  max_len: {max_len}', file=logstream)
+    print(f'  num_procs: {num_procs}', file=logstream)
+    print(f'  seed: {seed or "random"}', file=logstream)
+    print()
+
   q = mp.Queue()
 
   def collector(
     inputs: TextIO, ucis: TextIO,
     *, queue: mp.Queue,
     logstream: TextIO | None = None
   ):
```

### Comparing `pgn_clis-0.1.5/src/pgn_clis/scripts/random_samples.py` & `pgn_clis-0.1.6/src/pgn_clis/scripts/random_samples.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from argparse import ArgumentParser
 
 def main():
 
   parser = ArgumentParser()
   parser.add_argument('-n', '--num-samples', type=int, default=int(1e6))
   parser.add_argument('-l', '--max-len', type=int, default=150)
-  parser.add_argument('-s', '--seed', type=int, default=0)
+  parser.add_argument('-s', '--seed', type=int, default=None)
   parser.add_argument('-v', '--verbose', action='store_true')
   parser.add_argument('-r', '--replace', action='store_true')
   parser.add_argument('-p', '--num-procs', type=int, default=None)
 
   io_group = parser.add_mutually_exclusive_group(required=True)
   files_spec = io_group.add_argument_group()
   files_spec.add_argument('-i', '--inputs', type=str)
@@ -25,19 +25,14 @@
     os.makedirs(args.output, exist_ok=True)
     input_path = os.path.join(args.output, 'inputs.txt')
     uci_path = os.path.join(args.output, 'ucis.txt')
   else:
     input_path = args.inputs
     uci_path = args.ucis
 
-  print(f'Generating samples...')
-  print(f'  inputs: {input_path}')
-  print(f'  ucis: {uci_path}')
-  print()
-
   import sys
   from pgn_clis.lib.random_samples import random_samples
 
   mode = 'w' if args.replace else 'x'
   with open(input_path, mode) as inputs_f, open(uci_path, mode) as ucis_f:
     random_samples(
       inputs_f, ucis_f,
```

### Comparing `pgn_clis-0.1.5/src/pgn_clis/scripts/sans2ucis.py` & `pgn_clis-0.1.6/src/pgn_clis/scripts/sans2ucis.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.5/src/pgn_clis/scripts/style_sans.py` & `pgn_clis-0.1.6/src/pgn_clis/scripts/style_sans.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.5/src/pgn_clis.egg-info/SOURCES.txt` & `pgn_clis-0.1.6/src/pgn_clis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

