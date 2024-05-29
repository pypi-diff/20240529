# Comparing `tmp/cg_hermes-4.4.1.tar.gz` & `tmp/cg_hermes-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_hermes-4.4.1.tar", max compression
+gzip compressed data, was "cg_hermes-4.4.2.tar", max compression
```

## Comparing `cg_hermes-4.4.1.tar` & `cg_hermes-4.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       22 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/__init__.py
--rw-r--r--   0        0        0      289 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/__main__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/cli/__init__.py
--rw-r--r--   0        0        0     1025 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/cli/base.py
--rw-r--r--   0        0        0      946 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/cli/common.py
--rw-r--r--   0        0        0     1542 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/cli/convert.py
--rw-r--r--   0        0        0     3520 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/cli/export.py
--rw-r--r--   0        0        0     3176 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/cli/validate.py
--rw-r--r--   0        0        0    28216 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/balsamic.py
--rw-r--r--   0        0        0     1590 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/balsamic_qc.py
--rw-r--r--   0        0        0     5551 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/balsamic_umi.py
--rw-r--r--   0        0        0      846 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/fluffy.py
--rw-r--r--   0        0        0     2166 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/microsalt.py
--rw-r--r--   0        0        0     8540 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/mip_dna.py
--rw-r--r--   0        0        0     4551 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/mip_rna.py
--rw-r--r--   0        0        0     4354 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/mutant.py
--rw-r--r--   0        0        0      608 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/nextflow.py
--rw-r--r--   0        0        0     4156 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/rnafusion.py
--rw-r--r--   0        0        0     3930 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/taxprofiler.py
--rw-r--r--   0        0        0     7073 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/config/tomte.py
--rw-r--r--   0        0        0    27888 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/constants/tags.py
--rw-r--r--   0        0        0      872 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/constants/workflow.py
--rw-r--r--   0        0        0    12727 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/deliverables.py
--rw-r--r--   0        0        0      338 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/models/__init__.py
--rw-r--r--   0        0        0      642 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/models/tags.py
--rw-r--r--   0        0        0     2476 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/models/workflow_deliverables.py
--rw-r--r--   0        0        0      997 2024-04-29 07:59:35.191729 cg_hermes-4.4.1/cg_hermes/validate.py
--rw-r--r--   0        0        0      773 2024-04-29 07:59:35.195729 cg_hermes-4.4.1/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 cg_hermes-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/__init__.py
+-rw-r--r--   0        0        0      289 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/cli/__init__.py
+-rw-r--r--   0        0        0     1025 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/cli/base.py
+-rw-r--r--   0        0        0      946 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/cli/common.py
+-rw-r--r--   0        0        0     1542 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/cli/convert.py
+-rw-r--r--   0        0        0     3520 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/cli/export.py
+-rw-r--r--   0        0        0     3176 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/cli/validate.py
+-rw-r--r--   0        0        0    28216 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/balsamic.py
+-rw-r--r--   0        0        0     1590 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/balsamic_qc.py
+-rw-r--r--   0        0        0     5551 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/balsamic_umi.py
+-rw-r--r--   0        0        0      846 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/fluffy.py
+-rw-r--r--   0        0        0     2166 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/microsalt.py
+-rw-r--r--   0        0        0     8540 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/mip_dna.py
+-rw-r--r--   0        0        0     4551 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/mip_rna.py
+-rw-r--r--   0        0        0     4354 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/mutant.py
+-rw-r--r--   0        0        0      608 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/nextflow.py
+-rw-r--r--   0        0        0     4156 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/rnafusion.py
+-rw-r--r--   0        0        0     3930 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/taxprofiler.py
+-rw-r--r--   0        0        0     7260 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/config/tomte.py
+-rw-r--r--   0        0        0    28008 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/constants/tags.py
+-rw-r--r--   0        0        0      872 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/constants/workflow.py
+-rw-r--r--   0        0        0    12727 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/deliverables.py
+-rw-r--r--   0        0        0      338 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/models/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/models/tags.py
+-rw-r--r--   0        0        0     2476 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/models/workflow_deliverables.py
+-rw-r--r--   0        0        0      997 2024-05-29 07:54:17.674943 cg_hermes-4.4.2/cg_hermes/validate.py
+-rw-r--r--   0        0        0      773 2024-05-29 07:54:17.678943 cg_hermes-4.4.2/pyproject.toml
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 cg_hermes-4.4.2/PKG-INFO
```

### Comparing `cg_hermes-4.4.1/cg_hermes/cli/base.py` & `cg_hermes-4.4.2/cg_hermes/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/cli/common.py` & `cg_hermes-4.4.2/cg_hermes/cli/common.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/cli/convert.py` & `cg_hermes-4.4.2/cg_hermes/cli/convert.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/cli/export.py` & `cg_hermes-4.4.2/cg_hermes/cli/export.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/cli/validate.py` & `cg_hermes-4.4.2/cg_hermes/cli/validate.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/balsamic.py` & `cg_hermes-4.4.2/cg_hermes/config/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/balsamic_qc.py` & `cg_hermes-4.4.2/cg_hermes/config/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/balsamic_umi.py` & `cg_hermes-4.4.2/cg_hermes/config/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/fluffy.py` & `cg_hermes-4.4.2/cg_hermes/config/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/microsalt.py` & `cg_hermes-4.4.2/cg_hermes/config/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/mip_dna.py` & `cg_hermes-4.4.2/cg_hermes/config/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/mip_rna.py` & `cg_hermes-4.4.2/cg_hermes/config/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/mutant.py` & `cg_hermes-4.4.2/cg_hermes/config/mutant.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/nextflow.py` & `cg_hermes-4.4.2/cg_hermes/config/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/rnafusion.py` & `cg_hermes-4.4.2/cg_hermes/config/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/taxprofiler.py` & `cg_hermes-4.4.2/cg_hermes/config/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/config/tomte.py` & `cg_hermes-4.4.2/cg_hermes/config/tomte.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
         "used_by": [UsageTags.CG, UsageTags.LONG_TERM_STORAGE],
     },
     frozenset({"nextflow-config"}): {
         "is_mandatory": True,
         "tags": [NextflowTags.NEXTFLOW_CONFIG],
         "used_by": [UsageTags.CG, UsageTags.LONG_TERM_STORAGE],
     },
