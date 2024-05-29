# Comparing `tmp/dspy_ai-2.5.0rc1.tar.gz` & `tmp/dspy_ai-2.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspy_ai-2.5.0rc1.tar", max compression
+gzip compressed data, was "dspy_ai-2.5.0rc2.tar", max compression
```

## Comparing `dspy_ai-2.5.0rc1.tar` & `dspy_ai-2.5.0rc2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1085 2024-01-27 20:16:46.845164 dspy_ai-2.5.0rc1/LICENSE
--rw-r--r--   0        0        0    35950 2024-05-27 13:53:59.380701 dspy_ai-2.5.0rc1/README.md
--rw-r--r--   0        0        0     1180 2024-05-27 13:54:02.462908 dspy_ai-2.5.0rc1/dspy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 13:54:02.462971 dspy_ai-2.5.0rc1/dspy/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 13:54:02.463017 dspy_ai-2.5.0rc1/dspy/adapters/basic_adapter.py
--rw-r--r--   0        0        0        0 2024-05-27 13:54:02.463052 dspy_ai-2.5.0rc1/dspy/adapters/chatml_adapter.py
--rw-r--r--   0        0        0        0 2024-05-27 13:54:02.463085 dspy_ai-2.5.0rc1/dspy/adapters/llamachat_adapter.py
--rw-r--r--   0        0        0        0 2024-05-27 13:54:02.463120 dspy_ai-2.5.0rc1/dspy/adapters/vicuna_adapter.py
--rw-r--r--   0        0        0      122 2024-04-05 16:07:52.848121 dspy_ai-2.5.0rc1/dspy/datasets/__init__.py
--rw-r--r--   0        0        0     2986 2024-04-05 16:07:52.848222 dspy_ai-2.5.0rc1/dspy/datasets/colors.py
--rw-r--r--   0        0        0     4949 2024-05-27 13:54:02.463273 dspy_ai-2.5.0rc1/dspy/datasets/dataloader.py
--rw-r--r--   0        0        0     4098 2024-04-05 16:07:52.848414 dspy_ai-2.5.0rc1/dspy/datasets/dataset.py
--rw-r--r--   0        0        0     2618 2024-04-05 16:07:52.848498 dspy_ai-2.5.0rc1/dspy/datasets/gsm8k.py
--rw-r--r--   0        0        0     3286 2024-04-05 16:07:52.848598 dspy_ai-2.5.0rc1/dspy/datasets/hotpotqa.py
--rw-r--r--   0        0        0      127 2024-04-05 16:07:52.848699 dspy_ai-2.5.0rc1/dspy/evaluate/__init__.py
--rw-r--r--   0        0        0     1421 2024-04-05 16:07:52.848822 dspy_ai-2.5.0rc1/dspy/evaluate/auto_evaluation.py
--rw-r--r--   0        0        0    11414 2024-05-27 13:53:59.390403 dspy_ai-2.5.0rc1/dspy/evaluate/evaluate.py
--rw-r--r--   0        0        0      882 2024-04-05 16:07:52.852527 dspy_ai-2.5.0rc1/dspy/evaluate/metrics.py
--rw-r--r--   0        0        0       57 2024-04-05 16:07:52.852610 dspy_ai-2.5.0rc1/dspy/experimental/__init__.py
--rw-r--r--   0        0        0       26 2024-04-05 16:07:52.852700 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/__init__.py
--rw-r--r--   0        0        0      834 2024-04-05 16:07:52.852759 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/config.py
--rw-r--r--   0        0        0      527 2024-04-05 16:07:52.852825 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/instruction_suffixes.py
--rw-r--r--   0        0        0     5543 2024-04-05 16:07:52.852897 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/signatures.py
--rw-r--r--   0        0        0     9723 2024-05-27 13:54:02.463457 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/synthesizer.py
--rw-r--r--   0        0        0      599 2024-04-05 16:07:52.853143 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/utils.py
--rw-r--r--   0        0        0     4237 2024-05-27 13:53:59.390647 dspy_ai-2.5.0rc1/dspy/experimental/synthetic_data.py
--rw-r--r--   0        0        0       94 2024-04-05 16:07:52.853820 dspy_ai-2.5.0rc1/dspy/functional/__init__.py
--rw-r--r--   0        0        0    19491 2024-05-27 13:54:02.463645 dspy_ai-2.5.0rc1/dspy/functional/functional.py
--rw-r--r--   0        0        0      348 2024-04-05 16:07:52.854456 dspy_ai-2.5.0rc1/dspy/predict/__init__.py
--rw-r--r--   0        0        0     1842 2024-05-27 13:54:02.463800 dspy_ai-2.5.0rc1/dspy/predict/aggregation.py
--rw-r--r--   0        0        0     3589 2024-04-05 16:07:52.854648 dspy_ai-2.5.0rc1/dspy/predict/chain_of_thought.py
--rw-r--r--   0        0        0     1527 2024-04-05 16:07:52.854742 dspy_ai-2.5.0rc1/dspy/predict/chain_of_thought_with_hint.py
--rw-r--r--   0        0        0     1133 2024-05-27 13:53:59.392833 dspy_ai-2.5.0rc1/dspy/predict/knn.py
--rw-r--r--   0        0        0     6129 2024-05-27 13:53:59.392953 dspy_ai-2.5.0rc1/dspy/predict/langchain.py
--rw-r--r--   0        0        0     1659 2024-04-05 16:07:52.855060 dspy_ai-2.5.0rc1/dspy/predict/multi_chain_comparison.py
--rw-r--r--   0        0        0       58 2024-01-27 20:16:47.215842 dspy_ai-2.5.0rc1/dspy/predict/parameter.py
--rw-r--r--   0        0        0     5580 2024-05-27 13:54:02.463936 dspy_ai-2.5.0rc1/dspy/predict/predict.py
--rw-r--r--   0        0        0     7603 2024-05-27 13:54:02.464078 dspy_ai-2.5.0rc1/dspy/predict/program_of_thought.py
--rw-r--r--   0        0        0     4614 2024-05-27 13:53:59.393278 dspy_ai-2.5.0rc1/dspy/predict/react.py
--rw-r--r--   0        0        0     2977 2024-05-27 13:54:02.464208 dspy_ai-2.5.0rc1/dspy/predict/retry.py
--rw-r--r--   0        0        0      132 2024-04-05 16:07:52.855575 dspy_ai-2.5.0rc1/dspy/primitives/__init__.py
--rw-r--r--   0        0        0    11319 2024-05-27 13:53:59.393559 dspy_ai-2.5.0rc1/dspy/primitives/assertions.py
--rw-r--r--   0        0        0     7779 2024-01-27 20:16:47.216399 dspy_ai-2.5.0rc1/dspy/primitives/box.py
--rw-r--r--   0        0        0     3471 2024-05-27 13:54:02.464335 dspy_ai-2.5.0rc1/dspy/primitives/example.py
--rw-r--r--   0        0        0     3831 2024-05-27 13:53:59.393756 dspy_ai-2.5.0rc1/dspy/primitives/module.py
--rw-r--r--   0        0        0     2807 2024-05-27 13:54:02.464463 dspy_ai-2.5.0rc1/dspy/primitives/prediction.py
--rw-r--r--   0        0        0     3366 2024-04-05 16:07:52.856229 dspy_ai-2.5.0rc1/dspy/primitives/program.py
--rw-r--r--   0        0        0    25710 2024-04-05 16:07:52.856677 dspy_ai-2.5.0rc1/dspy/primitives/python_interpreter.py
--rw-r--r--   0        0        0       30 2024-01-27 20:16:47.216808 dspy_ai-2.5.0rc1/dspy/retrieve/__init__.py
--rw-r--r--   0        0        0    17405 2024-05-27 13:53:59.393937 dspy_ai-2.5.0rc1/dspy/retrieve/azureaisearch_rm.py
--rw-r--r--   0        0        0     5719 2024-05-27 13:54:02.464622 dspy_ai-2.5.0rc1/dspy/retrieve/chromadb_rm.py
--rw-r--r--   0        0        0     3275 2024-05-27 13:54:02.464778 dspy_ai-2.5.0rc1/dspy/retrieve/clarifai_rm.py
--rw-r--r--   0        0        0     6604 2024-05-27 13:53:59.394297 dspy_ai-2.5.0rc1/dspy/retrieve/databricks_rm.py
--rw-r--r--   0        0        0     3897 2024-05-27 13:54:02.464886 dspy_ai-2.5.0rc1/dspy/retrieve/deeplake_rm.py
--rwxr-xr-x   0        0        0     6605 2024-05-27 13:53:59.394532 dspy_ai-2.5.0rc1/dspy/retrieve/faiss_rm.py
--rw-r--r--   0        0        0     2937 2024-05-27 13:53:59.394597 dspy_ai-2.5.0rc1/dspy/retrieve/llama_index_rm.py
--rw-r--r--   0        0        0     3459 2024-04-05 16:07:52.857777 dspy_ai-2.5.0rc1/dspy/retrieve/marqo_rm.py
--rw-r--r--   0        0        0     3998 2024-05-27 13:53:59.394660 dspy_ai-2.5.0rc1/dspy/retrieve/milvus_rm.py
--rw-r--r--   0        0        0     3774 2024-04-05 16:07:52.857887 dspy_ai-2.5.0rc1/dspy/retrieve/mongodb_atlas_rm.py
--rw-r--r--   0        0        0     6213 2024-04-05 16:07:52.857964 dspy_ai-2.5.0rc1/dspy/retrieve/neo4j_rm.py
--rw-r--r--   0        0        0     5930 2024-05-27 13:54:02.465032 dspy_ai-2.5.0rc1/dspy/retrieve/pgvector_rm.py
--rw-r--r--   0        0        0    10476 2024-04-05 16:07:52.858267 dspy_ai-2.5.0rc1/dspy/retrieve/pinecone_rm.py
--rw-r--r--   0        0        0     4951 2024-05-27 13:53:59.394882 dspy_ai-2.5.0rc1/dspy/retrieve/qdrant_rm.py
--rw-r--r--   0        0        0     2425 2024-05-27 13:53:59.394959 dspy_ai-2.5.0rc1/dspy/retrieve/ragatouille_rm.py
--rw-r--r--   0        0        0     1442 2024-05-27 13:54:02.465140 dspy_ai-2.5.0rc1/dspy/retrieve/retrieve.py
--rw-r--r--   0        0        0     4575 2024-05-27 13:53:59.395131 dspy_ai-2.5.0rc1/dspy/retrieve/snowflake_rm.py
--rw-r--r--   0        0        0     5923 2024-05-27 13:53:59.395244 dspy_ai-2.5.0rc1/dspy/retrieve/vectara_rm.py
--rw-r--r--   0        0        0     4491 2024-05-27 13:54:02.465274 dspy_ai-2.5.0rc1/dspy/retrieve/weaviate_rm.py
--rw-r--r--   0        0        0      438 2024-02-10 21:45:26.556459 dspy_ai-2.5.0rc1/dspy/retrieve/weaviate_rm_test.py
--rw-r--r--   0        0        0     1678 2024-04-05 16:07:52.859233 dspy_ai-2.5.0rc1/dspy/retrieve/you_rm.py
--rw-r--r--   0        0        0       46 2024-01-27 20:16:47.217346 dspy_ai-2.5.0rc1/dspy/signatures/__init__.py
--rw-r--r--   0        0        0     2758 2024-04-05 16:07:52.859642 dspy_ai-2.5.0rc1/dspy/signatures/field.py
--rw-r--r--   0        0        0    14509 2024-05-27 13:54:02.465439 dspy_ai-2.5.0rc1/dspy/signatures/signature.py
--rw-r--r--   0        0        0      390 2024-04-05 16:07:52.860050 dspy_ai-2.5.0rc1/dspy/teleprompt/__init__.py
--rw-r--r--   0        0        0    10819 2024-05-27 13:54:02.465612 dspy_ai-2.5.0rc1/dspy/teleprompt/bootstrap.py
--rw-r--r--   0        0        0    18048 2024-05-27 13:54:02.465752 dspy_ai-2.5.0rc1/dspy/teleprompt/copro_optimizer.py
--rw-r--r--   0        0        0     1359 2024-04-05 16:07:52.860514 dspy_ai-2.5.0rc1/dspy/teleprompt/ensemble.py
--rw-r--r--   0        0        0     6292 2024-04-05 16:07:52.860625 dspy_ai-2.5.0rc1/dspy/teleprompt/finetune.py
--rw-r--r--   0        0        0     1002 2024-05-27 13:53:59.396186 dspy_ai-2.5.0rc1/dspy/teleprompt/knn_fewshot.py
--rw-r--r--   0        0        0    31123 2024-05-27 13:54:02.465932 dspy_ai-2.5.0rc1/dspy/teleprompt/mipro_optimizer.py
--rw-r--r--   0        0        0     8130 2024-05-27 13:53:59.396477 dspy_ai-2.5.0rc1/dspy/teleprompt/random_search.py
--rw-r--r--   0        0        0     2673 2024-05-27 13:53:59.396900 dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt.py
--rw-r--r--   0        0        0     3878 2024-04-05 16:07:52.861256 dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt_bayesian.py
--rw-r--r--   0        0        0    11876 2024-04-05 16:07:52.861442 dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt_typed.py
--rw-r--r--   0        0        0       57 2024-04-05 16:07:52.861522 dspy_ai-2.5.0rc1/dspy/teleprompt/teleprompt.py
--rw-r--r--   0        0        0     3206 2024-05-27 13:53:59.397045 dspy_ai-2.5.0rc1/dspy/teleprompt/teleprompt_optuna.py
--rw-r--r--   0        0        0      948 2024-04-05 16:07:52.861703 dspy_ai-2.5.0rc1/dspy/teleprompt/vanilla.py
--rw-r--r--   0        0        0       46 2024-05-27 13:53:59.397185 dspy_ai-2.5.0rc1/dspy/utils/__init__.py
--rw-r--r--   0        0        0     5643 2024-05-27 13:54:02.466118 dspy_ai-2.5.0rc1/dspy/utils/dummies.py
--rw-r--r--   0        0        0     3193 2024-05-27 13:53:59.397403 dspy_ai-2.5.0rc1/dspy/utils/logging.py
--rw-r--r--   0        0        0     7736 2024-05-27 14:12:47.032650 dspy_ai-2.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0    38956 1970-01-01 00:00:00.000000 dspy_ai-2.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-01-27 20:16:46.845164 dspy_ai-2.5.0rc2/LICENSE
+-rw-r--r--   0        0        0    35950 2024-05-27 13:53:59.380701 dspy_ai-2.5.0rc2/README.md
+-rw-r--r--   0        0        0     1204 2024-05-29 20:05:59.696560 dspy_ai-2.5.0rc2/dspy/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-05 16:07:52.848121 dspy_ai-2.5.0rc2/dspy/datasets/__init__.py
+-rw-r--r--   0        0        0     2986 2024-04-05 16:07:52.848222 dspy_ai-2.5.0rc2/dspy/datasets/colors.py
+-rw-r--r--   0        0        0     5162 2024-05-29 20:05:59.696687 dspy_ai-2.5.0rc2/dspy/datasets/dataloader.py
+-rw-r--r--   0        0        0     4098 2024-04-05 16:07:52.848414 dspy_ai-2.5.0rc2/dspy/datasets/dataset.py
+-rw-r--r--   0        0        0     2618 2024-04-05 16:07:52.848498 dspy_ai-2.5.0rc2/dspy/datasets/gsm8k.py
+-rw-r--r--   0        0        0     3286 2024-04-05 16:07:52.848598 dspy_ai-2.5.0rc2/dspy/datasets/hotpotqa.py
+-rw-r--r--   0        0        0      127 2024-04-05 16:07:52.848699 dspy_ai-2.5.0rc2/dspy/evaluate/__init__.py
+-rw-r--r--   0        0        0     1421 2024-04-05 16:07:52.848822 dspy_ai-2.5.0rc2/dspy/evaluate/auto_evaluation.py
+-rw-r--r--   0        0        0    11414 2024-05-27 13:53:59.390403 dspy_ai-2.5.0rc2/dspy/evaluate/evaluate.py
+-rw-r--r--   0        0        0      882 2024-04-05 16:07:52.852527 dspy_ai-2.5.0rc2/dspy/evaluate/metrics.py
+-rw-r--r--   0        0        0       57 2024-04-05 16:07:52.852610 dspy_ai-2.5.0rc2/dspy/experimental/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-05 16:07:52.852700 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/__init__.py
+-rw-r--r--   0        0        0      834 2024-04-05 16:07:52.852759 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/config.py
+-rw-r--r--   0        0        0      527 2024-04-05 16:07:52.852825 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/instruction_suffixes.py
+-rw-r--r--   0        0        0     5543 2024-04-05 16:07:52.852897 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/signatures.py
+-rw-r--r--   0        0        0     9567 2024-05-29 20:05:59.696817 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/synthesizer.py
+-rw-r--r--   0        0        0      599 2024-04-05 16:07:52.853143 dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/utils.py
+-rw-r--r--   0        0        0     4237 2024-05-27 13:53:59.390647 dspy_ai-2.5.0rc2/dspy/experimental/synthetic_data.py
+-rw-r--r--   0        0        0       94 2024-04-05 16:07:52.853820 dspy_ai-2.5.0rc2/dspy/functional/__init__.py
+-rw-r--r--   0        0        0    20120 2024-05-29 20:05:59.696945 dspy_ai-2.5.0rc2/dspy/functional/functional.py
+-rw-r--r--   0        0        0       47 2024-05-29 20:05:59.697246 dspy_ai-2.5.0rc2/dspy/modeling/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-29 20:05:59.697326 dspy_ai-2.5.0rc2/dspy/modeling/backends/__init__.py
+-rw-r--r--   0        0        0     4724 2024-05-29 20:05:59.697392 dspy_ai-2.5.0rc2/dspy/modeling/backends/base.py
+-rw-r--r--   0        0        0     3777 2024-05-29 20:05:59.697443 dspy_ai-2.5.0rc2/dspy/modeling/backends/json.py
+-rw-r--r--   0        0        0     7459 2024-05-29 20:05:59.697507 dspy_ai-2.5.0rc2/dspy/modeling/backends/text.py
+-rw-r--r--   0        0        0      348 2024-04-05 16:07:52.854456 dspy_ai-2.5.0rc2/dspy/predict/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-29 20:05:59.697772 dspy_ai-2.5.0rc2/dspy/predict/aggregation.py
+-rw-r--r--   0        0        0     3589 2024-04-05 16:07:52.854648 dspy_ai-2.5.0rc2/dspy/predict/chain_of_thought.py
+-rw-r--r--   0        0        0     1527 2024-04-05 16:07:52.854742 dspy_ai-2.5.0rc2/dspy/predict/chain_of_thought_with_hint.py
+-rw-r--r--   0        0        0     1133 2024-05-27 13:53:59.392833 dspy_ai-2.5.0rc2/dspy/predict/knn.py
+-rw-r--r--   0        0        0     6129 2024-05-27 13:53:59.392953 dspy_ai-2.5.0rc2/dspy/predict/langchain.py
+-rw-r--r--   0        0        0     1659 2024-04-05 16:07:52.855060 dspy_ai-2.5.0rc2/dspy/predict/multi_chain_comparison.py
+-rw-r--r--   0        0        0       58 2024-01-27 20:16:47.215842 dspy_ai-2.5.0rc2/dspy/predict/parameter.py
+-rw-r--r--   0        0        0     7252 2024-05-29 20:05:59.697915 dspy_ai-2.5.0rc2/dspy/predict/predict.py
+-rw-r--r--   0        0        0     7598 2024-05-29 20:05:59.698038 dspy_ai-2.5.0rc2/dspy/predict/program_of_thought.py
+-rw-r--r--   0        0        0     4614 2024-05-27 13:53:59.393278 dspy_ai-2.5.0rc2/dspy/predict/react.py
+-rw-r--r--   0        0        0     3115 2024-05-29 20:05:59.698147 dspy_ai-2.5.0rc2/dspy/predict/retry.py
+-rw-r--r--   0        0        0      132 2024-04-05 16:07:52.855575 dspy_ai-2.5.0rc2/dspy/primitives/__init__.py
+-rw-r--r--   0        0        0    11319 2024-05-27 13:53:59.393559 dspy_ai-2.5.0rc2/dspy/primitives/assertions.py
+-rw-r--r--   0        0        0     7779 2024-01-27 20:16:47.216399 dspy_ai-2.5.0rc2/dspy/primitives/box.py
+-rw-r--r--   0        0        0     3416 2024-05-29 20:05:59.698251 dspy_ai-2.5.0rc2/dspy/primitives/example.py
+-rw-r--r--   0        0        0     3831 2024-05-27 13:53:59.393756 dspy_ai-2.5.0rc2/dspy/primitives/module.py
+-rw-r--r--   0        0        0     4836 2024-05-29 20:05:59.698359 dspy_ai-2.5.0rc2/dspy/primitives/prediction.py
+-rw-r--r--   0        0        0     3366 2024-04-05 16:07:52.856229 dspy_ai-2.5.0rc2/dspy/primitives/program.py
+-rw-r--r--   0        0        0    25710 2024-04-05 16:07:52.856677 dspy_ai-2.5.0rc2/dspy/primitives/python_interpreter.py
+-rw-r--r--   0        0        0       30 2024-01-27 20:16:47.216808 dspy_ai-2.5.0rc2/dspy/retrieve/__init__.py
+-rw-r--r--   0        0        0    17405 2024-05-27 13:53:59.393937 dspy_ai-2.5.0rc2/dspy/retrieve/azureaisearch_rm.py
+-rw-r--r--   0        0        0     5683 2024-05-29 20:05:59.698525 dspy_ai-2.5.0rc2/dspy/retrieve/chromadb_rm.py
+-rw-r--r--   0        0        0     3264 2024-05-29 20:05:59.698629 dspy_ai-2.5.0rc2/dspy/retrieve/clarifai_rm.py
+-rw-r--r--   0        0        0     6604 2024-05-27 13:53:59.394297 dspy_ai-2.5.0rc2/dspy/retrieve/databricks_rm.py
+-rw-r--r--   0        0        0     3804 2024-05-29 20:05:59.698742 dspy_ai-2.5.0rc2/dspy/retrieve/deeplake_rm.py
+-rwxr-xr-x   0        0        0     6605 2024-05-27 13:53:59.394532 dspy_ai-2.5.0rc2/dspy/retrieve/faiss_rm.py
+-rw-r--r--   0        0        0     2937 2024-05-27 13:53:59.394597 dspy_ai-2.5.0rc2/dspy/retrieve/llama_index_rm.py
+-rw-r--r--   0        0        0     3459 2024-04-05 16:07:52.857777 dspy_ai-2.5.0rc2/dspy/retrieve/marqo_rm.py
+-rw-r--r--   0        0        0     3998 2024-05-27 13:53:59.394660 dspy_ai-2.5.0rc2/dspy/retrieve/milvus_rm.py
+-rw-r--r--   0        0        0     3774 2024-04-05 16:07:52.857887 dspy_ai-2.5.0rc2/dspy/retrieve/mongodb_atlas_rm.py
+-rw-r--r--   0        0        0     6213 2024-04-05 16:07:52.857964 dspy_ai-2.5.0rc2/dspy/retrieve/neo4j_rm.py
+-rw-r--r--   0        0        0     5904 2024-05-29 20:05:59.698885 dspy_ai-2.5.0rc2/dspy/retrieve/pgvector_rm.py
+-rw-r--r--   0        0        0    10476 2024-04-05 16:07:52.858267 dspy_ai-2.5.0rc2/dspy/retrieve/pinecone_rm.py
+-rw-r--r--   0        0        0     4951 2024-05-27 13:53:59.394882 dspy_ai-2.5.0rc2/dspy/retrieve/qdrant_rm.py
+-rw-r--r--   0        0        0     2425 2024-05-27 13:53:59.394959 dspy_ai-2.5.0rc2/dspy/retrieve/ragatouille_rm.py
+-rw-r--r--   0        0        0     1443 2024-05-29 20:05:59.698981 dspy_ai-2.5.0rc2/dspy/retrieve/retrieve.py
+-rw-r--r--   0        0        0     4575 2024-05-27 13:53:59.395131 dspy_ai-2.5.0rc2/dspy/retrieve/snowflake_rm.py
+-rw-r--r--   0        0        0     5923 2024-05-27 13:53:59.395244 dspy_ai-2.5.0rc2/dspy/retrieve/vectara_rm.py
+-rw-r--r--   0        0        0     4373 2024-05-29 20:05:59.699111 dspy_ai-2.5.0rc2/dspy/retrieve/weaviate_rm.py
+-rw-r--r--   0        0        0      438 2024-02-10 21:45:26.556459 dspy_ai-2.5.0rc2/dspy/retrieve/weaviate_rm_test.py
+-rw-r--r--   0        0        0     1678 2024-04-05 16:07:52.859233 dspy_ai-2.5.0rc2/dspy/retrieve/you_rm.py
+-rw-r--r--   0        0        0       46 2024-01-27 20:16:47.217346 dspy_ai-2.5.0rc2/dspy/signatures/__init__.py
+-rw-r--r--   0        0        0     2758 2024-04-05 16:07:52.859642 dspy_ai-2.5.0rc2/dspy/signatures/field.py
+-rw-r--r--   0        0        0    14752 2024-05-29 20:05:59.699252 dspy_ai-2.5.0rc2/dspy/signatures/signature.py
+-rw-r--r--   0        0        0      390 2024-04-05 16:07:52.860050 dspy_ai-2.5.0rc2/dspy/teleprompt/__init__.py
+-rw-r--r--   0        0        0    11291 2024-05-29 20:05:59.699407 dspy_ai-2.5.0rc2/dspy/teleprompt/bootstrap.py
+-rw-r--r--   0        0        0    17725 2024-05-29 20:05:59.699529 dspy_ai-2.5.0rc2/dspy/teleprompt/copro_optimizer.py
+-rw-r--r--   0        0        0     1359 2024-04-05 16:07:52.860514 dspy_ai-2.5.0rc2/dspy/teleprompt/ensemble.py
+-rw-r--r--   0        0        0     6292 2024-04-05 16:07:52.860625 dspy_ai-2.5.0rc2/dspy/teleprompt/finetune.py
+-rw-r--r--   0        0        0     1002 2024-05-27 13:53:59.396186 dspy_ai-2.5.0rc2/dspy/teleprompt/knn_fewshot.py
+-rw-r--r--   0        0        0    31024 2024-05-29 20:05:59.699712 dspy_ai-2.5.0rc2/dspy/teleprompt/mipro_optimizer.py
+-rw-r--r--   0        0        0     8130 2024-05-27 13:53:59.396477 dspy_ai-2.5.0rc2/dspy/teleprompt/random_search.py
+-rw-r--r--   0        0        0     2673 2024-05-27 13:53:59.396900 dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt.py
+-rw-r--r--   0        0        0     3878 2024-04-05 16:07:52.861256 dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt_bayesian.py
+-rw-r--r--   0        0        0    11876 2024-04-05 16:07:52.861442 dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt_typed.py
+-rw-r--r--   0        0        0       57 2024-04-05 16:07:52.861522 dspy_ai-2.5.0rc2/dspy/teleprompt/teleprompt.py
+-rw-r--r--   0        0        0     3206 2024-05-27 13:53:59.397045 dspy_ai-2.5.0rc2/dspy/teleprompt/teleprompt_optuna.py
+-rw-r--r--   0        0        0      948 2024-04-05 16:07:52.861703 dspy_ai-2.5.0rc2/dspy/teleprompt/vanilla.py
+-rw-r--r--   0        0        0       46 2024-05-27 13:53:59.397185 dspy_ai-2.5.0rc2/dspy/utils/__init__.py
+-rw-r--r--   0        0        0     7299 2024-05-29 20:05:59.699849 dspy_ai-2.5.0rc2/dspy/utils/dummies.py
+-rw-r--r--   0        0        0     3193 2024-05-27 13:53:59.397403 dspy_ai-2.5.0rc2/dspy/utils/logging.py
+-rw-r--r--   0        0        0     7736 2024-05-29 20:12:43.027428 dspy_ai-2.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    38956 1970-01-01 00:00:00.000000 dspy_ai-2.5.0rc2/PKG-INFO
```

### Comparing `dspy_ai-2.5.0rc1/LICENSE` & `dspy_ai-2.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/README.md` & `dspy_ai-2.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/__init__.py` & `dspy_ai-2.5.0rc2/dspy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dsp
 from dsp.modules.hf_client import ChatModuleClient, HFClientSGLang, HFClientVLLM, HFServerTGI
 
