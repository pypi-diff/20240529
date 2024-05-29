# Comparing `tmp/pwdata-0.2.13.tar.gz` & `tmp/pwdata-0.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwdata-0.2.13.tar", last modified: Tue May 28 02:07:45 2024, max compression
+gzip compressed data, was "pwdata-0.2.14.tar", last modified: Wed May 29 03:46:18 2024, max compression
```

## Comparing `pwdata-0.2.13.tar` & `pwdata-0.2.14.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.129897 pwdata-0.2.13/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    35148 2024-02-27 08:01:20.000000 pwdata-0.2.13/LICENSE
--rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      660 2024-05-28 02:07:45.129295 pwdata-0.2.13/PKG-INFO
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       51 2024-03-08 09:41:47.000000 pwdata-0.2.13/README.md
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.011114 pwdata-0.2.13/pwdata/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      283 2024-03-05 03:01:36.000000 pwdata-0.2.13/pwdata/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2657 2024-02-28 03:42:10.000000 pwdata-0.2.13/pwdata/atomconfig.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.029347 pwdata-0.2.13/pwdata/build/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:13.000000 pwdata-0.2.13/pwdata/build/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5902 2024-02-27 07:43:28.000000 pwdata-0.2.13/pwdata/build/cell.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2815 2024-02-28 03:47:20.000000 pwdata-0.2.13/pwdata/build/geometry.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3886 2024-03-05 02:57:00.000000 pwdata-0.2.13/pwdata/build/supercells.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    15467 2024-03-29 08:35:53.000000 pwdata-0.2.13/pwdata/build/write_struc.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.082070 pwdata-0.2.13/pwdata/calculators/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:16.000000 pwdata-0.2.13/pwdata/calculators/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14172 2024-02-27 07:43:28.000000 pwdata-0.2.13/pwdata/calculators/const.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     4873 2024-02-27 07:50:22.000000 pwdata-0.2.13/pwdata/calculators/unitconvert_lmps.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     7964 2024-02-27 07:43:28.000000 pwdata-0.2.13/pwdata/calculators/units.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14250 2024-02-28 03:43:29.000000 pwdata-0.2.13/pwdata/cp2kdata.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5439 2024-03-01 02:53:29.000000 pwdata-0.2.13/pwdata/datasets_saver.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6069 2024-05-27 01:29:52.000000 pwdata-0.2.13/pwdata/deepmd.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     8826 2024-02-28 03:44:14.000000 pwdata-0.2.13/pwdata/dump.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1649 2024-05-16 06:19:11.000000 pwdata-0.2.13/pwdata/extendedxyz.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    11611 2024-04-08 08:59:39.000000 pwdata-0.2.13/pwdata/image.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    13928 2024-02-28 03:45:13.000000 pwdata-0.2.13/pwdata/lammpsdata.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1661 2024-02-27 07:43:28.000000 pwdata-0.2.13/pwdata/lmps.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    16592 2024-03-27 09:50:17.000000 pwdata-0.2.13/pwdata/main.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5350 2024-03-18 07:39:03.000000 pwdata-0.2.13/pwdata/movement.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2587 2024-03-05 02:49:08.000000 pwdata-0.2.13/pwdata/movement_saver.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6925 2024-04-08 09:00:41.000000 pwdata-0.2.13/pwdata/outcar.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.128104 pwdata-0.2.13/pwdata/pertub/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:19.000000 pwdata-0.2.13/pwdata/pertub/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     9133 2024-03-05 02:56:31.000000 pwdata-0.2.13/pwdata/pertub/perturbation.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2446 2024-03-05 02:56:46.000000 pwdata-0.2.13/pwdata/pertub/scale.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3066 2024-02-28 03:46:19.000000 pwdata-0.2.13/pwdata/poscar.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2837 2024-04-08 07:46:55.000000 pwdata-0.2.13/pwdata/pwmlff.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.128637 pwdata-0.2.13/pwdata.egg-info/
--rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      660 2024-05-28 02:07:44.000000 pwdata-0.2.13/pwdata.egg-info/PKG-INFO
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      777 2024-05-28 02:07:44.000000 pwdata-0.2.13/pwdata.egg-info/SOURCES.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        1 2024-05-28 02:07:44.000000 pwdata-0.2.13/pwdata.egg-info/dependency_links.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        7 2024-05-28 02:07:44.000000 pwdata-0.2.13/pwdata.egg-info/top_level.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       38 2024-05-28 02:07:45.130009 pwdata-0.2.13/setup.cfg
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      825 2024-05-28 02:07:26.000000 pwdata-0.2.13/setup.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-29 03:46:18.774441 pwdata-0.2.14/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    35148 2024-02-27 08:01:20.000000 pwdata-0.2.14/LICENSE
+-rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      660 2024-05-29 03:46:18.773799 pwdata-0.2.14/PKG-INFO
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       51 2024-03-08 09:41:47.000000 pwdata-0.2.14/README.md
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-29 03:46:17.325539 pwdata-0.2.14/pwdata/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      283 2024-03-05 03:01:36.000000 pwdata-0.2.14/pwdata/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2657 2024-02-28 03:42:10.000000 pwdata-0.2.14/pwdata/atomconfig.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-29 03:46:18.714936 pwdata-0.2.14/pwdata/build/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:13.000000 pwdata-0.2.14/pwdata/build/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5902 2024-02-27 07:43:28.000000 pwdata-0.2.14/pwdata/build/cell.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2815 2024-02-28 03:47:20.000000 pwdata-0.2.14/pwdata/build/geometry.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3886 2024-03-05 02:57:00.000000 pwdata-0.2.14/pwdata/build/supercells.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    16158 2024-05-29 03:45:25.000000 pwdata-0.2.14/pwdata/build/write_struc.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-29 03:46:18.744953 pwdata-0.2.14/pwdata/calculators/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:16.000000 pwdata-0.2.14/pwdata/calculators/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14172 2024-02-27 07:43:28.000000 pwdata-0.2.14/pwdata/calculators/const.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     4873 2024-02-27 07:50:22.000000 pwdata-0.2.14/pwdata/calculators/unitconvert_lmps.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     7964 2024-02-27 07:43:28.000000 pwdata-0.2.14/pwdata/calculators/units.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14250 2024-02-28 03:43:29.000000 pwdata-0.2.14/pwdata/cp2kdata.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5439 2024-03-01 02:53:29.000000 pwdata-0.2.14/pwdata/datasets_saver.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6069 2024-05-27 01:29:52.000000 pwdata-0.2.14/pwdata/deepmd.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     8826 2024-02-28 03:44:14.000000 pwdata-0.2.14/pwdata/dump.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1649 2024-05-16 06:19:11.000000 pwdata-0.2.14/pwdata/extendedxyz.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    11611 2024-04-08 08:59:39.000000 pwdata-0.2.14/pwdata/image.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    13928 2024-02-28 03:45:13.000000 pwdata-0.2.14/pwdata/lammpsdata.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1661 2024-02-27 07:43:28.000000 pwdata-0.2.14/pwdata/lmps.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    16592 2024-03-27 09:50:17.000000 pwdata-0.2.14/pwdata/main.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5350 2024-03-18 07:39:03.000000 pwdata-0.2.14/pwdata/movement.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2587 2024-03-05 02:49:08.000000 pwdata-0.2.14/pwdata/movement_saver.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6925 2024-04-08 09:00:41.000000 pwdata-0.2.14/pwdata/outcar.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-29 03:46:18.772489 pwdata-0.2.14/pwdata/pertub/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:19.000000 pwdata-0.2.14/pwdata/pertub/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     9133 2024-03-05 02:56:31.000000 pwdata-0.2.14/pwdata/pertub/perturbation.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2446 2024-03-05 02:56:46.000000 pwdata-0.2.14/pwdata/pertub/scale.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3066 2024-02-28 03:46:19.000000 pwdata-0.2.14/pwdata/poscar.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2837 2024-04-08 07:46:55.000000 pwdata-0.2.14/pwdata/pwmlff.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-29 03:46:18.773105 pwdata-0.2.14/pwdata.egg-info/
+-rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      660 2024-05-29 03:46:16.000000 pwdata-0.2.14/pwdata.egg-info/PKG-INFO
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      777 2024-05-29 03:46:16.000000 pwdata-0.2.14/pwdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        1 2024-05-29 03:46:16.000000 pwdata-0.2.14/pwdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        7 2024-05-29 03:46:16.000000 pwdata-0.2.14/pwdata.egg-info/top_level.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       38 2024-05-29 03:46:18.774556 pwdata-0.2.14/setup.cfg
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      825 2024-05-29 03:45:49.000000 pwdata-0.2.14/setup.py
```

### Comparing `pwdata-0.2.13/LICENSE` & `pwdata-0.2.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/PKG-INFO` & `pwdata-0.2.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdata
-Version: 0.2.13
+Version: 0.2.14
 Summary: pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.
 Home-page: https://github.com/LonxunQuantum/pwdata
 Author: LonxunQuantum
 Author-email: lonxun@pwmat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pwdata-0.2.13/pwdata/atomconfig.py` & `pwdata-0.2.14/pwdata/atomconfig.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/build/cell.py` & `pwdata-0.2.14/pwdata/build/cell.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/build/geometry.py` & `pwdata-0.2.14/pwdata/build/geometry.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/build/supercells.py` & `pwdata-0.2.14/pwdata/build/supercells.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/build/write_struc.py` & `pwdata-0.2.14/pwdata/build/write_struc.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,39 +76,42 @@
                               axis=1)
                 if sum(mask) != 1:
                     raise RuntimeError(
                         'VASP requires that the direction of FixedLine '
                         'constraints is parallel with one of the cell axis')
                 sflags[constr.a] = ~mask'''
 
-    if sort:
-        if len(image.get_atomic_numbers()) == 0:
-            ind = np.argsort(image.atom_types_image)
-            symbols = np.array(image.atom_types_image)[ind]
-        else:
-            ind = np.argsort(image.get_atomic_numbers())
-            symbols = np.array(image.get_atomic_numbers())[ind]
-        coord = np.array(coord)[ind]
-        # if constraints:
-        #     sflags = sflags[ind]
-    else:
-        symbols = image.atom_types_image
-
     # Create a list sc of (symbol, count) pairs
     if symbol_count:
         # sc = symbol_count
         pass
     elif image.atom_type is None:
         sc = Counter(symbols)
         atom_type = list(sc.keys())
         atom_type_num = list(sc.values())
     else:
         atom_type = image.atom_type
         atom_type_num = image.atom_type_num
 
+    atom_types_image = np.array(image.atom_types_image)
+
+    if sort:
+        if len(image.get_atomic_numbers()) == 0:
+            indices_dict = {type: np.where(atom_types_image == type)[0] for type in atom_type}
+            sorted_indices = np.concatenate([np.sort(indices) for indices in indices_dict.values()])
+            symbols = atom_types_image[sorted_indices]
+        else:
+            sorted_indices = np.argsort(image.get_atomic_numbers())
+            symbols = np.array(image.get_atomic_numbers())[sorted_indices]
+        coord = np.array(coord)[sorted_indices]
+        # if constraints:
+        #     sflags = sflags[ind]
+    else:
+        symbols = image.atom_types_image
+
     # Write to file
     output_file = open(os.path.join(filepath, data_name), 'w')
     output_file.write('%d\n' % atom_nums)
     output_file.write('Lattice vector\n')
     for i in range(3):
         output_file.write('%19.16f %19.16f %19.16f\n' % tuple(image.lattice[i]))
     output_file.write(' Position, move_x, mov_y, move_z\n')
@@ -193,38 +196,41 @@
                               axis=1)
                 if sum(mask) != 1:
                     raise RuntimeError(
                         'VASP requires that the direction of FixedLine '
                         'constraints is parallel with one of the cell axis')
                 sflags[constr.a] = ~mask'''
     
