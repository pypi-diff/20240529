# Comparing `tmp/sparv_sbx_sentence_sentiment_kb_sent-0.1.0.tar.gz` & `tmp/sparv_sbx_sentence_sentiment_kb_sent-0.1.1.tar.gz`

## Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0.tar` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/.bumpversion.toml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/Makefile
--rw-r--r--   0        0        0   161889 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/pdm.lock
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/src/sbx_sentence_sentiment_kb_sent/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/src/sbx_sentence_sentiment_kb_sent/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/src/sbx_sentence_sentiment_kb_sent/py.typed
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/src/sbx_sentence_sentiment_kb_sent/sentiment_analyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0    79250 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/requirements-testing.lock
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/test_annotations.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/test_sentiment_analyzer.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/testing.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/__snapshots__/test_annotations.ambr
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/.gitignore
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/README.md
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/.bumpversion.toml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/Makefile
+-rw-r--r--   0        0        0   161889 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/pdm.lock
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/src/sbx_sentence_sentiment_kb_sent/__init__.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/src/sbx_sentence_sentiment_kb_sent/annotations.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/src/sbx_sentence_sentiment_kb_sent/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/src/sbx_sentence_sentiment_kb_sent/py.typed
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/src/sbx_sentence_sentiment_kb_sent/sentiment_analyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    79250 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/requirements-testing.lock
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/test_annotations.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/test_sentiment_analyzer.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/testing.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/__snapshots__/test_annotations.ambr
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/.gitignore
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/README.md
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 sparv_sbx_sentence_sentiment_kb_sent-0.1.1/PKG-INFO
```

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/.bumpversion.toml` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/.bumpversion.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.bumpversion]
-current_version = "0.1.0"
+current_version = "0.1.1"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 tag = true
 sign_tags = true
 tag_name = "sentence-sentiment-kb-sent-v{new_version}"
 tag_message = "bump version(sentence-sentiment-kb-sent): {current_version} → {new_version}"
 allow_dirty = false
```

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/Makefile` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/pdm.lock` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/pdm.lock`

 * *Files identical despite different names*

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/src/sbx_sentence_sentiment_kb_sent/annotations.py` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/src/sbx_sentence_sentiment_kb_sent/annotations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-"""Sparv annotator."""
+"""Sparv annotator for sentiment analysis on sentences."""
 
 from sparv import api as sparv_api  # type: ignore [import-untyped]
 
+from sbx_sentence_sentiment_kb_sent.constants import PROJECT_NAME
 from sbx_sentence_sentiment_kb_sent.sentiment_analyzer import SentimentAnalyzer
 
 logger = sparv_api.get_logger(__name__)
 
 
 @sparv_api.annotator("Sentiment analysis of sentences", language=["swe"])
 def annotate_sentence_sentiment(
     out_sentence_sentiment: sparv_api.Output = sparv_api.Output(
-        "<sentence>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-sent",
+        f"<sentence>:{PROJECT_NAME}.sentence-sentiment--kb-sent",
         # cls="sbx_sentence_sentiment_kb_sent",
         description="Sentiment analysis of sentence with KBLab/robust-swedish-sentiment-multiclass",  # noqa: E501
     ),
     word: sparv_api.Annotation = sparv_api.Annotation("<token:word>"),
     sentence: sparv_api.Annotation = sparv_api.Annotation("<sentence>"),
-    num_decimals_str: str = sparv_api.Config("sbx_sentence_sentiment_kb_sent.num_decimals"),
+    num_decimals_str: str = sparv_api.Config(f"{PROJECT_NAME}.num_decimals"),
 ) -> None:
     """Sentiment analysis of sentence with KBLab/robust-swedish-sentiment-multiclass."""
     try:
         num_decimals = int(num_decimals_str)
     except ValueError as exc:
         raise sparv_api.SparvErrorMessage(
-            f"'sbx_word_prediction_kb_bert.num_decimals' must contain an 'int' got: '{num_decimals_str}'"  # noqa: E501
+            f"'{PROJECT_NAME}.num_decimals' must contain an 'int' got: '{num_decimals_str}'"
         ) from exc
     sentences, _orphans = sentence.get_children(word)
     token_word = list(word.read())
     out_sentence_sentiment_annotation = sentence.create_empty_attribute()
 
     analyzer = SentimentAnalyzer(num_decimals=num_decimals)
```

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/src/sbx_sentence_sentiment_kb_sent/sentiment_analyzer.py` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/src/sbx_sentence_sentiment_kb_sent/sentiment_analyzer.py`

 * *Files identical despite different names*

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/requirements-testing.lock` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/requirements-testing.lock`

 * *Files identical despite different names*

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/test_annotations.py` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/test_sentiment_analyzer.py` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/test_sentiment_analyzer.py`

 * *Files identical despite different names*

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/tests/testing.py` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/tests/testing.py`

 * *Files identical despite different names*

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/.gitignore` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/README.md` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/sparv-sbx-sentence-sentiment-kb-sent)](https://pypi.org/project/sparv-sbx-sentence-sentiment-kb-sent/)
 
 [![Maturity badge - level 2](https://img.shields.io/badge/Maturity-Level%202%20--%20First%20Release-yellowgreen.svg)](https://github.com/spraakbanken/getting-started/blob/main/scorecard.md)
 [![Stage](https://img.shields.io/pypi/status/sparv-sbx-sentence-sentiment-kb-sent)](https://pypi.org/project/sparv-sbx-sentence-sentiment-kb-sent/)
 
 [![CI(release)](https://github.com/spraakbanken/sparv-sbx-sentiment-analysis/actions/workflows/release-sentence-sentiment-kb-sent.yml/badge.svg)](https://github.com/spraakbanken/sparv-sbx-sentiment-analysis/actions/workflows/release-sentence-sentiment-kb-sent.yml)
 
-Plugin for applying bert masking as a [Sparv](https://github.com/spraakbanken/sparv-pipeline) annotation.
+Plugin for computing sentence sentiment as a [Sparv](https://github.com/spraakbanken/sparv-pipeline) annotation.
 
 ## Install
 
 First, install Sparv as suggested:
 
 ```bash
 pipx install sparv-pipeline
