# Comparing `tmp/angle_emb-0.4.3.tar.gz` & `tmp/angle_emb-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angle_emb-0.4.3.tar", last modified: Sun May 26 05:30:34 2024, max compression
+gzip compressed data, was "angle_emb-0.4.4.tar", last modified: Wed May 29 03:56:58 2024, max compression
```

## Comparing `angle_emb-0.4.3.tar` & `angle_emb-0.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-26 05:30:34.302784 angle_emb-0.4.3/
--rw-r--r--   0 seanlee    (501) staff       (20)     1061 2024-01-15 11:58:12.000000 angle_emb-0.4.3/LICENSE
--rw-r--r--   0 seanlee    (501) staff       (20)    17282 2024-05-26 05:30:34.303133 angle_emb-0.4.3/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)    16565 2024-05-25 02:28:23.000000 angle_emb-0.4.3/README.md
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-26 05:30:34.284288 angle_emb-0.4.3/angle_emb/
--rw-r--r--   0 seanlee    (501) staff       (20)       70 2024-05-26 05:29:29.000000 angle_emb-0.4.3/angle_emb/__init__.py
--rw-r--r--   0 seanlee    (501) staff       (20)    70613 2024-05-26 05:29:24.000000 angle_emb-0.4.3/angle_emb/angle.py
--rw-r--r--   0 seanlee    (501) staff       (20)    13833 2024-05-22 08:19:50.000000 angle_emb-0.4.3/angle_emb/angle_trainer.py
--rw-r--r--   0 seanlee    (501) staff       (20)      512 2024-05-21 09:01:40.000000 angle_emb-0.4.3/angle_emb/utils.py
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-26 05:30:34.302147 angle_emb-0.4.3/angle_emb.egg-info/
--rw-r--r--   0 seanlee    (501) staff       (20)    17282 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)      355 2024-05-26 05:30:34.000000 angle_emb-0.4.3/angle_emb.egg-info/SOURCES.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/dependency_links.txt
--rw-r--r--   0 seanlee    (501) staff       (20)       63 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/entry_points.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-01-15 12:03:51.000000 angle_emb-0.4.3/angle_emb.egg-info/not-zip-safe
--rw-r--r--   0 seanlee    (501) staff       (20)       87 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/requires.txt
--rw-r--r--   0 seanlee    (501) staff       (20)       10 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/top_level.txt
--rw-r--r--   0 seanlee    (501) staff       (20)      202 2024-05-26 05:30:34.306904 angle_emb-0.4.3/setup.cfg
--rw-r--r--   0 seanlee    (501) staff       (20)     1529 2024-05-26 05:29:29.000000 angle_emb-0.4.3/setup.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-29 03:56:58.377304 angle_emb-0.4.4/
+-rw-r--r--   0 seanlee    (501) staff       (20)     1061 2024-05-29 03:39:55.000000 angle_emb-0.4.4/LICENSE
+-rw-r--r--   0 seanlee    (501) staff       (20)    17479 2024-05-29 03:56:58.377679 angle_emb-0.4.4/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)    16762 2024-05-29 03:45:40.000000 angle_emb-0.4.4/README.md
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-29 03:56:58.366336 angle_emb-0.4.4/angle_emb/
+-rw-r--r--   0 seanlee    (501) staff       (20)       70 2024-05-29 03:56:29.000000 angle_emb-0.4.4/angle_emb/__init__.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    68439 2024-05-29 03:55:42.000000 angle_emb-0.4.4/angle_emb/angle.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    13833 2024-05-29 03:39:55.000000 angle_emb-0.4.4/angle_emb/angle_trainer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)      512 2024-05-29 03:39:55.000000 angle_emb-0.4.4/angle_emb/utils.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-29 03:56:58.376714 angle_emb-0.4.4/angle_emb.egg-info/
+-rw-r--r--   0 seanlee    (501) staff       (20)    17479 2024-05-29 03:56:58.000000 angle_emb-0.4.4/angle_emb.egg-info/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)      355 2024-05-29 03:56:58.000000 angle_emb-0.4.4/angle_emb.egg-info/SOURCES.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-05-29 03:56:58.000000 angle_emb-0.4.4/angle_emb.egg-info/dependency_links.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)       63 2024-05-29 03:56:58.000000 angle_emb-0.4.4/angle_emb.egg-info/entry_points.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-05-29 03:56:58.000000 angle_emb-0.4.4/angle_emb.egg-info/not-zip-safe
+-rw-r--r--   0 seanlee    (501) staff       (20)       87 2024-05-29 03:56:58.000000 angle_emb-0.4.4/angle_emb.egg-info/requires.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)       10 2024-05-29 03:56:58.000000 angle_emb-0.4.4/angle_emb.egg-info/top_level.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)      202 2024-05-29 03:56:58.379601 angle_emb-0.4.4/setup.cfg
+-rw-r--r--   0 seanlee    (501) staff       (20)     1529 2024-05-29 03:56:29.000000 angle_emb-0.4.4/setup.py
```

### Comparing `angle_emb-0.4.3/LICENSE` & `angle_emb-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.3/PKG-INFO` & `angle_emb-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angle_emb
-Version: 0.4.3
+Version: 0.4.4
 Summary: AnglE-optimize Text Embeddings
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: angle_emb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -161,28 +161,28 @@
 
 ### ⌛ Infer LLM-based Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 If the pretrained weight is a LoRA-based model, you need to specify the backbone via `model_name_or_path` and specify the LoRA path via the `pretrained_lora_path` in `from_pretrained` method. 
 
 ```python
+import torch
 from angle_emb import AnglE, Prompts
 from angle_emb.utils import cosine_similarity
 
 angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
                               pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
                               pooling_strategy='last',
                               is_llm=True,
-                              torch_dtype='float16').cuda()
-
+                              torch_dtype=torch.float16).cuda()
 print('All predefined prompts:', Prompts.list_prompts())
 doc_vecs = angle.encode([
-    'The weather is great!',
-    'The weather is very good!',
-    'i am going to bed'
+    {'text': 'The weather is great!'},
+    {'text': 'The weather is very good!'},
+    {'text': 'i am going to bed'}
 ], prompt=Prompts.A)
 
 for i, dv1 in enumerate(doc_vecs):
     for dv2 in doc_vecs[i+1:]:
         print(cosine_similarity(dv1, dv2))
 ```
 
@@ -190,36 +190,43 @@
 ### ⌛ Infer BiLLM-based Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 Specify `apply_billm` and `billm_model_class` to load and infer billm models
 
 
 ```python
+import os
+# set an environment variable for billm start index
+os.environ['BiLLM_START_INDEX'] = '31'
+
+import torch
 from angle_emb import AnglE, Prompts
 from angle_emb.utils import cosine_similarity
 
 # specify `apply_billm` and `billm_model_class` to load billm models
 angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
                               pretrained_lora_path='SeanLee97/bellm-llama-7b-nli',
                               pooling_strategy='last',
                               is_llm=True,
                               apply_billm=True,
                               billm_model_class='LlamaForCausalLM',
-                              torch_dtype='float16').cuda()
+                              torch_dtype=torch.float16).cuda()
 
 doc_vecs = angle.encode([
-    'The weather is great!',
-    'The weather is very good!',
-    'i am going to bed'
+    {'text': 'The weather is great!'},
+    {'text': 'The weather is very good!'},
+    {'text': 'i am going to bed'}
 ], prompt='The representative word for sentence {text} is:"')
 
 for i, dv1 in enumerate(doc_vecs):
     for dv2 in doc_vecs[i+1:]:
         print(cosine_similarity(dv1, dv2))
 ```
