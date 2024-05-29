# Comparing `tmp/autocall-1.0.0.tar.gz` & `tmp/autocall-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocall-1.0.0.tar", last modified: Fri Mar 29 08:45:59 2024, max compression
+gzip compressed data, was "autocall-1.1.0.tar", last modified: Tue May 28 15:10:43 2024, max compression
```

## Comparing `autocall-1.0.0.tar` & `autocall-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-03-29 08:45:59.914511 autocall-1.0.0/
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     1081 2024-03-28 08:20:07.000000 autocall-1.0.0/LICENSE.txt
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     4028 2024-03-29 08:45:59.914511 autocall-1.0.0/PKG-INFO
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     1580 2024-03-28 09:05:02.000000 autocall-1.0.0/README.md
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     6569 2024-03-29 08:36:37.000000 autocall-1.0.0/pyproject.toml
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)       38 2024-03-29 08:45:59.914511 autocall-1.0.0/setup.cfg
-drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-03-29 08:45:59.914511 autocall-1.0.0/src/
-drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-03-29 08:45:59.914511 autocall-1.0.0/src/autocall/
--rwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)      159 2024-03-28 08:41:56.000000 autocall-1.0.0/src/autocall/__init__.py
--rwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)     2839 2024-03-28 08:41:56.000000 autocall-1.0.0/src/autocall/parser.py
-drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-03-29 08:45:59.914511 autocall-1.0.0/src/autocall.egg-info/
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     4028 2024-03-29 08:45:59.000000 autocall-1.0.0/src/autocall.egg-info/PKG-INFO
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)      263 2024-03-29 08:45:59.000000 autocall-1.0.0/src/autocall.egg-info/SOURCES.txt
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)        1 2024-03-29 08:45:59.000000 autocall-1.0.0/src/autocall.egg-info/dependency_links.txt
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)       39 2024-03-29 08:45:59.000000 autocall-1.0.0/src/autocall.egg-info/requires.txt
--rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)        9 2024-03-29 08:45:59.000000 autocall-1.0.0/src/autocall.egg-info/top_level.txt
+drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-05-28 15:10:43.602912 autocall-1.1.0/
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     1081 2024-05-28 13:34:08.000000 autocall-1.1.0/LICENSE.txt
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     4415 2024-05-28 15:10:43.602912 autocall-1.1.0/PKG-INFO
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     1967 2024-05-28 14:59:38.000000 autocall-1.1.0/README.md
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     6569 2024-05-28 15:09:58.000000 autocall-1.1.0/pyproject.toml
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)       38 2024-05-28 15:10:43.602912 autocall-1.1.0/setup.cfg
+drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-05-28 15:10:43.602912 autocall-1.1.0/src/
+drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-05-28 15:10:43.602912 autocall-1.1.0/src/autocall/
+-rwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)      240 2024-05-28 14:20:33.000000 autocall-1.1.0/src/autocall/__init__.py
+-rwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)     4032 2024-05-28 14:58:05.000000 autocall-1.1.0/src/autocall/parser.py
+drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-05-28 15:10:43.602912 autocall-1.1.0/src/autocall.egg-info/
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)     4415 2024-05-28 15:10:43.000000 autocall-1.1.0/src/autocall.egg-info/PKG-INFO
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)      277 2024-05-28 15:10:43.000000 autocall-1.1.0/src/autocall.egg-info/SOURCES.txt
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)        1 2024-05-28 15:10:43.000000 autocall-1.1.0/src/autocall.egg-info/dependency_links.txt
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)       39 2024-05-28 15:10:43.000000 autocall-1.1.0/src/autocall.egg-info/requires.txt
+-rw-r--r--   0 yjl00405  (1000) yjl00405  (1000)        9 2024-05-28 15:10:43.000000 autocall-1.1.0/src/autocall.egg-info/top_level.txt
+drwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)        0 2024-05-28 15:10:43.602912 autocall-1.1.0/tests/
+-rwxr-xr-x   0 yjl00405  (1000) yjl00405  (1000)      655 2024-05-28 14:51:01.000000 autocall-1.1.0/tests/test.py
```

### Comparing `autocall-1.0.0/LICENSE.txt` & `autocall-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autocall-1.0.0/PKG-INFO` & `autocall-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocall
-Version: 1.0.0
+Version: 1.1.0
 Summary: Call function directly in command line and a well help tips generately automatically
 Author-email: bajeer <z_bajer@yeah.net>
 Maintainer-email: bajeer <z_bajer@yeah.net>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -48,74 +48,79 @@
 Requires-Dist: coverage; extra == "test"
 
 # Call function directly in cmd line
 
 #### Features
 1. Allow user call functions directly in command line.
 2. Generate help tips automatically.
