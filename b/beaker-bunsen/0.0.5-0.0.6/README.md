# Comparing `tmp/beaker_bunsen-0.0.5.tar.gz` & `tmp/beaker_bunsen-0.0.6.tar.gz`

## Comparing `beaker_bunsen-0.0.5.tar` & `beaker_bunsen-0.0.6.tar`

### file list

```diff
@@ -1,97 +1,106 @@
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/DEFINITIONS.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/.github/workflows/build-publish.yaml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/.github/workflows/test.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/bunsen_agent.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/bunsen_context.py
--rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/corpus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/builder/__init__.py
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/builder/hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/scripts/__init__.py
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/scripts/bunsen.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/__init__.py
--rw-r--r--   0        0        0    14333 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/chromadb_store.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/types.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/vector_store.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/base.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/code.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/document.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/documentation.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/examples.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/__init__.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/base.py
--rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/code_library_loader.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/local_file_loader.py
--rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/schemes.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/util/helpers.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/util/splitters.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_base_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_build.py
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_chromadb.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_code_loaders.py
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_corpus.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_documentation_embedder.py
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_example_embedder.py
--rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_local_file_loader.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_schemes.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_utils.py
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_zipped_chromadb.py
--rw-r--r--   0        0        0  1828380 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/store.zip
--rw-r--r--   0        0        0  5947974 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/corpus.zip
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/config.yaml
--rw-r--r--   0        0        0  5692346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/store.zip
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.__version__
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.adapters
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.api
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.auth
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.certs
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.compat
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.cookies
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.exceptions
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.help
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.hooks
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.models
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.packages
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.sessions
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.status_codes
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.structures
--rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.utils
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documentation/ruff_readme.md
--rw-r--r--   0        0        0   137697 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/Lunar_Sample_Laboratory_Facility.html
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/yorkshire.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/yorkshire.txt.metadata
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/.metadata
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/ham_and_lentil_soup
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/irish_potato_caserole
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/tajine_maadnous
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/winter_risotto
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/winter_risotto.metadata
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/examples/example_1.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/examples/example_2.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/examples/example_3.md
--rw-r--r--   0        0        0   307464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/images/kitten-sad.jpg
--rw-r--r--   0        0        0   417493 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/images/kitten_hacker.jpg
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/images/puppy_hacker.jpg
--rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/images/puppy_sad.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/pyproject.toml
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/documentation/ruff_readme.md
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/examples/example_1.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/examples/example_2.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/examples/example_3.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/src/test_project/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/src/test_project/agent.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/src/test_project/context.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/README.md
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/DEFINITIONS.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/.github/workflows/build-publish.yaml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/__init__.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/bunsen_agent.py
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/bunsen_context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/builder/__init__.py
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/builder/hooks.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/__init__.py
+-rw-r--r--   0        0        0     9839 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/corpus.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/protocols.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/types.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/__init__.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/base.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/code.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/document.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/documentation.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/examples.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/__init__.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/base.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/code_library_loader.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/local_file_loader.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/schemes.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/resources/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/resources/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/util/__init__.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/util/helpers.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/util/logging.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/util/splitters.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/vector_stores/__init__.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/vector_stores/base_vector_store.py
+-rw-r--r--   0        0        0    14363 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/vector_stores/chromadb_store.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/scripts/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/scripts/bunsen.py
+-rw-r--r--   0        0        0    11511 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/scripts/extract_documentation.py
+-rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/scripts/extract_examples.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/src/beaker_bunsen/scripts/helpers.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_base_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_build.py
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_chromadb.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_code_loaders.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_corpus.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_documentation_embedder.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_example_embedder.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_local_file_loader.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_schemes.py
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_utils.py
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/test_zipped_chromadb.py
+-rw-r--r--   0        0        0  1828380 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/store.zip
+-rw-r--r--   0        0        0  5947974 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/corpus.zip
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/config.yaml
+-rw-r--r--   0        0        0  5692346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/store.zip
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.__version__
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils
+-rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.adapters
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.api
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.auth
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.certs
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.compat
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.cookies
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.exceptions
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.help
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.hooks
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.models
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.packages
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.sessions
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.status_codes
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.structures
+-rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.utils
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documentation/ruff_readme.md
+-rw-r--r--   0        0        0   137697 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/Lunar_Sample_Laboratory_Facility.html
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/yorkshire.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/yorkshire.txt.metadata
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/recipes/.metadata
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/recipes/ham_and_lentil_soup
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/recipes/irish_potato_caserole
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/recipes/tajine_maadnous
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/recipes/winter_risotto
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/documents/recipes/winter_risotto.metadata
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/examples/example_1.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/examples/example_2.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/examples/example_3.md
+-rw-r--r--   0        0        0   307464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/images/kitten-sad.jpg
+-rw-r--r--   0        0        0   417493 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/images/kitten_hacker.jpg
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/images/puppy_hacker.jpg
+-rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/images/puppy_sad.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/pyproject.toml
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/documentation/ruff_readme.md
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/examples/example_1.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/examples/example_2.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/examples/example_3.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/src/test_project/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/src/test_project/agent.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/tests/data/subproject/src/test_project/context.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/README.md
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.6/PKG-INFO
```

### Comparing `beaker_bunsen-0.0.5/DEFINITIONS.md` & `beaker_bunsen-0.0.6/DEFINITIONS.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/.github/workflows/build-publish.yaml` & `beaker_bunsen-0.0.6/.github/workflows/build-publish.yaml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/.github/workflows/test.yaml` & `beaker_bunsen-0.0.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/bunsen_agent.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/bunsen_agent.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/bunsen_context.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/bunsen_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from beaker_kernel.lib.autodiscovery import LIB_LOCATIONS
 from beaker_kernel.lib.context import BaseContext
 from beaker_kernel.lib.subkernels.python import PythonSubkernel
 from beaker_kernel.lib.utils import action
 
 from .bunsen_agent import BunsenAgent
-from .corpus import Corpus
+from .corpus.corpus import Corpus
 
 if TYPE_CHECKING:
     from beaker_kernel.kernel import LLMKernel
     from beaker_kernel.lib.subkernels.base import BaseSubkernel
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/corpus.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/corpus.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import tempfile
 import yaml
 import zipfile
 from collections import defaultdict
 from pathlib import Path
 from typing import Type
 from typing_extensions import Self
-from urllib.parse import urlparse
 
