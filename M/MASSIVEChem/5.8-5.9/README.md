# Comparing `tmp/massivechem-5.8.tar.gz` & `tmp/massivechem-5.9.tar.gz`

## Comparing `massivechem-5.8.tar` & `massivechem-5.9.tar`

### file list

```diff
@@ -1,52 +1,50 @@
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.8/MASSIVEChem.yml
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 massivechem-5.8/molecule_image.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.8/project_final.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.8/images/Focused_spectrum.png
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.8/images/Logo.jpg
--rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.8/images/Spectrum_output.png
--rw-r--r--   0        0        0   103428 2020-02-02 00:00:00.000000 massivechem-5.8/notebooks/backup.py
--rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 massivechem-5.8/notebooks/molecule_image.png
--rw-r--r--   0        0        0   373004 2020-02-02 00:00:00.000000 massivechem-5.8/notebooks/project_report.ipynb
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/all_in_one.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/calculate_unsaturation.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/double_plot.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/functional_group_display.py
--rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/functional_group_finder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/ionisation_method.py
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/main_function.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/mol_web_show.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/peak_merger.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/peak_sorter.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/smiles_to_3D_plot.py
--rw-r--r--   0        0        0    29747 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/spectrum.py
--rw-r--r--   0        0        0    30541 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/spectrum_3D.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.8/scripts/sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0   103489 2020-02-02 00:00:00.000000 massivechem-5.8/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.8/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.8/test/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_SMILEs_interpreter.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_calculate_unsaturation.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_delta_function_plotter.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_double_plot.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_functional_group_display.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_functional_group_finder.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_ionisation_method.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_main_function.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_mol_web_show.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_molecule_list_generator.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_peak_merger.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_peak_sorter.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_smiles_to_3D_plot.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_spectrum.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_spectrum_3D.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 massivechem-5.8/test/test_sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.8/LICENSE.txt
--rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 massivechem-5.8/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.8/pyproject.toml
--rw-r--r--   0        0        0    11377 2020-02-02 00:00:00.000000 massivechem-5.8/PKG-INFO
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.9/MASSIVEChem.yml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.9/project_final.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.9/images/Focused_spectrum.png
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.9/images/Logo.jpg
+-rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.9/images/Spectrum_output.png
+-rw-r--r--   0        0        0    30042 2020-02-02 00:00:00.000000 massivechem-5.9/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/calculate_unsaturation.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/double_plot.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/functional_group_display.py
+-rw-r--r--   0        0        0     8961 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/ionisation_method.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/main_function.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/peak_sorter.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    29626 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/spectrum.py
+-rw-r--r--   0        0        0    30401 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/spectrum_3D.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.9/scripts/sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0   103516 2020-02-02 00:00:00.000000 massivechem-5.9/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.9/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.9/test/__init__.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_SMILEs_interpreter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_all_tests.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_calculate_unsaturation.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_delta_function_plotter.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_double_plot.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_functional_group_display.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_functional_group_finder.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_ionisation_method.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_main_function.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_mol_web_show.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_molecule_list_generator.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_peak_merger.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_peak_sorter.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_smiles_to_3D_plot.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_spectrum.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_spectrum_3D.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 massivechem-5.9/test/test_sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.9/LICENSE.txt
+-rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 massivechem-5.9/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.9/pyproject.toml
+-rw-r--r--   0        0        0    11377 2020-02-02 00:00:00.000000 massivechem-5.9/PKG-INFO
```

### Comparing `massivechem-5.8/MASSIVEChem.yml` & `massivechem-5.9/MASSIVEChem.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/project_final.yml` & `massivechem-5.9/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/images/Logo.jpg` & `massivechem-5.9/images/Logo.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/images/Spectrum_output.png` & `massivechem-5.9/images/Spectrum_output.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/notebooks/backup.py` & `massivechem-5.9/src/MASSiveChem/MASSiveChem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 from rdkit import Chem
 from rdkit.Chem import Draw, AllChem
-
 import base64
-
-import os
-
 from bokeh.plotting import figure, row
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
 from bokeh.models.tickers import FixedTicker
 from bokeh.models.widgets import DataTable, TableColumn
 from bokeh.layouts import row, column
-
 from io import BytesIO
-
 import tempfile
-
 from xyz2graph import MolGraph, to_plotly_figure