+3. Add default called functions if not function was specific.
+
+#### Notice
+1. It's better to add argument type for each autocall functions.
+2. str type argument must be defined explicitly.
+3. @cmdline_default is a subset of @cmdline, which means function with @cmdline_default will have @cmdline implicitly.
+4. Arguments of function with @cmdline_default should be optional or no argument.
+
+#### TODO
+1. Support class's function with self as the first argument.
 
 #### Code example
 ``` python
-#!/bin/bash
+#!/bin/python3.8
 from autocall import *
 
 # The tar @cmdline is used to register the function.
 @cmdline
 def test1():
-	pass
-    
+    print(f'test1()')
+    pass
+
 @cmdline
-def test2(arg):
-	pass
-    
+@cmdline_default
+def test2(arg: int = 0):
+    print(f'test2({arg})')
+    pass
+
 @cmdline
 def test3(arg1, arg2: str = 'this is a string'):
-	print(arg2)
+    print(f'test3({arg1}, {arg2})')
     
 @cmdline
 def test4(arg1, arg2: int):
-	'You can add some extra information here.'
-	pass
-    
+    'You can add some extra information here.'
+    print(f'test4({arg1}, {arg2})')
+    pass
+
+@cmdline_default
+def test5(arg1: int = 1, arg2: str = 'good'):
+    print(f'test5({arg1}, {arg2})')
+
 # main function
 parse_and_run()
 ```
 #### Run the code
 ``` bash
-$ ./main.py --help
-Help Tips Provided by Autocall.
-  option:
-    --test1
-    
-    --test2     arg
-    
-    --test3     arg1  [arg2 = this is a string]
-    
-    --test4     arg1  arg2
-	            You can add some extra information here.
-    
-    --help      [verbose = notverbose]
-    		    Give the argument "verbose" instead of "notverbose" to print detail information.
-    
-$ ./main.py --help verbose
+~/autocall/src $ ./test.py --help
 Help Tips Provided by Autocall.
   option:
-    --test1
-    
-    --test2     arg
-    
-    --test3     arg1  [arg2(str) = this is a string]
-    
-    --test4     arg1  arg2(int)
-	            You can add some extra information here.
-    
-    --help      [verbose(str) = notverbose]
-    		    Give the argument "verbose" instead of "notverbose" to print detail information.
+    --test1     
+
+    --test2     [arg = 0]  
+                The function will be called directly if not specific.
+
+    --test3     arg1  [arg2 = this is a string]  
+
+    --test4     arg1  arg2  
+                You can add some extra information here.
+
+    --test5     [arg1 = 1]  [arg2 = good]  
+                The function will be called directly if not specific.
+
+    --help      [verbose = notverbose]  
+                Give the argument "verbose" instead of "notverbose" to print detail information.
 
-$ # call function test3 and pass arguments arg1=1
-$ ./main.py --test3 1
-this is a string
-
-$ # call function test3 and pass arguments arg1=1, arg2="this will be showed."     
-$ ./main.py --test3 1 "this will be showed."
-this will be showed.
+~/autocall/src $ ./test.py --test5 10 'hello'
+test5(10, hello)
+~/autocall/src $ ./test.py
+test2(0)
+test5(1, good)
 ```
