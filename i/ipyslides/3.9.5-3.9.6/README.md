# Comparing `tmp/ipyslides-3.9.5.tar.gz` & `tmp/ipyslides-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.9.5.tar", last modified: Tue May 28 02:17:38 2024, max compression
+gzip compressed data, was "ipyslides-3.9.6.tar", last modified: Tue May 28 18:30:39 2024, max compression
```

## Comparing `ipyslides-3.9.5.tar` & `ipyslides-3.9.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.449459 ipyslides-3.9.5/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.5/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-28 02:17:38.446990 ipyslides-3.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.373288 ipyslides-3.9.5/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.5/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-28 02:12:28.000000 ipyslides-3.9.5/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.441356 ipyslides-3.9.5/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.5/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    41105 2024-05-28 00:21:37.000000 ipyslides-3.9.5/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.5/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33033 2024-05-19 18:10:13.000000 ipyslides-3.9.5/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.5/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.5/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.5/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0     7917 2024-05-27 18:33:15.000000 ipyslides-3.9.5/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.444032 ipyslides-3.9.5/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.5/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1867 2024-05-28 02:16:56.000000 ipyslides-3.9.5/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.5/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2526 2024-05-28 02:12:02.000000 ipyslides-3.9.5/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    11908 2024-05-19 16:37:54.000000 ipyslides-3.9.5/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.5/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.5/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.5/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    16285 2024-05-28 00:22:32.000000 ipyslides-3.9.5/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    12585 2024-05-27 18:30:09.000000 ipyslides-3.9.5/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    47752 2024-05-28 00:20:37.000000 ipyslides-3.9.5/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.5/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.5/ipyslides/source.py
--rw-rw-rw-   0        0        0    29519 2024-05-19 18:02:34.000000 ipyslides-3.9.5/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.5/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.5/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.409452 ipyslides-3.9.5/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 02:17:38.449459 ipyslides-3.9.5/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:30:39.989714 ipyslides-3.9.6/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.6/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-28 18:30:39.987705 ipyslides-3.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 18:30:39.906798 ipyslides-3.9.6/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.6/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-28 18:09:40.000000 ipyslides-3.9.6/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:30:39.983171 ipyslides-3.9.6/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.6/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    41105 2024-05-28 00:21:37.000000 ipyslides-3.9.6/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6170 2024-05-28 17:17:01.000000 ipyslides-3.9.6/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33033 2024-05-19 18:10:13.000000 ipyslides-3.9.6/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.6/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.6/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.6/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0     7917 2024-05-27 18:33:15.000000 ipyslides-3.9.6/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:30:39.986721 ipyslides-3.9.6/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.6/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1874 2024-05-28 17:40:55.000000 ipyslides-3.9.6/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.6/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2620 2024-05-28 17:24:24.000000 ipyslides-3.9.6/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11908 2024-05-19 16:37:54.000000 ipyslides-3.9.6/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.6/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.6/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.6/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16285 2024-05-28 00:22:32.000000 ipyslides-3.9.6/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    12585 2024-05-27 18:30:09.000000 ipyslides-3.9.6/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47752 2024-05-28 00:20:37.000000 ipyslides-3.9.6/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.6/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.6/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29812 2024-05-28 18:27:31.000000 ipyslides-3.9.6/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.6/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.6/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:30:39.958213 ipyslides-3.9.6/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-28 18:30:39.000000 ipyslides-3.9.6/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-28 18:30:39.000000 ipyslides-3.9.6/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 18:30:39.000000 ipyslides-3.9.6/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-28 18:30:39.000000 ipyslides-3.9.6/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 18:30:39.000000 ipyslides-3.9.6/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 18:30:39.989714 ipyslides-3.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.6/setup.py
```

### Comparing `ipyslides-3.9.5/LICENSE` & `ipyslides-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/PKG-INFO` & `ipyslides-3.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.5
+Version: 3.9.6
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.5/README.md` & `ipyslides-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/_layout_css.py` & `ipyslides-3.9.6/ipyslides/_base/_layout_css.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/_widgets.py` & `ipyslides-3.9.6/ipyslides/_base/_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
 class HtmlWidget(anywidget.AnyWidget):
     """This introduces a trait 'click_state' which would be toggled between 0 and 1 on each click.
     You can either have a function for click or mimic a double click as well.
     """
     _esm = """
     export function render({ model, el }) {
+    el.classList.add("jupyter-widgets", "widget-html-content"); // for consistent view
     let div = document.createElement("div");
     div.classList.add("jp-RenderedHTMLCommon","custom-html","jp-mod-trusted");
     function set_html() {
         div.innerHTML = model.get("value");
     }
     el.tabIndex = -1; // need for clickable events
     el.onclick = (event) => {
```

### Comparing `ipyslides-3.9.5/ipyslides/_base/base.py` & `ipyslides-3.9.6/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/export_html.py` & `ipyslides-3.9.6/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/export_template.py` & `ipyslides-3.9.6/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/icons.py` & `ipyslides-3.9.6/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/intro.py` & `ipyslides-3.9.6/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/js/interaction.js` & `ipyslides-3.9.6/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/js/notes.js` & `ipyslides-3.9.6/ipyslides/_base/js/notes.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 // This needs more thoughts to send data properly
 
 function setupNotesWindow(notes_win) {
-    notes_win.resizeTo(screen.width / 2, screen.height / 2);
+    notes_win.resizeTo(screen.width / 3, screen.height / 3);
     notes_win.moveTo(0, 0); // top left corner
-    notes_win.document.title = 'Notes';
+    notes_win.document.title = 'IPySlides Notes';
     notes_win.document.body.style.background = 'var(--primary-bg)';
     notes_win.document.body.style.color = 'var(--primary-fg)';
     window.focus(); // Return focus to main window automatically
 };
 
 
 function setTime(notes_win) {
@@ -18,15 +18,15 @@
         let date = new Date();
         let timer = notes_win.document.getElementById("timer");
         timer.innerText = "" + pad(date.getHours()) + ":" + pad(date.getMinutes())
     }
 }
 
 function setValue(notes_win, value) {
-    let out = "<span style='position:absolute;right:4px;bottom:2px;'>🕑<b id='timer'>Time</b></span>" + value;
+    let out = "<span style='position:fixed;right:4px;bottom:2px;'>🕑<b id='timer'>Time</b></span>" + value;
     notes_win.document.body.innerHTML = out
     setTime(notes_win); // show time immediately
 }
 
 var timerId;
 
 export function render({
```

### Comparing `ipyslides-3.9.5/ipyslides/_base/navigation.py` & `ipyslides-3.9.6/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/notes.py` & `ipyslides-3.9.6/ipyslides/_base/notes.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,22 @@
     __call__ = insert # Can be called as function
     
     def display(self):
         def set_value(content):
             bg = self.main.settings.colors.get('primary_bg','white')
             fg = self.main.settings.colors.get('primary_fg','black')
             bg2 = self.main.settings.colors.get('secondary_bg','#181818')
+            font = self.main.settings._font_family.get('text', 'Roboto')
             return f"""<style>
         :root {{
             --primary-bg : {bg};
             --primary-fg : {fg};
             --secondary-bg: {bg2};
         }}