-    if sort:
-        if len(image.get_atomic_numbers()) == 0:
-            ind = np.argsort(image.atom_types_image)
-            symbols = np.array(image.atom_types_image)[ind]
-        else:
-            ind = np.argsort(image.get_atomic_numbers())
-            symbols = np.array(image.get_atomic_numbers())[ind]
-        coord = np.array(coord)[ind]
-        # if constraints:
-        #     sflags = sflags[ind]
-    else:
-        symbols = image.atom_types_image
-
     # Create a list sc of (symbol, count) pairs
     if symbol_count:
         # sc = symbol_count
         pass
     elif image.atom_type is None:
         sc = Counter(symbols)
         atom_type = list(sc.keys())
         atom_type_num = list(sc.values())
     else:
         atom_type = image.atom_type
         atom_type_num = image.atom_type_num
+
+    atom_types_image = np.array(image.atom_types_image)
+
+    if sort:
+        if len(image.get_atomic_numbers()) == 0:
+            indices_dict = {type: np.where(atom_types_image == type)[0] for type in atom_type}
+            sorted_indices = np.concatenate([np.sort(indices) for indices in indices_dict.values()])
+            symbols = atom_types_image[sorted_indices]
+        else:
+            sorted_indices = np.argsort(image.get_atomic_numbers())
+            symbols = np.array(image.get_atomic_numbers())[sorted_indices]
+        coord = np.array(coord)[sorted_indices]
+        # if constraints:
+        #     sflags = sflags[ind]
+    else:
+        symbols = image.atom_types_image
     
     atom_type = [elements[_] for _ in atom_type]
     # Write to file
     output_file = open(os.path.join(filepath, data_name), 'w')
     output_file.write('Created from %s\n' % data_name)
     output_file.write('1.0\n')
     for i in range(3):
