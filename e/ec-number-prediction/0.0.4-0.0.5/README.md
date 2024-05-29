# Comparing `tmp/ec_number_prediction-0.0.4.tar.gz` & `tmp/ec_number_prediction-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec_number_prediction-0.0.4.tar", last modified: Thu Mar  7 09:29:04 2024, max compression
+gzip compressed data, was "ec_number_prediction-0.0.5.tar", last modified: Wed May 29 13:11:42 2024, max compression
```

## Comparing `ec_number_prediction-0.0.4.tar` & `ec_number_prediction-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-03-07 09:29:04.798951 ec_number_prediction-0.0.4/
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1070 2024-01-24 10:18:01.000000 ec_number_prediction-0.0.4/LICENSE
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      108 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.4/MANIFEST.in
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    14896 2024-03-07 09:29:04.798951 ec_number_prediction-0.0.4/PKG-INFO
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    19564 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.4/README.md
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    13975 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.4/README_pypi.md
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      531 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.4/pyproject.toml
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1097 2024-03-07 09:29:04.799951 ec_number_prediction-0.0.4/setup.cfg
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)       69 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/setup.py
-drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-03-07 09:29:04.759951 ec_number_prediction-0.0.4/src/
-drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-03-07 09:29:04.785951 ec_number_prediction-0.0.4/src/ec_number_prediction/
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)       64 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/__init__.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    10192 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/_utils.py
-drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-03-07 09:29:04.796951 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      238 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/__init__.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1307 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/download_uniprot.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     4235 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/enrichment_with_trembl.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1109 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/filter_uniref.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     5593 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/multi_label_binarizer.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      785 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/n_classes_removal.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      984 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/scrape_uniprot.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     7733 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/split.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      853 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/underrepresented_labels_removal.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     5445 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/uniprot_xml_parser.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      985 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/uniref_xml_parser.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     9755 2024-03-01 14:25:00.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/ecpick.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1190 2024-01-29 16:11:38.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/enumerators.py
-drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-03-07 09:29:04.796951 ec_number_prediction-0.0.4/src/ec_number_prediction/feature_extraction/
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)        0 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/feature_extraction/__init__.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     5440 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/feature_extraction/generate_features.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    29855 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/labels_names.pkl
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    64416 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/labels_names_all_data.pkl
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    20608 2024-02-29 11:53:33.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/predictions.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      236 2024-01-26 12:55:20.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/run_data_processing_pipeline.py
-drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-03-07 09:29:04.797952 ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)        0 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/__init__.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    10237 2024-01-30 12:58:13.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/optimize_dnn.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    25463 2024-01-29 14:42:57.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/pipeline_runner.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     5032 2024-01-30 12:58:13.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/train_baselines.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     2872 2024-01-30 12:58:13.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/train_deep_ec.py
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     2933 2024-01-30 12:58:13.000000 ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/train_dspace.py
-drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-03-07 09:29:04.797952 ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)    14896 2024-03-07 09:29:04.000000 ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/PKG-INFO
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1925 2024-03-07 09:29:04.000000 ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/SOURCES.txt
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      108 2024-03-07 09:29:04.000000 ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/dependency_links.txt
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)        1 2024-01-24 13:18:14.000000 ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/not-zip-safe
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)      138 2024-03-07 09:29:04.000000 ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/requires.txt
--rw-r--r--   0 jcapela   (1018) jcapela   (1018)       21 2024-03-07 09:29:04.000000 ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/top_level.txt
+drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-05-29 13:11:42.281656 ec_number_prediction-0.0.5/
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1070 2024-01-24 10:18:01.000000 ec_number_prediction-0.0.5/LICENSE
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      108 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.5/MANIFEST.in
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    14896 2024-05-29 13:11:42.281656 ec_number_prediction-0.0.5/PKG-INFO
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    20072 2024-05-29 12:30:08.000000 ec_number_prediction-0.0.5/README.md
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    13975 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.5/README_pypi.md
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      531 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.5/pyproject.toml
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1097 2024-05-29 13:11:42.282656 ec_number_prediction-0.0.5/setup.cfg
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)       69 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/setup.py
+drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-05-29 13:11:42.240656 ec_number_prediction-0.0.5/src/
+drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-05-29 13:11:42.267656 ec_number_prediction-0.0.5/src/ec_number_prediction/
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)       64 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/__init__.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    10192 2024-02-29 11:01:09.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/_utils.py
+drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-05-29 13:11:42.278656 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      230 2024-04-16 12:31:04.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/__init__.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1307 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/download_uniprot.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     5519 2024-05-29 09:31:09.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/enrichment_with_trembl.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1109 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/filter_uniref.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     6704 2024-05-29 09:27:34.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/multi_label_binarizer.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      785 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/n_classes_removal.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      984 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/scrape_uniprot.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    10104 2024-05-29 09:23:54.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/split.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      853 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/underrepresented_labels_removal.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     5469 2024-05-29 06:44:00.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/uniprot_xml_parser.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      985 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/uniref_xml_parser.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     9755 2024-03-01 14:25:00.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/ecpick.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1118 2024-05-29 09:14:46.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/enumerators.py
+drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-05-29 13:11:42.278656 ec_number_prediction-0.0.5/src/ec_number_prediction/feature_extraction/
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)        0 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/feature_extraction/__init__.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     5440 2024-04-16 14:20:13.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/feature_extraction/generate_features.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    29855 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/labels_names.pkl
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    64416 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/labels_names_all_data.pkl
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    20608 2024-02-29 11:53:33.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/predictions.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      236 2024-01-26 12:55:20.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/run_data_processing_pipeline.py
+drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-05-29 13:11:42.279656 ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)        0 2024-01-24 10:18:02.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/__init__.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    10237 2024-01-30 12:58:13.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/optimize_dnn.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    25463 2024-01-29 14:42:57.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/pipeline_runner.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     5032 2024-01-30 12:58:13.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/train_baselines.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     2872 2024-01-30 12:58:13.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/train_deep_ec.py
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     2933 2024-01-30 12:58:13.000000 ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/train_dspace.py
+drwxr-xr-x   0 jcapela   (1018) jcapela   (1018)        0 2024-05-29 13:11:42.279656 ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)    14896 2024-05-29 13:11:42.000000 ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/PKG-INFO
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)     1925 2024-05-29 13:11:42.000000 ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/SOURCES.txt
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      108 2024-05-29 13:11:42.000000 ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/dependency_links.txt
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)        1 2024-01-24 13:18:14.000000 ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/not-zip-safe
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)      138 2024-05-29 13:11:42.000000 ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/requires.txt
+-rw-r--r--   0 jcapela   (1018) jcapela   (1018)       21 2024-05-29 13:11:42.000000 ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/top_level.txt
```

### Comparing `ec_number_prediction-0.0.4/LICENSE` & `ec_number_prediction-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/PKG-INFO` & `ec_number_prediction-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec_number_prediction
-Version: 0.0.4
+Version: 0.0.5
 Summary: ec_number_prediction
 Author: Joao Capela
 License: MIT
 Keywords: plants,secondary metabolism
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `ec_number_prediction-0.0.4/README.md` & `ec_number_prediction-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,20 @@
 generate_one_hot_encodings(save_folder="/home/working_dir", dataset_directory="/home/working_dir/data")
 ```
 
 ## Train models
 
 Training the baselines is also easy:
 
