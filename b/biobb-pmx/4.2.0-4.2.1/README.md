# Comparing `tmp/biobb_pmx-4.2.0.tar.gz` & `tmp/biobb_pmx-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_pmx-4.2.0.tar", last modified: Mon May 27 15:35:40 2024, max compression
+gzip compressed data, was "biobb_pmx-4.2.1.tar", last modified: Wed May 29 14:17:47 2024, max compression
```

## Comparing `biobb_pmx-4.2.0.tar` & `biobb_pmx-4.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.685871 biobb_pmx-4.2.0/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:55:35.000000 biobb_pmx-4.2.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6621 2024-05-27 15:35:40.685352 biobb_pmx-4.2.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5705 2024-05-24 11:12:34.000000 biobb_pmx-4.2.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.674403 biobb_pmx-4.2.0/biobb_pmx/
--rw-r--r--   0 pau        (501) staff       (20)       88 2024-05-24 11:12:01.000000 biobb_pmx-4.2.0/biobb_pmx/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.684017 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/
--rwxr-xr-x   0 pau        (501) staff       (20)      329 2024-05-21 10:57:48.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)     1836 2023-09-17 21:35:55.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13304 2024-05-24 08:55:34.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxanalyse.py
--rwxr-xr-x   0 pau        (501) staff       (20)    18207 2024-05-24 08:55:53.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxatom_mapping.py
--rwxr-xr-x   0 pau        (501) staff       (20)    10070 2024-05-24 08:56:05.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxcreate_top.py
--rwxr-xr-x   0 pau        (501) staff       (20)    10712 2024-05-24 08:56:14.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxgentop.py
--rwxr-xr-x   0 pau        (501) staff       (20)    16799 2024-05-24 08:56:23.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxligand_hybrid.py
--rwxr-xr-x   0 pau        (501) staff       (20)     7028 2024-05-24 08:56:31.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxmerge_ff.py
--rwxr-xr-x   0 pau        (501) staff       (20)    10077 2024-05-24 08:57:02.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxmutate.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.684872 biobb_pmx-4.2.0/biobb_pmx/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:55:35.000000 biobb_pmx-4.2.0/biobb_pmx/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.677329 biobb_pmx-4.2.0/biobb_pmx.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6621 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      579 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      380 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       37 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       10 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-27 15:35:40.686184 biobb_pmx-4.2.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1770 2024-05-24 11:10:09.000000 biobb_pmx-4.2.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-29 14:17:47.076632 biobb_pmx-4.2.1/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:55:35.000000 biobb_pmx-4.2.1/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6621 2024-05-29 14:17:47.075963 biobb_pmx-4.2.1/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5705 2024-05-29 14:15:45.000000 biobb_pmx-4.2.1/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-29 14:17:47.065974 biobb_pmx-4.2.1/biobb_pmx/
+-rw-r--r--   0 pau        (501) staff       (20)       88 2024-05-29 14:13:40.000000 biobb_pmx-4.2.1/biobb_pmx/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-29 14:17:47.074848 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/
+-rwxr-xr-x   0 pau        (501) staff       (20)      329 2024-05-21 10:57:48.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     1955 2024-05-29 13:18:02.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/common.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13340 2024-05-29 13:20:46.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxanalyse.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    18383 2024-05-29 13:25:06.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxatom_mapping.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10121 2024-05-29 13:33:57.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxcreate_top.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10756 2024-05-29 13:25:07.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxgentop.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    16893 2024-05-29 13:38:55.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxligand_hybrid.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     7089 2024-05-29 13:40:31.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxmerge_ff.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10133 2024-05-29 14:03:13.000000 biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxmutate.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-29 14:17:47.075596 biobb_pmx-4.2.1/biobb_pmx/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:55:35.000000 biobb_pmx-4.2.1/biobb_pmx/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-29 14:17:47.068379 biobb_pmx-4.2.1/biobb_pmx.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6621 2024-05-29 14:17:46.000000 biobb_pmx-4.2.1/biobb_pmx.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      579 2024-05-29 14:17:46.000000 biobb_pmx-4.2.1/biobb_pmx.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-29 14:17:46.000000 biobb_pmx-4.2.1/biobb_pmx.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      380 2024-05-29 14:17:46.000000 biobb_pmx-4.2.1/biobb_pmx.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       37 2024-05-29 14:17:46.000000 biobb_pmx-4.2.1/biobb_pmx.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       10 2024-05-29 14:17:46.000000 biobb_pmx-4.2.1/biobb_pmx.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-29 14:17:47.076820 biobb_pmx-4.2.1/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1770 2024-05-29 14:13:07.000000 biobb_pmx-4.2.1/setup.py
```

### Comparing `biobb_pmx-4.2.0/LICENSE` & `biobb_pmx-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_pmx-4.2.0/PKG-INFO` & `biobb_pmx-4.2.1/biobb_pmx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb_pmx
-Version: 4.2.0
+Name: biobb-pmx
+Version: 4.2.1
 Summary: Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Home-page: https://github.com/bioexcel/biobb_pmx
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-pmx.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pmx?label=Version)](https://GitHub.com/bioexcel/biobb_pmx/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pmx.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pmx/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pmx?label=Conda)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pmx?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pmx)
 [![](https://img.shields.io/pypi/pyversions/biobb-pmx.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pmx/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pmx)
 
 [![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest&label=Docs)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
@@ -59,60 +59,60 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pmx.readthedocs.io/en/latest/).
 
 ### Version
-v4.2.0 2023.3
+v4.2.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
-        pip install "biobb_pmx>=4.2.0"
+        pip install "biobb_pmx>=4.2.1"
 
 
 * Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pmx>=4.2.0"
+        conda install -c bioconda "biobb_pmx>=4.2.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pmx:4.2.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pmx:4.2.1--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0
+        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pmx.sif <command>
```

### Comparing `biobb_pmx-4.2.0/README.md` & `biobb_pmx-4.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pmx?label=Version)](https://GitHub.com/bioexcel/biobb_pmx/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pmx.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pmx/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pmx?label=Conda)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pmx?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pmx)
 [![](https://img.shields.io/pypi/pyversions/biobb-pmx.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pmx/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pmx)
 
 [![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest&label=Docs)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
@@ -37,60 +37,60 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pmx.readthedocs.io/en/latest/).
 
 ### Version
-v4.2.0 2023.3
+v4.2.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
-        pip install "biobb_pmx>=4.2.0"
+        pip install "biobb_pmx>=4.2.1"
 
 
 * Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pmx>=4.2.0"
+        conda install -c bioconda "biobb_pmx>=4.2.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pmx:4.2.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pmx:4.2.1--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0
+        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pmx.sif <command>
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/common.py` & `biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 
 MUTATION_DICT = {'ALA': 'A', 'ARG': 'R', 'ASN': 'N', 'ASP': 'D', 'ASPH': 'B', 'ASPP': 'B', 'ASH': 'B', 'CYS': 'C', 'CYS2': 'C', 'CYN': 'C', 'CYX': 'CX', 'CYM': 'CM', 'CYSH': 'C', 'GLU': 'E', 'GLUH': 'J', 'GLUP': 'J', 'GLH': 'J', 'GLN': 'Q', 'GLY': 'G', 'HIS': 'H', 'HIE': 'X', 'HISE': 'X', 'HSE': 'X', 'HIP': 'Z', 'HSP': 'Z', 'HISH': 'Z', 'HID': 'H', 'HSD': 'H', 'ILE': 'I', 'LEU': 'L', 'LYS': 'K', 'LYSH': 'K', 'LYP': 'K', 'LYN': 'O', 'LSN': 'O', 'MET': 'M', 'PHE': 'F', 'PRO': 'P', 'SER': 'S', 'SP1': 'SP1', 'SP2': 'SP2', 'THR': 'T', 'TRP': 'W', 'TYR': 'Y', 'VAL': 'V', 'A': 'A', 'T': 'T', 'C': 'C', 'G': 'G', 'U': 'U'}
 
 
 def create_mutations_file(input_mutations_path: str, mutation_list: Union[str, Iterable[str]], mutation_dict: Mapping) -> str:
     try:
         # Check if self.mutation_list is a string
-        mutation_list = mutation_list.replace(" ", "").split(',')
+        mutation_list = mutation_list.replace(" ", "").split(',')  # type: ignore
     except AttributeError:
         pass
     pattern = re.compile(r"(?P<chain>[a-zA-Z])*:?(?P<resnum>\d+)(?P<mt>[a-zA-Z0-9]+)")
     with open(input_mutations_path, 'w') as mut_file:
         for mut in mutation_list:
-            mut_groups_dict = pattern.match(mut.strip()).groupdict()
-            if mut_groups_dict.get('chain'):
-                mut_file.write(mut_groups_dict.get('chain') + ' ')
-            mut_file.write(mut_groups_dict.get('resnum') + ' ')
-            if not mut_groups_dict.get('mt').upper() in mutation_dict.keys():
-                raise TypeError(
-                    f"{mut_groups_dict.get('mt').upper()} is not a valid AA code or NA code. Possible values are {mutation_dict.keys()}")
-            mut_file.write(mutation_dict[mut_groups_dict.get('mt').upper()])
-            mut_file.write('\n')
+            match = pattern.match(mut.strip())
+            if match:
+                mut_groups_dict = match.groupdict()
+                if mut_groups_dict.get('chain'):
+                    mut_file.write(mut_groups_dict.get('chain', '') + ' ')
+                mut_file.write(mut_groups_dict.get('resnum', '') + ' ')
+                if not mut_groups_dict.get('mt', '').upper() in mutation_dict.keys():
+                    raise TypeError(
+                        f"{mut_groups_dict.get('mt','').upper()} is not a valid AA code or NA code. Possible values are {mutation_dict.keys()}")
+                mut_file.write(mutation_dict[mut_groups_dict.get('mt', '').upper()])
+                mut_file.write('\n')
 
     return input_mutations_path
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxanalyse.py` & `biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxanalyse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """Module containing the PMX analyse class and the command line interface."""
 import argparse
 from pathlib import Path
 import shutil
-from typing import Mapping
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxanalyse(BiobbObject):
@@ -71,15 +71,15 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_a_xvg_zip_path: str, input_b_xvg_zip_path: str, output_result_path: str, output_work_plot_path: str,
-                 properties: Mapping = None, **kwargs) -> None:
+                 properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -136,16 +136,16 @@
         list_a = list(filter(lambda f: Path(f).exists() and Path(f).stat().st_size > 10, fu.unzip_list(self.input_a_xvg_zip_path, list_a_dir, self.out_log)))
         list_b = list(filter(lambda f: Path(f).exists() and Path(f).stat().st_size > 10, fu.unzip_list(self.input_b_xvg_zip_path, list_b_dir, self.out_log)))
         string_a = " ".join(list_a)
         string_b = " ".join(list_b)
 
         # Copy extra files to container: two directories containing the xvg files
         if self.container_path:
-            shutil.copytree(list_a_dir, Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(list_a_dir).name))
-            shutil.copytree(list_b_dir, Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(list_b_dir).name))
+            shutil.copytree(list_a_dir, Path(self.stage_io_dict.get("unique_dir", "")).joinpath(Path(list_a_dir).name))
+            shutil.copytree(list_b_dir, Path(self.stage_io_dict.get("unique_dir", "")).joinpath(Path(list_b_dir).name))
             container_volume = " " + self.container_volume_path + "/"
             string_a = self.container_volume_path + "/" + container_volume.join(list_a)
             string_b = self.container_volume_path + "/" + container_volume.join(list_b)
 
         self.cmd = [self.binary_path, 'analyse',
                     '-fA', string_a,
                     '-fB', string_b,
@@ -196,24 +196,24 @@
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir"), list_a_dir, list_b_dir])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", ""), list_a_dir, list_b_dir])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxanalyse(input_a_xvg_zip_path: str, input_b_xvg_zip_path: str,
                output_result_path: str, output_work_plot_path: str,
-               properties: dict = None, **kwargs) -> int:
+               properties: Optional[Dict] = None, **kwargs) -> int:
     """Execute the :class:`Pmxanalyse <pmx.pmxanalyse.Pmxanalyse>` class and
     execute the :meth:`launch() <pmx.pmxanalyse.Pmxanalyse.launch> method."""
 
     return Pmxanalyse(input_a_xvg_zip_path=input_a_xvg_zip_path,
                       input_b_xvg_zip_path=input_b_xvg_zip_path,
                       output_result_path=output_result_path,
                       output_work_plot_path=output_work_plot_path,
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxatom_mapping.py` & `biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxatom_mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Module containing the PMX atom_mapping class and the command line interface."""
 import os
 import sys
 from pathlib import Path
 import shutil
 import argparse
-from typing import Mapping
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxatom_mapping(BiobbObject):
     """
@@ -76,17 +76,17 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_structure1_path: str, input_structure2_path: str, output_pairs1_path: str, output_pairs2_path: str,
-                 output_log_path: str, output_structure1_path: str = None, output_structure2_path: str = None, output_morph1_path: str = None,
-                 output_morph2_path: str = None, output_scaffold1_path: str = None, output_scaffold2_path: str = None, output_score_path: str = None,
-                 properties: Mapping = None, **kwargs) -> None:
+                 output_log_path: str, output_structure1_path: Optional[str] = None, output_structure2_path: Optional[str] = None, output_morph1_path: Optional[str] = None,
+                 output_morph2_path: Optional[str] = None, output_scaffold1_path: Optional[str] = None, output_scaffold2_path: Optional[str] = None, output_score_path: Optional[str] = None,
+                 properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -123,18 +123,18 @@
         self.swap = properties.get('swap')
         self.nochirality = properties.get('nochirality')
         self.distance = properties.get('distance')
         self.timeout = properties.get('timeout')
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
-        if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+        if not self.gmx_lib and os.environ.get('CONDA_PREFIX', ''):
             python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