+
+
 ### ⌛ Infer Espresso/Matryoshka Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 Specify `layer_index` and `embedding_size` to truncate embeddings.
 
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: angle_emb Version: 0.4.3 Summary: AnglE-optimize
+Metadata-Version: 2.1 Name: angle_emb Version: 0.4.4 Summary: AnglE-optimize
 Text Embeddings Author: sean lee Author-email: xmlee97@gmail.com Keywords:
 angle_emb Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -100,114 +100,118 @@
 angle.encode([ 'The weather is great!', 'The weather is very good!', 'i am
 going to bed' ]) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]:
 print(cosine_similarity(dv1, dv2)) ``` ### â Infer LLM-based Models [![Open
 In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 If the pretrained weight is a LoRA-based model, you need to specify the
 backbone via `model_name_or_path` and specify the LoRA path via the
-`pretrained_lora_path` in `from_pretrained` method. ```python from angle_emb
-import AnglE, Prompts from angle_emb.utils import cosine_similarity angle =
-AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+`pretrained_lora_path` in `from_pretrained` method. ```python import torch from
+angle_emb import AnglE, Prompts from angle_emb.utils import cosine_similarity
+angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
 pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
-pooling_strategy='last', is_llm=True, torch_dtype='float16').cuda() print('All
-predefined prompts:', Prompts.list_prompts()) doc_vecs = angle.encode([ 'The
-weather is great!', 'The weather is very good!', 'i am going to bed' ],
-prompt=Prompts.A) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]:
-print(cosine_similarity(dv1, dv2)) ``` ### â Infer BiLLM-based Models [![Open
-In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+pooling_strategy='last', is_llm=True, torch_dtype=torch.float16).cuda() print
+('All predefined prompts:', Prompts.list_prompts()) doc_vecs = angle.encode([
+{'text': 'The weather is great!'}, {'text': 'The weather is very good!'},
+{'text': 'i am going to bed'} ], prompt=Prompts.A) for i, dv1 in enumerate
+(doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1, dv2)) ```
+### â Infer BiLLM-based Models [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 Specify `apply_billm` and `billm_model_class` to load and infer billm models
-```python from angle_emb import AnglE, Prompts from angle_emb.utils import
-cosine_similarity # specify `apply_billm` and `billm_model_class` to load billm
-models angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+```python import os # set an environment variable for billm start index
+os.environ['BiLLM_START_INDEX'] = '31' import torch from angle_emb import
+AnglE, Prompts from angle_emb.utils import cosine_similarity # specify
+`apply_billm` and `billm_model_class` to load billm models angle =
+AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
 pretrained_lora_path='SeanLee97/bellm-llama-7b-nli', pooling_strategy='last',
 is_llm=True, apply_billm=True, billm_model_class='LlamaForCausalLM',
-torch_dtype='float16').cuda() doc_vecs = angle.encode([ 'The weather is
-great!', 'The weather is very good!', 'i am going to bed' ], prompt='The
-representative word for sentence {text} is:"') for i, dv1 in enumerate
+torch_dtype=torch.float16).cuda() doc_vecs = angle.encode([ {'text': 'The
+weather is great!'}, {'text': 'The weather is very good!'}, {'text': 'i am
+going to bed'} ], prompt='The representative word for sentence {text} is:"')
+for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]: print
+(cosine_similarity(dv1, dv2)) ``` ### â Infer Espresso/Matryoshka Models [!
+[Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/
+1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing) Specify `layer_index` and
+`embedding_size` to truncate embeddings. ```python from angle_emb import AnglE
+from angle_emb.utils import cosine_similarity angle = AnglE.from_pretrained
+('mixedbread-ai/mxbai-embed-2d-large-v1', pooling_strategy='cls').cuda() #
+specify layer_index and embedding size to truncate embeddings doc_vecs =
+angle.encode([ 'The weather is great!', 'The weather is very good!', 'i am
+going to bed' ], layer_index=22, embedding_size=768) for i, dv1 in enumerate
 (doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1, dv2)) ```
-### â Infer Espresso/Matryoshka Models [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
-Specify `layer_index` and `embedding_size` to truncate embeddings. ```python
-from angle_emb import AnglE from angle_emb.utils import cosine_similarity angle
-= AnglE.from_pretrained('mixedbread-ai/mxbai-embed-2d-large-v1',
-pooling_strategy='cls').cuda() # specify layer_index and embedding size to
-truncate embeddings doc_vecs = angle.encode([ 'The weather is great!', 'The
-weather is very good!', 'i am going to bed' ], layer_index=22,
-embedding_size=768) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:
-]: print(cosine_similarity(dv1, dv2)) ``` ### â Infer Third-party Models You
-can load any transformer-based third-party models such as `mixedbread-ai/mxbai-
-embed-large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-
-en-v1.5` using `angle_emb`. Here is an example: ```python from angle_emb import
-AnglE model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1',
-pooling_strategy='cls').cuda() vec = model.encode('hello world', to_numpy=True)
-print(vec) ``` ## ð¸ï¸ Custom Train ### ðï¸ 1. Data Prepation We
-currently support three dataset formats: 1) `DatasetFormats.A`: it is a pair
-format with three columns: `text1`, `text2`, and `label` (0/1). 2)
-`DatasetFormats.B`: it is a triple format with three columns: `text`,
-`positive`, and `negative`. `positive` and `negative` store the positive and
-negative samples of `text`. 3) `DatasetFormats.C`: it is a pair format with two
-columns: `text`, `positive`. `positive` store the positive sample of `text`.
-You need to prepare your data into huggingface `datasets.Dataset` in one of the
-formats in terms of your supervised data. ### ð 2. Train with CLI Use
-`angle-trainer` to train your AnglE model in cli mode. 1) Single gpu training:
-Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-trainer --help ``` 2) Multi-gpu
-training: Usage: ```bash CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 -
--master_port=1234 -m angle_emb.angle_trainer --help ``` ### ð 3. Custom
-Train [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-
-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing) ```python from datasets import load_dataset
-from angle_emb import AnglE, AngleDataTokenizer # 1. load pretrained model
-angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
-max_length=128, pooling_strategy='cls').cuda() # 2. load dataset # `text1`,
-`text2`, and `label` are three required columns. ds = load_dataset('mteb/
-stsbenchmark-sts') ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]),
-"text2": str(obj['sentence2']), "label": obj['score']}) ds = ds.select_columns(
-["text1", "text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle
-().map(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8)
-valid_ds = ds['validation'].map(AngleDataTokenizer(angle.tokenizer,
-angle.max_length), num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer
-(angle.tokenizer, angle.max_length), num_proc=8) # 4. fit angle.fit
-( train_ds=train_ds, valid_ds=valid_ds, output_dir='ckpts/sts-b',
-batch_size=32, epochs=5, learning_rate=2e-5, save_steps=100, eval_steps=1000,
-warmup_steps=0, gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0,
-'ibn_w': 1.0, 'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20
-}, fp16=True, logging_steps=100 ) # 5. evaluate corrcoef, accuracy =
-angle.evaluate(test_ds, device=angle.device) print('corrcoef:', corrcoef) ```
-### ð¡ Others - To enable `llm` training, please specify `--is_llm 1` and
-configure appropriate LoRA hyperparameters. - To enable `billm` training,
-please specify `--apply_billm 1` and configure appropriate `billm_model_class`
-such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/
-BiLLM?tab=readme-ov-file#usage). - To enable espresso sentence embeddings
-(ESE), please specify `--apply_ese 1` and configure appropriate ESE
-hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size
-integer`. - To convert the trained AnglE models to `sentence-transformers`,
-please run `python scripts/convert_to_sentence_transformers.py --help` for more
-details. ## ð¡ 4. Fine-tuning Tips 1ï¸â£ If your dataset format is
-`DatasetFormats.A`, it is recommended to slightly increase the weight for
-`cosine_w` or slightly decrease the weight for `ibn_w`. 2ï¸â£ If your dataset
-format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and
-increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is
-recommended to set to 20.0. 3ï¸â£ If your dataset format is
-`DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to
-tune other parameters. 4ï¸â£ To alleviate information forgetting in fine-
-tuning, it is better to specify the `teacher_name_or_path`. If the
-`teacher_name_or_path` equals `model_name_or_path`, it will conduct self-
-distillation. **It is worth to note that** `teacher_name_or_path` has to have
-the same tokenizer as `model_name_or_path`. Or it will lead to unexpected
-results. # ð«¡ Citation You are welcome to use our code and pre-trained
-models. If you use our code and pre-trained models, please support us by citing
-our work as follows: ```bibtex @article{li2023angle, title={AnglE-optimized
-Text Embeddings}, author={Li, Xianming and Li, Jing}, journal={arXiv preprint
-arXiv:2309.12871}, year={2023} } ``` # ð ChangeLogs | ð | Description |
-|----|------| | 2024 May 21 | support Espresso Sentence Embeddings | | 2024 Feb
-7 | support training with only positive pairs (`DatasetFormats.C`) | | 2023 Dec
-4 | Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-
-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an
-English pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 |
-Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-
-v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§
-Contact If you have any questions or suggestions, please feel free to contact
-us via email: xmlee97@gmail.com # Â© License This project is licensed under the
-MIT License. For the pretrained models, please refer to the corresponding
-license of the models.
+### â Infer Third-party Models You can load any transformer-based third-party
+models such as `mixedbread-ai/mxbai-embed-large-v1`, `sentence-transformers/
+all-MiniLM-L6-v2`, and `BAAI/bge-large-en-v1.5` using `angle_emb`. Here is an
+example: ```python from angle_emb import AnglE model = AnglE.from_pretrained
+('mixedbread-ai/mxbai-embed-large-v1', pooling_strategy='cls').cuda() vec =
+model.encode('hello world', to_numpy=True) print(vec) ``` ## ð¸ï¸ Custom
+Train ### ðï¸ 1. Data Prepation We currently support three dataset formats:
+1) `DatasetFormats.A`: it is a pair format with three columns: `text1`,
+`text2`, and `label` (0/1). 2) `DatasetFormats.B`: it is a triple format with
+three columns: `text`, `positive`, and `negative`. `positive` and `negative`
+store the positive and negative samples of `text`. 3) `DatasetFormats.C`: it is
+a pair format with two columns: `text`, `positive`. `positive` store the
+positive sample of `text`. You need to prepare your data into huggingface
+`datasets.Dataset` in one of the formats in terms of your supervised data. ###
+ð 2. Train with CLI Use `angle-trainer` to train your AnglE model in cli
+mode. 1) Single gpu training: Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-
+trainer --help ``` 2) Multi-gpu training: Usage: ```bash
+CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 --master_port=1234 -
+m angle_emb.angle_trainer --help ``` ### ð 3. Custom Train [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
+```python from datasets import load_dataset from angle_emb import AnglE,
+AngleDataTokenizer # 1. load pretrained model angle = AnglE.from_pretrained
+('SeanLee97/angle-bert-base-uncased-nli-en-v1', max_length=128,
+pooling_strategy='cls').cuda() # 2. load dataset # `text1`, `text2`, and
+`label` are three required columns. ds = load_dataset('mteb/stsbenchmark-sts')
+ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]), "text2": str(obj
+['sentence2']), "label": obj['score']}) ds = ds.select_columns(["text1",
+"text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle().map
+(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8) valid_ds =
+ds['validation'].map(AngleDataTokenizer(angle.tokenizer, angle.max_length),
+num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer(angle.tokenizer,
+angle.max_length), num_proc=8) # 4. fit angle.fit( train_ds=train_ds,
+valid_ds=valid_ds, output_dir='ckpts/sts-b', batch_size=32, epochs=5,
+learning_rate=2e-5, save_steps=100, eval_steps=1000, warmup_steps=0,
+gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0, 'ibn_w': 1.0,
+'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20 }, fp16=True,
+logging_steps=100 ) # 5. evaluate corrcoef, accuracy = angle.evaluate(test_ds,
+device=angle.device) print('corrcoef:', corrcoef) ``` ### ð¡ Others - To
+enable `llm` training, please specify `--is_llm 1` and configure appropriate
+LoRA hyperparameters. - To enable `billm` training, please specify `--
+apply_billm 1` and configure appropriate `billm_model_class` such as
+`LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/BiLLM?tab=readme-ov-
+file#usage). - To enable espresso sentence embeddings (ESE), please specify `--
+apply_ese 1` and configure appropriate ESE hyperparameters via `--
+ese_kl_temperature float` and `--ese_compression_size integer`. - To convert
+the trained AnglE models to `sentence-transformers`, please run `python
+scripts/convert_to_sentence_transformers.py --help` for more details. ## ð¡
+4. Fine-tuning Tips 1ï¸â£ If your dataset format is `DatasetFormats.A`, it is
+recommended to slightly increase the weight for `cosine_w` or slightly decrease
+the weight for `ibn_w`. 2ï¸â£ If your dataset format is `DatasetFormats.B`,
+it is recommended to set `cosine_w` to 0, and increase the weight for `ibn_w`
+such as 10 and 20. The `angle_tau` is recommended to set to 20.0. 3ï¸â£ If
+your dataset format is `DatasetFormats.C`, only `ibn_w` and `ibn_tau` are
+effective. You don't need to tune other parameters. 4ï¸â£ To alleviate
+information forgetting in fine-tuning, it is better to specify the
+`teacher_name_or_path`. If the `teacher_name_or_path` equals
+`model_name_or_path`, it will conduct self-distillation. **It is worth to note
+that** `teacher_name_or_path` has to have the same tokenizer as
+`model_name_or_path`. Or it will lead to unexpected results. # ð«¡ Citation
+You are welcome to use our code and pre-trained models. If you use our code and
+pre-trained models, please support us by citing our work as follows: ```bibtex
+@article{li2023angle, title={AnglE-optimized Text Embeddings}, author={Li,
+Xianming and Li, Jing}, journal={arXiv preprint arXiv:2309.12871}, year={2023}
+} ``` # ð ChangeLogs | ð | Description | |----|------| | 2024 May 21 |
+support Espresso Sentence Embeddings | | 2024 Feb 7 | support training with
+only positive pairs (`DatasetFormats.C`) | | 2023 Dec 4 | Release a universal
+English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://
+huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an English
+pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 | Release two
+chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and
+`SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§ Contact If
+you have any questions or suggestions, please feel free to contact us via
+email: xmlee97@gmail.com # Â© License This project is licensed under the MIT
+License. For the pretrained models, please refer to the corresponding license
+of the models.
```

### Comparing `angle_emb-0.4.3/README.md` & `angle_emb-0.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -141,28 +141,28 @@
 
 ### ⌛ Infer LLM-based Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 If the pretrained weight is a LoRA-based model, you need to specify the backbone via `model_name_or_path` and specify the LoRA path via the `pretrained_lora_path` in `from_pretrained` method. 
 
 ```python
+import torch
 from angle_emb import AnglE, Prompts
 from angle_emb.utils import cosine_similarity
 
 angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
                               pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
                               pooling_strategy='last',
                               is_llm=True,
-                              torch_dtype='float16').cuda()
-
+                              torch_dtype=torch.float16).cuda()
 print('All predefined prompts:', Prompts.list_prompts())
 doc_vecs = angle.encode([
-    'The weather is great!',
-    'The weather is very good!',
-    'i am going to bed'
+    {'text': 'The weather is great!'},
+    {'text': 'The weather is very good!'},
+    {'text': 'i am going to bed'}
 ], prompt=Prompts.A)
 
 for i, dv1 in enumerate(doc_vecs):
     for dv2 in doc_vecs[i+1:]:
         print(cosine_similarity(dv1, dv2))
 ```
 
