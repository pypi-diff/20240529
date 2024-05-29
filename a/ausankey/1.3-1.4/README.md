# Comparing `tmp/ausankey-1.3.tar.gz` & `tmp/ausankey-1.4.tar.gz`

## Comparing `ausankey-1.3.tar` & `ausankey-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ausankey-1.3/ausankey/__init__.py
--rw-r--r--   0        0        0    31411 2020-02-02 00:00:00.000000 ausankey-1.3/ausankey/ausankey.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ausankey-1.3/tests/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ausankey-1.3/tests/fruit.csv
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ausankey-1.3/tests/generic_test.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ausankey-1.3/tests/test_fruit_defaults.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ausankey-1.3/tests/test_fruit_setup.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ausankey-1.3/.gitignore
--rw-r--r--   0        0        0    35146 2020-02-02 00:00:00.000000 ausankey-1.3/LICENSE
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ausankey-1.3/README.md
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 ausankey-1.3/pyproject.toml
--rw-r--r--   0        0        0    43279 2020-02-02 00:00:00.000000 ausankey-1.3/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ausankey-1.4/ausankey/__init__.py
+-rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 ausankey-1.4/ausankey/ausankey.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ausankey-1.4/tests/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ausankey-1.4/tests/fruit.csv
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ausankey-1.4/tests/generic_test.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ausankey-1.4/tests/test_fruit_defaults.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ausankey-1.4/tests/test_fruit_setup.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ausankey-1.4/.gitignore
+-rw-r--r--   0        0        0    35146 2020-02-02 00:00:00.000000 ausankey-1.4/LICENSE
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ausankey-1.4/README.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 ausankey-1.4/pyproject.toml
+-rw-r--r--   0        0        0    43279 2020-02-02 00:00:00.000000 ausankey-1.4/PKG-INFO
```

### Comparing `ausankey-1.3/ausankey/ausankey.py` & `ausankey-1.4/ausankey/ausankey.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Produces simple Sankey Diagrams with matplotlib.
 
 @author: wspr
 
 Forked from: Anneya Golob & marcomanz & pierre-sassoulas & jorwoods
 """
 
-
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 ###########################################
 
 
@@ -26,20 +26,27 @@
     -------
 
     None (yet)
     """
 
     sky = Sankey(**kwargs)
     sky.setup(data)
+
+    sky.plot_init()
     sky.plot_frame()
 
-    # draw each segment
+    # draw each sankey
     for ii in range(sky.num_flow):
         sky.subplot(ii)
 
+    # draw titles
+    if sky.titles is not None:
+        for ii in range(sky.num_flow):
+            sky.plot_titles(ii)
+
 
 ###########################################
 
 
 class SankeyError(Exception):
     pass
 
@@ -129,17 +136,17 @@
         Normalised horizontal gap between the left/right of the
         plot edges and the label
         (1.0 = 100% of plot width)
 
     label_loc : [str1, str2, str3]
         Position to place labels next to the nodes.
 
-        * `str1`: position of first labels (`"left"`, `"right"`, `"center"`, or `"none"`)
-        * `str2`: position of middle labels (`"left"`, `"right"`, `"both"`, `"center"`, or `"none"`)
-        * `str3`: position of last labels (`"left"`, `"right"`, `"center"`, or `"none"`)
+        * `str1`: position of first labels (`"left"`, `"right"`, `"center"`,  `"top"`, or `"none"`)
+        * `str2`: position of middle labels (`"left"`, `"right"`, `"both"`, `"center"`,  `"top"`, or `"none"`)
+        * `str3`: position of last labels (`"left"`, `"right"`, `"center"`,  `"top"`, or `"none"`)
 
     label_duplicate : bool
         When set False, will only print a middle label if that label didn't
         appear in the previous stage. This minimises chart clutter but might
         be confusing in cases, hence defaulting to True.
 
     label_font : dict
@@ -301,15 +308,15 @@
         self.flow_alpha = flow_alpha
         self.flow_lw = flow_lw
         self.fontcolor = fontcolor
         self.fontsize = fontsize
         self.fontfamily = fontfamily
         self.frame_side = frame_side
         self.frame_gap = frame_gap
-        self.frame_color = frame_color
+        self.frame_color = frame_color or [0, 0, 0, 1]
         self.frame_lw = frame_lw
         self.label_dict = label_dict or {}
         self.label_width = label_width
         self.label_gap = label_gap
         self.label_loc = label_loc
         self.label_font = label_font or {}
         self.label_duplicate = True if label_duplicate is None else label_duplicate
