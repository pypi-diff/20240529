# Comparing `tmp/massivechem-5.3.tar.gz` & `tmp/massivechem-5.4.tar.gz`

## Comparing `massivechem-5.3.tar` & `massivechem-5.4.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.3/Focused_spectrum.png
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.3/Logo.jpg
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.3/MASSIVEChem.yml
--rw-r--r--   0        0        0    26315 2020-02-02 00:00:00.000000 massivechem-5.3/Schematic_mass_spectrum.png
--rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.3/Spectrum_output.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.3/project_final.yml
--rw-r--r--   0        0        0   104043 2020-02-02 00:00:00.000000 massivechem-5.3/notebooks/backup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.3/notebooks/checklist.txt
--rw-r--r--   0        0        0   110887 2020-02-02 00:00:00.000000 massivechem-5.3/notebooks/project_report.ipynb
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/all_in_one.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/calculate_unsaturation.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/double_plot.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/functional_group_display.py
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/functional_group_finder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/ionisation_method.py
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/main_function.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/mol_web_show.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/peak_merger.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/peak_sorter.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/smiles_to_3D_plot.py
--rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/spectrum.py
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/spectrum_3D.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.3/scripts/sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.3/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.3/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.3/test/__init__.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_SMILEs_interpreter.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_calculate_unsaturation.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_delta_function_plotter.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_double_plot.py
--rw-r--r--   0        0        0     7670 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_functional_group_display.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_functional_group_finder.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_ionisation_method.py
--rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_main_function.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_mol_web_show.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_molecule_list_generator.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_peak_merger.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_peak_sorter.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_smiles_to_3D_plot.py
--rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_spectrum.py
--rw-r--r--   0        0        0    31039 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_spectrum_3D.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.3/test/test_sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.3/LICENSE.txt
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 massivechem-5.3/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.3/pyproject.toml
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 massivechem-5.3/PKG-INFO
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.4/MASSIVEChem.yml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.4/project_final.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.4/images/Focused_spectrum.png
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.4/images/Logo.jpg
+-rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.4/images/Spectrum_output.png
+-rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.4/notebooks/backup.py
+-rw-r--r--   0        0        0     9376 2020-02-02 00:00:00.000000 massivechem-5.4/notebooks/molecule_image.png
+-rw-r--r--   0        0        0   216605 2020-02-02 00:00:00.000000 massivechem-5.4/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/calculate_unsaturation.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/double_plot.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/functional_group_display.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/ionisation_method.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/main_function.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/peak_sorter.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/spectrum.py
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/spectrum_3D.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.4/scripts/sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0   103206 2020-02-02 00:00:00.000000 massivechem-5.4/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.4/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.4/test/__init__.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_SMILEs_interpreter.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_calculate_unsaturation.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_delta_function_plotter.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_double_plot.py
+-rw-r--r--   0        0        0     7670 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_functional_group_display.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_functional_group_finder.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_ionisation_method.py
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_main_function.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_mol_web_show.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_molecule_list_generator.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_peak_merger.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_peak_sorter.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_spectrum.py
+-rw-r--r--   0        0        0    31039 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_spectrum_3D.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.4/test/test_sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.4/LICENSE.txt
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 massivechem-5.4/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.4/pyproject.toml
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 massivechem-5.4/PKG-INFO
```

### Comparing `massivechem-5.3/Logo.jpg` & `massivechem-5.4/images/Logo.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/MASSIVEChem.yml` & `massivechem-5.4/MASSIVEChem.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/Spectrum_output.png` & `massivechem-5.4/images/Spectrum_output.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/project_final.yml` & `massivechem-5.4/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/notebooks/backup.py` & `massivechem-5.4/notebooks/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,19 +48,20 @@
             N += 1
         elif atom.GetSymbol() in halogens_hydrogen:
             HX += 1
 
     unsaturation = C + 1 + (N - HX) / 2
 
     return unsaturation
-import time
+
 #2
 def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
-    begin = time.time()
+    
     mol_without_Hs = Chem.MolFromSmiles(mol_smi)
+
     #tests for wether the input is valid
     if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if imprecision_True_False not in [True, False]:
         raise ValueError('Enter a boolean value')
     if apparatus_resolution < 0:
         raise ValueError('Enter a positive value')