@@ -170,36 +170,43 @@
 ### ⌛ Infer BiLLM-based Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 Specify `apply_billm` and `billm_model_class` to load and infer billm models
 
 
 ```python
+import os
+# set an environment variable for billm start index
+os.environ['BiLLM_START_INDEX'] = '31'
+
+import torch
 from angle_emb import AnglE, Prompts
 from angle_emb.utils import cosine_similarity
 
 # specify `apply_billm` and `billm_model_class` to load billm models
 angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
                               pretrained_lora_path='SeanLee97/bellm-llama-7b-nli',
                               pooling_strategy='last',
                               is_llm=True,
                               apply_billm=True,
                               billm_model_class='LlamaForCausalLM',
-                              torch_dtype='float16').cuda()
+                              torch_dtype=torch.float16).cuda()
 
 doc_vecs = angle.encode([
-    'The weather is great!',
-    'The weather is very good!',
-    'i am going to bed'
+    {'text': 'The weather is great!'},
+    {'text': 'The weather is very good!'},
+    {'text': 'i am going to bed'}
 ], prompt='The representative word for sentence {text} is:"')
 
 for i, dv1 in enumerate(doc_vecs):
     for dv2 in doc_vecs[i+1:]:
         print(cosine_similarity(dv1, dv2))
 ```
+
+
 ### ⌛ Infer Espresso/Matryoshka Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 Specify `layer_index` and `embedding_size` to truncate embeddings.
 
 
 ```python
```

#### html2text {}

```diff
@@ -90,114 +90,118 @@
 angle.encode([ 'The weather is great!', 'The weather is very good!', 'i am
 going to bed' ]) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]:
 print(cosine_similarity(dv1, dv2)) ``` ### â Infer LLM-based Models [![Open
 In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 If the pretrained weight is a LoRA-based model, you need to specify the
 backbone via `model_name_or_path` and specify the LoRA path via the
-`pretrained_lora_path` in `from_pretrained` method. ```python from angle_emb
-import AnglE, Prompts from angle_emb.utils import cosine_similarity angle =
-AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+`pretrained_lora_path` in `from_pretrained` method. ```python import torch from
+angle_emb import AnglE, Prompts from angle_emb.utils import cosine_similarity
+angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
 pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
-pooling_strategy='last', is_llm=True, torch_dtype='float16').cuda() print('All
-predefined prompts:', Prompts.list_prompts()) doc_vecs = angle.encode([ 'The
-weather is great!', 'The weather is very good!', 'i am going to bed' ],
-prompt=Prompts.A) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]:
-print(cosine_similarity(dv1, dv2)) ``` ### â Infer BiLLM-based Models [![Open
-In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+pooling_strategy='last', is_llm=True, torch_dtype=torch.float16).cuda() print
+('All predefined prompts:', Prompts.list_prompts()) doc_vecs = angle.encode([
+{'text': 'The weather is great!'}, {'text': 'The weather is very good!'},
+{'text': 'i am going to bed'} ], prompt=Prompts.A) for i, dv1 in enumerate
+(doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1, dv2)) ```
+### â Infer BiLLM-based Models [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 Specify `apply_billm` and `billm_model_class` to load and infer billm models
-```python from angle_emb import AnglE, Prompts from angle_emb.utils import
-cosine_similarity # specify `apply_billm` and `billm_model_class` to load billm
-models angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+```python import os # set an environment variable for billm start index
+os.environ['BiLLM_START_INDEX'] = '31' import torch from angle_emb import
+AnglE, Prompts from angle_emb.utils import cosine_similarity # specify
+`apply_billm` and `billm_model_class` to load billm models angle =
+AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
 pretrained_lora_path='SeanLee97/bellm-llama-7b-nli', pooling_strategy='last',
 is_llm=True, apply_billm=True, billm_model_class='LlamaForCausalLM',
