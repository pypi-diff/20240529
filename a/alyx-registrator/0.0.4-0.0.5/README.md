# Comparing `tmp/alyx_registrator-0.0.4.tar.gz` & `tmp/alyx_registrator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alyx_registrator-0.0.4.tar", last modified: Fri May  3 09:58:13 2024, max compression
+gzip compressed data, was "alyx_registrator-0.0.5.tar", last modified: Wed May 29 17:14:20 2024, max compression
```

## Comparing `alyx_registrator-0.0.4.tar` & `alyx_registrator-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6234 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/README.md
--rw-r--r--   0        0        0       51 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/__init__.py
--rw-r--r--   0        0        0    28212 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/registration.py
--rw-r--r--   0        0        0    12095 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/rules.json
--rw-r--r--   0        0        0     2904 2024-05-03 09:58:04.603888 alyx_registrator-0.0.4/one_registrator/utils.py
--rw-r--r--   0        0        0      660 2024-05-03 09:58:13.759749 alyx_registrator-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6234 2024-05-29 17:14:10.969092 alyx_registrator-0.0.5/one_registrator/README.md
+-rw-r--r--   0        0        0       51 2024-05-29 17:14:10.969092 alyx_registrator-0.0.5/one_registrator/__init__.py
+-rw-r--r--   0        0        0    28329 2024-05-29 17:14:10.973092 alyx_registrator-0.0.5/one_registrator/registration.py
+-rw-r--r--   0        0        0    11707 2024-05-29 17:14:10.973092 alyx_registrator-0.0.5/one_registrator/rules.json
+-rw-r--r--   0        0        0     2904 2024-05-29 17:14:10.973092 alyx_registrator-0.0.5/one_registrator/utils.py
+-rw-r--r--   0        0        0      660 2024-05-29 17:14:20.592923 alyx_registrator-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.5/PKG-INFO
```

### Comparing `alyx_registrator-0.0.4/one_registrator/README.md` & `alyx_registrator-0.0.5/one_registrator/README.md`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.4/one_registrator/registration.py` & `alyx_registrator-0.0.5/one_registrator/registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,14 +436,16 @@
         if isinstance(rule, str):  # constant replacement
             return rule
         # then, it must be a dictionnary with pattern defined
         pattern_name = rule["pattern"]
         search_on = rule.get("search_on", "source_path")
         if search_on == "source_path":
             searched_string = file_record.source_path
+        elif search_on == "source_filename":
+            searched_string = os.path.basename(file_record.source_path)
         else:
             searched_string = file_record.source_alf_info[search_on]  # TODO make a list check in __init__ for that
 
         try:
             match = self.patterns[pattern_name].search(searched_string)
         except KeyError:
             # TODO : move that in __init__ to avoid errors at rule runtime, and indicate them at compile time.
```