@@ -138,18 +139,14 @@
                 'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 
                 'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 
                 'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 
                 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Ta', 'Ta', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 
                 'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 
                 'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
     
-
-    
-
-
     
     mol = Chem.AddHs(mol_without_Hs)
 
     '''molecule list generator'''
     list_atoms = []
     for atom in mol.GetAtoms():
         list_atoms.append(atom.GetSymbol())
@@ -620,30 +617,16 @@
 
     table_height = min(200 + num_groups * 60, 800)
 
     func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
     last = column(img_div, func_group_table)
     final = row(double_graph, last)
-    end = time.time()
-    print(f' {end-begin} seconds')
     return final
-from rdkit import Chem
-from rdkit.Chem import Draw
 
-from bokeh.plotting import figure, show, row
-from bokeh.models.tickers import FixedTicker
-from bokeh.layouts import row, column
-from bokeh.io import show
-from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
-from bokeh.models.widgets import DataTable, TableColumn
-
-import base64
-from io import BytesIO
-show(spectrum('CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C', False, 0.01))
 #3
 def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
 
     #lists of the data to facilitise the pip-installability of the package
 
     mol_smi_3D = mol_smi
 
@@ -2163,8 +2146,7 @@
 
     return fig
 
 
 
 
 
-
```

### Comparing `massivechem-5.3/scripts/SMILEs_interpreter.py` & `massivechem-5.4/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/all_in_one.py` & `massivechem-5.4/scripts/all_in_one.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 from bokeh.plotting import figure
 from bokeh.models import ColumnDataSource
 from bokeh.layouts import column, row
 from bokeh.models.widgets import DataTable, TableColumn
 
-def all_in_one(p1, p2, p3, p4):
+def all_in_one(p1, p2, p3):
 
     #---------------------------------------------------------------------------------------------#
     '''
     all_in_one(p1,p2,p3, p4)
     
     Input: 3 bokeh plots
             Usually used in this package:
                     - p1 : bokeh double plot of mass spectrometry
                     - p2 : image of the molecule
                     - p3 : table of functional groups
-                    - p4 : buttons with info on the molecule
     
     Output: bokeh page with all 4 graphs well arranged
 
     '''
     #---------------------------------------------------------------------------------------------#
     
     if not p1:
         raise ValueError("Enter a non-empty plot")
     if not p2:
         raise ValueError("Enter a non-empty plot")
     if not p3:
         raise ValueError("Enter a non-empty plot")
-    if not p4:
-        raise ValueError("Enter a non-empty plot")
-    
-    #creates a layout in row with p3 and p4
-    layout1 = row(p3, p4)
 
-    #creates a layout in column with p2 and layout1
-    layout2 = column(p2, layout1)
+    #creates a layout in column with p2 and p3
+    layout2 = column(p2, p3)
 
     #creates the final layout in row with layout1 and p1
     layout = row(p1, layout2)
 
     return layout
```

### Comparing `massivechem-5.3/scripts/calculate_unsaturation.py` & `massivechem-5.4/scripts/calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/delta_function_plotter.py` & `massivechem-5.4/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/double_plot.py` & `massivechem-5.4/scripts/double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/functional_group_display.py` & `massivechem-5.4/scripts/functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/functional_group_finder.py` & `massivechem-5.4/scripts/functional_group_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,8 +171,7 @@
                 if 'Amine' in functional_groups_contained:
                     functional_groups_contained.remove('Amine')
 
     
     
     return functional_groups_contained
 
-print(functional_group_finder('CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'))
```

### Comparing `massivechem-5.3/scripts/ionisation_method.py` & `massivechem-5.4/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/main_function.py` & `massivechem-5.4/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/mol_web_show.py` & `massivechem-5.4/scripts/mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/molecule_list_generator.py` & `massivechem-5.4/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/peak_merger.py` & `massivechem-5.4/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/peak_sorter.py` & `massivechem-5.4/scripts/peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/smiles_to_3D_plot.py` & `massivechem-5.4/scripts/smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/spectrum.py` & `massivechem-5.4/scripts/spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/spectrum_3D.py` & `massivechem-5.4/scripts/spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/sulphur_nitrogen_adder.py` & `massivechem-5.4/scripts/sulphur_nitrogen_adder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/scripts/sulphur_nitrogen_finder.py` & `massivechem-5.4/scripts/sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/src/MASSiveChem/MASSiveChem.py` & `massivechem-5.4/src/MASSiveChem/MASSiveChem.py`

 * *Files 0% similar despite different names*

```diff
@@ -2067,46 +2067,40 @@
     p.xgrid.grid_line_color = None
     p.ygrid.grid_line_color = None
     p.xaxis.visible = False
     p.yaxis.visible = False
 
     return p
  
