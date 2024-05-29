# Comparing `tmp/massivechem-5.4.tar.gz` & `tmp/massivechem-5.5.tar.gz`

## Comparing `massivechem-5.4.tar` & `massivechem-5.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.4/MASSIVEChem.yml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.4/project_final.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.4/images/Focused_spectrum.png
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.4/images/Logo.jpg
--rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.4/images/Spectrum_output.png
--rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.4/notebooks/backup.py
--rw-r--r--   0        0        0     9376 2020-02-02 00:00:00.000000 massivechem-5.4/notebooks/molecule_image.png
--rw-r--r--   0        0        0   216605 2020-02-02 00:00:00.000000 massivechem-5.4/notebooks/project_report.ipynb
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/all_in_one.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/calculate_unsaturation.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/double_plot.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/functional_group_display.py
--rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/functional_group_finder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/ionisation_method.py
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/main_function.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/mol_web_show.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/peak_merger.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/peak_sorter.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/smiles_to_3D_plot.py
--rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/spectrum.py
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/spectrum_3D.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0   103206 2020-02-02 00:00:00.000000 massivechem-5.4/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.4/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.4/test/__init__.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_SMILEs_interpreter.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_calculate_unsaturation.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_delta_function_plotter.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_double_plot.py
--rw-r--r--   0        0        0     7670 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_functional_group_display.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_functional_group_finder.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_ionisation_method.py
--rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_main_function.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_mol_web_show.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_molecule_list_generator.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_peak_merger.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_peak_sorter.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_smiles_to_3D_plot.py
--rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_spectrum.py
--rw-r--r--   0        0        0    31039 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_spectrum_3D.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.4/LICENSE.txt
--rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 massivechem-5.4/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.4/pyproject.toml
--rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 massivechem-5.4/PKG-INFO
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.5/MASSIVEChem.yml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.5/project_final.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.5/images/Focused_spectrum.png
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.5/images/Logo.jpg
+-rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.5/images/Spectrum_output.png
+-rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.5/notebooks/backup.py
+-rw-r--r--   0        0        0     9376 2020-02-02 00:00:00.000000 massivechem-5.5/notebooks/molecule_image.png
+-rw-r--r--   0        0        0   216605 2020-02-02 00:00:00.000000 massivechem-5.5/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/calculate_unsaturation.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/double_plot.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/functional_group_display.py
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/ionisation_method.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/main_function.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/peak_sorter.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/spectrum.py
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/spectrum_3D.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.5/scripts/sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0   103297 2020-02-02 00:00:00.000000 massivechem-5.5/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.5/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.5/test/__init__.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_calculate_unsaturation.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_delta_function_plotter.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_double_plot.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_functional_group_display.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_functional_group_finder.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_ionisation_method.py
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_main_function.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_mol_web_show.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_molecule_list_generator.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_peak_merger.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_peak_sorter.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_spectrum.py
+-rw-r--r--   0        0        0    31039 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_spectrum_3D.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.5/test/test_sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.5/LICENSE.txt
+-rw-r--r--   0        0        0    10213 2020-02-02 00:00:00.000000 massivechem-5.5/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.5/pyproject.toml
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 massivechem-5.5/PKG-INFO
```

### Comparing `massivechem-5.4/MASSIVEChem.yml` & `massivechem-5.5/MASSIVEChem.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/project_final.yml` & `massivechem-5.5/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/images/Logo.jpg` & `massivechem-5.5/images/Logo.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/images/Spectrum_output.png` & `massivechem-5.5/images/Spectrum_output.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/notebooks/backup.py` & `massivechem-5.5/notebooks/backup.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/notebooks/molecule_image.png` & `massivechem-5.5/notebooks/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/notebooks/project_report.ipynb` & `massivechem-5.5/notebooks/project_report.ipynb`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/SMILEs_interpreter.py` & `massivechem-5.5/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/all_in_one.py` & `massivechem-5.5/scripts/all_in_one.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/calculate_unsaturation.py` & `massivechem-5.5/scripts/calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/delta_function_plotter.py` & `massivechem-5.5/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/double_plot.py` & `massivechem-5.5/scripts/double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/functional_group_display.py` & `massivechem-5.5/scripts/functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/functional_group_finder.py` & `massivechem-5.5/scripts/functional_group_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,19 @@
     
     Output: list containing every functionl group contained (if a functional group is contained twice in the molecule, it will appear twice in this list)
     '''
     #---------------------------------------------------------------------------------------------#
 
     if not mol_smi:
         raise ValueError("Enter a non-empty string as argument")
+    if not Chem.MolFromSmiles(mol_smi):
+        raise ValueError("Enter correct SMILEs")
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
-    if not mol_in:
-        raise ValueError('Incorrect SMILEs input')
-
     # dictionnary of all the considered functional groups to check (some might be missing)
 
     functional_groups_smarts = {
         'Alcohol': 'C[Oh1+0]',
         'Aldehyde': 'C[Ch1]=O',
         'Ketone': 'CC(=O)C',
         'Carboxylic Acid': 'CC(=O)[Oh1]',
```