-torch_dtype='float16').cuda() doc_vecs = angle.encode([ 'The weather is
-great!', 'The weather is very good!', 'i am going to bed' ], prompt='The
-representative word for sentence {text} is:"') for i, dv1 in enumerate
+torch_dtype=torch.float16).cuda() doc_vecs = angle.encode([ {'text': 'The
+weather is great!'}, {'text': 'The weather is very good!'}, {'text': 'i am
+going to bed'} ], prompt='The representative word for sentence {text} is:"')
+for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]: print
+(cosine_similarity(dv1, dv2)) ``` ### â Infer Espresso/Matryoshka Models [!
+[Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/
+1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing) Specify `layer_index` and
+`embedding_size` to truncate embeddings. ```python from angle_emb import AnglE
+from angle_emb.utils import cosine_similarity angle = AnglE.from_pretrained
+('mixedbread-ai/mxbai-embed-2d-large-v1', pooling_strategy='cls').cuda() #
+specify layer_index and embedding size to truncate embeddings doc_vecs =
+angle.encode([ 'The weather is great!', 'The weather is very good!', 'i am
+going to bed' ], layer_index=22, embedding_size=768) for i, dv1 in enumerate
 (doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1, dv2)) ```
-### â Infer Espresso/Matryoshka Models [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
-Specify `layer_index` and `embedding_size` to truncate embeddings. ```python
-from angle_emb import AnglE from angle_emb.utils import cosine_similarity angle
-= AnglE.from_pretrained('mixedbread-ai/mxbai-embed-2d-large-v1',
-pooling_strategy='cls').cuda() # specify layer_index and embedding size to
-truncate embeddings doc_vecs = angle.encode([ 'The weather is great!', 'The
-weather is very good!', 'i am going to bed' ], layer_index=22,
-embedding_size=768) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:
-]: print(cosine_similarity(dv1, dv2)) ``` ### â Infer Third-party Models You
-can load any transformer-based third-party models such as `mixedbread-ai/mxbai-
-embed-large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-
-en-v1.5` using `angle_emb`. Here is an example: ```python from angle_emb import
-AnglE model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1',
-pooling_strategy='cls').cuda() vec = model.encode('hello world', to_numpy=True)
-print(vec) ``` ## ð¸ï¸ Custom Train ### ðï¸ 1. Data Prepation We
-currently support three dataset formats: 1) `DatasetFormats.A`: it is a pair
-format with three columns: `text1`, `text2`, and `label` (0/1). 2)
-`DatasetFormats.B`: it is a triple format with three columns: `text`,
-`positive`, and `negative`. `positive` and `negative` store the positive and
-negative samples of `text`. 3) `DatasetFormats.C`: it is a pair format with two
-columns: `text`, `positive`. `positive` store the positive sample of `text`.
-You need to prepare your data into huggingface `datasets.Dataset` in one of the
-formats in terms of your supervised data. ### ð 2. Train with CLI Use
-`angle-trainer` to train your AnglE model in cli mode. 1) Single gpu training:
-Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-trainer --help ``` 2) Multi-gpu
-training: Usage: ```bash CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 -
--master_port=1234 -m angle_emb.angle_trainer --help ``` ### ð 3. Custom
-Train [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-
-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing) ```python from datasets import load_dataset
-from angle_emb import AnglE, AngleDataTokenizer # 1. load pretrained model
-angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
-max_length=128, pooling_strategy='cls').cuda() # 2. load dataset # `text1`,
-`text2`, and `label` are three required columns. ds = load_dataset('mteb/
-stsbenchmark-sts') ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]),
-"text2": str(obj['sentence2']), "label": obj['score']}) ds = ds.select_columns(
-["text1", "text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle
-().map(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8)
-valid_ds = ds['validation'].map(AngleDataTokenizer(angle.tokenizer,
-angle.max_length), num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer
-(angle.tokenizer, angle.max_length), num_proc=8) # 4. fit angle.fit
-( train_ds=train_ds, valid_ds=valid_ds, output_dir='ckpts/sts-b',
-batch_size=32, epochs=5, learning_rate=2e-5, save_steps=100, eval_steps=1000,
-warmup_steps=0, gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0,
-'ibn_w': 1.0, 'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20
-}, fp16=True, logging_steps=100 ) # 5. evaluate corrcoef, accuracy =
-angle.evaluate(test_ds, device=angle.device) print('corrcoef:', corrcoef) ```
-### ð¡ Others - To enable `llm` training, please specify `--is_llm 1` and
-configure appropriate LoRA hyperparameters. - To enable `billm` training,
-please specify `--apply_billm 1` and configure appropriate `billm_model_class`
-such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/
-BiLLM?tab=readme-ov-file#usage). - To enable espresso sentence embeddings
-(ESE), please specify `--apply_ese 1` and configure appropriate ESE
-hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size
-integer`. - To convert the trained AnglE models to `sentence-transformers`,
-please run `python scripts/convert_to_sentence_transformers.py --help` for more
-details. ## ð¡ 4. Fine-tuning Tips 1ï¸â£ If your dataset format is
-`DatasetFormats.A`, it is recommended to slightly increase the weight for
-`cosine_w` or slightly decrease the weight for `ibn_w`. 2ï¸â£ If your dataset
-format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and
-increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is
-recommended to set to 20.0. 3ï¸â£ If your dataset format is
-`DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to
-tune other parameters. 4ï¸â£ To alleviate information forgetting in fine-
-tuning, it is better to specify the `teacher_name_or_path`. If the
-`teacher_name_or_path` equals `model_name_or_path`, it will conduct self-
-distillation. **It is worth to note that** `teacher_name_or_path` has to have
-the same tokenizer as `model_name_or_path`. Or it will lead to unexpected
-results. # ð«¡ Citation You are welcome to use our code and pre-trained
-models. If you use our code and pre-trained models, please support us by citing
-our work as follows: ```bibtex @article{li2023angle, title={AnglE-optimized
-Text Embeddings}, author={Li, Xianming and Li, Jing}, journal={arXiv preprint
-arXiv:2309.12871}, year={2023} } ``` # ð ChangeLogs | ð | Description |
-|----|------| | 2024 May 21 | support Espresso Sentence Embeddings | | 2024 Feb
-7 | support training with only positive pairs (`DatasetFormats.C`) | | 2023 Dec
-4 | Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-
-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an
-English pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 |
-Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-
-v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§
-Contact If you have any questions or suggestions, please feel free to contact
-us via email: xmlee97@gmail.com # Â© License This project is licensed under the
-MIT License. For the pretrained models, please refer to the corresponding
-license of the models.
+### â Infer Third-party Models You can load any transformer-based third-party
+models such as `mixedbread-ai/mxbai-embed-large-v1`, `sentence-transformers/
+all-MiniLM-L6-v2`, and `BAAI/bge-large-en-v1.5` using `angle_emb`. Here is an
+example: ```python from angle_emb import AnglE model = AnglE.from_pretrained
+('mixedbread-ai/mxbai-embed-large-v1', pooling_strategy='cls').cuda() vec =
+model.encode('hello world', to_numpy=True) print(vec) ``` ## ð¸ï¸ Custom
+Train ### ðï¸ 1. Data Prepation We currently support three dataset formats:
+1) `DatasetFormats.A`: it is a pair format with three columns: `text1`,
+`text2`, and `label` (0/1). 2) `DatasetFormats.B`: it is a triple format with
+three columns: `text`, `positive`, and `negative`. `positive` and `negative`
+store the positive and negative samples of `text`. 3) `DatasetFormats.C`: it is
+a pair format with two columns: `text`, `positive`. `positive` store the
+positive sample of `text`. You need to prepare your data into huggingface
+`datasets.Dataset` in one of the formats in terms of your supervised data. ###
+ð 2. Train with CLI Use `angle-trainer` to train your AnglE model in cli
+mode. 1) Single gpu training: Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-
+trainer --help ``` 2) Multi-gpu training: Usage: ```bash
+CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 --master_port=1234 -
+m angle_emb.angle_trainer --help ``` ### ð 3. Custom Train [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
+```python from datasets import load_dataset from angle_emb import AnglE,
+AngleDataTokenizer # 1. load pretrained model angle = AnglE.from_pretrained
+('SeanLee97/angle-bert-base-uncased-nli-en-v1', max_length=128,
+pooling_strategy='cls').cuda() # 2. load dataset # `text1`, `text2`, and
+`label` are three required columns. ds = load_dataset('mteb/stsbenchmark-sts')
+ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]), "text2": str(obj
+['sentence2']), "label": obj['score']}) ds = ds.select_columns(["text1",
+"text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle().map
+(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8) valid_ds =
+ds['validation'].map(AngleDataTokenizer(angle.tokenizer, angle.max_length),
+num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer(angle.tokenizer,
+angle.max_length), num_proc=8) # 4. fit angle.fit( train_ds=train_ds,
+valid_ds=valid_ds, output_dir='ckpts/sts-b', batch_size=32, epochs=5,
+learning_rate=2e-5, save_steps=100, eval_steps=1000, warmup_steps=0,
+gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0, 'ibn_w': 1.0,
+'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20 }, fp16=True,
+logging_steps=100 ) # 5. evaluate corrcoef, accuracy = angle.evaluate(test_ds,
+device=angle.device) print('corrcoef:', corrcoef) ``` ### ð¡ Others - To
+enable `llm` training, please specify `--is_llm 1` and configure appropriate
+LoRA hyperparameters. - To enable `billm` training, please specify `--
+apply_billm 1` and configure appropriate `billm_model_class` such as
+`LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/BiLLM?tab=readme-ov-
+file#usage). - To enable espresso sentence embeddings (ESE), please specify `--
+apply_ese 1` and configure appropriate ESE hyperparameters via `--
+ese_kl_temperature float` and `--ese_compression_size integer`. - To convert
+the trained AnglE models to `sentence-transformers`, please run `python
+scripts/convert_to_sentence_transformers.py --help` for more details. ## ð¡
+4. Fine-tuning Tips 1ï¸â£ If your dataset format is `DatasetFormats.A`, it is
+recommended to slightly increase the weight for `cosine_w` or slightly decrease
+the weight for `ibn_w`. 2ï¸â£ If your dataset format is `DatasetFormats.B`,
+it is recommended to set `cosine_w` to 0, and increase the weight for `ibn_w`
+such as 10 and 20. The `angle_tau` is recommended to set to 20.0. 3ï¸â£ If
+your dataset format is `DatasetFormats.C`, only `ibn_w` and `ibn_tau` are
+effective. You don't need to tune other parameters. 4ï¸â£ To alleviate
+information forgetting in fine-tuning, it is better to specify the
+`teacher_name_or_path`. If the `teacher_name_or_path` equals
+`model_name_or_path`, it will conduct self-distillation. **It is worth to note
+that** `teacher_name_or_path` has to have the same tokenizer as
+`model_name_or_path`. Or it will lead to unexpected results. # ð«¡ Citation
+You are welcome to use our code and pre-trained models. If you use our code and
+pre-trained models, please support us by citing our work as follows: ```bibtex
+@article{li2023angle, title={AnglE-optimized Text Embeddings}, author={Li,
+Xianming and Li, Jing}, journal={arXiv preprint arXiv:2309.12871}, year={2023}
+} ``` # ð ChangeLogs | ð | Description | |----|------| | 2024 May 21 |
+support Espresso Sentence Embeddings | | 2024 Feb 7 | support training with
+only positive pairs (`DatasetFormats.C`) | | 2023 Dec 4 | Release a universal
+English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://
+huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an English
+pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 | Release two
+chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and
+`SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§ Contact If
+you have any questions or suggestions, please feel free to contact us via
+email: xmlee97@gmail.com # Â© License This project is licensed under the MIT
+License. For the pretrained models, please refer to the corresponding license
+of the models.
```

### Comparing `angle_emb-0.4.3/angle_emb/angle.py` & `angle_emb-0.4.4/angle_emb/angle.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,15 @@
 
 
 def l2_normalize(arr: np.ndarray) -> np.ndarray:
     """
     Normalize array using L2
 
     :param arr: np.ndarray, input array
+
     :return: np.ndarray
     """
     norms = (arr**2).sum(axis=1, keepdims=True)**0.5
     return arr / np.clip(norms, 1e-8, np.inf)
 
 
 def optimal_threshold(y_true: np.ndarray, y_pred: np.ndarray) -> Tuple[float, float]:
@@ -701,14 +702,15 @@
                  inputs: Dict,
                  layer_index: int = -1,
                  embedding_start: Optional[int] = None,
                  embedding_size: Optional[int] = None,
                  return_all_layer_outputs: bool = False,
                  pooling_strategy: Optional[Union[int, str]] = None,) -> torch.Tensor:
         """ Get sentence embeddings.
+
         :param inputs: Dict. Model inputs.
         :param layer_index: Optional[int]. Get embeddings from specific layer.
         :param embedding_start: Optional[int]. Start index of embeddings.
         :param embedding_size: int. Set embedding size for sentence embeddings.
         :param return_all_layer_outputs: bool. Return all layer outputs or not. Default False.
         :param pooling_strategy: Optional[str].
             Currently support [`cls`, `last`, `avg`, `cls_avg`, `max`]. Default None.
@@ -786,14 +788,15 @@
                           kl_temperature: float = 1.0) -> torch.Tensor:
         """ Compute distillation loss.
 
         :param inputs: torch.Tensor. Input tensor.
         :param targets: torch.Tensor. Target tensor.
         :param mse_weight: float. MSE weight. Default 1.0.
         :param kl_temperature: float. KL temperature. Default 1.0.
+
         :return: torch.Tensor. Distillation loss.
         """
         loss = 0.
         if mse_weight > 0:
             loss += mse_weight * nn.MSELoss()(inputs, targets)
         if kl_temperature > 0:
             loss += nn.KLDivLoss(reduction='batchmean')(
@@ -804,14 +807,15 @@
 
     def compute_loss(self, model, inputs, return_outputs=False):
         """ Compute loss for AnglE.
 
         :param model: Huggingface model.
         :param inputs: Dict. Model inputs.
         :param return_outputs: bool. Return outputs or not. Default False.
+
         :return: torch.Tensor. Loss.
         """
         labels = inputs.pop("labels", None)
         if self.teacher_name_or_path is not None:
             all_outputs = self.pooler(inputs, layer_index=-1, return_all_layer_outputs=True)[-1]
             outputs = get_pooling(all_outputs, inputs,
                                   self.pooler.pooling_strategy,
@@ -838,15 +842,14 @@
     """
     Custom Huggingface Trainer for AnglE Espresso.
 
     :param pooler: Pooler. Required
     :param loss_kwargs: Optional[Dict]. Default None.
     :param dataset_format: str. Default DatasetFormats.A
     :param teacher_name_or_path: Optional[str]. For distribution alignment.
-
     :param **kwargs: other parameters of Trainer.
     """
     def __init__(self,
                  pooler: Pooler,
                  loss_kwargs: Optional[Dict] = None,
                  dataset_format: str = DatasetFormats.A,
                  teacher_name_or_path: Optional[str] = None,
@@ -864,16 +867,18 @@
         self.apply_ese_pca = apply_ese_pca
         self.n_layers = self.pooler.model.config.num_hidden_layers
         logger.info('Train with ☕️ Espresso!')
 
     @torch.no_grad()
     def pca_compress(self, m: torch.Tensor, k: int) -> torch.Tensor:
         """ Get topk feature via PCA.
+
         :param m: torch.Tensor. Input tensor.
         :param k: int. Top-k feature size.
+
         :return: torch.Tensor. Top-k feature.
         """
         A = F.softmax(m.T @ m / m.shape[-1]**0.5, dim=-1)
         u, s, _ = torch.svd_lowrank(A, q=k)
         # top-k principal components
         topk_deps = u @ torch.diag(s)
         return m @ topk_deps
@@ -902,17 +907,19 @@
                     self.pca_compress(student_outputs, self.ese_compression_size),
                     kl_temperature=self.ese_kl_temperature
                 ) / division
         return (loss + compression_loss) / (self.n_layers - 1)
 
     def compute_loss(self, model, inputs, return_outputs=False):
         """ Compute loss for Espresso.
+
         :param model: Huggingface model.
         :param inputs: Dict. Model inputs.
         :param return_outputs: bool. Return outputs or not. Default False.
+
         :return: torch.Tensor. Loss.
         """
         labels = inputs.pop("labels", None)
         # layer
         all_layer_outputs = self.pooler(inputs, layer_index=-1, return_all_layer_outputs=True)
         all_teacher_outputs = all_layer_outputs[-1]
         teacher_outputs = get_pooling(all_teacher_outputs, inputs,
@@ -992,14 +999,15 @@
     def __call__(self,
                  labels: torch.Tensor,
                  outputs: torch.Tensor) -> torch.Tensor:
         """ Compute loss for AnglE.
 
         :param labels: torch.Tensor. Labels.
         :param outputs: torch.Tensor. Outputs.