-def all_in_one(p1, p2, p3, p4):
+def all_in_one(p1, p2, p3):
 
     #---------------------------------------------------------------------------------------------#
     '''
     all_in_one(p1,p2,p3, p4)
     
     Input: 3 bokeh plots
             Usually used in this package:
                     - p1 : bokeh double plot of mass spectrometry
                     - p2 : image of the molecule
                     - p3 : table of functional groups
-                    - p4 : buttons with info on the molecule
     
     Output: bokeh page with all 4 graphs well arranged
 
     '''
     #---------------------------------------------------------------------------------------------#
     
     if not p1:
         raise ValueError("Enter a non-empty plot")
     if not p2:
         raise ValueError("Enter a non-empty plot")
     if not p3:
         raise ValueError("Enter a non-empty plot")
-    if not p4:
-        raise ValueError("Enter a non-empty plot")
-    
-    #creates a layout in row with p3 and p4
-    layout1 = row(p3, p4)
 
-    #creates a layout in column with p2 and layout1
-    layout2 = column(p2, layout1)
+    #creates a layout in column with p2 and p3
+    layout2 = column(p2, p3)
 
     #creates the final layout in row with layout1 and p1
     layout = row(p1, layout2)
 
     return layout
 
 def smiles_to_3D_plot(mol_smi):
