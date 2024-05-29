# Comparing `tmp/pondpy-0.1.1.tar.gz` & `tmp/pondpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pondpy-0.1.1.tar", max compression
+gzip compressed data, was "pondpy-0.1.2.tar", max compression
```

## Comparing `pondpy-0.1.1.tar` & `pondpy-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     1092 2024-05-24 22:17:18.743268 pondpy-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2024-05-21 20:36:12.387933 pondpy-0.1.1/pondpy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 13:18:41.574068 pondpy-0.1.1/pondpy/analysis/__init__.py
--rw-r--r--   0        0        0    30994 2024-05-24 22:17:18.743268 pondpy-0.1.1/pondpy/analysis/fem_analysis.py
--rw-r--r--   0        0        0    18848 2024-05-24 22:17:18.743268 pondpy-0.1.1/pondpy/analysis/pond_analysis.py
--rw-r--r--   0        0        0    11800 2024-05-25 01:57:14.493351 pondpy-0.1.1/pondpy/pondpy.py
--rw-r--r--   0        0        0      584 2024-05-25 05:31:43.480914 pondpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5381 2024-05-25 05:31:43.478652 pondpy-0.1.1/README.md
--rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 pondpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-24 22:17:18.743268 pondpy-0.1.2/LICENSE
+-rw-r--r--   0        0        0      466 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:18:41.574068 pondpy-0.1.2/pondpy/analysis/__init__.py
+-rw-r--r--   0        0        0    31007 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/analysis/fem_analysis.py
+-rw-r--r--   0        0        0    19704 2024-05-29 20:50:24.129982 pondpy-0.1.2/pondpy/analysis/pond_analysis.py
+-rw-r--r--   0        0        0        0 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/design/__init__.py
+-rw-r--r--   0        0        0       70 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/design/steel_beam_design.py
+-rw-r--r--   0        0        0       72 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/design/steel_joist_design.py
+-rw-r--r--   0        0        0    11405 2024-05-29 20:55:57.137409 pondpy-0.1.2/pondpy/pondpy.py
+-rw-r--r--   0        0        0      584 2024-05-29 20:57:47.729009 pondpy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5529 2024-05-26 23:17:09.445725 pondpy-0.1.2/README.md
+-rw-r--r--   0        0        0     6006 1970-01-01 00:00:00.000000 pondpy-0.1.2/PKG-INFO
```

### Comparing `pondpy-0.1.1/LICENSE` & `pondpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pondpy-0.1.1/pondpy/analysis/fem_analysis.py` & `pondpy-0.1.2/pondpy/analysis/fem_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class SteelBeamSize:
     '''
     A class representing a steel beam size.
 
     ...
 
     Attributes
-        ----------
+    ----------
     e_mod : int or float
         elastic modulus of steel in ksi
     name : str
         name of the steel beam size
     properties : steelpy object
         steelpy object containing properties for the specified steel beam size
     section_type : str
@@ -740,15 +740,15 @@
         lval_bmd_count = 0
         for i_lval_bmd in range(len(self.model_nodes)):
             lval_bmd[i_lval_bmd+lval_bmd_count] = self.model_nodes[i_lval_bmd]/12
             lval_bmd[i_lval_bmd+lval_bmd_count+1] = self.model_nodes[i_lval_bmd]/12
             lval_bmd_count += 1
         
         plt.figure()
-        plt.plot(lval_bmd.tolist(), bmd_val.tolist())
+        plt.plot(lval_bmd.tolist(), bmd_val.tolist(),'b-')
 
         plt.xlabel('Length (ft)')
         plt.ylabel(f'Bending Moment (k-ft)')
 
         plt.grid()
 
         return plt
@@ -772,15 +772,15 @@
             G_dof = self.dof_num[i_node][1]
             if G_dof != 0:
                 y_disp.append(self.global_displacement[G_dof-1][0]*scale)
             else:
                 y_disp.append(0.0)
         
         plt.figure()
-        plt.plot([x/12 for x in self.model_nodes], y_disp)
+        plt.plot([x/12 for x in self.model_nodes], y_disp, 'b-')
 
         plt.xlabel('Length (ft)')
         plt.ylabel(f'Deflection (in) - Scale={scale}:1')
 
         plt.grid()
 
         return plt
@@ -822,15 +822,15 @@
         lval_sfd_count = 0
         for i_lval_sfd in range(len(self.model_nodes)):
             lval_sfd[i_lval_sfd+lval_sfd_count] = self.model_nodes[i_lval_sfd]/12
             lval_sfd[i_lval_sfd+lval_sfd_count+1] = self.model_nodes[i_lval_sfd]/12
             lval_sfd_count += 1
 
         plt.figure()
-        plt.plot(lval_sfd.tolist(), sfd_val.tolist())
+        plt.plot(lval_sfd.tolist(), sfd_val.tolist(), 'b-')
 
         plt.xlabel('Length (ft)')
         plt.ylabel(f'Shear Force (k)')
 
         plt.grid()
 
         return plt
```

### Comparing `pondpy-0.1.1/pondpy/analysis/pond_analysis.py` & `pondpy-0.1.2/pondpy/analysis/pond_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,27 @@
         self.dead_load = dead_load # Units: k/in^2
         self.rain_load = rain_load # Units: k/in^2
         self.include_sw = include_sw
 
 class PrimaryMember(Beam):
     '''
     A class representing a primary member in the roof bay.
