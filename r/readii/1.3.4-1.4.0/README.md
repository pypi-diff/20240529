# Comparing `tmp/readii-1.3.4.tar.gz` & `tmp/readii-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readii-1.3.4.tar", max compression
+gzip compressed data, was "readii-1.4.0.tar", max compression
```

## Comparing `readii-1.3.4.tar` & `readii-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1069 2024-05-16 21:18:47.034889 readii-1.3.4/LICENSE
--rw-r--r--   0        0        0     2096 2024-05-16 21:18:47.034889 readii-1.3.4/README.md
--rw-r--r--   0        0        0     1450 2024-05-16 21:19:08.494909 readii-1.3.4/pyproject.toml
--rw-r--r--   0        0        0      100 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/data/__init__.py
--rw-r--r--   0        0        0      299 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/data/default_pyradiomics.yaml
--rw-r--r--   0        0        0    14813 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/feature_extraction.py
--rw-r--r--   0        0        0    12227 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/image_processing.py
--rw-r--r--   0        0        0     4192 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/loaders.py
--rw-r--r--   0        0        0     5959 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/metadata.py
--rw-r--r--   0        0        0    24474 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/negative_controls.py
--rw-r--r--   0        0        0     6126 2024-05-16 21:18:47.038889 readii-1.3.4/src/readii/pipeline.py
--rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 readii-1.3.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2024-05-29 20:05:18.366644 readii-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2096 2024-05-29 20:05:18.366644 readii-1.4.0/README.md
+-rw-r--r--   0        0        0     1450 2024-05-29 20:05:41.634602 readii-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/data/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/data/default_pyradiomics.yaml
+-rw-r--r--   0        0        0    15195 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/feature_extraction.py
+-rw-r--r--   0        0        0    12227 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/image_processing.py
+-rw-r--r--   0        0        0     4192 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/loaders.py
+-rw-r--r--   0        0        0     5959 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/metadata.py
+-rw-r--r--   0        0        0    24474 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/negative_controls.py
+-rw-r--r--   0        0        0     6365 2024-05-29 20:05:18.370644 readii-1.4.0/src/readii/pipeline.py
+-rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 readii-1.4.0/PKG-INFO
```

### Comparing `readii-1.3.4/LICENSE` & `readii-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readii-1.3.4/README.md` & `readii-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `readii-1.3.4/pyproject.toml` & `readii-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readii"
-version = "1.3.4"
+version = "1.4.0"
 description = "A package to extract radiomic features!"
 authors = ["Katy Scott"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
```

### Comparing `readii-1.3.4/src/readii/feature_extraction.py` & `readii-1.4.0/src/readii/feature_extraction.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,29 +46,32 @@
 from collections import OrderedDict
 
 def singleRadiomicFeatureExtraction(
     ctImage: sitk.Image,
     roiImage: sitk.Image,
     pyradiomicsParamFilePath: str = "./src/readii/data/default_pyradiomics.yaml",
     negativeControl: Optional[str] = None,
+    randomSeed: Optional[int] = None,
 ) -> OrderedDict[Any, Any]:
     """Function to perform radiomic feature extraction for a single CT image and its corresponding segmentation.
        CT and segmentation will be aligned and cropped prior to extraction.
 
     Parameters
     ----------
     ctImage : sitk.Image
         CT image to perform feature extraction on. Will be cropped and potentially generate a negative control (see negativeControl arg)
     roiImage : sitk.Image
         Region of interest (ROI) to extract radiomic features from within the CT.
     pyradiomicsParamFilePath : str
         Path to file containing configuration settings for pyradiomics feature extraction. Will use the provided config file in 'data/' by default if no file passed in.
     negativeControl : str
         Name of negative control to generate from the CT to perform feature extraction on. If set to None, will extract features from original CT image.
-
+    randomSeed : int
+        Value to set random seed with for negative control creation to be reproducible.
+        
     Returns
     -------
     OrderedDict[Any, Any]
         Dictionary containing image metadata, versions for key packages used for extraction, and radiomic features
     """
     # If no pyradiomics paramater file passed, use default
     if pyradiomicsParamFilePath == None:
@@ -96,14 +99,15 @@
         print("Generating ", negativeControl, "negative control for CT.")
         # Make negative control version of ctImage
         croppedCT = applyNegativeControl(
             nc_type=negativeControl,
             baseImage=croppedCT,
             baseROI=croppedROI,
             roiLabel=segmentationLabel,
+            randomSeed=randomSeed
         )
 
     # Load PyRadiomics feature extraction parameters to use
     # Initialize feature extractor with parameters
     try:
         featureExtractor = featureextractor.RadiomicsFeatureExtractor(pyradiomicsParamFilePath)
     except OSError as e:
@@ -121,14 +125,15 @@
 def radiomicFeatureExtraction(
     imageMetadataPath: str,
     imageDirPath: str,
     roiNames: Optional[str] = None,
     pyradiomicsParamFilePath: str = "src/readii/data/default_pyradiomics.yaml",
     outputDirPath: Optional[str] = None,
     negativeControl: Optional[str] = None,
+    randomSeed: Optional[int] = None,
     parallel: bool = False,
 ) -> pd.DataFrame:
     """Perform radiomic feature extraction using PyRadiomics on CT images with a corresponding segmentation.
        Utilizes outputs from med-imagetools (https://github.com/bhklab/med-imagetools) run on the image dataset.
 
     Parameters
     ----------
@@ -141,14 +146,16 @@
         Name pattern for the ROIs to load for the RTSTRUCTs. Can be None for DICOM SEG segmentations.
     pyradiomicsParamFilePath : str
         Path to file containing configuration settings for pyradiomics feature extraction. Will use the provided config file in 'data/' by default if no file passed in.
     outputDirPath : str
         Path to directory save the dataframe of extracted features to as a csv
     negativeControl : str
         Name of negative control to generate from the CT to perform feature extraction on. If set to None, will extract features from original CT image.
+    randomSeed : int
+        Value to set random seed with for negative control creation to be reproducible.
     parallel : bool
         Flag to decide whether to run extraction in parallel.
 
     Returns
     -------
     pd.DataFrame
         Dataframe containing the image metadata and extracted radiomic features.
@@ -265,14 +272,15 @@
 
                     # Extract radiomic features from this CT/segmentation pair
                     idFeatureVector = singleRadiomicFeatureExtraction(
                         ctImage,
                         roiImage=roiImage,
                         pyradiomicsParamFilePath=pyradiomicsParamFilePath,
                         negativeControl=negativeControl,
+                        randomSeed=randomSeed
                     )
 
                     # Create dictionary of image metadata to append to front of output table
                     sampleROIData = {
                         "patient_ID": patID,
                         "study_description": segSeriesInfo.iloc[0][
                             "study_description_CT"
```

### Comparing `readii-1.3.4/src/readii/image_processing.py` & `readii-1.4.0/src/readii/image_processing.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.4/src/readii/loaders.py` & `readii-1.4.0/src/readii/loaders.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.4/src/readii/metadata.py` & `readii-1.4.0/src/readii/metadata.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.4/src/readii/negative_controls.py` & `readii-1.4.0/src/readii/negative_controls.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.4/src/readii/pipeline.py` & `readii-1.4.0/src/readii/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,17 @@
                               Options: randomized_full,randomized_roi,randomized_non_roi,shuffled_full,shuffled_roi,shuffled_non_roi,randomized_sampled_full,randomized_sampled_roi,randomized_sampled_non_roi")
 
     parser.add_argument("--parallel", action="store_true",
                         help="Whether to run feature extraction in a parallel process. False by default.")
 
     parser.add_argument("--update", action="store_true", help="Flag to force rerun all steps of pipeline. False by default.")
 
+    parser.add_argument("--random_seed", type=int,
+                        help="Value to set random seed to for reproducible negative controls")
+
     return parser.parse_known_args()[0]
     
 
 def main():
     """Function to run READII radiomic feature extraction pipeline.
     """
     args = parser()
@@ -103,14 +106,15 @@
                 print("Starting radiomic feature extraction for negative control: ", negativeControl)
                 ncRadiomicFeatures = radiomicFeatureExtraction(imageMetadataPath = imageMetadataPath,
                                                                imageDirPath = parentDirPath,
                                                                roiNames = args.roi_names,
                                                                pyradiomicsParamFilePath = args.pyradiomics_setting,
                                                                outputDirPath = outputDir,
                                                                negativeControl = negativeControl,
+                                                               randomSeed=args.random_seed,
                                                                parallel = args.parallel)
             else:
                 print(negativeControl, " radiomic features have already been extracted. See ", ncRadFeatOutPath)
 
     
     print("Pipeline complete.")
```

### Comparing `readii-1.3.4/PKG-INFO` & `readii-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readii
-Version: 1.3.4
+Version: 1.4.0
 Summary: A package to extract radiomic features!
 License: MIT
 Author: Katy Scott
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

