# Comparing `tmp/jeffutils-0.6.4.tar.gz` & `tmp/jeffutils-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.6.4.tar", last modified: Fri May 24 16:00:05 2024, max compression
+gzip compressed data, was "jeffutils-0.6.5.tar", last modified: Tue May 28 19:36:52 2024, max compression
```

## Comparing `jeffutils-0.6.4.tar` & `jeffutils-0.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 16:00:05.691100 jeffutils-0.6.4/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.4/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-24 16:00:05.691100 jeffutils-0.6.4/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.6.4/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.4/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-24 16:00:05.691100 jeffutils-0.6.4/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-24 16:00:02.000000 jeffutils-0.6.4/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 16:00:05.691100 jeffutils-0.6.4/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 16:00:05.691100 jeffutils-0.6.4/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.4/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    29013 2024-05-24 15:59:42.000000 jeffutils-0.6.4/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 16:00:05.691100 jeffutils-0.6.4/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-24 16:00:05.000000 jeffutils-0.6.4/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-24 16:00:05.000000 jeffutils-0.6.4/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-24 16:00:05.000000 jeffutils-0.6.4/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-24 16:00:05.000000 jeffutils-0.6.4/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 19:36:52.470285 jeffutils-0.6.5/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.5/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-28 19:36:52.470285 jeffutils-0.6.5/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2613 2024-05-28 19:36:25.000000 jeffutils-0.6.5/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.5/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-28 19:36:52.470285 jeffutils-0.6.5/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      611 2024-05-28 19:36:48.000000 jeffutils-0.6.5/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 19:36:52.470285 jeffutils-0.6.5/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 19:36:52.470285 jeffutils-0.6.5/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.5/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    33111 2024-05-28 19:01:16.000000 jeffutils-0.6.5/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 19:36:52.470285 jeffutils-0.6.5/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-28 19:36:52.000000 jeffutils-0.6.5/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-28 19:36:52.000000 jeffutils-0.6.5/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-28 19:36:52.000000 jeffutils-0.6.5/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-28 19:36:52.000000 jeffutils-0.6.5/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.6.4/LICENSE.txt` & `jeffutils-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.4/setup.py` & `jeffutils-0.6.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.6.4',
+    version='0.6.5',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+    url="https://github.com/jeffxhansen/jeffutils",
     python_requires='>=3.6',
 )
```

### Comparing `jeffutils-0.6.4/src/jeffutils/utils.py` & `jeffutils-0.6.5/src/jeffutils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -588,32 +588,57 @@
             else:
                 pass
             
         # sleep for 1 minute, so that it only checks all of the threads
         # every minute
         time.sleep(60)
         
-def reimport(import_statement:str):
-    """ takes in any single import statement and imports/reimports the module
-    and handles associated aliases.
-    
-    Examples:
-    'import random' - imports 'random' in sys.modules
-    'import numpy as np' - imports 'numpy' in sys.modules and assigns the
-       alias 'np' in the globals() dictionary
-    'import numpy as np, pandas as pd' - imports both numpy and pandas
-       with their associated aliases
-    'from jeffutils.utils import pprint, stack_trace, log_print as lp' -
-       imports pprint, stack_trace and log_print as lp
-       
+def reimport(statements:str|list):
+    """ takes in python import code represented as a string or a list of strings, and
+    it reimports all of the modules and functions in the import statements. This allows
+    you to reimport modules that have been changed in the background without having to
+    restart the kernel.
+    
+    The input can either be:
+    - a string with a single import statement\n
+      ex: 'import numpy as np' or 'from random import choice, randint'
+    - a multiline string with multiple import statements\n
+      ex: '''import numpy as np\n
+      import pandas as pd\n
+      from random import choice, randint'''
+    - a list of strings where each string is an import statement\n
+      ex: ['import numpy as np', 'import pandas as pd', 'from random import choice, randint']
+      
+    This also handles situations where imports look like:\n
+    'from config import (
+        thing1,
+        thing2,
+        thing3
+    )'
+    
+    or that have the line continuation character \\ at the end of a line:\n
+    'from config import thing 1, \\
+        thing2, \\
+        thing3
+    '
+    
     raises:
     AttributeError: if the module or function is not found in sys.modules
