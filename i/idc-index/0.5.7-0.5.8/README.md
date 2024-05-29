# Comparing `tmp/idc_index-0.5.7.tar.gz` & `tmp/idc_index-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May 21 15:49:49 2024, max compression
+gzip compressed data, last modified: Wed May 29 08:17:53 2024, max compression
```

## Comparing `idc_index-0.5.7.tar` & `idc_index-0.5.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      125 2024-05-21 15:49:49.000000 idc_index-0.5.7/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-05-21 15:49:49.000000 idc_index-0.5.7/.gitattributes
--rw-r--r--   0        0        0     2357 2024-05-21 15:49:49.000000 idc_index-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-05-21 15:49:49.000000 idc_index-0.5.7/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-05-21 15:49:49.000000 idc_index-0.5.7/noxfile.py
--rw-r--r--   0        0        0     2394 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1585 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      920 2024-05-21 15:49:49.000000 idc_index-0.5.7/docs/conf.py
--rw-r--r--   0        0        0      662 2024-05-21 15:49:49.000000 idc_index-0.5.7/docs/index.md
--rw-r--r--   0        0        0      278 2024-05-21 15:49:49.000000 idc_index-0.5.7/docs/api/idc_index.rst
--rw-r--r--   0        0        0      262 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/_version.pyi
--rw-r--r--   0        0        0    66810 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/py.typed
--rw-r--r--   0        0        0        0 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/__init__.py
--rw-r--r--   0        0        0    14766 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      279 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/study_manifest_bogus.s5cmd
--rw-r--r--   0        0        0      419 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-05-21 15:49:49.000000 idc_index-0.5.7/.gitignore
--rw-r--r--   0        0        0     1077 2024-05-21 15:49:49.000000 idc_index-0.5.7/LICENSE
--rw-r--r--   0        0        0     4303 2024-05-21 15:49:49.000000 idc_index-0.5.7/README.md
--rw-r--r--   0        0        0     6269 2024-05-21 15:49:49.000000 idc_index-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     7588 2024-05-21 15:49:49.000000 idc_index-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-05-29 08:17:53.000000 idc_index-0.5.8/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-29 08:17:53.000000 idc_index-0.5.8/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-05-29 08:17:53.000000 idc_index-0.5.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-05-29 08:17:53.000000 idc_index-0.5.8/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-05-29 08:17:53.000000 idc_index-0.5.8/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-05-29 08:17:53.000000 idc_index-0.5.8/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-29 08:17:53.000000 idc_index-0.5.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-29 08:17:53.000000 idc_index-0.5.8/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-05-29 08:17:53.000000 idc_index-0.5.8/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1585 2024-05-29 08:17:53.000000 idc_index-0.5.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-05-29 08:17:53.000000 idc_index-0.5.8/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      920 2024-05-29 08:17:53.000000 idc_index-0.5.8/docs/conf.py
+-rw-r--r--   0        0        0     2994 2024-05-29 08:17:53.000000 idc_index-0.5.8/docs/index.md
+-rw-r--r--   0        0        0      278 2024-05-29 08:17:53.000000 idc_index-0.5.8/docs/api/idc_index.rst
+-rw-r--r--   0        0        0      262 2024-05-29 08:17:53.000000 idc_index-0.5.8/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-29 08:17:53.000000 idc_index-0.5.8/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-05-29 08:17:53.000000 idc_index-0.5.8/idc_index/_version.pyi
+-rw-r--r--   0        0        0     7438 2024-05-29 08:17:53.000000 idc_index-0.5.8/idc_index/cli.py
+-rw-r--r--   0        0        0    67151 2024-05-29 08:17:53.000000 idc_index-0.5.8/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:17:53.000000 idc_index-0.5.8/idc_index/py.typed
+-rw-r--r--   0        0        0        0 2024-05-29 08:17:53.000000 idc_index-0.5.8/tests/__init__.py
+-rw-r--r--   0        0        0    16458 2024-05-29 08:17:53.000000 idc_index-0.5.8/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-05-29 08:17:53.000000 idc_index-0.5.8/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      279 2024-05-29 08:17:53.000000 idc_index-0.5.8/tests/study_manifest_bogus.s5cmd
+-rw-r--r--   0        0        0      419 2024-05-29 08:17:53.000000 idc_index-0.5.8/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-05-29 08:17:53.000000 idc_index-0.5.8/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-05-29 08:17:53.000000 idc_index-0.5.8/.gitignore
+-rw-r--r--   0        0        0     1077 2024-05-29 08:17:53.000000 idc_index-0.5.8/LICENSE
+-rw-r--r--   0        0        0     4521 2024-05-29 08:17:53.000000 idc_index-0.5.8/README.md
+-rw-r--r--   0        0        0     6326 2024-05-29 08:17:53.000000 idc_index-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     7827 2024-05-29 08:17:53.000000 idc_index-0.5.8/PKG-INFO
```

### Comparing `idc_index-0.5.7/.pre-commit-config.yaml` & `idc_index-0.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/noxfile.py` & `idc_index-0.5.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/.github/CONTRIBUTING.md` & `idc_index-0.5.8/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/.github/matchers/pylint.json` & `idc_index-0.5.8/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/.github/workflows/cd.yml` & `idc_index-0.5.8/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/.github/workflows/ci.yml` & `idc_index-0.5.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/docs/conf.py` & `idc_index-0.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/idc_index/index.py` & `idc_index-0.5.8/idc_index/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 import idc_index_data
 import pandas as pd
 import psutil
 import requests
 from packaging.version import Version
 from tqdm import tqdm
 