-
 import panel as pn
 
 #main functions:
 #1
 def calculate_unsaturation(mol_smile) -> int:
     #---------------------------------------------------------------------------------------------#
     '''
@@ -55,14 +47,16 @@
 
 #2
 def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
     
     mol_without_Hs = Chem.MolFromSmiles(mol_smi)
 
     #tests for wether the input is valid
+    if mol_smi == '':
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if imprecision_True_False not in [True, False]:
         raise ValueError('Enter a boolean value')
     if apparatus_resolution < 0:
         raise ValueError('Enter a positive value')
     if type(apparatus_resolution) != float:
@@ -622,14 +616,28 @@
     last = column(img_div, func_group_table)
     final = row(double_graph, last)
     return final
 
 #3
 def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
 
+
+    mol_without_Hs = Chem.MolFromSmiles(mol_smi)
+
+    if mol_without_Hs is None:
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
+    if mol_smi == '':
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
+    if imprecision_True_False not in [True, False]:
+        raise ValueError('Enter a boolean value')
+    if apparatus_resolution < 0:
+        raise ValueError('Enter a positive value')
+    if type(apparatus_resolution) != float:
+        raise ValueError('Enter an integer value')
+
     #lists of the data to facilitise the pip-installability of the package
 
     mol_smi_3D = mol_smi
 
     mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
             136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 
             12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 
@@ -1586,16 +1594,19 @@
         raise ValueError("The fifth argument must be a positive integer")
     if count_S < 0:
         raise ValueError("The sixth argument must be a positive integer")
     if type(count_N) != int:
         raise ValueError("The fifth argument must be an integer")
     if type(count_S) != int:
         raise ValueError("The sixth argument must be an integer")
-    if x_in != sorted(x_in):
-        raise ValueError("The first list must be ordered")
+    if type(x_in) != list:
+        raise ValueError("The first argument must be a list")
+    if type(y_in) != list:
+        raise ValueError("The second argument must be a list")
+
 
     maximum = max(y_in)
 
     if has_N:
         x_in.append(x_in[1] - 0.006)  
         y_in.append(0.0035*count_N*maximum)  
     
@@ -1769,14 +1780,16 @@
     
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
@@ -2007,106 +2020,75 @@
 
     table_height = min(200 + num_groups * 60, 800)
 
     data_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
     return data_table
 
-def mol_web_show(mol_smi, show_Hs=False, show_3D = False):
+def mol_web_show(mol_smi):
 
     #---------------------------------------------------------------------------------------------#
     '''
-    mol_web_show(mol_smi, show_Hs=False, show_3D = False)
+    mol_web_show(mol_smi)
     
-    Input: SMILEs of a molecule. Also specify if want the function to show the hydrogens explicitely or the 3D
+    Input: SMILEs of a molecule
     
     Output: image of the molecule as a bokeh plot
     '''
     #---------------------------------------------------------------------------------------------#
 
-    # name of the file name to create
-    filename = 'molecule_image.png'
-
-    #finds the current directory
-    current_directory = os.getcwd()
-
-    #creates a file path to the current directory
-    filepath = os.path.join(current_directory, filename)
-
-    #checks if the file already exists
-    if not os.path.exists(filepath):
-
-        #if no, creates the path
-        with open(filepath, 'a'):
-            pass
-    else:
-
-        #else pass
-        pass
-
+    if not mol_smi:
+        raise ValueError('Incorrect SMILEs input')
+    
     # Generate the image from the molecule
     mol = Chem.MolFromSmiles(mol_smi)
 
-    # Adds the hydrogens to the molecule if specified
-    if show_Hs:
-        mol = Chem.AddHs(mol)
-
-    # Show the molecule in 3D if specified
-    if show_3D:
-        mol = AllChem.EmbedMolecule(mol)
+    if mol is None:
+        raise ValueError('Incorrect SMILEs input')
 
+    #Draws the image
     image = Draw.MolToImage(mol)
 
-    # Save the image to a file
-    image.save(filepath)
-
-    # Creating a Bokeh figure to display the molecule
-    p = figure(width=350, height=350,toolbar_location=None, x_range=(0, 1), y_range=(0, 1))
-    p.image_url(url=[filepath], x=0, y=1, w=1, h=1)
-
-    # Hide grid lines and axes
-    p.xgrid.grid_line_color = None
-    p.ygrid.grid_line_color = None
-    p.xaxis.visible = False
-    p.yaxis.visible = False
+    #stocks the image in a base64 format
+    buffered = BytesIO()
+    image.save(buffered, format="PNG")
+    image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
+    image_url = f"data:image/png;base64,{image_base64}"
 
-    return p
+    # Create a Div element to display the image
+    img_div = Div(text=f'<img src="{image_url}" style="width:350px;height:350px;">')
+   
+    return img_div
  
-def all_in_one(p1, p2, p3, p4):
+def all_in_one(p1, p2, p3):
 
     #---------------------------------------------------------------------------------------------#
     '''