+from .modeling import *
 from .predict import *
 from .primitives import *
 from .retrieve import *
 from .signatures import *
 from .utils.logging import logger, set_log_output
 
 # Functional must be imported after primitives, predict and signatures
```

### Comparing `dspy_ai-2.5.0rc1/dspy/datasets/colors.py` & `dspy_ai-2.5.0rc2/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/datasets/dataloader.py` & `dspy_ai-2.5.0rc2/dspy/datasets/dataloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from datasets import load_dataset
 
 import dspy
 from dspy.datasets.dataset import Dataset
 
 
 class DataLoader(Dataset):
-    def __init__(self,):
+    def __init__(
+        self,
+    ):
         pass
 
     def from_huggingface(
         self,
         dataset_name: str,
         *args,
         input_keys: Tuple[str] = (),
@@ -23,48 +25,59 @@
         if fields and not isinstance(fields, tuple):
             raise ValueError("Invalid fields provided. Please provide a tuple of fields.")
 
         if not isinstance(input_keys, tuple):
             raise ValueError("Invalid input keys provided. Please provide a tuple of input keys.")
 
         dataset = load_dataset(dataset_name, *args, **kwargs)
-        
+
         if isinstance(dataset, list) and isinstance(kwargs["split"], list):
-            dataset = {split_name:dataset[idx] for idx, split_name in enumerate(kwargs["split"])}
+            dataset = {split_name: dataset[idx] for idx, split_name in enumerate(kwargs["split"])}
 
         try:
             returned_split = {}
             for split_name in dataset.keys():
                 if fields:
-                    returned_split[split_name] = [dspy.Example({field:row[field] for field in fields}).with_inputs(*input_keys) for row in dataset[split_name]]
+                    returned_split[split_name] = [
+                        dspy.Example({field: row[field] for field in fields}).with_inputs(*input_keys)
+                        for row in dataset[split_name]
+                    ]
                 else:
-                    returned_split[split_name] = [dspy.Example({field:row[field] for field in row.keys()}).with_inputs(*input_keys) for row in dataset[split_name]]
+                    returned_split[split_name] = [
+                        dspy.Example({field: row[field] for field in row.keys()}).with_inputs(*input_keys)
+                        for row in dataset[split_name]
+                    ]
 
             return returned_split
         except AttributeError:
             if fields:
-                return [dspy.Example({field:row[field] for field in fields}).with_inputs(*input_keys) for row in dataset]
+                return [
+                    dspy.Example({field: row[field] for field in fields}).with_inputs(*input_keys) for row in dataset
+                ]
             else:
-                return [dspy.Example({field:row[field] for field in row.keys()}).with_inputs(*input_keys) for row in dataset]
+                return [
+                    dspy.Example({field: row[field] for field in row.keys()}).with_inputs(*input_keys)
+                    for row in dataset
+                ]
 
-    def from_csv(self, file_path:str, fields: List[str] = None, input_keys: Tuple[str] = ()) -> List[dspy.Example]:
+    def from_csv(self, file_path: str, fields: List[str] = None, input_keys: Tuple[str] = ()) -> List[dspy.Example]:
         dataset = load_dataset("csv", data_files=file_path)["train"]
-        
+
         if not fields:
             fields = list(dataset.features)
-        
-        return [dspy.Example({field:row[field] for field in fields}).with_inputs(*input_keys) for row in dataset]
 
-    def from_json(self, file_path:str, fields: List[str] = None, input_keys: Tuple[str] = ()) -> List[dspy.Example]:
+        return [dspy.Example({field: row[field] for field in fields}).with_inputs(*input_keys) for row in dataset]
+
+    def from_json(self, file_path: str, fields: List[str] = None, input_keys: Tuple[str] = ()) -> List[dspy.Example]:
         dataset = load_dataset("json", data_files=file_path)["train"]
-        
+
         if not fields:
             fields = list(dataset.features)
-        
-        return [dspy.Example({field:row[field] for field in fields}).with_inputs(*input_keys) for row in dataset]
+
+        return [dspy.Example({field: row[field] for field in fields}).with_inputs(*input_keys) for row in dataset]
 
     def from_parquet(self, file_path: str, fields: List[str] = None, input_keys: Tuple[str] = ()) -> List[dspy.Example]:
         dataset = load_dataset("parquet", data_files=file_path)["train"]
 
         if not fields:
             fields = list(dataset.features)
 
@@ -75,15 +88,15 @@
         dataset: List[dspy.Example],
         n: int,
         *args,
         **kwargs,
     ) -> List[dspy.Example]:
         if not isinstance(dataset, list):
             raise ValueError(f"Invalid dataset provided of type {type(dataset)}. Please provide a list of examples.")