-logger = logging.getLogger(__name__)
-logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.INFO)
-
 aws_endpoint_url = "https://s3.amazonaws.com"
 gcp_endpoint_url = "https://storage.googleapis.com"
 
+logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.INFO)
+logger = logging.getLogger(__name__)
+
 
 class IDCClient:
     # Default download hierarchy template
     DOWNLOAD_HIERARCHY_DEFAULT = (
         "%collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID"
     )
 
@@ -779,19 +779,15 @@
 
         if show_progress_bar:
             total_size_bytes = size_MB * 10**6  # Convert MB to bytes
             # temporary place holder. Accurate size is calculated in the next step
             initial_size_bytes = 0
             # Calculate the initial size of the directory
             for directory in list_of_directories:
-                path = Path(directory)
-                if path.exists() and path.is_dir():
-                    initial_size_bytes += sum(
-                        f.stat().st_size for f in path.iterdir() if f.is_file()
-                    )
+                initial_size_bytes = IDCClient._get_dir_sum_file_size(directory)
 
             logger.info("Initial size of the directory: %s bytes", initial_size_bytes)
             logger.info(
                 "Approx. Size of the files need to be downloaded: %s bytes",
                 total_size_bytes,
             )
 
@@ -801,19 +797,15 @@
                 unit_scale=True,
                 desc="Downloading data",
             )
 
             while True:
                 downloaded_bytes = 0
                 for directory in list_of_directories:
-                    path = Path(directory)
-                    if path.exists() and path.is_dir():
-                        downloaded_bytes += sum(
-                            f.stat().st_size for f in path.iterdir() if f.is_file()
-                        )
+                    downloaded_bytes += IDCClient._get_dir_sum_file_size(directory)
                 downloaded_bytes -= initial_size_bytes
                 pbar.n = min(
                     downloaded_bytes, total_size_bytes
                 )  # Prevent the progress bar from exceeding 100%
                 pbar.refresh()
 
                 if process.poll() is not None:
@@ -825,14 +817,29 @@
             _, stderr = process.communicate()
             pbar.close()
 
         else:
             while process.poll() is None:
                 time.sleep(0.5)
 
