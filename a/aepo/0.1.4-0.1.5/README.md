# Comparing `tmp/aepo-0.1.4.tar.gz` & `tmp/aepo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepo-0.1.4.tar", max compression
+gzip compressed data, was "aepo-0.1.5.tar", max compression
```

## Comparing `aepo-0.1.4.tar` & `aepo-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rwxr-xr-x   0        0        0     1074 2024-05-13 01:25:24.936000 aepo-0.1.4/LICENSE
--rwxr-xr-x   0        0        0     3245 2024-05-13 07:13:07.938000 aepo-0.1.4/README.md
--rwxr-xr-x   0        0        0      638 2024-05-15 08:48:40.706000 aepo-0.1.4/aepo/Makefile
--rwxr-xr-x   0        0        0       22 2024-05-13 06:47:12.539000 aepo-0.1.4/aepo/__init__.py
--rwxr-xr-x   0        0        0     6613 2024-05-15 10:09:17.525000 aepo-0.1.4/aepo/cli.py
--rwxr-xr-x   0        0        0      804 2024-05-15 08:48:40.721000 aepo-0.1.4/aepo/make.bat
--rwxr-xr-x   0        0        0        0 2024-05-13 01:21:42.945000 aepo-0.1.4/aepo/mbr/__init__.py
--rwxr-xr-x   0        0        0      144 2024-05-15 08:55:14.869000 aepo-0.1.4/aepo/mbr/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2833 2024-05-15 09:06:06.113000 aepo-0.1.4/aepo/mbr/__pycache__/mbr_engine.cpython-310.pyc
--rwxr-xr-x   0        0        0     2792 2024-05-15 09:06:12.067000 aepo-0.1.4/aepo/mbr/__pycache__/reward_engine.cpython-310.pyc
--rwxr-xr-x   0        0        0    11661 2024-05-15 09:06:14.176000 aepo-0.1.4/aepo/mbr/__pycache__/reward_model.cpython-310.pyc
--rwxr-xr-x   0        0        0     3011 2024-05-15 09:06:08.087000 aepo-0.1.4/aepo/mbr/__pycache__/utility_func.cpython-310.pyc
--rwxr-xr-x   0        0        0     2997 2024-05-15 09:01:40.322000 aepo-0.1.4/aepo/mbr/mbr_engine.py
--rwxr-xr-x   0        0        0        0 2024-05-13 01:21:43.086000 aepo-0.1.4/aepo/mbr/policy/__init__.py
--rwxr-xr-x   0        0        0      151 2024-05-15 08:55:21.386000 aepo-0.1.4/aepo/mbr/policy/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4244 2024-05-15 08:55:21.532000 aepo-0.1.4/aepo/mbr/policy/__pycache__/diverse_mbr.cpython-310.pyc
--rwxr-xr-x   0        0        0     1910 2024-05-15 09:06:10.053000 aepo-0.1.4/aepo/mbr/policy/__pycache__/mbr.cpython-310.pyc
--rwxr-xr-x   0        0        0     4828 2024-05-15 08:36:55.367000 aepo-0.1.4/aepo/mbr/policy/diverse_mbr.py
--rwxr-xr-x   0        0        0     2040 2024-05-15 09:00:10.253000 aepo-0.1.4/aepo/mbr/policy/mbr.py
--rwxr-xr-x   0        0        0     2728 2024-05-15 09:04:05.830000 aepo-0.1.4/aepo/mbr/reward_engine.py
--rwxr-xr-x   0        0        0    12493 2024-05-15 09:04:19.342000 aepo-0.1.4/aepo/mbr/reward_model.py
--rwxr-xr-x   0        0        0     8001 2024-05-15 09:05:33.205000 aepo-0.1.4/aepo/mbr/utility_func.py
--rwxr-xr-x   0        0        0     2656 2024-05-15 08:39:32.300000 aepo-0.1.4/aepo/preprocess.py
--rwxr-xr-x   0        0        0      712 2024-05-22 02:31:53.761000 aepo-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4309 2024-05-22 02:32:11.631355 aepo-0.1.4/setup.py
--rw-r--r--   0        0        0     4184 2024-05-22 02:32:11.632192 aepo-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-05-13 01:25:24.936000 aepo-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0     3875 2024-05-29 12:53:13.100000 aepo-0.1.5/README.md
+-rwxr-xr-x   0        0        0      638 2024-05-15 08:48:40.716000 aepo-0.1.5/aepo/Makefile
+-rwxr-xr-x   0        0        0       22 2024-05-13 06:47:06.243000 aepo-0.1.5/aepo/__init__.py
+-rwxr-xr-x   0        0        0     6613 2024-05-15 10:09:09.810000 aepo-0.1.5/aepo/cli.py
+-rwxr-xr-x   0        0        0      804 2024-05-15 08:48:40.731000 aepo-0.1.5/aepo/make.bat
+-rwxr-xr-x   0        0        0        0 2024-05-13 01:21:42.945000 aepo-0.1.5/aepo/mbr/__init__.py
+-rwxr-xr-x   0        0        0      144 2024-05-15 08:55:14.860000 aepo-0.1.5/aepo/mbr/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2833 2024-05-15 09:05:56.140000 aepo-0.1.5/aepo/mbr/__pycache__/mbr_engine.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2792 2024-05-15 09:05:59.908000 aepo-0.1.5/aepo/mbr/__pycache__/reward_engine.cpython-310.pyc
+-rwxr-xr-x   0        0        0    11661 2024-05-15 09:05:59.973000 aepo-0.1.5/aepo/mbr/__pycache__/reward_model.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3011 2024-05-15 09:05:57.218000 aepo-0.1.5/aepo/mbr/__pycache__/utility_func.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2997 2024-05-15 09:01:33.636000 aepo-0.1.5/aepo/mbr/mbr_engine.py
+-rwxr-xr-x   0        0        0        0 2024-05-13 01:21:43.086000 aepo-0.1.5/aepo/mbr/policy/__init__.py
+-rwxr-xr-x   0        0        0      151 2024-05-15 08:55:21.375000 aepo-0.1.5/aepo/mbr/policy/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4244 2024-05-15 08:55:21.521000 aepo-0.1.5/aepo/mbr/policy/__pycache__/diverse_mbr.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1910 2024-05-15 09:05:59.814000 aepo-0.1.5/aepo/mbr/policy/__pycache__/mbr.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4828 2024-05-15 08:36:47.107000 aepo-0.1.5/aepo/mbr/policy/diverse_mbr.py
+-rwxr-xr-x   0        0        0     2040 2024-05-15 09:00:03.657000 aepo-0.1.5/aepo/mbr/policy/mbr.py
+-rwxr-xr-x   0        0        0     2728 2024-05-15 09:03:59.289000 aepo-0.1.5/aepo/mbr/reward_engine.py
+-rwxr-xr-x   0        0        0    12493 2024-05-15 09:04:12.762000 aepo-0.1.5/aepo/mbr/reward_model.py
+-rwxr-xr-x   0        0        0     8001 2024-05-15 09:05:26.497000 aepo-0.1.5/aepo/mbr/utility_func.py
+-rwxr-xr-x   0        0        0     2656 2024-05-15 08:39:25.164000 aepo-0.1.5/aepo/preprocess.py
+-rwxr-xr-x   0        0        0      712 2024-05-29 12:49:00.942000 aepo-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 aepo-0.1.5/PKG-INFO
```

### Comparing `aepo-0.1.4/LICENSE` & `aepo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/README.md` & `aepo-0.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ## Annotation-Efficient Preference Optimization
 