-        .columns {{columns: 2 auto;}}
+        .columns {{columns: 2 auto;font-family: {font};}}
         .columns > div > * {{background: {bg2};padding:0.2em;font-size:110%;border-left: 2px inset {bg};}}
         .columns > div:first-child::before {{content:'This Slide';font-size:80%;font-weight:bold;}}
         .columns > div:last-child::before {{content:'Next Slide';font-size:80%;font-weight:bold;}}
         </style>{content}"""
 
         this_notes = self.main.current.notes 
         next_slide_index = (self.main.current.index + 1) % len(self.main)
```

### Comparing `ipyslides-3.9.5/ipyslides/_base/screenshot.py` & `ipyslides-3.9.6/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/settings.py` & `ipyslides-3.9.6/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/slide.py` & `ipyslides-3.9.6/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/styles.py` & `ipyslides-3.9.6/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_base/widgets.py` & `ipyslides-3.9.6/ipyslides/_base/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/_demo.py` & `ipyslides-3.9.6/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/core.py` & `ipyslides-3.9.6/ipyslides/core.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/formatters.py` & `ipyslides-3.9.6/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/source.py` & `ipyslides-3.9.6/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/utils.py` & `ipyslides-3.9.6/ipyslides/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,30 +414,35 @@
     if isinstance(obj,ipw.DOMWidget):
         return ipw.Box([obj]).add_class('align-center') # needs to wrap in another for cenering
     else:
         return XTML(f'<div class="align-center">{htmlize(obj)}</div>')
     
 def html(tag, children = None,className = None,**node_attrs):
     """Returns html node with given children and node attributes like style, id etc. If an ttribute needs '-' in its name, replace it with '_'.     
-    `tag` can be any valid html tag name. A `tag` that ends with `/` will be self closing e.g. `hr/` will be `<hr/>`.     
+    `tag` can be any valid html tag name. A `tag` that ends with `/` will be self closing e.g. `hr/` will be `<hr/>`.  Empty tag gives unwrapped children.
     `children` expects:
     
     - If None, returns node such as 'image' -> <img alt='Image'></img> and 'image/' -> <img alt='Image' />
     - str: A string to be added as node's text content.
     - list/tuple of [objects]: A list of objects that will be parsed and added as child nodes. Widgets are not supported.
     
     Example:
     ```python
     html('img',src='ir_uv.jpg') #Returns IPython.display.HTML("<img src='ir_uv.jpg'></img>") and displas image if last line in notebook's cell.
     ```
     
     ::: note-tip 
         To keep an image persistently embeded, use `ipyslides.utils.imge` function instead of just an html tag.
     """
-    if tag in 'hr/':
+    if not isinstance(tag, str):
+        raise TypeError('tag should be a string of html tags or empty string!')
+    
+    tag = tag.strip() # clean up
+    
+    if tag in ['hr', 'hr/']: 
         return XTML(f'<hr/>') # Special case for hr
     
     if children and tag.endswith('/'):
         raise RuntimeError(f'Parametr `children` should be None for self closing tag {tag!r}')
     
     if tag == 'style':
         node_attrs = {} # Ignore node_attrs for style tag
@@ -455,14 +460,17 @@
         content = ''
     elif isinstance(children,str):
         content = children
     elif isinstance(children,(list,tuple)):
         content = '\n'.join(htmlize(child) for child in children) # Convert to html nodes in sequence of rows
     else:
         raise TypeError(f'Children should be a list/tuple of objects or str, not {type(children)}')
+    
+    if not tag: # empty tag.
+        return XTML(content) # don't wrap in any node
         
     tag_in =  f'<{tag} {attrs}>' if attrs else f'<{tag}>' # space is must after tag, strip attrs spaces
     return XTML(f'{tag_in}{content}</{tag}>')
 
 def vspace(em = 1):
     "Returns html node with given height in `em`."
     return html('div',style=f'height:{em}em;')
```

### Comparing `ipyslides-3.9.5/ipyslides/writer.py` & `ipyslides-3.9.6/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides/xmd.py` & `ipyslides-3.9.6/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.9.6/ipyslides.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.5
+Version: 3.9.6
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.5/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.9.6/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.5/setup.py` & `ipyslides-3.9.6/setup.py`

 * *Files identical despite different names*