-        
+
         return random.sample(dataset, n, *args, **kwargs)
 
     def train_test_split(
         self,
         dataset: List[dspy.Example],
         train_size: Union[int, float] = 0.75,
         test_size: Union[int, float] = None,
@@ -111,10 +124,10 @@
                 raise ValueError("Invalid test_size. Please provide a float between 0 and 1 or an int.")
             if train_end + test_end > len(dataset_shuffled):
                 raise ValueError("train_size + test_size cannot exceed the total number of samples.")
         else:
             test_end = len(dataset_shuffled) - train_end
 
         train_dataset = dataset_shuffled[:train_end]
-        test_dataset = dataset_shuffled[train_end:train_end + test_end]
+        test_dataset = dataset_shuffled[train_end : train_end + test_end]
 
-        return {'train': train_dataset, 'test': test_dataset}
+        return {"train": train_dataset, "test": test_dataset}
```

### Comparing `dspy_ai-2.5.0rc1/dspy/datasets/dataset.py` & `dspy_ai-2.5.0rc2/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/datasets/gsm8k.py` & `dspy_ai-2.5.0rc2/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/datasets/hotpotqa.py` & `dspy_ai-2.5.0rc2/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/evaluate/auto_evaluation.py` & `dspy_ai-2.5.0rc2/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/evaluate/evaluate.py` & `dspy_ai-2.5.0rc2/dspy/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/evaluate/metrics.py` & `dspy_ai-2.5.0rc2/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/config.py` & `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/config.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/instruction_suffixes.py` & `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/instruction_suffixes.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/signatures.py` & `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/signatures.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/synthesizer.py` & `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/synthesizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 from datasets import Dataset
 from rich import print as rprint
 from tqdm import tqdm, trange
 
 import dspy
 
 from .config import SynthesizerArguments
-from .instruction_suffixes import (
-    INPUT_GENERATION_TASK_WITH_EXAMPLES_SUFFIX,
-    INPUT_GENERATION_TASK_WITH_FEEDBACK_SUFFIX,
-)
+from .instruction_suffixes import INPUT_GENERATION_TASK_WITH_EXAMPLES_SUFFIX, INPUT_GENERATION_TASK_WITH_FEEDBACK_SUFFIX
 from .signatures import (
     ExplainTask,
     GenerateFieldDescription,
     GenerateInputFieldsData,
     GenerateOutputFieldsData,
     GetFeedbackOnGeneration,
     UnderstandTask,
@@ -46,24 +43,23 @@
 
     def _gather_feedback(self, examples: dspy.Example) -> str:
         if self.config.feedback_mode == "human":
             input_keys = examples.inputs().keys()
 
             print("-"*75)
             print_text = "[bold blue]Generated Data:[bold blue]\n[bold red]Inputs:[bold red]\n"
-            
+
             for key in input_keys:
                 print_text += f"\t[bold yellow]{key}[bold yellow]: [green]{examples[key]}[green]\n"
-            
+
             rprint(print_text)
             feedback = input("Provide feedback on the generated data: ")
             print("-"*75)
 
             return feedback
-        
         elif self.config.feedback_mode == "llm":
             feedback = self.get_feedback_on_generation(
                 synthetic_data=[examples],
                 task_description=self.generate_output_data.__doc__,
             )
 
             return feedback.feedback
@@ -145,17 +141,17 @@
         return dspy.ChainOfThought(self.generate_input_data), dspy.Predict(self.generate_output_data)
 
     def _get_dataset_metadata(self, ground_source: Union[List[dspy.Example], dspy.Signature]):
         if isinstance(ground_source, dspy.SignatureMeta):
             task_description = ground_source.__doc__
             if task_description.startswith("Given the fields"):
                 task_description = self.understand_task(examples=ground_source.__doc__).explanation
-            
-            input_keys = {k:v.json_schema_extra["desc"] for k,v in ground_source.input_fields.items()}
-            output_keys = {k:v.json_schema_extra["desc"] for k,v in ground_source.output_fields.items()}
+
+            input_keys = {k: v.json_schema_extra["desc"] for k, v in ground_source.input_fields.items()}
+            output_keys = {k: v.json_schema_extra["desc"] for k, v in ground_source.output_fields.items()}
 
             return task_description, input_keys, output_keys
 
         elif isinstance(ground_source, list) and isinstance(ground_source[0], dspy.Example):
             task_description = self.explain_task(examples=ground_source).explanation
             input_keys = {key:f"${{{key}}}" for key in ground_source[0].inputs()}
             output_keys = {key:f"${{{key}}}" for key in ground_source[0].labels()}
@@ -172,15 +168,15 @@
         batch_size: int = 1,
     ):
         batch_size = batch_size or 1
         task_description, input_keys, output_keys = self._get_dataset_metadata(ground_source)
 
         if self.config.num_example_for_optim:
             self.generate_input_data.__doc__ += INPUT_GENERATION_TASK_WITH_EXAMPLES_SUFFIX
-        
+
         if self.config.feedback_mode:
             self.generate_input_data.__doc__ += INPUT_GENERATION_TASK_WITH_FEEDBACK_SUFFIX
 
         self.generate_output_data.__doc__ = task_description
 
         self.input_predictor, self.output_predictor = self._prepare_synthetic_data_predictors(
             input_keys=input_keys,
@@ -188,28 +184,28 @@
             ground_source=ground_source if self.config.num_example_for_optim else None,
         )
 
         data = []
         feedback = ""
 
         for idx in trange(0, num_data, batch_size, desc="Generating Synthetic Data"):
-            iter_temperature = 0.7+0.01*idx
+            iter_temperature = 0.7 + 0.01 * idx
             iter_seed = random.randint(0, 1000000)
 
             kwargs = {
                 "task_description": task_description,
                 "knowledge_seed": iter_seed,
                 "config": dict(temperature=iter_temperature, n=batch_size),
             }
 
             if self.config.num_example_for_optim:
                 if not isinstance(ground_source, list):
                     raise ValueError("Ground source must be a list of examples when `num_example_for_optim` is provided.")
                 kwargs["ground_source"] = random.sample(ground_source, k=self.config.num_example_for_optim)
-            
+
             with dspy.context(lm=self.input_lm):
                 inputs = self.input_predictor(**kwargs)
 
             input_kwargs = [{
                 key: getattr(completions, key)
                 for key in input_keys
             } for completions in inputs.completions]
@@ -220,24 +216,20 @@
                 with dspy.context(lm=self.output_lm, temperature=iter_temperature):
                     if self.config.output_teacher_module:
                         outputs = self.config.output_teacher_module(**kwargs)
 
                     else:
                         outputs = self.output_predictor(**kwargs, config=dict(temperature=iter_temperature))
 
-                output_kwargs = {
-                    key: getattr(outputs, key)
-                    for key in output_keys
-                }
+                output_kwargs = {key: getattr(outputs, key) for key in output_keys}
 
                 data.append(dspy.Example(**kwargs, **output_kwargs).with_inputs(*input_keys))
-            
+
             if self.config.feedback_mode and idx < self.config.num_example_for_feedback:
                 feedback = self._gather_feedback(data[-1])
-               
                 task_description = self.update_task_description(
                     task_description=task_description,
                     feedback=feedback,
                 ).updated_task_description
 
                 self.output_predictor.signature.__doc__ = task_description
```

### Comparing `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/utils.py` & `dspy_ai-2.5.0rc2/dspy/experimental/synthesizer/utils.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/experimental/synthetic_data.py` & `dspy_ai-2.5.0rc2/dspy/experimental/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/functional/functional.py` & `dspy_ai-2.5.0rc2/dspy/functional/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pydantic
 import ujson
 from pydantic.fields import FieldInfo
 
 import dspy
 from dsp.templates import passages2text
-from dspy.primitives.prediction import Prediction
+from dspy.primitives.prediction import Completions, Prediction
 from dspy.signatures.signature import ensure_signature, make_signature
 
 
 def predictor(*args, **kwargs):
     def _predictor(func) -> dspy.Module:
         """Decorator that creates a predictor module based on the provided function."""
         signature = _func_to_signature(func)
@@ -306,15 +306,14 @@
                     except (pydantic.ValidationError, ValueError) as e:
                         errors[name] = self._format_error(
                             e,
                             signature.fields[name],
                             value,
                             lm_explain=try_i + 1 < self.max_retries,
                         )
-
                         # If we can, we add an example to the error message
                         current_desc = field.json_schema_extra.get("desc", "")
                         i = current_desc.find("JSON Schema: ")
                         if i == -1:
                             continue  # Only add examples to JSON objects
                         suffix, current_desc = current_desc[i:], current_desc[:i]
                         prefix = "You MUST use this format: "
@@ -341,14 +340,15 @@
                         signature.instructions,
                         "\n\n".join(
                             "> " + field.json_schema_extra["prefix"] + " " + completion[name]
                             for name, field in signature.output_fields.items()
                         ),
                         lm_explain=try_i + 1 < self.max_retries,
                     )
