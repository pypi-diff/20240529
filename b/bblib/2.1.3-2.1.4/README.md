# Comparing `tmp/bblib-2.1.3.tar.gz` & `tmp/bblib-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-2.1.3.tar", max compression
+gzip compressed data, was "bblib-2.1.4.tar", max compression
```

## Comparing `bblib-2.1.3.tar` & `bblib-2.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-05-25 12:49:11.630163 bblib-2.1.3/LICENSE
--rw-r--r--   0        0        0     3939 2024-05-25 12:49:11.630163 bblib-2.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-25 12:49:11.630163 bblib-2.1.3/bblib/__init__.py
--rwxr-xr-x   0        0        0    38835 2024-05-25 12:49:11.630163 bblib-2.1.3/bblib/methods.py
--rwxr-xr-x   0        0        0    10130 2024-05-25 12:49:11.630163 bblib-2.1.3/bblib/models.py
--rwxr-xr-x   0        0        0    18200 2024-05-25 12:49:11.630163 bblib-2.1.3/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-05-25 12:49:23.326146 bblib-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     7470 1970-01-01 00:00:00.000000 bblib-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-05-29 13:10:06.716635 bblib-2.1.4/LICENSE
+-rw-r--r--   0        0        0     3939 2024-05-29 13:10:06.716635 bblib-2.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 13:10:06.716635 bblib-2.1.4/bblib/__init__.py
+-rwxr-xr-x   0        0        0    38802 2024-05-29 13:10:06.716635 bblib-2.1.4/bblib/methods.py
+-rwxr-xr-x   0        0        0     9986 2024-05-29 13:10:06.716635 bblib-2.1.4/bblib/models.py
+-rwxr-xr-x   0        0        0    15007 2024-05-29 13:10:06.716635 bblib-2.1.4/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-05-29 13:10:15.804591 bblib-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7470 1970-01-01 00:00:00.000000 bblib-2.1.4/PKG-INFO
```

### Comparing `bblib-2.1.3/LICENSE` & `bblib-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-2.1.3/README.md` & `bblib-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bblib-2.1.3/bblib/methods.py` & `bblib-2.1.4/bblib/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import om.lib.geometry as geometry
 from bblib.utils import (
     mask_peaks,
     center_of_mass,
     azimuthal_average,
     gaussian_lin,
     get_fwhm_map_global_min,
-    get_distance_map_global_min,
     correct_polarization,
     visualize_single_panel,
 )
 import math
 from scipy import ndimage
 from bblib.models import PF8Info, PF8
 import h5py
```

### Comparing `bblib-2.1.3/bblib/models.py` & `bblib-2.1.4/bblib/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,33 +116,24 @@
                 if x == "ss" or x == "fs"
             ]
 
             if frame_dim_structure[0] == "ss":
                 self.ss_in_rows = True
             else:
                 self.ss_in_rows = False
+            
+            ## The transformation matrix here are only for visualization purposes. Small stretching factors won't have an impact on the visualization of the images (slabby data).
             self.transformation_matrix = [
                 [
-                    detector_panels[panel_name]["fsx"],
-                    detector_panels[panel_name]["fsy"],
+                    int(detector_panels[panel_name]["fsx"]),
+                    int(detector_panels[panel_name]["fsy"]),
                 ],
                 [
-                    detector_panels[panel_name]["ssx"],
-                    detector_panels[panel_name]["ssy"],
-                ],
-            ]
-
-            self.transformation_matrix = [
-                [
-                    detector_panels[panel_name]["fsx"],
-                    detector_panels[panel_name]["fsy"],
-                ],
-                [
-                    detector_panels[panel_name]["ssx"],
-                    detector_panels[panel_name]["ssy"],
+                    int(detector_panels[panel_name]["ssx"]),
+                    int(detector_panels[panel_name]["ssy"]),
                 ],
             ]
 
     def get(self, parameter: str):
         if parameter == "max_num_peaks":
             return self.max_num_peaks
         elif parameter == "adc_threshold":
```

### Comparing `bblib-2.1.3/bblib/utils.py` & `bblib-2.1.4/bblib/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -356,112 +356,14 @@
         yc = -1
     else:
         if plots_flag:
             plt.savefig(f"{output_folder}/fwhm_map/{label}.png")
     plt.close()
     return [np.round(xc, 0), np.round(yc, 0)]
 