+                Path(os.environ.get('CONDA_PREFIX', '')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
                 self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
         self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
@@ -221,25 +221,25 @@
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
+        self.tmp_files.append(self.stage_io_dict.get("unique_dir", ""))
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxatom_mapping(input_structure1_path: str, input_structure2_path: str, output_pairs1_path: str, output_pairs2_path: str,
-                    output_log_path: str, output_structure1_path: str = None, output_structure2_path: str = None, output_morph1_path: str = None,
-                    output_morph2_path: str = None, output_scaffold1_path: str = None, output_scaffold2_path: str = None, output_score_path: str = None,
-                    properties: dict = None, **kwargs) -> int:
+                    output_log_path: str, output_structure1_path: Optional[str] = None, output_structure2_path: Optional[str] = None, output_morph1_path: Optional[str] = None,
+                    output_morph2_path: Optional[str] = None, output_scaffold1_path: Optional[str] = None, output_scaffold2_path: Optional[str] = None, output_score_path: Optional[str] = None,
+                    properties: Optional[Dict] = None, **kwargs) -> int:
     """Execute the :class:`Pmxatom_mapping <pmx.pmxmutate.Pmxatom_mapping>` class and
     execute the :meth:`launch() <pmx.pmxatom_mapping.Pmxatom_mapping.launch> method."""
 
     return Pmxatom_mapping(input_structure1_path=input_structure1_path, input_structure2_path=input_structure2_path,
                            output_pairs1_path=output_pairs1_path, output_pairs2_path=output_pairs2_path,
                            output_log_path=output_log_path,
                            output_structure1_path=output_structure1_path, output_structure2_path=output_structure2_path,
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxcreate_top.py` & `biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxcreate_top.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Module containing the PMX create_top class and the command line interface."""
 import os
 import sys
 from pathlib import Path, PurePath
 import shutil
 import argparse
-from typing import Mapping
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxcreate_top(BiobbObject):
@@ -58,15 +58,15 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_topology1_path: str, input_topology2_path: str, output_topology_path: str,
-                 properties: Mapping = None, **kwargs) -> None:
+                 properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -79,18 +79,18 @@
         self.force_field = properties.get('force_field', "amber99sb-star-ildn-mut.ff")
         self.water = properties.get('water', "tip3p")
         self.system_name = properties.get('system_name', "Pmx topology")
         self.mols = properties.get('mols', [['Protein', 1], ['Ligand', 1]])
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
-        if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+        if not self.gmx_lib and os.environ.get('CONDA_PREFIX', ''):
             python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
+                Path(os.environ.get('CONDA_PREFIX', '')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
                 self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
         self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
@@ -100,27 +100,27 @@
         """Execute the :class:`Pmxcreate_top <pmx.pmxcreate_top.Pmxcreate_top>` pmx.pmxcreate_top.Pmxcreate_top object."""
 #        os.chdir("/Users/hospital/BioBB/Notebooks_dev/biobb_wf_pmx_tutorial_ligands/biobb_wf_pmx_tutorial/notebooks")
         # Setup Biobb
         if self.check_restart():
             return 0
         self.stage_files()
 
-        self.out_log.info('Running create_top from pmx package...\n')
+        fu.log('Running create_top from pmx package...\n', self.out_log)
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
-        self.out_log.info('Creating %s temporary folder' % self.tmp_folder)
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
         itp = os.path.basename(os.path.normpath(self.stage_io_dict["in"]["input_topology1_path"]))
-        self.out_log.info('Creating %s itp file in temporary folder' % itp)
+        fu.log('Creating %s itp file in temporary folder' % itp, self.out_log)
         itp_local = str(PurePath(self.tmp_folder).joinpath(itp))
         shutil.copyfile(self.io_dict['in']['input_topology1_path'], itp_local)
 
         itp2 = os.path.basename(os.path.normpath(self.stage_io_dict["in"]["input_topology2_path"]))
-        self.out_log.info('Creating %s itp file in temporary folder' % itp2)
+        fu.log('Creating %s itp file in temporary folder' % itp2, self.out_log)
         itp2_local = str(PurePath(self.tmp_folder).joinpath(itp2))
         shutil.copyfile(self.io_dict['in']['input_topology2_path'], itp2_local)
 
         top_local = str(PurePath(self.tmp_folder).joinpath("topology.top"))
 
         # _create_top function, taken from the pmx AZ tutorial:
         # https://github.com/deGrootLab/pmx/blob/develop/tutorials/AZtutorial.py
@@ -152,31 +152,31 @@
         top_final = str(PurePath(current_cwd).joinpath(self.io_dict["out"]["output_topology_path"]))
 
         os.chdir(self.tmp_folder)
         fu.log('Compressing topology to: %s' % top_final, self.out_log, self.global_log)
         fu.zip_top(zip_file=top_final, top_file="topology.top", out_log=self.out_log)
         os.chdir(current_cwd)
 
-        self.out_log.info('Exit code 0\n')
+        fu.log('Exit code 0\n', self.out_log)
 
         # Run Biobb block
         # self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
+        self.tmp_files.append(self.stage_io_dict.get("unique_dir", ""))
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxcreate_top(input_topology1_path: str, input_topology2_path: str, output_topology_path: str,
-                  properties: dict = None, **kwargs) -> int:
+                  properties: Optional[Dict] = None, **kwargs) -> int:
     """Execute the :class:`Pmxcreate_top <pmx.pmxcreate_top.Pmxcreate_top>` class and
     execute the :meth:`launch() <pmx.pmxmcreate_top.Pmxmcreate_top.launch> method."""
 
     return Pmxcreate_top(input_topology1_path=input_topology1_path, input_topology2_path=input_topology2_path,
                          output_topology_path=output_topology_path,
                          properties=properties, **kwargs).launch()
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxgentop.py` & `biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxgentop.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Module containing the PMX gentop class and the command line interface."""
 import os
 import sys
 import argparse
 import shutil
 from pathlib import Path
-from typing import Mapping
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxgentop(BiobbObject):
@@ -57,15 +57,15 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_top_zip_path: str, output_top_zip_path: str,
-                 properties: Mapping = None, **kwargs) -> None:
+                 properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -79,18 +79,18 @@
         # Properties specific for BB
         self.force_field = properties.get('force_field', "amber99sb-star-ildn-mut")
         self.split = properties.get('split', False)
         self.scale_mass = properties.get('scale_mass', False)
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
-        if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+        if not self.gmx_lib and os.environ.get('CONDA_PREFIX', ''):
             python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
+                Path(os.environ.get('CONDA_PREFIX', '')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
                 self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.8/site-packages/pmx/data/mutff/"))
         self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
@@ -116,15 +116,15 @@
 
         # Copy extra files to container: topology folder
         if self.container_path:
             fu.log('Container execution enabled', self.out_log)
             fu.log(f"Unique dir: {self.stage_io_dict['unique_dir']}", self.out_log)
             fu.log(f"{self.stage_io_dict['unique_dir']} files: {os.listdir(self.stage_io_dict['unique_dir'])}", self.out_log)
             fu.log(f"Copy all files of the unzipped original topology to unique dir: {self.out_log}")
-            shutil.copytree(top_dir, str(Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(top_dir).name)))
+            shutil.copytree(top_dir, str(Path(self.stage_io_dict.get("unique_dir", "")).joinpath(Path(top_dir).name)))
             top_file = str(Path(self.container_volume_path).joinpath(Path(top_dir).name, Path(top_file).name))
 
         output_file_name = fu.create_name(prefix=self.prefix, step=self.step, name=str(Path(top_file).name))
         unique_dir_output_file = str(Path(fu.create_unique_dir()).joinpath(output_file_name))
         fu.log(f"unique_dir_output_file: {unique_dir_output_file}", self.out_log)
 
         if self.container_path:
@@ -148,15 +148,15 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         if self.container_path:
-            unique_dir_output_file = str(Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(unique_dir_output_file).name))
+            unique_dir_output_file = str(Path(self.stage_io_dict.get("unique_dir", "")).joinpath(Path(unique_dir_output_file).name))
 
         # Remove paths from top file
         with open(Path(unique_dir_output_file)) as top_fh:
             top_lines = top_fh.readlines()
         with open(Path(unique_dir_output_file), 'w') as top_fh:
             for line in top_lines:
                 top_fh.write(line.replace(str(Path(unique_dir_output_file).parent)+'/', ''))
@@ -167,22 +167,22 @@
                 shutil.copy(orig_itp_file, Path(unique_dir_output_file).parent)
                 fu.log(f'Copying {str(orig_itp_file)} to: {str(Path(unique_dir_output_file).parent)}', self.out_log, self.global_log)
 
         # zip topology
         fu.log('Compressing topology to: %s' % self.io_dict["out"]["output_top_zip_path"], self.out_log, self.global_log)
         fu.zip_top(zip_file=self.io_dict["out"]["output_top_zip_path"], top_file=str(Path(unique_dir_output_file)), out_log=self.out_log)
 
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir"), top_dir])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", ""), top_dir])
         # self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def pmxgentop(input_top_zip_path: str, output_top_zip_path: str, properties: dict = None, **kwargs) -> int:
+def pmxgentop(input_top_zip_path: str, output_top_zip_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Execute the :class:`Pmxgentop <pmx.pmxgentop.Pmxgentop>` class and
     execute the :meth:`launch() <pmx.pmxgentop.Pmxgentop.launch> method."""
 
     return Pmxgentop(input_top_zip_path=input_top_zip_path,
                      output_top_zip_path=output_top_zip_path,
                      properties=properties, **kwargs).launch()
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxligand_hybrid.py` & `biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxligand_hybrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Module containing the PMX ligand_hybrid class and the command line interface."""
 import os
 import sys
 from pathlib import Path
 import shutil
 import argparse
-from typing import Mapping
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxligand_hybrid(BiobbObject):
     """
@@ -78,16 +78,16 @@
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_structure1_path: str, input_structure2_path: str, input_topology1_path: str, input_topology2_path: str,
                  output_log_path: str, output_structure1_path: str, output_structure2_path: str, output_topology_path: str, output_atomtypes_path: str,
-                 input_scaffold1_path: str = None, input_scaffold2_path: str = None, input_pairs_path: str = None,
-                 properties: Mapping = None, **kwargs) -> None:
+                 input_scaffold1_path: Optional[str] = None, input_scaffold2_path: Optional[str] = None, input_pairs_path: Optional[str] = None,
+                 properties: Optional[Dict] = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
@@ -117,18 +117,18 @@
         self.scDUMa = properties.get('scDUMa')
         self.scDUMd = properties.get('scDUMd')
         self.deAng = properties.get('deAng')
         self.distance = properties.get('distance')
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
-        if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+        if not self.gmx_lib and os.environ.get('CONDA_PREFIX', ''):
             python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
+                Path(os.environ.get('CONDA_PREFIX', '')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
                 self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
         self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
@@ -194,25 +194,25 @@
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
+        self.tmp_files.append(self.stage_io_dict.get("unique_dir", ""))
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxligand_hybrid(input_structure1_path: str, input_structure2_path: str, input_topology1_path: str, input_topology2_path: str,
                      output_log_path: str, output_structure1_path: str, output_structure2_path: str, output_topology_path: str, output_atomtypes_path: str,
-                     input_scaffold1_path: str = None, input_scaffold2_path: str = None, input_pairs_path: str = None,
-                     properties: dict = None, **kwargs) -> int:
+                     input_scaffold1_path: Optional[str] = None, input_scaffold2_path: Optional[str] = None, input_pairs_path: Optional[str] = None,
+                     properties: Optional[Dict] = None, **kwargs) -> int:
     """Execute the :class:`Pmxligand_hybrid <pmx.pmxmutate.Pmxligand_hybrid>` class and
     execute the :meth:`launch() <pmx.pmxligand_hybrid.Pmxligand_hybrid.launch> method."""
 
     return Pmxligand_hybrid(input_structure1_path=input_structure1_path, input_structure2_path=input_structure2_path,
                             input_topology1_path=input_topology1_path, input_topology2_path=input_topology2_path,
                             output_log_path=output_log_path,
                             output_structure1_path=output_structure1_path, output_structure2_path=output_structure2_path,
@@ -246,16 +246,16 @@
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
     pmxligand_hybrid(input_structure1_path=args.input_structure1_path, input_structure2_path=args.input_structure2_path,
                      input_topology1_path=args.input_topology1_path, input_topology2_path=args.input_topology2_path,
-                     input_scaffold1_path=args.input_scaffold1_path, input_scaffold2_path=args.input_scaffold2_path,
-                     input_pairs_path=args.input_pairs_path, output_log_path=args.output_log_path,
-                     output_structure1_path=args.output_structure1_path, output_structure2_path=args.output_structure2_path,
-                     output_topology1_path=args.output_topology1_path, output_topology2_path=args.output_topology2_path,
+                     output_log_path=args.output_log_path, output_structure1_path=args.output_structure1_path,
+                     output_structure2_path=args.output_structure2_path, output_topology_path=args.output_topology_path,
+                     output_atomtypes_path=args.output_atomtypes_path, input_scaffold1_path=args.input_scaffold1_path,
+                     input_scaffold2_path=args.input_scaffold2_path, input_pairs_path=args.input_pairs_path,
                      properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxmerge_ff.py` & `biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxmerge_ff.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 """Module containing the PMX merge_ff class and the command line interface."""
 import os
 import sys
 from pathlib import Path
 import glob
 import argparse
-from pmx import ligand_alchemy
-from typing import Mapping
+from pmx import ligand_alchemy  # type: ignore
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxmerge_ff(BiobbObject):
@@ -52,15 +52,15 @@
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_topology_path: str, output_topology_path: str, properties: Mapping = None, **kwargs) -> None:
+    def __init__(self, input_topology_path: str, output_topology_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -70,18 +70,18 @@
         }
 
         # Properties specific for BB
         # None yet
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
-        if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+        if not self.gmx_lib and os.environ.get('CONDA_PREFIX', ''):
             python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
+                Path(os.environ.get('CONDA_PREFIX', '')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
                 self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
         self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
@@ -93,45 +93,45 @@
         # Setup Biobb
         if self.check_restart():
             return 0
         self.stage_files()
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
-        self.out_log.info('Creating %s temporary folder' % self.tmp_folder)
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
         fu.unzip_list(self.stage_io_dict["in"]["input_topology_path"], self.tmp_folder, out_log=self.out_log)
         files = glob.glob(self.tmp_folder+"/*.itp")
         ffsIn_list = []
         for itp in files:
             ffsIn_list.append(itp)
 
-        self.out_log.info('Running merge_FF_files from pmx package...\n')
+        fu.log('Running merge_FF_files from pmx package...\n', self.out_log)
         ligand_alchemy._merge_FF_files(self.stage_io_dict["out"]["output_topology_path"], ffsIn=ffsIn_list)
         # ffsIn=[self.stage_io_dict["in"]["input_topology1_path"],self.stage_io_dict["in"]["input_topology2_path"]] )
 
-        self.out_log.info('Exit code 0\n')
+        fu.log('Exit code 0\n', self.out_log)
 
         if self.gmx_lib:
             self.env_vars_dict['GMXLIB'] = self.gmx_lib
 
         # Run Biobb block
         # self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
+        self.tmp_files.append(self.stage_io_dict.get("unique_dir", ""))
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def pmxmerge_ff(input_topology_path: str, output_topology_path: str, properties: dict = None, **kwargs) -> int:
+def pmxmerge_ff(input_topology_path: str, output_topology_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Execute the :class:`Pmxmerge_ff <pmx.pmxmerge_ff.Pmxmerge_ff>` class and
     execute the :meth:`launch() <pmx.pmxmerge_ff.Pmxmerge_ff.launch> method."""
 
     return Pmxmerge_ff(input_topology_path=input_topology_path,
                        output_topology_path=output_topology_path,
                        properties=properties, **kwargs).launch()
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxmutate.py` & `biobb_pmx-4.2.1/biobb_pmx/pmxbiobb/pmxmutate.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Module containing the PMX mutate class and the command line interface."""
 import os
 from pathlib import Path
 import sys
 import shutil
 import argparse
-from typing import Mapping
+from typing import Dict, Optional
 from biobb_pmx.pmxbiobb.common import create_mutations_file, MUTATION_DICT
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 
 
@@ -60,16 +60,16 @@
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_structure_path: str, output_structure_path: str, input_b_structure_path: str = None,
-                 properties: Mapping = None, **kwargs) -> None:
+    def __init__(self, input_structure_path: str, output_structure_path: str, input_b_structure_path: Optional[str] = None,
+                 properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -85,17 +85,17 @@
         self.input_mutations_file = properties.get('mutations_file')
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
         if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
             python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
+                Path(os.environ.get('CONDA_PREFIX', '')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
-                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
+                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.8/site-packages/pmx/data/mutff/"))
         self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
@@ -121,15 +121,15 @@
                                                           mutation_list=self.mutation_list,
                                                           mutation_dict=MUTATION_DICT)
 
         # Copy extra files to container: mutations file
         if self.container_path:
             fu.log('Container execution enabled', self.out_log)
 
-            shutil.copy2(self.input_mutations_file, self.stage_io_dict.get("unique_dir"))
+            shutil.copy2(self.input_mutations_file, self.stage_io_dict.get("unique_dir", ""))
             self.input_mutations_file = str(Path(self.container_volume_path).joinpath(Path(self.input_mutations_file).name))
 
         self.cmd = [self.binary_path, 'mutate',
                     '-f', self.stage_io_dict["in"]["input_structure_path"],
                     '-o', self.stage_io_dict["out"]["output_structure_path"],
                     '-ff', self.force_field,
                     '--script', self.input_mutations_file]
@@ -145,23 +145,23 @@
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
+        self.tmp_files.append(self.stage_io_dict.get("unique_dir", ""))
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxmutate(input_structure_path: str, output_structure_path: str,
-              input_b_structure_path: str = None, properties: dict = None,
+              input_b_structure_path: Optional[str] = None, properties: Optional[Dict] = None,
               **kwargs) -> int:
     """Execute the :class:`Pmxmutate <pmx.pmxmutate.Pmxmutate>` class and
     execute the :meth:`launch() <pmx.pmxmutate.Pmxmutate.launch> method."""
 
     return Pmxmutate(input_structure_path=input_structure_path,
                      output_structure_path=output_structure_path,
                      input_b_structure_path=input_b_structure_path,
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx.egg-info/PKG-INFO` & `biobb_pmx-4.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb-pmx
-Version: 4.2.0
+Name: biobb_pmx
+Version: 4.2.1
 Summary: Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Home-page: https://github.com/bioexcel/biobb_pmx
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-pmx.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pmx?label=Version)](https://GitHub.com/bioexcel/biobb_pmx/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pmx.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pmx/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pmx?label=Conda)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pmx?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pmx)
 [![](https://img.shields.io/pypi/pyversions/biobb-pmx.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pmx/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pmx)
 
 [![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest&label=Docs)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
@@ -59,60 +59,60 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pmx.readthedocs.io/en/latest/).
 
 ### Version
-v4.2.0 2023.3
+v4.2.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
-        pip install "biobb_pmx>=4.2.0"
+        pip install "biobb_pmx>=4.2.1"
 
 
 * Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pmx>=4.2.0"
+        conda install -c bioconda "biobb_pmx>=4.2.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pmx:4.2.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pmx:4.2.1--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0
+        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pmx.sif <command>
```

### Comparing `biobb_pmx-4.2.0/biobb_pmx.egg-info/SOURCES.txt` & `biobb_pmx-4.2.1/biobb_pmx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_pmx-4.2.0/setup.py` & `biobb_pmx-4.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_pmx",
-    version="4.2.0",
+    version="4.2.1",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_pmx",
```

