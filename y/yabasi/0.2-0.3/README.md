# Comparing `tmp/yabasi-0.2.tar.gz` & `tmp/yabasi-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yabasi-0.2.tar", last modified: Thu Apr  4 16:59:00 2024, max compression
+gzip compressed data, was "yabasi-0.3.tar", last modified: Wed May 29 11:43:15 2024, max compression
```

## Comparing `yabasi-0.2.tar` & `yabasi-0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-04 16:59:00.154663 yabasi-0.2/
--rw-r--r--   0 ralf      (1000) priv      (1011)     1357 2024-04-02 10:17:11.000000 yabasi-0.2/LICENSE
--rw-r--r--   0 ralf      (1000) priv      (1011)     2286 2024-04-04 16:59:00.150663 yabasi-0.2/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     1327 2024-04-04 16:49:42.000000 yabasi-0.2/README.rst
--rw-r--r--   0 ralf      (1000) priv      (1011)        4 2024-04-04 16:58:57.000000 yabasi-0.2/VERSION
--rw-r--r--   0 ralf      (1000) priv      (1011)     2554 2024-04-04 16:57:11.000000 yabasi-0.2/pyproject.toml
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2024-04-04 16:59:00.154663 yabasi-0.2/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2928 2024-04-04 16:57:02.000000 yabasi-0.2/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-04 16:59:00.126664 yabasi-0.2/yabasi/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2024-04-04 16:58:57.000000 yabasi-0.2/yabasi/Version.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    32979 2024-04-02 10:07:35.000000 yabasi-0.2/yabasi/bas.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     3349 2024-03-31 14:44:12.000000 yabasi-0.2/yabasi/tokenizer.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-04 16:59:00.146664 yabasi-0.2/yabasi.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)     2286 2024-04-04 16:58:59.000000 yabasi-0.2/yabasi.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      284 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       43 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       10 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        7 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/top_level.txt
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-05-29 11:43:15.921682 yabasi-0.3/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1357 2024-04-02 10:17:11.000000 yabasi-0.3/LICENSE
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2765 2024-05-29 11:43:15.921682 yabasi-0.3/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1806 2024-05-29 11:40:27.000000 yabasi-0.3/README.rst
+-rw-r--r--   0 ralf      (1000) priv      (1011)        4 2024-05-29 11:43:12.000000 yabasi-0.3/VERSION
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2554 2024-04-04 16:57:11.000000 yabasi-0.3/pyproject.toml
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2024-05-29 11:43:15.925682 yabasi-0.3/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2928 2024-04-04 16:57:02.000000 yabasi-0.3/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-05-29 11:43:15.897682 yabasi-0.3/yabasi/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2024-05-29 11:43:12.000000 yabasi-0.3/yabasi/Version.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    32364 2024-05-29 11:22:37.000000 yabasi-0.3/yabasi/bas.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)    48928 2024-05-29 11:17:53.000000 yabasi-0.3/yabasi/parsetab.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     3349 2024-03-31 14:44:12.000000 yabasi-0.3/yabasi/tokenizer.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-05-29 11:43:15.917682 yabasi-0.3/yabasi.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2765 2024-05-29 11:43:15.000000 yabasi-0.3/yabasi.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      303 2024-05-29 11:43:15.000000 yabasi-0.3/yabasi.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2024-05-29 11:43:15.000000 yabasi-0.3/yabasi.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       43 2024-05-29 11:43:15.000000 yabasi-0.3/yabasi.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       10 2024-05-29 11:43:15.000000 yabasi-0.3/yabasi.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        7 2024-05-29 11:43:15.000000 yabasi-0.3/yabasi.egg-info/top_level.txt
```

### Comparing `yabasi-0.2/LICENSE` & `yabasi-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yabasi-0.2/pyproject.toml` & `yabasi-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yabasi-0.2/setup.py` & `yabasi-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `yabasi-0.2/yabasi/bas.py` & `yabasi-0.3/yabasi/bas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1041,75 +1041,43 @@
 
     def p_printlist (self, p):
         """
             printlist : empty
                       | expression
                       | printlist SEMIC expression
                       | printlist COMMA expression
+                      | printlist expression
                       | printlist SEMIC
                       | printlist COMMA
         """
         p1 = p [1]
         if len (p) == 2:
             def x ():
                 if p1 is None:
                     return []
                 return [p1]
         elif len (p) == 3:
-            p2 = self.print_special [p [2]][0]
-            def x ():
-                return p1 () + [p2]
+            if p [2] == ';' or p [2] == ',':
+                p2 = self.print_special [p [2]][0]
+                def x ():
+                    return p1 () + [p2]
+            else:
+                # Two expressions are equivalent to a left-out semicolon
+                px = self.print_special [';'][0]
+                p2 = p [2]
+                def x ():
+                    return p1 () + [px, p2]
         else:
             p2 = self.print_special [p [2]][0]
             p3 = p [3]
             def x ():
                 return p1 () + [p2, p3]
         p [0] = x
     # end def p_printlist
 
-    def p_printlist_ex_str (self, p):
-        """
-            printlist : printlist expression STRING
-        """
-        p1 = p [1]
-        p2 = p [2]
-        p3 = p [3]
-        def x ():
-            return p1 () + [p2, p3]
-        p [0] = x
-    # end def p_printlist_ex_str
-
-    def p_printlist_str_ex (self, p):
-        """
-            printlist : printlist STRING expression
-                      | STRING expression
-        """
-        p1 = p [1]
-        p2 = p [2]
-        if len (p) == 3:
-            def x ():
-                return [p1, p2]
-        else:
-            p3 = p [3]
-            def x ():
-                return p1 () + [p2, p3]
-        p [0] = x
-    # end def p_printlist_str_ex
-
-    def p_printlist_var (self, p):
-        """
-            printlist : printlist VAR
-        """
-        p1 = p [1]
-        p2 = p [2]
-        def x ():
-            return p1 () + [self._var_helper (p2)]
-        p [0] = x
-    # end def p_printlist_var
-
     def p_read_statement (self, p):
         """
             read-statement : READ varlist-complex
         """
         p [0] = (p [1], p [2])
     # end def p_read_statement
```

### Comparing `yabasi-0.2/yabasi/tokenizer.py` & `yabasi-0.3/yabasi/tokenizer.py`

 * *Files identical despite different names*

