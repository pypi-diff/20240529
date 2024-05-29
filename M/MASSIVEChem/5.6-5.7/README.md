# Comparing `tmp/massivechem-5.6.tar.gz` & `tmp/massivechem-5.7.tar.gz`

## Comparing `massivechem-5.6.tar` & `massivechem-5.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.6/MASSIVEChem.yml
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 massivechem-5.6/molecule_image.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.6/project_final.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.6/images/Focused_spectrum.png
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.6/images/Logo.jpg
--rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.6/images/Spectrum_output.png
--rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.6/notebooks/backup.py
--rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 massivechem-5.6/notebooks/molecule_image.png
--rw-r--r--   0        0        0   373004 2020-02-02 00:00:00.000000 massivechem-5.6/notebooks/project_report.ipynb
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/all_in_one.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/calculate_unsaturation.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/double_plot.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/functional_group_display.py
--rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/functional_group_finder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/ionisation_method.py
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/main_function.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/mol_web_show.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/peak_merger.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/peak_sorter.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/smiles_to_3D_plot.py
--rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/spectrum.py
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/spectrum_3D.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.6/scripts/sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0   103310 2020-02-02 00:00:00.000000 massivechem-5.6/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.6/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.6/test/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_SMILEs_interpreter.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_calculate_unsaturation.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_delta_function_plotter.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_double_plot.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_functional_group_display.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_functional_group_finder.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_ionisation_method.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_main_function.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_mol_web_show.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_molecule_list_generator.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_peak_merger.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_peak_sorter.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_smiles_to_3D_plot.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_spectrum.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_spectrum_3D.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 massivechem-5.6/test/test_sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.6/LICENSE.txt
--rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 massivechem-5.6/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.6/pyproject.toml
--rw-r--r--   0        0        0    11385 2020-02-02 00:00:00.000000 massivechem-5.6/PKG-INFO
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.7/MASSIVEChem.yml
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 massivechem-5.7/molecule_image.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.7/project_final.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.7/images/Focused_spectrum.png
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.7/images/Logo.jpg
+-rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.7/images/Spectrum_output.png
+-rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.7/notebooks/backup.py
+-rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 massivechem-5.7/notebooks/molecule_image.png
+-rw-r--r--   0        0        0   373004 2020-02-02 00:00:00.000000 massivechem-5.7/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/calculate_unsaturation.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/double_plot.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/functional_group_display.py
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/ionisation_method.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/main_function.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/peak_sorter.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/spectrum.py
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/spectrum_3D.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.7/scripts/sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0   103493 2020-02-02 00:00:00.000000 massivechem-5.7/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.7/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.7/test/__init__.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_calculate_unsaturation.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_delta_function_plotter.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_double_plot.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_functional_group_display.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_functional_group_finder.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_ionisation_method.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_main_function.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_mol_web_show.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_molecule_list_generator.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_peak_merger.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_peak_sorter.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_smiles_to_3D_plot.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_spectrum.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_spectrum_3D.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 massivechem-5.7/test/test_sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.7/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.7/LICENSE.txt
+-rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 massivechem-5.7/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.7/pyproject.toml
+-rw-r--r--   0        0        0    11377 2020-02-02 00:00:00.000000 massivechem-5.7/PKG-INFO
```

### Comparing `massivechem-5.6/MASSIVEChem.yml` & `massivechem-5.7/MASSIVEChem.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/molecule_image.png` & `massivechem-5.7/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/project_final.yml` & `massivechem-5.7/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/images/Logo.jpg` & `massivechem-5.7/images/Logo.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/images/Spectrum_output.png` & `massivechem-5.7/images/Spectrum_output.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/notebooks/backup.py` & `massivechem-5.7/notebooks/backup.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/notebooks/molecule_image.png` & `massivechem-5.7/notebooks/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/notebooks/project_report.ipynb` & `massivechem-5.7/notebooks/project_report.ipynb`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/SMILEs_interpreter.py` & `massivechem-5.7/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/all_in_one.py` & `massivechem-5.7/scripts/all_in_one.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/calculate_unsaturation.py` & `massivechem-5.7/scripts/calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/delta_function_plotter.py` & `massivechem-5.7/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/double_plot.py` & `massivechem-5.7/scripts/double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/functional_group_display.py` & `massivechem-5.7/scripts/functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/functional_group_finder.py` & `massivechem-5.7/scripts/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/ionisation_method.py` & `massivechem-5.7/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/main_function.py` & `massivechem-5.7/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/mol_web_show.py` & `massivechem-5.7/scripts/mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/molecule_list_generator.py` & `massivechem-5.7/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/peak_merger.py` & `massivechem-5.7/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/peak_sorter.py` & `massivechem-5.7/scripts/peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/smiles_to_3D_plot.py` & `massivechem-5.7/scripts/smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/spectrum.py` & `massivechem-5.7/scripts/spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/spectrum_3D.py` & `massivechem-5.7/scripts/spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/scripts/sulphur_nitrogen_adder.py` & `massivechem-5.7/scripts/sulphur_nitrogen_adder.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         raise ValueError("The fifth argument must be a positive integer")
     if count_S < 0:
         raise ValueError("The sixth argument must be a positive integer")
     if type(count_N) != int:
         raise ValueError("The fifth argument must be an integer")
     if type(count_S) != int:
         raise ValueError("The sixth argument must be an integer")
+    if type(x_in) != list:
+        raise ValueError("The first argument must be a list")
+    if type(y_in) != list:
+        raise ValueError("The second argument must be a list")
 
 
     maximum = max(y_in)
 
     if has_N:
         x_in.append(x_in[1] - 0.006)  
         y_in.append(0.0035*count_N*maximum)
```

