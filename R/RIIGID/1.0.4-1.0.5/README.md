# Comparing `tmp/RIIGID-1.0.4.tar.gz` & `tmp/RIIGID-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RIIGID-1.0.4.tar", last modified: Tue Apr 23 08:06:01 2024, max compression
+gzip compressed data, was "RIIGID-1.0.5.tar", last modified: Wed May 29 09:40:48 2024, max compression
```

## Comparing `RIIGID-1.0.4.tar` & `RIIGID-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     1065 2024-01-11 12:46:47.000000 RIIGID-1.0.4/LICENSE.md
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2023-12-21 09:34:18.000000 RIIGID-1.0.4/MANIFEST.in
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      345 2024-04-23 08:06:01.324062 RIIGID-1.0.4/PKG-INFO
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3521 2024-02-08 12:37:57.000000 RIIGID-1.0.4/README.rst
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.320062 RIIGID-1.0.4/RIIGID.egg-info/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      345 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/PKG-INFO
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      610 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/SOURCES.txt
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        1 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/dependency_links.txt
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)       29 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/requires.txt
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        7 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/top_level.txt
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/riigid/
--rw-r--r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      504 2024-01-17 09:04:14.000000 RIIGID-1.0.4/riigid/__init__.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      242 2024-04-19 13:07:04.000000 RIIGID-1.0.4/riigid/config.json
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/riigid/convergence/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      118 2024-01-16 15:58:55.000000 RIIGID-1.0.4/riigid/convergence/__init__.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3775 2024-01-16 16:14:49.000000 RIIGID-1.0.4/riigid/convergence/criterion.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     2401 2024-01-16 16:14:49.000000 RIIGID-1.0.4/riigid/convergence/displacement.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    18860 2024-04-19 11:27:53.000000 RIIGID-1.0.4/riigid/fragment.py
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/riigid/library/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-01-11 08:41:35.000000 RIIGID-1.0.4/riigid/library/__init__.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     5818 2024-02-08 12:37:57.000000 RIIGID-1.0.4/riigid/library/misc.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     6801 2024-01-16 16:14:49.000000 RIIGID-1.0.4/riigid/library/rotation.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     1869 2024-01-16 16:14:49.000000 RIIGID-1.0.4/riigid/optimization_step.py
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/riigid/optimizer/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    13952 2024-02-08 12:37:57.000000 RIIGID-1.0.4/riigid/optimizer/Deprecated_GDWAS.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    15707 2024-04-19 11:05:43.000000 RIIGID-1.0.4/riigid/optimizer/GDWAS.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      153 2024-01-25 08:48:31.000000 RIIGID-1.0.4/riigid/optimizer/__init__.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     2457 2024-02-08 12:37:57.000000 RIIGID-1.0.4/riigid/optimizer/optimizer.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    13522 2024-04-19 13:12:28.000000 RIIGID-1.0.4/riigid/riigid.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    19025 2024-04-19 13:27:18.000000 RIIGID-1.0.4/riigid/structure.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)       38 2024-04-23 08:06:01.324062 RIIGID-1.0.4/setup.cfg
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      544 2024-04-23 08:02:07.000000 RIIGID-1.0.4/setup.py
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-05-29 09:40:48.160157 RIIGID-1.0.5/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     1065 2024-01-11 12:46:47.000000 RIIGID-1.0.5/LICENSE.md
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2023-12-21 09:34:18.000000 RIIGID-1.0.5/MANIFEST.in
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      345 2024-05-29 09:40:48.160157 RIIGID-1.0.5/PKG-INFO
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3527 2024-04-25 11:08:25.000000 RIIGID-1.0.5/README.rst
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-05-29 09:40:48.156156 RIIGID-1.0.5/RIIGID.egg-info/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      345 2024-05-29 09:40:48.000000 RIIGID-1.0.5/RIIGID.egg-info/PKG-INFO
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      610 2024-05-29 09:40:48.000000 RIIGID-1.0.5/RIIGID.egg-info/SOURCES.txt
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        1 2024-05-29 09:40:48.000000 RIIGID-1.0.5/RIIGID.egg-info/dependency_links.txt
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)       29 2024-05-29 09:40:48.000000 RIIGID-1.0.5/RIIGID.egg-info/requires.txt
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        7 2024-05-29 09:40:48.000000 RIIGID-1.0.5/RIIGID.egg-info/top_level.txt
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-05-29 09:40:48.160157 RIIGID-1.0.5/riigid/
+-rw-r--r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      504 2024-01-17 09:04:14.000000 RIIGID-1.0.5/riigid/__init__.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      242 2024-04-19 13:07:04.000000 RIIGID-1.0.5/riigid/config.json
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-05-29 09:40:48.160157 RIIGID-1.0.5/riigid/convergence/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      118 2024-01-16 15:58:55.000000 RIIGID-1.0.5/riigid/convergence/__init__.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3775 2024-01-16 16:14:49.000000 RIIGID-1.0.5/riigid/convergence/criterion.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     2401 2024-01-16 16:14:49.000000 RIIGID-1.0.5/riigid/convergence/displacement.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    18956 2024-05-28 09:15:29.000000 RIIGID-1.0.5/riigid/fragment.py
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-05-29 09:40:48.160157 RIIGID-1.0.5/riigid/library/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-01-11 08:41:35.000000 RIIGID-1.0.5/riigid/library/__init__.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     5818 2024-02-08 12:37:57.000000 RIIGID-1.0.5/riigid/library/misc.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     6801 2024-01-16 16:14:49.000000 RIIGID-1.0.5/riigid/library/rotation.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3860 2024-05-28 13:34:41.000000 RIIGID-1.0.5/riigid/optimization_step.py
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-05-29 09:40:48.160157 RIIGID-1.0.5/riigid/optimizer/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    13968 2024-05-28 10:47:34.000000 RIIGID-1.0.5/riigid/optimizer/Deprecated_GDWAS.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    15723 2024-05-28 10:47:35.000000 RIIGID-1.0.5/riigid/optimizer/GDWAS.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      153 2024-01-25 08:48:31.000000 RIIGID-1.0.5/riigid/optimizer/__init__.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     2457 2024-02-08 12:37:57.000000 RIIGID-1.0.5/riigid/optimizer/optimizer.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    14297 2024-05-29 07:25:07.000000 RIIGID-1.0.5/riigid/riigid.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    19025 2024-04-19 13:27:18.000000 RIIGID-1.0.5/riigid/structure.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)       38 2024-05-29 09:40:48.160157 RIIGID-1.0.5/setup.cfg
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      544 2024-05-28 09:16:20.000000 RIIGID-1.0.5/setup.py
```

### Comparing `RIIGID-1.0.4/LICENSE.md` & `RIIGID-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.4/README.rst` & `RIIGID-1.0.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 Usage
 -----
 
 The user has to define the *atomic system* (as an ASE Atoms object), define the *fragments* and choose a *calculator*. Thanks to RIIGID's reliance on the ASE package, many different atomic structure codes (e.g.: `VASP <https://www.vasp.at/>`_) can be used as a calculator.
 
 RIIGID comes with its own optimizers and convergence criteria. The user can choose explicitly which optimizer and convergence criterion to use, or keep the defaults.
 