+    frozenset({"nextflow-params"}): {
+        "is_mandatory": True,
+        "tags": [NextflowTags.NEXTFLOW_PARAMS],
+        "used_by": [UsageTags.CG, UsageTags.LONG_TERM_STORAGE],
+    },
     frozenset({QCTags.QC_METRICS}): {
         "is_mandatory": True,
         "tags": [QCTags.QC_METRICS],
         "used_by": [UsageTags.CG, UsageTags.LONG_TERM_STORAGE],
     },
     frozenset({"multiqc", "multiqc-html"}): {
         "is_mandatory": True,
```

### Comparing `cg_hermes-4.4.1/cg_hermes/constants/tags.py` & `cg_hermes-4.4.2/cg_hermes/constants/tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,26 +636,28 @@
             self.OUTRIDER: "Aberrant expression calculated with DROP",
         }
         return descriptions.get(self, "Description not available")
 
 
 class NextflowTags(StrEnum):
     NEXTFLOW_CONFIG: str = "nextflow-config"
+    NEXTFLOW_PARAMS: str = "nextflow-params"
     SAMPLESHEET: str = "nextflow-samplesheet"
     SAMPLESHEET_VALID: str = "samplesheet-valid"
     SOFTWARE_VERSIONS: str = "software-versions"
 
     @classmethod
     def name(cls) -> str:
         return "Nextflow Tags"
 
     @property
     def description(self) -> str:
         descriptions: dict[str, NextflowTags] = {
             self.NEXTFLOW_CONFIG: "Nextflow config for analysis",
+            self.NEXTFLOW_PARAMS: "Nextflow parameters file for analysis",
             self.SAMPLESHEET: "Samplesheet for analysis",
             self.SAMPLESHEET_VALID: "Validated samplesheet",
             self.SOFTWARE_VERSIONS: "List of all software used and their versions",
         }
         return descriptions.get(self, "Description not available")
```

### Comparing `cg_hermes-4.4.1/cg_hermes/constants/workflow.py` & `cg_hermes-4.4.2/cg_hermes/constants/workflow.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/deliverables.py` & `cg_hermes-4.4.2/cg_hermes/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/models/tags.py` & `cg_hermes-4.4.2/cg_hermes/models/tags.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/models/workflow_deliverables.py` & `cg_hermes-4.4.2/cg_hermes/models/workflow_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/cg_hermes/validate.py` & `cg_hermes-4.4.2/cg_hermes/validate.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.4.1/pyproject.toml` & `cg_hermes-4.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cg-hermes"
-version = "4.4.1"
+version = "4.4.2"
 description = "Convert information between pipelines and CG"
 authors = ["Måns Magnusson <mans.magnusson@scilifelab.se>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.7.3"
 coloredlogs = "^14.0"
```

### Comparing `cg_hermes-4.4.1/PKG-INFO` & `cg_hermes-4.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg-hermes
-Version: 4.4.1
+Version: 4.4.2
 Summary: Convert information between pipelines and CG
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.se
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bump2version (>=1.0.1,<2.0.0)
```

