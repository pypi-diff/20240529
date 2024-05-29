# Comparing `tmp/pgn_clis-0.1.3.tar.gz` & `tmp/pgn_clis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgn_clis-0.1.3.tar", last modified: Wed May 29 14:51:21 2024, max compression
+gzip compressed data, was "pgn_clis-0.1.4.tar", last modified: Wed May 29 15:25:28 2024, max compression
```

## Comparing `pgn_clis-0.1.3.tar` & `pgn_clis-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 14:51:21.510963 pgn_clis-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 14:51:21.510963 pgn_clis-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-05-29 07:07:00.000000 pgn_clis-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      813 2024-05-29 14:51:19.000000 pgn_clis-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 14:51:21.510963 pgn_clis-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 14:51:21.510963 pgn_clis-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 14:51:21.510963 pgn_clis-0.1.3/src/pgn_clis/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-29 07:07:00.000000 pgn_clis-0.1.3/src/pgn_clis/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 14:51:21.510963 pgn_clis-0.1.3/src/pgn_clis/lib/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:42.000000 pgn_clis-0.1.3/src/pgn_clis/lib/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 07:13:23.000000 pgn_clis-0.1.3/src/pgn_clis/lib/clean.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-05-29 09:00:48.000000 pgn_clis-0.1.3/src/pgn_clis/lib/download.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      988 2024-05-29 14:50:36.000000 pgn_clis-0.1.3/src/pgn_clis/lib/random_samples.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-05-29 07:53:22.000000 pgn_clis-0.1.3/src/pgn_clis/lib/sans2ucis.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-05-29 08:19:20.000000 pgn_clis-0.1.3/src/pgn_clis/lib/style_sans.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 14:51:21.510963 pgn_clis-0.1.3/src/pgn_clis/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:52.000000 pgn_clis-0.1.3/src/pgn_clis/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      243 2024-05-29 07:14:41.000000 pgn_clis-0.1.3/src/pgn_clis/scripts/clean.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-29 08:12:42.000000 pgn_clis-0.1.3/src/pgn_clis/scripts/download.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1417 2024-05-29 14:47:35.000000 pgn_clis-0.1.3/src/pgn_clis/scripts/random_samples.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-29 07:53:46.000000 pgn_clis-0.1.3/src/pgn_clis/scripts/sans2ucis.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      526 2024-05-29 08:19:54.000000 pgn_clis-0.1.3/src/pgn_clis/scripts/style_sans.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 14:51:21.510963 pgn_clis-0.1.3/src/pgn_clis.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 14:51:21.000000 pgn_clis-0.1.3/src/pgn_clis.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      651 2024-05-29 14:51:21.000000 pgn_clis-0.1.3/src/pgn_clis.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 14:51:21.000000 pgn_clis-0.1.3/src/pgn_clis.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-05-29 14:51:21.000000 pgn_clis-0.1.3/src/pgn_clis.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-29 14:51:21.000000 pgn_clis-0.1.3/src/pgn_clis.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-29 14:51:21.000000 pgn_clis-0.1.3/src/pgn_clis.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:25:28.439868 pgn_clis-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 15:25:28.439868 pgn_clis-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-05-29 07:07:00.000000 pgn_clis-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      813 2024-05-29 15:25:25.000000 pgn_clis-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 15:25:28.439868 pgn_clis-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:25:28.429868 pgn_clis-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:25:28.429868 pgn_clis-0.1.4/src/pgn_clis/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-29 07:07:00.000000 pgn_clis-0.1.4/src/pgn_clis/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:25:28.429868 pgn_clis-0.1.4/src/pgn_clis/lib/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:42.000000 pgn_clis-0.1.4/src/pgn_clis/lib/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 07:13:23.000000 pgn_clis-0.1.4/src/pgn_clis/lib/clean.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-05-29 09:00:48.000000 pgn_clis-0.1.4/src/pgn_clis/lib/download.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1444 2024-05-29 15:25:05.000000 pgn_clis-0.1.4/src/pgn_clis/lib/random_samples.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-05-29 07:53:22.000000 pgn_clis-0.1.4/src/pgn_clis/lib/sans2ucis.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-05-29 08:19:20.000000 pgn_clis-0.1.4/src/pgn_clis/lib/style_sans.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:25:28.439868 pgn_clis-0.1.4/src/pgn_clis/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:52.000000 pgn_clis-0.1.4/src/pgn_clis/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      243 2024-05-29 07:14:41.000000 pgn_clis-0.1.4/src/pgn_clis/scripts/clean.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-29 08:12:42.000000 pgn_clis-0.1.4/src/pgn_clis/scripts/download.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1611 2024-05-29 15:24:21.000000 pgn_clis-0.1.4/src/pgn_clis/scripts/random_samples.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-29 07:53:46.000000 pgn_clis-0.1.4/src/pgn_clis/scripts/sans2ucis.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      526 2024-05-29 08:19:54.000000 pgn_clis-0.1.4/src/pgn_clis/scripts/style_sans.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 15:25:28.439868 pgn_clis-0.1.4/src/pgn_clis.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 15:25:28.000000 pgn_clis-0.1.4/src/pgn_clis.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      651 2024-05-29 15:25:28.000000 pgn_clis-0.1.4/src/pgn_clis.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 15:25:28.000000 pgn_clis-0.1.4/src/pgn_clis.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-05-29 15:25:28.000000 pgn_clis-0.1.4/src/pgn_clis.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-29 15:25:28.000000 pgn_clis-0.1.4/src/pgn_clis.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-29 15:25:28.000000 pgn_clis-0.1.4/src/pgn_clis.egg-info/top_level.txt
```

### Comparing `pgn_clis-0.1.3/pyproject.toml` & `pgn_clis-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pgn-clis"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "package_description"
 dependencies = [
   "chess-utils", "chess-notation", "fs-tools"
 ]