```

### Comparing `autocall-1.0.0/pyproject.toml` & `autocall-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 name = "autocall"  # REQUIRED, is the only field that cannot be marked as dynamic.
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.0"  # REQUIRED, although can be dynamic
+version = "1.1.0"  # REQUIRED, although can be dynamic
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Call function directly in command line and a well help tips generately automatically"
 
 # This is an optional longer description of your project that represents
```

### Comparing `autocall-1.0.0/src/autocall/parser.py` & `autocall-1.1.0/src/autocall/parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,38 @@
 #!/bin/python3
 import inspect
 import sys
 
+# functions taged by @cmdline
 __register_funcs = []
+__register_funcs_default = []
+
+def colorize(text, color):
+    return f"\033[{color}m{text}\033[0m"
+
+def cmdline_default(func):
+    funcname = func.__name__
+    parameters = inspect.getfullargspec(func)
+
+    if len(parameters.args) != 0 and len(parameters.args) != len(parameters.defaults):
+            print(colorize(f'[Autocall Warning]: arguments of function \'{funcname}\' should be optional.', 34))
+            return func
+    
+    __register_funcs_default.append(func)
+
+    if func not in __register_funcs:
+        __register_funcs.append(func)
+    
+    globals()[funcname] = func
+    return func
 
 def cmdline(func):
+    if func in __register_funcs:
+        return func
+    
     __register_funcs.append(func)
     globals()[func.__name__] = func
     return func
 
 def parse_run(argv = sys.argv[1:]):
     __argv = []
 
@@ -18,28 +42,30 @@
         elif _type == str:
             return _str
         else:
             raise Exception("Don't know the type")
 
     def match_and_check(name):
         res = [f for f in __register_funcs if f.__name__ == name]
+        res += [f for f in __register_funcs_default if f.__name__ == name]
         if not res:
             raise Exception("Couldn't found function")
 
         #if len(getfullargspec(res[0]).args) != len(res[0].__annotations__):
             #raise Exception("Target function's arguments should have determinded types")
 
         return res[0]
 
-    
+    # register this function into __register_funcs list
     @cmdline
     def help(verbose :str = 'notverbose'):
         'Give the argument \"verbose\" instead of \"notverbose\" to print detail information.'
         print('Help Tips Provided by Autocall.')
         print('  option:')
+
         for func in __register_funcs:
             parameters = inspect.signature(func).parameters
             print(f'    --{func.__name__:<10s}', end='')
             for name in parameters:
                 anno = parameters[name].annotation
                 defa = parameters[name].default
 
@@ -60,37 +86,42 @@
                     defa = f'{name}{anno}'
                 
                 print(f'{defa}  ', end='')
                 
             print()
             if func.__doc__:
                 print(f'                {func.__doc__:>20s}')
+            if func in __register_funcs_default:
+                print(f'                The function will be called directly if not specific.')
             print()
 
     
     # Parsing
     for arg in argv:
         if arg.startswith('--'):
             __argv.append([arg[2:]])
         elif arg.startswith('-'):
             __argv.append([arg[2:]])
         else:
             if not len(__argv):
                 continue
+            # -1 indicate one existed function name. arg will be appended after the function name into a new string.
             __argv[-1].append(arg)
-    
+
     # Call function
+    if not len(__argv):
+        __argv = [[funcname.__name__] for funcname in __register_funcs_default]
+    #print(__argv)
+    
     for item in __argv:
         name = item[0]
         func = match_and_check(name)
         args = inspect.getfullargspec(func).args
         anns = func.__annotations__
 
         arguments = ', '.join([(lambda argname, passvalue:
                           passvalue if anns.get(argname) != str
                           else f'\'{passvalue}\'')(k, v)
                          for k, v in zip(args, item[1:])])
 
         #print(globals())
         eval(f'{name}({arguments})')