+    @staticmethod
+    def _get_dir_sum_file_size(directory) -> int:
+        path = Path(directory)
+        sum_file_size = 0
+        if path.exists() and path.is_dir():
+            for f in path.iterdir():
+                if f.is_file():
+                    try:
+                        sum_file_size += f.stat().st_size
+                    except FileNotFoundError:
+                        # file must have been removed before we
+                        # could get its size
+                        pass
+        return sum_file_size
+
     def _parse_s5cmd_sync_output_and_generate_synced_manifest(
         self, stdout, downloadDir, dirTemplate
     ) -> Path:
         """
         Parse the output of s5cmd sync --dry-run to extract distinct folders and generate a synced manifest.
 
         Args:
@@ -1286,14 +1293,17 @@
                         citations.append(response.json())
                     else:
                         citations.append(response.text)
                     logger.debug("Received citation: " + citations[-1])
 
                 else:
                     logger.error(f"Failed to get citation for DOI: {url}")
+                    logger.error(
+                        f"DOI server response status code: {response.status_code}"
+                    )
 
         return citations
 
     def download_from_selection(
         self,
         downloadDir,
         dry_run=False,
```

### Comparing `idc_index-0.5.7/tests/idcindex.py` & `idc_index-0.5.8/tests/idcindex.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 import os
 import tempfile
 import unittest
 from itertools import product
 
 import pandas as pd
 import pytest
-from idc_index import index
+from click.testing import CliRunner
+from idc_index import cli, index
 
 # Run tests using the following command from the root of the repository:
 # python -m unittest -vv tests/idcindex.py
 
-logging.basicConfig(level=logging.INFO)
+logging.basicConfig(level=logging.DEBUG)
 
 
 @pytest.fixture(autouse=True)
 def _change_test_dir(request, monkeypatch):
     monkeypatch.chdir(request.fspath.dirname)
 
 
 class TestIDCClient(unittest.TestCase):
     def setUp(self):
         self.client = index.IDCClient()
+        self.download_from_manifest = cli.download_from_manifest
+        self.download_from_selection = cli.download_from_selection
 
         logger = logging.getLogger("idc_index")
         logger.setLevel(logging.DEBUG)
 
     def test_get_collections(self):
         collections = self.client.get_collections()
         self.assertIsNotNone(collections)
@@ -347,14 +350,16 @@
                     validate_manifest=validate_manifest,
                     show_progress_bar=show_progress_bar,
                     use_s5cmd_sync=use_s5cmd_sync,
                 )
 
                 self.assertEqual(len(os.listdir(temp_dir)), 0)
 
+    """
+    disabling these tests due to a consistent server timeout issue
     def test_citations(self):
         citations = self.client.citations_from_selection(
             collection_id="tcga_gbm",
             citation_format=index.IDCClient.CITATION_FORMAT_APA,
         )
         self.assertIsNotNone(citations)
 
@@ -368,11 +373,54 @@
             studyInstanceUID="1.2.840.113654.2.55.174144834924218414213677353968537663991",
             citation_format=index.IDCClient.CITATION_FORMAT_BIBTEX,
         )
         self.assertIsNotNone(citations)
 
         citations = self.client.citations_from_manifest("./study_manifest_aws.s5cmd")
         self.assertIsNotNone(citations)