-    all_in_one(p1,p2,p3, p4)
+    all_in_one(p1,p2,p3)
     
     Input: 3 bokeh plots
             Usually used in this package:
                     - p1 : bokeh double plot of mass spectrometry
                     - p2 : image of the molecule
                     - p3 : table of functional groups
-                    - p4 : buttons with info on the molecule
     
-    Output: bokeh page with all 4 graphs well arranged
+    Output: bokeh page with all 3 graphs well arranged
 
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
@@ -2117,16 +2099,23 @@
     
     Input: molecule is a SMILEs format
 
     Output: panel graph of the molecule in 3D and interactive
     '''
     #---------------------------------------------------------------------------------------------#
 
+    if not mol_smi:
+        raise ValueError("Enter a non-empty string as argument")
+
     # Generate 3D coordinates from SMILES string
     mol2 = Chem.MolFromSmiles(mol_smi)
+
+    if not mol2:
+        raise ValueError('Enter a correct SMILEs')
+    
     mol2 = Chem.AddHs(mol2)  # Add hydrogens for better geometry optimization
     AllChem.EmbedMolecule(mol2, randomSeed=42)  # Embed the molecule in 3D space
     AllChem.MMFFOptimizeMolecule(mol2)  # Optimize the geometry using MMFF94 force field
 
     # Create a temporary file to store the 
     with tempfile.NamedTemporaryFile(delete=False) as tmp:
         tmp.write(f"{mol2.GetNumAtoms()}\n\n".encode('utf-8'))  # Write number of atoms
@@ -2141,12 +2130,7 @@
     # Read the data from the temporary file
     mg.read_xyz(tmp_path)
 
     # Create the Plotly figure object
     fig = to_plotly_figure(mg)
 
     return fig
-
-
-
-
-
```

### Comparing `massivechem-5.8/scripts/SMILEs_interpreter.py` & `massivechem-5.9/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/calculate_unsaturation.py` & `massivechem-5.9/scripts/calculate_unsaturation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from rdkit import Chem
-from rdkit.Chem import Draw
 
 def calculate_unsaturation(mol_smile) -> int:
     #---------------------------------------------------------------------------------------------#
     '''
     calculate_unsaturation(mol_smile)
 
     Input: molecule under SMILEs representation
```

### Comparing `massivechem-5.8/scripts/delta_function_plotter.py` & `massivechem-5.9/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/double_plot.py` & `massivechem-5.9/scripts/double_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from bokeh.plotting import figure
 from bokeh.models.tickers import FixedTicker
 from bokeh.layouts import column
 from bokeh.models import WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS
 
-
-
 def double_plot(x_in,y_in):
 
     #---------------------------------------------------------------------------------------------#
     '''
     double_plot(x_in,y_in)
     
     Input: list of masses (x_in) and intensities (y_in)
@@ -74,12 +72,11 @@
     # adds the functionnality to the second figure
 
     p2.add_layout(box)
 
     # creates a layout that displays the 2 graphs
 
     layout = column(p1, p2)
-    print('here')
     return layout
```

### Comparing `massivechem-5.8/scripts/functional_group_display.py` & `massivechem-5.9/scripts/functional_group_display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter
 from bokeh.models.widgets import DataTable, TableColumn
-from bokeh.plotting import show
 import base64
 from io import BytesIO
-from bokeh.models import ColumnDataSource, HTMLTemplateFormatter
-from bokeh.models.widgets import DataTable, TableColumn
-from bokeh.plotting import show
 from rdkit import Chem
 from rdkit.Chem import Draw
 
 
 def functional_group_display(contained_functional_groups):
 
     #---------------------------------------------------------------------------------------------#
```

### Comparing `massivechem-5.8/scripts/functional_group_finder.py` & `massivechem-5.9/scripts/functional_group_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,11 +166,9 @@
         elif 'Amide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
                 if 'Amine' in functional_groups_contained:
                     functional_groups_contained.remove('Amine')
                 if 'Amine' in functional_groups_contained:
                     functional_groups_contained.remove('Amine')
 
-    
-    
     return functional_groups_contained
```

### Comparing `massivechem-5.8/scripts/ionisation_method.py` & `massivechem-5.9/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/main_function.py` & `massivechem-5.9/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/mol_web_show.py` & `massivechem-5.9/scripts/mol_web_show.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from rdkit import Chem
-from rdkit.Chem import Draw, AllChem
+from rdkit.Chem import Draw
 
 from io import BytesIO
 import base64
-
-from bokeh.plotting import show
-from bokeh.io import show
 from bokeh.models import Div
 
 
 def mol_web_show(mol_smi):
 
     #---------------------------------------------------------------------------------------------#
     '''