+
             if errors:
                 # Add new fields for each error
                 for name, error in errors.items():
                     modified_kwargs[f"error_{name}_{try_i}"] = error
                     if name == "general":
                         error_prefix = "General:"
                     else:
@@ -359,17 +359,34 @@
                         dspy.InputField(
                             prefix=f"Past Error{number} in {error_prefix}",
                             desc="An error to avoid in the future",
                         ),
                     )
             else:
                 # If there are no errors, we return the parsed results
-                return Prediction.from_completions(
-                    {key: [r[key] for r in parsed_results] for key in signature.output_fields},
+                examples = []
+                for r in parsed_results:
+                    example = dspy.Example()
+                    for key in signature.output_fields:
+                        example[key] = r[key]
+
+                    examples.append(example)
+
+                # TODO: Completions objects, are now tracking input args to provide a robust history.
+                # when constructed outside the general generation sense, we will need a way to construct
+                # partial completions
+                completions = Completions(
+                    signature=signature,
+                    examples=examples,
+                    input_kwargs={},
                 )
+
+                pred = Prediction.from_completions(completions)
+                return pred
+
         raise ValueError(
             "Too many retries trying to get the correct output format. " + "Try simplifying the requirements.",
             errors,
         )
 
 
 def _func_to_signature(func):
```

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/chain_of_thought.py` & `dspy_ai-2.5.0rc2/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/chain_of_thought_with_hint.py` & `dspy_ai-2.5.0rc2/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/knn.py` & `dspy_ai-2.5.0rc2/dspy/predict/knn.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/langchain.py` & `dspy_ai-2.5.0rc2/dspy/predict/langchain.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/multi_chain_comparison.py` & `dspy_ai-2.5.0rc2/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/predict.py` & `dspy_ai-2.5.0rc2/dspy/predict/predict.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 import random
 
 from pydantic import BaseModel
 
 import dsp
+import dspy
 from dspy.predict.parameter import Parameter
-from dspy.primitives.prediction import Prediction
+from dspy.primitives.prediction import Completions, Prediction
 from dspy.signatures.signature import ensure_signature, signature_to_template
 
 
 class Predict(Parameter):
     def __init__(self, signature, **config):
         self.stage = random.randbytes(8).hex()
         self.signature = ensure_signature(signature)
         self.config = config
         self.reset()
 
     def reset(self):
-        self.lm = None
+        if dspy.settings.get("backend", None) is not None:
+            self.backend = None
+        else:
+            self.lm = None
+
         self.traces = []
         self.train = []
         self.demos = []
 
     def dump_state(self):
-        state_keys = ["lm", "traces", "train"]
+        if dspy.settings.get("backend", None) is not None:
+            state_keys = ["backend", "traces", "train", "demos"]
+        else:
+            state_keys = ["lm", "traces", "train"]
         state = {k: getattr(self, k) for k in state_keys}
 
         state["demos"] = []
         for demo in self.demos:
             demo = demo.copy()
 
             for field in demo:
@@ -58,79 +66,117 @@
             self.signature = self.signature.with_updated_fields(last_key, prefix=prefix)
 
     def __call__(self, **kwargs):
         return self.forward(**kwargs)
 
     def forward(self, **kwargs):
         # Extract the three privileged keyword arguments.
-        new_signature = ensure_signature(kwargs.pop("new_signature", None))
-        signature = ensure_signature(kwargs.pop("signature", self.signature))
+        signature = kwargs.pop("new_signature", kwargs.pop("signature", self.signature))
         demos = kwargs.pop("demos", self.demos)
         config = dict(**self.config, **kwargs.pop("config", {}))
 
-        # Get the right LM to use.
-        lm = kwargs.pop("lm", self.lm) or dsp.settings.lm
-        assert lm is not None, "No LM is loaded."
-
-        # If temperature is 0.0 but its n > 1, set temperature to 0.7.
-        temperature = config.get("temperature")
-        temperature = lm.kwargs["temperature"] if temperature is None else temperature
-
-        num_generations = config.get("n")
-        if num_generations is None:
-            num_generations = lm.kwargs.get("n", lm.kwargs.get("num_generations", 1))
-
-        if (temperature is None or temperature <= 0.15) and num_generations > 1:
-            config["temperature"] = 0.7
-            # print(f"#> Setting temperature to 0.7 since n={num_generations} and prior temperature={temperature}.")
-
-        # All of the other kwargs are presumed to fit a prefix of the signature.
-        # That is, they are input variables for the bottom most generation, so
-        # we place them inside the input - x - together with the demos.
-        x = dsp.Example(demos=demos, **kwargs)
-
-        if new_signature is not None:
-            signature = new_signature
-
-        if not all(k in kwargs for k in signature.input_fields):
-            present = [k for k in signature.input_fields if k in kwargs]
-            missing = [k for k in signature.input_fields if k not in kwargs]
-            print(f"WARNING: Not all input fields were provided to module. Present: {present}. Missing: {missing}.")
+        # Check if we should use backend
+        backend = dspy.settings.get("backend", None)
 
-        # Switch to legacy format for dsp.generate
-        template = signature_to_template(signature)
+        if backend is not None:
+            if not all(k in kwargs for k in signature.input_fields):
+                present = [k for k in signature.input_fields if k in kwargs]
+                missing = [k for k in signature.input_fields if k not in kwargs]
+                dspy.logger.warning(
+                    f"WARNING: Not all input fields were provided to module. Present: {present}. Missing: {missing}.",
+                )
+
+            completions = backend(signature, demos=demos, config=config, **kwargs)
+
+            pred = Prediction.from_completions(completions)
+
+            trace = dspy.settings.get("trace")
+            if trace is not None and kwargs.pop("_trace", True):
+                trace.append((self, {**kwargs}, pred))
+
+            return pred
 
-        if self.lm is None:
-            x, C = dsp.generate(template, **config)(x, stage=self.stage)
         else:
-            # Note: query_only=True means the instructions and examples are not included.
-            # I'm not really sure why we'd want to do that, but it's there.
-            with dsp.settings.context(lm=self.lm, query_only=True):
+            lm = kwargs.pop("lm", self.lm) or dspy.settings.get("lm", None)
+            assert lm is not None, "No LM is loaded."
+
+            # If temperature is 0.0 but its n > 1, set temperature to 0.7
+            temperature = config.get("temperature")
+            temperature = lm.kwargs["temperature"] if temperature is None else temperature
+
+            num_generations = config.get("n")
+            if num_generations is None:
+                num_generations = lm.kwargs.get(
+                    "n",
+                    lm.kwargs.get("num_generations", None),
+                )
+
+            if (temperature is None or temperature <= 0.15) and num_generations > 1:
+                config["temperature"] = 0.7
+
+            # All of the other kwargs are presumed to fit a prefix of the signature.
+            # That is, they are input variables for the bottom most generation, so
+            # we place them inside the input - x - together with the demos.
+            x = dsp.Example(demos=demos, **kwargs)
+
+            if not all(k in kwargs for k in signature.input_fields):
+                present = [k for k in signature.input_fields if k in kwargs]
+                missing = [k for k in signature.input_fields if k not in kwargs]
+                dspy.logger.warning(
+                    f"WARNING: Not all input fields were provided to module. Present: {present}. Missing: {missing}.",
+                )
+
+            # Switch to legacy format for dsp.generate
+            template = signature_to_template(signature)
+
+            if self.lm is None:
                 x, C = dsp.generate(template, **config)(x, stage=self.stage)
+            else:
+                # Note: query_only=True means the instructions and examples are not included.
+                # I'm not really sure why we'd want to do that, but it's there.
+                with dsp.settings.context(lm=self.lm, query_only=True):
+                    x, C = dsp.generate(template, **config)(x, stage=self.stage)
 
-        assert self.stage in x, "The generated (input, output) example was not stored"
+            assert self.stage in x, "The generated (input, output) example was not stored"
 
         completions = []
 
         for c in C:
             completions.append({})
             for field in template.fields:
                 if field.output_variable not in kwargs.keys():
                     completions[-1][field.output_variable] = getattr(
                         c,
                         field.output_variable,
                     )
+            examples = []
+            for c in C:
+                example = dspy.Example()
+                for name in self.signature.input_fields:
+                    if name in kwargs.keys():
+                        example[name] = kwargs[name]
+
+                for name in self.signature.output_fields:
+                    example[name] = getattr(c, name)
+
+                examples.append(example)
+
+            completions = Completions(
+                signature=self.signature,
+                examples=examples,
+                input_kwargs=config,
+            )
+
+            pred = Prediction.from_completions(completions)
+
+            if kwargs.pop("_trace", True) and dsp.settings.trace is not None:
+                trace = dsp.settings.trace
+                trace.append((self, {**kwargs}, pred))
 
-        pred = Prediction.from_completions(completions, signature=signature)
-
-        if kwargs.pop("_trace", True) and dsp.settings.trace is not None:
-            trace = dsp.settings.trace
-            trace.append((self, {**kwargs}, pred))
-
-        return pred
+            return pred
 
     def update_config(self, **kwargs):
         self.config = {**self.config, **kwargs}
 
     def get_config(self):
         return self.config
```

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/program_of_thought.py` & `dspy_ai-2.5.0rc2/dspy/predict/program_of_thought.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,15 @@
             },
         }
         signature_dict.update(fields_for_mode[mode])
         return dspy.Signature(signature_dict)
 
     def _generate_instruction(self, mode):
         mode_inputs = ", ".join(
-            [
-                f"`{field_name}`"
-                for field_name in self._generate_signature(mode).input_fields
-            ],
+            [f"`{field_name}`" for field_name in self._generate_signature(mode).input_fields],
         )
         mode_outputs = f"`{self.output_field_name}`"
         if mode == "generate":
             instr = [
                 f"You will be given {mode_inputs} and you will respond with {mode_outputs}.",
                 f"Generating executable Python code that programmatically computes the correct {mode_outputs}.",
                 f"After you're done with the computation, make sure the last line in your code evaluates to the correct value for {mode_outputs}.",
@@ -123,33 +120,35 @@
                 f"Given the final code {mode_inputs}, provide the final {mode_outputs}.",
             ]
 
         return "\n".join(instr)
 
 
     def parse_code(self, code_data):