### Comparing `massivechem-5.6/scripts/sulphur_nitrogen_finder.py` & `massivechem-5.7/scripts/sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/src/MASSiveChem/MASSiveChem.py` & `massivechem-5.7/src/MASSiveChem/MASSiveChem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1598,14 +1598,18 @@
         raise ValueError("The fifth argument must be a positive integer")
     if count_S < 0:
         raise ValueError("The sixth argument must be a positive integer")
     if type(count_N) != int:
         raise ValueError("The fifth argument must be an integer")
     if type(count_S) != int:
         raise ValueError("The sixth argument must be an integer")
+    if type(x_in) != list:
+        raise ValueError("The first argument must be a list")
+    if type(y_in) != list:
+        raise ValueError("The second argument must be a list")
 
 
     maximum = max(y_in)
 
     if has_N:
         x_in.append(x_in[1] - 0.006)  
         y_in.append(0.0035*count_N*maximum)
```

### Comparing `massivechem-5.6/test/test_SMILEs_interpreter.py` & `massivechem-5.7/test/test_SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_calculate_unsaturation.py` & `massivechem-5.7/test/test_calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_delta_function_plotter.py` & `massivechem-5.7/test/test_delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_double_plot.py` & `massivechem-5.7/test/test_double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_functional_group_display.py` & `massivechem-5.7/test/test_functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_functional_group_finder.py` & `massivechem-5.7/test/test_functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_ionisation_method.py` & `massivechem-5.7/test/test_ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_main_function.py` & `massivechem-5.7/test/test_main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_mol_web_show.py` & `massivechem-5.7/test/test_mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_molecule_list_generator.py` & `massivechem-5.7/test/test_molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_peak_merger.py` & `massivechem-5.7/test/test_peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_peak_sorter.py` & `massivechem-5.7/test/test_peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_smiles_to_3D_plot.py` & `massivechem-5.7/test/test_smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_spectrum.py` & `massivechem-5.7/test/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_spectrum_3D.py` & `massivechem-5.7/test/test_spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/test/test_sulphur_nitrogen_adder.py` & `massivechem-5.7/test/test_sulphur_nitrogen_adder.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,11 +64,11 @@
 
     def test_no_atoms(self):
         with self.assertRaises(ValueError):
             MC.sulphur_nitrogen_adder([],[], True, True, 2, 2)
     
     def test_not_a_list(self):
         with self.assertRaises(ValueError):
-            MC.sulphur_nitrogen_adder("NSS", "NNS", True, True, 2, 2)
+            MC.sulphur_nitrogen_adder(['NNS'], ['NNS'], True, True, 2, 2)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `massivechem-5.6/test/test_sulphur_nitrogen_finder.py` & `massivechem-5.7/test/test_sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/.gitignore` & `massivechem-5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/LICENSE.txt` & `massivechem-5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-5.6/README.md` & `massivechem-5.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 ```bash
 pip show MASSIVEChem
 ```
 You can then compare the version that you have downloaded to that of the newest available version, which can be found on the PiPy page, https://pypi.org/project/MASSIVEChem/
 
 Then, if the version donwloaded is not the newest one, type the following command into the terminal:
 ```bash
-pip install MASSIVEChem -- upgrade
+pip install MASSIVEChem -U
 ```
 
 If problems persist, please feel free to contact any of the developpers for the package.
 
 
 
 ## Getting started
```

### Comparing `massivechem-5.6/pyproject.toml` & `massivechem-5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 4d41 5353 4956 4543 6865 6d22 0d0a   "MASSIVEChem"..
-00000070: 7665 7273 696f 6e20 3d20 2235 2e36 220d  version = "5.6".
+00000070: 7665 7273 696f 6e20 3d20 2235 2e37 220d  version = "5.7".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
```

### Comparing `massivechem-5.6/PKG-INFO` & `massivechem-5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 5.6
+Version: 5.7
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
@@ -179,15 +179,15 @@
 ```bash
 pip show MASSIVEChem
 ```
 You can then compare the version that you have downloaded to that of the newest available version, which can be found on the PiPy page, https://pypi.org/project/MASSIVEChem/
 
 Then, if the version donwloaded is not the newest one, type the following command into the terminal:
 ```bash
-pip install MASSIVEChem -- upgrade
+pip install MASSIVEChem -U
 ```
 
 If problems persist, please feel free to contact any of the developpers for the package.
 
 
 
 ## Getting started
```

