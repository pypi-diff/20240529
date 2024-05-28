# Comparing `tmp/pyCHNOSZ-0.8.8.tar.gz` & `tmp/pyCHNOSZ-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyCHNOSZ-0.8.8.tar", last modified: Tue Aug  9 18:12:35 2022, max compression
+gzip compressed data, was "dist/pyCHNOSZ-0.8.9.tar", last modified: Wed Aug 17 22:58:53 2022, max compression
```

## Comparing `pyCHNOSZ-0.8.8.tar` & `pyCHNOSZ-0.8.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2022-08-09 18:12:35.228105 pyCHNOSZ-0.8.8/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1087 2022-08-09 18:06:56.000000 pyCHNOSZ-0.8.8/LICENSE.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     6609 2022-08-09 18:12:35.224105 pyCHNOSZ-0.8.8/PKG-INFO
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     6163 2022-08-09 18:06:30.000000 pyCHNOSZ-0.8.8/README.md
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2022-08-09 18:12:35.208103 pyCHNOSZ-0.8.8/pyCHNOSZ/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      286 2022-08-09 18:08:40.000000 pyCHNOSZ-0.8.8/pyCHNOSZ/__init__.py
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)    98597 2022-08-09 18:08:39.000000 pyCHNOSZ-0.8.8/pyCHNOSZ/fun.py
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2022-08-09 18:12:35.220104 pyCHNOSZ-0.8.8/pyCHNOSZ.egg-info/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     6609 2022-08-09 18:12:35.000000 pyCHNOSZ-0.8.8/pyCHNOSZ.egg-info/PKG-INFO
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      257 2022-08-09 18:12:35.000000 pyCHNOSZ-0.8.8/pyCHNOSZ.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2022-08-09 18:12:35.000000 pyCHNOSZ-0.8.8/pyCHNOSZ.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2022-08-09 18:12:35.000000 pyCHNOSZ-0.8.8/pyCHNOSZ.egg-info/not-zip-safe
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       51 2022-08-09 18:12:35.000000 pyCHNOSZ-0.8.8/pyCHNOSZ.egg-info/requires.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        9 2022-08-09 18:12:35.000000 pyCHNOSZ-0.8.8/pyCHNOSZ.egg-info/top_level.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       38 2022-08-09 18:12:35.228105 pyCHNOSZ-0.8.8/setup.cfg
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      784 2022-08-09 18:06:47.000000 pyCHNOSZ-0.8.8/setup.py
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2022-08-17 22:58:53.322263 pyCHNOSZ-0.8.9/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1087 2022-08-17 22:55:23.000000 pyCHNOSZ-0.8.9/LICENSE.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     6609 2022-08-17 22:58:53.318262 pyCHNOSZ-0.8.9/PKG-INFO
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     6163 2022-08-17 22:55:23.000000 pyCHNOSZ-0.8.9/README.md
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2022-08-17 22:58:53.302261 pyCHNOSZ-0.8.9/pyCHNOSZ/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      286 2022-08-17 22:55:57.000000 pyCHNOSZ-0.8.9/pyCHNOSZ/__init__.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)    98592 2022-08-17 22:55:57.000000 pyCHNOSZ-0.8.9/pyCHNOSZ/fun.py
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2022-08-17 22:58:53.318262 pyCHNOSZ-0.8.9/pyCHNOSZ.egg-info/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     6609 2022-08-17 22:58:53.000000 pyCHNOSZ-0.8.9/pyCHNOSZ.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      257 2022-08-17 22:58:53.000000 pyCHNOSZ-0.8.9/pyCHNOSZ.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2022-08-17 22:58:53.000000 pyCHNOSZ-0.8.9/pyCHNOSZ.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2022-08-17 22:58:53.000000 pyCHNOSZ-0.8.9/pyCHNOSZ.egg-info/not-zip-safe
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       51 2022-08-17 22:58:53.000000 pyCHNOSZ-0.8.9/pyCHNOSZ.egg-info/requires.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        9 2022-08-17 22:58:53.000000 pyCHNOSZ-0.8.9/pyCHNOSZ.egg-info/top_level.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       38 2022-08-17 22:58:53.322263 pyCHNOSZ-0.8.9/setup.cfg
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      784 2022-08-17 22:57:06.000000 pyCHNOSZ-0.8.9/setup.py
```

### Comparing `pyCHNOSZ-0.8.8/LICENSE.txt` & `pyCHNOSZ-0.8.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyCHNOSZ-0.8.8/PKG-INFO` & `pyCHNOSZ-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCHNOSZ
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python wrapper for the R package CHNOSZ.
 Home-page: UNKNOWN
 Author: Grayson Boyer
 Author-email: gmboyer@asu.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCHNOSZ-0.8.8/README.md` & `pyCHNOSZ-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pyCHNOSZ-0.8.8/pyCHNOSZ/fun.py` & `pyCHNOSZ-0.8.9/pyCHNOSZ/fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -788,15 +788,15 @@
               'modeBarButtonsToRemove': ['zoom2d', 'pan2d', 'zoomIn2d', 'zoomOut2d',
                                          'autoScale2d', 'toggleSpikelines',
                                          'hoverClosestCartesian', 'hoverCompareCartesian']}
 
     fig.show(config=config)
 
     