```

### Comparing `massivechem-5.8/scripts/molecule_list_generator.py` & `massivechem-5.9/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/peak_merger.py` & `massivechem-5.9/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/peak_sorter.py` & `massivechem-5.9/scripts/peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/smiles_to_3D_plot.py` & `massivechem-5.9/scripts/smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/spectrum.py` & `massivechem-5.9/scripts/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from rdkit import Chem
 from rdkit.Chem import Draw
-
-from bokeh.plotting import figure, show, row
+from bokeh.plotting import figure, row
 from bokeh.models.tickers import FixedTicker
-from bokeh.layouts import row, column
-from bokeh.io import show
+from bokeh.layouts import column
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
 from bokeh.models.widgets import DataTable, TableColumn
-
 import base64
 from io import BytesIO
 
 
 def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
 
     #tests for wether the input is valid
@@ -582,8 +579,7 @@
 
     func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
     last = column(img_div, func_group_table)
     final = row(double_graph, last)
     return final
 
-show(spectrum('CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C', True, 0.01))
```

### Comparing `massivechem-5.8/scripts/spectrum_3D.py` & `massivechem-5.9/scripts/spectrum_3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 from rdkit import Chem
 from rdkit.Chem import Draw, AllChem
-
-from bokeh.plotting import figure, show, row
+from bokeh.plotting import figure, row
 from bokeh.models.tickers import FixedTicker
 from bokeh.layouts import row, column
-from bokeh.io import show
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
 from bokeh.models.widgets import DataTable, TableColumn
-
 import base64
 from io import BytesIO
-
 import panel as pn
-import xyz2graph
 import tempfile
 from xyz2graph import MolGraph, to_plotly_figure
 
-
-
-
-
 def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
     if mol_smi == '':
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if imprecision_True_False not in [True, False]:
         raise ValueError('Enter a boolean value')
@@ -612,11 +603,9 @@
     # Creates the final plot
     right_pane = pn.Column(fig_pane, last_pane)
 
     total_plot_pane = pn.Row(left_pane, right_pane)
 
     return total_plot_pane
 
-input_mol = input('Mol SMI: ')
-spectrum_3D(input_mol, True, 0.01).show()
```

### Comparing `massivechem-5.8/scripts/sulphur_nitrogen_adder.py` & `massivechem-5.9/scripts/sulphur_nitrogen_adder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/scripts/sulphur_nitrogen_finder.py` & `massivechem-5.9/scripts/sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_SMILEs_interpreter.py` & `massivechem-5.9/test/test_SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_calculate_unsaturation.py` & `massivechem-5.9/test/test_calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_delta_function_plotter.py` & `massivechem-5.9/test/test_delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_double_plot.py` & `massivechem-5.9/test/test_double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_functional_group_display.py` & `massivechem-5.9/test/test_functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_functional_group_finder.py` & `massivechem-5.9/test/test_functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_ionisation_method.py` & `massivechem-5.9/test/test_ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_main_function.py` & `massivechem-5.9/test/test_main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_mol_web_show.py` & `massivechem-5.9/test/test_mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_molecule_list_generator.py` & `massivechem-5.9/test/test_molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_peak_merger.py` & `massivechem-5.9/test/test_peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_peak_sorter.py` & `massivechem-5.9/test/test_peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_smiles_to_3D_plot.py` & `massivechem-5.9/test/test_smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_spectrum.py` & `massivechem-5.9/test/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_spectrum_3D.py` & `massivechem-5.9/test/test_spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_sulphur_nitrogen_adder.py` & `massivechem-5.9/test/test_sulphur_nitrogen_adder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/test/test_sulphur_nitrogen_finder.py` & `massivechem-5.9/test/test_sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/.gitignore` & `massivechem-5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/LICENSE.txt` & `massivechem-5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/README.md` & `massivechem-5.9/README.md`

 * *Files identical despite different names*

### Comparing `massivechem-5.8/pyproject.toml` & `massivechem-5.9/pyproject.toml`

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
-00000070: 7665 7273 696f 6e20 3d20 2235 2e38 220d  version = "5.8".
+00000070: 7665 7273 696f 6e20 3d20 2235 2e39 220d  version = "5.9".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
```

### Comparing `massivechem-5.8/PKG-INFO` & `massivechem-5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 5.8
+Version: 5.9
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
```