+
         :return: torch.Tensor. Loss.
         """
         if self.dataset_format == DatasetFormats.A:
             loss = 0.
             if self.cosine_w > 0:
                 loss += self.cosine_w * cosine_loss(labels, outputs, self.cosine_tau)
             if self.ibn_w > 0:
@@ -1086,15 +1094,14 @@
         Currently support [`cls`, `last`, `avg`, `cls_avg`, `max`]
     :param apply_lora: Optional[bool]. Whether apply lora. Default None.
     :param train_mode: bool. Whether load for training. Default True.
     :param load_kbit: Optional[int]. Specify kbit training from [4, 8, 16]. Default None.
     :param is_llm: Optional[bool]. Whether the model is llm. Default None.
     :param pretrained_model_path: Optional[str]. Default None.
     :param pretrained_lora_path: Optional[str]. Default None.
-    :param apply_bfloat16: Optional[bool]. Whether load using torch.bfloat16. Default None.
     :param torch_dtype: Optional[torch.dtype]. Specify torch_dtype. Default None.
     :param device: Optional[str]. Specify device. Default None.
     :param kbit_kwargs: Optional[Dict]. kwargs for kbit. Default None.
         details refer to: https://huggingface.co/docs/peft/package_reference/peft_model#peft.prepare_model_for_kbit_training
     :param tokenizer_padding_side: Optional[str]. Specify tokenizer padding side from [`left`, `right`]. Default None.
     :param **kwargs: Any.
     """  # NOQA
@@ -1109,15 +1116,14 @@
                  pooling_strategy: Optional[str] = None,
                  apply_lora: Optional[bool] = None,
                  train_mode: bool = True,
                  load_kbit: Optional[int] = None,
                  is_llm: Optional[bool] = None,
                  pretrained_model_path: Optional[str] = None,
                  pretrained_lora_path: Optional[str] = None,
-                 apply_bfloat16: Optional[bool] = None,
                  torch_dtype: Optional[torch.dtype] = None,
                  device: Optional[str] = None,
                  kbit_kwargs: Optional[Dict] = None,
                  tokenizer_padding_side: Optional[str] = None,
                  apply_billm: bool = False,
                  billm_model_class: Optional[str] = None,
                  **kwargs: Any):
@@ -1152,20 +1158,14 @@
         if self.device == 'cuda':
             self.gpu_count = torch.cuda.device_count()
         elif self.device == 'mps':
             self.gpu_count = 1
         else:
             self.gpu_count = 0
 
