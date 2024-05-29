# Comparing `tmp/behaverse-0.0.6.dev2.tar.gz` & `tmp/behaverse-0.0.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behaverse-0.0.6.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "behaverse-0.0.7.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `behaverse-0.0.6.dev2.tar` & `behaverse-0.0.7.dev1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1781 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.github/workflows/docs-publish.yml
--rw-r--r--   0        0        0     1243 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      160 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.gitignore
--rw-r--r--   0        0        0      158 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.pypirc
--rw-r--r--   0        0        0      375 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/LICENSE
--rw-r--r--   0        0        0      984 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/README.md
--rw-r--r--   0        0        0       54 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/.gitignore
--rw-r--r--   0        0        0       22 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0        0        0      126 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0        0        0     6853 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0        0        0     1366 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/_quarto.yml
--rw-r--r--   0        0        0     1222 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/getting_started.qmd
--rw-r--r--   0        0        0      261 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/index.qmd
--rw-r--r--   0        0        0     1255 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/system_design.qmd
--rw-r--r--   0        0        0      221 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/environment.yml
--rw-r--r--   0        0        0    10649 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/examples/1 Getting Started.ipynb
--rw-r--r--   0        0        0     1788 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/pyproject.toml
--rw-r--r--   0        0        0      494 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/__init__.py
--rw-r--r--   0        0        0      284 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/additional_storage/huggingface.py
--rw-r--r--   0        0        0      276 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/additional_storage/osf.py
--rw-r--r--   0        0        0      278 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/additional_storage/ulhpc.py
--rw-r--r--   0        0        0      279 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/additional_storage/zenodo.py
--rw-r--r--   0        0        0       27 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/conftest.py
--rw-r--r--   0        0        0     8702 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dataset.py
--rw-r--r--   0        0        0      238 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dataset_description.py
--rw-r--r--   0        0        0     1714 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dataset_test.py
--rw-r--r--   0        0        0     1619 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dvc_storage.py
--rw-r--r--   0        0        0      535 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dvc_storage_test.py
--rw-r--r--   0        0        0     2520 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/functional.py
--rw-r--r--   0        0        0       28 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/functions_test.py
--rw-r--r--   0        0        0     2571 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/http_storage.py
--rw-r--r--   0        0        0     1918 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/utils.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 behaverse-0.0.6.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1781 2024-05-28 12:05:34.561865 behaverse-0.0.7.dev1/.github/workflows/docs-publish.yml
+-rw-r--r--   0        0        0     1243 2024-05-28 12:05:34.561865 behaverse-0.0.7.dev1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      160 2024-05-28 12:05:34.561865 behaverse-0.0.7.dev1/.gitignore
+-rw-r--r--   0        0        0      158 2024-05-28 12:05:34.561865 behaverse-0.0.7.dev1/.pypirc
+-rw-r--r--   0        0        0      375 2024-05-28 12:05:34.561865 behaverse-0.0.7.dev1/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-05-28 12:05:34.561865 behaverse-0.0.7.dev1/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-28 12:05:34.561865 behaverse-0.0.7.dev1/README.md
+-rw-r--r--   0        0        0       54 2024-05-28 12:05:34.561865 behaverse-0.0.7.dev1/docs/.gitignore
+-rw-r--r--   0        0        0       22 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0        0        0      126 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0        0        0     6853 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0        0        0     1425 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/docs/_quarto.yml
+-rw-r--r--   0        0        0     1359 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/docs/getting_started.qmd
+-rw-r--r--   0        0        0      261 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/docs/index.qmd
+-rw-r--r--   0        0        0     1255 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/docs/system_design.qmd
+-rw-r--r--   0        0        0      221 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/environment.yml
+-rw-r--r--   0        0        0    10892 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/examples/1 Getting Started.ipynb
+-rw-r--r--   0        0        0     1788 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/conftest.py
+-rw-r--r--   0        0        0      471 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/__init__.py
+-rw-r--r--   0        0        0      284 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/additional_storage/huggingface.py
+-rw-r--r--   0        0        0      276 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/additional_storage/osf.py
+-rw-r--r--   0        0        0      278 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/additional_storage/ulhpc.py
+-rw-r--r--   0        0        0      279 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/additional_storage/zenodo.py
+-rw-r--r--   0        0        0     8713 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/dataset.py
+-rw-r--r--   0        0        0      519 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/dataset_description.py
+-rw-r--r--   0        0        0     1711 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/dataset_test.py
+-rw-r--r--   0        0        0     1619 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/dvc_storage.py
+-rw-r--r--   0        0        0      545 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/dvc_storage_test.py
+-rw-r--r--   0        0        0     2520 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/functional.py
+-rw-r--r--   0        0        0       28 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/functions_test.py
+-rw-r--r--   0        0        0     2571 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/http_storage.py
+-rw-r--r--   0        0        0     1918 2024-05-28 12:05:34.565865 behaverse-0.0.7.dev1/src/behaverse/data/utils.py
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 behaverse-0.0.7.dev1/PKG-INFO
```

### Comparing `behaverse-0.0.6.dev2/.github/workflows/docs-publish.yml` & `behaverse-0.0.7.dev1/.github/workflows/docs-publish.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/.github/workflows/pypi-publish.yml` & `behaverse-0.0.7.dev1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/LICENSE` & `behaverse-0.0.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/README.md` & `behaverse-0.0.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/docs/_extensions/machow/interlinks/interlinks.lua` & `behaverse-0.0.7.dev1/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/docs/_quarto.yml` & `behaverse-0.0.7.dev1/docs/_quarto.yml`

 * *Files 10% similar despite different names*

```diff
@@ -34,43 +34,43 @@
   - interlinks
 
 # tell quarto to read the generated sidebar
 metadata-files:
   - api/_sidebar.yml
 
 quartodoc:
-  package: behaverse
+  package: behaverse.data
   dir: api
   source_dir: ../src
   parser: 'google'
   title: "API"
   render_interlinks: true
 
   # # write sidebar data to this file
   sidebar: api/_sidebar.yml
 
   sections:
-  - title: Object-Oriented API
-    package: behaverse
+  - title: Behaverse Data (Object-Oriented API)
+    package: behaverse.data
     contents:
       - name: Dataset
         children: separate
         members:
           - open
           - where
           - describe
           - load
           - validate
       - name: DatasetDescription
         children: separate
-  - title: Functional API
-    package: behaverse
+  - title: Behaverse Data (Functional API)
+    package: behaverse.data
     contents:
       - list_datasets
       - open_dataset
       - load_dataset
       - describe_dataset
       - validate_dataset
-  - title: Utilities
-    package: behaverse.utils
+  - title: Data Utilities
+    package: behaverse.data.utils
     contents:
       - extract_dataset
```

### Comparing `behaverse-0.0.6.dev2/docs/getting_started.qmd` & `behaverse-0.0.7.dev1/docs/getting_started.qmd`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,38 @@
 execute:
   echo: true
 jupyter: python3
 ---
 
 # Getting Started
 
-To access datasets via the API, you first need to install the `behaverse` Python package. You can do this by running the following command:
+Make sure you have Python 3.10 or later installed on your system. We recommend using a virtual environment such as Mamba to manage your dependencies.
+
+You first need to install the `behaverse` Python package. You can do this by running the following command:
 
 ```bash
 pip install -U behaverse
 ```
 
-Make sure you have Python 3.10 or later installed on your system. We recommend using a virtual environment such as Mamba to manage your dependencies.
+Or if you prefer Conda/Mamba, you can add the following to your `environment.yml` file:
 
+```yaml
+dependencies:
+  - python>3.10
+  - pip
+  - pip:
+    - behaverse
+```
 
 # Usage
 
 The `behaverse` package provides a simple API to access datasets. You can use the `behaverse` package to download datasets, load them into memory, and access the data. Here is an example of how to use the package to list available datasets, download a dataset, select a subset of the dataset, and load it into memory:
 
 ```{python}
-from behaverse import list_datasets, download_dataset, load_dataset, open_dataset, describe_dataset
+from behaverse.data import list_datasets, download_dataset, load_dataset, open_dataset, describe_dataset
 from IPython.display import display
 
 # List available datasets
 display(list_datasets())
 
 # Open a dataset, select a subset of the data, and load it into memory
 dataset = open_dataset('P500_9subjects/L1m').where(subject_id=['001', '002']).load()
```

### Comparing `behaverse-0.0.6.dev2/docs/system_design.qmd` & `behaverse-0.0.7.dev1/docs/system_design.qmd`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/examples/1 Getting Started.ipynb` & `behaverse-0.0.7.dev1/examples/1 Getting Started.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9890003551136364%*

 * *Differences: {"'cells'": "{1: {'outputs': [], 'source': {insert: [(3, 'from behaverse.data import "*

 * *            "open_dataset')], delete: [3]}}, 3: {'execution_count': 2, 'outputs': {2: "*

 * *            "{'output_type': 'display_data', 'data': "*

 * *            "OrderedDict([('application/vnd.jupyter.widget-view+json', OrderedDict([('model_id', "*

 * *            "'768f0dd911274d9b9f6ed11af7938e35'), ('version_major', 2), ('version_minor', 0)])), "*

 * *            "('text/plain', ['Loading options:   0%|          | 0/282 [00:00<?, ?it/ […]*

```diff
@@ -13,57 +13,81 @@
                 "```\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/home/morteza/miniforge3/envs/behaverse/lib/python3.12/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html\n",