-Information about the optimization is written to the standard output. 
+Information about the optimization is written to RIIGID's own output files. 
 Additionally, an ASE trajectory file is produced. 
 
 Have a look at the `demo folder <https://github.com/siegfriedkaidisch/RIIGID/tree/main/demo>`_ for working examples!
 Note, that for the demo to work, ASE must be able to execute your VASP installation, see the `ASE documentation <https://wiki.fysik.dtu.dk/ase/ase/calculators/vasp.html#environment-variables.>`_
 
 
 Known issues
```

### Comparing `RIIGID-1.0.4/RIIGID.egg-info/SOURCES.txt` & `RIIGID-1.0.5/RIIGID.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.4/riigid/convergence/criterion.py` & `RIIGID-1.0.5/riigid/convergence/criterion.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.4/riigid/convergence/displacement.py` & `RIIGID-1.0.5/riigid/convergence/displacement.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.4/riigid/fragment.py` & `RIIGID-1.0.5/riigid/fragment.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,21 +288,22 @@
 
         Returns
         -------
         numpy.ndarray of shape (n_atoms_in_fragment,3)
             The positions of the fragment's atoms after the transformation; [Å]
 
         """
-        axis, angle = self.get_rotation_axis_and_angle_from_torque(
-            torque_on_center=torque_on_center, stepsize=stepsize
-        )
-
-        if angle != 0:
-            self.atoms.rotate(angle, axis, self.atoms.get_center_of_mass())
-            self.update_rotation_properties(angle=angle, axis=axis)
+        if len(self.atoms) > 1:
+            axis, angle = self.get_rotation_axis_and_angle_from_torque(
+                torque_on_center=torque_on_center, stepsize=stepsize
+            )
+
+            if angle != 0:
+                self.atoms.rotate(angle, axis, self.atoms.get_center_of_mass())
+                self.update_rotation_properties(angle=angle, axis=axis)
 
         return copy(self.atoms.positions)
 
     def get_rotation_axis_and_angle_from_torque(self, torque_on_center, stepsize=1.0):
         """Get the (normalized) rotation axis and angle corresponding to the applied applied torque and the given stepsize.
 
         Parameters