+### Models' implementation
+
+- DNN - [Fully connected neural network](https://github.com/jcapels/PlantsSM/blob/v0.0.2/src/plants_sm/models/fc/fc.py)
+- DeepEC CNN3 - [CNN](https://github.com/jcapels/PlantsSM/blob/v0.0.2/src/plants_sm/models/ec_number_prediction/deepec.py)
+- D-SPACE EC - [CNN](https://github.com/jcapels/PlantsSM/blob/v0.0.2/src/plants_sm/models/ec_number_prediction/d_space.py)
+
 ### Train baselines
 
 ```python
 from ec_number_prediction.train_models.train_baselines import train_dnn_baselines
 
 train_dnn_baselines(model = "esm2_t33_650M_UR50D", working_dir="/home/working_dir/")
 ```
@@ -211,39 +217,39 @@
 ### Predict with model
 
 Here you can see how to predict EC numbers with a model. Note that the model chosen in the following examples is
 "DNN ProtBERT all data", but you can choose any of the models:
 
 - DNN ProtBERT all data
 - DNN ESM1b all data
-- DNN ESM2 3B all data - note that this model requires at least **12 GB** of RAM to be run. If you intend to use GPU to 
-make the predictions, you need to have at least **20 GB** of GPU memory or 4 GPUs with **8 GB**.
+- DNN ESM2 3B all data - note that this model requires at least **25 GB** of RAM to be run. If you intend to use GPU to 
+make the predictions, you need to have at least **25 GB** of CPU memory or 4 GPUs with **8 GB** each.
 - ProtBERT trial 2 train plus validation (for this model, you need to pass all_data=False)
 - DNN ESM1b trial 4 train plus validation (for this model, you need to pass all_data=False)
 - DNN ESM2 3B trial 2 train plus validation (for this model, you need to pass all_data=False)
 
 Here you can see the time taken and memory usage for each model to predict for different number of data points:
 
 | Model           | Data Points | Time Taken | Memory Usage |
 |-----------------|-------------|---------|--------------|
 | DNN ProtBERT    | 25          | 0:00:05 | 1G           |
 | DNN ProtBERT    | 100         | 0:00:08 | 1G           |
 | DNN ProtBERT    | 1000        | 0:00:56 | 1G           |
 | DNN ProtBERT    | 10000       | 0:09:00 | 1G           |
 | DNN ProtBERT    | 100000      | 1:55:08 | 7G           |
-| DNN ESM1b       | 25          | 0:00:28 | 2G           |
-| DNN ESM1b       | 100         | 0:00:40 | 2G           |
-| DNN ESM1b       | 1000        | 0:02:22 | 2G           |
-| DNN ESM1b       | 10000       | 0:19:22 | 2G           |
-| DNN ESM1b       | 100000      | 3:35:04 | 7G           |
-| DNN ESM2 3B     | 25          | 0:01:35 | 10G          |
-| DNN ESM2 3B     | 100         | 0:03:40 | 10G          |
-| DNN ESM2 3B     | 1000        | 0:28:27 | 10G          |
-| DNN ESM2 3B     | 10000       | 4:33:50 | 10G          |
-| DNN ESM2 3B | 100000 | 1 day, 22:10:43 | 10G  |
+| DNN ESM1b       | 25          | 0:00:28 | 10G           |
+| DNN ESM1b       | 100         | 0:00:40 | 10G           |
+| DNN ESM1b       | 1000        | 0:02:22 | 10G           |
+| DNN ESM1b       | 10000       | 0:19:22 | 10G           |
+| DNN ESM1b       | 100000      | 3:35:04 | 10G           |
+| DNN ESM2 3B     | 25          | 0:01:35 | 25G          |
+| DNN ESM2 3B     | 100         | 0:03:40 | 25G          |
+| DNN ESM2 3B     | 1000        | 0:28:27 | 25G          |
+| DNN ESM2 3B     | 10000       | 4:33:50 | 25G          |
+| DNN ESM2 3B | 100000 | 1 day, 22:10:43 | 25G  |
 | BLAST | 25 | 0:01:37 | 264M |
 | BLAST | 100 | 0:07:29 | 264M |
 | BLAST | 1000 | 0:48:55 | 264M | 
 | BLAST | 10000 | 8:20:03 | 266M |
 | BLAST | 100000 | 2 days, 20:03:17.393101 | 351M |
  
 
@@ -347,15 +353,15 @@
                             fasta_path="/home/jcapela/ec_numbers_prediction/data/test_data.fasta",
                             output_path="test_blast_predictions.csv")
 ```
 
 
 ### Predict with an ensemble of BLAST and DL models
 
-Here you can see how to predict EC numbers with an ensemble between BLAST and models.
+Here you can see how to predict EC numbers with an ensemble between BLAST and models. **The ensemble requires over 25 GB of RAM.**
 
 The parameters of the function are the following:
 
 - **dataset_path**: path to the dataset to predict.
 - **output_path**: path to the output file.
 - **ids_field**: name of the column with the ids.
 - **sequences_field**: name of the column with the sequences.
@@ -379,15 +385,15 @@
 predict_with_ensemble_from_fasta(fasta_path="/home/jcapela/ec_numbers_prediction/data/test_data.fasta",
                         output_path="predictions_ensemble.csv",
                         device="cuda:0")
 ```
 
 ## Data availability
 
-Here you can see how to obtain the data used in the project: https://nextcloud.bio.di.uminho.pt/s/X9cYxappMpgGABn.
+Here you can see how to obtain the data used in the project: https://zenodo.org/records/11380947/files/Supplementary_Information_models_data_and_predictions.zip?download=1.
 In this link, you can find the following folders:
 
 - **data** - this folder contains the data used in the project - the data splits are here too.
 - **models** - this folder contains the models used in the project.
 - **predictions** - this folder contains the predictions made in the project.
 - **features** - this folder contains the features for the test sets.
 - **f1_scores** - this folder contains the F1 scores for the test sets.
```

### Comparing `ec_number_prediction-0.0.4/README_pypi.md` & `ec_number_prediction-0.0.5/README_pypi.md`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/pyproject.toml` & `ec_number_prediction-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/setup.cfg` & `ec_number_prediction-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ec_number_prediction
-version = 0.0.4
+version = 0.0.5
 description = ec_number_prediction
 long_description = file: README_pypi.md
 long_description_content_type = text/markdown
 keywords = plants, secondary metabolism
 author = Joao Capela
 license = MIT
 license_file = LICENSE
```

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/_utils.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/_utils.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/download_uniprot.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/download_uniprot.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/filter_uniref.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/filter_uniref.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/n_classes_removal.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/n_classes_removal.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/scrape_uniprot.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/scrape_uniprot.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/split.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/split.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from logging import Logger
 import logging
 import os
+from typing import Any, Tuple
 import luigi
 import numpy as np
 import pandas as pd
 
 from skmultilearn.model_selection import IterativeStratification
 
 from ec_number_prediction.data_processing_pipeline.n_classes_removal import NClassesRemoval
@@ -27,27 +28,72 @@
                 luigi.LocalTarget('splits/validation.csv'),
                 luigi.LocalTarget('splits/before_split_dataset_stats_test.html'),
                 luigi.LocalTarget('splits/after_split_dataset_stats_test.html'),
                 luigi.LocalTarget('splits/before_split_dataset_stats_final.html'),
                 luigi.LocalTarget('splits/after_split_dataset_stats_final.html')
                 ]
     
-    def apply_stratification_sklearn(self, X, y, test_size=0.15, train_size=0.85):
+    def apply_stratification_sklearn(self, X: np.ndarray, y: np.ndarray, test_size: float = 0.15, train_size: float = 0.85) -> Tuple[np.ndarray,
+                                                                                                                                     np.ndarray,
+                                                                                                                                     np.ndarray,
+                                                                                                                                     np.ndarray]:
+        """
+        Parameters
+        ----------
+        X : np.ndarray
+            Samples
+        y : np.ndarray
+            Labels
+        test_size : float, optional
+            Size of the test set, by default 0.15
+        train_size : float, optional
+            Size of the train set, by default 0.85
+        
+        Returns
+        -------
+        Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]
+            X_train, y_train, X_test, y_test
+        """
+
         
         stratifier = IterativeStratification(n_splits=2, order=2, sample_distribution_per_fold=[test_size, train_size])
         train_indexes, test_indexes = next(stratifier.split(X, y))
         X_train = X.iloc[train_indexes]
         y_train = y.iloc[train_indexes, :]
 
         X_test = X.iloc[test_indexes]
         y_test = y.iloc[test_indexes, :]
 
         return X_train, y_train, X_test, y_test
     
-    def correct_split(self, X_train, y_train, X_test, y_test, df_with_stats, validation = False):
+    def correct_split(self, X_train: np.ndarray, y_train: np.ndarray, X_test: np.ndarray, y_test: np.ndarray, 
+                      df_with_stats: pd.DataFrame, validation : bool = False) -> Tuple[np.ndarray, np.ndarray, np.ndarray,
+                                                                                        np.ndarray]:
+        """
+        Parameters
+        ----------
+        X_train : np.ndarray
+            Samples of the train set
+        y_train : np.ndarray
+            Labels of the train set
+        X_test : np.ndarray
+            Samples of the test set
+        y_test : np.ndarray
+            Labels of the test set
+        df_with_stats : pd.DataFrame
+            DataFrame with the stats of the split
+        validation : bool, optional
+            If the split is a validation split, by default False
+
+        Returns
+        -------
+        Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]
+            X_train, y_train, X_test, y_test
+        """
+
 
         X_train_copy = X_train.copy()
         y_train_copy = y_train.copy()
         X_test_copy = X_test.copy()
         y_test_copy = y_test.copy()
 
         for i in range(15):
@@ -66,15 +112,30 @@
                 y_test_copy = pd.concat((y_test_copy, y_train_copy.loc[indexes, :]))
 
                 X_train_copy = X_train_copy.drop(indexes)
                 y_train_copy = y_train_copy.drop(indexes)
 
         return X_train_copy, y_train_copy, X_test_copy, y_test_copy
 
-    def generate_stats(self, y_train, y_test, y_val=None):
+    def generate_stats(self, y_train: np.ndarray, y_test: np.ndarray, y_val: np.ndarray=None) -> Tuple[pd.DataFrame, Any]:
+        """
+        Parameters
+        ----------
+        y_train : np.ndarray
+            Labels of the train set
+        y_test : np.ndarray
+            Labels of the test set
+        y_val : np.ndarray, optional
+            Labels of the validation set, by default None
+        
+        Returns
+        -------
+        Tuple[pd.DataFrame, Any]
+            DataFrame with the stats of the split, styled table
+        """
         y_test_sum = np.sum(y_test)
         y_train_sum = np.sum(y_train)
 
         sum_of_all = pd.DataFrame([y_train_sum, y_test_sum], index=["train", "test"])
 
         if y_val is not None:
             y_val_sum = np.sum(y_val)
```

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/underrepresented_labels_removal.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/underrepresented_labels_removal.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/uniprot_xml_parser.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/uniprot_xml_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,12 +120,14 @@
             pd.DataFrame({"accession": protein_accessions,
                         "name": protein_names,
                         "sequence": protein_sequences,
                         "EC": protein_ecs,
                         "lineage": lineages,
                         "species": species,
                         "taxonomy_id": taxonomy_ids}).to_csv(output_filename, index=False)
+            
+
         
 if __name__ == "__main__":
     #UniprotXmlParser("/home/jcapela/uniprot_parsing/tasks/uniprot_sprot.xml.gz", "Embryophyta").parse("swiss_prot_ec_plants.csv")
-    UniprotXmlParser("/home/jcapela/uniprot_parsing/tasks/uniprot_trembl.xml.gz", "Embryophyta").parse("trembl_prot_ec_plants.csv")
-
+    # UniprotXmlParser("/home/jcapela/uniprot_parsing/tasks/uniprot_trembl.xml.gz", "Embryophyta").parse("trembl_prot_ec_plants.csv")
+    pass
```

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/data_processing_pipeline/uniref_xml_parser.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/data_processing_pipeline/uniref_xml_parser.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/ecpick.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/ecpick.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/feature_extraction/generate_features.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/feature_extraction/generate_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,26 +126,26 @@
                     ESMEncoder(esm_function=esm_function, batch_size=1, num_gpus=4)]
 
     # results_name = f"/scratch/jribeiro/results/{esm_function}"
     transform_datasets(transformers, save_folder, dataset_directory=dataset_directory)
 
 
 if __name__ == "__main__":