@@ -294,40 +300,42 @@
         if image.cartesian:                      # cartesian -> direct
             coord = image.get_scaled_positions(wrap=wrap)   
             image._set_orthorhombic()
         else:            # direct -> cartesian
             image._set_orthorhombic()
             coord = image._set_cartesian().position
 
-        
-        if sort:
-            if len(image.get_atomic_numbers()) == 0:
-                ind = np.argsort(image.atom_types_image)
-                symbols = np.array(image.atom_types_image)[ind]
-            else:
-                ind = np.argsort(image.get_atomic_numbers())
-                symbols = np.array(image.get_atomic_numbers())[ind]
-            coord = np.array(coord)[ind]
-            # if constraints:
-            #     sflags = sflags[ind]
-        else:
-            symbols = image.atom_types_image
-
         # Create a list sc of (symbol, count) pairs
         if symbol_count:
             # sc = symbol_count
             pass
         elif image.atom_type is None:
             sc = Counter(symbols)
             atom_type = list(sc.keys())
             atom_type_num = list(sc.values())
         else:
             atom_type = image.atom_type
             atom_type_num = image.atom_type_num
 
+        atom_types_image = np.array(image.atom_types_image)
+
+        if sort:
+            if len(image.get_atomic_numbers()) == 0:
+                indices_dict = {type: np.where(atom_types_image == type)[0] for type in atom_type}
+                sorted_indices = np.concatenate([np.sort(indices) for indices in indices_dict.values()])
+                symbols = atom_types_image[sorted_indices]
+            else:
+                sorted_indices = np.argsort(image.get_atomic_numbers())
+                symbols = np.array(image.get_atomic_numbers())[sorted_indices]
+            coord = np.array(coord)[sorted_indices]
+                # if constraints:
+                #     sflags = sflags[ind]
+        else:
+            symbols = image.atom_types_image
+
         p = 1
         atype = []
         # atom num & type list 
         for item in atom_type_num:
             atype += [p for _ in range(int(item))]
             p +=1