-        code = (
-            code_data.get("generated_code", "").split("---", 1)[0].split("\n\n\n", 1)[0]
-        )
+        code = code_data.get("generated_code", "").split("---", 1)[0].split("\n\n\n", 1)[0]
         code_match = re.search(r"```python[ \n](.*?)[ \n]```?", code, re.DOTALL)
         code_block = (code_match.group(1) if code_match else code).replace("\\n", "\n")
         if not code_block:
             return code, "Error: Empty code after parsing."
         if "\n" not in code_block and code_block.count("=") > 1:
             return code, "Error: Code format is not correct."
         lines = code_block.split("\n")
         last_line_match = re.match(r"^(\w+)\s*=", lines[-1].strip())
         if last_line_match and len(lines) > 1:
             code_block += "\n" + last_line_match.group(1)
         else:
             code_block = re.sub(
-                r"([a-zA-Z_]\w* *=.*?)(?=[a-zA-Z_]\w* *=)", r"\1\n", code_block,
+                r"([a-zA-Z_]\w* *=.*?)(?=[a-zA-Z_]\w* *=)",
+                r"\1\n",
+                code_block,
             )
             code_block = re.sub(
-                r"([a-zA-Z_]\w* *=.*?)([a-zA-Z_]\w*)$", r"\1\n\2", code_block,
+                r"([a-zA-Z_]\w* *=.*?)([a-zA-Z_]\w*)$",
+                r"\1\n\2",
+                code_block,
             )
         return code_block, None
 
     def execute_code(self, code):
         if not code:
             return code, None, "Error: Empty code before execution."
         code_prompt = CodePrompt(code, code_type="python")
@@ -178,8 +177,8 @@
             code, output, error = self.execute_code(parsed_code)
             hop += 1
             if hop == self.max_iters:
                 print("Max hops reached. Error persists.")
                 return None
         input_kwargs.update({"final_generated_code": code, "code_output": output})
         answer_gen_result = self.generate_answer(**input_kwargs)
-        return answer_gen_result
+        return answer_gen_result
```

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/react.py` & `dspy_ai-2.5.0rc2/dspy/predict/react.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/predict/retry.py` & `dspy_ai-2.5.0rc2/dspy/predict/retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,41 @@
 from .predict import Predict
 
 
 class Retry(Predict):
     def __init__(self, module):
         super().__init__(module.signature)
         self.module = module
-        self.original_signature = module.extended_signature if isinstance(module, dspy.ChainOfThought) else module.signature
+        self.original_signature = (
+            module.extended_signature if isinstance(module, dspy.ChainOfThought) else module.signature
+        )
         self.original_forward = module.forward
         self.new_signature = self._create_new_signature(self.original_signature)
 
     def _create_new_signature(self, signature):
         # Add "Past" input fields for each output field
         for key, value in signature.output_fields.items():
             actual_prefix = value.json_schema_extra["prefix"].split(":")[0] + ":"
-            signature = signature.append(f"past_{key}", dspy.InputField(
-                prefix="Previous " + actual_prefix,
-                desc=f"past {actual_prefix} with errors",
-                format=value.json_schema_extra.get("format"),
-            ))
-
-        signature = signature.append("feedback", dspy.InputField(
-            prefix="Instructions:",
-            desc="Some instructions you must satisfy",
-            format=str,
-        ))
+            signature = signature.append(
+                f"past_{key}",
+                dspy.InputField(
+                    prefix="Previous " + actual_prefix,
+                    desc=f"past {actual_prefix} with errors",
+                    format=value.json_schema_extra.get("format"),
+                ),
+            )
+
+        signature = signature.append(
+            "feedback",
+            dspy.InputField(
+                prefix="Instructions:",
+                desc="Some instructions you must satisfy",
+                format=str,
+            ),
+        )
 
         return signature
 
     def forward(self, *, past_outputs, **kwargs):
         # Take into account the possible new signature, as in TypedPredictor
         new_signature = kwargs.pop("new_signature", None)
         if new_signature:
```

### Comparing `dspy_ai-2.5.0rc1/dspy/primitives/assertions.py` & `dspy_ai-2.5.0rc2/dspy/primitives/assertions.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/primitives/box.py` & `dspy_ai-2.5.0rc2/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/primitives/example.py` & `dspy_ai-2.5.0rc2/dspy/primitives/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-
 class Example:
+
     def __init__(self, base=None, **kwargs):
         # Internal storage and other attributes
         self._store = {}
         self._demos = []
         self._input_keys = None
 
         # Initialize from a base Example if provided
@@ -12,95 +12,94 @@
 
         # Initialize from a dict if provided
         elif base and isinstance(base, dict):
             self._store = base.copy()
 
         # Update with provided kwargs
         self._store.update(kwargs)
-    
+
     def __getattr__(self, key):
-        if key.startswith('__') and key.endswith('__'):
+        if key.startswith("__") and key.endswith("__"):
             raise AttributeError
         if key in self._store:
             return self._store[key]
         raise AttributeError(f"'{type(self).__name__}' object has no attribute '{key}'")
 
     def __setattr__(self, key, value):
-        if key.startswith('_') or key in dir(self.__class__):  
+        if key.startswith("_") or key in dir(self.__class__):
             super().__setattr__(key, value)
         else:
             self._store[key] = value
-    
+
     def __getitem__(self, key):
         return self._store[key]
 
     def __setitem__(self, key, value):
         self._store[key] = value
 
     def __delitem__(self, key):
         del self._store[key]
 
     def __contains__(self, key):
         return key in self._store
-    
+
     def __len__(self):
-        return len([k for k in self._store if not k.startswith('dspy_')])
-    
+        return len([k for k in self._store if not k.startswith("dspy_")])
+
     def __repr__(self):
         # return f"Example({self._store})" + f" (input_keys={self._input_keys}, demos={self._demos})"
-        d = {k: v for k, v in self._store.items() if not k.startswith('dspy_')}
+        d = {k: v for k, v in self._store.items() if not k.startswith("dspy_")}
         return f"Example({d})" + f" (input_keys={self._input_keys})"
-    
+
     def __str__(self):
         return self.__repr__()
-    
+
     def __eq__(self, other):
         return isinstance(other, Example) and self._store == other._store
-    
     def __hash__(self):
         return hash(tuple(self._store.items()))
 
     def keys(self, include_dspy=False):
-        return [k for k in self._store.keys() if not k.startswith('dspy_') or include_dspy]
-    
+        return [k for k in self._store.keys() if not k.startswith("dspy_") or include_dspy]
+
     def values(self, include_dspy=False):
-        return [v for k, v in self._store.items() if not k.startswith('dspy_') or include_dspy]
+        return [v for k, v in self._store.items() if not k.startswith("dspy_") or include_dspy]
 
     def items(self, include_dspy=False):
-        return [(k, v) for k, v in self._store.items() if not k.startswith('dspy_') or include_dspy]
+        return [(k, v) for k, v in self._store.items() if not k.startswith("dspy_") or include_dspy]
 
     def get(self, key, default=None):
         return self._store.get(key, default)
-    
+
     def with_inputs(self, *keys):
         copied = self.copy()
         copied._input_keys = set(keys)
         return copied
-    
+
     def inputs(self):
         if self._input_keys is None:
             raise ValueError("Inputs have not been set for this example. Use `example.with_inputs()` to set them.")
 
         # return items that are in input_keys
         d = {key: self._store[key] for key in self._store if key in self._input_keys}
         return type(self)(d)