+
+    Attributes
+    ----------
+    dloads : list
+        list of dist load objects
+    length : float
+        length of the beam
+    size : steel beam size object
+        steel beam size object for the beam
+    supports : list
+        list of tuples indicating location and type of beam supports
+    ploads : list
+        list of point load objects
     '''
     pass
 
 class PrimaryFraming:
     '''
     A class representing the primary members in the framing system in the roof bay.
 
@@ -427,19 +440,22 @@
             impounded_length = bay_length
         else:
             impounded_length = d_impounded_i/roof_slope # Length of impounded water along secondary framing in inches
         
 
         # First deal with the primary members
         impounded_depth_p = {}
-        impounded_depth_p[0] = [d_impounded_i for _ in range(len(self.primary_models[0].model_nodes))]
-        if impounded_length <= bay_length:
-            impounded_depth_p[1] = [0.0 for _ in range(len(self.primary_models[0].model_nodes))]
-        elif impounded_length > bay_length:
-            impounded_depth_p[1] = [d_impounded_i-roof_slope*bay_length for _ in range(len(self.primary_models[0].model_nodes))]
+        for i_pmodel, p_model in enumerate(self.primary_models):
+            if i_pmodel == 0:
+                impounded_depth_p[i_pmodel] = [d_impounded_i for _ in range(len(p_model.model_nodes))]
+            else:
+                if impounded_length <= bay_length:
+                    impounded_depth_p[i_pmodel] = [0.0 for _ in range(len(p_model.model_nodes))]
+                elif impounded_length > bay_length:
+                    impounded_depth_p[1] = [d_impounded_i-roof_slope*bay_length for _ in range(len(p_model.model_nodes))]
 
         # Next deal with the secondary members
         impounded_depth_s = {}
         for idx, s_model in enumerate(self.secondary_models):
             cur_nodes = s_model.model_nodes
             nodal_depth = []
             for node in cur_nodes:
@@ -448,15 +464,15 @@
                 elif node > impounded_length:
                     cur_depth = 0.0
 
                 nodal_depth.append(cur_depth)
             
             impounded_depth_s[idx] = nodal_depth
 