-
-
```

### Comparing `autocall-1.0.0/src/autocall.egg-info/PKG-INFO` & `autocall-1.1.0/src/autocall.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocall
-Version: 1.0.0
+Version: 1.1.0
 Summary: Call function directly in command line and a well help tips generately automatically
 Author-email: bajeer <z_bajer@yeah.net>
 Maintainer-email: bajeer <z_bajer@yeah.net>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -48,74 +48,79 @@
 Requires-Dist: coverage; extra == "test"
 
 # Call function directly in cmd line
 
 #### Features
 1. Allow user call functions directly in command line.
 2. Generate help tips automatically.
+3. Add default called functions if not function was specific.
+
+#### Notice
+1. It's better to add argument type for each autocall functions.
+2. str type argument must be defined explicitly.
+3. @cmdline_default is a subset of @cmdline, which means function with @cmdline_default will have @cmdline implicitly.
+4. Arguments of function with @cmdline_default should be optional or no argument.
+
+#### TODO
+1. Support class's function with self as the first argument.
 
 #### Code example
 ``` python
-#!/bin/bash
+#!/bin/python3.8
 from autocall import *
 
 # The tar @cmdline is used to register the function.
 @cmdline
 def test1():
-	pass
-    
+    print(f'test1()')
+    pass
+
 @cmdline
-def test2(arg):
-	pass
-    
+@cmdline_default
+def test2(arg: int = 0):
+    print(f'test2({arg})')
+    pass
+
 @cmdline
 def test3(arg1, arg2: str = 'this is a string'):
-	print(arg2)
+    print(f'test3({arg1}, {arg2})')
     
 @cmdline
 def test4(arg1, arg2: int):
-	'You can add some extra information here.'
-	pass
-    
+    'You can add some extra information here.'
+    print(f'test4({arg1}, {arg2})')
+    pass
+
+@cmdline_default
+def test5(arg1: int = 1, arg2: str = 'good'):
+    print(f'test5({arg1}, {arg2})')
+
 # main function
 parse_and_run()
 ```
 #### Run the code
 ``` bash
-$ ./main.py --help
-Help Tips Provided by Autocall.
-  option:
-    --test1
-    
-    --test2     arg
-    
-    --test3     arg1  [arg2 = this is a string]
-    
-    --test4     arg1  arg2
-	            You can add some extra information here.
-    
-    --help      [verbose = notverbose]
-    		    Give the argument "verbose" instead of "notverbose" to print detail information.
-    
-$ ./main.py --help verbose
+~/autocall/src $ ./test.py --help
 Help Tips Provided by Autocall.
   option:
-    --test1
-    
-    --test2     arg
-    
-    --test3     arg1  [arg2(str) = this is a string]
-    
-    --test4     arg1  arg2(int)
-	            You can add some extra information here.
-    
-    --help      [verbose(str) = notverbose]
-    		    Give the argument "verbose" instead of "notverbose" to print detail information.
+    --test1     
+
+    --test2     [arg = 0]  
+                The function will be called directly if not specific.
+
+    --test3     arg1  [arg2 = this is a string]  
+
+    --test4     arg1  arg2  
+                You can add some extra information here.
+
+    --test5     [arg1 = 1]  [arg2 = good]  
+                The function will be called directly if not specific.
+
+    --help      [verbose = notverbose]  
+                Give the argument "verbose" instead of "notverbose" to print detail information.
 
-$ # call function test3 and pass arguments arg1=1
-$ ./main.py --test3 1
-this is a string
-
-$ # call function test3 and pass arguments arg1=1, arg2="this will be showed."     
-$ ./main.py --test3 1 "this will be showed."
-this will be showed.
+~/autocall/src $ ./test.py --test5 10 'hello'
+test5(10, hello)
+~/autocall/src $ ./test.py
+test2(0)
+test5(1, good)
 ```
```

