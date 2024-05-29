# Comparing `tmp/cpr_sdk-1.1.2.tar.gz` & `tmp/cpr_sdk-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpr_sdk-1.1.2.tar", max compression
+gzip compressed data, was "cpr_sdk-1.1.4.tar", max compression
```

## Comparing `cpr_sdk-1.1.2.tar` & `cpr_sdk-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1507 2024-04-25 10:37:27.273597 cpr_sdk-1.1.2/LICENSE
--rw-r--r--   0        0        0     6615 2024-04-25 10:37:27.273597 cpr_sdk-1.1.2/README.md
--rw-r--r--   0        0        0     2926 2024-04-25 10:38:35.301835 cpr_sdk-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       52 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/__init__.py
--rw-r--r--   0        0        0     5693 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/data_adaptors.py
--rw-r--r--   0        0        0     1118 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/embedding.py
--rw-r--r--   0        0        0      797 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/exceptions.py
--rw-r--r--   0        0        0    50630 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/models/__init__.py
--rw-r--r--   0        0        0    11979 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/models/search.py
--rw-r--r--   0        0        0    14816 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/parser_models.py
--rw-r--r--   0        0        0     2679 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/pipeline_general_models.py
--rw-r--r--   0        0        0    71013 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/resources/sensitive_query_terms.tsv
--rw-r--r--   0        0        0     2791 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/s3.py
--rw-r--r--   0        0        0     4584 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/search_adaptors.py
--rw-r--r--   0        0        0     4143 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/utils.py
--rw-r--r--   0        0        0      169 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/version.py
--rw-r--r--   0        0        0     6979 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/vespa.py
--rw-r--r--   0        0        0     7015 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/yql_builder.py
--rw-r--r--   0        0        0     7999 1970-01-01 00:00:00.000000 cpr_sdk-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/LICENSE
+-rw-r--r--   0        0        0     6865 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/README.md
+-rw-r--r--   0        0        0     2950 2024-05-29 13:53:31.660350 cpr_sdk-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/__init__.py
+-rw-r--r--   0        0        0     5693 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/data_adaptors.py
+-rw-r--r--   0        0        0     1118 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/embedding.py
+-rw-r--r--   0        0        0      797 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/exceptions.py
+-rw-r--r--   0        0        0    56174 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/models/__init__.py
+-rw-r--r--   0        0        0    11979 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/models/search.py
+-rw-r--r--   0        0        0    16341 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/parser_models.py
+-rw-r--r--   0        0        0     2679 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/pipeline_general_models.py
+-rw-r--r--   0        0        0    71013 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/resources/sensitive_query_terms.tsv
+-rw-r--r--   0        0        0     2791 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/s3.py
+-rw-r--r--   0        0        0     4584 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/search_adaptors.py
+-rw-r--r--   0        0        0     4143 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/utils.py
+-rw-r--r--   0        0        0      169 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/version.py
+-rw-r--r--   0        0        0     6979 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/vespa.py
+-rw-r--r--   0        0        0     7015 2024-05-29 13:52:24.799940 cpr_sdk-1.1.4/src/cpr_sdk/yql_builder.py
+-rw-r--r--   0        0        0     8294 1970-01-01 00:00:00.000000 cpr_sdk-1.1.4/PKG-INFO
```

### Comparing `cpr_sdk-1.1.2/LICENSE` & `cpr_sdk-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/README.md` & `cpr_sdk-1.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,25 @@
 dataset = Dataset(GSTDocument).from_huggingface(
     version="d8363af072d7e0f87ec281dd5084fb3d3f4583a9", # commit hash, optional
     limit=1000,
     token="my-huggingface-token", # required for private repos if not in env
 )
 ```
 
+The following flag is used for the passage level and flat dataset.
+
+```py
+dataset = Dataset(
+    document_model=BaseDocument
+).from_huggingface(
+    dataset_name="ClimatePolicyRadar/passage-level-flat-dataset",
+    passage_level_and_flat=True
+)
+```
+
 ### Loading from local storage or s3
 
 ```py
 # document_id is also the filename stem
 
 document = BaseDocument.load_from_local(folder_path="path/to/data/", document_id="document_1234")
```

### Comparing `cpr_sdk-1.1.2/pyproject.toml` & `cpr_sdk-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cpr_sdk"
 # This version is a placeholder that is overwritten during release.
 # The placeholder is replaced by the value from the cpr_sdk package itself.