### Comparing `alyx_registrator-0.0.4/one_registrator/rules.json` & `alyx_registrator-0.0.5/one_registrator/rules.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9842235725308642%*

 * *Differences: {"'re_patterns'": "{'FOV_NO': '^.*(?:(?:FOV)|(?:fieldOfView))[-_ \\\\.]*?(\\\\d+).*$', "*

 * *                  "'IOI_WITH_VERSIONS': "*

 * *                  "'^(?:stim.*?_)?([a-zA-Z0-9]+)(?:(?:_|.)((?:[vV]\\\\d+)|(?:crash)))?(?:stim)?.*$'}",*

 * * "'rules'": "{'field_of_view_png_rule1': {'if': {'object': OrderedDict([('contain', ['FOV', "*

 * *            '\'imaging\'])])}, \'rename\': {\'extra\': {\'eval\': "match[1].zfill(2) if match is '*

 * *            'not None and match.lastindex > 0 else \'\'"}}}, \'intrinsic_imaging_tdms […]*

```diff
@@ -23,17 +23,17 @@
         "Fiji_Analysis",
         "FijiAnalysis",
         "fijiAnalysis"
     ],
     "re_patterns": {
         "ALYX_PATH_EID": "\\w+(?:\\|/)\\d{4}\\-\\d{2}\\-\\d{2}(?:\\|/)\\d{3}",
         "CONDENSED_DATE": ".*?(20\\d{4,6}).*?",
-        "FOV_NO": "^.*(?:FOV)|(?:fieldOfView)[-_ \\.]*?(\\d+).*$",
+        "FOV_NO": "^.*(?:(?:FOV)|(?:fieldOfView))[-_ \\.]*?(\\d+).*$",
         "IOI_WHISKER": "^([a-zA-Z0-9]+)",
-        "IOI_WITH_VERSIONS": ".*_[vV]\\d",
+        "IOI_WITH_VERSIONS": "^(?:stim.*?_)?([a-zA-Z0-9]+)(?:(?:_|.)((?:[vV]\\d+)|(?:crash)))?(?:stim)?.*$",
         "SESSION_NO": ".*?20\\d{4,6}_(\\d).*?",
         "TDMS_TRIALS_TABLE_TIME": "(\\d{4}_\\d{2}_\\d{2}_\\d{2}_\\d{2})\\.tdms$",
         "TDMS_VIDEO_TRIAL_NO": ".*?(\\d+)\\.tdms$",
         "TIFF_FRAME_NO": ".*(\\d{5})\\.tiff?$",
         "VGAT_MOUSE_NO": "Vgat.*?(\\d{1,3}).*jRGECO"
     },
     "rules": {
@@ -214,24 +214,30 @@
                 "collection": [
                     "",
                     "imaging_data"
                 ],
                 "extension": [
                     "png",
                     "PNG"
-                ]
+                ],
+                "object": {
+                    "contain": [
+                        "FOV",
+                        "imaging"
+                    ]
+                }
             },
             "on": {
                 "match": "rename"
             },
             "rename": {
                 "attribute": "fieldOfView",
                 "collection": "imaging_data",
                 "extra": {
-                    "eval": "match[1].zfill(2) if match is not None else ''",
+                    "eval": "match[1].zfill(2) if match is not None and match.lastindex > 0 else ''",
                     "pattern": "FOV_NO"
                 },
                 "object": "imaging"
             }
         },
         "imaging_data_rule1": {
             "if": {
@@ -329,43 +335,21 @@
                 "match": "rename"
             },
             "rename": {
                 "attribute": "bin_delta_stim_images",
                 "collection": "intrinsic_optical_imaging",
                 "extension": "binlv",
                 "extra": {
-                    "eval": "match[1]",
-                    "pattern": "IOI_WHISKER",
-                    "search_on": "object"
+                    "eval": "match[1] + ('.' + match[2] if match.lastindex > 1 else '')",
+                    "pattern": "IOI_WITH_VERSIONS",
+                    "search_on": "source_filename"
                 },
                 "object": "imaging_intrinsic"
             }
         },
-        "intrinsic_imaging_exclude_versions_rule1": {
-            "if": {
-                "collection": {
-                    "exact": [
-                        "intrinsic_optical_imaging",
-                        "IOI"
-                    ]
-                },
-                "object": {
-                    "match": "IOI_WITH_VERSIONS"
-                }
-            },
-            "on": {
-                "match": "exclude"
-            },
-            "overrides": [
-                "intrinsic_imaging_binaries_rule1",
-                "intrinsic_imaging_vessels_rule1",
-                "intrinsic_imaging_tdms_rule1",
-                "intrinsic_imaging_alredy_renamed_versions_rule1"
-            ]
-        },
         "intrinsic_imaging_tdms_rule1": {
             "if": {
                 "collection": {
                     "exact": [
                         "intrinsic_optical_imaging",
                         "IOI"
                     ]
@@ -375,17 +359,17 @@
             "on": {
                 "match": "rename"
             },
             "rename": {
                 "attribute": "delta_stim_images",
                 "collection": "intrinsic_optical_imaging",
                 "extra": {
-                    "eval": "match[1]",
-                    "pattern": "IOI_WHISKER",
-                    "search_on": "object"
+                    "eval": "match[1] + ('.' + match[2] if match.lastindex > 1 else '')",
+                    "pattern": "IOI_WITH_VERSIONS",
+                    "search_on": "source_filename"
                 },
                 "object": "imaging_intrinsic"
             }
         },
         "intrinsic_imaging_vessels_rule1": {
             "if": {
                 "collection": {
```

### Comparing `alyx_registrator-0.0.4/one_registrator/utils.py` & `alyx_registrator-0.0.5/one_registrator/utils.py`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.4/pyproject.toml` & `alyx_registrator-0.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dependencies = [
     "numpy>=1.23",
     "alyx-connector>=1.16",
     "pandas>=1.4",
 ]
 requires-python = ">=3.11"
 dynamic = []
-version = "0.0.4"
+version = "0.0.5"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