```

### Comparing `pgn_clis-0.1.3/src/pgn_clis/lib/random_samples.py` & `pgn_clis-0.1.4/src/pgn_clis/lib/random_samples.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import Sequence, NamedTuple, Iterable, TextIO
+import os
+from multiprocessing import Pool
+import random
+from haskellian import iter as I
 from tqdm import tqdm
 import chess_utils as cu
 import chess
-import random
 
 class Sample(NamedTuple):
   inputs: Sequence[str]
   ucis: Sequence[str]
 
 def random_sample(max_len: int = 150, rng = random.Random()) -> Sample:
   board = chess.Board()
@@ -20,18 +23,25 @@
     san = board.san(move)
     board.push(move)
     inputs.append(san)
     ucis.append(move.uci())
 
   return Sample(inputs, ucis)
 
+def random_batch(num_samples: int, max_len: int = 150, rng = random.Random()) -> Sequence[Sample]:
+  return [random_sample(max_len, rng) for _ in range(num_samples)]
+
 def random_samples(
   inputs: TextIO, ucis: TextIO, *,
-  num_samples: int, max_len: int = 150,
-  seed: int | None = None, logstream: TextIO | None = None
+  num_samples: int, max_len: int = 150, chunk_size: int = 100,
+  seed: int | None = None, logstream: TextIO | None = None,
+  num_procs: int | None = None
 ):
+  num_procs = num_procs or os.cpu_count() or 1
   rng = random.Random(seed)
   iter = tqdm(range(num_samples), file=logstream, miniters=100) if logstream else range(num_samples)
-  for _ in iter:
-    sample = random_sample(max_len, rng)
-    print(' '.join(sample.inputs), file=inputs)
-    print(' '.join(sample.ucis), file=ucis)
+  with Pool() as pool:
+    for _ in I.batch(chunk_size, iter):
+      samples = pool.apply(random_batch, (chunk_size, max_len, rng))
+      for sample in samples:
+        print(' '.join(sample.inputs), file=inputs)
+        print(' '.join(sample.ucis), file=ucis)
```

### Comparing `pgn_clis-0.1.3/src/pgn_clis/scripts/random_samples.py` & `pgn_clis-0.1.4/src/pgn_clis/scripts/random_samples.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
   parser = ArgumentParser()
   parser.add_argument('-n', '--num-samples', type=int, default=int(1e6))
   parser.add_argument('-l', '--max-len', type=int, default=150)
   parser.add_argument('-s', '--seed', type=int, default=0)
   parser.add_argument('-v', '--verbose', action='store_true')
   parser.add_argument('-r', '--replace', action='store_true')
+  parser.add_argument('-c', '--chunk-size', type=int, default=100)
+  parser.add_argument('-p', '--num-procs', type=int, default=None)
 
   io_group = parser.add_mutually_exclusive_group(required=True)
   files_spec = io_group.add_argument_group()
   files_spec.add_argument('-i', '--inputs', type=str)
   files_spec.add_argument('-u', '--ucis', type=str)
 
   io_group.add_argument('-o', '--output', type=str)
@@ -37,9 +39,10 @@
   from pgn_clis.lib.random_samples import random_samples
 
   mode = 'w' if args.replace else 'x'
   with open(input_path, mode) as inputs_f, open(uci_path, mode) as ucis_f:
     random_samples(
       inputs_f, ucis_f,
       num_samples=args.num_samples, max_len=args.max_len,
+      chunk_size=args.chunk_size, num_procs=args.num_procs,
       seed=args.seed, logstream=sys.stderr if args.verbose else None
     )
```

### Comparing `pgn_clis-0.1.3/src/pgn_clis/scripts/sans2ucis.py` & `pgn_clis-0.1.4/src/pgn_clis/scripts/sans2ucis.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.3/src/pgn_clis/scripts/style_sans.py` & `pgn_clis-0.1.4/src/pgn_clis/scripts/style_sans.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.3/src/pgn_clis.egg-info/SOURCES.txt` & `pgn_clis-0.1.4/src/pgn_clis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