-
-def get_distance_map_global_min(
-    lines: list, output_folder: str, label: str, pixel_step: int, plots_flag: bool
-) -> tuple:
-    """
-    Open distance minimization plot, fit projections in both axis to get the point of minimum distance.
-
-    Parameters
-    ----------
-    lines: list
-        Output of grid search for FWHM optmization, each line should contain a dictionary contaning entries for xc, yc and fwhm_over_radius.
-    """
-
-    n = int(math.sqrt(len(lines)))
-    pixel_step /= 2
-    merged_dict = {}
-    for dictionary in lines[:]:
-        for key, value in dictionary.items():
-            if key in merged_dict:
-                merged_dict[key].append(value)
-            else:
-                merged_dict[key] = [value]
-
-    # Create a figure with three subplots
-    fig, (ax1, ax2, ax3) = plt.subplots(1, 3, figsize=(20, 5))
-
-    # Extract x, y, and z from merged_dict
-
-    x = np.array(merged_dict["xc"]).reshape((n, n))[0]
-    y = np.array(merged_dict["yc"]).reshape((n, n))[:, 0]
-    z = np.array(merged_dict["d"], dtype=np.float64).reshape((n, n))
-    z = np.nan_to_num(z)
-
-    pos1 = ax1.imshow(z, cmap="rainbow")
-    step = 20
-    n = z.shape[0]
-    ax1.set_xticks(np.arange(0, n, step, dtype=float))
-    ax1.set_yticks(np.arange(0, n, step, dtype=float))
-    step = round(step * (abs(x[0] - x[1])), 1)
-    ax1.set_xticklabels(
-        np.arange(round(x[0], 1), round(x[-1] + step, 1), step, dtype=int), rotation=45
-    )
-    ax1.set_yticklabels(
-        np.arange(round(y[0], 1), round(y[-1] + step, 1), step, dtype=int)
-    )
-
-    ax1.set_ylabel("yc [px]")
-    ax1.set_xlabel("xc [px]")
-    ax1.set_title("Distance [px]")
-
-    proj_x = np.sum(z, axis=0)
-    # print('proj',len(proj_x))
-    x = np.arange(x[0], x[-1] + pixel_step, pixel_step)
-
-    # print('x',len(x))
-    if len(proj_x) == len(x):
-        index_x = np.unravel_index(np.argmin(proj_x, axis=None), proj_x.shape)
-        xc = x[index_x]
-        ax2.scatter(x, proj_x + pixel_step, color="b")
-        ax2.scatter(xc, proj_x[index_x], color="r", label=f"xc: {np.round(xc,1)}")
-        ax2.set_ylabel("Average distance [px]")
-        ax2.set_xlabel("xc [px]")
-        ax2.set_title("Distance projection in x")
-        ax2.legend()
-    else:
-        converged = 0
-        xc = -1
-        yc = -1
-
-    proj_y = np.sum(z, axis=1)
-    x = np.arange(y[0], y[-1] + pixel_step, pixel_step)
-    if len(proj_y) == len(x):
-        index_y = np.unravel_index(np.argmin(proj_y, axis=None), proj_y.shape)
-        yc = x[index_y]
-        ax3.scatter(x, proj_y, color="b")
-        ax3.scatter(yc, proj_y[index_y], color="r", label=f"yc: {np.round(yc,1)}")
-        ax3.set_ylabel("Average Distance [px]")
-        ax3.set_xlabel("yc [px]")
-        ax3.set_title("Distance projection in y")
-        ax3.legend()
-        fig.colorbar(pos1, ax=ax1, shrink=0.6)
-    else:
-        converged = 0
-        xc = -1
-        yc = -1
-
-    if int(np.sum(proj_y)) == 0 or int(np.sum(proj_x)) == 0:
-        converged = 0
-        xc = -1
-        yc = -1
-    else:
-        converged = 1
-        if plots_flag:
-            plt.savefig(f"{output_folder}/distance_map/{label}.png")
-    plt.close()
-    return [np.round(xc, 1), np.round(yc, 1)]
-
-
 def circle_mask(data: np.ndarray, center: tuple, radius: int) -> np.ndarray:
     """
     Make a  ring mask for the data
 
     Parameters
     ----------
     data: np.ndarray
```

### Comparing `bblib-2.1.3/pyproject.toml` & `bblib-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "2.1.3"
+version = "2.1.4"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-2.1.3/PKG-INFO` & `bblib-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 2.1.3
+Version: 2.1.4
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