@@ -29,29 +29,29 @@
 
 Depending on how many explicit exports of annotations you have you can decide to use this
 annotation exclusively by adding it as the only annotation to export under `xml_export`:
 
 ```yaml
 xml_export:
     annotations:
-        - <token>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-bert
+        - <sentence>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-sent
 ```
 
 To use it together with other annotations you might add it under `export`:
 
 ```yaml
 export:
     annotations:
-        - <token>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-bert
+        - <sentence>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-sent
         ...
 ```
 
 ### Configuration
 
-You can configure this plugin by the number of neighbours to generate.
+You can configure this plugin in the following way.
 
 #### Number of Decimals
 
 The number of decimals defaults to `3` but can be configured in `config.yaml`:
 
 ```yaml
 sbx_sentence_sentiment_kb_sent:
```

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/pyproject.toml` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "sparv-sbx-sentence-sentiment-kb-sent"
-version = "0.1.0"
-description = "A sparv plugin for computing word neighbours using a BERT model."
+version = "0.1.1"
+description = "A sparv plugin for computing sentence sentiment."
 authors = [
     { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 dependencies = ["sparv-pipeline >=5.2.0", "transformers>=4.34.1"]
 license = "MIT"
 readme = "README.md"
@@ -51,11 +51,8 @@
 packages = ["src/sbx_sentence_sentiment_kb_sent"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 
 [tool.pdm.dev-dependencies]
-dev = [
-    "pytest>=8.0.0",
-    "syrupy>=4.6.1",
-]
+dev = ["pytest>=8.0.0", "syrupy>=4.6.1"]
```

### Comparing `sparv_sbx_sentence_sentiment_kb_sent-0.1.0/PKG-INFO` & `sparv_sbx_sentence_sentiment_kb_sent-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: sparv-sbx-sentence-sentiment-kb-sent
-Version: 0.1.0
-Summary: A sparv plugin for computing word neighbours using a BERT model.
+Version: 0.1.1
+Summary: A sparv plugin for computing sentence sentiment.
 Project-URL: Homepage, https://spraakbanken.gu.se
 Project-URL: Repository, https://github.com/spraakbanken/sparv-sbx-sentence-sentiment-analysis
 Project-URL: Bug Tracker, https://github.com/spraakbanken/sparv-sbx-sentence-sentiment-analysis/labels/project%3Asentence-sentiment--kb-sent
 Author-email: Språkbanken Text <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License-Expression: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/sparv-sbx-sentence-sentiment-kb-sent)](https://pypi.org/project/sparv-sbx-sentence-sentiment-kb-sent/)
 
 [![Maturity badge - level 2](https://img.shields.io/badge/Maturity-Level%202%20--%20First%20Release-yellowgreen.svg)](https://github.com/spraakbanken/getting-started/blob/main/scorecard.md)
 [![Stage](https://img.shields.io/pypi/status/sparv-sbx-sentence-sentiment-kb-sent)](https://pypi.org/project/sparv-sbx-sentence-sentiment-kb-sent/)
 
 [![CI(release)](https://github.com/spraakbanken/sparv-sbx-sentiment-analysis/actions/workflows/release-sentence-sentiment-kb-sent.yml/badge.svg)](https://github.com/spraakbanken/sparv-sbx-sentiment-analysis/actions/workflows/release-sentence-sentiment-kb-sent.yml)
 
-Plugin for applying bert masking as a [Sparv](https://github.com/spraakbanken/sparv-pipeline) annotation.
+Plugin for computing sentence sentiment as a [Sparv](https://github.com/spraakbanken/sparv-pipeline) annotation.
 
 ## Install
 
 First, install Sparv as suggested:
 
 ```bash
 pipx install sparv-pipeline
@@ -54,29 +54,29 @@
 
 Depending on how many explicit exports of annotations you have you can decide to use this
 annotation exclusively by adding it as the only annotation to export under `xml_export`:
 
 ```yaml
 xml_export:
     annotations:
-        - <token>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-bert
+        - <sentence>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-sent
 ```
 
 To use it together with other annotations you might add it under `export`:
 
 ```yaml
 export:
     annotations:
-        - <token>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-bert
+        - <sentence>:sbx_sentence_sentiment_kb_sent.sentence-sentiment--kb-sent
         ...
 ```
 
 ### Configuration
 
-You can configure this plugin by the number of neighbours to generate.
+You can configure this plugin in the following way.
 
 #### Number of Decimals
 
 The number of decimals defaults to `3` but can be configured in `config.yaml`:
 
 ```yaml
 sbx_sentence_sentiment_kb_sent:
```

