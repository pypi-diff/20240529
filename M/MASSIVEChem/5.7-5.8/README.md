# Comparing `tmp/massivechem-5.7.tar.gz` & `tmp/massivechem-5.8.tar.gz`

## Comparing `massivechem-5.7.tar` & `massivechem-5.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.7/MASSIVEChem.yml
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 massivechem-5.7/molecule_image.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.7/project_final.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.7/images/Focused_spectrum.png
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.7/images/Logo.jpg
--rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.7/images/Spectrum_output.png
--rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.7/notebooks/backup.py
--rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 massivechem-5.7/notebooks/molecule_image.png
--rw-r--r--   0        0        0   373004 2020-02-02 00:00:00.000000 massivechem-5.7/notebooks/project_report.ipynb
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/all_in_one.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/calculate_unsaturation.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/double_plot.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/functional_group_display.py
--rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/functional_group_finder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/ionisation_method.py
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/main_function.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/mol_web_show.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/peak_merger.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/peak_sorter.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/smiles_to_3D_plot.py
--rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/spectrum.py
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/spectrum_3D.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0   103493 2020-02-02 00:00:00.000000 massivechem-5.7/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.7/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.7/test/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_SMILEs_interpreter.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_calculate_unsaturation.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_delta_function_plotter.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_double_plot.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_functional_group_display.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_functional_group_finder.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_ionisation_method.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_main_function.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_mol_web_show.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_molecule_list_generator.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_peak_merger.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_peak_sorter.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_smiles_to_3D_plot.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_spectrum.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_spectrum_3D.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.7/LICENSE.txt
--rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 massivechem-5.7/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.7/pyproject.toml
--rw-r--r--   0        0        0    11377 2020-02-02 00:00:00.000000 massivechem-5.7/PKG-INFO
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.8/MASSIVEChem.yml
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 massivechem-5.8/molecule_image.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.8/project_final.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.8/images/Focused_spectrum.png
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.8/images/Logo.jpg
+-rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.8/images/Spectrum_output.png
+-rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.8/notebooks/backup.py
+-rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 massivechem-5.8/notebooks/molecule_image.png
+-rw-r--r--   0        0        0   373004 2020-02-02 00:00:00.000000 massivechem-5.8/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/calculate_unsaturation.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/double_plot.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/functional_group_display.py
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/ionisation_method.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/main_function.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/peak_sorter.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    29747 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/spectrum.py
+-rw-r--r--   0        0        0    30541 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/spectrum_3D.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0   103489 2020-02-02 00:00:00.000000 massivechem-5.8/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.8/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.8/test/__init__.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_calculate_unsaturation.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_delta_function_plotter.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_double_plot.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_functional_group_display.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_functional_group_finder.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_ionisation_method.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_main_function.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_mol_web_show.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_molecule_list_generator.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_peak_merger.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_peak_sorter.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_smiles_to_3D_plot.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_spectrum.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_spectrum_3D.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.8/LICENSE.txt
+-rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 massivechem-5.8/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.8/pyproject.toml
+-rw-r--r--   0        0        0    11377 2020-02-02 00:00:00.000000 massivechem-5.8/PKG-INFO
```

### Comparing `massivechem-5.7/MASSIVEChem.yml` & `massivechem-5.8/MASSIVEChem.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/molecule_image.png` & `massivechem-5.8/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/project_final.yml` & `massivechem-5.8/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/images/Logo.jpg` & `massivechem-5.8/images/Logo.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/images/Spectrum_output.png` & `massivechem-5.8/images/Spectrum_output.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/notebooks/backup.py` & `massivechem-5.8/notebooks/backup.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/notebooks/molecule_image.png` & `massivechem-5.8/notebooks/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/notebooks/project_report.ipynb` & `massivechem-5.8/notebooks/project_report.ipynb`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/SMILEs_interpreter.py` & `massivechem-5.8/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/all_in_one.py` & `massivechem-5.8/scripts/all_in_one.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/calculate_unsaturation.py` & `massivechem-5.8/scripts/calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/delta_function_plotter.py` & `massivechem-5.8/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/double_plot.py` & `massivechem-5.8/scripts/double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/functional_group_display.py` & `massivechem-5.8/scripts/functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/functional_group_finder.py` & `massivechem-5.8/scripts/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/ionisation_method.py` & `massivechem-5.8/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/main_function.py` & `massivechem-5.8/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/mol_web_show.py` & `massivechem-5.8/scripts/mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/molecule_list_generator.py` & `massivechem-5.8/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/peak_merger.py` & `massivechem-5.8/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/peak_sorter.py` & `massivechem-5.8/scripts/peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/smiles_to_3D_plot.py` & `massivechem-5.8/scripts/smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/scripts/spectrum.py` & `massivechem-5.8/scripts/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 import base64
 from io import BytesIO
 
 
 def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
 
     #tests for wether the input is valid
-    if mol_smi is None:
+    if mol_smi == '':
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
+    if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if imprecision_True_False not in [True, False]:
         raise ValueError('Enter a boolean value')
     if apparatus_resolution < 0:
         raise ValueError('Enter a positive value')
     if type(apparatus_resolution) != float:
         raise ValueError('Enter an integer value')
```

### Comparing `massivechem-5.7/scripts/spectrum_3D.py` & `massivechem-5.8/scripts/spectrum_3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,24 @@
 from xyz2graph import MolGraph, to_plotly_figure
 
 
 
 
 
 def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
+    if mol_smi == '':
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
+    if mol_without_Hs is None:
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
+    if imprecision_True_False not in [True, False]:
+        raise ValueError('Enter a boolean value')
+    if apparatus_resolution < 0:
+        raise ValueError('Enter a positive value')
+    if type(apparatus_resolution) != float:
+        raise ValueError('Enter an integer value')
 
     #lists of the data to facilitise the pip-installability of the package
 
     mol_smi_3D = mol_smi
 
     mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
             136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355,