```

### Comparing `massivechem-5.3/test/test_SMILEs_interpreter.py` & `massivechem-5.4/test/test_SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_calculate_unsaturation.py` & `massivechem-5.4/test/test_calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_delta_function_plotter.py` & `massivechem-5.4/test/test_delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_double_plot.py` & `massivechem-5.4/test/test_double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_functional_group_display.py` & `massivechem-5.4/test/test_functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_functional_group_finder.py` & `massivechem-5.4/test/test_functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_ionisation_method.py` & `massivechem-5.4/test/test_ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_main_function.py` & `massivechem-5.4/test/test_main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_mol_web_show.py` & `massivechem-5.4/test/test_mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_molecule_list_generator.py` & `massivechem-5.4/test/test_molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_peak_merger.py` & `massivechem-5.4/test/test_peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_peak_sorter.py` & `massivechem-5.4/test/test_peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_smiles_to_3D_plot.py` & `massivechem-5.4/test/test_smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_spectrum.py` & `massivechem-5.4/test/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_spectrum_3D.py` & `massivechem-5.4/test/test_spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_sulphur_nitrogen_adder.py` & `massivechem-5.4/test/test_sulphur_nitrogen_adder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/test/test_sulphur_nitrogen_finder.py` & `massivechem-5.4/test/test_sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/.gitignore` & `massivechem-5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/LICENSE.txt` & `massivechem-5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-5.3/README.md` & `massivechem-5.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img width="600" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Logo.jpg">
+<img width="830" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Logo.jpg">
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
 [![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 ![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
 [![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 
 
@@ -66,27 +66,21 @@
 ![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
 
 The package can also be installed from source by running the following commands
 
 First, clone the repository from github and go in the folder. 
 ```bash
 git clone https://github.com/ThomasCsson/MASSIVEChem.git
-cd MASSIVEChem
+cd path/to/MASSIVEChem
 ```
 Then, install the package using : 
 ```bash
 pip install -e .
 ```
 
-
-
-
-
-
-
 ## Requirments
 The package runs on python 3.10 but supports python 3.8 through 3.10.
 It requires several other packages to function correctly.
 
 ```bash
 bokeh
 rdkit
@@ -105,15 +99,15 @@
 If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
 
 ```bash
 pip install bokeh
 pip install rdkit
 pip install panel
 ```
-Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourslef, the following command needs to be run.
+Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourself, the following command needs to be run.
 
 ```bash
 python -m pip install git+https://github.com/zotko/xyz2graph.git
 ```
 
 
 ## Usage
@@ -130,32 +124,32 @@
 
 mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
 apparatus_resolution = 0.01
 
 show(MC.spectrum(mol_smi, True, apparatus_resolution))
 
 
-#The first input in ms.spectrum is the molecule under SMILEs representation,
-#and the third is the resolution of the apparatus (typically, this value is of 0.01
+#The first input in MC.spectrum is the molecule under SMILEs representation,
+#and the third is the resolution of the apparatus (typically, this value is of 0.01)
 #the second computes an approximate spectrum if True and the precise spectrum if False
 
 ```
 
 The output of this command will be:
 
-<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Spectrum_output.png">
+<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Spectrum_output.png">
 
 Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
 
 <img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
 
 ## Getting started
 [![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
 
 To begin to use the package the following jupyter notebook will give you information about all the package's functions:
 
-'''link to jupter notebook'''
+[![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-orange.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/notebooks/project_report.ipynb)
 
 ## Fun !
 🐰 If you've made it this far through our project, you might want to try to find the hidden easter egg in this ReadMe :)🐰
 
 (_hint: you might want to try clicking on various badges throughout the ReadMe_)
```

### Comparing `massivechem-5.3/pyproject.toml` & `massivechem-5.4/pyproject.toml`

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
-00000070: 7665 7273 696f 6e20 3d20 2235 2e33 220d  version = "5.3".
+00000070: 7665 7273 696f 6e20 3d20 2235 2e34 220d  version = "5.4".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
```

### Comparing `massivechem-5.3/PKG-INFO` & `massivechem-5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 5.3
+Version: 5.4
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: bokeh
 Requires-Dist: panel
 Requires-Dist: rdkit
 Description-Content-Type: text/markdown
 
-<img width="600" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Logo.jpg">
+<img width="830" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Logo.jpg">
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
 [![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 ![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
 [![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 
 
@@ -88,27 +88,21 @@
 ![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
 
 The package can also be installed from source by running the following commands
 
 First, clone the repository from github and go in the folder. 
 ```bash
 git clone https://github.com/ThomasCsson/MASSIVEChem.git
-cd MASSIVEChem
+cd path/to/MASSIVEChem
 ```
 Then, install the package using : 
 ```bash
 pip install -e .
 ```
 
-
-
-
-
-
-
 ## Requirments
 The package runs on python 3.10 but supports python 3.8 through 3.10.
 It requires several other packages to function correctly.
 
 ```bash
 bokeh
 rdkit
@@ -127,15 +121,15 @@
 If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
 
 ```bash
 pip install bokeh
 pip install rdkit
 pip install panel
 ```
-Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourslef, the following command needs to be run.
+Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourself, the following command needs to be run.
 
 ```bash
 python -m pip install git+https://github.com/zotko/xyz2graph.git
 ```
 
 
 ## Usage
@@ -152,32 +146,32 @@
 
 mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
 apparatus_resolution = 0.01
 
 show(MC.spectrum(mol_smi, True, apparatus_resolution))
 
 
-#The first input in ms.spectrum is the molecule under SMILEs representation,
-#and the third is the resolution of the apparatus (typically, this value is of 0.01
+#The first input in MC.spectrum is the molecule under SMILEs representation,
+#and the third is the resolution of the apparatus (typically, this value is of 0.01)
 #the second computes an approximate spectrum if True and the precise spectrum if False
 
 ```
 
 The output of this command will be:
 
-<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Spectrum_output.png">
+<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/images/Spectrum_output.png">
 
 Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
 
 <img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
 
 ## Getting started
 [![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
 
 To begin to use the package the following jupyter notebook will give you information about all the package's functions:
 
-'''link to jupter notebook'''
+[![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-orange.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/notebooks/project_report.ipynb)
 
 ## Fun !
 🐰 If you've made it this far through our project, you might want to try to find the hidden easter egg in this ReadMe :)🐰
 
 (_hint: you might want to try clicking on various badges throughout the ReadMe_)
```