-        self.apply_bfloat16 = apply_bfloat16
-        if self.apply_bfloat16 is None and 'llama' in model_name_or_path.lower():
-            logger.info('LLaMA detected, automatically set `apply_bfloat16=True`. '
-                        'You can change this setting by manually configuring the `apply_bfloat16`.')
-            self.apply_bfloat16 = True
-
         if torch_dtype is None:
             torch_dtype = torch.float32 if train_mode else None
 
         lora_config = None
         if self.apply_lora:
             lora_config = {
                 'task_type': TaskType.FEATURE_EXTRACTION,
@@ -1204,15 +1204,16 @@
             if train_mode and self.gpu_count > 1:
                 device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
             # LLM
             if self.apply_lora:
                 lora_config['bias'] = "none"
                 lora_config['task_type'] = TaskType.CAUSAL_LM
 
-                if load_kbit in [4, 8]:
+                is_kbit = load_kbit in [4, 8]
+                if is_kbit:
                     model = MODEL_CLASS.from_pretrained(
                         model_name_or_path,
                         config=None,
                         quantization_config=BitsAndBytesConfig(
                             load_in_4bit=load_kbit == 4,
                             load_in_8bit=load_kbit == 8,
                             llm_int8_threshold=6.0,
@@ -1221,78 +1222,51 @@
                             bnb_4bit_use_double_quant=True,
                             bnb_4bit_quant_type='nf4',
                         ),
                         torch_dtype=torch.float32,
                         device_map=device_map,
                         trust_remote_code=True,
                     )
-                    if train_mode:
-                        model = prepare_model_for_kbit_training(model, **kbit_kwargs)
-                    if pretrained_lora_path is not None:
-                        print(f'Load lora weight from {pretrained_lora_path}')
-                        model = PeftModel.from_pretrained(
-                            model,
-                            pretrained_lora_path,
-                            torch_dtype=torch.float32,
-                            device_map=device_map,
-                            is_trainable=train_mode
-                        )
-                    elif train_mode:
-                        if 'target_modules' not in lora_config or lora_config.get('target_modules', None) is None:
-                            target_modules = find_all_linear_names(
-                                model, linear_type=bnb.nn.Linear4bit if load_kbit == 4 else nn.Linear)
-                            lora_config['target_modules'] = target_modules
-                            logger.info(f'lora target modules={target_modules}')
-                        peft_config = LoraConfig(**lora_config)
-                        model = get_peft_model(model, peft_config)
-                    model = AnglE.kbit_post_handle(model)
-                    self.backbone = model
                 else:
-                    if self.apply_bfloat16:
-                        model = MODEL_CLASS.from_pretrained(model_name_or_path,
-                                                            output_hidden_states=True,
-                                                            trust_remote_code=True).bfloat16()
-                    else:
-                        model = MODEL_CLASS.from_pretrained(model_name_or_path,
-                                                            device_map=device_map,
-                                                            output_hidden_states=True,
-                                                            trust_remote_code=True,
-                                                            torch_dtype=torch_dtype or torch.float16)
+                    model = MODEL_CLASS.from_pretrained(model_name_or_path,
+                                                        device_map=device_map,
+                                                        output_hidden_states=True,
+                                                        trust_remote_code=True,
+                                                        torch_dtype=torch_dtype or torch.float16)
+                if train_mode and is_kbit:
+                    model = prepare_model_for_kbit_training(model, **kbit_kwargs)
 
+                if pretrained_lora_path is not None:
+                    logger.info(f'Load lora weight from {pretrained_lora_path}')
+                    model = PeftModel.from_pretrained(
+                        model,
+                        pretrained_lora_path,
+                        torch_dtype=torch.float32 if is_kbit else (torch_dtype or torch.float16),
+                        device_map=device_map,
+                        is_trainable=train_mode
+                    )
+                elif train_mode:
                     if 'target_modules' not in lora_config or lora_config.get('target_modules', None) is None:
-                        target_modules = find_all_linear_names(model)
+                        target_modules = find_all_linear_names(
+                            model, linear_type=bnb.nn.Linear4bit if load_kbit == 4 else nn.Linear)
                         lora_config['target_modules'] = target_modules
                         logger.info(f'lora target modules={target_modules}')
+                    peft_config = LoraConfig(**lora_config)
+                    model = get_peft_model(model, peft_config)
 
-                    if pretrained_lora_path is not None:
-                        print(f'Load lora weight from {pretrained_lora_path}')
-                        model = PeftModel.from_pretrained(
-                            model,
-                            pretrained_lora_path,
-                            torch_dtype=torch.float16 if load_kbit == 16 else torch.float32,
-                            device_map=device_map,
-                            is_trainable=train_mode
-                        )
-                    else:
-                        if train_mode:
-                            peft_config = LoraConfig(**lora_config)
-                            model = get_peft_model(model, peft_config)
+                if is_kbit:
+                    model = AnglE.kbit_post_handle(model)
 
-                    self.backbone = model
+                self.backbone = model
             else:
-                if self.apply_bfloat16:
-                    model = MODEL_CLASS.from_pretrained(model_name_or_path,
-                                                        output_hidden_states=True,
-                                                        trust_remote_code=True).bfloat16()
-                else:
-                    model = MODEL_CLASS.from_pretrained(model_name_or_path,
-                                                        device_map=device_map,
-                                                        output_hidden_states=True,
-                                                        trust_remote_code=True,
-                                                        torch_dtype=torch_dtype or torch.float16)
+                model = MODEL_CLASS.from_pretrained(model_name_or_path,
+                                                    device_map=device_map,
+                                                    output_hidden_states=True,
+                                                    trust_remote_code=True,
+                                                    torch_dtype=torch_dtype or torch.float16)
                 self.backbone = model
         else:
             # non-LLMs
             if self.apply_lora:
                 model = AutoModel.from_pretrained(pretrained_model_path or model_name_or_path, trust_remote_code=True)
                 if pretrained_lora_path is not None:
                     model = PeftModel.from_pretrained(
@@ -1337,16 +1311,17 @@
             'billm_model_class': billm_model_class,
             'apply_lora': self.apply_lora,
             'tokenizer_padding_side': tokenizer_padding_side,
         }
         self.__cfg.update(kwargs)
 
     def cuda(self):
-        if self.load_kbit is None:
-            self.backbone = self.backbone.to(torch.device(self.device))
+        if self.gpu_count > 1 and self.is_llm:
+            return self
+        self.backbone = self.backbone.to(torch.device(self.device))
         return self
 
     def to(self, device: Any):
         if isinstance(device, str):
             device = torch.device(device)
         self.backbone = self.backbone.to(device)
         self.device = device
```

### Comparing `angle_emb-0.4.3/angle_emb/angle_trainer.py` & `angle_emb-0.4.4/angle_emb/angle_trainer.py`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.3/angle_emb/utils.py` & `angle_emb-0.4.4/angle_emb/utils.py`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.3/angle_emb.egg-info/PKG-INFO` & `angle_emb-0.4.4/angle_emb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angle-emb
-Version: 0.4.3
+Version: 0.4.4
 Summary: AnglE-optimize Text Embeddings
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: angle_emb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -161,28 +161,28 @@
 
 ### ⌛ Infer LLM-based Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 If the pretrained weight is a LoRA-based model, you need to specify the backbone via `model_name_or_path` and specify the LoRA path via the `pretrained_lora_path` in `from_pretrained` method. 
 
 ```python
+import torch
 from angle_emb import AnglE, Prompts
 from angle_emb.utils import cosine_similarity
 
 angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
                               pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
                               pooling_strategy='last',
                               is_llm=True,
-                              torch_dtype='float16').cuda()
-
+                              torch_dtype=torch.float16).cuda()
 print('All predefined prompts:', Prompts.list_prompts())
 doc_vecs = angle.encode([
-    'The weather is great!',
-    'The weather is very good!',
-    'i am going to bed'
+    {'text': 'The weather is great!'},
+    {'text': 'The weather is very good!'},
+    {'text': 'i am going to bed'}
 ], prompt=Prompts.A)
 
 for i, dv1 in enumerate(doc_vecs):
     for dv2 in doc_vecs[i+1:]:
         print(cosine_similarity(dv1, dv2))
 ```
 
@@ -190,36 +190,43 @@
 ### ⌛ Infer BiLLM-based Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 Specify `apply_billm` and `billm_model_class` to load and infer billm models
 
 
 ```python
+import os
+# set an environment variable for billm start index
+os.environ['BiLLM_START_INDEX'] = '31'
+
+import torch
 from angle_emb import AnglE, Prompts
 from angle_emb.utils import cosine_similarity
 
 # specify `apply_billm` and `billm_model_class` to load billm models
 angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
                               pretrained_lora_path='SeanLee97/bellm-llama-7b-nli',
                               pooling_strategy='last',
                               is_llm=True,
                               apply_billm=True,
                               billm_model_class='LlamaForCausalLM',
-                              torch_dtype='float16').cuda()
+                              torch_dtype=torch.float16).cuda()
 
 doc_vecs = angle.encode([
-    'The weather is great!',
-    'The weather is very good!',
-    'i am going to bed'
+    {'text': 'The weather is great!'},
+    {'text': 'The weather is very good!'},
+    {'text': 'i am going to bed'}
 ], prompt='The representative word for sentence {text} is:"')
 
 for i, dv1 in enumerate(doc_vecs):
     for dv2 in doc_vecs[i+1:]:
         print(cosine_similarity(dv1, dv2))
 ```
+
+
 ### ⌛ Infer Espresso/Matryoshka Models
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 
 Specify `layer_index` and `embedding_size` to truncate embeddings.
 
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: angle-emb Version: 0.4.3 Summary: AnglE-optimize
+Metadata-Version: 2.1 Name: angle-emb Version: 0.4.4 Summary: AnglE-optimize
 Text Embeddings Author: sean lee Author-email: xmlee97@gmail.com Keywords:
 angle_emb Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -100,114 +100,118 @@
 angle.encode([ 'The weather is great!', 'The weather is very good!', 'i am
 going to bed' ]) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]:
 print(cosine_similarity(dv1, dv2)) ``` ### â Infer LLM-based Models [![Open
 In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 If the pretrained weight is a LoRA-based model, you need to specify the
 backbone via `model_name_or_path` and specify the LoRA path via the
-`pretrained_lora_path` in `from_pretrained` method. ```python from angle_emb
-import AnglE, Prompts from angle_emb.utils import cosine_similarity angle =
-AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+`pretrained_lora_path` in `from_pretrained` method. ```python import torch from
+angle_emb import AnglE, Prompts from angle_emb.utils import cosine_similarity
+angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
 pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
-pooling_strategy='last', is_llm=True, torch_dtype='float16').cuda() print('All
-predefined prompts:', Prompts.list_prompts()) doc_vecs = angle.encode([ 'The
-weather is great!', 'The weather is very good!', 'i am going to bed' ],
-prompt=Prompts.A) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]:
-print(cosine_similarity(dv1, dv2)) ``` ### â Infer BiLLM-based Models [![Open
-In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+pooling_strategy='last', is_llm=True, torch_dtype=torch.float16).cuda() print
+('All predefined prompts:', Prompts.list_prompts()) doc_vecs = angle.encode([
+{'text': 'The weather is great!'}, {'text': 'The weather is very good!'},
+{'text': 'i am going to bed'} ], prompt=Prompts.A) for i, dv1 in enumerate
+(doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1, dv2)) ```
+### â Infer BiLLM-based Models [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
 Specify `apply_billm` and `billm_model_class` to load and infer billm models
-```python from angle_emb import AnglE, Prompts from angle_emb.utils import
-cosine_similarity # specify `apply_billm` and `billm_model_class` to load billm
-models angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+```python import os # set an environment variable for billm start index
+os.environ['BiLLM_START_INDEX'] = '31' import torch from angle_emb import
+AnglE, Prompts from angle_emb.utils import cosine_similarity # specify
+`apply_billm` and `billm_model_class` to load billm models angle =
+AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
 pretrained_lora_path='SeanLee97/bellm-llama-7b-nli', pooling_strategy='last',
 is_llm=True, apply_billm=True, billm_model_class='LlamaForCausalLM',
-torch_dtype='float16').cuda() doc_vecs = angle.encode([ 'The weather is
-great!', 'The weather is very good!', 'i am going to bed' ], prompt='The
-representative word for sentence {text} is:"') for i, dv1 in enumerate
+torch_dtype=torch.float16).cuda() doc_vecs = angle.encode([ {'text': 'The
+weather is great!'}, {'text': 'The weather is very good!'}, {'text': 'i am
+going to bed'} ], prompt='The representative word for sentence {text} is:"')
+for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]: print
+(cosine_similarity(dv1, dv2)) ``` ### â Infer Espresso/Matryoshka Models [!
+[Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/
+1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing) Specify `layer_index` and
+`embedding_size` to truncate embeddings. ```python from angle_emb import AnglE
+from angle_emb.utils import cosine_similarity angle = AnglE.from_pretrained
+('mixedbread-ai/mxbai-embed-2d-large-v1', pooling_strategy='cls').cuda() #
+specify layer_index and embedding size to truncate embeddings doc_vecs =
+angle.encode([ 'The weather is great!', 'The weather is very good!', 'i am
+going to bed' ], layer_index=22, embedding_size=768) for i, dv1 in enumerate
 (doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1, dv2)) ```
-### â Infer Espresso/Matryoshka Models [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1QJcA2Mvive4pBxWweTpZz9OgwvE42eJZ?usp=sharing)
-Specify `layer_index` and `embedding_size` to truncate embeddings. ```python
-from angle_emb import AnglE from angle_emb.utils import cosine_similarity angle
-= AnglE.from_pretrained('mixedbread-ai/mxbai-embed-2d-large-v1',
-pooling_strategy='cls').cuda() # specify layer_index and embedding size to
-truncate embeddings doc_vecs = angle.encode([ 'The weather is great!', 'The
-weather is very good!', 'i am going to bed' ], layer_index=22,
-embedding_size=768) for i, dv1 in enumerate(doc_vecs): for dv2 in doc_vecs[i+1:
-]: print(cosine_similarity(dv1, dv2)) ``` ### â Infer Third-party Models You
-can load any transformer-based third-party models such as `mixedbread-ai/mxbai-
-embed-large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-
-en-v1.5` using `angle_emb`. Here is an example: ```python from angle_emb import
-AnglE model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1',
-pooling_strategy='cls').cuda() vec = model.encode('hello world', to_numpy=True)
-print(vec) ``` ## ð¸ï¸ Custom Train ### ðï¸ 1. Data Prepation We
-currently support three dataset formats: 1) `DatasetFormats.A`: it is a pair
-format with three columns: `text1`, `text2`, and `label` (0/1). 2)
-`DatasetFormats.B`: it is a triple format with three columns: `text`,
-`positive`, and `negative`. `positive` and `negative` store the positive and
-negative samples of `text`. 3) `DatasetFormats.C`: it is a pair format with two
-columns: `text`, `positive`. `positive` store the positive sample of `text`.
-You need to prepare your data into huggingface `datasets.Dataset` in one of the
-formats in terms of your supervised data. ### ð 2. Train with CLI Use
-`angle-trainer` to train your AnglE model in cli mode. 1) Single gpu training:
-Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-trainer --help ``` 2) Multi-gpu
-training: Usage: ```bash CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 -
--master_port=1234 -m angle_emb.angle_trainer --help ``` ### ð 3. Custom
-Train [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-
-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing) ```python from datasets import load_dataset
-from angle_emb import AnglE, AngleDataTokenizer # 1. load pretrained model
-angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
-max_length=128, pooling_strategy='cls').cuda() # 2. load dataset # `text1`,
-`text2`, and `label` are three required columns. ds = load_dataset('mteb/
-stsbenchmark-sts') ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]),
-"text2": str(obj['sentence2']), "label": obj['score']}) ds = ds.select_columns(
-["text1", "text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle
-().map(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8)
-valid_ds = ds['validation'].map(AngleDataTokenizer(angle.tokenizer,
-angle.max_length), num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer
-(angle.tokenizer, angle.max_length), num_proc=8) # 4. fit angle.fit
-( train_ds=train_ds, valid_ds=valid_ds, output_dir='ckpts/sts-b',
-batch_size=32, epochs=5, learning_rate=2e-5, save_steps=100, eval_steps=1000,
-warmup_steps=0, gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0,
-'ibn_w': 1.0, 'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20
-}, fp16=True, logging_steps=100 ) # 5. evaluate corrcoef, accuracy =
-angle.evaluate(test_ds, device=angle.device) print('corrcoef:', corrcoef) ```
-### ð¡ Others - To enable `llm` training, please specify `--is_llm 1` and
-configure appropriate LoRA hyperparameters. - To enable `billm` training,
-please specify `--apply_billm 1` and configure appropriate `billm_model_class`
-such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/
-BiLLM?tab=readme-ov-file#usage). - To enable espresso sentence embeddings
-(ESE), please specify `--apply_ese 1` and configure appropriate ESE
-hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size
-integer`. - To convert the trained AnglE models to `sentence-transformers`,
-please run `python scripts/convert_to_sentence_transformers.py --help` for more
-details. ## ð¡ 4. Fine-tuning Tips 1ï¸â£ If your dataset format is
-`DatasetFormats.A`, it is recommended to slightly increase the weight for
-`cosine_w` or slightly decrease the weight for `ibn_w`. 2ï¸â£ If your dataset
-format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and
-increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is
-recommended to set to 20.0. 3ï¸â£ If your dataset format is
-`DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to
-tune other parameters. 4ï¸â£ To alleviate information forgetting in fine-
-tuning, it is better to specify the `teacher_name_or_path`. If the
-`teacher_name_or_path` equals `model_name_or_path`, it will conduct self-
-distillation. **It is worth to note that** `teacher_name_or_path` has to have
-the same tokenizer as `model_name_or_path`. Or it will lead to unexpected
-results. # ð«¡ Citation You are welcome to use our code and pre-trained
-models. If you use our code and pre-trained models, please support us by citing
-our work as follows: ```bibtex @article{li2023angle, title={AnglE-optimized
-Text Embeddings}, author={Li, Xianming and Li, Jing}, journal={arXiv preprint
-arXiv:2309.12871}, year={2023} } ``` # ð ChangeLogs | ð | Description |
-|----|------| | 2024 May 21 | support Espresso Sentence Embeddings | | 2024 Feb
-7 | support training with only positive pairs (`DatasetFormats.C`) | | 2023 Dec
-4 | Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-
-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an
-English pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 |
-Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-
-v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§
-Contact If you have any questions or suggestions, please feel free to contact
-us via email: xmlee97@gmail.com # Â© License This project is licensed under the
-MIT License. For the pretrained models, please refer to the corresponding
-license of the models.
+### â Infer Third-party Models You can load any transformer-based third-party
+models such as `mixedbread-ai/mxbai-embed-large-v1`, `sentence-transformers/
+all-MiniLM-L6-v2`, and `BAAI/bge-large-en-v1.5` using `angle_emb`. Here is an
+example: ```python from angle_emb import AnglE model = AnglE.from_pretrained
+('mixedbread-ai/mxbai-embed-large-v1', pooling_strategy='cls').cuda() vec =
+model.encode('hello world', to_numpy=True) print(vec) ``` ## ð¸ï¸ Custom
+Train ### ðï¸ 1. Data Prepation We currently support three dataset formats:
+1) `DatasetFormats.A`: it is a pair format with three columns: `text1`,
+`text2`, and `label` (0/1). 2) `DatasetFormats.B`: it is a triple format with
+three columns: `text`, `positive`, and `negative`. `positive` and `negative`
+store the positive and negative samples of `text`. 3) `DatasetFormats.C`: it is
+a pair format with two columns: `text`, `positive`. `positive` store the
+positive sample of `text`. You need to prepare your data into huggingface
+`datasets.Dataset` in one of the formats in terms of your supervised data. ###
+ð 2. Train with CLI Use `angle-trainer` to train your AnglE model in cli
+mode. 1) Single gpu training: Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-
+trainer --help ``` 2) Multi-gpu training: Usage: ```bash
+CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 --master_port=1234 -
+m angle_emb.angle_trainer --help ``` ### ð 3. Custom Train [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
+```python from datasets import load_dataset from angle_emb import AnglE,
+AngleDataTokenizer # 1. load pretrained model angle = AnglE.from_pretrained
+('SeanLee97/angle-bert-base-uncased-nli-en-v1', max_length=128,
+pooling_strategy='cls').cuda() # 2. load dataset # `text1`, `text2`, and
+`label` are three required columns. ds = load_dataset('mteb/stsbenchmark-sts')
+ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]), "text2": str(obj
+['sentence2']), "label": obj['score']}) ds = ds.select_columns(["text1",
+"text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle().map
+(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8) valid_ds =
+ds['validation'].map(AngleDataTokenizer(angle.tokenizer, angle.max_length),
+num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer(angle.tokenizer,
+angle.max_length), num_proc=8) # 4. fit angle.fit( train_ds=train_ds,
+valid_ds=valid_ds, output_dir='ckpts/sts-b', batch_size=32, epochs=5,
+learning_rate=2e-5, save_steps=100, eval_steps=1000, warmup_steps=0,
+gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0, 'ibn_w': 1.0,
+'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20 }, fp16=True,
+logging_steps=100 ) # 5. evaluate corrcoef, accuracy = angle.evaluate(test_ds,
+device=angle.device) print('corrcoef:', corrcoef) ``` ### ð¡ Others - To
+enable `llm` training, please specify `--is_llm 1` and configure appropriate
+LoRA hyperparameters. - To enable `billm` training, please specify `--
+apply_billm 1` and configure appropriate `billm_model_class` such as
+`LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/BiLLM?tab=readme-ov-
+file#usage). - To enable espresso sentence embeddings (ESE), please specify `--
+apply_ese 1` and configure appropriate ESE hyperparameters via `--
+ese_kl_temperature float` and `--ese_compression_size integer`. - To convert
+the trained AnglE models to `sentence-transformers`, please run `python
+scripts/convert_to_sentence_transformers.py --help` for more details. ## ð¡
+4. Fine-tuning Tips 1ï¸â£ If your dataset format is `DatasetFormats.A`, it is
+recommended to slightly increase the weight for `cosine_w` or slightly decrease
+the weight for `ibn_w`. 2ï¸â£ If your dataset format is `DatasetFormats.B`,
+it is recommended to set `cosine_w` to 0, and increase the weight for `ibn_w`
+such as 10 and 20. The `angle_tau` is recommended to set to 20.0. 3ï¸â£ If
+your dataset format is `DatasetFormats.C`, only `ibn_w` and `ibn_tau` are
+effective. You don't need to tune other parameters. 4ï¸â£ To alleviate
+information forgetting in fine-tuning, it is better to specify the
+`teacher_name_or_path`. If the `teacher_name_or_path` equals
+`model_name_or_path`, it will conduct self-distillation. **It is worth to note
+that** `teacher_name_or_path` has to have the same tokenizer as
+`model_name_or_path`. Or it will lead to unexpected results. # ð«¡ Citation
+You are welcome to use our code and pre-trained models. If you use our code and
+pre-trained models, please support us by citing our work as follows: ```bibtex
+@article{li2023angle, title={AnglE-optimized Text Embeddings}, author={Li,
+Xianming and Li, Jing}, journal={arXiv preprint arXiv:2309.12871}, year={2023}
+} ``` # ð ChangeLogs | ð | Description | |----|------| | 2024 May 21 |
+support Espresso Sentence Embeddings | | 2024 Feb 7 | support training with
+only positive pairs (`DatasetFormats.C`) | | 2023 Dec 4 | Release a universal
+English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://
+huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an English
+pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 | Release two
+chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and
+`SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§ Contact If
+you have any questions or suggestions, please feel free to contact us via
+email: xmlee97@gmail.com # Â© License This project is licensed under the MIT
+License. For the pretrained models, please refer to the corresponding license
+of the models.
```

### Comparing `angle_emb-0.4.3/setup.py` & `angle_emb-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     requirements = [l for l in f.read().splitlines() if l]
 
 with open('dev-requirements.txt', encoding='utf-8') as f:
     test_requirements = [l for l in f.read().splitlines() if l][1:]
 
 setup(
     name='angle_emb',
-    version='0.4.3',
+    version='0.4.4',
     description='AnglE-optimize Text Embeddings',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='sean lee',
     author_email='xmlee97@gmail.com',
     packages=find_packages(exclude=("tests", "tests.*", "examples", "examples.*")),
     install_requires=requirements,
```