```

### Comparing `massivechem-5.7/scripts/sulphur_nitrogen_adder.py` & `massivechem-5.8/scripts/sulphur_nitrogen_adder.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Output: two lists:
     1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
     2. ordered list of the probabilities of apparation of each of the molecules
     
     (the mass in list 1 at index i is associated to the probability at index i in list 2)
     '''
     #---------------------------------------------------------------------------------------------#
-
+    
     if not x_in:
         raise ValueError("Enter a non-empty list")
     if not y_in:
         raise ValueError("Enter a non-empty list")
     if len(x_in) != len(y_in):
         raise ValueError("The two lists must have the same length")
     if has_N not in [True, False]:
```

### Comparing `massivechem-5.7/scripts/sulphur_nitrogen_finder.py` & `massivechem-5.8/scripts/sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/src/MASSiveChem/MASSiveChem.py` & `massivechem-5.8/src/MASSiveChem/MASSiveChem.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 #2
 def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
     
     mol_without_Hs = Chem.MolFromSmiles(mol_smi)
 
     #tests for wether the input is valid
-    if mol_smi is None:
+    if mol_smi == '':
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if imprecision_True_False not in [True, False]:
         raise ValueError('Enter a boolean value')
     if apparatus_resolution < 0:
         raise ValueError('Enter a positive value')
@@ -623,15 +623,15 @@
 
     last = column(img_div, func_group_table)
     final = row(double_graph, last)
     return final
 
 #3
 def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
-    if mol_smi is None:
+    if mol_smi == '':
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if imprecision_True_False not in [True, False]:
         raise ValueError('Enter a boolean value')
     if apparatus_resolution < 0:
         raise ValueError('Enter a positive value')
```

### Comparing `massivechem-5.7/test/test_SMILEs_interpreter.py` & `massivechem-5.8/test/test_SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_calculate_unsaturation.py` & `massivechem-5.8/test/test_calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_delta_function_plotter.py` & `massivechem-5.8/test/test_delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_double_plot.py` & `massivechem-5.8/test/test_double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_functional_group_display.py` & `massivechem-5.8/test/test_functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_functional_group_finder.py` & `massivechem-5.8/test/test_functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_ionisation_method.py` & `massivechem-5.8/test/test_ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_main_function.py` & `massivechem-5.8/test/test_main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_mol_web_show.py` & `massivechem-5.8/test/test_mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_molecule_list_generator.py` & `massivechem-5.8/test/test_molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_peak_merger.py` & `massivechem-5.8/test/test_peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_peak_sorter.py` & `massivechem-5.8/test/test_peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_smiles_to_3D_plot.py` & `massivechem-5.8/test/test_smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/test/test_spectrum.py` & `massivechem-5.8/test/test_spectrum.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         result = MC.spectrum(mol_smi, imprecision_True_False, self.apparatus_resolution)
         self.assertIsNotNone(result)
 
     def test_empty_input(self):
         
         with self.assertRaises(ValueError):
             imprecision_True_False= False
-            MC.spectrum("",imprecision_True_False, self.apparatus_resolution)
+            MC.spectrum_3D("",imprecision_True_False, self.apparatus_resolution)
 
     def test_invalid_input(self):
         
         with self.assertRaises(ValueError):
             imprecision_True_False = False
             MC.spectrum("invalid_smiles",imprecision_True_False, self.apparatus_resolution)
```

### Comparing `massivechem-5.7/test/test_spectrum_3D.py` & `massivechem-5.8/test/test_spectrum_3D.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,20 +14,14 @@
     
     def test_butane_True(self):
         mol_smi = "CCCC"
         imprecision_True_False = True
         result = MC.spectrum_3D(mol_smi, imprecision_True_False, self.apparatus_resolution)
         self.assertIsNotNone(result)
 
-    def test_empty_input(self):
-        
-        with self.assertRaises(ValueError):
-            imprecision_True_False= False
-            MC.spectrum_3D("",imprecision_True_False, self.apparatus_resolution)
-
     def test_invalid_input(self):
         
         with self.assertRaises(ValueError):
             imprecision_True_False = False
             MC.spectrum_3D("invalid_smiles",imprecision_True_False, self.apparatus_resolution)
```

### Comparing `massivechem-5.7/test/test_sulphur_nitrogen_adder.py` & `massivechem-5.8/test/test_sulphur_nitrogen_adder.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,11 +64,11 @@
 
     def test_no_atoms(self):
         with self.assertRaises(ValueError):
             MC.sulphur_nitrogen_adder([],[], True, True, 2, 2)
     
     def test_not_a_list(self):
         with self.assertRaises(ValueError):
-            MC.sulphur_nitrogen_adder(['NNS'], ['NNS'], True, True, 2, 2)
+            MC.sulphur_nitrogen_adder('NNS', 'NNS', True, True, 2, 2)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `massivechem-5.7/test/test_sulphur_nitrogen_finder.py` & `massivechem-5.8/test/test_sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/.gitignore` & `massivechem-5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/LICENSE.txt` & `massivechem-5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/README.md` & `massivechem-5.8/README.md`

 * *Files identical despite different names*

### Comparing `massivechem-5.7/pyproject.toml` & `massivechem-5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 4d41 5353 4956 4543 6865 6d22 0d0a   "MASSIVEChem"..
-00000070: 7665 7273 696f 6e20 3d20 2235 2e37 220d  version = "5.7".
+00000070: 7665 7273 696f 6e20 3d20 2235 2e38 220d  version = "5.8".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
```

### Comparing `massivechem-5.7/PKG-INFO` & `massivechem-5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 5.7
+Version: 5.8
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
```