-    
+
     def labels(self):
         # return items that are NOT in input_keys
         input_keys = self.inputs().keys()
         d = {key: self._store[key] for key in self._store if key not in input_keys}
         return type(self)(d)
-    
+
     def __iter__(self):
         return iter(dict(self._store))
 
     def copy(self, **kwargs):
         return type(self)(base=self, **kwargs)
 
     def without(self, *keys):
         copied = self.copy()
         for key in keys:
             del copied[key]
         return copied
-    
+
     def toDict(self):
         return self._store.copy()
```

### Comparing `dspy_ai-2.5.0rc1/dspy/primitives/module.py` & `dspy_ai-2.5.0rc2/dspy/primitives/module.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/primitives/program.py` & `dspy_ai-2.5.0rc2/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/primitives/python_interpreter.py` & `dspy_ai-2.5.0rc2/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/azureaisearch_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/azureaisearch_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/chromadb_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/chromadb_rm.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 import openai
 
 import dspy
 from dsp.utils import dotdict
 
 try:
     import openai.error
+
     ERRORS = (openai.error.RateLimitError, openai.error.ServiceUnavailableError, openai.error.APIError)
 except Exception:
     ERRORS = (openai.RateLimitError, openai.APIError)
 
 try:
     import chromadb
     import chromadb.utils.embedding_functions as ef
-    from chromadb.api.types import (
-        Embeddable,
-        EmbeddingFunction,
-    )
+    from chromadb.api.types import Embeddable, EmbeddingFunction
     from chromadb.config import Settings
     from chromadb.utils import embedding_functions
 except ImportError:
     raise ImportError(
         "The chromadb library is required to use ChromadbRM. Install it with `pip install dspy-ai[chromadb]`",
     )
 
@@ -49,45 +47,44 @@
         dspy.Prediction: An object containing the retrieved passages.
 
     Examples:
         Below is a code snippet that shows how to use this as the default retriever:
         ```python
         llm = dspy.OpenAI(model="gpt-3.5-turbo")
         # using default chromadb client
-        retriever_model = ChromadbRM('collection_name', 'db_path')
+        retriever_model = ChromadbRM("collection_name", "db_path")
         dspy.settings.configure(lm=llm, rm=retriever_model)
         # to test the retriever with "my query"
         retriever_model("my query")
         ```
 
         Use provided chromadb client
         ```python
         import chromadb
+
         llm = dspy.OpenAI(model="gpt-3.5-turbo")
         # say you have a chromadb running on a different port
-        client = chromadb.HttpClient(host='localhost', port=8889)
-        retriever_model = ChromadbRM('collection_name', 'db_path', client=client)
+        client = chromadb.HttpClient(host="localhost", port=8889)
+        retriever_model = ChromadbRM("collection_name", "db_path", client=client)
         dspy.settings.configure(lm=llm, rm=retriever_model)
         # to test the retriever with "my query"
         retriever_model("my query")
         ```
 
         Below is a code snippet that shows how to use this in the forward() function of a module
         ```python
-        self.retrieve = ChromadbRM('collection_name', 'db_path', k=num_passages)
+        self.retrieve = ChromadbRM("collection_name", "db_path", k=num_passages)
         ```
     """
 
     def __init__(
         self,
         collection_name: str,
         persist_directory: str,
-        embedding_function: Optional[
-            EmbeddingFunction[Embeddable]
-        ] = ef.DefaultEmbeddingFunction(),
+        embedding_function: Optional[EmbeddingFunction[Embeddable]] = ef.DefaultEmbeddingFunction(),
         client: Optional[chromadb.Client] = None,
         k: int = 7,
     ):
         self._init_chromadb(collection_name, persist_directory, client=client)
         self.ef = embedding_function
 
         super().__init__(k=k)
@@ -112,15 +109,15 @@
             self._chromadb_client = client
         else:
             self._chromadb_client = chromadb.Client(
                 Settings(
                     persist_directory=persist_directory,
                     is_persistent=True,
                 ),
-        )
+            )
         self._chromadb_collection = self._chromadb_client.get_or_create_collection(
             name=collection_name,
         )
 
     @backoff.on_exception(
         backoff.expo,
         ERRORS,
@@ -134,37 +131,39 @@
 
         Returns:
             List[List[float]]: List of embeddings corresponding to each query.
         """
         return self.ef(queries)
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None, **kwargs,
+        self,
+        query_or_queries: Union[str, List[str]],
+        k: Optional[int] = None,
+        **kwargs,
     ) -> dspy.Prediction:
         """Search with db for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
 
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
         """
-        queries = (
-            [query_or_queries]
-            if isinstance(query_or_queries, str)
-            else query_or_queries
-        )
+        queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
         queries = [q for q in queries if q]  # Filter empty queries
         embeddings = self._get_embeddings(queries)
 
         k = self.k if k is None else k
         results = self._chromadb_collection.query(
-            query_embeddings=embeddings, n_results=k,**kwargs,
+            query_embeddings=embeddings,
+            n_results=k,
+            **kwargs,
         )
 
         zipped_results = zip(
-            results["ids"][0], 
-            results["distances"][0], 
-            results["documents"][0], 
-            results["metadatas"][0])
-        results = [dotdict({"id": id, "score": dist, "long_text": doc, "metadatas": meta }) for id, dist, doc, meta in zipped_results]
+            results["ids"][0], results["distances"][0], results["documents"][0], results["metadatas"][0],
+        )
+        results = [
+            dotdict({"id": id, "score": dist, "long_text": doc, "metadatas": meta})
+            for id, dist, doc, meta in zipped_results
+        ]
         return results
```

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/clarifai_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/clarifai_rm.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,20 +36,21 @@
         clarifai_user_id: str,
         clarfiai_app_id: str,
         clarifai_pat: Optional[str] = None,
         k: int = 3,
     ):
         self.app_id = clarfiai_app_id
         self.user_id = clarifai_user_id
-        self.pat = (
-            clarifai_pat if clarifai_pat is not None else os.environ["CLARIFAI_PAT"]
-        )
+        self.pat = clarifai_pat if clarifai_pat is not None else os.environ["CLARIFAI_PAT"]
         self.k = k
         self.clarifai_search = Search(
-            user_id=self.user_id, app_id=self.app_id, top_k=k, pat=self.pat,
+            user_id=self.user_id,
+            app_id=self.app_id,
+            top_k=k,
+            pat=self.pat,
         )
         super().__init__(k=k)
 
     def retrieve_hits(self, hits):
         header = {"Authorization": f"Key {self.pat}"}
         request = requests.get(hits.input.data.text.url, headers=header)
         request.encoding = request.apparent_encoding
@@ -67,24 +68,23 @@
         Returns:
              passages in format of dotdict
 
         Examples:
         Below is a code snippet that shows how to use Marqo as the default retriver:
          ```python
          import clarifai
+
          llm = dspy.Clarifai(model=MODEL_URL, api_key="YOUR CLARIFAI_PAT")
-         retriever_model = ClarifaiRM(clarifai_user_id="USER_ID", clarfiai_app_id="APP_ID", clarifai_pat="YOUR CLARIFAI_PAT")
+         retriever_model = ClarifaiRM(
+             clarifai_user_id="USER_ID", clarfiai_app_id="APP_ID", clarifai_pat="YOUR CLARIFAI_PAT"
+         )
          dspy.settings.configure(lm=llm, rm=retriever_model)
          ```
         """
-        queries = (
-            [query_or_queries]
-            if isinstance(query_or_queries, str)
-            else query_or_queries
-        )
+        queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
         passages = []
         queries = [q for q in queries if q]
 
         for query in queries:
             search_response = self.clarifai_search.query(ranks=[{"text_raw": query}],**kwargs)
 
             # Retrieve hits
```

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/databricks_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/databricks_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/deeplake_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/deeplake_rm.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         openai.error.APIError,
     )
 except Exception:
     ERRORS = (openai.error.RateLimitError, openai.error.APIError)
 
 
 class DeeplakeRM(dspy.Retrieve):
-    
+
     """
     A retriever module that uses deeplake to return the top passages for a given query.
 
     Assumes that a Deep Lake Vector Store has been created and populated with the following payload:
         - text: The text of the passage
 
     Args:
@@ -35,14 +35,15 @@
         deeplake_client (VectorStore): An instance of the Deep Lake client.
         k (int, optional): The default number of top passages to retrieve. Defaults to 3.
 
     Examples:
         Below is a code snippet that shows how to use Deep Lake as the default retriver:
         ```python
         from deeplake import VectorStore
+
         llm = dspy.OpenAI(model="gpt-3.5-turbo")
         deeplake_client = VectorStore
         retriever_model = DeeplakeRM("my_vectorstore_path", deeplake_client=deeplake_client)
         dspy.settings.configure(lm=llm, rm=retriever_model)
         ```
 
         Below is a code snippet that shows how to use Deep Lake in the forward() function of a module
@@ -54,64 +55,55 @@
     def __init__(
         self,
         deeplake_vectorstore_name: str,
         deeplake_client,
         k: int = 3,
     ):
         try:
-          from deeplake import VectorStore
+            from deeplake import VectorStore
         except ImportError:
-          raise ImportError(
-              "The 'deeplake' extra is required to use DeepLakeRM. Install it with `pip install dspy-ai[deeplake]`",
-          )
+            raise ImportError(
+                "The 'deeplake' extra is required to use DeepLakeRM. Install it with `pip install dspy-ai[deeplake]`",
+            )
         self._deeplake_vectorstore_name = deeplake_vectorstore_name
         self._deeplake_client = deeplake_client
 
         super().__init__(k=k)
 
     def embedding_function(self, texts, model="text-embedding-ada-002"):
         if isinstance(texts, str):
             texts = [texts]
 
         texts = [t.replace("\n", " ") for t in texts]
-        return [
-            data["embedding"]
-            for data in openai.Embedding.create(input=texts, model=model)["data"]
-        ]
+        return [data["embedding"] for data in openai.Embedding.create(input=texts, model=model)["data"]]
 
     def forward(
         self, query_or_queries: Union[str, List[str]], k: Optional[int],**kwargs,
     ) -> dspy.Prediction:
-        
         """Search with DeepLake for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
 
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
         """
-        queries = (
-            [query_or_queries]
-            if isinstance(query_or_queries, str)
-            else query_or_queries
-        )
+        queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
         queries = [q for q in queries if q]  # Filter empty queries
 
         k = k if k is not None else self.k
 
         passages = defaultdict(float)
-        #deeplake doesn't support batch querying, manually querying each query and storing them
+        # deeplake doesn't support batch querying, manually querying each query and storing them
         for query in queries:
             results = self._deeplake_client(
-            path=self._deeplake_vectorstore_name,
-            embedding_function=self.embedding_function,
+                path=self._deeplake_vectorstore_name,
+                embedding_function=self.embedding_function,
             ).search(query, k=k,**kwargs)
 
-            for score,text in zip(results.get('score',0.0),results.get('text',"")):
+            for score, text in zip(results.get("score", 0.0), results.get("text", "")):
                 passages[text] += score
 
-        sorted_passages = sorted(
-            passages.items(), key=lambda x: x[1], reverse=True)[:k]
-        
-        return [dotdict({"long_text": p}) for p, _ in sorted_passages]
+        sorted_passages = sorted(passages.items(), key=lambda x: x[1], reverse=True)[:k]
+
+        return [dotdict({"long_text": p}) for p, _ in sorted_passages]
```

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/faiss_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/faiss_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/llama_index_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/llama_index_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/marqo_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/marqo_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/milvus_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/milvus_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/mongodb_atlas_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/neo4j_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/neo4j_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/pgvector_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/pgvector_rm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import warnings
 from typing import Callable, Optional
 
+import openai
+
 import dspy
 
 try:
     import psycopg2
     from pgvector.psycopg2 import register_vector
     from psycopg2 import sql
 except ImportError:
@@ -58,14 +60,15 @@
         ```
 
         Below is a code snippet that shows how to use PgVector in the forward() function of a module
         ```python
         self.retrieve = PgVectorRM(db_url, openai_client=openai_client, "paragraphs", fields=["text", "document_id"], k=20)
         ```
     """