-from .vectordb.chromadb_store import ChromaDBLocalStore, ZippedChromaDBStore
-from .vectordb.vector_store import VectorStore
-from .vectordb.loaders import BaseLoader, BaseCodeLoader, LocalFileLoader, PythonLibraryLoader
-from .vectordb.loaders.schemes import read_from_uri, CorpusResourceScheme
-from .vectordb.embedders import BaseEmbedder, DocumentationEmbedder
-from .vectordb.types import (
-    Record, Resource, Embedding, Image, Metadata, QueryResponse, QueryResult, RecordBundle, EmbeddingFunction,
-    DefaultType, Default,
+from .vector_stores.chromadb_store import ChromaDBLocalStore, ZippedChromaDBStore
+from .vector_stores.base_vector_store import VectorStore
+from .loaders import BaseLoader, BaseCodeLoader, LocalFileLoader, PythonLibraryLoader
+from .loaders.schemes import read_from_uri, CorpusResourceScheme
+from .embedders import BaseEmbedder, DocumentationEmbedder
+from .types import (
+    Record, Embedding, Image, Metadata, QueryResponse, QueryResult, RecordBundle,
+    DefaultType, Default, URI,
 )
-from .vectordb.util.helpers import common_path_portion
-
+from .protocols import EmbeddingFunction
+from .resources import Resource
+from .util.helpers import common_path_portion
 
 
 class Corpus:
     """
     A corpus is a single, self-contained interface for querying over documents and other records embedded in a vector database.
     """
     embedder_map: dict[str, BaseEmbedder]
@@ -63,14 +63,15 @@
         if not dir_path.is_dir():
             raise FileNotFoundError(f"Provided corpus directory `{dir_path}` does not exist or is invalid.")
         if not (config_path.is_file() and store_path.is_file() and resource_dir.is_dir()):
             raise FileNotFoundError(f"Corpus is corrupt or missing required files and cannot be loaded.")
 
         store_config = config.get("store", {})
         if "default_embedding_function" in store_config:
+            print("config", store_config)
             func = EmbeddingFunction.from_uri(store_config["default_embedding_function"])
             store_config["default_embedding_function"] = func
         store = ZippedChromaDBStore(
             path=store_path,
             **store_config
         )
         default_embedding_function = EmbeddingFunction.from_uri(config.get("default_embedding_function", None))
@@ -154,29 +155,28 @@
             for record in temp_store.get_all(partition=partition, include_embeddings=True):
                 if record.uri:
                     resources[partition].add(record.uri)
                     records_to_update_by_partition[partition].append(record)
 
         partition_common_paths = {
             partition: common_path_portion([
-                urlparse(uri).path
+                uri.path
                 for uri in resources[partition]
                 if uri.startswith(("file:", "zipped-file:"))
             ])
             for partition in partitions
         }
 
         uri_remap = {}
         for (partition, resource_set) in resources.items():
             for resource_uri in resource_set:
-                uri_parts = urlparse(resource_uri)
-                if uri_parts.scheme in ("file", "zipped-file"):
-                    uri_path = Path(uri_parts.path).relative_to(partition_common_paths[partition])
+                if resource_uri.scheme in ("file", "zipped-file"):
+                    uri_path = Path(resource_uri.path).relative_to(partition_common_paths[partition])
                 else:
-                    uri_path = Path(uri_parts.path)
+                    uri_path = Path(resource_uri.path)
 
                 resource_path = Path(partition) / uri_path
                 new_uri = CorpusResourceScheme.get_uri_for_location(resource_path)
                 content = read_from_uri(resource_uri)
                 mode = "wb" if isinstance(content, bytes) else "w"
                 dest = resource_dir / resource_path
                 if not dest.parent.exists():
@@ -219,19 +219,20 @@
                         arcpath = os.path.join(dirpath.removeprefix(tmpdir), file).lstrip('/')
                         filepath = os.path.join(dirpath, file)
                         corpus_zipfile.write(filename=filepath, arcname=arcpath)
         finally:
             shutil.rmtree(tmpdir)
 
     def read_resource(self, location_or_uri: str):
-        parsed_uri = urlparse(str(location_or_uri))
-        if parsed_uri.scheme and parsed_uri.scheme != CorpusResourceScheme.URI_SCHEME:
+        uri = URI(location_or_uri)
+        # parsed_uri = urlparse(str(location_or_uri))
+        if uri.scheme and uri.scheme != CorpusResourceScheme.URI_SCHEME:
             return read_from_uri(location_or_uri)
 
-        resource_location = parsed_uri.path.lstrip("/")
+        resource_location = uri.path.lstrip("/")
         full_resource_path = Path(self.resource_location) / resource_location
         with full_resource_path.open() as resource_fp:
             content = resource_fp.read()
         return content
 
     def query(self,
         query_string: str,
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/builder/hooks.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/builder/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from typing import Any
 
 from hatchling.builders.config import BuilderConfig
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 from hatchling.plugin import hookimpl
 
 from beaker_kernel.lib.context import BaseContext
-from ..vectordb.embedders import DocumentationEmbedder, ExampleEmbedder, CodeEmbedder, PythonEmbedder
-from ..vectordb.loaders import LocalFileLoader, PythonLibraryLoader, RCRANSourceLoader
-from ..vectordb.loaders.code_library_loader import RCRANLocalCache
-from ..vectordb.chromadb_store import ZippedChromaDBStore
-from ..corpus import Corpus
+from ..corpus.corpus import Corpus
+from ..corpus.resources import ResourceType
+from ..corpus.embedders import DocumentationEmbedder, ExampleEmbedder, CodeEmbedder, PythonEmbedder
+from ..corpus.loaders import LocalFileLoader, PythonLibraryLoader, RCRANSourceLoader
+from ..corpus.loaders.code_library_loader import RCRANLocalCache
+from ..corpus.vector_stores.chromadb_store import ZippedChromaDBStore
 
 
 logger = logging.getLogger("bunsen_build")
 
 class BuildError(Exception):
     pass
 
@@ -100,54 +101,58 @@
         corpus = Corpus(store=store)
 
         documentation_path = self.config.get("documentation_path", "documentation")
         examples_path = self.config.get("examples_path", "examples")
         python_libraries = self.config.get("python_libraries", [])
         r_cran_libraries = self.config.get("r_cran_libraries", [])
 
-        if documentation_path and os.path.exists(documentation_path):
-            corpus.ingest(
-                embedder_cls=DocumentationEmbedder,
-                loader=LocalFileLoader(locations=[documentation_path]),
-                partition="documentation",
-            )
-
-        if examples_path and os.path.exists(examples_path):
-            corpus.ingest(
-                embedder_cls=ExampleEmbedder,
-                loader=LocalFileLoader(locations=[examples_path]),
-                partition="examples",
-            )
-
-        if python_libraries:
-            corpus.ingest(
-                embedder_cls=PythonEmbedder,
-                loader=PythonLibraryLoader(locations=python_libraries, metadata={"language": "python"}),
-                partition="code"
-            )
-
-        if r_cran_libraries:
-            with RCRANLocalCache(locations=r_cran_libraries):
+        with RCRANLocalCache(locations=r_cran_libraries) as cache:
+            if r_cran_libraries:
                 corpus.ingest(
                     embedder_cls=CodeEmbedder,
-                    loader=RCRANSourceLoader(locations=r_cran_libraries, metadata={"language": "r"}),
+                    loader=RCRANSourceLoader(
+                        locations=[*r_cran_libraries, "!/man", "!/vignettes"],
+                        metadata={"language": "r"}
+                    ),
                     partition="code",
                 )
 
-        examples = corpus.store.get_all(partition="examples")
-        if examples:
-            failures = self.test_examples(examples)
-            if failures and not self.config.get("ignore_example_errors", False):
-                # TODO: Finish this
-                # TODO: Should example testing just be in the ExampleEmbedder durring embedding instead of here?
-                print("These examples failed")
-                print(failures)
-                raise BuildError("Example test failed and not ignored.")
+            if documentation_path and os.path.exists(documentation_path):
+                corpus.ingest(
+                    embedder_cls=DocumentationEmbedder,
+                    loader=LocalFileLoader(locations=[documentation_path], resource_type=ResourceType.Documentation),
+                    partition="documentation",
+                )
+
+            if examples_path and os.path.exists(examples_path):
+                corpus.ingest(
+                    embedder_cls=ExampleEmbedder,
+                    loader=LocalFileLoader(locations=[examples_path], resource_type=ResourceType.Example),
+                    partition="examples",
+                )
+
+            if python_libraries:
+                corpus.ingest(
+                    embedder_cls=PythonEmbedder,
+                    loader=PythonLibraryLoader(locations=python_libraries, metadata={"language": "python"}),
+                    partition="code"
+                )
+
+
+            examples = corpus.store.get_all(partition="examples")
+            if examples:
+                failures = self.test_examples(examples)
+                if failures and not self.config.get("ignore_example_errors", False):
+                    # TODO: Finish this
+                    # TODO: Should example testing just be in the ExampleEmbedder durring embedding instead of here?
+                    print("These examples failed")
+                    print(failures)
+                    raise BuildError("Example test failed and not ignore-test-fail not set.")
 
-        corpus.save_to_dir(corpus_path, overwrite=True)
+            corpus.save_to_dir(corpus_path, overwrite=True)
 
         return corpus_path
 
     def build_beaker_context(self, base_path: str):
 
         dest_dir = "build/contexts"
         pkg_name = os.path.basename(base_path)
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/scripts/bunsen.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/scripts/extract_documentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,32 @@
 import click
 import datetime
 import json
 import os
 import os.path
+import re
 import toml
 from collections import defaultdict
+from functools import reduce
 from pathlib import Path
 from urllib.parse import urlparse
 
 import openai
 
-from ..vectordb.types import Resource
-from ..vectordb.loaders.schemes import unmap_scheme, read_from_uri
-from ..vectordb.loaders.code_library_loader import RCRANLocalCache
-
-
-def find_pyproject_file() -> Path | None:
-    cwd = Path.cwd()
-    for path in [cwd, *cwd.parents]:
-        potential_file = path / "pyproject.toml"
-        if potential_file.is_file():
-            return potential_file
-    return None
+from ..corpus.resources import Resource
+from ..corpus.loaders.schemes import unmap_scheme, read_from_uri
+from ..corpus.loaders.code_library_loader import RCRANLocalCache
 
-
-@click.group()
-def cli():
-    """
-    CLI Tooling to help build Bunsen contexts
-    """
-    pass
+from .helpers import find_pyproject_file
 
 
 # TODO: Add optional param for setting destination
-@cli.command()
+@click.command()
 @click.argument("locations", type=str, required=False, nargs=-1)
-def extract_examples(locations: list[str]):
+def extract_documentation(locations: list[str]):
 
     dest = 'examples-unverified'
     if not os.path.exists(dest):
         os.makedirs(dest)
 
     sources: dict[str, list[str]] = defaultdict(lambda: [])
     if locations:
@@ -108,23 +95,29 @@
                 content = resource.content
             else:
                 if resource.file_handle and not resource.file_handle.closed and resource.file_handle.readable():
                     content = resource.file_handle.read()
                 else:
                     content = read_from_uri(resource.uri)
 
+            content_lines = content.splitlines(keepends=True)
             prompt = """
 A document is provided below. It contains line numbers on the left, the content on the right, with the sides separated by ` : `.
 The provided document may be a source code file, a documentation page, an executable notebook, or hand extracted examples created by hand.
 It may contain one or more curated examples as for how to accomplish something using relevant libraries.
-Please identify any such examples and generate a short description of the purpose of the example code, along with the line number on which it occurs.
+Please identify any such examples and generate a short description of the purpose of the example code, along with the start/stop line numbers (inclusive) where the example occurs.
+For example, if the example is a single line on the line labeled 34, both `start_line` and `stop_line` would be equal to 34.
+If the example was spread of 5 lines, starting at line 12, the values would be `start_line` = 12, `stop_line` = 16.
 Also, make sure to include a prelude of code that contains any imports or definitions needed so the example is as complete as possible and has everything it needs to run as a stand-alone code block.
 The prelude will later be combined with the example to help use the libraries these documents are related to.
 Please ensure that all imports and definitions in the prelude are complete. Do not use statements like "put your code here..." or summarize what should be done.
 Do not identify/extract regular source code from files as examples. Only extract unique tasks that demonstrate how to properly use the library.
+That is, all exracted examples should show usage of functions, not just the code that defines a function. Assume the user will be able to look up argument and parameter information.
+You should err on the side of fewer, more complete examples which show an entire "step" of work rather than examples of subtasks.
+As an example, if you find sample code where a dataset is sorted and a comparison function is defined to help sort, only extract one example that includes all the code. Do not create a separate example of how to define a comparison function.
 If you do not find any examples in the document, do not generate one yourself. Instead return an empty list.
 
 Please be sure to format your answer in json format as response object that matches this format with one object per example object in the `examples` list:
   {
     "examples": [
       {
         "description": str,
@@ -136,15 +129,15 @@
     ]
   }
 
 The document from which to extract begins below this line and runs until the end of the input:\n"""
 
             full_prompt = "\n".join([
                 prompt,
-                "".join(f"{line_no:6} : {line}" for line_no, line in enumerate(content.splitlines(keepends=True), start=1)),
+                "".join(f"{line_no:6} : {line}" for line_no, line in enumerate(content_lines, start=1)),
             ])
             model = "gpt-4o"
 
             response = openai.chat.completions.create(
                 model=model,
                 messages=[
                     {
@@ -160,15 +153,15 @@
                         "content": full_prompt,
                     }
                 ],
                 response_format={"type": "json_object"},
             )
 
             metadata = {
-                "resource_d": resource.id,
+                "resource_id": resource.id,
                 "source_uri": resource.uri,
                 "generated_at": datetime.datetime.utcnow().isoformat(),
                 "source_sha256_hash": "TODO",
             }
 
             if not response:
                 continue
@@ -186,40 +179,85 @@
                         f"{'====' * 20}\n"
                     )
                     json.dump(metadata, failure_file, indent=2)
                     failure_file.write(
                         f"\n{'====' * 20}\n"
                         f"{err}\n{err.msg}\n"
                     )
-
                 continue
+
             if not example_list:
                 continue
 
             click.echo(f"Found {len(example_list)} examples in {resource.uri}")
             for example_num, example in enumerate(example_list, start=1):
                 example_filename = os.path.join(dest, f"example_{num}_{example_num}.md")
                 example_metadata_filename = f"{example_filename}.metadata"
                 start = int(example["start_line"]) - 1
                 stop = int(example["stop_line"])
-                example_code = "".join(content.splitlines(keepends=True)[start:stop])
+                prelude_lines = example.get("prelude", "").splitlines(keepends=True)
+                prelude = clean_codeblock(prelude_lines) if prelude_lines else ""
+                example_code_lines = content_lines[start:stop]
+                example_code = clean_codeblock(example_code_lines)
+
                 example_metadata = {
                     **metadata,
                     "start_line": start,
                     "stop_line": stop,
                 }
 
                 with open(example_filename, "w") as example_file, open(example_metadata_filename, "w") as example_metadata_file:
                     example_file.write(f"""
 # Description
 {example["description"]}
 
 # Code
 ```
-{example["prelude"]}
+{prelude}
 {example_code}
 ```
 """.lstrip())
                     json.dump(example_metadata, example_metadata_file, indent=2)
 
             # Iterate source file num for next loop
             num += 1
+
+
+def should_ignore_line(line: str) -> bool:
+    """
+    Returns a boolean as to whether a particular line should be kept or ignored when importing code.
+    We should ignore extraneous whitespace, code-block indicators, decorative lines, etc that do are not semantically
+    meaningful.
+    """
+    # Todo: Other leading/trailing lines we need to clean?
+    if (
+        re.search(r'\S', line) == None  # Line does not contain at least one non-whitespace character
+        or line.startswith('```')
+    ):
+        return True
+    return False
+
+
+def clean_codeblock(code: list[str]) -> str:
+    if not code:
+        return ""
+    top, bottom = 0, len(code) - 1
+    while should_ignore_line(code[top]) and top < len(code) - 1:
+        top += 1
+    while should_ignore_line(code[bottom]) and bottom > top:
+        bottom -= 1
+    split_lines = [re.split(r'(\s)', line) for line in code[top:bottom]]
+    line_count = len(split_lines)
+    vertical_parts = list(zip(*split_lines))
+    for idx, section in enumerate(vertical_parts):
+        correct_size = len(section) == line_count
+        all_match, _ = reduce(
+            lambda match_tuple, next_val: (match_tuple[1] == next_val, match_tuple[1]),
+            section,
+            (True, section[0])
+        )
+        if not (correct_size and all_match):
+            break
+    else:
+        idx = None
+    unprefixed_lines = ["".join(split_line[idx:]) for split_line in split_lines]
+    return "".join(unprefixed_lines)
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/chromadb_store.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/vector_stores/chromadb_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from typing import Any, Sequence, Callable
 from typing_extensions import Self
 from zipfile import ZipFile
 
 import chromadb
 from chromadb.api import ClientAPI
 
-from .types import Record, RecordBundle, QueryResponse, QueryResponse, EmbeddingFunction
-from .vector_store import VectorStore
-from .loaders.base import BaseLoader
+from ..types import Record, RecordBundle, QueryResponse, QueryResponse
+from ..protocols import EmbeddingFunction
+from .base_vector_store import VectorStore
+from ..loaders.base import BaseLoader
 
 
 class BaseChromaDBStore(VectorStore):
     client: ClientAPI
     default_partition: str
 
     _chromadb_get_include = ["documents", "metadatas", "uris"]
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/vector_store.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/vector_stores/base_vector_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from dataclasses import dataclass
 from typing import Any, Union, Sequence, TypedDict
 from typing_extensions import Self
 from numpy.typing import NDArray
 import logging
 import numpy as np
 
-from .types import Record, RecordBundle, QueryResponse, Resource, EmbeddingFunction
-from .loaders.base import BaseLoader
+from ..types import Record, RecordBundle, QueryResponse
+from ..protocols import EmbeddingFunction
+from ..resources import Resource
+from ..loaders.base import BaseLoader
 
 
 logger = logging.getLogger("beaker_bunsen")
 
 
 class VectorStore(ABC):
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/base.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-from typing import Iterator
+import logging
+from typing import Iterator, TYPE_CHECKING
 
-from .. import logger
+from ..protocols import EmbeddingFunction
 from ..loaders.base import BaseLoader
 from ..loaders.schemes import read_from_uri
-from ..types import Resource, Record, RecordBundle, EmbeddingFunction, DefaultType, Default
-from ..vector_store import VectorStore
+from ..types import Record, RecordBundle, DefaultType, Default
+from ..resources import Resource
+from ..vector_stores.base_vector_store import VectorStore
+
+
+logger = logging.getLogger("beaker_bunsen")
 
 
 class BaseEmbedder:
     default_loader: BaseLoader | None
     store: VectorStore
     embedding_function: EmbeddingFunction | None
     chunk_size: int
@@ -25,30 +30,16 @@
 
         self.default_loader = loader
         self.store = store
         self.embedding_function = embedding_function
         self.chunk_size = chunk_size
         self.chunk_overlap = chunk_overlap
 
-    def read_resource(self, resource: Resource) -> str | bytes | None:
-        if resource.content:
-            return resource.content
-        elif resource.file_handle:
-            try:
-                resource.file_handle.seek(0)
-            except IOError:
-                pass
-            return resource.file_handle.read()
-        elif resource.uri:
-            return read_from_uri(resource.uri)
-        else:
-            return None
-
     def prepare_records_from_resource(self, resource: Resource) -> Iterator[Record]:
-        content = self.read_resource(resource)
+        content = resource.read()
 
         if not content:
             raise ValueError(f"Unable to determine content for resource `{resource.id}` @ `{resource.uri}`")
 
         record = Record(
             id=resource.id,
             uri=resource.uri,
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/code.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/code.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 from typing import Iterator
-from urllib.parse import urlparse
 
-from beaker_bunsen.vectordb.loaders.base import BaseLoader
-from beaker_bunsen.vectordb.types import EmbeddingFunction
-from beaker_bunsen.vectordb.vector_store import VectorStore
+from beaker_bunsen.corpus.loaders.base import BaseLoader
+from beaker_bunsen.corpus.vector_stores.base_vector_store import VectorStore
 
-from ..types import Resource, Record
-from .base import BaseEmbedder
 from .document import DocumentEmbedder
+from ..resources import Resource
 from ..loaders.schemes import read_from_uri
 from ..util.helpers import count_words
 from ..util.splitters import RecursiveCharacterTextSplitter
 
 
 class CodeEmbedder(DocumentEmbedder):
 
     SCHEME_MAP = {
         "py-mod": 'python',
     }
 
     def get_splitter(self, resource: Resource):
-        url_parts = urlparse(resource.uri)
-        scheme = url_parts.scheme
-        path = url_parts.path
+        scheme = resource.uri.scheme
+        path = resource.uri.path
         language = self.SCHEME_MAP.get(scheme, None)
         if language and language in RecursiveCharacterTextSplitter.SEPARATORS_BY_LANGUAGE:
             return RecursiveCharacterTextSplitter.from_language(
                 language=language,
                 chunk_size=self.chunk_size,
                 chunk_overlap=self.chunk_overlap
             )
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/document.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/document.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Iterator, Type
 
-from beaker_bunsen.vectordb.loaders.base import BaseLoader
-from beaker_bunsen.vectordb.types import EmbeddingFunction
-from beaker_bunsen.vectordb.vector_store import VectorStore
+from beaker_bunsen.corpus.loaders.base import BaseLoader
+from beaker_bunsen.corpus.vector_stores.base_vector_store import VectorStore
 
-from ..types import Resource, Record
 from .base import BaseEmbedder
+from ..protocols import EmbeddingFunction
+from ..types import Record
+from ..resources import Resource
 from ..loaders.schemes import read_from_uri
 from ..util.helpers import count_words
 from ..util.splitters import TextSplitter, RecursiveCharacterTextSplitter
 
 
 class DocumentEmbedder(BaseEmbedder):
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/documentation.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/documentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Iterator
 
-from ..types import Resource, Record
+from ..resources import Resource
 from .base import BaseEmbedder
 from .document import DocumentEmbedder
 from ..loaders.schemes import read_from_uri
 from ..util.helpers import count_words
 from ..util.splitters import RecursiveCharacterTextSplitter
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/examples.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/embedders/examples.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import marko
 from marko.md_renderer import MarkdownRenderer
 from typing import Iterator
 
 import marko.md_renderer
 
-from beaker_bunsen.vectordb.types import Resource, Record
+from ..types import Record
+from ..resources import Resource
 
 from .base import BaseEmbedder
 
 
 class ExampleEmbedder(BaseEmbedder):
 
     def prepare_records_from_resource(self, resource: Resource) -> Iterator[Record]:
-        content = self.read_resource(resource)
+        content = resource.read()
         try:
             tree = marko.Parser().parse(content)
         except Exception as err:
             raise ValueError(
                 f"Example file at `{resource.uri}` does not seem to be valid Example markdown file."
             ) from err
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/base.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import uuid
 from abc import ABC, abstractmethod
 from typing import Optional
 
-from ..types import Resource, Default, DefaultType
+from ..types import Default, DefaultType
+from ..resources import Resource
 
 
 class BaseLoader(ABC):
 
     SLUG: str
     URI_SCHEME: str
 
@@ -31,14 +32,16 @@
 
     @abstractmethod
     def discover(
         self,
         locations: list[str] | DefaultType = Default,
         metadata: dict | DefaultType = Default,
         exclusions: list[str] | DefaultType = Default,
+        *args,
+        **kwargs,
     ):
         ...
 
     @abstractmethod
     def read(
         self,
         location: str,
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/code_library_loader.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/code_library_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 import requests
 import sys
 import tarfile
 import tempfile
 from collections import deque, defaultdict
 from pathlib import Path
 from typing import Any
-from urllib.parse import urlparse
 
 from .base import BaseLoader
 from .schemes import LocalFileScheme, PythonModuleScheme, RCranScheme, read_from_uri
-from ..types import Resource, Default, DefaultType
+from . import schemes
+from ..types import Default, DefaultType
+from ..resources import Resource, CodeResource, ExampleResource, DocumentationResource
 
 logger = logging.getLogger("beaker_bunsen")
 
 class BaseCodeLoader(BaseLoader):
 
     Scheme = LocalFileScheme
     # URI_SCHEME = "file"
@@ -71,15 +72,18 @@
         locations, parsed_exclusions = self.parse_locations(locations)
         exclusions.extend(parsed_exclusions)
 
         modules_to_collect = deque()
         for module_name in locations:
             module_spec = importlib.util.find_spec(module_name)
             if module_spec is None:
-                raise ValueError(f"Module '{module_name}' is not able to be imported. Please ensure that it is listed as a requirement and that 'require-runtime-dependencies' is enabled if error encountered during build.")
+                raise ValueError(
+                    f"Module '{module_name}' is not able to be imported. Please ensure that it is listed as a "
+                    f"requirement and that 'require-runtime-dependencies' is enabled if error encountered during build."
+                )
             modules_to_collect.append(module_spec)
 
         while modules_to_collect:
             module_spec = modules_to_collect.popleft()
 
             if not module_spec.origin.endswith('.py'):
                 logger.info(f"Skipping importing non-python file {module_spec.origin}")
@@ -106,18 +110,22 @@
             for sys_path in sys.path:
                 if origin_path.is_relative_to(sys_path):
                     basedir = sys_path
                     break
             else:
                 basedir = ""
 
-            resource = Resource(
+            resource = CodeResource(
                 uri=self.Scheme.get_uri_for_location(module_spec.name),
                 content=source,
-                metadata=metadata,
+                metadata={
+                    "package": module_spec.name,
+                    "type": "code",
+                    **metadata,
+                }
                 # basedir=basedir
             )
             resource.id = self.get_id_for_resource(resource)
             yield resource
 
 
 class RCRANLocalCache(contextlib.AbstractContextManager):
@@ -136,22 +144,23 @@
         self.context_locations = locations
         if not self.remote_package_cache:
             self.build_package_cache()
 
     def __enter__(self) -> dict[str, str]:
         results = {}
         for location in self.context_locations:
+            # Increase ref counter to reflect usage in new context
+            self.__class__.ref_counts[location] += 1
 
             # Return the cached if it exists
             existing_cache = self.local_package_cache.get(location, None)
             if existing_cache and os.path.isdir(existing_cache):
                 results[location] = existing_cache
                 continue
 
-            self.ref_counts[location] += 1
             if '@' in location:
                 package_name, version = location.split("@", maxsplit=1)
             else:
                 package = self.remote_package_cache.get(location, None)
                 if not package:
                     raise LookupError(f"Unable to find CRAN package name '{location}'")
                 package_name = package["package"]
@@ -169,27 +178,27 @@
             tar_file = tarfile.open(mode="r:gz", fileobj=tarball_req.raw)
             tar_file.extractall(path=tmpdir)
         return results
 
     def __exit__(self, exc_type, exc_value, traceback):
         # Update ref counts for local context
         for location in self.context_locations:
-            self.ref_counts[location] -= 1
+            self.__class__.ref_counts[location] -= 1
         # Clean up if there are no references
         locations_to_cleanup = [
             location
-            for location, ref_count in self.ref_counts.items()
+            for location, ref_count in self.__class__.ref_counts.items()
             if ref_count == 0
         ]
         for location in locations_to_cleanup:
             context_mgr = self.tempdir_context_holder[location]
             context_mgr.__exit__(exc_type, exc_value, traceback)
             del self.tempdir_context_holder[location]
             del self.local_package_cache[location]
-            del self.ref_counts[location]
+            del self.__class__.ref_counts[location]
         return super().__exit__(exc_type, exc_value, traceback)
 
     def build_package_cache(self):
         package_page = f"{self.repo}/PACKAGES"
         package_req = requests.get(package_page)
         package_content = package_req.text
         packages = {}
@@ -250,30 +259,44 @@
             exclusions = self.exclusions
 
         # Update or define locations and exclusions based on '!' prefix in location.
         locations, parsed_exclusions = self.parse_locations(locations)
         exclusions.extend(parsed_exclusions)
 
         with RCRANLocalCache(locations=locations) as cache:
-            for location, tempdir in cache.items():
+            for package_name, tempdir in cache.items():
                 for dirpath, _dirnames, filenames in os.walk(top=tempdir):
                     for filename in filenames:
                         if filename.startswith('.'):
                             continue
                         full_path = Path(os.path.join(dirpath, filename))
-                        # Only load in R library files, which are found in a suddirectory named `R` and have extension `.R`
-                        # Glob equivalent: `**/R/**.R`
-                        if not ("R" in full_path.parts and full_path.suffix == ".R"):
+                        if "R" in full_path.parts and full_path.suffix == ".R":
+                            resource_type = CodeResource
+                            location = str(full_path.relative_to(tempdir))
+                        elif "vignettes" in full_path.parts and full_path.suffix.startswith(".R"):
+                            resource_type = ExampleResource
+                            location = str(full_path.relative_to(tempdir))
+                        elif "man" in full_path.parts and full_path.suffix.startswith(".R"):
+                            resource_type = DocumentationResource
+                            location = str(full_path.relative_to(tempdir))
+                        else:
                             continue
 
-                        sub_path = full_path.relative_to(tempdir)
                         with open(full_path, 'r') as fh:
                             content = fh.read()
                             fh.seek(0)
-                            resource = Resource(
-                                uri=self.Scheme.get_uri_for_location(base=location, location=str(sub_path)),
+                            resource = resource_type(
+                                uri=self.Scheme.get_uri_for_location(
+                                    base=package_name,
+                                    location=location,
+                                ),
                                 file_handle=fh,
                                 content=content,
-                                metadata=metadata
+                                metadata={
+                                    "package": package_name,
+                                    "path": str(full_path),
+                                    "type": resource_type.resource_type.value,
+                                    **metadata,
+                                }
                             )
                             resource.id = self.get_id_for_resource(resource)
                             yield resource
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/local_file_loader.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/local_file_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,35 +2,39 @@
 import os
 from collections import deque
 from pathlib import Path
 from typing import Optional
 
 from .base import BaseLoader
 from .schemes import LocalFileScheme, read_from_uri
-from ..types import Resource, Default, DefaultType
+from ..types import Default, DefaultType
+from ..resources import Resource, ResourceType, get_resource_cls
 
 
 class LocalFileLoader(BaseLoader):
 
     Scheme = LocalFileScheme
     SLUG = "local"
 
     def __init__(
         self,
         locations: list[str] | None = None,
         metadata: dict | None = None,
         exclusions: list[str] | None = None,
+        resource_type: ResourceType = ResourceType.Generic,
     ):
         exclusions = exclusions or []
         if locations:
             locations, parsed_exclusions = self.parse_locations(locations)
             exclusions.extend(parsed_exclusions)
             self._check_locations_exist(locations)
+        self.resource_type = resource_type
         super().__init__(locations, metadata, exclusions)
 
+
     @staticmethod
     def _check_locations_exist(locations: list[str]):
         missing_locations = []
         for location in locations:
             if isinstance(location, Path):
                 location = str(location.absolute())
             if not os.path.exists(location):
@@ -46,15 +50,16 @@
                 collapsed_metadata.update(metadata)
         return collapsed_metadata
 
     def discover(
         self,
         locations: list[str] | DefaultType = Default,
         metadata: dict | DefaultType = Default,
-        exclusions: list[str] = Default,
+        exclusions: list[str] | DefaultType = Default,
+        resource_type: ResourceType | DefaultType = Default
     ):
         # Initialize exclusions first so we can extend it if there are any negated locations
         if exclusions is Default:
             exclusions = self.exclusions
 
         # Validate locations if they are passed in. If they are not, use location from initialization.
         if locations is not Default:
@@ -68,14 +73,17 @@
         if locations is None:
             raise ValueError("No locations specified to discover local files")
 
         if metadata is Default:
             metadata = {}
             metadata.update(self.metadata)
 
+        if resource_type is Default:
+            resource_type = self.resource_type
+
         locations_queue = deque((location, [metadata]) for location in locations)
         while locations_queue:
             location, location_metadata = locations_queue.popleft()
             if isinstance(location, Path):
                 location = str(location.absolute())
 
             if self.should_exclude(str(location)):
@@ -100,15 +108,16 @@
                 if os.path.isfile(metadata_filename):
                     with open(metadata_filename, 'r') as metadata_file:
                         dir_metadata = json.load(metadata_file)
                         location_metadata.append(dir_metadata)
 
                 metadata = self.collapse_metadata(location_metadata)
                 with open(location, 'r') as doc:
-                    resource = Resource(uri=self.Scheme.get_uri_for_location(location), file_handle=doc, metadata=metadata)
+                    resource_cls: type[Resource] = get_resource_cls(resource_type)
+                    resource = resource_cls(uri=self.Scheme.get_uri_for_location(location), file_handle=doc, metadata=metadata)
                     resource.id = self.get_id_for_resource(resource)
                     yield resource
 
     def read(self, location: str, base: str = ""):
         if location.startswith(self.Scheme.URI_SCHEME):
             uri = location
         else:
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/schemes.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/loaders/schemes.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import pkgutil
 import sys
 import zipfile
 from abc import ABC, abstractmethod
 from functools import cache
 from pathlib import Path
 from typing import Any, TYPE_CHECKING, Type
-from urllib.parse import urlparse
 
+from ..types import URI
 if TYPE_CHECKING:
-    from ...corpus import Corpus
+    from .. import Corpus
     from .base import BaseLoader
+    from ..embedders import BaseEmbedder
 
 
 def _is_scheme(obj: Any):
     return bool(
         inspect.isclass(obj)
         and issubclass(obj, Scheme)
         and callable(getattr(obj, "read", None))
@@ -28,22 +29,21 @@
     current_module = sys.modules[__name__]
     for _cls_name, cls in inspect.getmembers(current_module, predicate=_is_scheme):
         cls_uri_scheme = getattr(cls, "URI_SCHEME", None)
         if cls_uri_scheme is not None and cls_uri_scheme == scheme:
             return cls
 
 
-def determine_scheme(uri: str) -> "Scheme | None":
-    uri = os.fsdecode(uri)
-    scheme = urlparse(uri).scheme
-    scheme_cls = unmap_scheme(scheme)
+def determine_scheme(uri: URI | str | Path) -> "Scheme | None":
+    uri = URI(uri)
+    scheme_cls = unmap_scheme(uri.scheme)
     if scheme_cls:
             return scheme_cls
     else:
-        raise ValueError(f"Unable to Scheme for '{scheme}'")
+        raise ValueError(f"Unable to Scheme for '{uri.scheme}'")
 
 
 def read_from_uri(
     uri: str,
     *args,
     **kwargs,
 ) -> bytes:
@@ -56,14 +56,19 @@
 
     @classmethod
     def default_loader(cls) -> "Type[BaseLoader]":
         from .local_file_loader import LocalFileLoader
         return LocalFileLoader
 
     @classmethod
+    def default_embedder(cls) -> "Type[BaseEmbedder]":
+        from ..embedders import DocumentEmbedder
+        return DocumentEmbedder
+
+    @classmethod
     @abstractmethod
     def read(
         cls,
         uri: str,
         *args,
         **kwargs,
     ) -> bytes | str:
@@ -99,26 +104,26 @@
     @classmethod
     def join_parts(cls, *parts: list[str]) -> str:
         return os.path.join(*parts)
 
     @classmethod
     def read(
         cls,
-        uri: str,
+        uri: URI | str,
         base_dir: str | Path = "",
         *args,
         **kwargs,
     ) -> bytes | str:
-        parsed_uri = urlparse(uri)
-        if parsed_uri.scheme != cls.URI_SCHEME:
-            raise ValueError(f"Provided scheme '{parsed_uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
-        if not parsed_uri.path.startswith('/'):
-            path = os.path.join(base_dir, parsed_uri.path)
+        uri = URI(uri)
+        if uri.scheme != cls.URI_SCHEME:
+            raise ValueError(f"Provided scheme '{uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
+        if not uri.path.startswith('/'):
+            path = os.path.join(base_dir, uri.path)
         else:
-            path = parsed_uri.path
+            path = uri.path
         try:
             with open(path, 'r') as resource_file:
                 result = resource_file.read()
         except UnicodeDecodeError:
             with open(path, 'rb') as resource_file:
                 result = resource_file.read()
         return result
@@ -183,19 +188,19 @@
     @classmethod
     def read(
         cls,
         uri: str,
         *args,
         **kwargs,
     ) -> bytes | str:
-        parsed_uri = urlparse(uri)
-        if parsed_uri.scheme != cls.URI_SCHEME:
-            raise ValueError(f"Provided scheme '{parsed_uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
+        uri = URI(uri)
+        if uri.scheme != cls.URI_SCHEME:
+            raise ValueError(f"Provided scheme '{uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
 
-        mod_name = parsed_uri.path
+        mod_name = uri.path
         file_path = cls.get_module_path(mod_name)
 
         if file_path and os.path.isfile(file_path):
             with open(file_path, 'r') as resource_file:
                 result = resource_file.read()
             return result
 
@@ -246,19 +251,19 @@
     @classmethod
     def read(
         cls,
         uri: str,
         *args,
         **kwargs,
     ):
-        parsed_uri = urlparse(uri)
-        if parsed_uri.scheme != cls.URI_SCHEME:
-            raise ValueError(f"Provided scheme '{parsed_uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
-        zipfile_path = parsed_uri.path
-        inner_file = parsed_uri.fragment
+        uri = URI(uri)
+        if uri.scheme != cls.URI_SCHEME:
+            raise ValueError(f"Provided scheme '{uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
+        zipfile_path = uri.path
+        inner_file = uri.fragment
         with zipfile.ZipFile(zipfile_path) as zipfile_fh:
             with zipfile_fh.open(inner_file) as inner_file_fh:
                 content = inner_file_fh.read()
         try:
             return content.decode()
         except UnicodeDecodeError:
             return content
@@ -282,18 +287,18 @@
     def read(
         cls,
         uri: str,
         corpus: "Corpus",
         *args,
         **kwargs,
     ):
-        parsed_uri = urlparse(uri)
-        if parsed_uri.scheme != cls.URI_SCHEME:
-            raise ValueError(f"Provided scheme '{parsed_uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
-        return corpus.read_resource(parsed_uri.path)
+        uri = URI(uri)
+        if uri.scheme != cls.URI_SCHEME:
+            raise ValueError(f"Provided scheme '{uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
+        return corpus.read_resource(uri.path)
 
 
 class RCranScheme(Scheme):
     URI_SCHEME = "rcran-package"
 
     local_file_cache: dict[str, str] = {}
 
@@ -317,18 +322,18 @@
     def read(
         cls,
         uri: str,
         *args,
         **kwargs,
     ):
         from .code_library_loader import RCRANLocalCache
-        parsed_uri = urlparse(uri)
-        if parsed_uri.scheme != cls.URI_SCHEME:
-            raise ValueError(f"Provided scheme '{parsed_uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
+        uri = URI(uri)
+        if uri.scheme != cls.URI_SCHEME:
+            raise ValueError(f"Provided scheme '{uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
 
-        package = parsed_uri.fragment
-        subpath = parsed_uri.path
+        package = uri.fragment
+        subpath = uri.path
         with RCRANLocalCache([package]) as cache:
             target_file = Path(cache[package]) / subpath
             with target_file.open() as source:
                 content = source.read()
         return content
```

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/util/helpers.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/util/helpers.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/util/splitters.py` & `beaker_bunsen-0.0.6/src/beaker_bunsen/corpus/util/splitters.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     Iterable,
     List,
     Optional,
     TypeVar,
 )
 
 from .helpers import count_tokens
-from .. import logger
+# from .logging import logger
+logger = lambda *a: a
 
 
 def _split_text_with_regex(
     text: str, separator: str, keep_separator: bool
 ) -> List[str]:
     # Now that we have the separator, split the text
     if separator:
```

### Comparing `beaker_bunsen-0.0.5/tests/test_base_embedder.py` & `beaker_bunsen-0.0.6/tests/test_base_embedder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import pytest
 from pathlib import Path
 
-from beaker_bunsen.vectordb.types import Resource
-from beaker_bunsen.vectordb.chromadb_store import ChromaDBLocalStore
-from beaker_bunsen.vectordb.embedders.base import BaseEmbedder
-from beaker_bunsen.vectordb.loaders.local_file_loader import LocalFileLoader
-from beaker_bunsen.vectordb.embedders.documentation import DocumentationEmbedder
+from beaker_bunsen.corpus.resources import Resource
+from beaker_bunsen.corpus.vector_stores.chromadb_store import ChromaDBLocalStore
+from beaker_bunsen.corpus.embedders.base import BaseEmbedder
+from beaker_bunsen.corpus.loaders.local_file_loader import LocalFileLoader
+from beaker_bunsen.corpus.embedders.documentation import DocumentationEmbedder
 
 @pytest.fixture()
 def chromadb_store_path(tmp_path_factory):
     return str(tmp_path_factory.mktemp("test"))
 
 
 @pytest.fixture()
```

### Comparing `beaker_bunsen-0.0.5/tests/test_chromadb.py` & `beaker_bunsen-0.0.6/tests/test_chromadb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from pathlib import Path
 import pytest
-from beaker_bunsen.vectordb.chromadb_store import ChromaDBLocalStore, Record
+from beaker_bunsen.corpus.vector_stores.chromadb_store import ChromaDBLocalStore, Record
 
 @pytest.fixture()
 def chromadb_store(tmp_path_factory):
     store_path = str(tmp_path_factory.mktemp("test"))
     store = ChromaDBLocalStore(path=store_path, settings={'default_partition': "testing"})
     return store
```

### Comparing `beaker_bunsen-0.0.5/tests/test_code_loaders.py` & `beaker_bunsen-0.0.6/tests/test_code_loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pytest
 from packaging.version import Version
 from pathlib import Path
 from urllib.parse import urlparse
 
-from beaker_bunsen.vectordb.types import Resource
-from beaker_bunsen.vectordb.loaders.code_library_loader import PythonLibraryLoader, RCRANSourceLoader, RCRANLocalCache
+from beaker_bunsen.corpus.resources import Resource
+from beaker_bunsen.corpus.loaders.code_library_loader import PythonLibraryLoader, RCRANSourceLoader, RCRANLocalCache
 
 
 def test_python_module_discovery():
     python_loader = PythonLibraryLoader()
 
     os_records = list(python_loader.discover(locations=["os"]))
     requests_records = list(python_loader.discover(locations=["requests"]))
```

### Comparing `beaker_bunsen-0.0.5/tests/test_corpus.py` & `beaker_bunsen-0.0.6/tests/test_corpus.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import pytest
 import zipfile
 from pathlib import Path
 
-from beaker_bunsen.vectordb.types import Resource
-from beaker_bunsen.vectordb.chromadb_store import BaseChromaDBStore, ZippedChromaDBStore
-from beaker_bunsen.vectordb.embedders import BaseEmbedder, DocumentationEmbedder, ExampleEmbedder, CodeEmbedder
-from beaker_bunsen.vectordb.loaders import LocalFileLoader, PythonLibraryLoader
-from beaker_bunsen.vectordb.loaders.schemes import read_from_uri
-from beaker_bunsen.corpus import Corpus
+from beaker_bunsen.corpus.resources import Resource
+from beaker_bunsen.corpus.vector_stores.chromadb_store import BaseChromaDBStore, ZippedChromaDBStore
+from beaker_bunsen.corpus.embedders import BaseEmbedder, DocumentationEmbedder, ExampleEmbedder, CodeEmbedder
+from beaker_bunsen.corpus.loaders import LocalFileLoader, PythonLibraryLoader
+from beaker_bunsen.corpus.loaders.schemes import read_from_uri
+from beaker_bunsen.corpus.corpus import Corpus
 
 def get_all_records_by_partition(store: BaseChromaDBStore):
     return sorted(
         ((partition, sorted(store.get_all(partition=partition), key=lambda p:p.id))
         for partition in store.get_partitions())
     )
```

### Comparing `beaker_bunsen-0.0.5/tests/test_documentation_embedder.py` & `beaker_bunsen-0.0.6/tests/test_documentation_embedder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pytest
 from pathlib import Path
 
-from beaker_bunsen.vectordb.types import Resource
-from beaker_bunsen.vectordb.chromadb_store import ChromaDBLocalStore
-from beaker_bunsen.vectordb.loaders.local_file_loader import LocalFileLoader
-from beaker_bunsen.vectordb.embedders.documentation import DocumentationEmbedder
+from beaker_bunsen.corpus.resources import Resource
+from beaker_bunsen.corpus.vector_stores.chromadb_store import ChromaDBLocalStore
+from beaker_bunsen.corpus.loaders.local_file_loader import LocalFileLoader
+from beaker_bunsen.corpus.embedders.documentation import DocumentationEmbedder
 
 
 @pytest.fixture()
 def chromadb_store_path(tmp_path_factory):
     return str(tmp_path_factory.mktemp("test"))
 
 @pytest.fixture()
@@ -37,15 +37,16 @@
     embedder.ingest()
 
     ingested_records = sorted(store.get_all(), key=lambda record: record.id)
     first_record, second_record = ingested_records[:2]
     record_ids = sorted(record.id for record in ingested_records)
 
     assert len(ingested_records) > 1
-    assert first_record.content[-20:] in second_record.content[:400]  # Assert overlap feature is working
+    # Due to change in chunking, overlap is no longer assured.
+    # assert first_record.content[-20:] in second_record.content[:400]  # Assert overlap feature is working
     assert first_record.uri == f"file:{filename}"
     with open(filename) as rawfile:
         raw_data = rawfile.read()
         for record in ingested_records:
             assert record.content in raw_data
         assert raw_data.startswith(first_record.content)
     assert record_ids[0].endswith(f"{filename}:1")
```

### Comparing `beaker_bunsen-0.0.5/tests/test_example_embedder.py` & `beaker_bunsen-0.0.6/tests/test_example_embedder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import pytest
 from pathlib import Path
 
-from beaker_bunsen.vectordb.types import Resource
-from beaker_bunsen.vectordb.chromadb_store import ChromaDBLocalStore
-from beaker_bunsen.vectordb.embedders.base import BaseEmbedder
-from beaker_bunsen.vectordb.loaders.local_file_loader import LocalFileLoader
-from beaker_bunsen.vectordb.embedders.examples import ExampleEmbedder
+from beaker_bunsen.corpus.resources import Resource
+from beaker_bunsen.corpus.vector_stores.chromadb_store import ChromaDBLocalStore
+from beaker_bunsen.corpus.loaders.local_file_loader import LocalFileLoader
+from beaker_bunsen.corpus.embedders.examples import ExampleEmbedder
 
 @pytest.fixture()
 def chromadb_store_path(tmp_path_factory):
     return str(tmp_path_factory.mktemp("test"))
 
 
 @pytest.fixture()
```

### Comparing `beaker_bunsen-0.0.5/tests/test_local_file_loader.py` & `beaker_bunsen-0.0.6/tests/test_local_file_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import pytest
 from pathlib import Path
 
-from beaker_bunsen.vectordb.types import Resource
-from beaker_bunsen.vectordb.loaders.local_file_loader import LocalFileLoader
-from beaker_bunsen.vectordb.loaders.schemes import LocalFileScheme
+from beaker_bunsen.corpus.resources import Resource
+from beaker_bunsen.corpus.loaders.local_file_loader import LocalFileLoader
+from beaker_bunsen.corpus.loaders.schemes import LocalFileScheme
 
 
 @pytest.fixture()
 def test_data_path():
     return Path(__file__).parent / "data"
```

### Comparing `beaker_bunsen-0.0.5/tests/test_schemes.py` & `beaker_bunsen-0.0.6/tests/test_schemes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import pytest
 import zipfile
 from pathlib import Path
 
-from beaker_bunsen.vectordb.loaders.schemes import (
+from beaker_bunsen.corpus.loaders.schemes import (
     read_from_uri,
     LocalFileScheme, PythonModuleScheme, ZipfileScheme, CorpusResourceScheme,
 )
-from beaker_bunsen.corpus import Corpus
+from beaker_bunsen.corpus.corpus import Corpus
 
 
 @pytest.fixture()
 def test_data_path():
     return Path(__file__).parent / "data"
 
 
@@ -99,14 +99,17 @@
 
 
 def test_load_resource_from_corpus_dir(test_data_path):
     corpus_path = test_data_path / "corpuses" / "test-corpus"
     resource_from_corpus = Path("code/requests.adapters")
 
     corpus_uri = CorpusResourceScheme.get_uri_for_location(location=str(resource_from_corpus))
+    print(corpus_uri)
+    print(corpus_path)
+    print(resource_from_corpus)
     corpus = Corpus.from_dir(corpus_path)
 
     innercontent = read_from_uri(corpus_uri, corpus=corpus)
     with open(corpus_path / "resources" / resource_from_corpus) as resource_file:
         rawcontent = resource_file.read()
 
     # Assert that this call fails when a corpus is not provided
```

### Comparing `beaker_bunsen-0.0.5/tests/test_utils.py` & `beaker_bunsen-0.0.6/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from beaker_bunsen.vectordb.util.helpers import count_words, extract_md_codeblocks, extract_json, common_path_portion
+from beaker_bunsen.corpus.util.helpers import count_words, extract_md_codeblocks, extract_json, common_path_portion
 
 
 def test_word_count():
     count5 = "This sentence has five words."
     count7 = """
 This
 block
```

### Comparing `beaker_bunsen-0.0.5/tests/test_zipped_chromadb.py` & `beaker_bunsen-0.0.6/tests/test_zipped_chromadb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import pytest
 import shutil
 from pathlib import Path
 from zipfile import ZipFile
 
-from beaker_bunsen.vectordb.chromadb_store import ChromaDBLocalStore, Record, ZippedChromaDBStore
+from beaker_bunsen.corpus.vector_stores.chromadb_store import ChromaDBLocalStore, Record, ZippedChromaDBStore
 
 @pytest.fixture()
 def chromadb_store(test_temp_path):
     store_path = str(Path(test_temp_path) / "store")
     store = ChromaDBLocalStore(path=store_path, settings={'default_partition': "testing"})
     return store
```

### Comparing `beaker_bunsen-0.0.5/tests/data/store.zip` & `beaker_bunsen-0.0.6/tests/data/store.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/corpus.zip` & `beaker_bunsen-0.0.6/tests/data/corpuses/corpus.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/store.zip` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/store.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.adapters` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.adapters`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.api` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.api`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.auth` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.auth`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.compat` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.compat`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.cookies` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.cookies`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.exceptions` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.exceptions`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.help` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.help`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.hooks` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.hooks`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.models` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.models`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.packages` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.packages`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.sessions` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.sessions`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.status_codes` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.status_codes`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.structures` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.structures`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.utils` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/code/requests.utils`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md` & `beaker_bunsen-0.0.6/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.6/tests/data/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/documentation/ruff_readme.md` & `beaker_bunsen-0.0.6/tests/data/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/documents/Lunar_Sample_Laboratory_Facility.html` & `beaker_bunsen-0.0.6/tests/data/documents/Lunar_Sample_Laboratory_Facility.html`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/documents/yorkshire.txt` & `beaker_bunsen-0.0.6/tests/data/documents/yorkshire.txt`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/documents/recipes/irish_potato_caserole` & `beaker_bunsen-0.0.6/tests/data/documents/recipes/irish_potato_caserole`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/documents/recipes/tajine_maadnous` & `beaker_bunsen-0.0.6/tests/data/documents/recipes/tajine_maadnous`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/documents/recipes/winter_risotto` & `beaker_bunsen-0.0.6/tests/data/documents/recipes/winter_risotto`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/images/kitten-sad.jpg` & `beaker_bunsen-0.0.6/tests/data/images/kitten-sad.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/images/kitten_hacker.jpg` & `beaker_bunsen-0.0.6/tests/data/images/kitten_hacker.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/images/puppy_hacker.jpg` & `beaker_bunsen-0.0.6/tests/data/images/puppy_hacker.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/images/puppy_sad.png` & `beaker_bunsen-0.0.6/tests/data/images/puppy_sad.png`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/subproject/pyproject.toml` & `beaker_bunsen-0.0.6/tests/data/subproject/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/subproject/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.6/tests/data/subproject/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/tests/data/subproject/documentation/ruff_readme.md` & `beaker_bunsen-0.0.6/tests/data/subproject/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/.gitignore` & `beaker_bunsen-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/LICENSE.txt` & `beaker_bunsen-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/README.md` & `beaker_bunsen-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.5/pyproject.toml` & `beaker_bunsen-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   "archytas~=1.1.6",
   "chromadb~=0.4.22",
   "tenacity~=8.2.3",
   "tiktoken~=0.5.2",
   "marko~=2.0.3",
   "hatchling",
   "click~=8.1.7",
+  "beautifulsoup4",  # Whichever vrsion is installed by jupyter via beaker-kernel
 ]
 
 [project.scripts]
 bunsen= "beaker_bunsen.scripts.bunsen:cli"
 
 [project.entry-points.hatch]
 bunsen = "beaker_bunsen.builder.hooks"
```

### Comparing `beaker_bunsen-0.0.5/PKG-INFO` & `beaker_bunsen-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: beaker-bunsen
-Version: 0.0.5
+Version: 0.0.6
 Summary: Quickly generate new Beaker contexts for new domains and libraries.
 Project-URL: Documentation, https://github.com/unknown/beaker-bunsen#readme
 Project-URL: Issues, https://github.com/unknown/beaker-bunsen/issues
 Project-URL: Source, https://github.com/unknown/beaker-bunsen
 Author-email: Matthew Printz <matt@jataware.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: archytas~=1.1.6
 Requires-Dist: beaker-kernel~=1.5.1
+Requires-Dist: beautifulsoup4
 Requires-Dist: chromadb~=0.4.22
 Requires-Dist: click~=8.1.7
 Requires-Dist: hatchling
 Requires-Dist: marko~=2.0.3
 Requires-Dist: tenacity~=8.2.3
 Requires-Dist: tiktoken~=0.5.2
 Description-Content-Type: text/markdown
```