+    """
+
+    def test_cli_download_from_selection(self):
+        runner = CliRunner()
+        with tempfile.TemporaryDirectory() as temp_dir:
+            result = runner.invoke(
+                self.download_from_selection,
+                [
+                    "--download-dir",
+                    temp_dir,
+                    "--dry-run",
+                    False,
+                    "--quiet",
+                    True,
+                    "--show-progress-bar",
+                    True,
+                    "--use-s5cmd-sync",
+                    False,
+                    "--study-instance-uid",
+                    "1.3.6.1.4.1.14519.5.2.1.7695.1700.114861588187429958687900856462",
+                ],
+            )
+            assert len(os.listdir(temp_dir)) != 0
+
+    def test_cli_download_from_manifest(self):
+        runner = CliRunner()
+        with tempfile.TemporaryDirectory() as temp_dir:
+            result = runner.invoke(
+                self.download_from_manifest,
+                [
+                    "--manifest-file",
+                    "./study_manifest_aws.s5cmd",
+                    "--download-dir",
+                    temp_dir,
+                    "--quiet",
+                    True,
+                    "--show-progress-bar",
+                    True,
+                    "--use-s5cmd-sync",
+                    False,
+                ],
+            )
+            assert len(os.listdir(temp_dir)) != 0
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `idc_index-0.5.7/.gitignore` & `idc_index-0.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/LICENSE` & `idc_index-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.7/README.md` & `idc_index-0.5.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,73 +17,78 @@
 > about it by opening issues in this repository, or by starting a discussion in
 > [IDC User forum](https://discourse.canceridc.dev/).
 
 <!-- SPHINX-START -->
 
 ## About
 
-`idc-index` is a Python package that enables query of the basic metadata and
-download of DICOM files hosted by the
-[NCI Imaging Data Commons (IDC)](https://imaging.datacommons.cancer.gov).
+`idc-index` is a Python package that enables basic operations for working with
+[NCI Imaging Data Commons (IDC)](https://imaging.datacommons.cancer.gov):
 
-## Usage
+- subsetting of the IDC data using selected metadata attributes
+- download of the files corresponding to selection
+- generation of the viewer URLs for the selected data
 
-There are no prerequisites - just install the package ...
+## Getting started
+
+Install the latest version of the package.
 
 ```bash
-$ pip install idc-index
+$ pip install --upgrade idc-index
 ```
 
-... and download files corresponding to any collection, DICOM
-PatientID/Study/Series as follows:
+Instantiate `IDCClient`, which provides the interface for main operations.
 
 ```python
 from idc_index import index
 
 client = index.IDCClient()
+```
 
-all_collection_ids = client.get_collections()
+You can use [IDC Portal](https://imaging.datacommons.cancer.gov/explore) to
+browse collections, cases, studies and series, copy their identifiers and
+download the corresponding files using `idc-index` helper functions.
 
-client.download_from_selection(collection_id="rider_pilot", downloadDir="/some/dir")
+You can try this out with the `rider_pilot` collection, which is just 10.5 GB in
+size:
+
+```
+client.download_from_selection(collection_id="rider_pilot", downloadDir=".")
 ```
 
-... or run queries against the "mini" index of Imaging Data Commons data!
+... or run queries against the "mini" index of Imaging Data Commons data, and
+download images that match your selection criteria! The following will select
+all Magnetic Resonance (MR) series, and will download the first 10.
 
 ```python
 from idc_index import index
 
 client = index.IDCClient()
 
 query = """
 SELECT
-  collection_id,
-  STRING_AGG(DISTINCT(Modality)) as modalities,
-  STRING_AGG(DISTINCT(BodyPartExamined)) as body_parts
+  SeriesInstanceUID
 FROM
   index
