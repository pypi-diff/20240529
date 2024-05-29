# Comparing `tmp/bpetokenizer-1.0.3.tar.gz` & `tmp/bpetokenizer-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpetokenizer-1.0.3.tar", last modified: Tue May 28 08:28:49 2024, max compression
+gzip compressed data, was "bpetokenizer-1.0.31.tar", last modified: Wed May 29 08:43:08 2024, max compression
```

## Comparing `bpetokenizer-1.0.3.tar` & `bpetokenizer-1.0.31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:28:49.072679 bpetokenizer-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-28 08:28:49.068679 bpetokenizer-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-28 08:28:45.000000 bpetokenizer-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:28:49.068679 bpetokenizer-1.0.3/bpetokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 08:28:45.000000 bpetokenizer-1.0.3/bpetokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-28 08:28:45.000000 bpetokenizer-1.0.3/bpetokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-28 08:28:45.000000 bpetokenizer-1.0.3/bpetokenizer/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 08:28:45.000000 bpetokenizer-1.0.3/bpetokenizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:28:49.068679 bpetokenizer-1.0.3/bpetokenizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-28 08:28:49.000000 bpetokenizer-1.0.3/bpetokenizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-28 08:28:49.000000 bpetokenizer-1.0.3/bpetokenizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:28:49.000000 bpetokenizer-1.0.3/bpetokenizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 08:28:49.000000 bpetokenizer-1.0.3/bpetokenizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 08:28:49.000000 bpetokenizer-1.0.3/bpetokenizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:28:49.072679 bpetokenizer-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-28 08:28:45.000000 bpetokenizer-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:28:49.068679 bpetokenizer-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-28 08:28:45.000000 bpetokenizer-1.0.3/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:43:08.843165 bpetokenizer-1.0.31/
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-29 08:43:08.843165 bpetokenizer-1.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-29 08:42:59.000000 bpetokenizer-1.0.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:43:08.843165 bpetokenizer-1.0.31/bpetokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 08:42:59.000000 bpetokenizer-1.0.31/bpetokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-05-29 08:42:59.000000 bpetokenizer-1.0.31/bpetokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-29 08:42:59.000000 bpetokenizer-1.0.31/bpetokenizer/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 08:42:59.000000 bpetokenizer-1.0.31/bpetokenizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:43:08.843165 bpetokenizer-1.0.31/bpetokenizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-29 08:43:08.000000 bpetokenizer-1.0.31/bpetokenizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-29 08:43:08.000000 bpetokenizer-1.0.31/bpetokenizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:43:08.000000 bpetokenizer-1.0.31/bpetokenizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 08:43:08.000000 bpetokenizer-1.0.31/bpetokenizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 08:43:08.000000 bpetokenizer-1.0.31/bpetokenizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:43:08.843165 bpetokenizer-1.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-29 08:42:59.000000 bpetokenizer-1.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:43:08.843165 bpetokenizer-1.0.31/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-29 08:42:59.000000 bpetokenizer-1.0.31/tests/test_tokenizer.py
```

### Comparing `bpetokenizer-1.0.3/PKG-INFO` & `bpetokenizer-1.0.31/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: bpetokenizer
-Version: 1.0.3
-Summary: Byte Pair Encoding Tokenizer with special tokens and regex pattern
-Home-page: https://github.com/Hk669/bpetokenizer
-Author: Hrushikesh Dokala
-Author-email: hrushi669@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9,<3.13
-Description-Content-Type: text/markdown
-Requires-Dist: regex
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
 # bpetokenizer
 
 A Byte Pair Encoding (BPE) tokenizer, which algorithmically follows along the GPT tokenizer. The tokenizer is capable of handling special tokens and uses a customizable regex pattern for tokenization(includes the gpt4 regex pattern). supports `save` and `load` tokenizers in the `json` and `file` format.
 
 
 ### Overview
 
@@ -124,16 +106,21 @@
 print('---')
 print(ids)
 
 decode_text = tokenizer.decode(ids)
 print('---')
 print(decode_text)
 