@@ -408,16 +409,17 @@
 
         Returns
         -------
         numpy.ndarray of shape (n_atoms_in_fragment,3)
             The positions of the fragment's atoms after the transformation; [Å]
 
         """
-        self.atoms.rotate(angle, axis, self.atoms.get_center_of_mass())
-        self.update_rotation_properties(angle=angle, axis=axis)
+        if len(self.atoms) > 1:
+            self.atoms.rotate(angle, axis, self.atoms.get_center_of_mass())
+            self.update_rotation_properties(angle=angle, axis=axis)
         return copy(self.atoms.positions)
 
     def move_random_step(self, displacement, angle, respect_restrictions, seed=1234):
         """Randomly rotate and translate the fragment.
 
         Useful to escape saddle points, especially when starting a new optimization.
```

### Comparing `RIIGID-1.0.4/riigid/library/misc.py` & `RIIGID-1.0.5/riigid/library/misc.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.4/riigid/library/rotation.py` & `RIIGID-1.0.5/riigid/library/rotation.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.4/riigid/optimizer/Deprecated_GDWAS.py` & `RIIGID-1.0.5/riigid/optimizer/Deprecated_GDWAS.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             _, _ = updated_structure.move(
                 forces=self.current_forces, stepsize=self.stepsize
             )
 
             # Add Optimization step to history
             new_step = OptimizationStep(
                 structure=self.current_structure,
-                forces=self.current_forces,
+                force_on_atoms=self.current_forces,
                 energy=self.current_energy,
                 updated_structure=updated_structure,
             )
             self.optimization_history.append(new_step)
 
             # Prepare next iteration
             self.iteration += 1
@@ -260,15 +260,15 @@
             prev_energy = self.optimization_history[-1].energy
             current_energy = self.current_energy
             if prev_energy < current_energy:
                 # Return to structure, forces and energy, previous to the last update
                 self.current_structure = deepcopy(
                     self.optimization_history[-1].structure
                 )