-GROUP BY
-  collection_id
-ORDER BY
-  collection_id ASC
+WHERE
+  Modality = 'MR'
 """
 
-client.sql_query(query)
-```
+selection_df = client.sql_query(query)
 
-Details of the attributes included in the index are in the release notes.
+client.download_from_selection(
+    seriesInstanceUID=selection_df["SeriesInstanceUID"].values[:10], downloadDir="."
+)
+```
 
 ## Tutorial
 
-This package was first presented at the 2023 Annual meeting of Radiological
-Society of North America (RSNA) Deep Learning Lab
-[IDC session](https://github.com/RSNA/AI-Deep-Learning-Lab-2023/tree/main/sessions/idc).
-
 Please check out
 [this tutorial notebook](https://github.com/ImagingDataCommons/IDC-Tutorials/blob/master/notebooks/labs/idc_rsna2023.ipynb)
-for the introduction into using `idc-index` for navigating IDC data.
+for the introduction into using `idc-index`.
 
 ## Resources
 
 - [Imaging Data Commons Portal](https://imaging.datacommons.cancer.gov/) can be
   used to explore the content of IDC from the web browser
 - [s5cmd](https://github.com/peak/s5cmd) is a highly efficient, open source,
   multi-platform S3 client that we use for downloading IDC data, which is hosted
```

### Comparing `idc_index-0.5.7/pyproject.toml` & `idc_index-0.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
+  "click",
   'duckdb>=0.10.0',
   "idc-index-data==18.0.1",
   "packaging",
   "pandas<2.2",
   "psutil",
   "pyarrow",
   "requests",
@@ -56,14 +57,17 @@
   "sphinx>=7.0",
   "myst_parser>=0.13",
   "sphinx_copybutton",
   "sphinx_autodoc_typehints",
   "furo>=2023.08.17",
 ]
 
+[project.scripts]
+idc = 'idc_index.cli:main'
+
 [project.urls]
 Homepage = "https://github.com/ImagingDataCommons/idc-index"
 "Bug Tracker" = "https://github.com/ImagingDataCommons/idc-index/issues"
 Discussions = "https://discourse.canceridc.dev/"
 Changelog = "https://github.com/ImagingDataCommons/idc-index/releases"
```

### Comparing `idc_index-0.5.7/PKG-INFO` & `idc_index-0.5.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.5.7
+Version: 0.5.8
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
@@ -41,14 +41,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
+Requires-Dist: click
 Requires-Dist: duckdb>=0.10.0
 Requires-Dist: idc-index-data==18.0.1
 Requires-Dist: packaging
 Requires-Dist: pandas<2.2
 Requires-Dist: psutil
 Requires-Dist: pyarrow
 Requires-Dist: requests
@@ -87,73 +88,78 @@
 > about it by opening issues in this repository, or by starting a discussion in
 > [IDC User forum](https://discourse.canceridc.dev/).
 
 <!-- SPHINX-START -->
 
 ## About
 
-`idc-index` is a Python package that enables query of the basic metadata and
-download of DICOM files hosted by the
-[NCI Imaging Data Commons (IDC)](https://imaging.datacommons.cancer.gov).
+`idc-index` is a Python package that enables basic operations for working with
+[NCI Imaging Data Commons (IDC)](https://imaging.datacommons.cancer.gov):
 
-## Usage
+- subsetting of the IDC data using selected metadata attributes
+- download of the files corresponding to selection
+- generation of the viewer URLs for the selected data
 
-There are no prerequisites - just install the package ...
+## Getting started
+
+Install the latest version of the package.
 
 ```bash
-$ pip install idc-index
+$ pip install --upgrade idc-index
 ```
 
-... and download files corresponding to any collection, DICOM
-PatientID/Study/Series as follows:
+Instantiate `IDCClient`, which provides the interface for main operations.
 
 ```python
 from idc_index import index
 
 client = index.IDCClient()
+```
 
-all_collection_ids = client.get_collections()
+You can use [IDC Portal](https://imaging.datacommons.cancer.gov/explore) to
+browse collections, cases, studies and series, copy their identifiers and
+download the corresponding files using `idc-index` helper functions.
 
-client.download_from_selection(collection_id="rider_pilot", downloadDir="/some/dir")
+You can try this out with the `rider_pilot` collection, which is just 10.5 GB in
+size:
+
+```
+client.download_from_selection(collection_id="rider_pilot", downloadDir=".")
 ```
 
-... or run queries against the "mini" index of Imaging Data Commons data!
+... or run queries against the "mini" index of Imaging Data Commons data, and
+download images that match your selection criteria! The following will select
+all Magnetic Resonance (MR) series, and will download the first 10.
 
 ```python
 from idc_index import index
 
 client = index.IDCClient()
 
 query = """
 SELECT
-  collection_id,
-  STRING_AGG(DISTINCT(Modality)) as modalities,
-  STRING_AGG(DISTINCT(BodyPartExamined)) as body_parts
+  SeriesInstanceUID
 FROM
   index
-GROUP BY
-  collection_id
-ORDER BY
-  collection_id ASC
+WHERE
+  Modality = 'MR'
 """
 
-client.sql_query(query)
-```
+selection_df = client.sql_query(query)
 
-Details of the attributes included in the index are in the release notes.
+client.download_from_selection(
+    seriesInstanceUID=selection_df["SeriesInstanceUID"].values[:10], downloadDir="."
+)
+```
 
 ## Tutorial
 
-This package was first presented at the 2023 Annual meeting of Radiological
-Society of North America (RSNA) Deep Learning Lab
-[IDC session](https://github.com/RSNA/AI-Deep-Learning-Lab-2023/tree/main/sessions/idc).
-
 Please check out
 [this tutorial notebook](https://github.com/ImagingDataCommons/IDC-Tutorials/blob/master/notebooks/labs/idc_rsna2023.ipynb)
-for the introduction into using `idc-index` for navigating IDC data.
+for the introduction into using `idc-index`.
 
 ## Resources
 
 - [Imaging Data Commons Portal](https://imaging.datacommons.cancer.gov/) can be
   used to explore the content of IDC from the web browser
 - [s5cmd](https://github.com/peak/s5cmd) is a highly efficient, open source,
   multi-platform S3 client that we use for downloading IDC data, which is hosted
```