-        self.initial_impounded_depth = {
+        return {
             'Primary':impounded_depth_p,
             'Secondary':impounded_depth_s,
         }
 
     def analyze_roof_bay(self, rain_load):
         '''
         Analyzes the roof bay for the dead load and the input rain loads.
@@ -497,20 +513,33 @@
 
         Returns
         -------
         None
         '''
         self._create_primary_models()
         self._create_secondary_models()
-        self._initial_impounded_water_depth()
+        self.initial_impounded_depth = self._initial_impounded_water_depth()
         self.initial_secondary_rl = self._get_secondary_rl(impounded_depth=self.initial_impounded_depth)
 
 class SecondaryMember(Beam):
     '''
     A class representing a secondary member in the roof bay.
+
+    Attributes
+    ----------
+    dloads : list
+        list of dist load objects
+    length : float
+        length of the beam
+    size : steel beam size object
+        steel beam size object for the beam
+    supports : list
+        list of tuples indicating location and type of beam supports
+    ploads : list
+        list of point load objects
     '''
     pass
 
 class SecondaryFraming:
     '''
     A class representing the secondary members in the framing system in the roof bay.
```

### Comparing `pondpy-0.1.1/pondpy/pondpy.py` & `pondpy-0.1.2/pondpy/pondpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from scipy import integrate
 import time
 
-from pondpy.analysis.pond_analysis import (
+from pondpy import (
     RoofBay,
     RoofBayModel,
 )
 
 class PondPyModel:
     '''
     A class to represent a pondpy analysis object.
@@ -75,15 +75,15 @@
         self.mirrored_right = mirrored_right
         self.primary_framing = primary_framing
         self.secondary_framing = secondary_framing
         self.show_results = show_results
         self.stop_criterion = stop_criterion
 
         self._create_roof_bay_model()
-        self.impounded_depth = self.roof_bay_model.initial_impounded_depth
+        self.impounded_depth = self.roof_bay_model._initial_impounded_water_depth()
 
     def _calculate_impounded_weight(self, impounded_depth):
         '''
         Calculates the weight of the impounded water on the roof bay.
 
         Parameters
         ----------
@@ -186,15 +186,15 @@
 
             impounded_depth_s[i_smodel] = nodal_depth
 
         # Next determine the depth of water considering the straight-line depth and deflection
         # at each node for each primary member.
         # Note: Impounded depth for the primary members is not required for analysis. All rain
         # loads are assumed to be transferred to the primary members by the secondary members.
-        impounded_depth_p = {}
+        '''impounded_depth_p = {}
         for i_pmodel, p_model in enumerate(self.roof_bay_model.primary_models):
             cur_disp = []
             for i_node in range(len(p_model.model_nodes)):
                 G_dof = p_model.dof_num[i_node][1]
                 if G_dof != 0:
                     cur_disp.append(p_model.global_displacement[G_dof-1][0])
                 else:
@@ -202,20 +202,19 @@
 
             nodal_depth = []
             if i_pmodel == 0:
                 for i_node, node in enumerate(p_model.model_nodes):
                     cur_depth = self.roof_bay_model.initial_impounded_depth['Primary'][i_pmodel][i_node] - cur_disp[i_node]
                     nodal_depth.append(cur_depth)
                         
-            impounded_depth_p[i_pmodel] = nodal_depth
+            impounded_depth_p[i_pmodel] = nodal_depth'''
 
         impounded_depth = {
-            'Primary':impounded_depth_p,
             'Secondary':impounded_depth_s,
-        }           
+        }         
 
         return impounded_depth
 
     def _create_roof_bay_model(self):
         '''
         Creates the roof bay model to be used in the iterative analysis.
 
@@ -238,22 +237,14 @@
         ----------
         None
 
         Returns
         -------
         output : dict
             dictionary of output variables
-            Keys
-            ----
-            Iterations --> iterations : int
-                number of iterations run
-            Time --> time_elapsed : float
-                amount of time the analysis took to run in seconds
-            Weight --> impounded_weight : list
-                list of impounded weight for each iteration
         '''
         iteration = 0
         impounded_weight = []
         out_str = 'Iteration\t|\tWater Weight (k)\t|\tDifference\n'
         start = time.time()
         while True:
             rain_load = self.roof_bay_model._get_secondary_rl(self.impounded_depth)
```

### Comparing `pondpy-0.1.1/pyproject.toml` & `pondpy-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pondpy"
-version = "0.1.1"
+version = "0.1.2"
 description = "Package to aid in the design of low-slope roof systems for ponding stability and impounded rain load."
 authors = ["Matthew Upshaw <matthew.upshaw02@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `pondpy-0.1.1/README.md` & `pondpy-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -138,7 +138,11 @@
   support_reactions = [member.support_reactions[node] for node in support_nodes]
   ```
 
 Several other attributes of the BeamModel object can be accessed in a similar
 fashion.
 
 Note that only the final analysis results can currently be accessed.
+
+### Additional Information
+- [Documentation](https://pondpy.readthedocs.io/en/latest/)
+- [PyPI Distribution](https://pypi.org/project/pondpy/)
```

### Comparing `pondpy-0.1.1/PKG-INFO` & `pondpy-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pondpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package to aid in the design of low-slope roof systems for ponding stability and impounded rain load.
 License: MIT
 Author: Matthew Upshaw
 Author-email: matthew.upshaw02@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -157,7 +157,11 @@
   ```
 
 Several other attributes of the BeamModel object can be accessed in a similar
 fashion.
 
 Note that only the final analysis results can currently be accessed.
 
+### Additional Information
+- [Documentation](https://pondpy.readthedocs.io/en/latest/)
+- [PyPI Distribution](https://pypi.org/project/pondpy/)
+
```