-                self.current_forces = copy(self.optimization_history[-1].forces)
+                self.current_forces = copy(self.optimization_history[-1].force_on_atoms)
                 self.current_energy = copy(self.optimization_history[-1].energy)
                 self.optimization_history.pop()
 
     def adapt_stepsize_to_prevent_too_large_steps(self, max_atomic_displacement):
         """Prevent too large atomic movement.
 
         If max_atomic_displacement > self.max_step, the stepsize is lowered, such that
```

### Comparing `RIIGID-1.0.4/riigid/optimizer/GDWAS.py` & `RIIGID-1.0.5/riigid/optimizer/GDWAS.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             _, _ = updated_structure.move(
                 forces=self.current_forces, stepsize=self.stepsize
             )
 
             # Add Optimization step to history
             new_step = OptimizationStep(
                 structure=self.current_structure,
-                forces=self.current_forces,
+                force_on_atoms=self.current_forces,
                 energy=self.current_energy,
                 updated_structure=updated_structure,
             )
             self.optimization_history.append(new_step)
 
             # Prepare next iteration
             self.iteration += 1
@@ -264,15 +264,15 @@
             prev_energy = self.optimization_history[-1].energy
             current_energy = self.current_energy
             if prev_energy < current_energy:
                 # Return to structure, forces and energy, previous to the last update
                 self.current_structure = deepcopy(
                     self.optimization_history[-1].structure
                 )
-                self.current_forces = copy(self.optimization_history[-1].forces)
+                self.current_forces = copy(self.optimization_history[-1].force_on_atoms)
                 self.current_energy = copy(self.optimization_history[-1].energy)
                 self.optimization_history.pop()
 
     def adapt_stepsize_to_prevent_too_large_steps(self):
         """Prevent too large movement of the fragments.
 
         If a fragment is found to translate more than self.max_trans, the stepsize is lowered in such a way,
```

### Comparing `RIIGID-1.0.4/riigid/optimizer/optimizer.py` & `RIIGID-1.0.5/riigid/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.4/riigid/riigid.py` & `RIIGID-1.0.5/riigid/riigid.py`

 * *Files 10% similar despite different names*

```diff
@@ -329,12 +329,27 @@
         )
 
     @redirect_stdout_to_file(out_file)
     def save_optimization_summary(self):
         """Save Information about the optimization to a separate file."""
         fn = opt_file
         with open(fn, "w") as file:
-            file.write("Summary of Optimization:\n")
+            # Write the header
+            # file.write("Summary of Optimization:\n")
+            file.write(
+                f"{'':<6}|{'':>20}|{'Max. Force on Fragments':>25}|{'Max. Torque on Fragments':>25}|{'Max. Force on Atoms':>25}|\n"
+            )
+            file.write(
+                f"{'Step':<6}|{'Energy [eV]':>20}|{'[eV/A]':>20}{'#':>5}|{'[eV]':>20}{'#':>5}|{'[eV/A]':>20}{'#':>5}|\n"
+            )
+            file.write("=" * (6 + 20 + 25 + 25 + 25 + 5 * 1) + "\n")
+
+            # Write the data rows
             optimization_history = self.optimizer.optimization_history
             for iteration, step in enumerate(optimization_history):
-                file.write("Optimization Step " + str(iteration) + ":\n")
-                file.write("   Energy [eV]: " + str(step.energy) + "\n")
+                energy = step.energy
+                fmax_fragments = step.max_force_on_fragment
+                tmax_fragments = step.max_torque_on_fragment
+                fmax_atoms = step.max_force_on_atom
+                file.write(
+                    f"{iteration:<6}|{energy:>20.10f}|{fmax_fragments[0]:>20.10f}{fmax_fragments[1]:>5}|{tmax_fragments[0]:>20.10f}{tmax_fragments[1]:>5}|{fmax_atoms[0]:>20.10f}{fmax_atoms[1]:>5}|\n"
+                )
```

### Comparing `RIIGID-1.0.4/riigid/structure.py` & `RIIGID-1.0.5/riigid/structure.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.4/setup.py` & `RIIGID-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RIIGID",
-    version="1.0.4",
+    version="1.0.5",
     description="RIIGID - RIgid Interface Geometry IDentification",
     packages=find_packages(),
     license="MIT",
     python_requires=">3.8.0",
     url="https://github.com/siegfriedkaidisch/RIIGID",
     author="Siegfried Kaidisch",
     author_email="siegfried.kaidisch@uni-graz.at",
```