+# you can also print the tokens and the text chunks split with the pattern.
+tokens = tokenizer.tokens(encode_text, verbose=True) # if verbose, prints the text chunks and also the pattern used to split.
+print('---')
+print("tokens: ", tokens)
+
 ```
-refer to the [load_json_vocab](sample/load_json_vocab/) and run the `bpetokenizer_json` to get an overview of `vocab`, `merges`, `special_tokens`.
+refer to the [load_json_vocab](sample/load_json_vocab/) and run the `bpetokenizer_json` to get an overview of `vocab`, `merges`, `special_tokens` and to view the tokens that are split by the tokenizer using pattern, look at [tokens](sample/load_json_vocab/tokens.py)
 
 ### Run Tests
 
 the tests folder `tests/` include the tests of the tokenizer, uses pytest.
 
 ```
 python3 -m pytest
@@ -157,8 +144,8 @@
 
 ### License
 
 This project is licensed under the MIT License.
 
 ----
 
-*this tokenizer is inspired from the [minbpe](https://github.com/karpathy/minbpe), but more optimized.
+*this tokenizer is inspired from the [minbpe](https://github.com/karpathy/minbpe), but more optimized.
```

### Comparing `bpetokenizer-1.0.3/README.md` & `bpetokenizer-1.0.31/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: bpetokenizer
+Version: 1.0.31
+Summary: Byte Pair Encoding Tokenizer with special tokens and regex pattern
+Home-page: https://github.com/Hk669/bpetokenizer
+Author: Hrushikesh Dokala
+Author-email: hrushi669@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9,<3.13
+Description-Content-Type: text/markdown
+Requires-Dist: regex
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
 # bpetokenizer
 
 A Byte Pair Encoding (BPE) tokenizer, which algorithmically follows along the GPT tokenizer. The tokenizer is capable of handling special tokens and uses a customizable regex pattern for tokenization(includes the gpt4 regex pattern). supports `save` and `load` tokenizers in the `json` and `file` format.
 
 
 ### Overview
 
@@ -106,16 +124,21 @@
 print('---')
 print(ids)
 
 decode_text = tokenizer.decode(ids)
 print('---')
 print(decode_text)
 
+# you can also print the tokens and the text chunks split with the pattern.
+tokens = tokenizer.tokens(encode_text, verbose=True) # if verbose, prints the text chunks and also the pattern used to split.
+print('---')
+print("tokens: ", tokens)
+
 ```
-refer to the [load_json_vocab](sample/load_json_vocab/) and run the `bpetokenizer_json` to get an overview of `vocab`, `merges`, `special_tokens`.
+refer to the [load_json_vocab](sample/load_json_vocab/) and run the `bpetokenizer_json` to get an overview of `vocab`, `merges`, `special_tokens` and to view the tokens that are split by the tokenizer using pattern, look at [tokens](sample/load_json_vocab/tokens.py)
 
 ### Run Tests
 
 the tests folder `tests/` include the tests of the tokenizer, uses pytest.
 
 ```
 python3 -m pytest
@@ -139,8 +162,8 @@
 
 ### License
 
 This project is licensed under the MIT License.
 
 ----
 
-*this tokenizer is inspired from the [minbpe](https://github.com/karpathy/minbpe), but more optimized.
+*this tokenizer is inspired from the [minbpe](https://github.com/karpathy/minbpe), but more optimized.
```

### Comparing `bpetokenizer-1.0.3/bpetokenizer/base.py` & `bpetokenizer-1.0.31/bpetokenizer/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 This file will contains all the helper functions
 and Base class which has the methods to save/load model,
 also required to build the BPETokenizer.
 """
+
+import regex as re
 from .version import __version__
 
 def get_stats(tokens, counts=None) -> dict:
     """Get statistics of the tokens. Includes the frequency of each consecutive pair of tokens"""
     counts = {} if counts is None else counts
     for pair in zip(tokens, tokens[1:]):
         counts[pair] = counts.get(pair, 0) + 1
@@ -58,14 +60,15 @@
 
 class Tokenizer:
     """A Base class for the tokenizer, used for training and encoding/decoding the text without special tokens."""
 
     def __init__(self):
         self.merges = {}
         self.pattern = "" # the regex pattern
+        self.compiled_pattern = re.compile(self.pattern) if self.pattern else ""
         self.special_tokens = {}
         self.vocab = self._build_vocab() if self.merges else {}
 
     def _build_vocab(self) -> dict:
         """Build the vocab from the merges and special tokens. This will be used to encode/decode the tokens."""
         vocab = {idx: bytes([idx]) for idx in range(256)}
         for (p0, p1), idx in self.merges.items():
@@ -79,15 +82,15 @@
         """
         Writes metadata and vocabulary information to the model and vocab files.
         mode: str, default="file" | "json" to save the model and vocab in json format.
         """
         if mode == "file":
             model_file = file_name + ".model"
             with open(model_file, 'w') as f:
-                f.write("bpetokenizer v1.0.0\n")
+                f.write(f"{__version__}\n")
                 f.write(f"{self.pattern}\n")
                 f.write(f"{len(self.special_tokens)}\n")
                 if self.special_tokens:
                     for special, idx in self.special_tokens.items():
                         f.write(f"{special} {idx}\n")
 
                 for idx1, idx2 in self.merges: # this will give the tokens of pair which are merged
@@ -131,15 +134,15 @@
         """
         if mode == "file":
             assert file_name.endswith(".model")
             merges = {}
             special_tokens = {}
             idx = 256
             with open(file_name, 'r', encoding="utf-8") as f:
-                assert f.readline().strip() == "bpetokenizer v1.0.0"
+                assert f.readline().strip() == __version__
                 self.pattern = f.readline().strip().split()
                 num_special = int(f.readline().strip()) # no of lines of special_tokens
                 for _ in range(num_special):
                     special, idx = f.readline().strip().split()
                     special_tokens[special] = int(idx)
                 for line in f:
                     idx1, idx2 = map(int, line.strip().split())
@@ -152,15 +155,20 @@
 
         elif mode == "json":
             assert file_name.endswith(".json")
 
             import json
             with open(file_name, "r", encoding="utf-8") as f:
                 data = json.load(f)
-                self.pattern = data[r"pattern"]
+                assert data["version"] == __version__
+                pattern = data["pattern"]
+                pattern_regex = re.compile(r'regex.Regex\("(.+)", flags=(regex\.\w+)\)')
+                match = pattern_regex.match(pattern)
+                if match:
+                    self.pattern = match.group(1)
                 self.special_tokens = data["special_tokens"]
                 self.inverse_special_tokens = {v: k for k, v in self.special_tokens.items()}
                 merges = data["merges"]
                 self.merges = {tuple(map(int, k.strip('()').split(','))): v for k, v in merges.items()}
                 vocab = data["vocab"]
                 self.vocab = {int(k): v.encode("utf-8") for k, v in vocab.items()}
```

### Comparing `bpetokenizer-1.0.3/bpetokenizer/tokenizer.py` & `bpetokenizer-1.0.31/bpetokenizer/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,40 +22,41 @@
 
 
 class BPETokenizer(Tokenizer):
     """Byte Pair Encoding tokenizer. Which handles the special tokens and the pattern for tokenization."""
 
     def __init__(self, pattern=None, special_tokens=None):
         super().__init__()
-        self.pattern = re.compile(GPT4_SPLIT_PATTERN) if pattern is None else pattern
+        self.pattern = GPT4_SPLIT_PATTERN if pattern is None else pattern
+        self.compiled_pattern = re.compile(self.pattern)
         self.special_tokens = {} if special_tokens is None else special_tokens
         self.inverse_special_tokens = {} if special_tokens is None else {v: k for k, v in special_tokens.items()}
 
 
     def train(self, texts, vocab_size, verbose=False) -> None:
         """Train the tokenizer on the given texts and vocab size. The vocab size should be greater than 256."""
         assert vocab_size >= 256
         num_merges = vocab_size - 256
 
-        text_chunks = re.findall(self.pattern, texts) # handles the desired pattern of tokens with regex pattern
+        text_chunks = re.findall(self.compiled_pattern, texts) # handles the desired pattern of tokens with regex pattern
 
-        ids = [list(tokens.encode("utf-8")) for tokens in text_chunks]
+        ids = [list(tokens.encode("utf-8")) for tokens in text_chunks]      # List[List[int]]
         merges = {}
         vocab = {idx: bytes([idx]) for idx in range(256)} # vocab for first 255 bytes
 
         # bpe algorithm
         for i in range(num_merges):
             stats = {}
             for chunk in ids:
                 get_stats(chunk, stats)
 
             pair = max(stats, key=stats.get) # returns the highest frequency pair
             idx = 256 + i
 
-            ids = [merge(chunk_ids, pair, idx) for chunk_ids in ids]
+            ids = [merge(chunk_ids, pair, idx) for chunk_ids in ids] # merge all the max occuring pair in the each chunk in ids
             merges[pair] = idx
             vocab[idx] = vocab[pair[0]] + vocab[pair[1]] # concat of bytes
 
             if verbose:
                 print(f"merging {i+1}/{num_merges}: {pair} -> {idx} ({vocab[idx]}) had {stats[pair]} frequency")
 
         self.merges = merges
@@ -75,15 +76,15 @@
             # otherwise let's merge the best pair (lowest merge index)
             idx = self.merges[pair]
             ids = merge(ids, pair, idx)
         return ids
     
 
     def encode_ord(self, text) -> list:
-        text_chunks = re.findall(self.pattern, text)
+        text_chunks = re.findall(self.compiled_pattern, text)
         ids = []
         for chunk in text_chunks:
             _bytes = chunk.encode("utf-8")
             chunk_ids = self._encode(_bytes)
             ids.extend(chunk_ids)
         return ids
 
@@ -140,7 +141,20 @@
 
     def _special_tokens(self, special_tokens) -> None:
         """Set the special tokens for the tokenizer. If not passed when initializing, it will be empty."""
         self.special_tokens = special_tokens
         self.inverse_special_tokens = {v: k for k, v in special_tokens.items()}
     
 
+    def tokens(self, text, verbose=False) -> list:
+        text_chunks = re.findall(self.compiled_pattern, text)
+        
+        _tokens = []
+        for chunk in text_chunks:
+            _bytes = chunk.encode("utf-8")
+            chunk_ids = self._encode(_bytes)
+            chunk_tokens = [self.vocab[idx].decode("utf-8", errors="replace") if idx in self.vocab else f"[UNK{idx}]" for idx in chunk_ids]
+            _tokens.extend(chunk_tokens)
+        if verbose:
+            print(f"---\ntext chunks: {text_chunks}\n")
+            print(f"---\npattern: {self.pattern}\n")
+        return _tokens
```

### Comparing `bpetokenizer-1.0.3/bpetokenizer.egg-info/PKG-INFO` & `bpetokenizer-1.0.31/bpetokenizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpetokenizer
-Version: 1.0.3
+Version: 1.0.31
 Summary: Byte Pair Encoding Tokenizer with special tokens and regex pattern
 Home-page: https://github.com/Hk669/bpetokenizer
 Author: Hrushikesh Dokala
 Author-email: hrushi669@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -124,16 +124,21 @@
 print('---')
 print(ids)
 
 decode_text = tokenizer.decode(ids)
 print('---')
 print(decode_text)
 
+# you can also print the tokens and the text chunks split with the pattern.
+tokens = tokenizer.tokens(encode_text, verbose=True) # if verbose, prints the text chunks and also the pattern used to split.
+print('---')
+print("tokens: ", tokens)
+
 ```
-refer to the [load_json_vocab](sample/load_json_vocab/) and run the `bpetokenizer_json` to get an overview of `vocab`, `merges`, `special_tokens`.
+refer to the [load_json_vocab](sample/load_json_vocab/) and run the `bpetokenizer_json` to get an overview of `vocab`, `merges`, `special_tokens` and to view the tokens that are split by the tokenizer using pattern, look at [tokens](sample/load_json_vocab/tokens.py)
 
 ### Run Tests
 
 the tests folder `tests/` include the tests of the tokenizer, uses pytest.
 
 ```
 python3 -m pytest
```

### Comparing `bpetokenizer-1.0.3/setup.py` & `bpetokenizer-1.0.31/setup.py`

 * *Files identical despite different names*

### Comparing `bpetokenizer-1.0.3/tests/test_tokenizer.py` & `bpetokenizer-1.0.31/tests/test_tokenizer.py`

 * *Files identical despite different names*

