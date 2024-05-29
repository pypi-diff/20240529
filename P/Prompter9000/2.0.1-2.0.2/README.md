# Comparing `tmp/Prompter9000-2.0.1.tar.gz` & `tmp/prompter9000-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Prompter9000-2.0.1.tar", last modified: Wed Nov 22 11:51:06 2023, max compression
+gzip compressed data, was "prompter9000-2.0.2.tar", last modified: Wed May 29 16:52:45 2024, max compression
```

## Comparing `Prompter9000-2.0.1.tar` & `prompter9000-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-22 11:51:06.217149 Prompter9000-2.0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-18 19:48:50.000000 Prompter9000-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     1703 2023-11-22 11:51:06.216148 Prompter9000-2.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-11-22 11:51:06.199147 Prompter9000-2.0.1/Prompter9000/
--rw-rw-rw-   0        0        0     7422 2023-11-22 10:46:45.000000 Prompter9000-2.0.1/Prompter9000/PyCount.py
--rw-rw-rw-   0        0        0     6475 2023-09-29 13:34:23.000000 Prompter9000-2.0.1/Prompter9000/PyEdit.py
--rw-rw-rw-   0        0        0       33 2023-11-22 11:48:58.000000 Prompter9000-2.0.1/Prompter9000/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-22 11:51:06.214146 Prompter9000-2.0.1/Prompter9000.egg-info/
--rw-rw-rw-   0        0        0     1703 2023-11-22 11:51:06.000000 Prompter9000-2.0.1/Prompter9000.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-11-22 11:51:06.000000 Prompter9000-2.0.1/Prompter9000.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-22 11:51:06.000000 Prompter9000-2.0.1/Prompter9000.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-22 11:51:06.000000 Prompter9000-2.0.1/Prompter9000.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1180 2023-11-22 10:56:12.000000 Prompter9000-2.0.1/README.md
--rw-rw-rw-   0        0        0      511 2023-11-22 11:49:50.000000 Prompter9000-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-22 11:51:06.218150 Prompter9000-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 16:52:45.032479 prompter9000-2.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 19:48:50.000000 prompter9000-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1998 2024-05-29 16:52:45.030526 prompter9000-2.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 16:52:45.001213 prompter9000-2.0.2/Prompter9000/
+-rw-rw-rw-   0        0        0     7422 2023-11-22 10:46:45.000000 prompter9000-2.0.2/Prompter9000/PyCount.py
+-rw-rw-rw-   0        0        0     7809 2024-05-29 16:28:04.000000 prompter9000-2.0.2/Prompter9000/PyEdit.py
+-rw-rw-rw-   0        0        0       33 2023-11-22 11:48:58.000000 prompter9000-2.0.2/Prompter9000/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:52:45.028571 prompter9000-2.0.2/Prompter9000.egg-info/
+-rw-rw-rw-   0        0        0     1998 2024-05-29 16:52:44.000000 prompter9000-2.0.2/Prompter9000.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-29 16:52:44.000000 prompter9000-2.0.2/Prompter9000.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 16:52:44.000000 prompter9000-2.0.2/Prompter9000.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 16:52:44.000000 prompter9000-2.0.2/Prompter9000.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1475 2024-05-29 16:52:09.000000 prompter9000-2.0.2/README.md
+-rw-rw-rw-   0        0        0      511 2024-05-29 16:11:46.000000 prompter9000-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 16:52:45.032479 prompter9000-2.0.2/setup.cfg
```

### Comparing `Prompter9000-2.0.1/LICENSE` & `prompter9000-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Prompter9000-2.0.1/PKG-INFO` & `prompter9000-2.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: Prompter9000
-Version: 2.0.1
+Version: 2.0.2
 Summary: C.L.I <-> G.U.I Dictionary Editor
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/Blog9000
 Project-URL: Bug Tracker, https://github.com/soft9000/Blog9000/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Prompter9000
