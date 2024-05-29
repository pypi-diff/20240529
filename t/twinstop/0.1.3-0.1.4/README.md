# Comparing `tmp/twinstop-0.1.3.tar.gz` & `tmp/twinstop-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinstop-0.1.3.tar", last modified: Wed May 22 09:27:45 2024, max compression
+gzip compressed data, was "twinstop-0.1.4.tar", last modified: Wed May 29 13:24:05 2024, max compression
```

## Comparing `twinstop-0.1.3.tar` & `twinstop-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.622280 twinstop-0.1.3/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.1.3/LICENSE
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     1800 2024-05-22 09:27:45.622280 twinstop-0.1.3/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      928 2024-05-22 09:20:18.000000 twinstop-0.1.3/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.1.3/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1054 2024-05-22 09:27:45.622280 twinstop-0.1.3/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.1.3/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.614280 twinstop-0.1.3/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.618280 twinstop-0.1.3/src/twinstop/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.1.3/src/twinstop/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2024-05-22 09:20:40.000000 twinstop-0.1.3/src/twinstop/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4218 2023-07-28 21:23:19.000000 twinstop-0.1.3/src/twinstop/block_selection.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.622280 twinstop-0.1.3/src/twinstop/data_files/
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.1.3/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.def.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.pre.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.sen.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.1.3/src/twinstop/data_files/scaler.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.bkp2.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   120533 2023-07-28 21:22:59.000000 twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.bkp3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   141246 2024-05-22 09:14:30.000000 twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6950 2023-07-28 21:23:28.000000 twinstop-0.1.3/src/twinstop/test_alignment_methods.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.622280 twinstop-0.1.3/src/twinstop.egg-info/
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     1800 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      740 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      206 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-29 13:24:05.230742 twinstop-0.1.4/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.1.4/LICENSE
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     1812 2024-05-29 13:24:05.230742 twinstop-0.1.4/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      928 2024-05-22 09:20:18.000000 twinstop-0.1.4/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.1.4/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1068 2024-05-29 13:24:05.230742 twinstop-0.1.4/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.1.4/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-29 13:24:05.226742 twinstop-0.1.4/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-29 13:24:05.226742 twinstop-0.1.4/src/twinstop/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.1.4/src/twinstop/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2024-05-24 14:30:00.000000 twinstop-0.1.4/src/twinstop/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4218 2023-07-28 21:23:19.000000 twinstop-0.1.4/src/twinstop/block_selection.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-29 13:24:05.230742 twinstop-0.1.4/src/twinstop/data_files/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.1.4/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.4/src/twinstop/data_files/logistic_regression_model.def.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.4/src/twinstop/data_files/logistic_regression_model.pre.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.1.4/src/twinstop/data_files/logistic_regression_model.sen.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.1.4/src/twinstop/data_files/scaler.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.1.4/src/twinstop/denovo_selenoproteins_h3.bkp2.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   120533 2023-07-28 21:22:59.000000 twinstop-0.1.4/src/twinstop/denovo_selenoproteins_h3.bkp3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   144372 2024-05-28 09:16:47.000000 twinstop-0.1.4/src/twinstop/denovo_selenoproteins_h3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     7124 2024-05-24 15:37:41.000000 twinstop-0.1.4/src/twinstop/test_alignment_methods.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-29 13:24:05.230742 twinstop-0.1.4/src/twinstop.egg-info/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     1812 2024-05-29 13:24:05.000000 twinstop-0.1.4/src/twinstop.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      740 2024-05-29 13:24:05.000000 twinstop-0.1.4/src/twinstop.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2024-05-29 13:24:05.000000 twinstop-0.1.4/src/twinstop.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      218 2024-05-29 13:24:05.000000 twinstop-0.1.4/src/twinstop.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2024-05-29 13:24:05.000000 twinstop-0.1.4/src/twinstop.egg-info/top_level.txt
```

### Comparing `twinstop-0.1.3/LICENSE` & `twinstop-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/PKG-INFO` & `twinstop-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.1.3
+Version: 0.1.4
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,20 +12,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython<=1.81,>=1.78
 Requires-Dist: easyterm>=1.0.0
 Requires-Dist: easybioinfo>=0.3.1
 Requires-Dist: orf_tools>=0.0.1
 Requires-Dist: file-chunk-iterators>=0.0.1
-Requires-Dist: pyranges>=0.0.120
-Requires-Dist: pandas>=1.3.5
+Requires-Dist: pyranges<1.0.0,>=0.1.2
+Requires-Dist: pandas<2.0.0,>=1.3.5
 Requires-Dist: pyfaidx>=0.7.2
 Requires-Dist: multiprocess>=0.70.14
 Requires-Dist: numpy>=1.21.5
-Requires-Dist: scikit-learn>=1.3.0
+Requires-Dist: scikit-learn==1.3.0
 
 # twinstop
 Twinstop identifies selenoproteins in close related transcriptomes
 
 # Installation
 In a new conda environment, run::
```

### Comparing `twinstop-0.1.3/README.md` & `twinstop-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/setup.cfg` & `twinstop-0.1.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 python_requires = >=3.7
 install_requires = 
 	biopython >= 1.78, <=1.81
 	easyterm >= 1.0.0
 	easybioinfo >= 0.3.1
 	orf_tools >= 0.0.1
 	file-chunk-iterators >= 0.0.1
-	pyranges >= 0.0.120
-	pandas >= 1.3.5
+	pyranges >= 0.1.2, <1.0.0
+	pandas >= 1.3.5, <2.0.0
 	pyfaidx >= 0.7.2
 	multiprocess >= 0.70.14
 	numpy >= 1.21.5