-version = "1.1.2"
+version = "1.1.4"
 description = ""
 authors = ["CPR Tech <tech@climatepolicyradar.org>"]
 readme = "README.md"
 packages = [{ include = "cpr_sdk", from = "src" }]
 classifiers = [
   "Intended Audience :: Science/Research",
   "Programming Language :: Python :: 3",
@@ -28,25 +28,26 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.4.0"
 boto3 = "^1.26.16"
 tqdm = "^4.64.1"
 aws-error-utils = "^2.7.0"
 pandas = "^1.5.3"
-datasets = "^2.14.0"
+datasets = "^2.19.0"
 langdetect = "^1.0.9"
 deprecation = "^2.1.0"
 numpy = ">=1.23.5"
 
 pyvespa = { version = "^0.37.1", optional = true }
 pyyaml = { version = "^6.0.1", optional = true }
 sentence-transformers = { version = "^2.2.2", optional = true }
 torch = { version = "^2.0.0", optional = true }
 spacy = { version = "^3.5.1", optional = true }
 poetry = "^1.8.2"
+flatten-dict = "^0.4.2"
 
 [tool.poetry.extras]
 vespa = ["pyvespa", "pyyaml", "sentence-transformers", "torch"]
 spacy = ["spacy"]
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/data_adaptors.py` & `cpr_sdk-1.1.4/src/cpr_sdk/data_adaptors.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/embedding.py` & `cpr_sdk-1.1.4/src/cpr_sdk/embedding.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/exceptions.py` & `cpr_sdk-1.1.4/src/cpr_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/models/__init__.py` & `cpr_sdk-1.1.4/src/cpr_sdk/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,157 @@
 """Data models for data access."""
 
+import datetime
+import hashlib
 import itertools
+import logging
+import os
+import random
+from functools import cached_property
+from pathlib import Path
 from typing import (
+    Annotated,
+    Any,
+    Dict,
     Iterable,
-    Sequence,
-    Optional,
     List,
-    Dict,
+    Literal,
+    Optional,
+    Sequence,
     Tuple,
-    Any,
-    Union,
     TypeVar,
-    Literal,
-    Annotated,
+    Union,
 )
-from pathlib import Path
-import datetime
-import hashlib
-import logging
-from functools import cached_property
-import os
 
+import cpr_sdk.data_adaptors as adaptors
+import numpy as np
 import pandas as pd
+from cpr_sdk.parser_models import (
+    PDF_PAGE_METADATA_KEY,
+    BackendDocument,
+    BaseParserOutput,
+    BlockType,
+    HTMLData,
+    HTMLTextBlock,
+    ParserOutput,
+    PDFData,
+    PDFPageMetadata,
+    PDFTextBlock,
+)
+from cpr_sdk.pipeline_general_models import (
+    CONTENT_TYPE_HTML,
+    CONTENT_TYPE_PDF,
+    Json,
+)
+from datasets import Dataset as HFDataset
+from datasets import DatasetInfo, load_dataset
+from flatten_dict import unflatten as unflatten_dict
 from pydantic import (
     AnyHttpUrl,
     BaseModel,
+    ConfigDict,
     Field,
-    StringConstraints,
     NonNegativeInt,
     PrivateAttr,
+    StringConstraints,
     model_validator,
-    ConfigDict,
 )
 from tqdm.auto import tqdm
-import numpy as np
-import random
-
-from datasets import Dataset as HFDataset, DatasetInfo, load_dataset
-import cpr_sdk.data_adaptors as adaptors
-from cpr_sdk.parser_models import BlockType, BaseParserOutput
-from cpr_sdk.pipeline_general_models import (
-    CONTENT_TYPE_HTML,
-    CONTENT_TYPE_PDF,
-    Json,
-)
 
 LOGGER = logging.getLogger(__name__)
 
 AnyDocument = TypeVar("AnyDocument", bound="BaseDocument")
 
 
+def passage_level_df_to_document_model(
+    df: pd.DataFrame, document_model: type[AnyDocument]
+) -> AnyDocument:
+    """
+    A function to group the passage level data and convert to a document model.
+
+    The document model must be of a type that is either a BaseDocument or inherist from
+    that type. To create this we create an intermediate model called ParserOutput before
+    using the from_parser_output method on the BaseDocument class.
+    """
+    pdf_data = None
+    html_data = None
+
+    if df["document_content_type"].iloc[0] == CONTENT_TYPE_PDF:
+        page_metadata = []
+        md5sum = df["document_md5_sum"].iloc[0]
+        text_blocks = []
+
+        for _, row in df.iterrows():
+            text_block_page_metadata = PDFPageMetadata(
+                page_number=row[PDF_PAGE_METADATA_KEY]["page_number"],
+                dimensions=row[PDF_PAGE_METADATA_KEY]["dimensions"],
+            )
+            if text_block_page_metadata not in page_metadata:
+                page_metadata.append(text_block_page_metadata)
+
+            text_blocks.append(
+                PDFTextBlock(
+                    text=[row["text"]],
+                    text_block_id=row["text_block_id"],
+                    language=row["language"],
+                    type=row["type"],
+                    type_confidence=row["type_confidence"],
+                    page_number=row["page_number"],
+                    coords=row["coords"],
+                )
+            )
+
+        pdf_data = PDFData(
+            page_metadata=page_metadata,
+            text_blocks=text_blocks,
+            md5sum=md5sum,
+        )
+
+    elif df["document_content_type"].iloc[0] == CONTENT_TYPE_HTML:
+        text_blocks = []
+        for _, row in df.iterrows():
+            text_blocks.append(
+                HTMLTextBlock(
+                    text=[row["text"]],
+                    text_block_id=row["text_block_id"],
+                    language=row["language"],
+                    type=row["type"],
+                    type_confidence=row["type_confidence"],
+                )
+            )
+
+        html_data = HTMLData(
+            detected_title=df["html_data"].iloc[0]["detected_title"],
+            detected_date=df["html_data"].iloc[0]["detected_date"],
+            has_valid_text=df["html_data"].iloc[0]["has_valid_text"],
+            text_blocks=text_blocks,
+        )
+    else:
+        raise ValueError("The content type is not supported")
+
+    document_dict = df.iloc[0].to_dict()
+
+    document_dict["pdf_data"] = pdf_data.model_dump() if pdf_data else None
+    document_dict["html_data"] = html_data.model_dump() if html_data else None
+    document_dict["languages"] = document_dict["languages"].tolist()
+    document_dict["document_metadata"]["languages"] = document_dict[
+        "document_metadata"
+    ]["languages"].tolist()
+    document_dict["document_metadata"] = (
+        document_dict["document_metadata"] if document_dict["document_metadata"] else {}
+    )
+    document_dict["pipeline_metadata"] = (
+        document_dict["pipeline_metadata"] if document_dict["pipeline_metadata"] else {}
+    )
+
+    parser_output = ParserOutput.model_validate(document_dict)
+
+    return document_model.from_parser_output(parser_output)
+
+
 def _load_and_validate_metadata_csv(
     metadata_csv_path: Path, target_model: type[AnyDocument]
 ) -> pd.DataFrame:
     """
     Load a metadata CSV
 
     Raise a ValueError if it does not exist or doesn't have the expected columns.
@@ -393,15 +491,15 @@
     has_valid_text: bool
     text_blocks: Optional[
         Sequence[TextBlock]
     ] = None  # None if there is no content type
     page_metadata: Optional[
         Sequence[PageMetadata]
     ] = None  # Properties such as page numbers and dimensions for paged documents
-    document_metadata: BaseMetadata
+    document_metadata: Union[BaseMetadata, BackendDocument]
     # The current fields are set in the document parser:
     # https://github.com/climatepolicyradar/navigator-document-parser/blob/5a2872389a85e9f81cdde148b388383d7490807e/cli/parse_pdfs.py#L435
     # These are azure_api_version, azure_model_id and parsing_date
     pipeline_metadata: Json = {}
 
     @classmethod
     def from_parser_output(
@@ -1271,14 +1369,60 @@
             "languages": "document_languages",
         }
 
         huggingface_dataset = huggingface_dataset.rename_columns(rename_map)
 
         return huggingface_dataset
 
+    def _from_huggingface_passage_level_flat_parquet(
+        self,
+        huggingface_dataset: HFDataset,
+        limit: Optional[int] = None,
+    ) -> "Dataset":
+        """Create a dataset from a huggingface dataset."""
+        hf_dataframe = huggingface_dataset.to_pandas()  # type: ignore
+        if not isinstance(hf_dataframe, pd.DataFrame):
+            raise ValueError("Expected a DataFrame from the huggingface dataset.")
+
+        unflattened_columns = unflatten_dict(
+            {k: None for k in hf_dataframe.columns}, splitter="dot"
+        )
+        df_unflattened = pd.DataFrame({}, columns=unflattened_columns)
+
+        for indx, row in hf_dataframe.iterrows():
+            unflattened_row = unflatten_dict(row.to_dict(), splitter="dot")
+            df_unflattened.loc[indx] = pd.Series(unflattened_row)
+        hf_dataframe: pd.DataFrame = df_unflattened
+
+        documents = []
+        document_ids = hf_dataframe["document_id"].unique()
+
+        if limit is not None:
+            document_ids = document_ids[:limit]
+            hf_dataframe = hf_dataframe[hf_dataframe["document_id"].isin(document_ids)]
+
+        for document_id in document_ids:
+            document_df = hf_dataframe[hf_dataframe["document_id"] == document_id]
+            document_languages = np.unique(document_df["languages"])
+
+            for document_language in document_languages:
+                document_language: list = list(document_language)
+                document_lang_df = document_df[
+                    document_df["languages"] == document_language[0]
+                ]
+
+                parser_output = passage_level_df_to_document_model(
+                    df=document_lang_df, document_model=self.document_model
+                )
+                documents.append(parser_output)
+
+        self.documents = documents
+
+        return self
+
     def _from_huggingface_parquet(
         self,
         huggingface_dataset: HFDataset,
         limit: Optional[int] = None,
     ) -> "Dataset":
         """
         Create a dataset from a huggingface dataset.
@@ -1352,14 +1496,15 @@
         return self
 
     def from_huggingface(
         self,
         dataset_name: Optional[str] = None,
         dataset_version: Optional[str] = None,
         limit: Optional[int] = None,
+        passage_level_and_flat: bool = False,
         **kwargs,
     ) -> "Dataset":
         """
         Load documents from a huggingface hub dataset.
 
         For private repos a token should be provided either as a `token` kwarg or as
         environment variable HUGGINGFACE_TOKEN. Any additional keyword arguments are
@@ -1385,8 +1530,11 @@
             )
 
         huggingface_dataset = load_dataset(
             dataset_name, dataset_version, token=token, split="train", **kwargs
         )
 
         # TODO: validate the result coming from the below method
-        return self._from_huggingface_parquet(huggingface_dataset, limit)  # type: ignore
+        if passage_level_and_flat:
+            return self._from_huggingface_passage_level_flat_parquet(huggingface_dataset, limit)  # type: ignore
+        else:
+            return self._from_huggingface_parquet(huggingface_dataset, limit)  # type: ignore
```

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/models/search.py` & `cpr_sdk-1.1.4/src/cpr_sdk/models/search.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/parser_models.py` & `cpr_sdk-1.1.4/src/cpr_sdk/parser_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+import json
 import logging
 import logging.config
 from collections import Counter
 from datetime import date
 from enum import Enum
-import json
-from typing import List, Optional, Sequence, Tuple, TypeVar, Union, Any
+from typing import Any, Final, List, Optional, Sequence, Tuple, TypeVar, Union
 
 from cpr_sdk.pipeline_general_models import (
     CONTENT_TYPE_HTML,
     CONTENT_TYPE_PDF,
     BackendDocument,
     Json,
 )
 from cpr_sdk.utils import remove_key_if_all_nested_vals_none, unflatten_json
 from langdetect import DetectorFactory, LangDetectException, detect
 from pydantic import AnyHttpUrl, BaseModel, Field, model_validator
 
 _LOGGER = logging.getLogger(__name__)
 
-PARSER_METADATA_KEY = "parser_metadata"
-AZURE_API_VERSION_KEY = "azure_api_version"
-AZURE_MODEL_ID_KEY = "azure_model_id"
-PARSING_DATE_KEY = "parsing_date"
+PARSER_METADATA_KEY: Final = "parser_metadata"
+AZURE_API_VERSION_KEY: Final = "azure_api_version"
+AZURE_MODEL_ID_KEY: Final = "azure_model_id"
+PARSING_DATE_KEY: Final = "parsing_date"
+PDF_PAGE_METADATA_KEY: Final = "pdf_data_page_metadata"
+PDF_DATA_PASSAGE_LEVEL_EXPAND_FIELDS: Final = {"text_blocks", "page_metadata"}
+HTML_DATA_PASSAGE_LEVEL_EXPAND_FIELDS: Final = {"text_blocks"}
 
 
 class VerticalFlipError(Exception):
     """Exception for when a vertical flip fails."""
 
     pass
 
@@ -391,37 +394,64 @@
         model_dump_json method and then reloading with json.load is as objects like
         Enums and child pydantic objects persist when using the model_dump method.
         We don't want these when we push to huggingface.
         """
         if self.text_blocks is None:
             return []
 
-        common_fields_dict = json.loads(
+        fixed_fields_dict = json.loads(
             self.model_dump_json(
                 exclude={
-                    "pdf_data": {"text_blocks", "page_metadata"},
-                    "html_data": {"text_blocks"},
+                    "pdf_data": PDF_DATA_PASSAGE_LEVEL_EXPAND_FIELDS,
+                    "html_data": HTML_DATA_PASSAGE_LEVEL_EXPAND_FIELDS,
                 }
             )
         )
 
         passages_array = [
-            common_fields_dict
+            fixed_fields_dict
             | json.loads(block.model_dump_json(exclude={"text"}))
             | {"text": block.to_string(), "block_index": idx}
             for idx, block in enumerate(self.text_blocks)
         ]
 
+        for passage in passages_array:
+            page_number = passage.get("page_number")
+            passage[PDF_PAGE_METADATA_KEY] = (
+                self.get_page_metadata_by_page_number(page_number)
+                if page_number
+                else None
+            )
+
         empty_html_text_block_keys: list[str] = list(HTMLTextBlock.model_fields.keys())
         empty_pdf_text_block_keys: list[str] = list(PDFTextBlock.model_fields.keys())
 
         passages_array_filled = []
         for passage in passages_array:
             for key in empty_html_text_block_keys:
                 if key not in passage:
                     passage[key] = None
             for key in empty_pdf_text_block_keys:
                 if key not in passage:
                     passage[key] = None
             passages_array_filled.append(passage)
 
         return passages_array_filled
+
+    def get_page_metadata_by_page_number(self, page_number: int) -> Optional[dict]:
+        """
+        Retrieve the first element of PDF page metadata where the page number matches the given page number.
+
+        The reason we convert from the pydantic BaseModel to a string using the
+        model_dump_json method and then reloading with json.load is as objects like
+        Enums and child pydantic objects persist when using the model_dump method.
+        We don't want these when we push to huggingface.
+
+        :param pdf_data: PDFData object containing the metadata.
+        :param page_number: The page number to match.
+        :return: The first matching PDFPageMetadata object, or None if no match is found.
+        """
+        if self.pdf_data and self.pdf_data.page_metadata:
+            for metadata in self.pdf_data.page_metadata:
+                if metadata.page_number == page_number:
+                    return json.loads(metadata.model_dump_json())
+        return None
```

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/pipeline_general_models.py` & `cpr_sdk-1.1.4/src/cpr_sdk/pipeline_general_models.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/resources/sensitive_query_terms.tsv` & `cpr_sdk-1.1.4/src/cpr_sdk/resources/sensitive_query_terms.tsv`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/s3.py` & `cpr_sdk-1.1.4/src/cpr_sdk/s3.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/search_adaptors.py` & `cpr_sdk-1.1.4/src/cpr_sdk/search_adaptors.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/utils.py` & `cpr_sdk-1.1.4/src/cpr_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/vespa.py` & `cpr_sdk-1.1.4/src/cpr_sdk/vespa.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/src/cpr_sdk/yql_builder.py` & `cpr_sdk-1.1.4/src/cpr_sdk/yql_builder.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.2/PKG-INFO` & `cpr_sdk-1.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpr_sdk
-Version: 1.1.2
+Version: 1.1.4
 Summary: 
 License: LICENSE
 Author: CPR Tech
 Author-email: tech@climatepolicyradar.org
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
@@ -14,16 +14,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: spacy
 Provides-Extra: vespa
 Requires-Dist: aws-error-utils (>=2.7.0,<3.0.0)
 Requires-Dist: boto3 (>=1.26.16,<2.0.0)
-Requires-Dist: datasets (>=2.14.0,<3.0.0)
+Requires-Dist: datasets (>=2.19.0,<3.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Requires-Dist: flatten-dict (>=0.4.2,<0.5.0)
 Requires-Dist: langdetect (>=1.0.9,<2.0.0)
 Requires-Dist: numpy (>=1.23.5)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: poetry (>=1.8.2,<2.0.0)
 Requires-Dist: pydantic (>=2.4.0,<3.0.0)
 Requires-Dist: pyvespa (>=0.37.1,<0.38.0) ; extra == "vespa"
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0) ; extra == "vespa"
@@ -56,14 +57,25 @@
 dataset = Dataset(GSTDocument).from_huggingface(
     version="d8363af072d7e0f87ec281dd5084fb3d3f4583a9", # commit hash, optional
     limit=1000,
     token="my-huggingface-token", # required for private repos if not in env
 )
 ```
 
+The following flag is used for the passage level and flat dataset.
+
+```py
+dataset = Dataset(
+    document_model=BaseDocument
+).from_huggingface(
+    dataset_name="ClimatePolicyRadar/passage-level-flat-dataset",
+    passage_level_and_flat=True
+)
+```
+
 ### Loading from local storage or s3
 
 ```py
 # document_id is also the filename stem
 
 document = BaseDocument.load_from_local(folder_path="path/to/data/", document_id="document_1234")
```