### Comparing `massivechem-5.4/scripts/ionisation_method.py` & `massivechem-5.5/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/main_function.py` & `massivechem-5.5/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/mol_web_show.py` & `massivechem-5.5/scripts/mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/molecule_list_generator.py` & `massivechem-5.5/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/peak_merger.py` & `massivechem-5.5/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/peak_sorter.py` & `massivechem-5.5/scripts/peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/smiles_to_3D_plot.py` & `massivechem-5.5/scripts/smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/spectrum.py` & `massivechem-5.5/scripts/spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/spectrum_3D.py` & `massivechem-5.5/scripts/spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/sulphur_nitrogen_adder.py` & `massivechem-5.5/scripts/sulphur_nitrogen_adder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/scripts/sulphur_nitrogen_finder.py` & `massivechem-5.5/scripts/sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/src/MASSiveChem/MASSiveChem.py` & `massivechem-5.5/src/MASSiveChem/MASSiveChem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1769,14 +1769,16 @@
     
     Output: list containing every functionl group contained (if a functional group is contained twice in the molecule, it will appear twice in this list)
     '''
     #---------------------------------------------------------------------------------------------#
 
     if not mol_smi:
         raise ValueError("Enter a non-empty string as argument")
+    if not Chem.MolFromSmiles(mol_smi):
+        raise ValueError("Enter correct SMILEs")
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
     # dictionnary of all the considered functional groups to check (some might be missing)
 
     functional_groups_smarts = {'Alcohol': 'C[Oh1+0]','Aldehyde': 'C[Ch1]=O','Ketone': 'CC(=O)C','Carboxylic Acid': 'CC(=O)[Oh1]',
         'Ester': 'CC(=O)[Oh0]','Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[C][N]','Nitrile': 'C#N','Chloride': 'Cl',
```

### Comparing `massivechem-5.4/test/test_SMILEs_interpreter.py` & `massivechem-5.5/test/test_SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_calculate_unsaturation.py` & `massivechem-5.5/test/test_calculate_unsaturation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,42 @@
-from rdkit import Chem
-from rdkit.Chem import Draw
-
-def calculate_unsaturation(mol_smile) -> int:
-    #---------------------------------------------------------------------------------------------#
-    '''
-    calculate_unsaturation(mol_smile)
-
-    Input: molecule under SMILEs representation
-
-    Output: unsaturation of the input molecule (integer value)
-    '''
-    #---------------------------------------------------------------------------------------------# 
-    if mol_smile == None:
-        raise ValueError('Enter a non-empty input')
-    
-    C, N, HX, halogens_hydrogen = 0, 0, 0, ['F', 'Cl', 'Br', 'I', 'At', 'H']
-
-    mol = Chem.AddHs(Chem.MolFromSmiles(mol_smile))
-    
-    if mol == None:
-        raise ValueError('Invalid SMILEs representation')
-    
-    for atom in mol.GetAtoms():
-        if atom.GetSymbol() == 'C':
-            C += 1
-        elif atom.GetSymbol() == 'N':
-            N += 1
-        elif atom.GetSymbol() in halogens_hydrogen:
-            HX += 1
-
-    unsaturation = C + 1 + (N - HX) / 2
-
-    return unsaturation
-
+import MASSiveChem.MASSiveChem as MC
 import unittest
 
 class TestCalculateUnsaturation(unittest.TestCase):
 
     def test_one_unsaturation(self):
 
-        result = calculate_unsaturation("C=C")  
+        result = MC.calculate_unsaturation("C=C")  
         self.assertEqual(result, 1)
 
     def test_nitrogen_and_no_halogens(self):
 
-        result = calculate_unsaturation("CC=O")  
+        result = MC.calculate_unsaturation("CC=O")  
         self.assertEqual(result, 1)
 
     def test_nitrogen_and_halogens(self):
 
-        result = calculate_unsaturation("CNC(Cl)Br")  
+        result = MC.calculate_unsaturation("CNC(Cl)Br")  
         self.assertEqual(result, 0)
 
     def test_multiple_nitrogen_and_halogens(self):
 
-        result = calculate_unsaturation("BrC=CC(Br)(Cl)CC(N)CCN") 
+        result = MC.calculate_unsaturation("BrC=CC(Br)(Cl)CC(N)CCN") 
         self.assertEqual(result, 1)
 
     def test_multiple_unsaturations(self):
 
-        result = calculate_unsaturation("C1=CC=CC=C1") 
+        result = MC.calculate_unsaturation("C1=CC=CC=C1") 
         self.assertEqual(result, 4)
 
     def test_no_atoms(self):
 
-        result = calculate_unsaturation("") 
+        result = MC.calculate_unsaturation("") 
         self.assertEqual(result, 1)
 
     def test_no_nitrogen_and_halogens(self):
 
-        result = calculate_unsaturation("CCCl")
+        result = MC.calculate_unsaturation("CCCl")
         self.assertEqual(result, 0)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `massivechem-5.4/test/test_ionisation_method.py` & `massivechem-5.5/test/test_ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_main_function.py` & `massivechem-5.5/test/test_main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_mol_web_show.py` & `massivechem-5.5/test/test_mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_molecule_list_generator.py` & `massivechem-5.5/test/test_molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_peak_merger.py` & `massivechem-5.5/test/test_peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_peak_sorter.py` & `massivechem-5.5/test/test_peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_smiles_to_3D_plot.py` & `massivechem-5.5/test/test_smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_spectrum.py` & `massivechem-5.5/test/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_spectrum_3D.py` & `massivechem-5.5/test/test_spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_sulphur_nitrogen_adder.py` & `massivechem-5.5/test/test_sulphur_nitrogen_adder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/test/test_sulphur_nitrogen_finder.py` & `massivechem-5.5/test/test_sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/.gitignore` & `massivechem-5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/LICENSE.txt` & `massivechem-5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-5.4/README.md` & `massivechem-5.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,155 +1,200 @@
-<img width="830" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Logo.jpg">
-
-[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
-[![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
-![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
-[![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
-
-
-# -         MASSIVEChem       - 
-
-[![GitHub2](https://img.shields.io/badge/Maintained%3F-yes-turquoise.svg)](https://pypi.org/user/Arthur.hmy/)
-[![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=orange)](https://www.python.org)
-[![GitHub3](https://img.shields.io/badge/Contributors-3-green.svg)](https://github.com/ThomasCsson/MASSIVEChem/graphs/contributors)
-[![GitHub3](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
-[![GitHub3](https://img.shields.io/badge/EPFL-CH200-red.svg)](https://edu.epfl.ch/studyplan/en/bachelor/chemistry-and-chemical-engineering/coursebook/practical-programming-in-chemistry-CH-200)
-
-
- - Python package for applied analytical chemistry focused primarily on mass speectrometry 
-#### Project within _practical programming in chemistry_ course -- EPFL CH-200
-
-## Package description
-[![GitHub3](http://ForTheBadge.com/images/badges/built-with-science.svg)](https://x.com/pschwllr/status/1760713822111723990)
-[![GitHub4](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-
-MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable python package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
-The aim of this package is to provide the user with functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
-
-Developpers:
-- Thomas Viking Christiansson, student in chemical engineering at EPFL    [![jhc github](https://img.shields.io/badge/GitHub-ThomasCsson-181717.svg?style=flat&logo=github)](https://github.com/ThomasCsson)
-- Igor Gonteri, student in chemistry at EPFL                             [![jhc github](https://img.shields.io/badge/GitHub-igorgonteri-181717.svg?style=flat&logo=github)](https://github.com/igorgonteri)
-- Arthur Humery, student in chemical engineering at EPFL                [![jhc github](https://img.shields.io/badge/GitHub-Arthurhmy-181717.svg?style=flat&logo=github)](https://github.com/Arthurhmy)
-
-### What is mass spectrometry ?
-
-Mass spectrometry (MS) is an analytical technique used to measure the mass-to-charge ratio of ions. It helps identify the structure of the chemical compound present in a sample by generating a spectrum of the masses of its ions. The process involves three main steps:
-
-Ionisation: The sample is ionised, which means its molecules are converted into charged particles (ions). This can be done using various methods, such as electron impact (EI), electrospray ionisation (ESI), or matrix-assisted laser desorption/ionisation (MALDI). In this case, the ionisation is set to the most commonly used method; deprotonation.
-
-Mass Analysis: The ions are separated based on their mass-to-charge ratio (m/z). This is usually done using a mass analyser, such as a quadrupole, time-of-flight (TOF), or an ion trap. Each type of mass analyser works differently but ultimately serves to distinguish ions by their specific m/z values. The unit of these m/z values is 1 Th or 1 $\frac{Da}{e}$.
-
-On the y axis of the output spectrum, the relative abundance of the different ions is plotted. This abundance is given by the different natural abundances of the different isotopes of the atoms in the molecule. For example, the relative abundance of $^{13}C$ is 1.1% and that of $^{12}C$ is 98.9%.
-
-Mass spectrometry is widely used in various fields, including:
-
-Chemistry: For molecular identification and structural elucidation. Biochemistry: For studying proteins, peptides, and other biomolecules. Pharmaceuticals: For drug development and metabolite analysis. Environmental Science: For detecting pollutants and analysing environmental samples. Clinical Diagnostics: For identifying biomarkers and analysing complex biological samples. The technique's sensitivity, accuracy, and ability to analyse complex mixtures make it an essential tool in both research and applied sciences.
-
-Now, let us go through the steps required to use this package!
-
-## Installation
-[![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/MASSIVEChem/)
-
-MASSIVEChem can be installed using pip as
-```bash
-pip install MASSIVEChem
-```
-
-
-[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem?tab=readme-ov-file)
-
-Alternatively, the package can be directly installed from the GitHub repository via pip using the following command in the terminal
-```bash
-pip install git+https://github.com/ThomasCsson/MASSIVEChem
-```
-
-
-![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
-
-The package can also be installed from source by running the following commands
-
-First, clone the repository from github and go in the folder. 
-```bash
-git clone https://github.com/ThomasCsson/MASSIVEChem.git
-cd path/to/MASSIVEChem
-```
-Then, install the package using : 
-```bash
-pip install -e .
-```
-
-## Requirments
-The package runs on python 3.10 but supports python 3.8 through 3.10.
-It requires several other packages to function correctly.
-
-```bash
-bokeh
-rdkit
-panel
-```
-
-(Note: panel is not directly used, but is required for added functionality involving the 3 dimmensinal visualisation of the input molecule)
-
-If all goes well during installation, the preceding packages should all install automatically.
-But this can be checked by veryfying that they have all been installed in the desired environment. To do this, simply write the following command in the terminal:
-
-```bash
-pip show "name of the package"
-```
-
-If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
-
-```bash
-pip install bokeh
-pip install rdkit
-pip install panel
-```
-Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourself, the following command needs to be run.
-
-```bash
-python -m pip install git+https://github.com/zotko/xyz2graph.git
-```
-
-
-## Usage
-
-The principal function of this package takes the SMILEs of a molecule as an input and displays the mass spectrometry of the molecule as well as the molecule itself and  the functional groups it contains.
-
-An example on how to make the function work is shown below for benzylpenicilin:
-
-The ionization method is set to monodeprotonation and the resolution of the apparatus is 0.01 Th
-
-```bash
-import MASSIVEChem.MASSIVEChem as MC
-from bokeh.plotting import show
-
-mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
-apparatus_resolution = 0.01
-
-show(MC.spectrum(mol_smi, True, apparatus_resolution))
-
-
-#The first input in MC.spectrum is the molecule under SMILEs representation,
-#and the third is the resolution of the apparatus (typically, this value is of 0.01)
-#the second computes an approximate spectrum if True and the precise spectrum if False
-
-```
-
-The output of this command will be:
-
-<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Spectrum_output.png">
-
-Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
-
-<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
-
-## Getting started
-[![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
-
-To begin to use the package the following jupyter notebook will give you information about all the package's functions:
-
-[![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-orange.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/notebooks/project_report.ipynb)
-
-## Fun !
-🐰 If you've made it this far through our project, you might want to try to find the hidden easter egg in this ReadMe :)🐰
-
-(_hint: you might want to try clicking on various badges throughout the ReadMe_)
+Metadata-Version: 2.3
+Name: MASSIVEChem
+Version: 5.5
+Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
+Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
+Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
+Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
+Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
+Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
+License-Expression: MIT
+License-File: LICENSE.txt
+Keywords: Mass spectroscopy,chemical-engineering,chemical-property-prediction,cheminformatics,chemistry,chemistry-lab,functional group,spectrometry,spectroscopy,unsaturation
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Requires-Dist: bokeh
+Requires-Dist: panel
+Requires-Dist: rdkit
+Description-Content-Type: text/markdown
+
+<img width="830" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Logo.jpg">
+
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
+[![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
+![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
+[![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
+
+
+# -         MASSIVEChem       - 
+
+[![GitHub2](https://img.shields.io/badge/Maintained%3F-yes-turquoise.svg)](https://pypi.org/user/Arthur.hmy/)
+[![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=orange)](https://www.python.org)
+[![GitHub3](https://img.shields.io/badge/Contributors-3-green.svg)](https://github.com/ThomasCsson/MASSIVEChem/graphs/contributors)
+[![GitHub3](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
+[![GitHub3](https://img.shields.io/badge/EPFL-CH200-red.svg)](https://edu.epfl.ch/studyplan/en/bachelor/chemistry-and-chemical-engineering/coursebook/practical-programming-in-chemistry-CH-200)
+
+
+ - Python package for applied analytical chemistry focused primarily on mass spectrometry 
+#### Project within _practical programming in chemistry_ course -- EPFL CH-200
+
+## Package description
+[![GitHub3](http://ForTheBadge.com/images/badges/built-with-science.svg)](https://x.com/pschwllr/status/1760713822111723990)
+[![GitHub4](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+
+MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable python package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
+The aim of this package is to provide the user with functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
+
+Developpers:
+- Thomas Viking Christiansson, student in chemical engineering at EPFL    [![jhc github](https://img.shields.io/badge/GitHub-ThomasCsson-181717.svg?style=flat&logo=github)](https://github.com/ThomasCsson)
+- Igor Gonteri, student in chemistry at EPFL                             [![jhc github](https://img.shields.io/badge/GitHub-igorgonteri-181717.svg?style=flat&logo=github)](https://github.com/igorgonteri)
+- Arthur Humery, student in chemical engineering at EPFL                [![jhc github](https://img.shields.io/badge/GitHub-Arthurhmy-181717.svg?style=flat&logo=github)](https://github.com/Arthurhmy)
+
+### What is mass spectrometry ?
+
+Mass spectrometry (MS) is an analytical technique used to measure the mass-to-charge ratio of ions. It helps identify the structure of the chemical compound present in a sample by generating a spectrum of the masses of its ions. The process involves two main steps:
+
+Ionisation: The sample is ionised, which means its molecules are converted into charged particles (ions). This can be done using various methods, such as electron impact (EI), electrospray ionisation (ESI), or matrix-assisted laser desorption/ionisation (MALDI). In this case, the ionisation is set to the most commonly used method; deprotonation.
+
+Mass Analysis: The ions are separated based on their mass-to-charge ratio (m/z). This is usually done using a mass analyser, such as a quadrupole, time-of-flight (TOF), or an ion trap. Each type of mass analyser works differently but ultimately serves to distinguish ions by their specific $\frac{m}{z}$ values. The unit of these $\frac{m}{z}$ values is 1 Th or 1 $\frac{Da}{e}$.
+
+On the y axis of the output spectrum, the relative abundance of the different ions is plotted. This abundance is given by the different natural abundances of the different isotopes of the atoms in the molecule. For example, the relative abundance of $^{13}C$ is 1.1% and that of $^{12}C$ is 98.9%.
+
+Mass spectrometry is widely used in various fields, including:
+
+Chemistry, for molecular identification and structural elucidation. Biochemistry, for studying proteins, peptides, and other biomolecules. Pharmaceuticals, for drug development and metabolite analysis. Environmental Science, for detecting pollutants and analysing environmental samples. Clinical Diagnostics, for identifying biomarkers and analysing complex biological samples. The technique's sensitivity, accuracy, and ability to analyse complex mixtures make it an essential tool in both research and applied sciences.
+
+The mathematical reasoning behind the calculation of these relative abundances is simply applying combinatorics to each isotope of each atom in the given molecule.
+
+To find the probability of a molecule composed of isotopes $I_{1}$ , $I_{2}$ , ... , $I_{n}$ is given by the following formula:
+
+$Pr(I_{1},I_{2},...,I_{n})$ = $Pr(I_{1})$ $\cdot$ $Pr(I_{2})$ $\cdot$ ... $\cdot$ $Pr(I_{n})$
+
+This probability is then the relative abundance of the molecule composed of those isotopes.
+
+Now, let us go through the steps required to use this package!
+
+## Installation
+[![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/MASSIVEChem/)
+
+MASSIVEChem can be installed using pip as
+```bash
+pip install MASSIVEChem
+```
+
+
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem?tab=readme-ov-file)
+
+Alternatively, the package can be directly installed from the GitHub repository via pip using the following command in the terminal
+```bash
+pip install git+https://github.com/ThomasCsson/MASSIVEChem
+```
+
+
+![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
+
+The package can also be installed from source by running the following commands
+
+First, clone the repository from github and go in the folder. 
+```bash
+git clone https://github.com/ThomasCsson/MASSIVEChem.git
+cd path/to/MASSIVEChem
+```
+Then, install the package using : 
+```bash
+pip install -e .
+```
+
+## Requirments
+The package runs on python 3.10 but supports python 3.8 through 3.10.
+It requires several other packages to function correctly.
+
+```bash
+bokeh
+rdkit
+panel
+```
+
+(Note: panel is not directly used, but is required for added functionality involving the 3 dimmensinal visualisation of the input molecule)
+
+If all goes well during installation, the preceding packages should all install automatically.
+But this can be checked by veryfying that they have all been installed in the desired environment. To do this, simply write the following command in the terminal:
+
+```bash
+pip show MASSIVEChem
+```
+
+If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
+
+```bash
+pip install bokeh
+pip install rdkit
+pip install panel
+```
+
+Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourself, the following command needs to be run.
+
+```bash
+python -m pip install git+https://github.com/zotko/xyz2graph.git
+```
+
+
+## Usage
+
+The principal function of this package takes the SMILEs of a molecule as an input and displays the mass spectrum of the molecule as well as the molecule itself and  the functional groups it contains.
+
+An example on how to make the function work is shown below for benzylpenicilin:
+
+The ionization method is set to monodeprotonation and the resolution of the apparatus is set to 0.01 Th
+
+```bash
+import MASSIVEChem.MASSIVEChem as MC
+from bokeh.plotting import show
+
+mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
+apparatus_resolution = 0.01
+
+show(MC.spectrum(mol_smi, True, apparatus_resolution))
+
+
+#The first input in MC.spectrum is the molecule under SMILEs representation,
+#and the third is the resolution of the apparatus (typically, this value is of 0.01)
+#the second computes an approximate spectrum if True and the precise spectrum if False
+
+```
+
+The output of this command will be:
+
+<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Spectrum_output.png">
+
+Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
+
+<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
+
+## Trouble shooting
+
+If there is a problem with the functions of the package, first, verify that your version is up to date. To do this, type the following command into the terminal:
+```bash
+pip show MASSIVEChem
+```
+You can then compare the version that you have downloaded to that of the newest available version, which can be found on the PiPy page, https://pypi.org/project/MASSIVEChem/
+
+Then, if the version donwloaded is not the newest one, type the following command into the terminal:
+```bash
+pip intall MASSIVEChem -- upgrade
+```
+
+
+
+## Getting started
+[![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-orange.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/notebooks/project_report.ipynb)
+
+To begin to use the package, the following jupyter notebook will give you information about all of its functions:
+
+
+## Fun !
+🐰 If you've made it this far through our project, you might want to try to find the hidden easter egg in this ReadMe :)🐰
+
+(_hint: you might want to try clicking on various badges throughout the ReadMe_)
```

### Comparing `massivechem-5.4/pyproject.toml` & `massivechem-5.5/pyproject.toml`

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
-00000070: 7665 7273 696f 6e20 3d20 2235 2e34 220d  version = "5.4".
+00000070: 7665 7273 696f 6e20 3d20 2235 2e35 220d  version = "5.5".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
```

### Comparing `massivechem-5.4/PKG-INFO` & `massivechem-5.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,177 +1,178 @@
-Metadata-Version: 2.3
-Name: MASSIVEChem
-Version: 5.4
-Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
-Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
-Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
-Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
-Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
-Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
-License-Expression: MIT
-License-File: LICENSE.txt
-Keywords: Mass spectroscopy,chemical-engineering,chemical-property-prediction,cheminformatics,chemistry,chemistry-lab,functional group,spectrometry,spectroscopy,unsaturation
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: bokeh
-Requires-Dist: panel
-Requires-Dist: rdkit
-Description-Content-Type: text/markdown
-
-<img width="830" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Logo.jpg">
-
-[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
-[![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
-![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
-[![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
-
-
-# -         MASSIVEChem       - 
-
-[![GitHub2](https://img.shields.io/badge/Maintained%3F-yes-turquoise.svg)](https://pypi.org/user/Arthur.hmy/)
-[![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=orange)](https://www.python.org)
-[![GitHub3](https://img.shields.io/badge/Contributors-3-green.svg)](https://github.com/ThomasCsson/MASSIVEChem/graphs/contributors)
-[![GitHub3](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
-[![GitHub3](https://img.shields.io/badge/EPFL-CH200-red.svg)](https://edu.epfl.ch/studyplan/en/bachelor/chemistry-and-chemical-engineering/coursebook/practical-programming-in-chemistry-CH-200)
-
-
- - Python package for applied analytical chemistry focused primarily on mass speectrometry 
-#### Project within _practical programming in chemistry_ course -- EPFL CH-200
-
-## Package description
-[![GitHub3](http://ForTheBadge.com/images/badges/built-with-science.svg)](https://x.com/pschwllr/status/1760713822111723990)
-[![GitHub4](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-
-MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable python package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
-The aim of this package is to provide the user with functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
-
-Developpers:
-- Thomas Viking Christiansson, student in chemical engineering at EPFL    [![jhc github](https://img.shields.io/badge/GitHub-ThomasCsson-181717.svg?style=flat&logo=github)](https://github.com/ThomasCsson)
-- Igor Gonteri, student in chemistry at EPFL                             [![jhc github](https://img.shields.io/badge/GitHub-igorgonteri-181717.svg?style=flat&logo=github)](https://github.com/igorgonteri)
-- Arthur Humery, student in chemical engineering at EPFL                [![jhc github](https://img.shields.io/badge/GitHub-Arthurhmy-181717.svg?style=flat&logo=github)](https://github.com/Arthurhmy)
-
-### What is mass spectrometry ?
-
-Mass spectrometry (MS) is an analytical technique used to measure the mass-to-charge ratio of ions. It helps identify the structure of the chemical compound present in a sample by generating a spectrum of the masses of its ions. The process involves three main steps:
-
-Ionisation: The sample is ionised, which means its molecules are converted into charged particles (ions). This can be done using various methods, such as electron impact (EI), electrospray ionisation (ESI), or matrix-assisted laser desorption/ionisation (MALDI). In this case, the ionisation is set to the most commonly used method; deprotonation.
-
-Mass Analysis: The ions are separated based on their mass-to-charge ratio (m/z). This is usually done using a mass analyser, such as a quadrupole, time-of-flight (TOF), or an ion trap. Each type of mass analyser works differently but ultimately serves to distinguish ions by their specific m/z values. The unit of these m/z values is 1 Th or 1 $\frac{Da}{e}$.
-
-On the y axis of the output spectrum, the relative abundance of the different ions is plotted. This abundance is given by the different natural abundances of the different isotopes of the atoms in the molecule. For example, the relative abundance of $^{13}C$ is 1.1% and that of $^{12}C$ is 98.9%.
-
-Mass spectrometry is widely used in various fields, including:
-
-Chemistry: For molecular identification and structural elucidation. Biochemistry: For studying proteins, peptides, and other biomolecules. Pharmaceuticals: For drug development and metabolite analysis. Environmental Science: For detecting pollutants and analysing environmental samples. Clinical Diagnostics: For identifying biomarkers and analysing complex biological samples. The technique's sensitivity, accuracy, and ability to analyse complex mixtures make it an essential tool in both research and applied sciences.
-
-Now, let us go through the steps required to use this package!
-
-## Installation
-[![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/MASSIVEChem/)
-
-MASSIVEChem can be installed using pip as
-```bash
-pip install MASSIVEChem
-```
-
-
-[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem?tab=readme-ov-file)
-
-Alternatively, the package can be directly installed from the GitHub repository via pip using the following command in the terminal
-```bash
-pip install git+https://github.com/ThomasCsson/MASSIVEChem
-```
-
-
-![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
-
-The package can also be installed from source by running the following commands
-
-First, clone the repository from github and go in the folder. 
-```bash
-git clone https://github.com/ThomasCsson/MASSIVEChem.git
-cd path/to/MASSIVEChem
-```
-Then, install the package using : 
-```bash
-pip install -e .
-```
-
-## Requirments
-The package runs on python 3.10 but supports python 3.8 through 3.10.
-It requires several other packages to function correctly.
-
-```bash
-bokeh
-rdkit
-panel
-```
-
-(Note: panel is not directly used, but is required for added functionality involving the 3 dimmensinal visualisation of the input molecule)
-
-If all goes well during installation, the preceding packages should all install automatically.
-But this can be checked by veryfying that they have all been installed in the desired environment. To do this, simply write the following command in the terminal:
-
-```bash
-pip show "name of the package"
-```
-
-If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
-
-```bash
-pip install bokeh
-pip install rdkit
-pip install panel
-```
-Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourself, the following command needs to be run.
-
-```bash
-python -m pip install git+https://github.com/zotko/xyz2graph.git
-```
-
-
-## Usage
-
-The principal function of this package takes the SMILEs of a molecule as an input and displays the mass spectrometry of the molecule as well as the molecule itself and  the functional groups it contains.
-
-An example on how to make the function work is shown below for benzylpenicilin:
-
-The ionization method is set to monodeprotonation and the resolution of the apparatus is 0.01 Th
-
-```bash
-import MASSIVEChem.MASSIVEChem as MC
-from bokeh.plotting import show
-
-mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
-apparatus_resolution = 0.01
-
-show(MC.spectrum(mol_smi, True, apparatus_resolution))
-
-
-#The first input in MC.spectrum is the molecule under SMILEs representation,
-#and the third is the resolution of the apparatus (typically, this value is of 0.01)
-#the second computes an approximate spectrum if True and the precise spectrum if False
-
-```
-
-The output of this command will be:
-
-<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Spectrum_output.png">
-
-Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
-
-<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
-
-## Getting started
-[![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
-
-To begin to use the package the following jupyter notebook will give you information about all the package's functions:
-
-[![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-orange.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/notebooks/project_report.ipynb)
-
-## Fun !
-🐰 If you've made it this far through our project, you might want to try to find the hidden easter egg in this ReadMe :)🐰
-
-(_hint: you might want to try clicking on various badges throughout the ReadMe_)
+<img width="830" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Logo.jpg">
+
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
+[![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
+![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
+[![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
+
+
+# -         MASSIVEChem       - 
+
+[![GitHub2](https://img.shields.io/badge/Maintained%3F-yes-turquoise.svg)](https://pypi.org/user/Arthur.hmy/)
+[![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=orange)](https://www.python.org)
+[![GitHub3](https://img.shields.io/badge/Contributors-3-green.svg)](https://github.com/ThomasCsson/MASSIVEChem/graphs/contributors)
+[![GitHub3](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
+[![GitHub3](https://img.shields.io/badge/EPFL-CH200-red.svg)](https://edu.epfl.ch/studyplan/en/bachelor/chemistry-and-chemical-engineering/coursebook/practical-programming-in-chemistry-CH-200)
+
+
+ - Python package for applied analytical chemistry focused primarily on mass spectrometry 
+#### Project within _practical programming in chemistry_ course -- EPFL CH-200
+
+## Package description
+[![GitHub3](http://ForTheBadge.com/images/badges/built-with-science.svg)](https://x.com/pschwllr/status/1760713822111723990)
+[![GitHub4](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+
+MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable python package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
+The aim of this package is to provide the user with functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
+
+Developpers:
+- Thomas Viking Christiansson, student in chemical engineering at EPFL    [![jhc github](https://img.shields.io/badge/GitHub-ThomasCsson-181717.svg?style=flat&logo=github)](https://github.com/ThomasCsson)
+- Igor Gonteri, student in chemistry at EPFL                             [![jhc github](https://img.shields.io/badge/GitHub-igorgonteri-181717.svg?style=flat&logo=github)](https://github.com/igorgonteri)
+- Arthur Humery, student in chemical engineering at EPFL                [![jhc github](https://img.shields.io/badge/GitHub-Arthurhmy-181717.svg?style=flat&logo=github)](https://github.com/Arthurhmy)
+
+### What is mass spectrometry ?
+
+Mass spectrometry (MS) is an analytical technique used to measure the mass-to-charge ratio of ions. It helps identify the structure of the chemical compound present in a sample by generating a spectrum of the masses of its ions. The process involves two main steps:
+
+Ionisation: The sample is ionised, which means its molecules are converted into charged particles (ions). This can be done using various methods, such as electron impact (EI), electrospray ionisation (ESI), or matrix-assisted laser desorption/ionisation (MALDI). In this case, the ionisation is set to the most commonly used method; deprotonation.
+
+Mass Analysis: The ions are separated based on their mass-to-charge ratio (m/z). This is usually done using a mass analyser, such as a quadrupole, time-of-flight (TOF), or an ion trap. Each type of mass analyser works differently but ultimately serves to distinguish ions by their specific $\frac{m}{z}$ values. The unit of these $\frac{m}{z}$ values is 1 Th or 1 $\frac{Da}{e}$.
+
+On the y axis of the output spectrum, the relative abundance of the different ions is plotted. This abundance is given by the different natural abundances of the different isotopes of the atoms in the molecule. For example, the relative abundance of $^{13}C$ is 1.1% and that of $^{12}C$ is 98.9%.
+
+Mass spectrometry is widely used in various fields, including:
+
+Chemistry, for molecular identification and structural elucidation. Biochemistry, for studying proteins, peptides, and other biomolecules. Pharmaceuticals, for drug development and metabolite analysis. Environmental Science, for detecting pollutants and analysing environmental samples. Clinical Diagnostics, for identifying biomarkers and analysing complex biological samples. The technique's sensitivity, accuracy, and ability to analyse complex mixtures make it an essential tool in both research and applied sciences.
+
+The mathematical reasoning behind the calculation of these relative abundances is simply applying combinatorics to each isotope of each atom in the given molecule.
+
+To find the probability of a molecule composed of isotopes $I_{1}$ , $I_{2}$ , ... , $I_{n}$ is given by the following formula:
+
+$Pr(I_{1},I_{2},...,I_{n})$ = $Pr(I_{1})$ $\cdot$ $Pr(I_{2})$ $\cdot$ ... $\cdot$ $Pr(I_{n})$
+
+This probability is then the relative abundance of the molecule composed of those isotopes.
+
+Now, let us go through the steps required to use this package!
+
+## Installation
+[![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/MASSIVEChem/)
+
+MASSIVEChem can be installed using pip as
+```bash
+pip install MASSIVEChem
+```
+
+
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem?tab=readme-ov-file)
+
+Alternatively, the package can be directly installed from the GitHub repository via pip using the following command in the terminal
+```bash
+pip install git+https://github.com/ThomasCsson/MASSIVEChem
+```
+
+
+![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
+
+The package can also be installed from source by running the following commands
+
+First, clone the repository from github and go in the folder. 
+```bash
+git clone https://github.com/ThomasCsson/MASSIVEChem.git
+cd path/to/MASSIVEChem
+```
+Then, install the package using : 
+```bash
+pip install -e .
+```
+
+## Requirments
+The package runs on python 3.10 but supports python 3.8 through 3.10.
+It requires several other packages to function correctly.
+
+```bash
+bokeh
+rdkit
+panel
+```
+
+(Note: panel is not directly used, but is required for added functionality involving the 3 dimmensinal visualisation of the input molecule)
+
+If all goes well during installation, the preceding packages should all install automatically.
+But this can be checked by veryfying that they have all been installed in the desired environment. To do this, simply write the following command in the terminal:
+
+```bash
+pip show MASSIVEChem
+```
+
+If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
+
+```bash
+pip install bokeh
+pip install rdkit
+pip install panel
+```
+
+Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourself, the following command needs to be run.
+
+```bash
+python -m pip install git+https://github.com/zotko/xyz2graph.git
+```
+
+
+## Usage
+
+The principal function of this package takes the SMILEs of a molecule as an input and displays the mass spectrum of the molecule as well as the molecule itself and  the functional groups it contains.
+
+An example on how to make the function work is shown below for benzylpenicilin:
+
+The ionization method is set to monodeprotonation and the resolution of the apparatus is set to 0.01 Th
+
+```bash
+import MASSIVEChem.MASSIVEChem as MC
+from bokeh.plotting import show
+
+mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
+apparatus_resolution = 0.01
+
+show(MC.spectrum(mol_smi, True, apparatus_resolution))
+
+
+#The first input in MC.spectrum is the molecule under SMILEs representation,
+#and the third is the resolution of the apparatus (typically, this value is of 0.01)
+#the second computes an approximate spectrum if True and the precise spectrum if False
+
+```
+
+The output of this command will be:
+
+<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Spectrum_output.png">
+
+Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
+
+<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
+
+## Trouble shooting
+
+If there is a problem with the functions of the package, first, verify that your version is up to date. To do this, type the following command into the terminal:
+```bash
+pip show MASSIVEChem
+```
+You can then compare the version that you have downloaded to that of the newest available version, which can be found on the PiPy page, https://pypi.org/project/MASSIVEChem/
+
+Then, if the version donwloaded is not the newest one, type the following command into the terminal:
+```bash
+pip intall MASSIVEChem -- upgrade
+```
+
+
+
+## Getting started
+[![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-orange.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/notebooks/project_report.ipynb)
+
+To begin to use the package, the following jupyter notebook will give you information about all of its functions:
+
+
+## Fun !
+🐰 If you've made it this far through our project, you might want to try to find the hidden easter egg in this ReadMe :)🐰
+
+(_hint: you might want to try clicking on various badges throughout the ReadMe_)
```