-This repository implements the Annotation-Efficient Preference Optimization (AEPO) algorithm.
+![illustration](aepo.png)
+
+This repository implements the [Annotation-Efficient Preference Optimization (AEPO) algorithm](https://arxiv.org/abs/2405.13541).
 
 The code is tested on Ubuntu 20.04 using Python 3.9 and CUDA 11.0 (Docker image nvidia/cuda:11.0.3-cudnn8-devel-ubuntu20.04).
 
 ## Install
 
 You can install aepo via pip.
 ```
@@ -64,11 +66,28 @@
 ```
 
 This will pick the best and worst responses as the chosen and rejected. The rest of the responses are discarded.
 It would be useful to construct a pairwise preference dataset.
 
 ## Reference
 
-TBA. Yuu Jinnai and Honda Ukyo. Annotation-Efficient Preference Optimization for Language Model Alignment, 2024.
+[Jinnai, Y., Honda, U. (2024). Annotation-Efficient Preference Optimization for Language Model Alignment. arXiv preprint arXiv:2405.13541.](https://arxiv.org/abs/2405.13541)
+
+
+Bibtex:
+
+```
+@misc{jinnai2024annotationefficient,
+      title={Annotation-Efficient Preference Optimization for Language Model Alignment}, 
+      author={Yuu Jinnai and Ukyo Honda},
+      year={2024},
+      eprint={2405.13541},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
 
 ## Contact
 For any questions, feel free to raise an issue or contact me at jinnai_yu@cyberagent.co.jp.
+
+## Acknowledgements
+[AlpacaFarm dataset](https://github.com/tatsu-lab/alpaca_farm) is licensed under [Attribution-NonCommercial 4.0 International](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE).
```

### Comparing `aepo-0.1.4/aepo/Makefile` & `aepo-0.1.5/aepo/Makefile`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/cli.py` & `aepo-0.1.5/aepo/cli.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/make.bat` & `aepo-0.1.5/aepo/make.bat`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/__pycache__/mbr_engine.cpython-310.pyc` & `aepo-0.1.5/aepo/mbr/__pycache__/mbr_engine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/__pycache__/reward_engine.cpython-310.pyc` & `aepo-0.1.5/aepo/mbr/__pycache__/reward_engine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/__pycache__/reward_model.cpython-310.pyc` & `aepo-0.1.5/aepo/mbr/__pycache__/reward_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/__pycache__/utility_func.cpython-310.pyc` & `aepo-0.1.5/aepo/mbr/__pycache__/utility_func.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/mbr_engine.py` & `aepo-0.1.5/aepo/mbr/mbr_engine.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/policy/__pycache__/diverse_mbr.cpython-310.pyc` & `aepo-0.1.5/aepo/mbr/policy/__pycache__/diverse_mbr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/policy/__pycache__/mbr.cpython-310.pyc` & `aepo-0.1.5/aepo/mbr/policy/__pycache__/mbr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/policy/diverse_mbr.py` & `aepo-0.1.5/aepo/mbr/policy/diverse_mbr.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/policy/mbr.py` & `aepo-0.1.5/aepo/mbr/policy/mbr.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/reward_engine.py` & `aepo-0.1.5/aepo/mbr/reward_engine.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/reward_model.py` & `aepo-0.1.5/aepo/mbr/reward_model.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/mbr/utility_func.py` & `aepo-0.1.5/aepo/mbr/utility_func.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/aepo/preprocess.py` & `aepo-0.1.5/aepo/preprocess.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.4/pyproject.toml` & `aepo-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aepo"
-version = "0.1.4"
+version = "0.1.5"
 description = "Annotation Efficient Preference Optimization"
 authors = ["Yuu Jinnai <ddyuudd@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/CyberAgentAILab/annotation-efficient-po"
 documentation = "https://CyberAgentAILab.github.io/annotation-efficient-po"
 
 [tool.poetry.dependencies]
```

### Comparing `aepo-0.1.4/setup.py` & `aepo-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,118 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aepo
+Version: 0.1.5
+Summary: Annotation Efficient Preference Optimization
+Home-page: https://github.com/CyberAgentAILab/annotation-efficient-po
+Author: Yuu Jinnai
+Author-email: ddyuudd@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: datasets (>=2.10.0,<3.0.0)
+Requires-Dist: evaluate (>=0.4.2,<0.5.0)
+Requires-Dist: llm-blender (>=0.0.2,<0.0.3)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: torch (>=2.3.0,<3.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
+Requires-Dist: transformers (>=4.40.2,<5.0.0)
+Project-URL: Documentation, https://CyberAgentAILab.github.io/annotation-efficient-po
+Project-URL: Repository, https://github.com/CyberAgentAILab/annotation-efficient-po
+Description-Content-Type: text/markdown
 
-packages = \
-['aepo', 'aepo.mbr', 'aepo.mbr.policy']
+## Annotation-Efficient Preference Optimization
 
-package_data = \
-{'': ['*']}
+![illustration](aepo.png)
 
-install_requires = \
-['datasets>=2.10.0,<3.0.0',
- 'evaluate>=0.4.2,<0.5.0',
- 'llm-blender>=0.0.2,<0.0.3',
- 'numpy>=1.26.4,<2.0.0',
- 'pandas>=2.0.0,<3.0.0',
- 'torch>=2.3.0,<3.0.0',
- 'tqdm>=4.66.4,<5.0.0',
- 'transformers>=4.40.2,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['aepo = aepo.cli:aepo']}
-
-setup_kwargs = {
-    'name': 'aepo',
-    'version': '0.1.4',
-    'description': 'Annotation Efficient Preference Optimization',
-    'long_description': '## Annotation-Efficient Preference Optimization\n\nThis repository implements the Annotation-Efficient Preference Optimization (AEPO) algorithm.\n\nThe code is tested on Ubuntu 20.04 using Python 3.9 and CUDA 11.0 (Docker image nvidia/cuda:11.0.3-cudnn8-devel-ubuntu20.04).\n\n## Install\n\nYou can install aepo via pip.\n```\npip install aepo\n```\n\nSource install is available too. Clone this repository and run `pip install .`.\n```\ngit clone git@github.com:CyberAgentAILab/annotation-efficient-po.git\ncd annotation-efficient-po\npip install .\n```\n\n\n## Usage\n\nThe command line interface is available.\nThe input dataset can be csv file or a dataset uploaded to Huggingface Hub.\nThe dataset should have a column named *prompt* or *instruction*. aepo recognize it as the user prompt given to the system and the rest of the columns to be the responses generated by the system.\n\nI prepared an example dataset in `dataset/alpaca_samples.csv`.\nThe csv file includes 128 responses generated by [HuggingFaceH4/mistral-7b-sft-beta](https://huggingface.co/HuggingFaceH4/mistral-7b-sft-beta) for each instruction of the `alpaca_human_preference` split of [tatsu-lab/alpaca_farm](https://huggingface.co/datasets/tatsu-lab/alpaca_eval).\nYou can try aepo using this dataset with the following command:\n\n```\naepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 2 --num_instructions 10\n```\n\n`--num_responses` is the number of input responses you use. The dataset has to have responses larger than or equal to `--num_responses`. `--num_annotations` is the number of responses after the subsampling process. It is also the number of times the reward model is queried per instruction.\n\n### Example: Running AEPO\n\nYou can generate a pair of responses for each instruction using aepo using the following command.\n\n```\naepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 2 --num_instructions 10\n```\n\nTo subsample four responses for e.g., [LiPO](https://arxiv.org/abs/2402.01878v1), set `--num_annotations` to four.\n\n```\naepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 4 --num_instructions 10\n```\n\n### Example: Running West-of-N over 8 samples\n[West-of-N](https://arxiv.org/abs/2401.12086) is a strategy to pick the Best-of-N as the chosen response, and Worst-of-N as a rejected response. It is shown to be effective for DPO and reward modeling.\nYou can run West-of-N using this package by setting `--num_annotations` == `--num_responses`.\n\n```\naepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 8 --num_instructions 10\n```\n\nThis command will generate a dataset with 8 responses, ranked by their rewards. If you only need the best and worst of the N samples, then use `--west_of_n` option.\n\n```\naepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 8 --num_instructions 10 --west_of_n\n```\n\nThis will pick the best and worst responses as the chosen and rejected. The rest of the responses are discarded.\nIt would be useful to construct a pairwise preference dataset.\n\n## Reference\n\nTBA. Yuu Jinnai and Honda Ukyo. Annotation-Efficient Preference Optimization for Language Model Alignment, 2024.\n\n## Contact\nFor any questions, feel free to raise an issue or contact me at jinnai_yu@cyberagent.co.jp.\n',
-    'author': 'Yuu Jinnai',
-    'author_email': 'ddyuudd@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/CyberAgentAILab/annotation-efficient-po',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+This repository implements the [Annotation-Efficient Preference Optimization (AEPO) algorithm](https://arxiv.org/abs/2405.13541).
+
+The code is tested on Ubuntu 20.04 using Python 3.9 and CUDA 11.0 (Docker image nvidia/cuda:11.0.3-cudnn8-devel-ubuntu20.04).
+
+## Install
+
+You can install aepo via pip.
+```
+pip install aepo
+```
+
+Source install is available too. Clone this repository and run `pip install .`.
+```
+git clone git@github.com:CyberAgentAILab/annotation-efficient-po.git
+cd annotation-efficient-po
+pip install .
+```
+
+
+## Usage
+
+The command line interface is available.
+The input dataset can be csv file or a dataset uploaded to Huggingface Hub.
+The dataset should have a column named *prompt* or *instruction*. aepo recognize it as the user prompt given to the system and the rest of the columns to be the responses generated by the system.
+
+I prepared an example dataset in `dataset/alpaca_samples.csv`.
+The csv file includes 128 responses generated by [HuggingFaceH4/mistral-7b-sft-beta](https://huggingface.co/HuggingFaceH4/mistral-7b-sft-beta) for each instruction of the `alpaca_human_preference` split of [tatsu-lab/alpaca_farm](https://huggingface.co/datasets/tatsu-lab/alpaca_eval).
+You can try aepo using this dataset with the following command:
+
+```
+aepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 2 --num_instructions 10
+```
+
+`--num_responses` is the number of input responses you use. The dataset has to have responses larger than or equal to `--num_responses`. `--num_annotations` is the number of responses after the subsampling process. It is also the number of times the reward model is queried per instruction.
+
+### Example: Running AEPO
+
+You can generate a pair of responses for each instruction using aepo using the following command.
+
+```
+aepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 2 --num_instructions 10
+```
+
+To subsample four responses for e.g., [LiPO](https://arxiv.org/abs/2402.01878v1), set `--num_annotations` to four.
+
+```
+aepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 4 --num_instructions 10
+```
+
+### Example: Running West-of-N over 8 samples
+[West-of-N](https://arxiv.org/abs/2401.12086) is a strategy to pick the Best-of-N as the chosen response, and Worst-of-N as a rejected response. It is shown to be effective for DPO and reward modeling.
+You can run West-of-N using this package by setting `--num_annotations` == `--num_responses`.
+
+```
+aepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 8 --num_instructions 10
+```
+
+This command will generate a dataset with 8 responses, ranked by their rewards. If you only need the best and worst of the N samples, then use `--west_of_n` option.
+
+```
+aepo dataset/alpaca_samples.csv --num_responses 8 --num_annotations 8 --num_instructions 10 --west_of_n
+```
+
+This will pick the best and worst responses as the chosen and rejected. The rest of the responses are discarded.
+It would be useful to construct a pairwise preference dataset.
+
+## Reference
+
+[Jinnai, Y., Honda, U. (2024). Annotation-Efficient Preference Optimization for Language Model Alignment. arXiv preprint arXiv:2405.13541.](https://arxiv.org/abs/2405.13541)
+
+
+Bibtex:
+
+```
+@misc{jinnai2024annotationefficient,
+      title={Annotation-Efficient Preference Optimization for Language Model Alignment}, 
+      author={Yuu Jinnai and Ukyo Honda},
+      year={2024},
+      eprint={2405.13541},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
 }
+```
+
+## Contact
+For any questions, feel free to raise an issue or contact me at jinnai_yu@cyberagent.co.jp.
 
+## Acknowledgements
+[AlpacaFarm dataset](https://github.com/tatsu-lab/alpaca_farm) is licensed under [Attribution-NonCommercial 4.0 International](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE).
 
-setup(**setup_kwargs)
```

