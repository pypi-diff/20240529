# Comparing `tmp/prompter9000-2.0.2.tar.gz` & `tmp/prompter9000-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompter9000-2.0.2.tar", last modified: Wed May 29 16:52:45 2024, max compression
+gzip compressed data, was "prompter9000-2.5.0.tar", last modified: Wed May 29 17:36:12 2024, max compression
```

## Comparing `prompter9000-2.0.2.tar` & `prompter9000-2.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 16:52:45.032479 prompter9000-2.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-18 19:48:50.000000 prompter9000-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     1998 2024-05-29 16:52:45.030526 prompter9000-2.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-29 16:52:45.001213 prompter9000-2.0.2/Prompter9000/
--rw-rw-rw-   0        0        0     7422 2023-11-22 10:46:45.000000 prompter9000-2.0.2/Prompter9000/PyCount.py
--rw-rw-rw-   0        0        0     7809 2024-05-29 16:28:04.000000 prompter9000-2.0.2/Prompter9000/PyEdit.py
--rw-rw-rw-   0        0        0       33 2023-11-22 11:48:58.000000 prompter9000-2.0.2/Prompter9000/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:52:45.028571 prompter9000-2.0.2/Prompter9000.egg-info/
--rw-rw-rw-   0        0        0     1998 2024-05-29 16:52:44.000000 prompter9000-2.0.2/Prompter9000.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-29 16:52:44.000000 prompter9000-2.0.2/Prompter9000.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 16:52:44.000000 prompter9000-2.0.2/Prompter9000.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 16:52:44.000000 prompter9000-2.0.2/Prompter9000.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1475 2024-05-29 16:52:09.000000 prompter9000-2.0.2/README.md
--rw-rw-rw-   0        0        0      511 2024-05-29 16:11:46.000000 prompter9000-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 16:52:45.032479 prompter9000-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 17:36:12.633386 prompter9000-2.5.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-29 17:17:49.000000 prompter9000-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2006 2024-05-29 17:36:12.630454 prompter9000-2.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 17:36:12.605061 prompter9000-2.5.0/Prompter9000/
+-rw-rw-rw-   0        0        0     8766 2024-05-29 17:30:34.000000 prompter9000-2.5.0/Prompter9000/PyCount.py
+-rw-rw-rw-   0        0        0     7809 2024-05-29 16:28:04.000000 prompter9000-2.5.0/Prompter9000/PyEdit.py
+-rw-rw-rw-   0        0        0       33 2023-11-22 11:48:58.000000 prompter9000-2.5.0/Prompter9000/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:36:12.628501 prompter9000-2.5.0/Prompter9000.egg-info/
+-rw-rw-rw-   0        0        0     2006 2024-05-29 17:36:12.000000 prompter9000-2.5.0/Prompter9000.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-29 17:36:12.000000 prompter9000-2.5.0/Prompter9000.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:36:12.000000 prompter9000-2.5.0/Prompter9000.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 17:36:12.000000 prompter9000-2.5.0/Prompter9000.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1475 2024-05-29 16:52:09.000000 prompter9000-2.5.0/README.md
+-rw-rw-rw-   0        0        0      521 2024-05-29 17:35:45.000000 prompter9000-2.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:36:12.633386 prompter9000-2.5.0/setup.cfg
```

### Comparing `prompter9000-2.0.2/LICENSE` & `prompter9000-2.5.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Randall Nagy
+Copyright (c) 2024 Randall Nagy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `prompter9000-2.0.2/PKG-INFO` & `prompter9000-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Prompter9000
-Version: 2.0.2
+Version: 2.5.0
 Summary: C.L.I <-> G.U.I Dictionary Editor
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
-Project-URL: Homepage, https://github.com/soft9000/Blog9000
-Project-URL: Bug Tracker, https://github.com/soft9000/Blog9000/issues
+Project-URL: Homepage, https://github.com/soft9000/Prompter9000
+Project-URL: Bug Tracker, https://github.com/soft9000/Prompter9000/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `prompter9000-2.0.2/Prompter9000/PyCount.py` & `prompter9000-2.5.0/Prompter9000/PyCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,14 +69,48 @@
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
     def begin(fields, title="Counter",
              font_size=16, font_name='TkFixedFont',
              align='e'):
         ''' Create the frame, add the title, as well as the input fields.'''
         self = Counter(fields, font_size, font_name, align)
         self.tk = Tk()
@@ -151,21 +185,23 @@
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
```

### Comparing `prompter9000-2.0.2/Prompter9000/PyEdit.py` & `prompter9000-2.5.0/Prompter9000/PyEdit.py`

 * *Files identical despite different names*

### Comparing `prompter9000-2.0.2/Prompter9000.egg-info/PKG-INFO` & `prompter9000-2.5.0/Prompter9000.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Prompter9000
-Version: 2.0.2
+Version: 2.5.0
 Summary: C.L.I <-> G.U.I Dictionary Editor
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
-Project-URL: Homepage, https://github.com/soft9000/Blog9000
-Project-URL: Bug Tracker, https://github.com/soft9000/Blog9000/issues
+Project-URL: Homepage, https://github.com/soft9000/Prompter9000
+Project-URL: Bug Tracker, https://github.com/soft9000/Prompter9000/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `prompter9000-2.0.2/README.md` & `prompter9000-2.5.0/README.md`

 * *Files identical despite different names*