-                        "  from .autonotebook import tqdm as notebook_tqdm\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "%reload_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
-                "from behaverse import open_dataset"
+                "from behaverse.data import open_dataset"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now, we open the dataset, select a subset of the data, and then load the data into memory.\n",
                 "\n",
                 "For the two selected subjects, it may take a few minutes to download the dataset and then a few seconds to load the subset of data. Downloading the dataset is a one-time process."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {
                 "notebookRunGroups": {
                     "groupValue": "3"
                 }
             },
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Loading responses: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 282/282 [00:01<00:00, 146.36it/s]\n",
-                        "Loading stimuli: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 282/282 [00:00<00:00, 505.99it/s]\n",
-                        "Loading options: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 282/282 [00:00<00:00, 491.49it/s]\n"
-                    ]
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "38b5a1e0fe0541c5a8b179a5f8266615",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Loading responses:   0%|          | 0/282 [00:00<?, ?it/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "bb3f2cb0470b45a7a6628aaf7201ba32",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Loading stimuli:   0%|          | 0/282 [00:00<?, ?it/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "768f0dd911274d9b9f6ed11af7938e35",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Loading options:   0%|          | 0/282 [00:00<?, ?it/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
@@ -266,24 +290,22 @@
                             "2   NaN NaN         NaN         NaN  \n",
                             "3   NaN NaN         NaN         NaN  \n",
                             "4   NaN NaN         NaN         NaN  \n",
                             "\n",
                             "[5 rows x 67 columns]"
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "selected_subject_ids = ['001', '002']\n",
-                "\n",
                 "dataset = (open_dataset('P500_9subjects/L1m')\n",
-                "           .where(subject_id=selected_subject_ids)\n",
+                "           .where(subject_id=['001', '002'])\n",
                 "           .load()\n",
                 ")\n",
                 "\n",
                 "dataset.response_table.head()\n",
                 "# dataset.stimulus_table\n",
                 "# dataset.option_table"
             ]
```

### Comparing `behaverse-0.0.6.dev2/pyproject.toml` & `behaverse-0.0.7.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/src/behaverse/dataset.py` & `behaverse-0.0.7.dev1/src/behaverse/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 
         self.option_table = pd.concat(option_dfs, axis=0, ignore_index=True)
         # !SECTION option table
 
         return self
 
     @classmethod
-    def open(cls, name: str, download: bool = True, storage: str='http') -> 'Dataset':
+    def open(cls, name: str, download: bool = True, storage: str = 'http') -> 'Dataset':
         """Open the dataset with the given name, and optionally download it if it does not exist.
 
         Args:
             name: Name of the dataset to open.
             download: whether to download the dataset if it does not exist.
             storage: storage backend to use (`http` or `dvc`). Defaults to 'http'.
 
@@ -209,15 +209,15 @@
             download_dataset(name)
 
         return cls(name, allow_instantiation=True)
 
     def describe(self) -> DatasetDescription:
         """Provides metadata and information card for the dataset."""
         # TODO add dataset-level attributes
-        description = DatasetDescription()
+        description = DatasetDescription(self.name)
         return description
 
     def validate(self) -> bool:
         """Simple validations to check if the dataset is valid and consistent.
 
         :::{.callout-note}
```

### Comparing `behaverse-0.0.6.dev2/src/behaverse/dataset_test.py` & `behaverse-0.0.7.dev1/src/behaverse/data/dataset_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,8 @@
     dataset = Dataset.open('P500_9subjects/L1m').where(subject_id=subject_ids).load()
 
     assert dataset.name == 'P500_9subjects/L1m'
     assert len(dataset.subjects) == len(subject_ids)
     assert len(dataset.study_flow.subject_id.unique()) == len(subject_ids)
 
     # FIXME subject_index in response table must be renamed to subject_id
-    assert len(dataset.response_table['subject_index'].unique()) == len(subject_ids)
+    assert len(dataset.response_table['subject_id'].unique()) == len(subject_ids)
```

### Comparing `behaverse-0.0.6.dev2/src/behaverse/dvc_storage.py` & `behaverse-0.0.7.dev1/src/behaverse/data/dvc_storage.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/src/behaverse/dvc_storage_test.py` & `behaverse-0.0.7.dev1/src/behaverse/data/dvc_storage_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Test for dvc_storage.py module."""
 
 
 def test_download_dataset_functional():
     """Test functional download method."""
-    from behaverse.dvc_storage import download_dataset
+    from behaverse.data.dvc_storage import download_dataset
     path = download_dataset('P500_9subjects/L1m')
 
     assert path.exists()
     assert path.is_dir()
     assert path.stem == 'L1m'
 
 
 def test_download_dataset_oop():
     """Test object-oriented download method."""
-    from behaverse import Dataset
+    from behaverse.data import Dataset
     dataset = Dataset.open('P500_9subjects/L1m', download=True, storage='dvc')
     assert dataset.validate()
```

### Comparing `behaverse-0.0.6.dev2/src/behaverse/functional.py` & `behaverse-0.0.7.dev1/src/behaverse/data/functional.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/src/behaverse/http_storage.py` & `behaverse-0.0.7.dev1/src/behaverse/data/http_storage.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/src/behaverse/utils.py` & `behaverse-0.0.7.dev1/src/behaverse/data/utils.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev2/PKG-INFO` & `behaverse-0.0.7.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: behaverse
-Version: 0.0.6.dev2
-Summary: Behaverse Python Package.
+Version: 0.0.7.dev1
+Summary: Behaverse package.
 Author-email: xCIT Development Team <contact@xcit.org>
 Maintainer-email: Morteza Ansarinia <ansarinia@me.com>, Hoorieh Afkari <hoorieh.afkari@uni.lu>, Pedro Cardoso-Leite <pedro.cardosoleite@uni.lu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

