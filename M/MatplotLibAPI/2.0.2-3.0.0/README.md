# Comparing `tmp/MatplotLibAPI-2.0.2.tar.gz` & `tmp/matplotlibapi-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MatplotLibAPI-2.0.2.tar", last modified: Fri Oct 13 11:06:50 2023, max compression
+gzip compressed data, was "matplotlibapi-3.0.0.tar", last modified: Wed May 29 09:06:35 2024, max compression
```

## Comparing `MatplotLibAPI-2.0.2.tar` & `matplotlibapi-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 11:06:50.381023 MatplotLibAPI-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 11:06:50.377023 MatplotLibAPI-2.0.2/MatplotLibAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Bubble.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Network.py
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 11:06:50.377023 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-10-13 11:06:50.381023 MatplotLibAPI-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 11:06:50.381023 MatplotLibAPI-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:35.538916 matplotlibapi-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:35.534916 matplotlibapi-3.0.0/MatplotLibAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/Bubble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/Composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/Network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/Pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/Style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/Timeserie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/MatplotLibAPI/pdAccessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:35.538916 matplotlibapi-3.0.0/MatplotLibAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 09:06:35.000000 matplotlibapi-3.0.0/MatplotLibAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 09:06:35.000000 matplotlibapi-3.0.0/MatplotLibAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:06:35.000000 matplotlibapi-3.0.0/MatplotLibAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 09:06:35.000000 matplotlibapi-3.0.0/MatplotLibAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 09:06:35.000000 matplotlibapi-3.0.0/MatplotLibAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 09:06:35.538916 matplotlibapi-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:06:35.538916 matplotlibapi-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-29 09:06:31.000000 matplotlibapi-3.0.0/setup.py
```

### Comparing `MatplotLibAPI-2.0.2/LICENSE` & `matplotlibapi-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MatplotLibAPI-2.0.2/MatplotLibAPI/Network.py` & `matplotlibapi-3.0.0/MatplotLibAPI/Network.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 import logging
 from collections import defaultdict
 from collections.abc import Iterable
 from typing import Any, Dict, List, Optional, Tuple
 
 import matplotlib.pyplot as plt
+from matplotlib.axes import Axes
+import seaborn as sns
 import networkx as nx
 import numpy as np
 import pandas as pd
 from networkx import Graph
 from networkx.classes.graph import Graph
 
+
+from .Style import StyleTemplate, string_formatter, _validate_panda,format_func
+
+NETWORK_STYLE_TEMPLATE = StyleTemplate(
+)
+
 DEFAULT = {"MAX_EDGES": 100,
            "MAX_NODES": 30,
            "MIN_NODE_SIZE": 100,
            "MAX_NODE_SIZE": 2000,
            "MAX_EDGE_WIDTH": 10,
            "GRAPH_SCALE": 2,
-           "MAX_FONT_SIZE": 12,
+           "MAX_FONT_SIZE": 20,
            "MIN_FONT_SIZE": 8
            }
 
 
 def softmax(x):
     return (np.exp(x - np.max(x)) / np.exp(x - np.max(x)).sum())
 
 
