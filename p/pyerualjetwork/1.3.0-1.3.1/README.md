# Comparing `tmp/pyerualjetwork-1.3.0.tar.gz` & `tmp/pyerualjetwork-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.3.0.tar", last modified: Tue May 28 20:46:11 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.3.1.tar", last modified: Tue May 28 20:54:26 2024, max compression
```

## Comparing `pyerualjetwork-1.3.0.tar` & `pyerualjetwork-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 20:46:11.074909 pyerualjetwork-1.3.0/
--rw-rw-rw-   0        0        0      421 2024-05-28 20:46:11.073909 pyerualjetwork-1.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-28 20:46:11.051211 pyerualjetwork-1.3.0/plan/
--rw-rw-rw-   0        0        0      352 2024-05-26 16:54:30.000000 pyerualjetwork-1.3.0/plan/__init__.py
--rw-rw-rw-   0        0        0    42347 2024-05-28 20:20:20.000000 pyerualjetwork-1.3.0/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-28 20:46:11.071905 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      421 2024-05-28 20:46:10.000000 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-28 20:46:10.000000 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 20:46:10.000000 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-28 20:46:10.000000 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 20:46:11.075904 pyerualjetwork-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-28 20:46:04.000000 pyerualjetwork-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:54:26.655541 pyerualjetwork-1.3.1/
+-rw-rw-rw-   0        0        0      421 2024-05-28 20:54:26.654545 pyerualjetwork-1.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 20:54:26.629903 pyerualjetwork-1.3.1/plan/
+-rw-rw-rw-   0        0        0      352 2024-05-26 16:54:30.000000 pyerualjetwork-1.3.1/plan/__init__.py
+-rw-rw-rw-   0        0        0    42343 2024-05-28 20:54:14.000000 pyerualjetwork-1.3.1/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:54:26.651323 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      421 2024-05-28 20:54:26.000000 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-28 20:54:26.000000 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 20:54:26.000000 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-28 20:54:26.000000 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 20:54:26.656539 pyerualjetwork-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-28 20:53:36.000000 pyerualjetwork-1.3.1/setup.py
```

### Comparing `pyerualjetwork-1.3.0/plan/plan.py` & `pyerualjetwork-1.3.1/plan/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,16 +203,16 @@
         
         if Visualize == 'y':
         
             TrainLabelsVisual = np.copy(TrainLabels) 
             TrainLabelsVisual = np.argmax(TrainLabelsVisual, axis=1)
             
             plt.figure(figsize=(12, 6))
-            sns.kdeplot(TrainLabelsVisual, label='Real Outputs', shade=True)
-            sns.kdeplot(TrainPredictions, label='Predictions', shade=True)
+            sns.kdeplot(TrainLabelsVisual, label='Real Outputs', fill=True)
+            sns.kdeplot(TrainPredictions, label='Predictions', fill=True)
             plt.legend()
             plt.xlabel('Class')
             plt.ylabel('Data size')
             plt.title('Predictions and Real Outputs for Training KDE Plot')
             plt.show()
             
             if index + 1 != len(TrainInputs):
@@ -627,16 +627,16 @@
             
             if Visualize == 'y':
             
                 TestLabelsVisual = np.copy(TestLabels) 
                 TestLabelsVisual = np.argmax(TestLabelsVisual, axis=1)
                 
                 plt.figure(figsize=(12, 6))
-                sns.kdeplot(TestLabelsVisual, label='Real Outputs', shade=True)
-                sns.kdeplot(TestPredictions, label='Predictions', shade=True)
+                sns.kdeplot(TestLabelsVisual, label='Real Outputs', fill=True)
+                sns.kdeplot(TestPredictions, label='Predictions', fill=True)
                 plt.legend()
                 plt.xlabel('Class')
                 plt.ylabel('Data size')
                 plt.title('Predictions and Real Outputs for Testing KDE Plot')
                 plt.show()
                 
                 if inpIndex + 1 != len(TestInputs):
```

### Comparing `pyerualjetwork-1.3.0/setup.py` & `pyerualjetwork-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.3.0",
+      version = "1.3.1",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library. New Visualize parameter added ('y' or 'n') for TrainPLAN and TestPLAN funcs. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
```

