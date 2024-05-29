# Comparing `tmp/sourmash_plugin_pangenomics-0.1.tar.gz` & `tmp/sourmash_plugin_pangenomics-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_pangenomics-0.1.tar", last modified: Wed May 15 14:44:27 2024, max compression
+gzip compressed data, was "sourmash_plugin_pangenomics-0.2.tar", last modified: Wed May 29 16:14:21 2024, max compression
```

## Comparing `sourmash_plugin_pangenomics-0.1.tar` & `sourmash_plugin_pangenomics-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-15 14:44:27.902131 sourmash_plugin_pangenomics-0.1/
--rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-14 18:12:22.000000 sourmash_plugin_pangenomics-0.1/LICENSE
--rw-r--r--   0 t          (502) staff       (20)      986 2024-05-15 14:44:27.901941 sourmash_plugin_pangenomics-0.1/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      668 2024-05-14 18:27:01.000000 sourmash_plugin_pangenomics-0.1/README.md
--rw-r--r--   0 t          (502) staff       (20)      632 2024-05-15 14:43:30.000000 sourmash_plugin_pangenomics-0.1/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2024-05-15 14:44:27.902169 sourmash_plugin_pangenomics-0.1/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-15 14:44:27.900070 sourmash_plugin_pangenomics-0.1/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-15 14:44:27.901748 sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.egg-info/
--rw-r--r--   0 t          (502) staff       (20)      986 2024-05-15 14:44:27.000000 sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      429 2024-05-15 14:44:27.000000 sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2024-05-15 14:44:27.000000 sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)      216 2024-05-15 14:44:27.000000 sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       19 2024-05-15 14:44:27.000000 sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       28 2024-05-15 14:44:27.000000 sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)    19017 2024-05-15 14:39:31.000000 sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-15 14:44:27.901445 sourmash_plugin_pangenomics-0.1/tests/
--rw-r--r--   0 t          (502) staff       (20)      454 2024-05-14 18:27:01.000000 sourmash_plugin_pangenomics-0.1/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-29 16:14:21.209192 sourmash_plugin_pangenomics-0.2/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-14 18:12:22.000000 sourmash_plugin_pangenomics-0.2/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     4234 2024-05-29 16:14:21.208998 sourmash_plugin_pangenomics-0.2/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     3916 2024-05-29 16:07:59.000000 sourmash_plugin_pangenomics-0.2/README.md
+-rw-r--r--   0 t          (502) staff       (20)      692 2024-05-29 16:13:40.000000 sourmash_plugin_pangenomics-0.2/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2024-05-29 16:14:21.209225 sourmash_plugin_pangenomics-0.2/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-29 16:14:21.207320 sourmash_plugin_pangenomics-0.2/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-29 16:14:21.208796 sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     4234 2024-05-29 16:14:21.000000 sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      429 2024-05-29 16:14:21.000000 sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2024-05-29 16:14:21.000000 sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      274 2024-05-29 16:14:21.000000 sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       19 2024-05-29 16:14:21.000000 sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       28 2024-05-29 16:14:21.000000 sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)    19316 2024-05-29 16:07:59.000000 sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-29 16:14:21.208474 sourmash_plugin_pangenomics-0.2/tests/
+-rw-r--r--   0 t          (502) staff       (20)      454 2024-05-14 18:27:01.000000 sourmash_plugin_pangenomics-0.2/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_pangenomics-0.1/LICENSE` & `sourmash_plugin_pangenomics-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_pangenomics-0.1/pyproject.toml` & `sourmash_plugin_pangenomics-0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "sourmash_plugin_pangenomics"
 description = "sourmash plugin to do pangenomics."
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.1"
+version = "0.2"
 authors = [
   {name = "Colton Baumler", email = "ccbaumler@ucdavis.edu"},
   {name = "Titus Brown", email = "titus@idyll.org"},
 ]
 
 dependencies = ["sourmash>=4.8.8,<5"]
 
 [metadata]
 license = { text = "BSD 3-Clause License" }
 
 [project.entry-points."sourmash.cli_script"]
 createdb_command = "sourmash_plugin_pangenomics:Command_CreateDB"