-def scale_weights(weights, scale_min=0,scale_max=1):
+def scale_weights(weights, scale_min=0, scale_max=1):
     deciles = np.percentile(weights, [10, 20, 30, 40, 50, 60, 70, 80, 90])
     outs = np.searchsorted(deciles, weights)
     return [out * (scale_max-scale_min)/len(deciles)+scale_min for out in outs]
 
 
 class NodeView(nx.classes.reportviews.NodeView):
     def sort(self,
@@ -156,65 +164,72 @@
         fonts_size = dict(fonts_size)
 
         return node_size, edges_width, fonts_size
 
     def subgraphX(self, node_list=None, max_edges: int = DEFAULT["MAX_EDGES"]):
         if node_list is None:
             node_list = self.nodes.sort("weight")[:DEFAULT["MAX_NODES"]]
-        connected_subgraph_nodes=list(self.find_connected_subgraph())
-        node_list = [node for node in node_list if node in connected_subgraph_nodes]
+        connected_subgraph_nodes = list(self.find_connected_subgraph())
+        node_list = [
+            node for node in node_list if node in connected_subgraph_nodes]
 
         subgraph = nx.subgraph(
             self, nbunch=node_list)
         edges = subgraph.top_k_edges(attribute="weight", k=5).keys()
         subgraph = subgraph.edge_subgraph(list(edges)[:max_edges])
         return subgraph
 
-    def plotX(self):
+    def plotX(self,
+              title: str = "Test",
+              style: StyleTemplate = NETWORK_STYLE_TEMPLATE,
+              ax: Optional[Axes] = None) -> Axes:
         """
         Plots the degree distribution of the graph, including a degree rank plot and a degree histogram.
         """
         degree_sequence = sorted([d for n, d in self.degree()], reverse=True)
         dmax = max(degree_sequence)
-
-        fig, ax = plt.subplots()
+        sns.set_palette(style.palette)
+        if ax is None:
+            ax = plt.gca()
 
         node_sizes, edge_widths, font_sizes = self.layout(
-            DEFAULT["MAX_NODE_SIZE"], DEFAULT["MAX_EDGE_WIDTH"], 14)
+            min_node_size=DEFAULT["MIN_NODE_SIZE"]/5,
+            max_node_size=DEFAULT["MAX_NODE_SIZE"],
+            max_edge_width=DEFAULT["MAX_EDGE_WIDTH"],
+            min_font_size=style.font_mapping.get(0),
+            max_font_size=style.font_mapping.get(4))
         pos = nx.spring_layout(self, k=1)
         # nodes
         nx.draw_networkx_nodes(self,
                                pos,
                                ax=ax,
                                node_size=list(node_sizes),
-                               # node_color=list(node_sizes.values()),
-                               cmap=plt.cm.Blues)
+                               node_color=node_sizes,
+                               cmap=plt.cm.get_cmap(style.palette))
         # edges
         nx.draw_networkx_edges(self,
                                pos,
                                ax=ax,
-                               alpha=0.4,
+                               edge_color=style.font_color,
+                               edge_cmap=plt.cm.get_cmap(style.palette),
                                width=edge_widths)
         # labels
         for font_size, nodes in font_sizes.items():
             nx.draw_networkx_labels(
                 self,
                 pos,
                 ax=ax,
                 font_size=font_size,
-                labels={n: n for n in nodes},
-                alpha=0.4)
-
-        ax.set_title(self.name)
+                font_color=style.font_color,
+                labels={n: string_formatter(n) for n in nodes})
+        ax.set_facecolor(style.background_color)
+        ax.set_title(title, color=style.font_color, fontsize=style.font_size*2)
         ax.set_axis_off()
 