@@ -347,352 +354,389 @@
 
         num_col = len(self.data.columns)
         self.data.columns = range(num_col)  # force numeric column headings
         self.num_stages = int(num_col / 2)  # number of stages
         self.num_flow = self.num_stages - 1
 
         # sizes
-        col_hgt = np.empty(self.num_stages)
         self.node_sizes = {}
         self.nodes_uniq = {}
 
+        self.node_pos_voffset = {}
+        self.node_pos_bot = {}
+        self.node_pos_top = {}
+
         # weight and reclassify
         self.weight_labels()
         for ii in range(self.num_stages):
-            for nn, lbl in enumerate(self.data[2 * ii]):
+            for nn, lbl in enumerate([x for x in self.data[2 * ii] if x is not None]):
                 val = self.node_sizes[ii][lbl]
-                if lbl is not None and (
+                if (
                     val < self.other_thresh_val
                     or val < self.other_thresh_sum * self.weight_sum[ii]
                     or val < self.other_thresh_max * max(self.data[2 * ii + 1])
                 ):
                     self.data.iat[nn, 2 * ii] = self.other_name
         self.weight_labels()
 
         # sort and calc
-        self.plot_height_nom = max(self.weight_sum)
         for ii in range(self.num_stages):
             self.node_sizes[ii] = self.sort_node_sizes(self.node_sizes[ii], self.sort)
-            col_hgt[ii] = self.weight_sum[ii] + (len(self.nodes_uniq[ii]) - 1) * self.node_gap * self.plot_height_nom
 
-        # overall dimensions
-        self.plot_height = max(col_hgt)
-        self.sub_width = self.plot_height
-        self.plot_width_nom = (self.num_stages - 1) * self.sub_width
-        self.plot_width = (
-            (self.num_stages - 1) * self.sub_width
-            + 2 * self.plot_width_nom * (self.label_gap + self.label_width)
-            + self.num_stages * self.plot_width_nom * self.node_width
-        )
+        self.calc_plot_height()
+        self.calc_plot_dimens()
 
-        # offsets for alignment
-        vscale_dict = {"top": 1, "center": 0.5, "bottom": 0}
-        self.vscale = vscale_dict.get(self.valign, 0)
-        self.voffset = np.empty(self.num_stages)
-        for ii in range(self.num_stages):
-            self.voffset[ii] = self.vscale * (col_hgt[1] - col_hgt[ii])
+        self.x_lr = {}
+        self.nodesize_l = {}
+        self.nodesize_r = {}
+        self.node_pairs = {}
+        for ii in range(self.num_flow):
+            x_left = (
+                self.x_node_width + self.x_label_gap + self.x_label_width + ii * (self.sub_width + self.x_node_width)
+            )
+            self.x_lr[ii] = (x_left, x_left + self.sub_width)
+            self.nodesize_l[ii] = {}
+            self.nodesize_r[ii] = {}
+            self.node_pairs[ii] = []
+            for lbl_l in self.node_sizes[ii]:
+                self.nodesize_l[ii][lbl_l] = {}
+                self.nodesize_r[ii][lbl_l] = {}
+                for lbl_r in self.node_sizes[ii + 1]:
+                    ind = (self.data[2 * ii] == lbl_l) & (self.data[2 * ii + 2] == lbl_r)
+                    if not any(ind):
+                        continue
+                    self.node_pairs[ii].append((lbl_l, lbl_r))
+                    self.nodesize_l[ii][lbl_l][lbl_r] = self.data[2 * ii + 1][ind].sum()
+                    self.nodesize_r[ii][lbl_l][lbl_r] = self.data[2 * ii + 3][ind].sum()
+
+        # All node sizes and positions
+        for ii in range(self.num_flow):
+            self.node_pos_voffset[ii] = [{}, {}]
+            self.node_pos_bot[ii] = [{}, {}]
+            self.node_pos_top[ii] = [{}, {}]
+            prev_label = None  # avoid lint error
+            for lr in [0, 1]:
+                for i, (label, node_height) in enumerate(self.node_sizes[ii + lr].items()):
+                    this_side_height = self.node_indiv_heights[ii][lr].get(label, 0)
+                    self.node_pos_voffset[ii][lr][label] = self.vscale * (node_height - this_side_height)
+                    if i == 0:
+                        tmp_top = self.voffset[ii + lr]
+                    else:
+                        tmp_top = self.node_pos_top[ii][lr][prev_label] + self.y_node_gap
+                    self.node_pos_bot[ii][lr][label] = tmp_top
+                    self.node_pos_top[ii][lr][label] = tmp_top + node_height
+                    prev_label = label
 
         # labels
         label_record = self.data[range(0, 2 * self.num_stages, 2)].to_records(index=False)
         flattened = [item for sublist in label_record for item in sublist]
         self.all_labels = pd.Series(flattened).unique()
 
         # If no color_dict given, make one
         color_dict_new = {}
-        cmap = plt.cm.get_cmap(self.colormap)
+        cmap = getattr(mpl.cm, self.colormap, None)
         color_palette = cmap(np.linspace(0, 1, len(self.all_labels)))
         for i, label in enumerate(self.all_labels):
             color_dict_new[label] = self.color_dict.get(label, color_palette[i])
-        # check_colors_match_labels(self.all_labels, color_dict_new)
         self.color_dict = color_dict_new
 
+    ###########################################
+
+    def plot_init(self):
         # initialise plot
         self.ax = self.ax or plt.gca()
         self.ax.axis("off")
 
     ###########################################
 
     def weight_labels(self):
         """Calculates sizes of each node, taking into account discontinuities"""
         self.weight_sum = np.empty(self.num_stages)
 
+        self.node_indiv_heights = {}
+
         for ii in range(self.num_stages):
-            self.nodes_uniq[ii] = pd.Series(self.data[2 * ii]).unique()
+            self.nodes_uniq[ii] = pd.Series(self.data[2 * ii]).dropna().unique()
 
         for ii in range(self.num_stages):
             self.node_sizes[ii] = {}
+            self.node_indiv_heights[ii] = {}
+            self.node_indiv_heights[ii][0] = {}
+            if ii > 0:
+                self.node_indiv_heights[ii - 1][1] = {}
             for lbl in self.nodes_uniq[ii]:
+                i_p = 2 if ii > 0 else 0
+                i_n = 2 if ii < self.num_flow else 0
+                ind_this = self.data[2 * ii] == lbl
+                none_prev = self.data[2 * ii - i_p].isna()
+                none_next = self.data[2 * ii + i_n].isna()
+
+                ind_cont = ind_this & ~none_prev & ~none_next
+                ind_only = ind_this & none_prev & none_next
+                ind_stop = ind_this & ~none_prev & none_next
+                ind_strt = ind_this & none_prev & ~none_next
+
+                weight_cont = self.data[2 * ii + 1][ind_cont].sum()
+                weight_only = self.data[2 * ii + 1][ind_only].sum()
+                weight_stop = self.data[2 * ii + 1][ind_stop].sum()
+                weight_strt = self.data[2 * ii + 1][ind_strt].sum()
+
                 if ii == 0:
-                    ind_prev = self.data[2 * ii - 0] == lbl
-                    ind_this = self.data[2 * ii + 0] == lbl
-                    ind_next = self.data[2 * ii + 2] == lbl
-                elif ii == self.num_flow:
-                    ind_prev = self.data[2 * ii - 2] == lbl
-                    ind_this = self.data[2 * ii + 0] == lbl
-                    ind_next = self.data[2 * ii + 0] == lbl
+                    self.node_indiv_heights[ii][0][lbl] = weight_cont + weight_only + weight_stop
+                elif ii == self.num_stages:
+                    self.node_indiv_heights[ii - 1][1][lbl] = weight_cont + weight_only + weight_strt
                 else:
-                    ind_prev = self.data[2 * ii - 2] == lbl
-                    ind_this = self.data[2 * ii + 0] == lbl
-                    ind_next = self.data[2 * ii + 2] == lbl
-                weight_cont = self.data[2 * ii + 1][ind_this & ind_prev & ind_next].sum()
-                weight_only = self.data[2 * ii + 1][ind_this & ~ind_prev & ~ind_next].sum()
-                weight_stop = self.data[2 * ii + 1][ind_this & ind_prev & ~ind_next].sum()
-                weight_strt = self.data[2 * ii + 1][ind_this & ~ind_prev & ind_next].sum()
+                    self.node_indiv_heights[ii][0][lbl] = weight_cont + weight_only + weight_stop
+                    self.node_indiv_heights[ii - 1][1][lbl] = weight_cont + weight_only + weight_strt
                 self.node_sizes[ii][lbl] = weight_cont + weight_only + max(weight_stop, weight_strt)
 
             self.weight_sum[ii] = pd.Series(self.node_sizes[ii].values()).sum()
 
     ###########################################
 
+    def calc_plot_height(self):
+        """Calculate column heights, offsets, and total plot height"""
+
+        self.plot_height_nom = max(self.weight_sum)
+
+        vscale_dict = {"top": 1, "center": 0.5, "bottom": 0}
+        self.vscale = vscale_dict.get(self.valign, 0)
+
+        self.voffset = np.empty(self.num_stages)
+        col_hgt = np.empty(self.num_stages)
+        for ii in range(self.num_stages):
+            col_hgt[ii] = self.weight_sum[ii] + (len(self.nodes_uniq[ii]) - 1) * self.node_gap * self.plot_height_nom
+            self.voffset[ii] = self.vscale * (col_hgt[0] - col_hgt[ii])
+
+        self.plot_height = max(col_hgt)
+
+    ###########################################
+
+    def calc_plot_dimens(self):
+        """Calculate absolute size of plot dimens based on scaling factors"""
+
+        # overall dimensions
+        self.sub_width = self.plot_height
+        self.plot_width_nom = (self.num_stages - 1) * self.sub_width
+        self.plot_width = (
+            (self.num_stages - 1) * self.sub_width
+            + 2 * self.plot_width_nom * (self.label_gap + self.label_width)
+            + self.num_stages * self.plot_width_nom * self.node_width
+        )
+
+        # vertical positions
+        self.y_node_gap = self.node_gap * self.plot_height_nom
+        self.y_title_gap = self.title_gap * self.plot_height_nom
+        self.y_frame_gap = self.frame_gap * self.plot_height_nom
+        self.y_label_gap = self.label_gap * self.plot_height_nom
+
+        # horizontal positions
+        self.x_node_width = self.node_width * self.plot_width_nom
+        self.x_label_width = self.label_width * self.plot_width_nom
+        self.x_label_gap = self.label_gap * self.plot_width_nom
+        self.x_value_gap = self.value_gap * self.plot_width_nom
+
+    ###########################################
+
     def plot_frame(self):
-        """Plot frame on top/bottom edges"""
+        """Plot frame on top/bottom edges.
+
+        We always plot them to ensure the exported plot width is correct.
+        If the frame is not requested it is drawn with 100% transparency.
+        """
 
         frame_top = self.frame_side in ("top", "both")
         frame_bot = self.frame_side in ("bottom", "both")
 
-        frame_color = self.frame_color or [0, 0, 0, 1]
-
-        y_frame_gap = self.frame_gap * self.plot_height
-
-        col = frame_color if frame_top else [1, 1, 1, 0]
         self.ax.plot(
             [0, self.plot_width],
-            min(self.voffset) + (self.plot_height) + y_frame_gap + [0, 0],
-            color=col,
+            min(self.voffset) + (self.plot_height) + self.y_frame_gap + [0, 0],
+            color=self.frame_color if frame_top else [1, 1, 1, 0],
             lw=self.frame_lw,
         )
 
-        col = frame_color if frame_bot else [1, 1, 1, 0]
         self.ax.plot(
             [0, self.plot_width],
-            min(self.voffset) - y_frame_gap + [0, 0],
-            color=col,
+            min(self.voffset) - self.y_frame_gap + [0, 0],
+            color=self.frame_color if frame_bot else [1, 1, 1, 0],
             lw=self.frame_lw,
         )
 
     ###########################################
 
     def subplot(self, ii):
         """Subroutine for plotting horizontal sections of the Sankey plot
 
         Some special-casing is used for plotting/labelling differently
         for the first and last cases.
         """
 
-        lastind = 4 if ii < self.num_flow - 1 else 2
-        labels_lr = [
-            self.data[2 * ii],
-            self.data[2 * ii + 2],
-            self.data[2 * ii + lastind],
-        ]
-        weights_lr = [
-            self.data[2 * ii + 1],
-            self.data[2 * ii + 1 + 2],
-            self.data[2 * ii + 1 + lastind],
-        ]
-
-        nodes_lr = [
-            self.sort_nodes(labels_lr[0], self.node_sizes[ii]),
-            self.sort_nodes(labels_lr[1], self.node_sizes[ii + 1]),
-        ]
-
-        # vertical positions
-        y_node_gap = self.node_gap * self.plot_height_nom
-        y_title_gap = self.title_gap * self.plot_height_nom
-        y_frame_gap = self.frame_gap * self.plot_height_nom
-
-        # horizontal positions
-        x_node_width = self.node_width * self.plot_width_nom
-        x_label_width = self.label_width * self.plot_width_nom
-        x_label_gap = self.label_gap * self.plot_width_nom
-        x_value_gap = self.value_gap * self.plot_width_nom
-        x_left = x_node_width + x_label_gap + x_label_width + ii * (self.sub_width + x_node_width)
-        x_lr = [x_left, x_left + self.sub_width]
+        # Abbrev
 
-        # All node sizes and positions
-
-        node_voffset = [{}, {}]
-        node_pos_bot = [{}, {}]
-        node_pos_top = [{}, {}]
-        nodesize = [{}, {}]
-
-        for lbl_l in nodes_lr[0]:
-            nodesize[0][lbl_l] = {}
-            nodesize[1][lbl_l] = {}
-            for lbl_r in nodes_lr[1]:
-                ind = (labels_lr[0] == lbl_l) & (labels_lr[1] == lbl_r)
-                nodesize[0][lbl_l][lbl_r] = weights_lr[0][ind].sum()
-                nodesize[1][lbl_l][lbl_r] = weights_lr[1][ind].sum()
-
-        for lr in [0, 1]:
-            for i, label in enumerate(nodes_lr[lr]):
-                node_height = self.node_sizes[ii + lr][label]
-                this_side_height = weights_lr[lr][labels_lr[lr] == label].sum()
-                node_voffset[lr][label] = self.vscale * (node_height - this_side_height)
-                next_bot = node_pos_top[lr][nodes_lr[lr][i - 1]] + y_node_gap if i > 0 else 0
-                node_pos_bot[lr][label] = self.voffset[ii + lr] if i == 0 else next_bot
-                node_pos_top[lr][label] = node_pos_bot[lr][label] + node_height
+        x_lr = self.x_lr[ii]
 
         # Draw nodes
 
         for lr in [0, 1] if ii == 0 else [1]:
-            for label in nodes_lr[lr]:
+            for label in self.node_sizes[ii + lr]:
                 self.draw_node(
-                    x_lr[lr] - x_node_width * (1 - lr),
-                    x_node_width,
-                    node_pos_bot[lr][label],
+                    x_lr[lr] - self.x_node_width * (1 - lr),
+                    self.x_node_width,
+                    self.node_pos_bot[ii][lr][label],
                     self.node_sizes[ii + lr][label],
                     label,
                 )
 
         # Draw node labels
 
-        ha_dict = {"left": "right", "right": "left", "center": "center"}
+        ha_dict = {"left": "right", "right": "left", "center": "center", "top": "center"}
 
         # first row of labels
         lr = 0
         if ii == 0 and self.label_loc[0] != "none":
             if self.label_loc[0] in ("left"):
-                xx = x_lr[lr] - x_label_gap - x_node_width
+                xx = x_lr[lr] - self.x_label_gap - self.x_node_width
             elif self.label_loc[0] in ("right"):
-                xx = x_lr[lr] + x_label_gap
-            elif self.label_loc[0] in ("center"):
-                xx = x_lr[lr] - x_node_width / 2
-            for label in nodes_lr[lr]:
-                yy = node_pos_bot[lr][label] + self.node_sizes[ii + lr][label] / 2
+                xx = x_lr[lr] + self.x_label_gap
+            elif self.label_loc[0] in ("center", "top"):
+                xx = x_lr[lr] - self.x_node_width / 2
+            for label in self.node_sizes[ii + lr]:
+                if self.label_loc[0] in ("top"):
+                    yy = self.node_pos_bot[ii][lr][label] + self.node_sizes[ii + lr][label] + self.y_label_gap
+                else:
+                    yy = self.node_pos_bot[ii][lr][label] + self.node_sizes[ii + lr][label] / 2
                 self.draw_label(xx, yy, label, ha_dict[self.label_loc[0]])
 
         # inside labels, left
         lr = 1
         if ii < self.num_flow - 1 and self.label_loc[1] in ("left", "both"):
-            xx = x_lr[lr] - x_label_gap
-            ha = "right"
-            for label in nodes_lr[lr]:
-                if (label not in nodes_lr[lr - 1]) or self.label_duplicate:
-                    yy = node_pos_bot[lr][label] + self.node_sizes[ii + lr][label] / 2
-                    self.draw_label(xx, yy, label, ha)
+            xx = x_lr[lr] - self.x_label_gap
+            for label in self.node_sizes[ii + lr]:
+                if (label not in self.node_sizes[ii]) or self.label_duplicate:
+                    yy = self.node_pos_bot[ii][lr][label] + self.node_sizes[ii + lr][label] / 2
+                    self.draw_label(xx, yy, label, "right")
 
         # inside labels, center
         if ii < self.num_flow - 1 and self.label_loc[1] in ("center"):
-            xx = x_lr[lr] + x_node_width / 2
-            ha = "center"
-            for label in nodes_lr[lr]:
-                if (label not in nodes_lr[lr - 1]) or self.label_duplicate:
-                    yy = node_pos_bot[lr][label] + self.node_sizes[ii + lr][label] / 2
-                    self.draw_label(xx, yy, label, ha)
+            xx = x_lr[lr] + self.x_node_width / 2
+            for label in self.node_sizes[ii + lr]:
+                if (label not in self.node_sizes[ii]) or self.label_duplicate:
+                    yy = self.node_pos_bot[ii][lr][label] + self.node_sizes[ii + lr][label] / 2
+                    self.draw_label(xx, yy, label, "center")
+
+        # inside labels, top
+        if ii < self.num_flow - 1 and self.label_loc[1] in ("top"):
+            xx = x_lr[lr] + self.x_node_width / 2
+            for label in self.node_sizes[ii + lr]:
+                if (label not in self.node_sizes[ii]) or self.label_duplicate:
+                    yy = self.node_pos_bot[ii][lr][label] + self.node_sizes[ii + lr][label] + self.y_label_gap
+                    self.draw_label(xx, yy, label, "center")
 
         # inside labels, right
         if ii < self.num_flow - 1 and self.label_loc[1] in ("right", "both"):
-            xx = x_lr[lr] + x_label_gap + x_node_width
-            ha = "left"
-            for label in nodes_lr[lr]:
-                if (label not in nodes_lr[lr - 1]) or self.label_duplicate:
-                    yy = node_pos_bot[lr][label] + self.node_sizes[ii + lr][label] / 2
-                    self.draw_label(xx, yy, label, ha)
+            xx = x_lr[lr] + self.x_label_gap + self.x_node_width
+            for label in self.node_sizes[ii + lr]:
+                if (label not in self.node_sizes[ii]) or self.label_duplicate:
+                    yy = self.node_pos_bot[ii][lr][label] + self.node_sizes[ii + lr][label] / 2
+                    self.draw_label(xx, yy, label, "left")
 
         # last row of labels
         if ii == self.num_flow - 1 and self.label_loc[2] != "none":
             if self.label_loc[2] in ("left"):
-                xx = x_lr[lr] - x_label_gap
+                xx = x_lr[lr] - self.x_label_gap
             elif self.label_loc[2] in ("right"):
-                xx = x_lr[lr] + x_label_gap + x_node_width
-            elif self.label_loc[2] in ("center"):
-                xx = x_lr[lr] + x_node_width / 2
-            for label in nodes_lr[lr]:
-                yy = node_pos_bot[lr][label] + self.node_sizes[ii + lr][label] / 2
+                xx = x_lr[lr] + self.x_label_gap + self.x_node_width
+            elif self.label_loc[2] in ("center", "top"):
+                xx = x_lr[lr] + self.x_node_width / 2
+            for label in self.node_sizes[ii + lr]:
+                if self.label_loc[0] in ("top"):
+                    yy = self.node_pos_bot[ii][lr][label] + self.node_sizes[ii + lr][label] + self.y_label_gap
+                else:
+                    yy = self.node_pos_bot[ii][lr][label] + self.node_sizes[ii + lr][label] / 2
                 self.draw_label(xx, yy, label, ha_dict[self.label_loc[2]])
 
         # Plot flows
 
-        for lbl_l in nodes_lr[0]:
-            for lbl_r in nodes_lr[1]:
-                lind = labels_lr[0] == lbl_l
-                rind = labels_lr[1] == lbl_r
-                if not any(lind & rind):
-                    continue
-
-                lbot = node_voffset[0][lbl_l] + node_pos_bot[0][lbl_l]
-                rbot = node_voffset[1][lbl_r] + node_pos_bot[1][lbl_r]
-                llen = nodesize[0][lbl_l][lbl_r]
-                rlen = nodesize[1][lbl_l][lbl_r]
-                bot_lr = [lbot, rbot]
-                len_lr = [llen, rlen]
-
-                ys_d = self.create_curve(lbot, rbot)
-                ys_u = self.create_curve(lbot + llen, rbot + rlen)
-
-                # Update bottom edges at each label
-                # so next strip starts at the right place
-                node_pos_bot[0][lbl_l] += llen
-                node_pos_bot[1][lbl_r] += rlen
-
-                xx = np.linspace(x_lr[0], x_lr[1], len(ys_d))
-                cc = self.combine_colours(self.color_dict[lbl_l], self.color_dict[lbl_r], len(ys_d))
-
-                for jj in range(len(ys_d) - 1):
-                    self.draw_flow(
-                        xx[[jj, jj + 1]],
-                        ys_d[[jj, jj + 1]],
-                        ys_u[[jj, jj + 1]],
-                        cc[:, jj],
-                    )
+        for lbl_l, lbl_r in self.node_pairs[ii]:
+            lbot = self.node_pos_voffset[ii][0][lbl_l] + self.node_pos_bot[ii][0][lbl_l]
+            rbot = self.node_pos_voffset[ii][1][lbl_r] + self.node_pos_bot[ii][1][lbl_r]
+            llen = self.nodesize_l[ii][lbl_l][lbl_r]
+            rlen = self.nodesize_r[ii][lbl_l][lbl_r]
+            bot_lr = [lbot, rbot]
+            len_lr = [llen, rlen]
+
+            ys_d = self.create_curve(lbot, rbot)
+            ys_u = self.create_curve(lbot + llen, rbot + rlen)
+
+            # Update bottom edges at each label
+            # so next strip starts at the right place
+            self.node_pos_bot[ii][0][lbl_l] += llen
+            self.node_pos_bot[ii][1][lbl_r] += rlen
+
+            xx = np.linspace(x_lr[0], x_lr[1], len(ys_d))
+            cc = self.combine_colours(self.color_dict[lbl_l], self.color_dict[lbl_r], len(ys_d))
+
+            for jj in range(len(ys_d) - 1):
+                self.draw_flow(
+                    xx[[jj, jj + 1]],
+                    ys_d[[jj, jj + 1]],
+                    ys_u[[jj, jj + 1]],
+                    cc[:, jj],
+                )
 
-                ha = ["left", "right"]
-                sides = []
-                if ii == 0:
-                    ind = 0
-                elif ii == self.num_flow - 1:
-                    ind = 2
-                else:
-                    ind = 1
-                if self.value_loc[ind] in ("left", "both"):
-                    sides.append(0)
-                if self.value_loc[ind] in ("right", "both"):
-                    sides.append(1)
-                for lr in sides:
-                    val = len_lr[lr]
-                    if (
-                        val < self.value_thresh_val
-                        or val < self.value_thresh_sum * self.weight_sum[ii + lr]
-                        or val < self.value_thresh_max * max(self.data[2 * ii + 1])
-                    ):
-                        continue
-                    self.ax.text(
-                        x_lr[lr] + (1 - 2 * lr) * x_value_gap,
+            ha = ["left", "right"]
+            sides = []
+            if ii == 0:
+                ind = 0
+            elif ii == self.num_flow - 1:
+                ind = 2
+            else:
+                ind = 1
+            if self.value_loc[ind] in ("left", "both"):
+                sides.append(0)
+            if self.value_loc[ind] in ("right", "both"):
+                sides.append(1)
+            for lr in sides:
+                val = len_lr[lr]
+                if not (
+                    val < self.value_thresh_val
+                    or val < self.value_thresh_sum * self.weight_sum[ii + lr]
+                    or val < self.value_thresh_max * max(self.data[2 * ii + 1])
+                ):
+                    self.draw_value(
+                        x_lr[lr] + (1 - 2 * lr) * self.x_value_gap,
                         bot_lr[lr] + len_lr[lr] / 2,
-                        f"{format(val,self.value_format)}",
-                        {
-                            "ha": ha[lr],
-                            "va": "center",
-                            "fontfamily": self.fontfamily,
-                            "fontsize": self.fontsize,
-                            "color": self.fontcolor,
-                            **self.value_font,
-                        },
+                        val,
+                        ha[lr],
                     )
 
-        # Place "titles"
-        if self.titles is not None:
-            last_label = [lbl_l, lbl_r]
-            title_x = [x_lr[0] - x_node_width / 2, x_lr[1] + x_node_width / 2]
-
-            for lr in [0, 1] if ii == 0 else [1]:
-                if self.title_side in ("top", "both"):
-                    if self.title_loc == "outer":
-                        yt = min(self.voffset) + y_title_gap + y_frame_gap + self.plot_height
-                    elif self.title_loc == "inner":
-                        yt = y_title_gap + node_pos_top[lr][last_label[lr]]
-                    self.draw_title(title_x[lr], yt, self.titles[ii + lr], "bottom")
-
-                if self.title_side in ("bottom", "both"):
-                    if self.title_loc == "outer":
-                        yt = min(self.voffset) - y_title_gap - y_frame_gap
-                    elif self.title_loc == "inner":
-                        yt = self.voffset[ii + lr] - y_title_gap
-                    self.draw_title(title_x[lr], yt, self.titles[ii + lr], "top")
+    ###########################################
+
+    def plot_titles(self, ii):
+        """Subroutine for placing titles"""
+
+        x_lr = self.x_lr[ii]
+
+        title_x = [x_lr[0] - self.x_node_width / 2, x_lr[1] + self.x_node_width / 2]
+
+        for lr in [0, 1] if ii == 0 else [1]:
+            last_label = list(self.node_sizes[ii + lr])[-1]
+            if self.title_side in ("top", "both"):
+                if self.title_loc == "outer":
+                    yt = min(self.voffset) + self.y_title_gap + self.y_frame_gap + self.plot_height
+                elif self.title_loc == "inner":
+                    yt = self.y_title_gap + self.node_pos_top[ii][lr][last_label]
+                self.draw_title(title_x[lr], yt, self.titles[ii + lr], "bottom")
+
+            if self.title_side in ("bottom", "both"):
+                if self.title_loc == "outer":
+                    yt = min(self.voffset) - self.y_title_gap - self.y_frame_gap
+                elif self.title_loc == "inner":
+                    yt = self.voffset[ii + lr] - self.y_title_gap
+                self.draw_title(title_x[lr], yt, self.titles[ii + lr], "top")
 
     ###########################################
 
     def draw_node(self, x, dx, y, dy, label):
         """Draw a single node"""
         edge_lw = self.node_lw if self.node_edge else 0
         self.ax.fill_between(
@@ -762,14 +806,32 @@
                 "color": self.fontcolor,
                 **self.label_font,
             },
         )
 
     ###########################################
 
+    def draw_value(self, x, y, val, ha):
+        """Place a single value label"""
+        self.ax.text(
+            x,
+            y,
+            f"{format(val,self.value_format)}",
+            {
+                "ha": ha,
+                "va": "center",
+                "fontfamily": self.fontfamily,
+                "fontsize": self.fontsize,
+                "color": self.fontcolor,
+                **self.value_font,
+            },
+        )
+
+    ###########################################
+
     def draw_title(self, x, y, label, va):
         """Place a single title"""
         self.ax.text(
             x,
             y,
             label,
             {
@@ -780,31 +842,14 @@
                 "color": self.fontcolor,
                 **self.title_font,
             },
         )
 
     ###########################################
 
-    def sort_nodes(self, lbl, node_sizes):
-        """Creates a sorted list of unique labels into a list"""
-
-        arr = {}
-        for uniq in lbl.unique():
-            if uniq is not None:
-                arr[uniq] = True
-
-        sort_arr = sorted(
-            arr.items(),
-            key=lambda item: list(node_sizes).index(item[0]),
-        )
-
-        return list(dict(sort_arr).keys())
-
-    ###########################################
-
     def sort_node_sizes(self, lbl, sorting):
         """Sorts list of labels and their weights into a dictionary"""
 
         if sorting == "top":
             s = 1
         elif sorting == "bottom":
             s = -1
```

### Comparing `ausankey-1.3/tests/test_fruit_defaults.py` & `ausankey-1.4/tests/test_fruit_defaults.py`

 * *Files identical despite different names*

### Comparing `ausankey-1.3/LICENSE` & `ausankey-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ausankey-1.3/README.md` & `ausankey-1.4/README.md`

 * *Files identical despite different names*

### Comparing `ausankey-1.3/pyproject.toml` & `ausankey-1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "ausankey"
-version = "1.3"
+version = "1.4"
 
 description = "Sankey diagrams simply"
 readme = "README.md"
 license = {file = "LICENSE"}
 
 dependencies = [
     "matplotlib",
@@ -70,16 +70,16 @@
 ]
 
 [tool.hatch.envs.doc]
 dependencies = ["mkdocs", "mkdocstrings[python]"]
 
 [tool.hatch.envs.doc.scripts]
 ref = "mkdocs -v build"
-img = "cd docs; python sankey_doc_examples.py"
-icp = "cd docs; cp -v *.png ../_site/"
+img = "cd docs; python sankey_doc_examples.py; python example_plastics.py"
+icp = "cd docs; cp -v *.png ../_site/; cp -v example_*.png ../_site/examples/"
 
 
 [tool.hatch.envs.test]
 dependencies = [
     "pytest", "coverage", "coveralls",
     "mkdocstrings","mkdocstrings-python",
 ]
```

### Comparing `ausankey-1.3/PKG-INFO` & `ausankey-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ausankey
-Version: 1.3
+Version: 1.4
 Summary: Sankey diagrams simply
 Project-URL: Homepage, https://github.com/AUMAG/ausankey
 Project-URL: Documentation, https://aumag.github.io/ausankey/
 Project-URL: Repository, https://github.com/AUMAG/ausankey.git
 Project-URL: Issues, https://github.com/AUMAG/ausankey/issues
 Project-URL: Changelog, https://github.com/AUMAG/ausankey/blob/master/CHANGELOG.md
 Author-email: Will Robertson <wspr81@gmail.com>
```