+merge_command = "sourmash_plugin_pangenomics:Command_Merge"
 ranktable_command = "sourmash_plugin_pangenomics:Command_RankTable"
 classify_command = "sourmash_plugin_pangenomics:Command_Classify"
```

### Comparing `sourmash_plugin_pangenomics-0.1/src/sourmash_plugin_pangenomics.py` & `sourmash_plugin_pangenomics-0.2/src/sourmash_plugin_pangenomics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,120 +1,204 @@
 """pangenomics plugin"""
 
-epilog="""
+epilog = """
 See https://github.com/dib-lab/sourmash_plugin_pangenomics for more examples.
 
 Need help? Have questions? Ask at http://github.com/sourmash-bio/sourmash/issues!
 """
 
 import argparse
-import sourmash
+import sys
+from collections import Counter, defaultdict
+import csv
+import os
+import re
+import pprint
 
+import sourmash
+from sourmash import sourmash_args
+from sourmash.tax import tax_utils
 from sourmash.logging import debug_literal
 from sourmash.plugins import CommandLinePlugin
+from sourmash.save_load import SaveSignaturesToLocation
+
+
+CENTRAL_CORE = 1
+EXTERNAL_CORE = 2
+SHELL = 3
+INNER_CLOUD = 4
+SURFACE_CLOUD = 5
+
+NAMES = {
+    CENTRAL_CORE: "central core",
+    EXTERNAL_CORE: "external core",
+    SHELL: "shell",
+    INNER_CLOUD: "inner cloud",
+    SURFACE_CLOUD: "surface cloud",
+}
+
 
 ###
 
 #
 # CLI plugins - supports 'sourmash scripts <commands>'
 #
 
+
 class Command_CreateDB(CommandLinePlugin):
-    command = 'pangenomics_createdb'             # 'scripts <command>'
-    description = "@CTB"       # output with -h
-    usage = "@CTB"               # output with no args/bad args as well as -h
-    epilog = epilog             # output with -h
-    formatter_class = argparse.RawTextHelpFormatter # do not reformat multiline
+    command = "pangenome_createdb"  # 'scripts <command>'
+    description = "create a database of sketches merged at given rank"  # output with -h
+    usage = "pangenome_createdb <db> -t <lineagedb> -o <merged>.zip"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
 
     def __init__(self, subparser):
         super().__init__(subparser)
         p = subparser
 
         p.add_argument(
-            '-t', '--taxonomy-file', '--taxonomy', metavar='FILE',
-            action="extend", nargs='+', required=True,
-            help='database lineages file'
-        )
-        p.add_argument(
-            'sketches', nargs='+',
-            help='sketches to combine'
-        )
-        p.add_argument('--scaled', default=1000, type=int)
-        p.add_argument('-k', '--ksize', default=31, type=int)
-        p.add_argument('-m', '--moltype') # Use to assert that the moltype in the sketches == moltype use wants
-        p.add_argument('-o', '--output', required=True,
-                        help='Define a filename for the pangenome signatures (.zip preferred).')
-        p.add_argument('--csv', help='A CSV file generated to contain the lineage rank, genome name, hash count, and genome count.')
-        p.add_argument('-r', '--rank', default='species')
-        p.add_argument('-a', '--abund', action='store_true', help='Enable abundance tracking of hashes across rank selection.')
+            "-t",
+            "--taxonomy-file",
+            "--taxonomy",
+            metavar="FILE",
+            action="extend",
+            nargs="+",
+            required=True,
+            help="database lineages file",
+        )
+        p.add_argument("sketches", nargs="+", help="sketches to combine")
+        p.add_argument("--scaled", default=1000, type=int)
+        p.add_argument("-k", "--ksize", default=31, type=int)
+        p.add_argument(
+            "-m", "--moltype",
+            default="DNA"
+        )
+        p.add_argument(
+            "-o",
+            "--output",
+            required=True,
+            help="Define a filename for the pangenome signatures (.zip preferred).",
+        )
+        p.add_argument(
+            "--csv",
+            help="A CSV file generated to contain the lineage rank, genome name, hash count, and genome count.",
+        )
+        p.add_argument("-r", "--rank", default="species")
+        p.add_argument(
+            "-a",
+            "--abund",
+            action="store_true",
+            help="Enable abundance tracking of hashes across rank selection.",
+        )
 
     def main(self, args):
-        # code that we actually run.
         super().main(args)
-        return make_pangenome_sketches_main(args)
+        return pangenome_createdb_main(args)
+
+
+class Command_Merge(CommandLinePlugin):
+    command = "pangenome_merge"  # 'scripts <command>'
+    description = "merge sketches into a pangenome database a la createdb"  # output with -h
+    usage = "pangenome_merge <sketches> -o <merged>.zip"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
+
+    def __init__(self, subparser):
+        super().__init__(subparser)
+        p = subparser
+
+        p.add_argument("sketches", nargs="+", help="sketches to combine")
+        p.add_argument("--scaled", default=1000, type=int)
+        p.add_argument("-k", "--ksize", default=31, type=int)
+        p.add_argument(
+            "-m", "--moltype",
+            default="DNA"
+        )
+        p.add_argument(
+            "-o",
+            "--output",
+            required=True,
+            help="Define a filename for the pangenome signatures (.zip preferred).",
+        )
+
+    def main(self, args):
+        super().main(args)
+        return pangenome_merge_main(args)
 
 
 class Command_RankTable(CommandLinePlugin):
-    command = 'pangenomics_ranktable'             # 'scripts <command>'
-    description = "@CTB"       # output with -h
-    usage = "@CTB"               # output with no args/bad args as well as -h
-    epilog = epilog             # output with -h
-    formatter_class = argparse.RawTextHelpFormatter # do not reformat multiline
+    command = "pangenome_ranktable"  # 'scripts <command>'
+    description = "create a CSV ranktable that annotates hashes with pangenome characters"  # output with -h
+    usage = "pangenome_ranktable <merged.zip> -o <ranktable>.csv -l <lineage>"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
 
     def __init__(self, subparser):
         super().__init__(subparser)
         p = subparser
-        p.add_argument('data', metavar='SOURMASH_DATABASE', help='The sourmash dictionary created from `process_ss.py`')
-        p.add_argument('-k', '--ksize', type=int, default=31, help='The ksize of the sourmash pangenome database')
-        p.add_argument('-l', '--lineage', help='The specific lineage to extract from the sourmash pangenome database (e.g. "s__Escherichia coli")')
-        p.add_argument('-i', '--ignore-case', action='store_true', help='Ignore the casing of search terms')
-        p.add_argument('-o', '--output-hash-classification', required=False,
-                       help='CSV file containing classification of each hash')
+        p.add_argument(
+            "data",
+            metavar="SOURMASH_DATABASE",
+            help="The sourmash dictionary created from 'pangenome_creatdb --abund'",
+        )
+        p.add_argument(
+            "-k",
+            "--ksize",
+            type=int,
+            default=31,
+            help="The ksize of the sourmash pangenome database",
+        )
+        p.add_argument(
+            "-l",
+            "--lineage",
+            help='The specific lineage to extract from the sourmash pangenome database (e.g. "s__Escherichia coli")',
+        )
+        p.add_argument(
+            "-i",
+            "--ignore-case",
+            action="store_true",
+            help="Ignore the casing of search terms",
+        )
+        p.add_argument(
+            "-o",
+            "--output-hash-classification",
+            required=False,
+            help="CSV file containing classification of each hash",
+        )
 
     def main(self, args):
-        # code that we actually run.
         super().main(args)
-        print('RUNNING cmd', self, args)
-        return pangenome_elements_main(args)
+        return pangenome_ranktable_main(args)
 
 
 class Command_Classify(CommandLinePlugin):
-    command = 'pangenomics_classify'             # 'scripts <command>'
-    description = "@CTB"       # output with -h
-    usage = "@CTB"               # output with no args/bad args as well as -h
-    epilog = epilog             # output with -h
-    formatter_class = argparse.RawTextHelpFormatter # do not reformat multiline
+    command = "pangenome_classify"  # 'scripts <command>'
+    description = "classify the hashes in a sketch based on given ranktable characters"  # output with -h
+    usage = "pangenome_classify <sketch> <ranktable1> [<ranktable2> ...]"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
 
     def __init__(self, subparser):
         super().__init__(subparser)
         p = subparser
-        # add argparse arguments here.
-        debug_literal('RUNNING cmd_xyz.__init__')
-        p.add_argument('metagenome_sig')
-        p.add_argument('-k', '--ksize', default=31, help='k-mer size', type=int)
-        p.add_argument('classify_csv_files', nargs='+')
+        p.add_argument("metagenome_sig")
+        p.add_argument("-k", "--ksize", default=31, help="k-mer size", type=int)
+        p.add_argument("ranktable_csv_files", nargs="+",
+                       help="rank tables produced by pangenome_ranktable")
 
     def main(self, args):
-        # code that we actually run.
         super().main(args)
         return classify_hashes_main(args)
 
 
-### script make-pangenome-sketches.py
-
-import argparse
-import sys
-from collections import Counter, defaultdict
-import csv
-import os
-import sourmash
-from sourmash import sourmash_args
-from sourmash.tax import tax_utils
+#
+# pangenome_createdb
+#
 
-def make_pangenome_sketches_main(args):
+def pangenome_createdb_main(args):
     print(f"loading taxonomies from {args.taxonomy_file}")
     taxdb = sourmash.tax.tax_utils.MultiLineageDB.load(args.taxonomy_file)
     print(f"found {len(taxdb)} identifiers in taxdb.")
 
     ident_d = {}
     revtax_d = {}
     accum = defaultdict(dict)
@@ -124,51 +208,55 @@
         csv_file = check_csv(args.csv)
 
     # Load the database
     for filename in args.sketches:
         print(f"loading file {filename} as index => manifest")
         db = sourmash_args.load_file_as_index(filename)
         db = db.select(ksize=args.ksize)
+        # @CTB check moltype
         mf = db.manifest
         assert mf, "no matching sketches for given ksize!?"
 
-        if args.csv: chunk = []
+        if args.csv:
+            chunk = []
 
         # Work on a single signature at a time across the database
         for n, ss in enumerate(db.signatures()):
             if n and n % 1000 == 0:
-                print(f'...{n} - loading')
+                print(f"...{n} - loading")
 
             name = ss.name
             ident = tax_utils.get_ident(name)
 
             # grab relevant lineage name
             try:
                 lineage_tup = taxdb[ident]
-            except KeyError: # older versions of genbank are not named with version!
+            except KeyError:  # older versions of genbank are not named with version!
                 try:
-                    if '.' in ident:
-                        short_ident = ident.split('.')[0]
+                    if "." in ident:
+                        short_ident = ident.split(".")[0]
                         lineage_tup = taxdb[short_ident]
                     else:
-                        for i in range(1,10):
+                        for i in range(1, 10):
                             try:
                                 new_ident = f"{ident}.{i}"
                                 lineage_tup = taxdb[new_ident]
                                 break
                             except KeyError:
                                 continue
                 except:
                     print("Wow, that sucks!")
 
             lineage_tup = tax_utils.RankLineageInfo(lineage=lineage_tup)
             lineage_pair = lineage_tup.lineage_at_rank(args.rank)
             lineage_name = lineage_pair[-1].name
 
-            ident_d[lineage_name] = ident # pick an ident to represent this set of pangenome sketches
+            ident_d[lineage_name] = (
+                ident  # pick an ident to represent this set of pangenome sketches
+            )
 
             # Accumulate the count within lineage names if `--abund` in cli
             if args.abund:
                 c = Counter(ss.minhash.hashes)
                 if lineage_name in counts:
                     counts[lineage_name].update(c)
                 else:
@@ -185,80 +273,135 @@
 
             ## Add {name, hash_count} to a lineage key then
             ## create a simpler dict for writing the csv
             if args.csv:
                 # Accumulated counts of hashes in lineage by genome
                 hash_count = len(mh.hashes)
 
-                accum[lineage_name][name] = accum[lineage_name].get(name, 0) + hash_count
-                chunk.append({'lineage': lineage_name, 'sig_name': name, 'hash_count': hash_count, 'genome_count': n})
+                accum[lineage_name][name] = (
+                    accum[lineage_name].get(name, 0) + hash_count
+                )
+                chunk.append(
+                    {
+                        "lineage": lineage_name,
+                        "sig_name": name,
+                        "hash_count": hash_count,
+                        "genome_count": n,
+                    }
+                )
 
-            if args.csv and len(chunk) >= 1000: #args.chunk_size?
-                write_chunk(chunk, csv_file) #args.outputfilenameforcsv?
+            if args.csv and len(chunk) >= 1000:  # args.chunk_size?
+                write_chunk(chunk, csv_file)  # args.outputfilenameforcsv?
                 accum = defaultdict(dict)
                 chunk = []
 
         # Write remaining data
         if args.csv and len(chunk) > 0:
             write_chunk(chunk, csv_file)
             accum = defaultdict(dict)
             chunk = []
 
-   # save!
+    # save!
+    print(f"Writing output sketches to '{args.output}'")
     with sourmash_args.SaveSignaturesToLocation(args.output) as save_sigs:
         for n, (lineage_name, ident) in enumerate(ident_d.items()):
             if n and n % 1000 == 0:
-                print(f'...{n} - saving')
+                print(f"...{n} - saving")
 
-            sig_name = f'{ident} {lineage_name}'
+            sig_name = f"{ident} {lineage_name}"
 
             # retrieve merged MinHash
             mh = revtax_d[lineage_name]
 
             # Add abundance to signature if `--abund` in cli
             if args.abund:
                 abund_d = dict(counts[lineage_name])
 
                 abund_mh = mh.copy_and_clear()
                 abund_mh.track_abundance = True
                 abund_mh.set_abundances(abund_d)
 
-            # Create a signature with abundance only if `abund` in cli. Otherwise, create a 'flat' sig
-            ss = sourmash.SourmashSignature(abund_mh, name=sig_name) if args.abund else sourmash.SourmashSignature(mh, name=sig_name)
+                ss = sourmash.SourmashSignature(abund_mh, name=sig_name)
+            else:
+                ss = sourmash/SourmashSignature(mh, name=sig_name)
 
             save_sigs.add(ss)
 
+
 # Chunk function to limit the memory used by the hash_count dict and list
 def write_chunk(chunk, output_file):
-    with open(output_file, 'a', newline='') as csvfile:
-        fieldnames = ['lineage', 'sig_name', 'hash_count', 'genome_count']
+    with open(output_file, "a", newline="") as csvfile:
+        fieldnames = ["lineage", "sig_name", "hash_count", "genome_count"]
         writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
         writer.writerows(chunk)
 
+
+# @CTB do we need this?
 def check_csv(csv_file):
     if csv_file is None:
         return
 
     if os.path.exists(csv_file):
         raise argparse.ArgumentTypeError("\n%s already exists" % csv_file)
 
     count_csv = os.path.splitext(csv_file)[0] + ".csv"
     return count_csv
 
-### db_process function from script process_ss.py
 
-import sourmash
-from sourmash import sourmash_args
-import argparse
-import sys
-import os
-import re
+#
+# pangenome_merge
+#
+
+def pangenome_merge_main(args):
+    # Load the database
+    for filename in args.sketches:
+        print(f"loading file {filename} as index => manifest")
+        db = sourmash_args.load_file_as_index(filename)
+        db = db.select(ksize=args.ksize)
+        # @CTB check moltype
+        mf = db.manifest
+        assert mf, "no matching sketches for given ksize!?"
+
+        c = Counter()
+        mh = None
+
+        # work across the entire database
+        for n, ss in enumerate(db.signatures()):
+            if n and n % 1000 == 0:
+                print(f"...{n} - loading")
+
+            c.update(ss.minhash.hashes)
+
+            if mh is None:
+                mh = ss.minhash.to_mutable()
+            else:
+                mh += ss.minhash
+
+    # save!
+    print(f"Writing output sketches to '{args.output}'")
+
+    sig_name = "merged" # @CTB update with --name?
 
+    abund_mh = mh.copy_and_clear() # hmm, don't need mh tracked above?
+    abund_mh.track_abundance = True
+    abund_mh.set_abundances(dict(c))
+
+    with sourmash_args.SaveSignaturesToLocation(args.output) as save_sigs:
+        print(f"saving to '{args.output}'")
 
-def db_process(filename, ignore_case, invert_match, user_input, process_db, k=31, lineage_name='None'):
+        ss = sourmash.SourmashSignature(abund_mh, name=sig_name)
+        save_sigs.add(ss)
+
+
+def db_process(
+    filename,
+    ignore_case,
+    k=31,
+    lineage_name="None",
+):
     bname = os.path.basename(filename)
     ss_dict = {}
     print(f"\nloading file {bname} as index => manifest")
 
     db = sourmash_args.load_file_as_index(filename)
     db = db.select(ksize=k)
     mf = db.manifest
@@ -271,156 +414,84 @@
         # build the search pattern
         pattern = lineage_name
         if ignore_case:
             pattern = re.compile(pattern, re.IGNORECASE)
         else:
             pattern = re.compile(pattern)
 
-        if invert_match:
-
-            def search_pattern(vals):
-                return all(not pattern.search(val) for val in vals)
-        else:
-
-            def search_pattern(vals):
-                return any(pattern.search(val) for val in vals)
+        def search_pattern(vals):
+            return any(pattern.search(val) for val in vals)
 
         # find all matching rows.
-        sub_mf = mf.filter_on_columns(
-            search_pattern, ["name", "filename", "md5"]
-            )
-
+        sub_mf = mf.filter_on_columns(search_pattern, ["name", "filename", "md5"])
 
         selected_sigs = []
-        print(f'Found {len(sub_mf)} signatures in {bname}:')
+        print(f"Found {len(sub_mf)} signatures in {bname}:")
 
         for n, row in enumerate(sub_mf.rows, start=1):
             print(f'{n:<15} \033[0;31m{row.get("name")}\033[0m')
-            selected_sigs.append(row.get('name'))
-
-
-        if user_input:
-            while True:
-                user_input = input('\nSelect signatures to process (Comma-separated index value, "all", or "quit"): ')
-
-                if user_input.strip().lower() == 'quit' or user_input.strip().lower() == 'q':
-                    print("Exiting...")
-                    sys.exit(0)
-
-                if user_input.strip().lower() == 'all' or user_input.strip().lower() == 'a':
-                    break
-
-                else:
-                    try:
-                        #create a list of only digits no matter if letters or additional commas
-                        indices = [int(idx.strip()) for idx in user_input.split(',') if idx.strip().isdigit()]
-                        if not indices:
-                            raise ValueError("Invalid input string: Please enter a comma-separated integer list, 'all', or 'quit'.")
-
-                        outlier = [idx for idx in indices if not 1 <= idx <= len(selected_sigs)]
-
-                        if outlier:
-                            raise ValueError(f'Out of range integers: {", ".join([str(item) for item in outlier])}')
-
-                        indices = [n - 1 for n in indices]
-                        selected_names = [selected_sigs[n] for n in indices]
-
-                        def search_name(vals):
-                            return any(val in selected_names for val in vals)
-
-                        sub_mf = sub_mf.filter_on_columns(search_name, ["name"])
-
-                        break
-                    except Exception as e:
-                        print(f'{e}')
-                        continue
+            selected_sigs.append(row.get("name"))
 
         sub_picklist = sub_mf.to_picklist()
 
         try:
             db = db.select(picklist=sub_picklist)
         except ValueError:
             error("Chosen lineage name input not supported")
 
         for ss in db.signatures():
             name = ss.name
 
-            print(f'Found \033[0;31m{name}\033[0m in {bname}')
+            print(f"Found \033[0;31m{name}\033[0m in {bname}")
 
             mh = ss.minhash
             hashes = mh.hashes
             ss_dict[name] = hashes
 
         total_rows_examined = 0
         total_rows_examined += len(mf)
 
-        print(f"\nloaded {total_rows_examined} total that matched ksize & molecule type")
+        print(
+            f"\nloaded {total_rows_examined} total that matched ksize & molecule type"
+        )
 
         if ss_dict:
             print(f"extracted {len(ss_dict)} signatures from {len(db)} file(s)\n")
 
         else:
             print("no matching signatures found!\n")
             sys.exit(-1)
 
     else:
-        #process the entire database
-
-        if process_db:
-            for n, ss in enumerate(db.signatures()):
-
-                if n % 10 ==0:
-                    print(f'...Processing {n} of {len(mf)}', end='\r', flush=True)
-
-                    name = ss.name
+        # process the entire database
 
+        for n, ss in enumerate(db.signatures()):
+            if n % 10 == 0:
+                print(f"...Processing {n} of {len(mf)}", end="\r", flush=True)
 
-                    mh = ss.minhash
-                    hashes = mh.hashes
-                    ss_dict[name] = hashes
+                name = ss.name
 
-                print(f'...Processed {n} of {len(mf)} \n')
+                mh = ss.minhash
+                hashes = mh.hashes
+                ss_dict[name] = hashes
 
-        else:
-            print('\nDid you mean to use `-l/--lineage-name` to process specific signatures?')
-            print('Nothing to process. Exiting...\n')
-            sys.exit()
+            print(f"...Processed {n} of {len(mf)} \n")
 
     return ss_dict
 
 
-### script pangenome_elements.py
-
-import sys
-import argparse
-import csv
-
-
-CENTRAL_CORE=1
-EXTERNAL_CORE=2
-SHELL=3
-INNER_CLOUD=4
-SURFACE_CLOUD=5
-
-NAMES = { CENTRAL_CORE: 'central core',
-          EXTERNAL_CORE: 'external core',
-          SHELL: 'shell',
-          INNER_CLOUD: 'inner cloud',
-          SURFACE_CLOUD: 'surface cloud' }
-
-
 def pangenome_elements(data):
     # get the pangenome elements of the dicts for each rank pangenome
     for i, (key, nested_dict) in enumerate(data.items()):
         max_value = max(nested_dict.values())
 
-        central_core_threshold = 0.95 #0.95 is core , 90% is technically soft core
+        central_core_threshold = 0.95  # 0.95 is core , 90% is technically soft core
         external_core_threshold = 0.90
-        shell_threshold = 0.10 #0.10
-        inner_cloud_threshold = 0.01 # 0.0 is the full cloud, but trimming (0.001?) may be necessary to create the viz...?
+        shell_threshold = 0.10  # 0.10
+        inner_cloud_threshold = 0.01  # 0.0 is the full cloud, but trimming (0.001?) may be necessary to create the viz...?
         surface_cloud_threshold = 0.00
 
         central_core = []
         external_core = []
         shell = []
         inner_cloud = []
         surface_cloud = []
@@ -434,67 +505,71 @@
                 shell.append((nested_key, nested_value))
             elif nested_value >= max_value * inner_cloud_threshold:
                 inner_cloud.append((nested_key, nested_value))
             elif nested_value >= max_value * surface_cloud_threshold:
                 surface_cloud.append((nested_key, nested_value))
         return central_core, external_core, shell, inner_cloud, surface_cloud
 
-def pangenome_elements_main(args):
-    ss_dict = db_process(filename=args.data, k=args.ksize, lineage_name=args.lineage, ignore_case=args.ignore_case, invert_match=False, user_input=False, process_db=True)
-    results = pangenome_elements(data=ss_dict)
+#
+# pangenome_ranktable
+#
+
+def pangenome_ranktable_main(args):
+    ss_dict = db_process(
+        filename=args.data,
+        k=args.ksize,
+        lineage_name=args.lineage,
+        ignore_case=args.ignore_case,
+    )
+    results = pangenome_elements(ss_dict)
 
     if args.output_hash_classification:
-        print(f"Writing hash classification to CSV file '{args.output_hash_classification}'")
-        with open(args.output_hash_classification, 'w', newline='') as fp:
+        print(
+            f"Writing hash classification to CSV file '{args.output_hash_classification}'"
+        )
+        with open(args.output_hash_classification, "w", newline="") as fp:
             w = csv.writer(fp)
-            w.writerow(['hashval', 'pangenome_classification'])
+            w.writerow(["hashval", "pangenome_classification"])
             central_core, external_core, shell, inner_cloud, surface_cloud = results
 
             for xx, classify_code in (
-                    (central_core, CENTRAL_CORE),
-                    (external_core, EXTERNAL_CORE),
-                    (shell, SHELL),
-                    (inner_cloud, INNER_CLOUD),
-                    (surface_cloud, SURFACE_CLOUD)
-                    ):
+                (central_core, CENTRAL_CORE),
+                (external_core, EXTERNAL_CORE),
+                (shell, SHELL),
+                (inner_cloud, INNER_CLOUD),
+                (surface_cloud, SURFACE_CLOUD),
+            ):
                 for hashval, _ in xx:
                     w.writerow([hashval, classify_code])
 
 
-### script classify-hashes.py
-
-import sys
-import csv
-import argparse
-import sourmash
-from collections import defaultdict
-import pprint
-
-from sourmash.save_load import SaveSignaturesToLocation
+#
+# pangenome_classify
+#
 
 def classify_hashes_main(args):
     db = sourmash.load_file_as_index(args.metagenome_sig)
     db = db.select(ksize=args.ksize)
     sketches = list(db.signatures())
     assert len(sketches) == 1
     sketch = sketches[0]
     minhash = sketch.minhash
     hashes = minhash.hashes
 
     central_core_mh = minhash.copy_and_clear()
     shell_mh = minhash.copy_and_clear()
 
-    for csv_file in args.classify_csv_files:
-        with open(csv_file, 'r', newline='') as fp:
+    for csv_file in args.ranktable_csv_files:
+        with open(csv_file, "r", newline="") as fp:
             r = csv.DictReader(fp)
 
             classify_d = {}
             for row in r:
-                hashval = int(row['hashval'])
-                classify_as = int(row['pangenome_classification'])
+                hashval = int(row["hashval"])
+                classify_as = int(row["pangenome_classification"])
                 classify_d[hashval] = classify_as
 
         # now, classify_d has the classifications we care about. Let's
         # do terrible things to the sketch now.
 
         counter_d = defaultdict(int)
         total_classified = 0
@@ -503,25 +578,17 @@
             counter_d[classify] += 1
             if classify >= 0:
                 total_classified += 1
             if classify == CENTRAL_CORE:
                 central_core_mh.add_hash(hashval)
             elif classify == SHELL:
                 shell_mh.add_hash(hashval)
- 
 
         print(f"For '{csv_file}', signature '{sketch.name}' contains:")
         for int_id in sorted(NAMES):
             name = NAMES[int_id]
             count = counter_d.get(int_id, 0)
             percent = count / total_classified * 100
             print(f"\t {count} ({percent:.1f}%) hashes are classified as {name}")
 
         count = counter_d.get(-1, 0)
         print(f"\t ...and {count} hashes are NOT IN the csv file")
-
-        #core_ss = sourmash.SourmashSignature(central_core_mh, name='core')
-        #with SaveSignaturesToLocation('core.sig.gz') as save_sig:
-        #    save_sig.add(core_ss)
-        #shell_ss = sourmash.SourmashSignature(shell_mh, name='shell')
-        #with SaveSignaturesToLocation('shell.sig.gz') as save_sig:
-        #    save_sig.add(shell_ss)
```