```

### Comparing `pwdata-0.2.13/pwdata/calculators/const.py` & `pwdata-0.2.14/pwdata/calculators/const.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/calculators/unitconvert_lmps.py` & `pwdata-0.2.14/pwdata/calculators/unitconvert_lmps.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/calculators/units.py` & `pwdata-0.2.14/pwdata/calculators/units.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/cp2kdata.py` & `pwdata-0.2.14/pwdata/cp2kdata.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/datasets_saver.py` & `pwdata-0.2.14/pwdata/datasets_saver.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/deepmd.py` & `pwdata-0.2.14/pwdata/deepmd.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/dump.py` & `pwdata-0.2.14/pwdata/dump.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/extendedxyz.py` & `pwdata-0.2.14/pwdata/extendedxyz.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/image.py` & `pwdata-0.2.14/pwdata/image.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/lammpsdata.py` & `pwdata-0.2.14/pwdata/lammpsdata.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/lmps.py` & `pwdata-0.2.14/pwdata/lmps.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/main.py` & `pwdata-0.2.14/pwdata/main.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/movement.py` & `pwdata-0.2.14/pwdata/movement.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/movement_saver.py` & `pwdata-0.2.14/pwdata/movement_saver.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/outcar.py` & `pwdata-0.2.14/pwdata/outcar.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/pertub/perturbation.py` & `pwdata-0.2.14/pwdata/pertub/perturbation.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/pertub/scale.py` & `pwdata-0.2.14/pwdata/pertub/scale.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/poscar.py` & `pwdata-0.2.14/pwdata/poscar.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata/pwmlff.py` & `pwdata-0.2.14/pwdata/pwmlff.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/pwdata.egg-info/PKG-INFO` & `pwdata-0.2.14/pwdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdata
-Version: 0.2.13
+Version: 0.2.14
 Summary: pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.
 Home-page: https://github.com/LonxunQuantum/pwdata
 Author: LonxunQuantum
 Author-email: lonxun@pwmat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pwdata-0.2.13/pwdata.egg-info/SOURCES.txt` & `pwdata-0.2.14/pwdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.13/setup.py` & `pwdata-0.2.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pwdata", 
-    version="0.2.13",
+    version="0.2.14",
     author="LonxunQuantum",
     author_email="lonxun@pwmat.com",
     description="pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LonxunQuantum/pwdata",
     packages=setuptools.find_packages(),
```