-
-
-        fig.tight_layout()
-        return fig
+        return ax
 
     def analysis(self, node_list: Optional[List] = None,
                  scale: int = DEFAULT["GRAPH_SCALE"],
                  node_scale: int = DEFAULT["MAX_NODE_SIZE"],
                  edge_scale: float = DEFAULT["MAX_EDGE_WIDTH"],
                  max_nodes: int = DEFAULT["MAX_NODES"],
                  max_edges: int = DEFAULT["MAX_EDGES"],
@@ -238,20 +253,22 @@
 
         while removed_node:
             removed_node = False
             # Iterate over the nodes
             for node in list(H.nodes):
                 if H.degree(node) < 2:
                     # Remove the node and its incident edges
-                    logging.info(f'Removing the {node} node and its incident edges')
+                    logging.info(
+                        f'Removing the {node} node and its incident edges')
                     H.remove_node(node)
                     removed_node = True
                     break
 
         return H
+
     def top_k_edges(self, attribute: str, reverse: bool = True, k: int = 5) -> Dict[Any, List[Tuple[Any, Dict]]]:
         """
         Returns the top k edges per node based on the given attribute.
 
         Parameters:
         attribute (str): The attribute name to be used for sorting.
         reverse (bool): Flag indicating whether to sort in reverse order (default: True).
@@ -271,31 +288,31 @@
             top_k_edges = edges_sorted[:k]
             for u, v, data in top_k_edges:
                 edge_key = (u, v)
                 top_list[edge_key] = data[attribute]
         return top_list
 
     @staticmethod
-    def from_pandas_edgelist(df,
-                             source: Optional[str] = "source",
-                             target: Optional[str] = "target",
-                             weight: Optional[str] = "weight"):
+    def from_pandas_edgelist(df: pd.DataFrame,
+                             source: str = "source",
+                             target: str = "target",
+                             weight: str = "weight"):
         """
         Initialize netX instance with a simple dataframe
 
         :param df_source: DataFrame containing network data.
         :param source: Name of source nodes column in df_source.
         :param target: Name of target nodes column in df_source.
         :param weight: Name of edges weight column in df_source.
 
         """
         G = Graph()
         G = nx.from_pandas_edgelist(
             df, source=source, target=target, edge_attr=weight, create_using=G)
-        G=G.find_connected_subgraph()
+        G = G.find_connected_subgraph()
 
         edge_aggregates = G.top_k_edges(attribute=weight, k=10)
         node_aggregates = {}
         for (u, v), weight_value in edge_aggregates.items():
             if u not in node_aggregates:
                 node_aggregates[u] = 0
             if v not in node_aggregates:
@@ -304,15 +321,27 @@
             node_aggregates[v] += weight_value
 
         nx.set_node_attributes(G, node_aggregates, name=weight)
 
         G = G.edge_subgraph(edges=G.top_k_edges(attribute=weight))
         return G
 
-def plot_network(data:pd.DataFrame):
-    graph = Graph.from_pandas_edgelist(data)
-    graph = graph.subgraphX()
-    return graph.analysis()
-
-
-
 
+def plot_network(pd_df: pd.DataFrame,
+                 source: str = "source",
+                 target: str = "target",
+                 weight: str = "weight",
+                 title: str = "Test",
+                 style: StyleTemplate = NETWORK_STYLE_TEMPLATE,
+                 sort_by: Optional[str] = None,
+                 ascending: bool = False,
+                 ax: Optional[Axes] = None) -> Axes:
+
+    _validate_panda(pd_df, cols=[source, target, weight], sort_by=sort_by)
+    
+    graph = Graph.from_pandas_edgelist(pd_df,
+                                       source=source,
+                                       target=target,
+                                       weight=weight)
+    return graph.plotX(title=title,
+                       style=style,
+                       ax=ax)
```

### Comparing `MatplotLibAPI-2.0.2/MatplotLibAPI/Pivot.py` & `matplotlibapi-3.0.0/MatplotLibAPI/Pivot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,130 @@
+# Hint for Visual Code Python Interactive window
+# %%
 from typing import List, Optional, Union
 
 import pandas as pd
 
 import matplotlib.dates as mdates
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.dates import DateFormatter, MonthLocator
 
-from .Utils import (PIVOTBARS_STYLE_TEMPLATE, PIVOTLINES_STYLE_TEMPLATE,
-                    DynamicFuncFormatter, StyleTemplate, generate_ticks)
 
 
-def plot_pivotbar(data, metric, n_top, title):
-    # Sort the data by metric column in descending order
-    data_sorted = data.sort_values(by=metric, ascending=False)
+from .Style import DynamicFuncFormatter, StyleTemplate, generate_ticks, string_formatter, _validate_panda, percent_formatter,format_func
 
-    # Select the top rows
-    top_rows = data_sorted.head(n_top)
-
-    # Plotting the top 50 data points with tag labels
-    fig, ax = plt.subplots(figsize=(12, 6))
-
-    # Plot the 'Used' data points (where Used == 1) in green
-    used_data = top_rows[top_rows['used'] == 1]
-    ax.bar(used_data.tag, used_data[metric],
-           color='green', label='Used', alpha=0.7)
-
-    # Plot the 'Not Used' data points (where Used == 0) in red
-    not_used_data = top_rows[top_rows['used'] == 0]
-    ax.bar(not_used_data.tag, not_used_data[metric],
-           color='red', label='Not Used', alpha=0.7)
+PIVOTBARS_STYLE_TEMPLATE = StyleTemplate(
+    background_color='black',
+    fig_border='darkgrey',
+    font_color='white',
+    palette='magma',
+    format_funcs={"y": percent_formatter, 
+                  "label": string_formatter}
+)
+PIVOTLINES_STYLE_TEMPLATE = StyleTemplate(
+    background_color='white',
+    fig_border='lightgrey',
+    palette='viridis',
+    format_funcs={"y": percent_formatter, "label": string_formatter}
+)
+
+def plot_pivotbar(pd_df: pd.DataFrame,
+                  label: str,
+                  x: str,
+                  y: str,
+                  agg: str = "sum",
+                  style: StyleTemplate = PIVOTBARS_STYLE_TEMPLATE,
+                  title: Optional[str] = None,
+                  sort_by: Optional[str] = None,
+                  ascending: bool = False,
+                  ax: Optional[Axes] = None):
+
+    _validate_panda(pd_df, cols=[label, x, y], sort_by=sort_by)
+    style.format_funcs=format_func(style.format_funcs,label=label,x=x,y=y)
+    pivot_df = pd.pivot_table(pd_df, values=y, index=[
+                              x], columns=[label], aggfunc=agg)
+    # Reset index to make x a column again
+    pivot_df = pivot_df.reset_index()
+
+    if not ax:
+        ax = plt.gca()
+
+    # Plot each label's data
+    for column in pivot_df.columns[1:]:
+        _label = column
+        if style.format_funcs.get(column):
+            _label = style.format_funcs[column](column)
+        ax.bar(x=pivot_df[x],
+               height=pivot_df[column],
+               label=_label, alpha=0.7)
 
     # Set labels and title
-    ax.set_ylabel('UVs')
-    ax.set_title(f'{title}\nTop {n_top} tags')
-    ax.legend()
+    ax.set_ylabel(string_formatter(y))
+    ax.set_xlabel(string_formatter(x))
+    if title:
+        ax.set_title(f'{title}')
+    ax.legend(fontsize=style.font_size-2,
+              title_fontsize=style.font_size+2,
+              labelcolor='linecolor',
+              facecolor=style.background_color)
 
     ax.tick_params(axis='x', rotation=90)
-    return fig
+    return ax
 
 
-def plot_lines(ax: Axes,
-               data: pd.DataFrame,
-               x_col: str,
-               y_col: Union[str, List[str]],
-               style: Optional[StyleTemplate] = None,
-               fig_title: Optional[str] = None,
-               n_top: int = 4,
-               z_col: str = "browser") -> Axes:
-    """
-    This function plots time series lines for the top n elements in the specified dimension.
-
-    Parameters:
-    ax (matplotlib.axes._axes.Axes): The ax to plot on.
-    data (pd.DataFrame): The data to plot.
-    metrics (Union[str, List[str]]): The column name(s) in data to plot.
-    date_col (str): The column name containing the date information.
-    ... (other parameters): Various parameters to customize the plot.
-    date_format (str): The format of the date to display on the x-axis.
-    date_locator (matplotlib.dates.Locator): Locator object to determine the date ticks on the x-axis.
-
-    Returns:
-    ax (matplotlib.axes._axes.Axes): The ax with the plot.
-    """
-
-    # Validate inputs
-    if x_col not in data.columns:
-        raise ValueError(f"'{x_col}' column not found in the data")
-    if not isinstance(y_col, list) and not isinstance(y_col, str):
-        raise TypeError("'metrics' should be a string or a list of strings")
-    if isinstance(y_col, list) and not len(y_col) >= 2:
-        raise ValueError(
-            f"metrics should be 2 of lengths column not found in the data")
-    ax.clear()
-    if fig_title is not None:
-        ax.set_title(fig_title)
-    if style is None:
-        style = PIVOTLINES_STYLE_TEMPLATE
-    ax.figure.set_facecolor(style.fig_background_color)
+def plot_lines(
+    data: pd.DataFrame,
+    label: str,
+    x: str,
+    y: Union[str, List[str]],
+    title: Optional[str] = None,
+    style: Optional[StyleTemplate] = PIVOTBARS_STYLE_TEMPLATE,
+    max_values: int = 4,
+    sort_by: Optional[str] = None,
+    ascending: bool = False,
+    ax: Optional[Axes] = None
+) -> Axes:
+
+    if title is not None:
+        ax.set_title(title)
+    ax.figure.set_facecolor(style.background_color)
     ax.figure.set_edgecolor(style.fig_border)
-
-    display_metric = y_col[0]
-    sort_metric = y_col[1]
     # Get the top n elements in the specified z
     top_elements = data.groupby(
-        z_col)[sort_metric].sum().nlargest(n_top).index.tolist()
-    top_elements_df = data[data[z_col].isin(top_elements)]
+        label)[y].sum().nlargest(max_values).index.tolist()
+    top_elements_df = data[data[label].isin(top_elements)]
     y_min = 0
     # Plot the time series lines for each of the top elements
     for element in top_elements:
-        subset = top_elements_df[top_elements_df[z_col] == element]
-        # Define the line style based on the element name
-        if element == "Chrome":
-            line_style = '-'
-            color = 'green'
-        elif element == "Android Webview":
-            line_style = '--'
-            color = 'green'
-        elif element == "Safari":
-            line_style = '-'
-            color = 'red'
-        elif element == "Safari (in-app)":
-            line_style = '--'
-            color = 'red'
-        else:
-            line_style = '-'
-            color = 'black'
-        y_min = min(y_min, subset[display_metric].min())
-
-        ax.plot(subset[x_col], subset[display_metric], label=element)
+        subset = top_elements_df[top_elements_df[label] == element]
+        y_min = min(y_min, subset[y].min())
+        ax.plot(subset[x], subset[y], label=element)
 
     # Set x-axis date format and locator
         if style.x_formatter is not None:
-            x_min = data[x_col].min()
-            x_max = data[x_col].max()
+            x_min = data[x].min()
+            x_max = data[x].max()
 
             if style.x_formatter == "year_month_formatter":
                 ax.xaxis.set_major_locator(plt.matplotlib.dates.MonthLocator())
             else:
                 ax.xaxis.set_major_formatter(
                     DynamicFuncFormatter(style.x_formatter))
                 ax.set_xticks(generate_ticks(
                     x_min, x_max, num_ticks=style.x_ticks))
 
     ax.set_xticklabels(ax.get_xticklabels(), rotation=45)
 
     # Set title and labels
-    ax.set_xlabel(x_col)
-    y_max = data[display_metric].dropna().quantile(0.95)
+    ax.set_xlabel(x)
+    y_max = data[y].dropna().quantile(0.95)
 
     ax.set_ylim(y_min, y_max)
-    ax.set_ylabel(display_metric)
+    ax.set_ylabel(y)
     if style.y_formatter is not None:
         ax.yaxis.set_major_formatter(
             DynamicFuncFormatter(style.y_formatter))
         ax.set_yticks(generate_ticks(
             y_min, y_max, num_ticks=style.y_ticks))
     else:
         ylabels = ['{:,.0f}%'.format(y) for y in ax.get_yticks()*100]
```

### Comparing `MatplotLibAPI-2.0.2/MatplotLibAPI/Table.py` & `matplotlibapi-3.0.0/MatplotLibAPI/Table.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,65 @@
-import logging
-from typing import List, Optional, Dict, Callable
+from typing import List, Optional
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
+from .Style import StyleTemplate, _validate_panda, string_formatter
 
-
-def plot_table(ax: Axes,
-               data: pd.DataFrame,
-               mappings: Dict[str, Callable[[pd.Series], pd.Series]],
-               sort_column: str = "INDEX",
-               sort_ascending: bool = False,
-               num_rows: int = None,
-               fig_background_color: str = 'black',
-               fig_border: str = 'white',
-               font_name: str = 'Arial',
-               font_size: int = 10,
-               font_color="black",
-               fig_title: Optional[str] = None,
-               col_widths: Optional[List[float]] = None) -> Axes:
-    """
-    Plots a table using Matplotlib in the provided axis.
-
-    Parameters:
-        ax (Axes): The Matplotlib axis to plot the table in.
-        data (pd.DataFrame): The pandas DataFrame containing the table data.
-        mappings (dict): Dictionary mapping column names to functions that transform the column data.
-        sort_column (str, optional): Column to sort the data by. Default is "INDEX".
-        sort_ascending (bool, optional): Whether to sort in ascending order. Default is False.
-        num_rows (int, optional): Number of rows to display. Default is 10.
-        fig_background_color (str, optional): Background color of the figure. Default is 'skyblue'.
-        fig_border (str, optional): Border color of the figure. Default is 'steelblue'.
-        font_name (str, optional): Font name for the table cells. Default is 'Arial'.
-        font_size (int, optional): Font size for the table cells. Default is 10.
-        col_widths (list, optional): List of relative column widths. Default is None.
-
-    Returns:
-        Axes: The Matplotlib axis with the plotted table.
-    """
-
-    if num_rows is None:
-        num_rows = len(data.index)
-    cols = list(mappings.keys())
-    plot_data = data[cols].copy().sort_values(
-        by=sort_column, ascending=sort_ascending).head(num_rows).reset_index(drop=True)
-
-    for col, func in mappings.items():
-        plot_data[col] = plot_data[col].apply(func)
-    if fig_title is not None:
-        ax.text(0.5, 1.05,
-                fig_title,
-                va='top',
-                ha='center',
-                fontsize=font_size*1.5,
-                fontname=font_name,
-                color=font_color,
-                transform=ax.transAxes)
-    table = ax.table(cellText=plot_data.values, colLabels=plot_data.columns,
-                     cellLoc='center', colWidths=col_widths, loc="center")
-    table.auto_set_font_size(False)
-    table.set_fontsize(font_size)
-
-    for key, cell in table.get_celld().items():
-        cell.get_text().set_fontname(font_name)
-        cell.get_text().set_color(font_color)
-    table.scale(1, 4)
-    table.auto_set_column_width(col=list(range(len(plot_data.columns))))
-    ax.axis('off')
-
+TABLE_STYLE_TEMPLATE = StyleTemplate(
+    background_color='black',
+    fig_border='darkgrey',
+    font_color='white',
+    palette='magma'
+)
+
+
+def plot_table(pd_df: pd.DataFrame,
+               cols: List[str],
+               title: Optional[str] = None,
+               style: StyleTemplate = TABLE_STYLE_TEMPLATE,
+               max_values: int = 20,
+               sort_by: Optional[str] = None,
+               ascending: bool = False,
+               ax: Optional[Axes] = None
+               ) -> Axes:
+    _validate_panda(pd_df, cols=cols, sort_by=sort_by)
+    
+    if not sort_by:
+        sort_by = cols[0]
+
+    plot_df = pd_df[cols].sort_values(
+        by=sort_by, ascending=ascending).head(max_values)
+
+    col_labels = cols
+
+    if style.format_funcs:
+        for col, func in style.format_funcs.items():
+            if col in plot_df.columns:
+                plot_df[col] = plot_df[col].apply(func)
+
+    def format_table(table):
+        table.auto_set_font_size(False)
+        table.set_fontsize(style.font_size)
+        table.scale(1.2, 1.2)
+
+        for key, cell in table.get_celld().items():
+            cell.set_fontsize(style.font_size)
+            cell.set_facecolor(style.background_color)
+            cell.get_text().set_color(style.font_color)
+
+    if ax is None:
+        ax = plt.gca()
+
+    table_plot = ax.table(
+        cellText=plot_df.values,
+        colLabels=[string_formatter(colLabel) for colLabel in col_labels],
+        cellLoc='center',
+        colWidths=style.col_widths,
+        bbox=[0, -0.3, 1, 1.3])
+    format_table(table_plot)
+    ax.set_facecolor(style.background_color)
+    ax.set_axis_off()
+    ax.grid(False)
+    if title:
+        ax.set_title(title, color=style.font_color, fontsize=style.font_size*2)
+        ax.title.set_position([0.5, 1.05])
     return ax
```