-Quick &amp; easy way to edit dictionaries and create counters. Console & programmatic usages are supported.
+Quick &amp; easy way to edit dictionaries and create counters. Console & programmatic 
+usages are supported.
+
+**NEW:** *Verson 2.0.2*
+1. Data types can now be preserved. 
+2. Boolean detection, as well.
+3. Result Key [__conv_ok]
+    - == *True* iff types preserved. 
+    - *False* == at least one defaulted to string.
+4.) Result Key [__btn_ok]
+    - == *True* when [Okay] was pressed
+    - else *False*.
 
 ### Programatic
 Edit a dictionary:
 ```
 from Prompter9000.PyEdit import *
-params = {"NAME":'My', "PHONE":'123-456', "EMAIL":'a.Geekbo@zbobo.com'}
+params = {"NAME":'My', "ACCOUNT":123456, "Subscriber":False}
 EditDict.edit(params)
 ```
 
 Create a click-counter:
 ```
 from Prompter9000.PyCount import *
 params = {'Hits': '0', 'Miss': '0', 'Other': '10'}
```

### Comparing `Prompter9000-2.0.1/Prompter9000/PyCount.py` & `prompter9000-2.0.2/Prompter9000/PyCount.py`

 * *Files identical despite different names*

### Comparing `Prompter9000-2.0.1/Prompter9000/PyEdit.py` & `prompter9000-2.0.2/Prompter9000/PyEdit.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 class EditDict:
     '''Graphically exchange a dictionary of strings with a user. Dictionary keys match fields requested. Font, size, and label allignment can be selected upon construction as per Tkinter definition.
 
 G.U.I Usage:
 ===========
 from Prompter9000.PyEdit import *
-params = {"NAME":'My', "PHONE":'123-456', "EMAIL":'a.Geekbo@zbobo.com'}
+params = {"NAME":'My', "ACCOUNT":123456, "EMAIL":'a.Geekbo@zbobo.com'}
 EditDict.edit(params)
 
 NOTE: Dictionary results will be returned ONLY IF the data was changed. Otherwise an empty dictionary will be returned.
 
 Console Usage:
 =============    
-python PyEdit.py "{'NAME': 'My', 'PHONE': '123-456', 'EMAIL': 'a.Geekbo@zbobo.com'}"{'NAME': 'My', 'PHONE': '123-456', 'EMAIL': 'a.Geekbo@zbobo.com', '__btn_ok': True}
+python PyEdit.py "{'NAME': 'My', 'ACCOUNT': '123456', 'EMAIL': 'a.Geekbo@zbobo.com'}"{'NAME': 'My', 'PHONE': '123-456', 'EMAIL': 'a.Geekbo@zbobo.com', '__btn_ok': True}
 
 NOTES: Please encode your dictionary as a single str(dict()) parameter when using the CLI. Results will be returned as a dictionary of strings. A __btn_ok key is added and will be `True` if [Okay] was selected, else is `False` if user pressed [Cancel].
 '''
     def __init__(self, a_dict, font_size=16, font_name='TkFixedFont', align='e'):
         '''
         Initialize fileds. Optional horizontal alignments
         are n, s, [e], w ... Tk's `sticky` grid options.
@@ -45,14 +45,48 @@
         self._isOk = True
         self.tk.quit()
 
     def _cancel(self):
         self._isOk = False
         self.tk.quit()
 
+    def as_bool(self, _input:str)->bool:
+        ''' Read boolean from the string input.
+        Returns True if input is either 'yes', 'true', or '1'
+        '''
+        if _input:
+            _input = _input.lower()
+            if  (_input[0] == 'y') or \
+                (_input[0] == 't') or \
+                (_input[0] == '1'):
+                    return True
+        return False
+
+    def _convert(self, row, field, value):
+        ''' Attempt to convert + assign a string value
+            back to a row's input type. Default is to 
+            simply assign value as-passed. 
+            Return False on error.
+        '''
+        if not isinstance(row, dict):
+            return False
+        try:
+            target = row[field]
+            if isinstance(target, bool):
+                row[field] = self.as_bool(value)
+            elif isinstance(target, int):
+                row[field] = int(value)
+            elif isinstance(target, float):
+                row[field] = float(value)
+            else:
+                row[field] = value
+            return True
+        except:
+            return False
+
     @staticmethod
     def begin(fields, title="Input",
              font_size=16, font_name='TkFixedFont',
              align='e'):
         ''' Create the frame, add the title, as well as the input fields.'''
         self = EditDict(fields, font_size, font_name, align)
         self.tk = Tk()
@@ -117,21 +151,23 @@
         return True
 
     def show(self):
         ''' Display the dialog - extract the results.'''
         from collections import OrderedDict
         self.tk.mainloop()
         try:
-            results = OrderedDict()
             if not self._isOk:
-                return results
-
-            for ref in self._dict.keys():
-                results[ref] = (self._dict[ref]).get()
-            return results
+                return dict()
+            self._data['__conv_ok'] = True # New!
+            for tag in self._dict.keys():
+                value = (self._dict[tag]).get()
+                if not self._convert(self._data, tag, value):
+                    self._data['__conv_ok']  = False
+                    self._data[tag] = value    # gigo
+            return dict(self._data)
         finally:
             try:
                 self.tk.destroy()
                 # self.tk = None
             except:
                 pass
 
@@ -155,15 +191,15 @@
     cmd_name = sys.argv[0]
     if cmd_name.find('\\'):
         cmd_name = cmd_name.split('\\')[-1]
     if cmd_name.find('/'):
         cmd_name = cmd_name.split('/')[-1]
     
     sz = len(sys.argv)
-    params = {"NAME":'R.A. Geekbo', "PHONE":'123-456-7890', "EMAIL":'a.Geekbo@zbobo.com'}
+    params = {"NAME":'R.A. Geekbo', "ACCOUNT":1234567890, "EMAIL":'a.Geekbo@zbobo.com'}
     if sz > 2:
         print("Input: One stringified dictionary as a parameter, please.")
         print(f"Example: \"{str(params)}\"")
         print("\t(i.e: surrounding quotations are os-required)")
         quit()
     elif sz == 2:
         data = sys.argv[1:][0]
```

### Comparing `Prompter9000-2.0.1/Prompter9000.egg-info/PKG-INFO` & `prompter9000-2.0.2/Prompter9000.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: Prompter9000
-Version: 2.0.1
+Version: 2.0.2
 Summary: C.L.I <-> G.U.I Dictionary Editor
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/Blog9000
 Project-URL: Bug Tracker, https://github.com/soft9000/Blog9000/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Prompter9000
-Quick &amp; easy way to edit dictionaries and create counters. Console & programmatic usages are supported.
+Quick &amp; easy way to edit dictionaries and create counters. Console & programmatic 
+usages are supported.
+
+**NEW:** *Verson 2.0.2*
+1. Data types can now be preserved. 
+2. Boolean detection, as well.
+3. Result Key [__conv_ok]
+    - == *True* iff types preserved. 
+    - *False* == at least one defaulted to string.
+4.) Result Key [__btn_ok]
+    - == *True* when [Okay] was pressed
+    - else *False*.
 
 ### Programatic
 Edit a dictionary:
 ```
 from Prompter9000.PyEdit import *
-params = {"NAME":'My', "PHONE":'123-456', "EMAIL":'a.Geekbo@zbobo.com'}
+params = {"NAME":'My', "ACCOUNT":123456, "Subscriber":False}
 EditDict.edit(params)
 ```
 
 Create a click-counter:
 ```
 from Prompter9000.PyCount import *
 params = {'Hits': '0', 'Miss': '0', 'Other': '10'}
```