-def diagram_interactive(data, title=None, borders=True,
+def diagram_interactive(data, title=None, borders=0,
                         annotation=None, annotation_coords=[0, 0],
                         balance=None, xlab=None, ylab=None, colormap="viridis",
                         width=600, height=520, alpha=False, messages=True,
                         plot_it=True, save_as=None, save_format=None, save_scale=1):
     
     """
     Produce an interactive diagram.
@@ -805,16 +805,18 @@
     ----------
     data : rpy2.ListVector
         Output from `equilibrate` or `affinity`.
     
     title : str, optional
         Title of the plot.
     
-    borders : bool, default True
-        Show lines that indicate borders between regions?
+    borders : float, default 0
+        If set to a value greater than 0, shows lines that indicate borders
+        between regions in predominance diagrams. Value indicates thickness
+        of the border, in pixels.
     
     annotation : str, optional
         Annotation to add to the plot.
     
     annotation_coords : list of numeric, default [0, 0], optional
         Coordinates of annotation, where 0,0 is bottom left and 1,1 is top
         right.
@@ -1063,102 +1065,102 @@
                                              'filename': save_as,
                                              'height': height,
                                              'width': width,
                                              'scale': save_scale,
                                           },
                  }
         
-#         if borders:
+        if borders > 0:
             
-#             unique_x_vals = list(dict.fromkeys(df["pH"]))
-#             unique_y_vals = list(dict.fromkeys(df["T"]))
+            unique_x_vals = list(dict.fromkeys(df[xvar]))
+            unique_y_vals = list(dict.fromkeys(df[yvar]))
             
-#             def mov_mean(numbers=[], window_size=2):
-#                 i = 0
-#                 moving_averages = []
-#                 while i < len(numbers) - window_size + 1:
-#                     this_window = numbers[i : i + window_size]
-
-#                     window_average = sum(this_window) / window_size
-#                     moving_averages.append(window_average)
-#                     i += 1
-#                 return moving_averages
+            def mov_mean(numbers=[], window_size=2):
+                i = 0
+                moving_averages = []
+                while i < len(numbers) - window_size + 1:
+                    this_window = numbers[i : i + window_size]
+
+                    window_average = sum(this_window) / window_size
+                    moving_averages.append(window_average)
+                    i += 1
+                return moving_averages
             
-#             x_mov_mean = mov_mean(unique_x_vals)
-#             y_mov_mean = mov_mean(unique_y_vals)
+            x_mov_mean = mov_mean(unique_x_vals)
+            y_mov_mean = mov_mean(unique_y_vals)
 
-#             x_plot_min = x_mov_mean[0] - (x_mov_mean[1] - x_mov_mean[0])
-#             y_plot_min = y_mov_mean[0] - (y_mov_mean[1] - y_mov_mean[0])
+            x_plot_min = x_mov_mean[0] - (x_mov_mean[1] - x_mov_mean[0])
+            y_plot_min = y_mov_mean[0] - (y_mov_mean[1] - y_mov_mean[0])
 
-#             x_plot_max = x_mov_mean[-1] + (x_mov_mean[1] - x_mov_mean[0])
-#             y_plot_max = y_mov_mean[-1] + (y_mov_mean[1] - y_mov_mean[0])
+            x_plot_max = x_mov_mean[-1] + (x_mov_mean[1] - x_mov_mean[0])
+            y_plot_max = y_mov_mean[-1] + (y_mov_mean[1] - y_mov_mean[0])
 
-#             x_vals_border = [x_plot_min] + x_mov_mean + [x_plot_max]
-#             y_vals_border = [y_plot_min] + y_mov_mean + [y_plot_max]
+            x_vals_border = [x_plot_min] + x_mov_mean + [x_plot_max]
+            y_vals_border = [y_plot_min] + y_mov_mean + [y_plot_max]
             
-#             data = np.array(df.pred)
-#             shape = (len(xvals), len(yvals))
-#             dmap = data.reshape(shape)
+            data = np.array(df.pred)
+            shape = (len(xvals), len(yvals))
+            dmap = data.reshape(shape)
             
-#             def find_line(dmap, row_index):
-#                 return [i for i in range(0, len(dmap[row_index])-1) if dmap[row_index][i] != dmap[row_index][i+1]]
+            def find_line(dmap, row_index):
+                return [i for i in range(0, len(dmap[row_index])-1) if dmap[row_index][i] != dmap[row_index][i+1]]
 
-#             nrows, ncols = dmap.shape
-#             vlines = []
-#             for row_i in range(0, nrows):
-#                 vlines.append(find_line(dmap, row_i))
-
-#             dmap_transposed = dmap.transpose()
-#             nrows, ncols = dmap_transposed.shape
-#             hlines = []
-#             for row_i in range(0, nrows):
-#                 hlines.append(find_line(dmap_transposed, row_i))
-#             y_coord_list_vertical = []
-#             x_coord_list_vertical = []
-#             for i,row in enumerate(vlines):
-#                 for line in row:
-#                     x_coord_list_vertical += [x_vals_border[line+1], x_vals_border[line+1], np.nan]
-#                     y_coord_list_vertical += [y_vals_border[i], y_vals_border[i+1], np.nan]
-
-#             y_coord_list_horizontal = []
-#             x_coord_list_horizontal = []
-#             for i,col in enumerate(hlines):
-#                 for line in col:
-#                     y_coord_list_horizontal += [y_vals_border[line+1], y_vals_border[line+1], np.nan]
-#                     x_coord_list_horizontal += [x_vals_border[i], x_vals_border[i+1], np.nan]
-
-#             fig.add_trace(
-#                 go.Scatter(
-#               mode= 'lines',
-#               x= x_coord_list_horizontal,
-#               y= y_coord_list_horizontal,
-#               line= {
-#                 "width": 0.5,
-#                 "color": 'black'
-#               },
-#               hoverinfo= 'skip',
-#               showlegend=False,
-#                 )
-#             )
-#             fig.add_trace(
-#                 go.Scatter(
-#               mode= 'lines',
-#               x= x_coord_list_vertical,
-#               y= y_coord_list_vertical,
-#               line= {
-#                 "width": 0.5,
-#                 "color": 'black'
-#               },
-#               hoverinfo= 'skip',
-#               showlegend=False,
-#                 )
-#             )
+            nrows, ncols = dmap.shape
+            vlines = []
+            for row_i in range(0, nrows):
+                vlines.append(find_line(dmap, row_i))
+
+            dmap_transposed = dmap.transpose()
+            nrows, ncols = dmap_transposed.shape
+            hlines = []
+            for row_i in range(0, nrows):
+                hlines.append(find_line(dmap_transposed, row_i))
+            y_coord_list_vertical = []
+            x_coord_list_vertical = []
+            for i,row in enumerate(vlines):
+                for line in row:
+                    x_coord_list_vertical += [x_vals_border[line+1], x_vals_border[line+1], np.nan]
+                    y_coord_list_vertical += [y_vals_border[i], y_vals_border[i+1], np.nan]
+
+            y_coord_list_horizontal = []
+            x_coord_list_horizontal = []
+            for i,col in enumerate(hlines):
+                for line in col:
+                    y_coord_list_horizontal += [y_vals_border[line+1], y_vals_border[line+1], np.nan]
+                    x_coord_list_horizontal += [x_vals_border[i], x_vals_border[i+1], np.nan]
+                    
+            fig.add_trace(
+                go.Scatter(
+              mode= 'lines',
+              x= x_coord_list_horizontal,
+              y= y_coord_list_horizontal,
+              line= {
+                "width": borders,
+                "color": 'black'
+              },
+              hoverinfo= 'skip',
+              showlegend=False,
+                )
+            )
+            fig.add_trace(
+                go.Scatter(
+              mode= 'lines',
+              x= x_coord_list_vertical,
+              y= y_coord_list_vertical,
+              line= {
+                "width": borders,
+                "color": 'black'
+              },
+              hoverinfo= 'skip',
+              showlegend=False,
+                )
+            )
         
-#             fig.update_yaxes(range=[min(yvals), max(yvals)], autorange=False, mirror=True)
-#             fig.update_xaxes(range=[min(xvals), max(xvals)], autorange=False, mirror=True)
+            fig.update_yaxes(range=[min(yvals), max(yvals)], autorange=False, mirror=True)
+            fig.update_xaxes(range=[min(xvals), max(xvals)], autorange=False, mirror=True)
         
         
     if plot_it:
         fig.show(config=config)
     
     return df, fig
 
@@ -1785,19 +1787,20 @@
     -------
     a : rpy2.ListVector
         Output from `diagram`.
     args : dict
         Dictionary of arguments supplied to `diagram`.
     """
     
+    if lwd == None:
+        borders = 0
+    else:
+        borders = lwd
+    
     if interactive:
-        if lwd == 0:
-            borders = False
-        else:
-            borders = True
             
         df, fig = diagram_interactive(data=eout, title=main, borders=borders,
                                  annotation=annotation,
                                  annotation_coords=annotation_coords,
                                  balance=balance,
                                  xlab=xlab, ylab=ylab,
                                  colormap=fill,
```

### Comparing `pyCHNOSZ-0.8.8/pyCHNOSZ.egg-info/PKG-INFO` & `pyCHNOSZ-0.8.9/pyCHNOSZ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCHNOSZ
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python wrapper for the R package CHNOSZ.
 Home-page: UNKNOWN
 Author: Grayson Boyer
 Author-email: gmboyer@asu.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCHNOSZ-0.8.8/setup.py` & `pyCHNOSZ-0.8.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyCHNOSZ",
-    version="0.8.8",
+    version="0.8.9",
     author="Grayson Boyer",
     author_email="gmboyer@asu.edu",
     description="Python wrapper for the R package CHNOSZ.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={},
     packages=['pyCHNOSZ'],
```