-    encoding_type = sys.argv[0]
+    encoding_type = sys.argv[1]
 
     if encoding_type == "one_hot":
-        save_folder = sys.argv[1]
-        dataset_directory = sys.argv[2]
+        save_folder = sys.argv[2]
+        dataset_directory = sys.argv[3]
         generate_one_hot_encodings(dataset_directory, save_folder)
     elif encoding_type == "prot_bert":
-        save_folder = sys.argv[1]
-        dataset_directory = sys.argv[2]
-        generate_prot_bert_vectors(save_folder, dataset_directory)
-    elif encoding_type == "esm":
-        esm_function = sys.argv[1]
         save_folder = sys.argv[2]
         dataset_directory = sys.argv[3]
+        generate_prot_bert_vectors(save_folder, dataset_directory)
+    elif encoding_type == "esm":
+        esm_function = sys.argv[2]
+        save_folder = sys.argv[3]
+        dataset_directory = sys.argv[4]
         generate_esm_vectors(esm_function, save_folder, dataset_directory)
 
     else:
         raise ValueError("Invalid encoding type. They can be one_hot, prot_bert or esm."
                          "If you want to use esm, you need to specify the esm function.")
```

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/labels_names.pkl` & `ec_number_prediction-0.0.5/src/ec_number_prediction/labels_names.pkl`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/labels_names_all_data.pkl` & `ec_number_prediction-0.0.5/src/ec_number_prediction/labels_names_all_data.pkl`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/predictions.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/predictions.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/optimize_dnn.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/optimize_dnn.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/pipeline_runner.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/pipeline_runner.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/train_baselines.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/train_baselines.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/train_deep_ec.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/train_deep_ec.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction/train_models/train_dspace.py` & `ec_number_prediction-0.0.5/src/ec_number_prediction/train_models/train_dspace.py`

 * *Files identical despite different names*

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/PKG-INFO` & `ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec_number_prediction
-Version: 0.0.4
+Version: 0.0.5
 Summary: ec_number_prediction
 Author: Joao Capela
 License: MIT
 Keywords: plants,secondary metabolism
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `ec_number_prediction-0.0.4/src/ec_number_prediction.egg-info/SOURCES.txt` & `ec_number_prediction-0.0.5/src/ec_number_prediction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