+    
+    DEPENDENCY NOTE: 
+    If you make changes to two files file_1.py and file_2.py, and file_2 imports file_1, if you
+    reimport file_2, then the changes in file_1 will not be reflected in file_2. You must reimport
+    both file_1 and file_2 to see the changes in file_1 reflected in file_2.
+       
     """
+    ##########################
+    # inner helper functions #
+    ##########################
     
-    def import_one(module:str):
+    def _import_one(module:str):
         """ takes in a string like 'random' or 'numpy as np' and imports that
         module with its alias if given
         """
         if 'as' in module:
             module_name, alias = module.split(' as ')
             if module_name in sys.modules:
                 importlib.reload(sys.modules[module_name])
@@ -625,58 +650,125 @@
         else:
             if module in sys.modules:
                 importlib.reload(sys.modules[module])
                 module_obj = sys.modules[module]
             else:
                 module_obj = importlib.import_module(module)
             
-    def import_sub_func(module, func):
+    def _import_sub_fun(module, func):
         """ handles something like "from random import randint" where 'random'
         is the module and 'randint' is the function
         """
         if module not in sys.modules:
             raise AttributeError(f"Module {module} not found in sys.modules")
         module_obj = sys.modules[module]
         
         if 'as' in func:
             func_name, alias = func.split(' as ')
             if func_name in dir(module_obj):
                 globals()[alias] = getattr(module_obj, func_name)
             else:
                 raise AttributeError(f"Function {func_name} not found in module {module}")
-        
         else:
             if func in dir(module_obj):
                 globals()[func] = getattr(module_obj, func)
             else:
                 raise AttributeError(f"Function {func} not found in module {module}")
+            
+    def _process_single_import_statement(import_statement:str):
+        """ takes in a single import statement like 'import numpy as np' or 'from random import choice'
+        and imports the module or function
+        """
+        # remove whitespace at the start and end of the import statement
+        import_statement = import_statement.strip()
+        
+        # extract all of the modules names ('os', 'numpy as np', 'jeffutils.utils', 'stack_trace')
+        module_re = re.compile(r"(\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b\sas\s\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b|\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b)")
+        module_names = module_re.findall(import_statement)
+        
+        # if a vanilla import statement, import each module
+        if import_statement.startswith("import"):
+            for module_name in module_names:
+                _import_one(module_name)
+            
+        # if importing functions/sub-modules from a module
+        elif import_statement.startswith("from"):
+            
+            # import the base module
+            module = module_names[0]
+            _import_one(module)
+            
+            # import each sub-function from the module
+            for func_name in module_names[1:]:
+                _import_sub_fun(module, func_name)
+                
+    def _get_statements_from_str(statements):
+        """ takes in a statement representing python import code and returns a list of
+        all of the import statements in that code. This handles situations where the import
+        statements are split by newlines or have (...) blocks in them
+        """
+        # first strip the input string of any leading/trailing whitespace
+        statements = statements.strip()
+        
+        # if there is any () to break up an import statement, convert this to one line
+        if "(" in statements and ")" in statements:
+            
+            # extract the (...) block
+            start_paren = statements.index("(")
+            end_paren = statements.index(")")
+            sub_str = statements[start_paren:end_paren+1]
+            
+            # make the entire statement a single line
+            sub_strs = sub_str.split("\n")
+            sub_strs = [s.strip() for s in sub_strs]
+            sub_str = " ".join(sub_strs)
+            
+            # get rid of the parentheses
+            sub_str = sub_str.replace("(", " ").replace(")", " ")
+            
+            # replace the original statement with the new one and call the function again recursively
+            new_statements = statements[:start_paren] + sub_str + statements[end_paren+1:]
+            return _get_statements_from_str(new_statements)
+        
+        # if any '\' python line continuation characters are present, remove them
+        if "\\" in statements:
+            slash_remove = re.compile(r"\\\s?\n\s?")
+            statements = slash_remove.sub("", statements)
+        
+        # initialize a list of all of the statements that will be processed
+        statements_res = []
+        
+        # if there are multiple import statements split by newlines, split them up
+        if "\n" in statements:
+            statements = statements.split("\n")
+            for statement in statements:
+                statements_res.append(statement)
+        else:
+            statements_res.append(statements)
+        
+        return statements_res
     
-    # remove whitespace at the start and end of the import statement
-    import_statement = import_statement.strip()
-    
-    # extract all of the modules names ('os', 'numpy as np', 'jeffutils.utils', 'stack_trace')
-    module_re = re.compile(r"(\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b\sas\s\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b|\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b)")
-    module_names = module_re.findall(import_statement)
-    
-    # if a vanilla import statement, import each module
-    if import_statement.startswith("import"):
-        for module_name in module_names:
-            import_one(module_name)
-        
-    # if importing functions/sub-modules from a module
-    elif import_statement.startswith("from"):
-        
-        # import the base module
-        module = module_names[0]
-        import_one(module)
-        
-        # import each sub-function from the module
-        for func_name in module_names[1:]:
-            import_sub_func(module, func_name)
-    
+    ##########################
+    # main code for reimport #
+    ##########################
+    
+    if isinstance(statements, str):
+        for statement in _get_statements_from_str(statements):
+            _process_single_import_statement(statement)
+    elif isinstance(statements, list) and len(statements) > 0 and isinstance(statements[0], str):
+        for statement in statements:
+            for sttmnt in _get_statements_from_str(statement):
+                _process_single_import_statement(sttmnt)
+    else:
+        raise ValueError(
+            "Input should be a string or a list of strings, where each string is "
+            "an import statement like 'import random', 'import numpy as np', "
+            "'from jeffuitls.utils import stack_trace', etc."
+        )
+
         
 ############################################################
 #                       SQL FUNCTIONS                      #
 ############################################################
 
 def get_sql_tables_info(db_path, verbose=True):
     """
```

