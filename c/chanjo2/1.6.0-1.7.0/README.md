# Comparing `tmp/chanjo2-1.6.0.tar.gz` & `tmp/chanjo2-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanjo2-1.6.0.tar", max compression
+gzip compressed data, was "chanjo2-1.7.0.tar", max compression
```

## Comparing `chanjo2-1.6.0.tar` & `chanjo2-1.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      759 2024-04-23 10:55:14.717780 chanjo2-1.6.0/pyproject.toml
--rw-r--r--   0        0        0       66 2024-04-23 10:55:14.717780 chanjo2-1.6.0/src/chanjo2/__init__.py
--rw-r--r--   0        0        0     3102 2024-04-23 10:55:14.717780 chanjo2-1.6.0/src/chanjo2/constants.py
--rw-r--r--   0        0        0     2640 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/crud/cases.py
--rw-r--r--   0        0        0     7002 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/crud/intervals.py
--rw-r--r--   0        0        0     3886 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/crud/samples.py
--rw-r--r--   0        0        0     1117 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/dbutil.py
--rw-r--r--   0        0        0      346 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/demo/109_green.bed
--rw-r--r--   0        0        0     2101 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/demo/__init__.py
--rw-r--r--   0        0        0   450444 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/demo/panelapp_109_example.d4
--rw-r--r--   0        0        0        0 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/__init__.py
--rw-r--r--   0        0        0     1594 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/cases.py
--rw-r--r--   0        0        0     8272 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/coverage.py
--rw-r--r--   0        0        0     6109 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/intervals.py
--rw-r--r--   0        0        0     3808 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/overview.py
--rw-r--r--   0        0        0     3247 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/report.py
--rw-r--r--   0        0        0     2024 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/samples.py
--rw-r--r--   0        0        0     2150 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/main.py
--rw-r--r--   0        0        0        0 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/__init__.py
--rw-r--r--   0        0        0     1249 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_bed.py
--rw-r--r--   0        0        0     2433 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_completeness_tasks.py
--rw-r--r--   0        0        0    12286 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_d4.py
--rw-r--r--   0        0        0     7608 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_load_intervals.py
--rw-r--r--   0        0        0     8877 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_report_contents.py
--rw-r--r--   0        0        0      335 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/models/__init__.py
--rw-r--r--   0        0        0    10600 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/models/pydantic_models.py
--rw-r--r--   0        0        0     4512 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/models/sql_models.py
--rw-r--r--   0        0        0     2552 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/populate_demo.py
--rw-r--r--   0        0        0      344 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/static/main.css
--rw-r--r--   0        0        0     1778 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/templates/base-layout.html
--rw-r--r--   0        0        0     1253 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/templates/gene-overview.html
--rw-r--r--   0        0        0     3415 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/templates/overview.html
--rw-r--r--   0        0        0     8274 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/templates/report.html
--rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 chanjo2-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      759 2024-05-29 12:19:56.597289 chanjo2-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/__init__.py
+-rw-r--r--   0        0        0     3102 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/constants.py
+-rw-r--r--   0        0        0     2640 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/crud/cases.py
+-rw-r--r--   0        0        0     7002 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/crud/intervals.py
+-rw-r--r--   0        0        0     3886 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/crud/samples.py
+-rw-r--r--   0        0        0     1117 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/dbutil.py
+-rw-r--r--   0        0        0      346 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/demo/109_green.bed
+-rw-r--r--   0        0        0     2101 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/demo/__init__.py
+-rw-r--r--   0        0        0   450444 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/demo/panelapp_109_example.d4
+-rw-r--r--   0        0        0        0 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/endpoints/__init__.py
+-rw-r--r--   0        0        0     1594 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/endpoints/cases.py
+-rw-r--r--   0        0        0     8272 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/endpoints/coverage.py
+-rw-r--r--   0        0        0     6109 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/endpoints/intervals.py
+-rw-r--r--   0        0        0     3808 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/endpoints/overview.py
+-rw-r--r--   0        0        0     3247 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/endpoints/report.py
+-rw-r--r--   0        0        0     2024 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/endpoints/samples.py
+-rw-r--r--   0        0        0     2150 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/main.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/meta/__init__.py
+-rw-r--r--   0        0        0     1249 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/meta/handle_bed.py
+-rw-r--r--   0        0        0     2433 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/meta/handle_completeness_tasks.py
+-rw-r--r--   0        0        0    12286 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/meta/handle_d4.py
+-rw-r--r--   0        0        0     7608 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/meta/handle_load_intervals.py
+-rw-r--r--   0        0        0     8989 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/meta/handle_report_contents.py
+-rw-r--r--   0        0        0      335 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/models/__init__.py
+-rw-r--r--   0        0        0    10600 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/models/pydantic_models.py
+-rw-r--r--   0        0        0     4512 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/models/sql_models.py
+-rw-r--r--   0        0        0     2552 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/populate_demo.py
+-rw-r--r--   0        0        0      344 2024-05-29 12:19:56.597289 chanjo2-1.7.0/src/chanjo2/static/main.css
+-rw-r--r--   0        0        0     1778 2024-05-29 12:19:56.601289 chanjo2-1.7.0/src/chanjo2/templates/base-layout.html
+-rw-r--r--   0        0        0     1253 2024-05-29 12:19:56.601289 chanjo2-1.7.0/src/chanjo2/templates/gene-overview.html
+-rw-r--r--   0        0        0     3415 2024-05-29 12:19:56.601289 chanjo2-1.7.0/src/chanjo2/templates/overview.html
+-rw-r--r--   0        0        0     8253 2024-05-29 12:19:56.601289 chanjo2-1.7.0/src/chanjo2/templates/report.html
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 chanjo2-1.7.0/PKG-INFO
```

### Comparing `chanjo2-1.6.0/pyproject.toml` & `chanjo2-1.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chanjo2"
-version = "1.6.0"
+version = "1.7.0"
 description = "Next generation coverage analysis"
 authors = ["northwestwitch <chiara.rasi@scilifelab.se>"]
 
 [tool.poetry_bumpversion.file."src/chanjo2/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `chanjo2-1.6.0/src/chanjo2/constants.py` & `chanjo2-1.7.0/src/chanjo2/constants.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/crud/cases.py` & `chanjo2-1.7.0/src/chanjo2/crud/cases.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/crud/intervals.py` & `chanjo2-1.7.0/src/chanjo2/crud/intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/crud/samples.py` & `chanjo2-1.7.0/src/chanjo2/crud/samples.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/dbutil.py` & `chanjo2-1.7.0/src/chanjo2/dbutil.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/demo/__init__.py` & `chanjo2-1.7.0/src/chanjo2/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/demo/panelapp_109_example.d4` & `chanjo2-1.7.0/src/chanjo2/demo/panelapp_109_example.d4`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/endpoints/cases.py` & `chanjo2-1.7.0/src/chanjo2/endpoints/cases.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/endpoints/coverage.py` & `chanjo2-1.7.0/src/chanjo2/endpoints/coverage.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/endpoints/intervals.py` & `chanjo2-1.7.0/src/chanjo2/endpoints/intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/endpoints/overview.py` & `chanjo2-1.7.0/src/chanjo2/endpoints/overview.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/endpoints/report.py` & `chanjo2-1.7.0/src/chanjo2/endpoints/report.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/endpoints/samples.py` & `chanjo2-1.7.0/src/chanjo2/endpoints/samples.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/main.py` & `chanjo2-1.7.0/src/chanjo2/main.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/meta/handle_bed.py` & `chanjo2-1.7.0/src/chanjo2/meta/handle_bed.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/meta/handle_completeness_tasks.py` & `chanjo2-1.7.0/src/chanjo2/meta/handle_completeness_tasks.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/meta/handle_d4.py` & `chanjo2-1.7.0/src/chanjo2/meta/handle_d4.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/meta/handle_load_intervals.py` & `chanjo2-1.7.0/src/chanjo2/meta/handle_load_intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/meta/handle_report_contents.py` & `chanjo2-1.7.0/src/chanjo2/meta/handle_report_contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,18 @@
     data: Dict = {
         "levels": get_ordered_levels(threshold_levels=query.completeness_thresholds),
         "extras": {
             "panel_name": query.panel_name,
             "default_level": query.default_level,
             "interval_type": query.interval_type.value,
             "case_name": query.case_display_name,
-            "hgnc_gene_ids": [gene.hgnc_id for gene in genes],
+            "hgnc_gene_ids": [gene.hgnc_id for gene in genes]
+            or query.hgnc_gene_ids
+            or query.hgnc_gene_symbols
+            or query.ensembl_gene_ids,
             "build": query.build.value,
             "completeness_thresholds": query.completeness_thresholds,
             "samples": [_serialize_sample(sample) for sample in query.samples],
         },
         "completeness_rows": [],
         "incomplete_coverage_rows": [],
         "default_level_completeness_rows": [],
```

### Comparing `chanjo2-1.6.0/src/chanjo2/models/pydantic_models.py` & `chanjo2-1.7.0/src/chanjo2/models/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/models/sql_models.py` & `chanjo2-1.7.0/src/chanjo2/models/sql_models.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/populate_demo.py` & `chanjo2-1.7.0/src/chanjo2/populate_demo.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/templates/base-layout.html` & `chanjo2-1.7.0/src/chanjo2/templates/base-layout.html`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/templates/gene-overview.html` & `chanjo2-1.7.0/src/chanjo2/templates/gene-overview.html`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/templates/overview.html` & `chanjo2-1.7.0/src/chanjo2/templates/overview.html`

 * *Files identical despite different names*

### Comparing `chanjo2-1.6.0/src/chanjo2/templates/report.html` & `chanjo2-1.7.0/src/chanjo2/templates/report.html`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 						  <option value="{{ level }}" {% if level == extras.default_level %} selected {% endif %}>{{ level }}x</option>
 						{% endfor %}
 					  </select>
 					</div>
 
 				<div class="col-6">
 				  <label class="form-label">Gene panel name to display</label>
-				  <input class="form-control" id="panel_name" type="text" placeholder="Skeletal dysplasia 3.2" value="{{ extras.panel_name or '' }}">
+				  <input class="form-control" id="panel_name" name="panel_name" type="text" placeholder="Skeletal dysplasia 3.2" value="{{ extras.panel_name or '' }}">
 				</div>
 			  </div>
 			</div>
 
 			<div class="row">
 				<div class="col-7">
 				  <label class="form-label">Included genes (Comma separated list HGNC IDs, HGNC symbols or Ensembl IDs)</label>
@@ -120,18 +120,20 @@
 	  {% endfor %}
 	</tbody>
   </table>
 </div>
 {% endmacro %}
 
 {% macro default_level_metrics() %}
- <div class="col-xs-1 col-xs-offset-9" style="text-align: right;"><input type="checkbox" name="show_genes" onclick="toggle_visibility(['incompletelyCoveredGenesHeader', 'incompletelyCoveredGenesCell']);"></div>
-	 <div class="col-xs-2">
-		 <label class="control-label">Show genes</label>
-	 </div>
+<div>
+	<label>
+		Show genes
+		<input type="checkbox" name="show_genes" style="vertical-align:middle;" onKeyDown="doSomething();" tabindex="0" onclick="toggle_visibility(['incompletelyCoveredGenesHeader', 'incompletelyCoveredGenesCell']);">
+	</label>
+</div>
 <table class="table table-bordered table-hover">
 	 <caption>Genes/Transcripts/Exons coverage at default coverage threshold</caption>
       <thead>
         <tr>
           <th>Sample</th>
           <th>Fully covered {{ interval_type }} [%]</th>
           <th>Incompletely covered {{ interval_type }}</th>
```

#### html2text {}

```diff
@@ -23,16 +23,15 @@
 {% endmacro %} {% macro important_metrics() %}
                AAvveerraaggee ccoovveerraaggee aanndd ccoovveerraaggee ccoommpplleetteenneessss ddaattaa
 SSaammppllee       AAvveerraaggee ccoovveerraaggee[[xx]]             CCoommpplleetteenneessss {{{{ lleevveell__iinntt }}}}xx [[%%]]
              {{ stats.mean_coverage|round(2) {{ stats[level_key] if stats
 {{ sample }} if stats.mean_coverage is       [level_key] is defined }}
              defined }}
 {% endmacro %} {% macro default_level_metrics() %}
-??
-Show genes
+Show genes??
         GGeenneess//TTrraannssccrriippttss//EExxoonnss ccoovveerraaggee aatt ddeeffaauulltt ccoovveerraaggee tthhrreesshhoolldd
             FFuullllyy ccoovveerreedd IInnccoommpplleetteellyy
             {{             ccoovveerreedd {{     IInnccoommpplleetteellyy
 SSaammppllee      {{             {{             ccoovveerreedd ggeenneess
             iinntteerrvvaall__ttyyppee iinntteerrvvaall__ttyyppee
             }}}} [[%%]]        }}}}
             No incompletely covered                                 {{ data
```

### Comparing `chanjo2-1.6.0/PKG-INFO` & `chanjo2-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chanjo2
-Version: 1.6.0
+Version: 1.7.0
 Summary: Next generation coverage analysis
 Author: northwestwitch
 Author-email: chiara.rasi@scilifelab.se
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