+
     def __init__(
             self,
             db_url: str,
             pg_table_name: str,
             openai_client: Optional[openai.OpenAI] = None,
             embedding_func: Optional[Callable] = None,
             k: int = 20,
@@ -89,15 +92,14 @@
         self.embedding_model = embedding_model
         self.include_similarity = include_similarity
 
         super().__init__(k=k)
 
     def forward(self, query: str):
         """Search with PgVector for self.k top passages for query using cosine similarity
-
         Args:
             query  (str): The query to search for
             include_similarity (bool): Whether or not to include the similarity for each record
         Returns:
             dspy.Prediction: an object containing the retrieved passages.
         """
         # Embed query
@@ -127,17 +129,15 @@
             fields=fields,
             table=sql.Identifier(self.pg_table_name),
             embedding_field=sql.Identifier(self.embedding_field),
         )
 
         with self.conn as conn:
             with conn.cursor() as cur:
-                cur.execute(
-                    sql_query,
-                    args)
+                cur.execute(sql_query, args)
                 rows = cur.fetchall()
                 columns = [descrip[0] for descrip in cur.description]
                 for row in rows:
                     data = dict(zip(columns, row))
                     retrieved_docs.append(dspy.Example(**data))
         # Return Prediction
         return retrieved_docs
```

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/pinecone_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/qdrant_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/qdrant_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/ragatouille_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/ragatouille_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/retrieve.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/retrieve.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,17 @@
             setattr(self, name, value)
 
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
 
     def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,**kwargs) -> Prediction:
         queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
-        queries = [query.strip().split('\n')[0].strip() for query in queries]
+        queries = [query.strip().split("\n")[0].strip() for query in queries]
 
         # print(queries)
         # TODO: Consider removing any quote-like markers that surround the query too.
         k = k if k is not None else self.k
         passages = dsp.retrieveEnsemble(queries, k=k,**kwargs)
         return Prediction(passages=passages)
 
+
 # TODO: Consider doing Prediction.from_completions with the individual sets of passages (per query) too.
```

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/snowflake_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/snowflake_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/vectara_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/vectara_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/weaviate_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/weaviate_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,32 +31,35 @@
     Examples:
         Below is a code snippet that shows how to use Weaviate as the default retriver:
         ```python
         import weaviate
 
         llm = dspy.OpenAI(model="gpt-3.5-turbo")
         weaviate_client = weaviate.Client("your-path-here")
-        retriever_model = WeaviateRM(weaviate_collection_name="my_collection_name",
-                                     weaviate_collection_text_key="content", 
-                                     weaviate_client=weaviate_client)
+        retriever_model = WeaviateRM(
+            weaviate_collection_name="my_collection_name",
+            weaviate_collection_text_key="content",
+            weaviate_client=weaviate_client,
+        )
         dspy.settings.configure(lm=llm, rm=retriever_model)
         ```
 
         Below is a code snippet that shows how to use Weaviate in the forward() function of a module
         ```python
         self.retrieve = WeaviateRM("my_collection_name", weaviate_client=weaviate_client, k=num_passages)
         ```
     """
 
-    def __init__(self, 
-                 weaviate_collection_name: str, 
-                 weaviate_client: weaviate.WeaviateClient,
-                 k: int = 3,
-                 weaviate_collection_text_key: Optional[str] = "content",
-                 weaviate_alpha: Optional[float] = 0.5,
+    def __init__(
+        self,
+        weaviate_collection_name: str,
+        weaviate_client: weaviate.WeaviateClient,
+        k: int = 3,
+        weaviate_collection_text_key: Optional[str] = "content",
+    weaviate_alpha: Optional[float] = 0.5,
                  weaviate_fusion_type: Optional[HybridFusion] = HybridFusion.RELATIVE_SCORE,
         ):
         self._weaviate_collection_name = weaviate_collection_name
         self._weaviate_client = weaviate_client
         self._weaviate_collection_text_key = weaviate_collection_text_key
         self._weaviate_alpha = weaviate_alpha
         self._weaviate_fusion_type = weaviate_fusion_type
@@ -69,19 +72,15 @@
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
         """
 
         k = k if k is not None else self.k
-        queries = (
-            [query_or_queries]
-            if isinstance(query_or_queries, str)
-            else query_or_queries
-        )
+        queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
         queries = [q for q in queries if q]
         passages = []
         for query in queries:
             collection = self._weaviate_client.collections.get(self._weaviate_collection_name)
             results = collection.query.hybrid(query=query,
                                               limit=k,
                                               alpha=self._weaviate_alpha,
```

### Comparing `dspy_ai-2.5.0rc1/dspy/retrieve/you_rm.py` & `dspy_ai-2.5.0rc2/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/signatures/field.py` & `dspy_ai-2.5.0rc2/dspy/signatures/field.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/signatures/signature.py` & `dspy_ai-2.5.0rc2/dspy/signatures/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,14 +294,23 @@
 def _parse_arg_string(string: str, names=None) -> Dict[str, str]:
     args = ast.parse("def f(" + string + "): pass").body[0].args.args
     names = [arg.arg for arg in args]
     types = [str if arg.annotation is None else _parse_type_node(arg.annotation) for arg in args]
     return zip(names, types)
 
 
+def _parse_named_type_node(node, names=None) -> Any:
+    parts = node.split(":")
+    if len(parts) == 1:
+        return parts[0], str
+    name, type_str = parts
+    type_ = _parse_type_node(ast.parse(type_str), names)
+    return name, type_
+
+
 def _parse_type_node(node, names=None) -> Any:
     """Recursively parse an AST node representing a type annotation.
 
     without using structural pattern matching introduced in Python 3.10.
     """
     if names is None:
         names = typing.__dict__
```

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/bootstrap.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/bootstrap.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,33 +28,34 @@
 
 # TODO: When this bootstraps for another teleprompter like finetune, we want all demos we gather.
 # But when it's for direct use we may want to sample ONE demo per predictor--example pair.
 # This is important for "multi-use" modules.
 
 # TODO: Add baselines=[...]
 
+
 class BootstrapFewShot(Teleprompter):
     def __init__(
         self,
         metric=None,
         metric_threshold=None,
-        teacher_settings: Optional[Dict]=None,
+        teacher_settings: Optional[Dict] = None,
         max_bootstrapped_demos=4,
         max_labeled_demos=16,
         max_rounds=1,
         max_errors=5,
     ):
         """
         A Teleprompter class that composes a set of demos/examples to go into a predictor's prompt.
         These demos come from a combination of labeled examples in the training set, and bootstrapped demos.
 
         Parameters
         ----------
         metric: Callable
-            A function that compares an expected value and predicted value, outputting the result of that comparison. 
+            A function that compares an expected value and predicted value, outputting the result of that comparison.
         metric_threshold: optional float, default `None`
             If the metric yields a numerical value, then check it against this threshold when
             deciding whether or not to accept a bootstrap example.
         teacher_settings: dict, optional
             Settings for the `teacher` model.
         max_bootstrapped_demos: int, default 4
             Maximum number of bootstrapped demonstrations to include
@@ -96,31 +97,38 @@
         self.student = student.reset_copy()
         self.teacher = teacher.deepcopy() if teacher is not None else student.reset_copy()
 
         assert getattr(self.student, "_compiled", False) is False, "Student must be uncompiled."
 
         if self.max_labeled_demos and getattr(self.teacher, "_compiled", False) is False:
             teleprompter = LabeledFewShot(k=self.max_labeled_demos)
-            self.teacher = teleprompter.compile(self.teacher.reset_copy(), trainset=self.trainset)
+            self.teacher = teleprompter.compile(
+                self.teacher.reset_copy(),
+                trainset=self.trainset,
+            )
 
     def _prepare_predictor_mappings(self):
         name2predictor, predictor2name = {}, {}
         student, teacher = self.student, self.teacher
 
         assert len(student.predictors()) == len(
             teacher.predictors(),
         ), "Student and teacher must have the same number of predictors."
 
-        for (name1, predictor1), (name2, predictor2) in zip(student.named_predictors(), teacher.named_predictors()):
+        for (name1, predictor1), (name2, predictor2) in zip(
+            student.named_predictors(),
+            teacher.named_predictors(),
+        ):
             assert name1 == name2, "Student and teacher must have the same program structure."
             assert predictor1.signature.equals(
                 predictor2.signature,
-            ), (f"Student and teacher must have the same signatures. "
+            ), (
+                f"Student and teacher must have the same signatures. "
                 f"{type(predictor1.signature)} != {type(predictor2.signature)}"
-                )
+            )
             assert id(predictor1) != id(predictor2), "Student and teacher must be different objects."
 
             name2predictor[name1] = None  # dict(student=predictor1, teacher=predictor2)
             predictor2name[id(predictor1)] = name1
 
             # FIXME(shangyint): This is an ugly hack to bind traces of
             # retry.module to retry
@@ -204,18 +212,26 @@
             dspy.logger.error(f"Failed to run or to evaluate example {example} with {self.metric} due to {e}.")
 
         if success:
             for step in trace:
                 predictor, inputs, outputs = step
 
                 if "dspy_uuid" in example:
-                    demo = Example(augmented=True, dspy_uuid=example.dspy_uuid, **inputs, **outputs)
+                    demo = Example(
+                        augmented=True,
+                        dspy_uuid=example.dspy_uuid,
+                        **inputs,
+                        **outputs,
+                    )
                 else:
                     # TODO: FIXME: This is a hack. RandomSearch will complain for now in this edge case.
-                    demo = Example(augmented=True, **inputs, **outputs)
+                    # The predictor, now adds the input into the output Prediction directly
+                    # therefore we have to dedupe this before creating the example
+                    inputs.update(**outputs)
+                    demo = Example(augmented=True, **inputs)
 
                 try:
                     predictor_name = self.predictor2name[id(predictor)]
                 except KeyError:
                     continue  # FIXME: !
 
                     # # TODO: Look closer into this. It's a bit tricky to reproduce.
@@ -235,15 +251,18 @@
     def _train(self):
         rng = random.Random(0)
         raw_demos = self.validation
 
         for name, predictor in self.student.named_predictors():
             augmented_demos = self.name2traces[name][: self.max_bootstrapped_demos]
 
-            sample_size = min(self.max_labeled_demos - len(augmented_demos), len(raw_demos))
+            sample_size = min(
+                self.max_labeled_demos - len(augmented_demos),
+                len(raw_demos),
+            )
             sample_size = max(0, sample_size)
 
             raw_demos = rng.sample(raw_demos, sample_size)
 
             if dspy.settings.release >= 20230928:
                 predictor.demos = raw_demos + augmented_demos
             else:
```

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/copro_optimizer.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/copro_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,16 +170,14 @@
             else:
                 instruct = dspy.Predict(
                     BasicGenerateInstruction,
                     n=self.breadth - 1,
                     temperature=self.init_temperature,
                 )(basic_instruction=basic_instruction)
             # Add in our initial prompt as a candidate as well
-            instruct.completions.proposed_instruction.append(basic_instruction)
-            instruct.completions.proposed_prefix_for_output_field.append(basic_prefix)
             candidates[id(predictor)] = instruct.completions
             evaluated_candidates[id(predictor)] = {}
 
         if self.prompt_model:
             dspy.logger.debug(f"{self.prompt_model.inspect_history(n=1)}")
 
         latest_candidates = candidates
@@ -320,17 +318,16 @@
                         temperature=self.init_temperature,
                     )(attempted_instructions=attempts)
 
                 if self.prompt_model:
                     dspy.logger.debug(f"(self.prompt_model.inspect_history(n=1)) {self.prompt_model.inspect_history(n=1)}")
                 # Get candidates for each predictor
                 new_candidates[id(p_base)] = instr.completions