-	scikit-learn >= 1.3.0
+	scikit-learn == 1.3.0
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = data_files/*
```

### Comparing `twinstop-0.1.3/src/twinstop/block_selection.py` & `twinstop-0.1.4/src/twinstop/block_selection.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/src/twinstop/data_files/Matrix_BLOSUM62sel.txt` & `twinstop-0.1.4/src/twinstop/data_files/Matrix_BLOSUM62sel.txt`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.def.pkl` & `twinstop-0.1.4/src/twinstop/data_files/logistic_regression_model.def.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.pre.pkl` & `twinstop-0.1.4/src/twinstop/data_files/logistic_regression_model.pre.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.sen.pkl` & `twinstop-0.1.4/src/twinstop/data_files/logistic_regression_model.sen.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/src/twinstop/data_files/scaler.pkl` & `twinstop-0.1.4/src/twinstop/data_files/scaler.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.bkp2.py` & `twinstop-0.1.4/src/twinstop/denovo_selenoproteins_h3.bkp2.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.bkp3.py` & `twinstop-0.1.4/src/twinstop/denovo_selenoproteins_h3.bkp3.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.py` & `twinstop-0.1.4/src/twinstop/denovo_selenoproteins_h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 -q <str>   query file path: a transcriptome in fasta format
 -s <str>   subject file path: a nucleotide transcriptome in fasta format (run  makeblastdb beforehand)
 -o <str>   output folder path, where files generated by Twinstop will be saved
 
 ### Common optional arguments:
 #    Memory and CPU control
 -c <int>          nº of CPUs employed. Default: 1
--time_mem <bool>  prints time and memory usage throughout the pipeline. Defalt: False
+-time_mem <bool>  prints time and memory usage throughout the pipeline. Default: False
 
 #    Workflow
 -force <int>  controls the rerun of the phases of Twinstop. By default, it runs phases for which no output is detected.
               Provide a number, representing the phase from which Twinstop will start the rerun
               For information about phases, run:  twinstop -h phases
 
 #    Output: these switches control the optional output files written for candidates
@@ -37,14 +37,15 @@
 
 #    Optional phase 7, annotation of candidates:
 -ann <bool>    perform the annotation of candidates (Phase 7). Requires -ann_db
 -ann_db <str>  path to database (protein fasta) to annotate candidates; recommended: Uniref50.
                Note: makeblastdb must have been run on this file beforehand to use it
 
 ### Other options:
+-v         <bool>   verbose output for warnings
 -print_opt <bool>   print currently active options
 -h | --help <bool>  print this help and exit.
                     For a full list of options, run:   twinstop -h full"""
 )
 
 full_help = """### Advanced usage:
 # Twinstop can be very memory intensive, so it splits tables into chunks which are load and processed serially.
@@ -71,17 +72,15 @@
     5: "PAIRWISE ALIGNMENT",
     6: "UGA ALIGNMENT FILTER",
     7: "FINAL FILTER",
     8: "BLASTP FOR ANNOTATION",
     9: "OUTPUT",
 }
 
-colors = {"phase": "green",
-          "count": "magenta",
-          "bm": "yellow"}
+colors = {"phase": "green", "count": "magenta", "bm": "yellow"}
 
 
 def write_phase(n):
     write(f"\n### PHASE {n}: {titles_of_phases[n]}", how=colors["phase"])
 
 
 description_of_phases = {
@@ -130,14 +129,15 @@
 advanced_help_dict = {
     "phases": phases_help,
     "benchmark": benchmark_help,
     "full": full_help,
 }
 
 def_opt = {
+    "v": False,
     "q": "",
     "s": "",
     "o": "twinstop_out/",
     "c": 1,
     "par_fct": 1,
     "n_chunks": 10,
     "n_lines": 2500000,
@@ -171,35 +171,56 @@
 from sklearn.metrics import confusion_matrix
 import pickle
 import multiprocess as mp
 import numpy as np
 from datetime import datetime
 from Bio import pairwise2
 
-from easyterm import command_line_options, check_file_presence, write, CommandLineOptions
+from easyterm import (
+    command_line_options,
+    check_file_presence,
+    write,
+    CommandLineOptions,
+)
 from easybioinfo import count_coding_changes, count_coding_sites, translate
 from orf_tools import extend_orfs
 from file_chunk_iterators import (
     iterate_file_in_chunks,
     iterate_file_in_chunks_with_key,
     buf_count_newlines_gen,
 )
 
 # external scripts:
 from ._version import __version__
 from .block_selection import dictionary_seleno, score, block_dict
-from .test_alignment_methods import multiprocessing, mafft
+from .test_alignment_methods import multiprocessing, mafft, chunkify
+
+
+import warnings
+import traceback
+
+
+def custom_warning(message, category, filename, lineno, file=None, line=None):
+    log = f"{filename}:{lineno}: {category.__name__}: {message}\n"
+    log += "".join(traceback.format_stack()[:-1])
+    print(log)
+
+
+# fixing warning, future error
+# pd.DataFrame.swapaxes = pd.DataFrame.transpose
+
 
 # we create the dictionary of tuples with the scores of each aminoacid alignment with each other.
 # alignment score values are based on BLOSUM62 matrix. Scores for 'U' (selenocysteine) are added.
 blosum_matrix = dictionary_seleno()
 twinstop_libpath = os.path.dirname(os.path.realpath(__file__)) + "/data_files/"
 
 benchmark, debugging = False, False
 
+
 def run_tblastx(
     path_query_file, path_db_file, n_cpu, IsFormat6FileForced, tblastx_format_6_outfile
 ):
     """
     Runs tBLASTx in tabular 6 format with two nucleotide transcriptomes in fasta format.
     Output columns: subject transcript name (sacc), subject alignment start (sstart),
     subject alignment end (send), subject frame (sframe), query transcript name (qacc),
@@ -215,28 +236,27 @@
         Subject transcriptome path. It must be previously recognized by BLAST with 'makeblastdb'
     n_cpu : <int>, easyterm object opt['c']
         Number of CPUs used to run tBLASTx
     IsFormat6FileForced : <bool>,
         Decides if tBLASTx should be repeteated
     tblastx_format_6_outfile : <str>
         tBLASTx tabular format 6 output path
-
     Raises
     ------
     Exception
         We raise an exception to stop the program in case returncode is
         different that zero, indicating that subprocess.run has not run
         successfully.
         We also print the stdout and stderr to know more about the problem
     """
     # if not os.path.exists(tblastx_format_6_outfile) or IsFormat6FileForced:
     if True:
         # to avoid BLAST 'No such file or directory error', we make sure to build the subject
         # transcriptome as a BLAST db before running tBLASTx.
-            
+
         temp_tblastx_format_6_outfile = "temp_tblastx.tsv"
         # command to run tBLASTx format 6 table with specific columns
         format_6_cmd = (
             "tblastx -query "
             + path_query_file
             + " -db "
             + path_db_file
@@ -249,15 +269,15 @@
         # shlex.split converts the command into a list that can be run by subprocess.run
         format_6_cmd_list = shlex.split(format_6_cmd)
         y = subprocess.run(format_6_cmd_list, capture_output=True)
         # in case of an error an Exception will be raised
         if y.returncode != 0:
             write(y.stderr, y.stdout)
             raise Exception()
-        #write("Format 6 tBLASTx ran successfully")
+        # write("Format 6 tBLASTx ran successfully")
         # initial columns:
         colnames = [
             "ID",
             "Chromosome",
             "Start",
             "End",
             "Subj_fr",
@@ -276,15 +296,15 @@
         with open(tblastx_format_6_outfile, "w") as fw:
             fw.write("\t".join(colnames) + "\n")
             with open(temp_tblastx_format_6_outfile) as fr:
                 for index, line in enumerate(fr):
                     fw.write(str(index + 1) + "\t" + line)
         # removes temp tblastx file
         os.remove(temp_tblastx_format_6_outfile)
-        #write(f"tBLASTx output with header in {tblastx_format_6_outfile}")
+        # write(f"tBLASTx output with header in {tblastx_format_6_outfile}")
 
 
 def get_overlap_id(row):
     """
     Key function to keep all the same query/subject transcripts pair alignments in the same chunk during the
     overlapping/extend_orfs phases.
 
@@ -392,41 +412,41 @@
                 # lock = mp.Manager().Lock()
                 # shared_list = manager.list()
                 completed_results = []
 
                 # the following block is only for pairwise phase: do with python, or with mafft for alignments taking too long
                 if pairwise:
                     results = []
-                    for row in np.array_split(chunkdf, len(chunkdf)):
+                    for row in chunkify(chunkdf, len(chunkdf)):
                         result = pool.apply_async(func, args=(row,))
                         results.append(result)
                     for result in results:
                         try:
                             completed_results.append(result.get(timeout=timeout))
                         except mp.context.TimeoutError:
-                            write("A result took too long")
+                            # write("A result took too long")
                             pass
                     df_chunk = pd.concat(completed_results, axis=0, ignore_index=True)
                     if chunkdf.shape[0] != df_chunk.shape[0]:
-                        sel_for_mafft=~(chunkdf["ID"].isin(df_chunk["ID"]))
-                        write(f'WARNING {sel_for_mafft.sum()} alignments took too long with Bio python, now performing them with mafft ...')
+                        sel_for_mafft = ~(chunkdf["ID"].isin(df_chunk["ID"]))
+                        write(
+                            f"WARNING {sel_for_mafft.sum()} alignments took too long with Bio python, now performing them with mafft ..."
+                        )
                         mis_align = chunkdf[sel_for_mafft]
                         results = multiprocessing(mis_align, mafft, n_cpu, timeout)
                         df_chunk = pd.concat(
                             [df_chunk, results], axis=0, ignore_index=True
                         )
                 else:
                     # if len(chunkdf)/(n * n_cpu) < 2 and ext_orfs: # ext_orfs must have an input with at least 2 rows.
                     #     result = pool.map_async(func, iterable=np.array_split(chunkdf, len(chunkdf)//2 - 1))
                     # else:
                     result = pool.map_async(
                         func,
-                        iterable=np.array_split(
-                            chunkdf, min([len(chunkdf), n * n_cpu])
-                        ),
+                        iterable=chunkify(chunkdf, min([len(chunkdf), n * n_cpu])),
                     )
                     r = result.get(timeout=timeout)
                     completed_results.extend(r)
                     df_chunk = pd.concat(completed_results, axis=0, ignore_index=True)
 
             mode = "w" if chunkindex == 0 else "a"
             del chunkdf
@@ -474,15 +494,17 @@
                         # print(f'Df: {df.columns}')
                         filtered_out_overlapping = chunkdf[~(chunkdf.ID.isin(df.ID))]
                         # print(f'filtered_out_overlapping: {filtered_out_overlapping.columns}')
                         filtered_out_subset = filtered_out_overlapping[
                             ["Chromosome", "Q_ID", "Q_fr", "Score", "Subj_fr"]
                         ]
                         filtered_out_subset = filtered_out_subset.groupby(
-                            by=["Chromosome", "Q_ID", "Q_fr", "Subj_fr"], as_index=False
+                            by=["Chromosome", "Q_ID", "Q_fr", "Subj_fr"],
+                            as_index=False,
+                            observed=False,
                         ).sum()
                         filtered_out_subset.rename(
                             columns={"Score": "Tot_Score"}, inplace=True
                         )
                         filtered_out_overlapping = filtered_out_overlapping.merge(
                             filtered_out_subset,
                             on=["Chromosome", "Q_ID", "Q_fr", "Subj_fr"],
@@ -557,17 +579,15 @@
                 with mp.Pool(processes=n_cpu) as pool:
                     # lock = mp.Manager().Lock()
                     # shared_list = manager.list()
                     completed_results = []
 
                     result = pool.map_async(
                         func,
-                        iterable=np.array_split(
-                            chunkdf, min([len(chunkdf), n * n_cpu])
-                        ),
+                        iterable=chunkify(chunkdf, min([len(chunkdf), n * n_cpu])),
                     )
                     r = result.get(timeout=timeout)
                     completed_results.extend(r)
 
                     mode = "w" if chunkindex == 0 else "a"
                     # when Dataframe, 'path_or_buf' is the argument | if PyRanges, it is 'path'
                     del chunkdf
@@ -609,53 +629,55 @@
 
     query_df = extend_orfs(
         p=query_df,
         fasta_path=path_query_file,
         keep_off_bounds=True,
         starts=[],
         stops=["TAG", "TAA"],
-        chunk_size=1800
+        chunk_size=1800,
     )
     subj_df = extend_orfs(
         p=subj_df,
         fasta_path=path_subj_file,
         keep_off_bounds=True,
         starts=[],
         stops=["TAG", "TAA"],
-        chunk_size=1800
+        chunk_size=1800,
     )
     # we need to get the protein sequences for the extended sequences.
     query_df, subj_df = get_cds_prot_seq(
         subj_df, query_df, path_subj_file, path_query_file, CDS_sequences=True
     )
-    
+
     # renames the PyRanges-format query columns to merge both query/subj DataFrames.
     query_df = query_df.rename(
         columns={
             "Chromosome": "Q_ID",
             "Start": "Q_align_s",
             "End": "Q_align_e",
             "Strand": "Q_Strand",
         }
     )
     # merges both DataFrames by 'ID' column.
     joined_df = subj_df.merge(query_df.set_index(["ID"]), on="ID")
     # print(f'joined_df_1: {joined_df.columns}')
-    #print(f'joined_df_1:\n{joined_df}')
+    # print(f'joined_df_1:\n{joined_df}')
 
     ## removing identical extended ORFs
     joined_df.drop_duplicates(
         subset=["Chromosome", "Q_ID", "Start", "Q_align_s", "End", "Q_align_e"],
         ignore_index=True,
         keep="first",
         inplace=True,
     )
-    #selenoproteins = joined_df.apply(counting_selenos, axis=1)
-    selenoproteins = (joined_df.Subj_align_prot_seq.str.count('U') > 0 ) & (joined_df.Q_align_prot_seq.str.count('U') > 0 )
-    
+    # selenoproteins = joined_df.apply(counting_selenos, axis=1)
+    selenoproteins = (joined_df.Subj_align_prot_seq.str.count("U") > 0) & (
+        joined_df.Q_align_prot_seq.str.count("U") > 0
+    )
+
     joined_df = joined_df[selenoproteins]
     joined_df = joined_df.reindex(
         columns=[
             "ID",
             "Chromosome",
             "Start",
             "End",
@@ -671,15 +693,15 @@
             "Subj_CDS",
             "Query_CDS",
             "Subj_align_prot_seq",
             "Q_align_prot_seq",
         ]
     )
     # print(f'joined_df_2: {joined_df.columns}')
-    #print(f'joined_df_2:\n{joined_df}')
+    # print(f'joined_df_2:\n{joined_df}')
 
     return joined_df
 
 
 # def counting_selenos(row):
 #     """
 
@@ -793,15 +815,15 @@
         columns={"Q_ID": "Chromosome", "Q_align_s": "Start", "Q_align_e": "End"}
     )
     # write('Renaming Query columns in query df, PyRanges format')
     # query_df["Strand"] = query_df["Q_fr"].copy(deep=True)
     # # Strand column needs to have '+' or '-' only.
     # query_df["Strand"] = (query_df["Strand"] > 0).replace({True: "+", False: "-"})
     # write('Strand column created for query')
-    query_df['Strand'] = np.where( query_df["Q_fr"] > 0, '+', '-' )
+    query_df["Strand"] = np.where(query_df["Q_fr"] > 0, "+", "-")
 
     return query_df, subj_df
 
 
 def join_dfs(chunk_df, path_subj_file, path_query_file):
     """
     Rejoins query and subject DataFrames after obtaining the aligned query/subject protein sequences with
@@ -989,15 +1011,15 @@
     """
     # write(f'Overlapping')
     fragments_df_subset = fragments_df[
         ["Chromosome", "Subj_fr", "Q_ID", "Q_fr", "Score"]
     ]
     qsf_score = (
         fragments_df_subset.groupby(
-            by=["Chromosome", "Q_ID", "Q_fr", "Subj_fr"], as_index=False
+            by=["Chromosome", "Q_ID", "Q_fr", "Subj_fr"], as_index=False, observed=False
         )
         .sum()
         .sort_values("Score", ascending=False, ignore_index=True)
     )
     qsf_score.drop_duplicates(
         subset=["Chromosome"], inplace=True, ignore_index=True, keep="first"
     )
@@ -1010,15 +1032,15 @@
     # creates a 'Cluster' column identifying the overlapping sequences
     clusters_pr = pr.PyRanges(fragments_df).cluster(strand=False, slack=0, nb_cpu=n_cpu)
     del fragments_df
     clusters_df = clusters_pr.as_df()
     del clusters_pr
     clusters_df = (
         clusters_df.sort_values(by="Score", ascending=False)
-        .groupby("Cluster", as_index=False)
+        .groupby("Cluster", as_index=False, observed=False)
         .first()
     )
     clusters_df.drop("Cluster", axis=1, inplace=True)
     # clusters_df['Start'] = clusters_df['Start'] + 1
     # clusters_df['Q_align_s'] = clusters_df['Q_align_s'] + 1
     clusters_df = clusters_df.reindex(
         columns=[
@@ -1154,18 +1176,16 @@
     query_prot_seq : <str>
         Query aligned protein sequence.
     subj_prot_seq : <str>
         Subject aligned protein sequence.
 
     Returns
     -------
-    u_subj : <int>
-        Index of the 'U' responsible for read-through in the subject protein sequence.
-    u_query : <int>
-        Index of the 'U' responsible for read-through in the query protein sequence.
+    index_u
+        Index of the 'U' responsible for read-through in the aligned protein sequences
     """
 
     list_aligned_ugas = list()
     # center_alignment_subj = len(subj_prot_seq)/2
     center_alignment_q = len(query_prot_seq) / 2
 
     for idx, x in enumerate(subj_prot_seq):
@@ -1296,15 +1316,19 @@
             "Subj_align_prot_seq",
             "Q_align_prot_seq",
         ]
     )
     if debugging:
         filtered_out_candidates = pd.DataFrame()
     aligned_hits_df.reset_index(drop=True, inplace=True)
+    
     for i, row in aligned_hits_df.iterrows():
+        # print('\n'+'*'*200)
+        # print('q: '+row["Q_align_prot_seq"])
+        # print('s: '+row["Subj_align_prot_seq"])
         aligned = True
         # first, we need to select the U responsible for readthrough
         index_u = UGA(row["Q_align_prot_seq"], row["Subj_align_prot_seq"])
         # filters candidates with at least one aligned 'U'
         if not index_u is None:
             # counts the number of U's in both protein sequences
             n_stops_subj = row["Subj_align_prot_seq"].count("U")
@@ -1331,17 +1355,18 @@
                                 "-", ""
                             )
                         )
                         * 3
                     )
                     # print('U downstream query')
                     # print(f"row Q_align_prot_seq:\n {row['Q_align_prot_seq']}")
-                    row["Q_align_prot_seq"] = row["Q_align_prot_seq"][
-                        : list_down_query[0] + 1
-                    ] + "-" * (len(row["Q_align_prot_seq"]) - list_down_query[0] - 1)
+                    row["Q_align_prot_seq"] = (row["Q_align_prot_seq"][
+                        : list_down_query[0] # + 1 #MM
+                    ] + "*" + #MM
+                                               "-" * (len(row["Q_align_prot_seq"]) - list_down_query[0] - 1))
                     # print(f"row Q_align_prot_seq:\n {row['Q_align_prot_seq']}")
                     # print(f"row Query_CDS:\n {row['Query_CDS']}")
                     row["Query_CDS"] = row["Query_CDS"][
                         : (
                             list_down_query[0]
                             + 1
                             - row["Q_align_prot_seq"][: list_down_query[0] + 1].count(
@@ -1362,38 +1387,42 @@
                     ) * 3
                     # print('U upstream query')
                     # print(f"row Q_align_prot_seq:\n {row['Q_align_prot_seq']}")
                     gaps_up = row["Q_align_prot_seq"][: list_up_query[-1] + 1].count(
                         "-"
                     )
                     row["Q_align_prot_seq"] = (
-                        "-" * (list_up_query[-1] + 1)
-                        + row["Q_align_prot_seq"][list_up_query[-1] + 1 :]
+                        "-" * (list_up_query[-1]) #MM + 1)
+                        +'*' #MM
+                        + row["Q_align_prot_seq"][list_up_query[-1]+1:]
                     )
                     # print(f"row Q_align_prot_seq:\n {row['Q_align_prot_seq']}")
                     # print(f"row Query_CDS:\n {row['Query_CDS']}")
                     row["Query_CDS"] = row["Query_CDS"][
-                        (list_up_query[-1] + 1 - gaps_up) * 3 :
+                        (list_up_query[-1] # + 1 #MM
+                         - gaps_up) * 3 :
                     ]
                     # print(f"row Query_CDS:\n {row['Query_CDS']}")
+
                 if len(list_down_subj) != 0:
                     subj_cd = (
                         len(
                             row["Subj_align_prot_seq"][list_down_subj[0] + 1 :].replace(
                                 "-", ""
                             )
                         )
                         * 3
                     )
                     # print(f'subj_cd: {subj_cd}')
                     # print('U downstream subject')
                     # print(f"row Subj_align_prot_seq:\n {row['Subj_align_prot_seq']}")
-                    row["Subj_align_prot_seq"] = row["Subj_align_prot_seq"][
-                        : list_down_subj[0] + 1
-                    ] + "-" * (len(row["Subj_align_prot_seq"]) - list_down_subj[0] - 1)
+                    row["Subj_align_prot_seq"] = (row["Subj_align_prot_seq"][
+                        : list_down_subj[0] # + 1 #MM
+                    ] + '*'+  #MM
+                    "-" * (len(row["Subj_align_prot_seq"]) - list_down_subj[0] - 1))
                     # print(f"row Subj_align_prot_seq:\n {row['Subj_align_prot_seq']}")
                     # print(f"row Subj_CDS:\n {row['Subj_CDS']}")
                     row["Subj_CDS"] = row["Subj_CDS"][
                         : (
                             list_down_subj[0]
                             + 1
                             - row["Subj_align_prot_seq"][: list_down_subj[0] + 1].count(
@@ -1415,21 +1444,23 @@
                     # print(f'subj_cu: {subj_cu}')
                     # print('U upstream subject')
                     # print(f"row Subj_align_prot_seq:\n {row['Subj_align_prot_seq']}")
                     gaps_up = row["Subj_align_prot_seq"][: list_up_subj[-1] + 1].count(
                         "-"
                     )
                     row["Subj_align_prot_seq"] = (
-                        "-" * (list_up_subj[-1] + 1)
-                        + row["Subj_align_prot_seq"][list_up_subj[-1] + 1 :]
+                        "-" * (list_up_subj[-1]) #MM + 1)
+                        +'*' # MM
+                        + row["Subj_align_prot_seq"][list_up_subj[-1]+1:]
                     )
                     # print(f"row Subj_align_prot_seq:\n {row['Subj_align_prot_seq']}")
                     # print(f"row Subj_CDS:\n {row['Subj_CDS']}")
                     row["Subj_CDS"] = row["Subj_CDS"][
-                        (list_up_subj[-1] + 1 - gaps_up) * 3 :
+                        (list_up_subj[-1] #+ 1 #MM
+                         - gaps_up) * 3 :
                     ]
                     # print(f"row Subj_CDS:\n {row['Subj_CDS']}")
 
                 # updates the start/end positions according to strand value.
                 if len(list_up_subj) != 0:
                     # print('U upstream subject')
                     if row["Strand"] == "+":
@@ -1507,14 +1538,17 @@
                         # row['Q_align_s'] = (
                         #     row['Q_align_s'] +
                         #     len(row['Q_align_prot_seq'][list_down_query[0] + 1:].replace('-', '')))
                         # print(f"row Q_align_s:\n {row['Q_align_s']}")
 
                 prot_seq_query = ""
                 prot_seq_subj = ""
+                # print('\nafter processing\n')
+                # print('q: '+row["Q_align_prot_seq"])
+                # print('s: '+row["Subj_align_prot_seq"])
                 # deletes the non-sense gaps.
                 for idx, x in enumerate(row["Subj_align_prot_seq"]):
                     if x == "-" and row["Q_align_prot_seq"][idx] == "-":
                         continue
                     else:
                         prot_seq_query += row["Q_align_prot_seq"][idx]
                         prot_seq_subj += x
@@ -1555,15 +1589,16 @@
                 )
                 list_score.append(row["Score"])
                 # calculates the density score (score/length of the alignment).
                 density_score = round(row["Score"] / len(row["Q_align_prot_seq"]), 2)
                 list_density_score.append(density_score)
                 # using .iloc in this way, we take the entire row.
                 candidates = pd.concat(
-                    [candidates, aligned_hits_df.iloc[[i]]], ignore_index=True
+                    [i for i in [candidates, aligned_hits_df.iloc[[i]]] if not i.empty],
+                    ignore_index=True,
                 )
         else:
             if debugging:
                 aligned = False
                 reason = "No selenocysteine alignment in protein sequences"
         if not aligned:
             if debugging:
@@ -1617,15 +1652,15 @@
     # DataFrame is sorted by 'Density_Score' and saved.
     candidates.sort_values(by="Density_Score", inplace=True, ignore_index=True)
 
     return candidates
 
 
 def UGA_filter_each_row(row):
-    #write(row, how='green')
+    # write(row, how='green')
     aligned = True
     # first, we need to select the U responsible for readthrough
     index_u = UGA(row["Q_align_prot_seq"], row["Subj_align_prot_seq"])
     # filters candidates with at least one aligned 'U'
     if not index_u is None:
         # counts the number of U's in both protein sequences
         n_stops_subj = row["Subj_align_prot_seq"].count("U")
@@ -1635,17 +1670,15 @@
         if n_stops_subj >= 2 or n_stops_query >= 2:
             # then the others Us (if any) indexes are stored in four lists
             (
                 list_up_query,
                 list_down_query,
                 list_up_subj,
                 list_down_subj,
-            ) = list_UGAs(
-                row["Q_align_prot_seq"], row["Subj_align_prot_seq"], index_u
-            )
+            ) = list_UGAs(row["Q_align_prot_seq"], row["Subj_align_prot_seq"], index_u)
             # cuts protein/nucleotide sequences from the closest up/downstream U to the selected 'U'.
             # first, we cut downstream not to change the length of the sequences in case
             # we need to cut upstream too. Trimmed parts are replaced with gaps.
             if len(list_down_query) != 0:
                 query_cd = (
                     len(
                         row["Q_align_prot_seq"][list_down_query[0] + 1 :].replace(
@@ -1657,35 +1690,27 @@
                 row["Q_align_prot_seq"] = row["Q_align_prot_seq"][
                     : list_down_query[0] + 1
                 ] + "-" * (len(row["Q_align_prot_seq"]) - list_down_query[0] - 1)
                 row["Query_CDS"] = row["Query_CDS"][
                     : (
                         list_down_query[0]
                         + 1
-                        - row["Q_align_prot_seq"][: list_down_query[0] + 1].count(
-                            "-"
-                        )
+                        - row["Q_align_prot_seq"][: list_down_query[0] + 1].count("-")
                     )
                     * 3
                 ]
                 # print(f"row Query_CDS:\n {row['Query_CDS']}")
             if len(list_up_query) != 0:
                 query_cu = (
-                    len(
-                        row["Q_align_prot_seq"][: list_up_query[-1]].replace(
-                            "-", ""
-                        )
-                    )
+                    len(row["Q_align_prot_seq"][: list_up_query[-1]].replace("-", ""))
                     + 1
                 ) * 3
                 # print('U upstream query')
                 # print(f"row Q_align_prot_seq:\n {row['Q_align_prot_seq']}")
-                gaps_up = row["Q_align_prot_seq"][: list_up_query[-1] + 1].count(
-                    "-"
-                )
+                gaps_up = row["Q_align_prot_seq"][: list_up_query[-1] + 1].count("-")
                 row["Q_align_prot_seq"] = (
                     "-" * (list_up_query[-1] + 1)
                     + row["Q_align_prot_seq"][list_up_query[-1] + 1 :]
                 )
                 # print(f"row Q_align_prot_seq:\n {row['Q_align_prot_seq']}")
                 # print(f"row Query_CDS:\n {row['Query_CDS']}")
                 row["Query_CDS"] = row["Query_CDS"][
@@ -1709,33 +1734,25 @@
                 ] + "-" * (len(row["Subj_align_prot_seq"]) - list_down_subj[0] - 1)
                 # print(f"row Subj_align_prot_seq:\n {row['Subj_align_prot_seq']}")
                 # print(f"row Subj_CDS:\n {row['Subj_CDS']}")
                 row["Subj_CDS"] = row["Subj_CDS"][
                     : (
                         list_down_subj[0]
                         + 1
-                        - row["Subj_align_prot_seq"][: list_down_subj[0] + 1].count(
-                            "-"
-                        )
+                        - row["Subj_align_prot_seq"][: list_down_subj[0] + 1].count("-")
                     )
                     * 3
                 ]
                 # print(f"row Subj_CDS:\n {row['Subj_CDS']}")
             if len(list_up_subj) != 0:
                 subj_cu = (
-                    len(
-                        row["Subj_align_prot_seq"][: list_up_subj[-1]].replace(
-                            "-", ""
-                        )
-                    )
+                    len(row["Subj_align_prot_seq"][: list_up_subj[-1]].replace("-", ""))
                     + 1
                 ) * 3
-                gaps_up = row["Subj_align_prot_seq"][: list_up_subj[-1] + 1].count(
-                    "-"
-                )
+                gaps_up = row["Subj_align_prot_seq"][: list_up_subj[-1] + 1].count("-")
                 row["Subj_align_prot_seq"] = (
                     "-" * (list_up_subj[-1] + 1)
                     + row["Subj_align_prot_seq"][list_up_subj[-1] + 1 :]
                 )
                 row["Subj_CDS"] = row["Subj_CDS"][
                     (list_up_subj[-1] + 1 - gaps_up) * 3 :
                 ]
@@ -1788,26 +1805,26 @@
         index_3t_nucl_subj = (index_u - n_gaps_subj) * 3
         index_3t_nucl_query = (index_u - n_gaps_query) * 3
 
         # filters only when the selected 'U' = 'TGA'.
         if not (
             (row["Subj_CDS"][index_3t_nucl_subj : index_3t_nucl_subj + 3] == "TGA")
             and (
-                row["Query_CDS"][index_3t_nucl_query : index_3t_nucl_query + 3]
-                == "TGA"
+                row["Query_CDS"][index_3t_nucl_query : index_3t_nucl_query + 3] == "TGA"
             )
         ):
             raise SystemExit("Stop codon comparison did not match on:\n %s" % row)
     else:
         aligned = False
-    row['aligned']=aligned
+    row["aligned"] = aligned
     return row
 
+
 def UGA_filter(df):
-    """ MM modified
+    """MM modified
     Second filter of the script. During this filter, we will get only those hits
     with aligned selenocysteines (U) and minimum values of conservation upstream
     and downstream the in-frame-UGA.
     Alignments with more than one aligned 'U' are cut to keep only one per hit.
 
     Parameters
     ----------
@@ -1816,17 +1833,17 @@
 
     Returns
     -------
     None
         Modifies dataframe in place; also add column Aligned with boolean filter
     """
 
-    df['aligned']=False
-    edited_columns='Q_align_s Q_align_e Start End Q_align_prot_seq Subj_align_prot_seq Query_CDS Subj_CDS'.split()
-    df[edited_columns]=df.apply(UGA_filter_each_row, axis=1)[edited_columns]
+    df["aligned"] = False
+    edited_columns = "Q_align_s Q_align_e Start End Q_align_prot_seq Subj_align_prot_seq Query_CDS Subj_CDS".split()
+    df[edited_columns] = df.apply(UGA_filter_each_row, axis=1)[edited_columns]
     return df
 
     if debugging:
         pretty_out = pretty_output(filtered_out_candidates)
         with open("filtered_out_candidates.txt", "w") as fw:
             fw.write(pretty_out)
 
@@ -1866,15 +1883,14 @@
     )
     # DataFrame is sorted by 'Density_Score' and saved.
     candidates.sort_values(by="Density_Score", inplace=True, ignore_index=True)
 
     return candidates
 
 
-
 def find_sec_pos(row):
     # sec_annot_df = pd.DataFrame(columns=['ID', 'Chromosome', 'Start', 'End'])
     index_u = UGA(row["Q_align_prot_seq"], row["Subj_align_prot_seq"])
     if row["Strand"] == "+":
         sec_start = (
             index_u - row["Subj_align_prot_seq"][:index_u].count("-")
         ) * 3 + row["Start"]
@@ -1984,18 +2000,15 @@
 
     Returns
     -------
     u_dN_dS : <str>/<float>
         Non-synonymous/synonymous ratio upstream U.
     d_dN_dS : <str>/<float>
         Non-synonymous/synonymous ratio downstream U.
-    changes_dN_dS_u : <int>
-        Number of CDS mutations upstream U.
-    changes_dN_dS_d : <int>
-        Number of CDS mutations downstream U.
+
     """
 
     # before measuring dN/dS we need to have the cds sequences with the same
     # length, so we insert the gaps.
     (subj_aligned_cds, query_aligned_cds) = make_aligned_cds(
         row["Subj_CDS"],
         row["Query_CDS"],
@@ -2106,15 +2119,15 @@
     if x.returncode != 0:
         write(x.stderr, x.stdout)
         raise Exception()
 
     os.remove(fasta_query_prot_seq)
     # creates a table DataFrame and names the columns
     uniprot_IDs_df = pd.read_table(blastp_outfile, names=["Q_ID", "Annot_Title"])
-    uniprot_IDs_df = uniprot_IDs_df.groupby("Q_ID", as_index=False).agg(
+    uniprot_IDs_df = uniprot_IDs_df.groupby("Q_ID", as_index=False, observed=False).agg(
         {"Annot_Title": join_titles}
     )
     selenocandidates_df = selenocandidates_df.join(
         uniprot_IDs_df.set_index("Q_ID"), on="Q_ID"
     )
 
     os.remove(blastp_outfile)
@@ -2284,17 +2297,32 @@
 
 
 def pretty_output(df):
     pretty_outfile = ""
     for i, row in df.iterrows():
         pretty_outfile += "=" * 80 + "\n"
         comparison_string = ""
+        cds_string1, cds_string2, cds_string3 = "", "", ""
         Us_string = ""
+
+        (subj_aligned_cds, query_aligned_cds) = make_aligned_cds(
+            row["Subj_CDS"],
+            row["Query_CDS"],
+            row["Subj_align_prot_seq"],
+            row["Q_align_prot_seq"],
+        )
+
         # write(row)
         for index, x in enumerate(row["Q_align_prot_seq"]):
+
+            codon = subj_aligned_cds[index * 3 : index * 3 + 3]
+            cds_string1 += codon[0].lower()
+            cds_string2 += codon[1].lower()
+            cds_string3 += codon[2].lower()
+
             if x == "-" or row["Subj_align_prot_seq"][index] == "-":
                 comparison_string += " "
                 Us_string += " "
                 continue
             try:
                 if x == row["Subj_align_prot_seq"][index]:
                     comparison_string += x
@@ -2319,14 +2347,24 @@
             row["Q_align_prot_seq"][q : q + n]
             for q in range(0, len(comparison_string), n)
         ]
         subj_chunks = [
             row["Subj_align_prot_seq"][s : s + n]
             for s in range(0, len(comparison_string), n)
         ]
+        cds_string1_chunks = [
+            cds_string1[s : s + n] for s in range(0, len(comparison_string), n)
+        ]
+        cds_string2_chunks = [
+            cds_string2[s : s + n] for s in range(0, len(comparison_string), n)
+        ]
+        cds_string3_chunks = [
+            cds_string3[s : s + n] for s in range(0, len(comparison_string), n)
+        ]
+
         U_chunks = [Us_string[u : u + n] for u in range(0, len(comparison_string), n)]
 
         pretty_outfile += "\n"
         pretty_outfile += (
             f" ID = {row['ID']},  Score = {row['Score']},  Evalue = {row['Evalue']}\n"
         )
         if "Density_Score" in df:
@@ -2336,16 +2374,18 @@
         pretty_outfile += f" Subj_ID = {row['Chromosome']},  Query_ID = {row['Q_ID']}\n"
         if "Annot_Title" in df:
             pretty_outfile += f" Uniprot_ID = {row['Annot_Title']}\n"
         if "dN_dS_up" in df:
             pretty_outfile += (
                 f" udN/dS = {row['dN_dS_up']}, ddN/dS = {row['dN_dS_down']}\n"
             )
+        if "changes_dN_dS_u" in df:
+            pretty_outfile += f" uNSC + uSC = {row['changes_dN_dS_u']} , dNSC + dSC = {row['changes_dN_dS_down']}\n"
         if "Conservation_up" in df:
-            pretty_outfile += f" uNSC + uSC = {row['Conservation_up']} , dNSC + dSC = {row['Conservation_down']}\n"
+            pretty_outfile += f" Conservation up = {row['Conservation_up']} , Conservation down = {row['Conservation_down']}\n"
         if "Reason" in df:
             pretty_outfile += f" Reason to be filtered out : {row['Reason']}\n"
         # df_row = pd.DataFrame(row).transpose()
         # if 'Q_stop_codon' in df_row:
         #     pretty_outfile += f" Query stop codon : {row['Q_stop_codon']}, Subj stop codon : {row['Subj_stop_codon']}\n"
         pretty_outfile += "\n"
 
@@ -2380,15 +2420,18 @@
             else:
                 if row["Strand"] == "+":
                     pretty_outfile += f"Sbjct  {row['Start'] + n * idx * 3 + 1 - acumulated_gaps_subj * 3:<5d}  {subj_chunks[idx]}  {row['Start'] + (n * idx + len(subj_chunks[idx]) - gaps_subj) * 3:<5d}\n"
                 else:
                     pretty_outfile += f"Sbjct  {row['End'] - n * idx * 3 - 1 + acumulated_gaps_subj * 3:<5d}  {subj_chunks[idx]}  {row['End'] + (-1 * (n * idx + len(subj_chunks[idx])) + gaps_subj) * 3:<5d}\n"
                 acumulated_gaps_subj = gaps_subj
 
-            pretty_outfile += f"              {U_chunks[idx]}\n"
+            pretty_outfile += f"              {cds_string1_chunks[idx]}\n"
+            pretty_outfile += f"              {cds_string2_chunks[idx]}\n"
+            pretty_outfile += f"              {cds_string3_chunks[idx]}\n"
+            pretty_outfile += f"              {U_chunks[idx]}\n\n"
 
     return pretty_outfile
 
 
 def make_outputs(
     selenocandidates_df,
     IsQueryCDSeqReturned,
@@ -2399,15 +2442,15 @@
     path_pep_q,
     IsTargetProtSeqReturned,
     path_pep_t,
     IsQueryGFFileReturned,
     IsTargetGFFileReturned,
     path_query_gff,
     path_subj_gff,
-        output_folder
+    output_folder,
 ):
     """
     Function with the several optional script outfiles dependent on boolean
     values.
 
     Parameters
     ----------
@@ -2452,33 +2495,32 @@
 
     for i, row in selenocandidates_df.iterrows():
         # (subj_aligned_cds,
         #  query_aligned_cds) = make_aligned_cds(row['Subj_CDS'],
         #                                        row['Query_CDS'],
         #                                        row['Subj_align_prot_seq'],
         #                                        row['Q_align_prot_seq'])
-        prefix=row['Run_info']+',' if 'Run_info' in row else ''
+        prefix = row["Run_info"] + "," if "Run_info" in row else ""
+        title_q = f">{prefix}TwS.{row['ID']} {row['Q_ID']}[{row['Q_align_s']}:{row['Q_align_e']}] Annotation: {str(row['Annot_Title'])}\n" if "Annot_Title" in selenocandidates_df else f">{prefix}TwS.{row['ID']} {row['Q_ID']}[{row['Q_align_s']}:{row['Q_align_e']}]\n"
+        title_s = f">{prefix}TwS.{row['ID']} {row['Chromosome']}[{row['Start']}:{row['End']}] Annotation: {str(row['Annot_Title'])}\n" if "Annot_Title" in selenocandidates_df else f">{prefix}TwS.{row['ID']} {row['Chromosome']}[{row['Start']}:{row['End']}]\n"
+
         if IsQueryCDSeqReturned:
-            write("Annot_Title" in selenocandidates_df)
-            if "Annot_Title" in selenocandidates_df:
-                output_cds_q += f">{prefix}{row['Q_ID']}[{row['Q_align_s']}:{row['Q_align_e']}],{row['ID']},{str(row['Annot_Title']).replace(' ', '_').replace(',', '.')}\n"
-            else:
-                output_cds_q += f">{prefix}{row['Q_ID']}[{row['Q_align_s']}:{row['Q_align_e']}],{row['ID']}\n"
+            output_cds_q += title_q
             output_cds_q += f"{row['Query_CDS']}\n"
+
         if IsTargetCDSeqReturned:
-            output_cds_t += f">{prefix}{row['Chromosome']}[{row['Start']}:{row['End']}],{row['ID']}\n"
+            output_cds_t += title_s
             output_cds_t += f"{row['Subj_CDS']}\n"
+
         if IsQueryProtSeqReturned:
-            if "Annot_Title" in selenocandidates_df:
-                output_pep_q += f">{prefix}{row['Q_ID']}[{row['Q_align_s']}:{row['Q_align_e']}],{row['ID']},{str(row['Annot_Title']).replace(' ', '_').replace(',', '.')}\n"
-            else:
-                output_pep_q += f">{prefix}{row['Q_ID']}[{row['Q_align_s']}:{row['Q_align_e']}],{row['ID']}\n"
+            output_pep_q += title_q
             output_pep_q += f"{row['Q_align_prot_seq'].replace('-', '')}\n"
+
         if IsTargetProtSeqReturned:
-            output_pep_t += f">{prefix}{row['Chromosome']}[{row['Start']}:{row['End']}],{row['ID']}\n"
+            output_pep_t += title_s
             output_pep_t += f"{row['Subj_align_prot_seq'].replace('-', '')}\n"
 
     if IsQueryCDSeqReturned:
         write(f"> Output: fasta of query CDSs  --> {output_folder+'/'+path_cds_q}")
         with open(path_cds_q, "w") as fw:
             fw.write(output_cds_q)
     if IsTargetCDSeqReturned:
@@ -2493,14 +2535,15 @@
         write(f"> Output: fasta of subject proteins --> {output_folder+'/'+path_pep_t}")
         with open(path_pep_t, "w") as fw:
             fw.write(output_pep_t)
 
     # if IsCandidatesDotplotReturned:
     #     dot_plot(selenocandidates_df, path_dotplot)
 
+    selenocandidates_df["ID"] = selenocandidates_df["ID"].astype(str)
     selenocandidates_df.rename(columns={"ID": "Gene_ID"}, inplace=True)
     selenocandidates_df["Feature"] = "CDS"
     selenocandidates_df["Source"] = "Twinstop"
 
     if IsQueryGFFileReturned:
         query_df = selenocandidates_df.copy()
         query_df.drop(["Chromosome", "Start", "End", "Strand"], axis=1, inplace=True)
@@ -2599,15 +2642,15 @@
         )
         candidates["dN_dS_down"] = candidates["dN_dS_down"].where(
             candidates["dN_dS_down"] <= maxdnds, maxdnds
         )
         # print(candidates['dN_dS_up'].isnull().values.any())
         # print(candidates['dN_dS_down'].isnull().values.any())
 
-    test_ml = candidates[
+    test_ml = candidates.copy()[
         [
             "Density_Score",
             "Conservation_up",
             "Conservation_down",
             "dN_dS_up",
             "dN_dS_down",
             "sec_start",
@@ -2656,17 +2699,17 @@
             "K": "positive",
             "U": "stop",
             "*": "stop",
             "Z": "outofbounds",
         }
     )
 
-    test_ml[
-        ["U+1", "U+2", "U+3", "U+4", "U+5", "U-1", "U-2", "U-3", "U-4", "U-5"]
-    ] = replaced_col
+    test_ml[["U+1", "U+2", "U+3", "U+4", "U+5", "U-1", "U-2", "U-3", "U-4", "U-5"]] = (
+        replaced_col
+    )
     # test_ml.rename(columns={'dN_dS_up': 'dN/dS_up', 'dN_dS_down': 'dN/dS_down'}, inplace=True)
 
     # X = test_ml.drop(['true_positive'], axis=1)
     X = pd.get_dummies(
         test_ml,
         columns=["U+1", "U+2", "U+3", "U+4", "U+5", "U-1", "U-2", "U-3", "U-4", "U-5"],
         dtype="int",
@@ -2708,29 +2751,27 @@
     with open(lr_filepath, "rb") as file:
         lr = pickle.load(file)
 
     lr.n_jobs = ncpus
 
     return lr.predict(X_stand), y
 
+
 def final_benchmark(candidates_df, sp4_subj_gff):
-    true_positives = candidates_df[
-        ["ID", "Chromosome", "sec_start", "sec_end"]
-    ].merge(
+    true_positives = candidates_df[["ID", "Chromosome", "sec_start", "sec_end"]].merge(
         sp4_subj_gff[["Chromosome", "sec_start", "sec_end"]],
         on=["Chromosome", "sec_start", "sec_end"],
         how="inner",
     )
     # true_positives = true_positives[true_positives.sec_start_ts.eq(true_positives.sec_start_sp4)]
     # print(candidates_df.dtypes)
     # print(candidates_df['sec_start_ts'] == candidates_df['sec_start_sp4'])
     # print(true_positive)
     candidates_df["true_positive"] = candidates_df.ID.isin(true_positives.ID)
     return candidates_df
-    
 
 
 def preprocessing_candidates(candidates_df, q_file, subj_file):
     # abbreviations = dict(
     #     {
     #         "Chlorella_sorokiniana_nt": "Cs",
     #         "Chlamydomonas_acidophila_nt": "Ca",
@@ -2961,19 +3002,21 @@
 
     write(
         f' TwinStop v{__version__} | Date: {datetime.now().strftime("%Y-%m-%d %H:%M:%S")} '.center(
             70, "*"
         )
     )
 
-    write(' arguments and options provided: '.center(70, '_'))
-    write(CommandLineOptions({k:opt[k] for k in def_opt if def_opt[k] != opt[k]}))
-    write('_'*70)
-          
-    
+    write(" arguments and options provided: ".center(70, "_"))
+    write(CommandLineOptions({k: opt[k] for k in def_opt if def_opt[k] != opt[k]}))
+    write("_" * 70)
+
+    if opt["v"]:
+        warnings.showwarning = custom_warning
+
     # most used opt options are saved in variables
     n_cpu = opt["c"]
     n_chunks = opt["n_chunks"]
     n_lines = opt["n_lines"]
     n = opt["par_fct"]
     n_section = opt["force"]
     time_memory_control = opt["time_mem"]
@@ -3028,15 +3071,15 @@
         ]
         if selenos_annot.shape[0] != sp4_prediction_subj.shape[0]:
             unpresent_sel = sp4_prediction_subj[
                 ~sp4_prediction_subj.Sel_family.isin(sp4_prediction_query.Sel_family)
             ]
             write(
                 f"For benchmark, omitting selenoprotein families not present in query: {len(unpresent_sel)} belonging to families {' '.join(unpresent_sel.Sel_family.drop_duplicates())}",
-                how=colors['bm']
+                how=colors["bm"],
             )
         # deletes a Python variable (empthy memory)
         del sp4_prediction_subj, sp4_prediction_query
 
         # # I want to get rid of the selenoprotein families which are unreachable for this script (terminal selenocysteines)
         # unavailable_Sel_families = opt["unavailable_families"]
         # # keeps the rest of selenos
@@ -3047,41 +3090,40 @@
         #     unavailable_sel = selenos_annot[
         #         selenos_annot.Sel_family.isin(unavailable_Sel_families)
         #     ]
         #     write(
         #         f"Unavailable Selenoprotein families predicted by Selenoprofiles 4:\n\n{unavailable_sel}"
         #     )
         available_selenos = selenos_annot.copy()
-        write(f'Subject selenoproteins for benchmark: {len(available_selenos)} belonging to families {" ".join(available_selenos.Sel_family.drop_duplicates())}',
-              how=colors['bm'])
+        write(
+            f'Subject selenoproteins for benchmark: {len(available_selenos)} belonging to families {" ".join(available_selenos.Sel_family.drop_duplicates())}',
+            how=colors["bm"],
+        )
         del selenos_annot
 
     # os.chdir(path) allows to change directory in python. We work from the output folder
     os.chdir(output_folder)
 
-
-        
     # write('\n### PHASE 0: TBLASTX', how=colors['phase'])
     write_phase(0)
 
     # first phase of the script is to run a tblastx between the query and subject transcriptomes to get the best
     # alignments among the transcripts.
     if not os.path.exists(path_tblastx_outfile) or n_section == 0:
-
-        if not os.path.exists(subj_file+'.nin'):
-            write('The subject file is not formatted for blast! Running makeblastdb')
+        if not os.path.exists(subj_file + ".nin"):
+            write("The subject file is not formatted for blast! Running makeblastdb")
             cmd_makeblastdb = "makeblastdb -in " + subj_file + " -dbtype nucl"
             cmd_makeblastdb_list = shlex.split(cmd_makeblastdb)
             # subprocess.run allows to execute external programs inside a Python code
             y = subprocess.run(cmd_makeblastdb_list, capture_output=True)
             # controls that the subject transcriptome is nucleotide dtype, else raises Exception
             if y.returncode != 0:
                 write(y.stderr, y.stdout)
                 raise Exception()
-        
+
         write(description_of_phases[0])
         run_tblastx(
             q_file,
             subj_file,
             n_cpu,
             True,  # n_section==0,
             path_tblastx_outfile + ".tmp",
@@ -3097,27 +3139,29 @@
         path_tblastx_outfile,
         usecols=["Chromosome"],
         sep="\t",
         header=0,
         index_col=False,
     )["Chromosome"]
     # write(f'Nº of tBLASTx hits: {buf_count_newlines_gen(path_tblastx_outfile)}', how=colors['count'])
-    write(f"= After tBLASTx, Nº of hits: {len(trans_candidates):,.0f}", how=colors['count'])
+    write(
+        f"= After tBLASTx, Nº of hits: {len(trans_candidates):,.0f}",
+        how=colors["count"],
+    )
     write(
         f"= After tBLASTx, Nº of unique subject transcripts: {len(trans_candidates.unique()):,.0f}",
-        how=colors['count'],
+        how=colors["count"],
     )
 
     if benchmark:
-        num=available_selenos.Transcript.isin(trans_candidates).sum()
-        denom=len(available_selenos)
+        num = available_selenos.Transcript.isin(trans_candidates).sum()
+        denom = len(available_selenos)
         # and we check how many expected selenoprotein transcripts have successfully passed the filter
         write(
-            f"% Benchmark TP: {num}/{denom}  Recall={num/denom:.2%}",
-            how=colors['bm']
+            f"% Benchmark TP: {num}/{denom}  Recall={num/denom:.2%}", how=colors["bm"]
         )
     del trans_candidates
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
@@ -3138,15 +3182,17 @@
             mp_join_dfs,
             n_cpu,
             None,
             path_postchunking_outfile + ".tmp",
             n,
         )
         os.rename(path_postchunking_outfile + ".tmp", path_postchunking_outfile)
-        write(f"> Table including sequences created --> {output_folder+'/'+path_postchunking_outfile}")
+        write(
+            f"> Table including sequences created --> {output_folder+'/'+path_postchunking_outfile}"
+        )
 
     else:
         write(f"File found: {path_postchunking_outfile}")
 
     # using time_memory_control==True we can know the time and memory (current and peak) in each phase
     if time_memory_control:
         time_mem_usage(initial_time)
@@ -3193,46 +3239,47 @@
             None,
             path_overlapping_outfile + ".tmp",
             n,
             overlapping=True,
             chunk_by_key=True,
         )
         os.rename(path_overlapping_outfile + ".tmp", path_overlapping_outfile)
-        write(f"> Table with non-overlapping hits created --> {output_folder+'/'+path_overlapping_outfile}")
+        write(
+            f"> Table with non-overlapping hits created --> {output_folder+'/'+path_overlapping_outfile}"
+        )
 
         run_phase3 = True
     else:
         write(f"File found: {path_overlapping_outfile}")
 
-    if True: #run_phase3 or benchmark:
+    if True:  # run_phase3 or benchmark:
         trans_candidates = pd.read_csv(
             path_overlapping_outfile,
             usecols=["Chromosome"],
             sep="\t",
             header=0,
             index_col=False,
         )["Chromosome"]
 
         write(
             f"= After removing overlapping hits, Nº of hits: {len(trans_candidates):,.0f}",
-            how=colors['count'],
-        )        
+            how=colors["count"],
+        )
         write(
             f"= After removing overlapping hits, Nº of unique subject transcripts: {len(trans_candidates.unique()):,.0f}",
-            how=colors['count'],
+            how=colors["count"],
         )
 
         if benchmark:
-
-            num=available_selenos.Transcript.isin(trans_candidates).sum()
-            denom=len(available_selenos)
+            num = available_selenos.Transcript.isin(trans_candidates).sum()
+            denom = len(available_selenos)
             # and we check how many expected selenoprotein transcripts have successfully passed the filter
             write(
                 f"% Benchmark TP: {num}/{denom}  Recall={num/denom:.2%}",
-                how=colors['bm']
+                how=colors["bm"],
             )
 
         del trans_candidates
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
@@ -3257,42 +3304,43 @@
             path_extend_outfile + ".tmp",
             n,
             ext_orfs=True,
             chunk_by_key=True,
         )
         os.rename(path_extend_outfile + ".tmp", path_extend_outfile)
         run_phase4 = True
-        write(f"> Table with non-identical extended ORFs --> {output_folder+'/'+path_extend_outfile}")
+        write(
+            f"> Table with non-identical extended ORFs --> {output_folder+'/'+path_extend_outfile}"
+        )
     else:
         write(f"File found: {path_extend_outfile}")
 
-    if True: #run_phase4 or benchmark:
+    if True:  # run_phase4 or benchmark:
         trans_candidates = pd.read_csv(
             path_extend_outfile,
             sep="\t",
             header=0,
             index_col=False,
             usecols=["Chromosome"],
         )["Chromosome"]
         write(
             f"= After removing duplicated and non-UGA extended ORFs, Nº of hits: {len(trans_candidates):,.0f}",
-            how=colors['count'],
+            how=colors["count"],
         )
         write(
             f"= After removing duplicated and non-UGA extended ORFs, Nº of unique subject transcripts: {len(trans_candidates.unique()):,.0f}",
-            how=colors['count'],
+            how=colors["count"],
         )
         if benchmark:
-
-            num=available_selenos.Transcript.isin(trans_candidates).sum()
-            denom=len(available_selenos)
+            num = available_selenos.Transcript.isin(trans_candidates).sum()
+            denom = len(available_selenos)
             # and we check how many expected selenoprotein transcripts have successfully passed the filter
             write(
                 f"% Benchmark TP: {num}/{denom}  Recall={num/denom:.2%}",
-                how=colors['bm']
+                how=colors["bm"],
             )
 
         del trans_candidates
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
@@ -3311,15 +3359,17 @@
             n_cpu,
             opt["timeout"],
             path_pairwise_outfile + ".tmp",
             n,
             pairwise=True,
         )
         os.rename(path_pairwise_outfile + ".tmp", path_pairwise_outfile)
-        write(f"> Table including aligned sequences --> {output_folder+'/'+path_pairwise_outfile}")
+        write(
+            f"> Table including aligned sequences --> {output_folder+'/'+path_pairwise_outfile}"
+        )
     else:
         write(f"File found: {path_pairwise_outfile}")
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
@@ -3332,24 +3382,34 @@
         write(description_of_phases[6])
         # as we are not using chunking(), pre-phase file must be read to pass it as arg to the next phase function
         aln_orfs = pd.read_csv(
             path_pairwise_outfile, sep="\t", header=0, index_col=False
         )
         # calling function
         candidates_df = UGA_alignments(aln_orfs)
+
+        # MM: replacing U with * except for target UGA; also updating score
+        # candidates_df[["Q_align_prot_seq", "Subj_align_prot_seq", "Score"]] = (
+        #     candidates_df[["Q_align_prot_seq", "Subj_align_prot_seq", "Score"]].apply(
+        #         replace_non_target_ugas, axis=1, result_type="expand"
+        #     )
+        # )
+
         # saving dataframe as a csv file
         candidates_df = candidates_df.sort_values(
             by="Score", ascending=False, ignore_index=True
         ).drop_duplicates("Chromosome", ignore_index=True)
         candidates_df.to_csv(
             path_or_buf=path_candidates_outfile + ".tmp", sep="\t", index=False
         )
         os.rename(path_candidates_outfile + ".tmp", path_candidates_outfile)
 
-        write(f"> Table created with candidates --> {output_folder+'/'+path_candidates_outfile}")
+        write(
+            f"> Table created with candidates --> {output_folder+'/'+path_candidates_outfile}"
+        )
 
         run_phase6 = True
         ##########  MODIFY TO: do chunking if not benchmarking; if benchmark, keep code above
         ###
 
         # else:
         #     chunking(path_pairwise_outfile, n_chunks, 0, UGA_alignments,
@@ -3364,39 +3424,39 @@
         #     .sort_values(by='Score', ascending=False, ignore_index=True) \
         #     .drop_duplicates('Chromosome', ignore_index=True)
         # candidates_df.to_csv(path_or_buf=path_candidates_outfile, sep='\t', index=False)
         # here there is a control to prevent empty dfs to be passed to the next phase causing an error
         if len(candidates_df) == 0:
             write(f"Empty file {candidates_df}")
 
-    if True: #run_phase6 or benchmark:
+    if True:  # run_phase6 or benchmark:
         write(
             f"= After the UGA alignment filter, Nº of candidates: {len(candidates_df):,.0f}",
-            how=colors['count'],
+            how=colors["count"],
         )
         write(
             f"= After the UGA alignment filter, Nº of unique subject transcripts: {len(candidates_df.Chromosome.unique()):,.0f}",
-            how=colors['count'],
+            how=colors["count"],
         )
 
         candidates_df[["sec_start", "sec_end"]] = candidates_df.apply(
             find_sec_pos, axis=1, result_type="expand"
         )
         if benchmark:
-            candidates_df= final_benchmark(candidates_df, sp4_subj_gff)
+            candidates_df = final_benchmark(candidates_df, sp4_subj_gff)
             tp = candidates_df[candidates_df.true_positive == True].shape[0]
             fp = candidates_df[candidates_df.true_positive == False].shape[0]
             fn = available_selenos.shape[0] - tp
             precision = tp / (tp + fp)
             recall = tp / (tp + fn)
-            write(f"% Precise benchmark TP: {tp}/{tp+fn} Recall={recall:.2%} Precision={precision:.2%}",
-                  how=colors['bm'])
-
+            write(
+                f"% Precise benchmark TP: {tp}/{tp+fn} Recall={recall:.2%} Precision={precision:.2%}",
+                how=colors["bm"],
+            )
 
-        
         # if benchmark:
         #     num=available_selenos.Transcript.isin(candidates_df.Chromosome).sum()
         #     denom=len(available_selenos)
         #     # and we check how many expected selenoprotein transcripts have successfully passed the filter
         #     write(
         #         f"% Benchmark TP: {num}/{denom}  Recall={num/denom:.2%}",
         #         how=colors['bm']
@@ -3428,34 +3488,33 @@
     # sp4_subj_gff['sec_start'] -= 1
     # sp4_subj_gff = sp4_subj_gff[sp4_subj_gff['feature'] == 'Selenocysteine'].reset_index(drop=True)
     # print(sp4_subj_gff)
     if not os.path.exists(path_selenocandidates_outfile) or n_section < 8:
         write(description_of_phases[7])
         selenocandidates_df = preprocessing_candidates(candidates_df, q_file, subj_file)
         del candidates_df
-            
+
         if opt["model"] == "d":
             lr_filepath = twinstop_libpath + "logistic_regression_model.def.pkl"
         elif opt["model"] == "p":
             lr_filepath = twinstop_libpath + "logistic_regression_model.pre.pkl"
         elif opt["model"] == "s":
             lr_filepath = twinstop_libpath + "logistic_regression_model.sen.pkl"
 
-
-
-            
         lr_preds, y = regression_filter(selenocandidates_df, lr_filepath, n_cpu)
         selenocandidates_df = selenocandidates_df[lr_preds]
         selenocandidates_df.sort_values(
             by="Density_Score", inplace=True, ignore_index=True, ascending=False
         )
         selenocandidates_df.to_csv(
             path_or_buf=path_selenocandidates_outfile, sep="\t", index=False
         )
-        write(f"> Table with final set of candidates --> {output_folder+'/'+path_selenocandidates_outfile}")
+        write(
+            f"> Table with final set of candidates --> {output_folder+'/'+path_selenocandidates_outfile}"
+        )
 
         # if benchmark:
         #     (_, fp_ml, fn_ml, tp_ml) = confusion_matrix(y, lr_preds).ravel()
         #     precision_ml = round(tp_ml / (tp_ml + fp_ml), 4)
         #     recall_ml = round(tp_ml / (tp_ml + fn_ml), 4)
         #     write(f"\nPrecision_lr: {precision_ml}")
         #     write(f"\nSensitivity_lr: {recall_ml}\n")
@@ -3463,48 +3522,48 @@
         #     write(f"\nSensitivity Twinstop: {recall * recall_ml}\n")
     else:
         selenocandidates_df = pd.read_csv(
             path_selenocandidates_outfile, sep="\t", header=0, index_col=False
         )
         write(f"File found: {path_selenocandidates_outfile}")
 
-
     # write(f'After final filter, Nº of candidates: {buf_count_newlines_gen(path_selenocandidates_outfile)}', how=colors['count'])
     write(
         f"= After final filter, Nº of candidates: {len(selenocandidates_df)}",
-        how=colors['count'],
+        how=colors["count"],
     )
     write(
         f"= After final filter, Nº of unique subject transcripts: {len(selenocandidates_df.Chromosome.unique())}",
-        how=colors['count'],
+        how=colors["count"],
     )
     # write(f'\nTP: {available_selenos.Transcript.isin(selenocandidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
     if benchmark:
-        selenocandidates_df= final_benchmark(selenocandidates_df, sp4_subj_gff)
+        selenocandidates_df = final_benchmark(selenocandidates_df, sp4_subj_gff)
         tp = selenocandidates_df[selenocandidates_df.true_positive == True].shape[0]
         fp = selenocandidates_df[selenocandidates_df.true_positive == False].shape[0]
         fn = available_selenos.shape[0] - tp
         precision = tp / (tp + fp)
         recall = tp / (tp + fn)
-        write(f"% Precise benchmark TP: {tp}/{tp+fn} Recall={recall:.2%} Precision={precision:.2%}",
-              how=colors['bm'])
+        write(
+            f"% Precise benchmark TP: {tp}/{tp+fn} Recall={recall:.2%} Precision={precision:.2%}",
+            how=colors["bm"],
+        )
 
-    
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
     if opt["ann"]:
         # write('\n### PHASE 8: BLASTP FOR ANNOTATION', how=colors['phase'])
         write_phase(8)
     else:
         write("\n### Skipping PHASE 8 because not requested...")
 
-    if not "Annot_Title" in selenocandidates_df and opt["ann"]:
+    if opt['ann'] and ( not os.path.exists(path_selenocandidates_annotated_outfile) or n_section < 9 ):
         write(description_of_phases[8])
         selenocandidates_df = run_blastp(
             selenocandidates_df,
             opt["ann_db"],
             n_cpu,
             path_blastp_outfile,
             path_fasta_query_prot_seq,
@@ -3513,14 +3572,20 @@
             by="Density_Score", inplace=True, ignore_index=True, ascending=False
         )
         selenocandidates_df.to_csv(
             sep="\t", path_or_buf=path_selenocandidates_annotated_outfile, index=False
         )
         # write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
         # write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
+    elif opt['ann'] and os.path.exists(path_selenocandidates_annotated_outfile):
+        del selenocandidates_df
+        selenocandidates_df = pd.read_csv(
+            path_selenocandidates_annotated_outfile, sep="\t", header=0, index_col=False
+        )
+        write(f"File found: {path_selenocandidates_annotated_outfile}")
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
     # write('\n### PHASE 9: OUTPUT', how=colors['phase'])
     write_phase(9)
@@ -3543,23 +3608,50 @@
         path_pep_q,
         opt["pep_s"],
         path_pep_t,
         opt["gff_q"],
         opt["gff_s"],
         path_gff_q,
         path_gff_t,
-        output_folder
+        output_folder,
     )
 
     if time_memory_control:
         time_mem_usage(initial_time)
 
     write("")
     write(
         f' Twinstop completed | Date: {datetime.now().strftime("%Y-%m-%d %H:%M:%S")} '.center(
             70, "*"
         )
     )
 
 
+# def replace_non_target_ugas(row):
+#     """Replace all Us with * in query and subject aligned sequences, except the one corresponding to index_u
+
+#     Returns:
+#       (updated_query_seq, updated_subj_seq, updated score)
+
+#     """
+#     # MM
+#     index_u = UGA(row["Q_align_prot_seq"], row["Subj_align_prot_seq"])
+#     q_aligned_seq = "".join(
+#         [
+#             "*" if (qaa == "U" and index != index_u) else qaa
+#             for index, qaa in enumerate(row["Q_align_prot_seq"])
+#         ]
+#     )
+#     s_aligned_seq = "".join(
+#         [
+#             "*" if (saa == "U" and index != index_u) else saa
+#             for index, saa in enumerate(row["Subj_align_prot_seq"])
+#         ]
+#     )
+
+#     the_score = score(q_aligned_seq, s_aligned_seq, blosum_matrix)["Score"]
+
+#     return (q_aligned_seq, s_aligned_seq, score)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `twinstop-0.1.3/src/twinstop/test_alignment_methods.py` & `twinstop-0.1.4/src/twinstop/test_alignment_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,22 +130,26 @@
 #     #         print(f'Second pairwise worked with timeout {timeout}')
 #     # else:
 #     #     post_df = pd.concat(results, axis=0, ignore_index=True)
 #     #     print(f'Second pairwise worked with timeout {timeout}')
 #
 #     return results
 
+def chunkify(df, n):
+    """Split DataFrame into n chunks."""
+    k, m = divmod(len(df), n)
+    return (df.iloc[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)] for i in range(n))
 
 def multiprocessing(chunkdf, func, n_cpu, timeout):
     with mp.Pool(processes=n_cpu) as pool:
         # lock = mp.Manager().Lock()
         # shared_list = manager.list()
         results = []
         completed_results = []
-        for row in np.array_split(chunkdf, len(chunkdf)):
+        for row in chunkify(chunkdf, len(chunkdf)):
             result = pool.apply_async(func, args=(row,))
             results.append(result)
         for result in results:
             try:
                 completed_results.append(result.get(timeout=timeout))
             except mp.context.TimeoutError:
                 print(f"A result took too long")
```

### Comparing `twinstop-0.1.3/src/twinstop.egg-info/PKG-INFO` & `twinstop-0.1.4/src/twinstop.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.1.3
+Version: 0.1.4
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,20 +12,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython<=1.81,>=1.78
 Requires-Dist: easyterm>=1.0.0
 Requires-Dist: easybioinfo>=0.3.1
 Requires-Dist: orf_tools>=0.0.1
 Requires-Dist: file-chunk-iterators>=0.0.1
-Requires-Dist: pyranges>=0.0.120
-Requires-Dist: pandas>=1.3.5
+Requires-Dist: pyranges<1.0.0,>=0.1.2
+Requires-Dist: pandas<2.0.0,>=1.3.5
 Requires-Dist: pyfaidx>=0.7.2
 Requires-Dist: multiprocess>=0.70.14
 Requires-Dist: numpy>=1.21.5
-Requires-Dist: scikit-learn>=1.3.0
+Requires-Dist: scikit-learn==1.3.0
 
 # twinstop
 Twinstop identifies selenoproteins in close related transcriptomes
 
 # Installation
 In a new conda environment, run::
```

### Comparing `twinstop-0.1.3/src/twinstop.egg-info/SOURCES.txt` & `twinstop-0.1.4/src/twinstop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