-                all_candidates[id(p_base)].proposed_instruction.extend(instr.completions.proposed_instruction)
-                all_candidates[id(p_base)].proposed_prefix_for_output_field.extend(
-                    instr.completions.proposed_prefix_for_output_field,
+                all_candidates[id(p_base)].completions.extend_examples(
+                    instr.completions,
                 )
 
             if self.prompt_model:
                 dspy.logger.debug(f"{self.prompt_model.inspect_history(n=1)}")
             latest_candidates = new_candidates
 
         candidates = []
```

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/ensemble.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/ensemble.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/finetune.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/finetune.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/knn_fewshot.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/knn_fewshot.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/mipro_optimizer.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/mipro_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 * prompt_model: The model used for prompt generation. When unspecified, defaults to the model set in settings (i.e., dspy.settings.configure(lm=task_model)).
 * task_model: The model used for prompt generation. When unspecified, defaults to the model set in settings (i.e., dspy.settings.configure(lm=task_model)).
 * metric: The task metric used for optimization.
 * num_candidates: The number of new prompts and sets of fewshot examples to generate and evaluate. Default=10.
 * init_temperature: The temperature used to generate new prompts. Higher roughly equals more creative. Default=1.0.
 * verbose: Tells the method whether or not to print intermediate steps.
 * track_stats: Tells the method whether or not to track statistics about the optimization process.
-                If True, the method will track a dictionary with a key corresponding to the trial number, 
+                If True, the method will track a dictionary with a key corresponding to the trial number,
                 and a value containing a dict with the following keys:
                     * program: the program being evaluated at a given trial
                     * score: the last average evaluated score for the program
                     * pruned: whether or not this program was pruned
                 This information will be returned as attributes of the best program.
 """
 
@@ -291,20 +291,18 @@
                             basic_instruction=basic_instruction,
                             observations=self.observations,
                             examples=example_sets[id(predictor)][i],
                         )
                         if not instruct:
                             instruct = new_instruct
                         else:
-                            instruct.completions.proposed_instruction.extend(
-                                new_instruct.completions.proposed_instruction,
-                            )
-                            instruct.completions.proposed_prefix_for_output_field.extend(
-                                new_instruct.completions.proposed_prefix_for_output_field,
+                            instruct.completions.extend_examples(
+                                new_instruct.completions.examples,
                             )
+
                 # Just data
                 elif view_data:
                     instruct = dspy.Predict(
                         BasicGenerateInstructionWithDataObservations,
                         n=N - 1,
                         temperature=self.init_temperature,
                     )(basic_instruction=basic_instruction, observations=self.observations)
@@ -332,16 +330,20 @@
                 # Neither
                 else:
                     instruct = dspy.Predict(BasicGenerateInstruction, n=N - 1, temperature=self.init_temperature)(
                         basic_instruction=basic_instruction,
                     )
 
             # Add in our initial prompt as a candidate as well
-            instruct.completions.proposed_instruction.insert(0, basic_instruction)
-            instruct.completions.proposed_prefix_for_output_field.insert(0, basic_prefix)
+            new_example = dspy.Example(
+                basic_instruction=basic_instruction,
+                proposed_instruction=basic_instruction,
+                proposed_prefix_for_output_field=basic_prefix,
+            )
+            instruct.completions.add_example(new_example, 0)
             candidates[id(predictor)] = instruct.completions
             evaluated_candidates[id(predictor)] = {}
 
         if self.verbose:
             self._print_model_history(self.prompt_model)
 
         return candidates, evaluated_candidates
@@ -369,40 +371,42 @@
         random.seed(seed)
 
         estimated_task_model_calls_wo_module_calls = len(trainset) * num_trials  # M * T * P
         estimated_prompt_model_calls = 10 + self.num_candidates * len(
             student.predictors(),
         )  # num data summary calls + N * P
 
-        user_message = textwrap.dedent(f"""\
+        user_message = textwrap.dedent(
+            f"""\
             {YELLOW}{BOLD}WARNING: Projected Language Model (LM) Calls{ENDC}
 
             Please be advised that based on the parameters you have set, the maximum number of LM calls is projected as follows:
 
             {YELLOW}- Task Model: {BLUE}{BOLD}{len(trainset)}{ENDC}{YELLOW} examples in dev set * {BLUE}{BOLD}{num_trials}{ENDC}{YELLOW} trials * {BLUE}{BOLD}# of LM calls in your program{ENDC}{YELLOW} = ({BLUE}{BOLD}{estimated_task_model_calls_wo_module_calls} * # of LM calls in your program{ENDC}{YELLOW}) task model calls{ENDC}
             {YELLOW}- Prompt Model: # data summarizer calls (max {BLUE}{BOLD}10{ENDC}{YELLOW}) + {BLUE}{BOLD}{self.num_candidates}{ENDC}{YELLOW} * {BLUE}{BOLD}{len(student.predictors())}{ENDC}{YELLOW} lm calls in program = {BLUE}{BOLD}{estimated_prompt_model_calls}{ENDC}{YELLOW} prompt model calls{ENDC}
 
             {YELLOW}{BOLD}Estimated Cost Calculation:{ENDC}
 
-            {YELLOW}Total Cost = (Number of calls to task model * (Avg Input Token Length per Call * Task Model Price per Input Token + Avg Output Token Length per Call * Task Model Price per Output Token) 
+            {YELLOW}Total Cost = (Number of calls to task model * (Avg Input Token Length per Call * Task Model Price per Input Token + Avg Output Token Length per Call * Task Model Price per Output Token)
                         + (Number of calls to prompt model * (Avg Input Token Length per Call * Task Prompt Price per Input Token + Avg Output Token Length per Call * Prompt Model Price per Output Token).{ENDC}
 
             For a preliminary estimate of potential costs, we recommend you perform your own calculations based on the task
             and prompt models you intend to use. If the projected costs exceed your budget or expectations, you may consider:
 
             {YELLOW}- Reducing the number of trials (`num_trials`), the size of the trainset, or the number of LM calls in your program.{ENDC}
             {YELLOW}- Using a cheaper task model to optimize the prompt.{ENDC}""")
 
         user_confirmation_message = textwrap.dedent(f"""\
             To proceed with the execution of this program, please confirm by typing {BLUE}'y'{ENDC} for yes or {BLUE}'n'{ENDC} for no.
 
             If you would like to bypass this confirmation step in future executions, set the {YELLOW}`requires_permission_to_run`{ENDC} flag to {YELLOW}`False` when calling compile.{ENDC}
 
             {YELLOW}Awaiting your input...{ENDC}
-        """)
+        """,
+        )
 
         print(user_message)
 
         sys.stdout.flush()  # Flush the output buffer to force the message to print
 
         run = True
         if requires_permission_to_run:
```

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/random_search.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/random_search.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt_bayesian.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt_typed.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/signature_opt_typed.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/teleprompt_optuna.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/teleprompt_optuna.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/teleprompt/vanilla.py` & `dspy_ai-2.5.0rc2/dspy/teleprompt/vanilla.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/dspy/utils/dummies.py` & `dspy_ai-2.5.0rc2/dspy/utils/dummies.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import random
 import re
+import typing as t
 from typing import Union
 
 import numpy as np
+from pydantic import BaseModel, Field
 
 from dsp.modules import LM
 from dsp.utils.utils import dotdict
+from dspy.modeling.backends.text import TextBackend
+from dspy.primitives.example import Example
+from dspy.primitives.prediction import Completions
+from dspy.signatures.signature import InputField, OutputField, Signature
 
 
 class DummyLM(LM):
     """Dummy language model for unit testing purposes."""
 
     def __init__(self, answers: Union[list[str], dict[str, str]], follow_examples: bool = False):
         """Initializes the dummy language model.
@@ -37,21 +43,26 @@
                 _instructions, _format, *examples, _output = prompt.split("\n---\n")
                 examples_str = "\n".join(examples)
                 possible_answers = re.findall(prefix + r"\s*(.*)", examples_str)
                 if possible_answers:
                     # We take the last answer, as the first one is just from
                     # the "Follow the following format" section.
                     answer = possible_answers[-1]
-                    print(f"DummyLM got found previous example for {prefix} with value {answer=}")
+                    print(
+                        f"DummyLM got found previous example for {prefix} with value {answer=}",
+                    )
                 else:
                     print(f"DummyLM couldn't find previous example for {prefix=}")
 
             if answer is None:
                 if isinstance(self.answers, dict):
-                    answer = next((v for k, v in self.answers.items() if k in prompt), None)
+                    answer = next(
+                        (v for k, v in self.answers.items() if k in prompt),
+                        None,
+                    )
                 else:
                     if len(self.answers) > 0:
                         answer = self.answers[0]
                         self.answers = self.answers[1:]
 
             if answer is None:
                 answer = "No more responses"
@@ -143,7 +154,48 @@
                 vec[self._hash(gram)] += 1
             vecs.append(vec)
 
         vecs = np.array(vecs, dtype=np.float32)
         vecs -= np.mean(vecs, axis=1, keepdims=True)
         vecs /= np.linalg.norm(vecs, axis=1, keepdims=True) + 1e-10  # Added epsilon to avoid division by zero
         return vecs
+
+
+class DummySignature(Signature):
+    """Produce the answer given the question"""
+
+    question = InputField()
+    answer = OutputField()
+
+
+def make_dummy_completions(signature, list_of_dicts: list[dict[str, t.Any]]):
+    examples = [Example(**kwargs) for kwargs in list_of_dicts]
+    return Completions(
+        signature=DummySignature,
+        examples=examples,
+        input_kwargs={},
+    )
+
+
+class DummyResponse(BaseModel):
+    choices: list = Field(default_factory=list)
+
+
+class DummyBackend(TextBackend):
+    model: str = Field(default="dummy")
+    answers: list[list[str]] = Field(default_factory=list)
+    step: int = Field(default=0)
+
+    def generate(self, signature: Signature, demos: list[str], config: dict[str, t.Any], **kwargs) -> Completions:
+        example = Example(demos=demos, **kwargs)
+
+        model_kwargs = self.prepare_request(signature, example, config)
+
+        if len(self.answers) <= self.step:
+            raise ValueError("not enough answers provided")
+
+        response = DummyResponse(
+            choices=[{"message": {"content": c}, "finish_reason": "done"} for c in self.answers[self.step]],
+        )
+        self.step += 1
+
+        return self.process_response(signature, example, response, input_kwargs=model_kwargs)
```

### Comparing `dspy_ai-2.5.0rc1/dspy/utils/logging.py` & `dspy_ai-2.5.0rc2/dspy/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dspy_ai-2.5.0rc1/pyproject.toml` & `dspy_ai-2.5.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dspy-ai"
-version = "2.5.0rc1"
+version = "2.5.0rc2"
 description = "DSPy"
 readme = "README.md"
 authors = [{ name = "Omar Khattab", email = "okhattab@stanford.edu" }]
 license = { text = "MIT License" }
 requires-python = ">=3.9, <3.13"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -64,15 +64,15 @@
 fastembed = ["fastembed>=0.2.0"]
 
 [project.urls]
 homepage = "https://github.com/stanfordnlp/dspy"
 
 [tool.poetry]
 name = "dspy-ai"
-version = "2.5.0rc1"
+version = "2.5.0rc2"
 description = "DSPy: The framework for programming—not prompting—foundation models"
 authors = ["Omar Khattab <okhattab@stanford.edu>"]
 maintainers = ["Cyrus Nouroozi <cyrus@edendaolab.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/stanfordnlp/dspy"
 repository = "https://github.com/stanfordnlp/dspy"
```

### Comparing `dspy_ai-2.5.0rc1/PKG-INFO` & `dspy_ai-2.5.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.5.0rc1
+Version: 2.5.0rc2
 Summary: DSPy: The framework for programming—not prompting—foundation models
 Home-page: https://github.com/stanfordnlp/dspy
 License: MIT
 Keywords: dspy,ai,language models,llm,openai
 Author: Omar Khattab
 Author-email: okhattab@stanford.edu
 Maintainer: Cyrus Nouroozi
```

