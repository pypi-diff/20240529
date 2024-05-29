# Comparing `tmp/splashlab-0.0.9.tar.gz` & `tmp/splashlab-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splashlab-0.0.9.tar", last modified: Thu Feb 23 06:22:45 2023, max compression
+gzip compressed data, was "splashlab-0.1.0.tar", last modified: Wed May 29 13:03:16 2024, max compression
```

## Comparing `splashlab-0.0.9.tar` & `splashlab-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.491730 splashlab-0.0.9/
--rw-rw-rw-   0        0        0     1087 2023-02-12 17:06:38.000000 splashlab-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      833 2023-02-23 06:22:45.491730 splashlab-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-02-12 16:23:56.000000 splashlab-0.0.9/README.md
--rw-rw-rw-   0        0        0       86 2023-02-23 06:22:45.492853 splashlab-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1927 2023-02-23 06:22:01.000000 splashlab-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.395456 splashlab-0.0.9/splashlab/
--rw-rw-rw-   0        0        0        0 2023-02-12 18:31:45.000000 splashlab-0.0.9/splashlab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.413474 splashlab-0.0.9/splashlab/computer_vision/
--rw-rw-rw-   0        0        0        0 2023-02-23 05:59:44.000000 splashlab-0.0.9/splashlab/computer_vision/__init__.py
--rw-rw-rw-   0        0        0     6819 2023-02-20 18:20:05.000000 splashlab-0.0.9/splashlab/computer_vision/image_util.py
-drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.475057 splashlab-0.0.9/splashlab/dimensional_analysis/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:34:04.000000 splashlab-0.0.9/splashlab/dimensional_analysis/__init__.py
--rw-rw-rw-   0        0        0     2238 2023-02-09 10:04:02.000000 splashlab-0.0.9/splashlab/dimensional_analysis/convert.py
--rw-rw-rw-   0        0        0     1954 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/data_reader.py
--rw-rw-rw-   0        0        0     2155 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/fluid_types.py
--rw-rw-rw-   0        0        0     1369 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/group_of_parameter.py
--rw-rw-rw-   0        0        0     3597 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/parameter.py
--rw-rw-rw-   0        0        0     7699 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/unit.py
--rw-rw-rw-   0        0        0      897 2023-02-09 10:04:02.000000 splashlab-0.0.9/splashlab/dimensional_analysis/util.py
-drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.413474 splashlab-0.0.9/splashlab.egg-info/
--rw-rw-rw-   0        0        0      833 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      652 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:03:16.896029 splashlab-0.1.0/
+-rw-rw-rw-   0        0        0     1087 2023-02-12 17:06:38.000000 splashlab-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2247 2024-05-29 13:03:16.896029 splashlab-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1396 2023-10-05 10:56:52.000000 splashlab-0.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-29 13:03:16.901044 splashlab-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1894 2024-05-29 13:02:27.000000 splashlab-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:03:16.869029 splashlab-0.1.0/splashlab/
+-rw-rw-rw-   0        0        0      398 2024-03-18 14:01:09.000000 splashlab-0.1.0/splashlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:03:16.884030 splashlab-0.1.0/splashlab/computer_vision/
+-rw-rw-rw-   0        0        0       52 2023-02-23 08:36:04.000000 splashlab-0.1.0/splashlab/computer_vision/__init__.py
+-rw-rw-rw-   0        0        0    25911 2024-05-29 12:58:03.000000 splashlab-0.1.0/splashlab/computer_vision/image_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:03:16.885033 splashlab-0.1.0/splashlab/data_management/
+-rw-rw-rw-   0        0        0     4413 2024-05-29 13:01:04.000000 splashlab-0.1.0/splashlab/data_management/experiment.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:03:16.894029 splashlab-0.1.0/splashlab/dimensional_analysis/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:34:04.000000 splashlab-0.1.0/splashlab/dimensional_analysis/__init__.py
+-rw-rw-rw-   0        0        0     2281 2023-04-15 13:58:21.000000 splashlab-0.1.0/splashlab/dimensional_analysis/convert.py
+-rw-rw-rw-   0        0        0     1954 2023-02-23 07:46:40.000000 splashlab-0.1.0/splashlab/dimensional_analysis/data_reader.py
+-rw-rw-rw-   0        0        0     1453 2023-03-08 11:06:42.000000 splashlab-0.1.0/splashlab/dimensional_analysis/group_of_parameter.py
+-rw-rw-rw-   0        0        0     3601 2023-02-23 08:45:34.000000 splashlab-0.1.0/splashlab/dimensional_analysis/parameter.py
+-rw-rw-rw-   0        0        0     7717 2023-04-04 13:45:14.000000 splashlab-0.1.0/splashlab/dimensional_analysis/unit.py
+-rw-rw-rw-   0        0        0     8087 2023-07-06 13:44:43.000000 splashlab-0.1.0/splashlab/dimensional_analysis/unit_dataframe.py
+-rw-rw-rw-   0        0        0     3214 2023-07-11 10:02:03.000000 splashlab-0.1.0/splashlab/dimensional_analysis/util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:03:16.895029 splashlab-0.1.0/splashlab.egg-info/
+-rw-rw-rw-   0        0        0     2247 2024-05-29 13:03:16.000000 splashlab-0.1.0/splashlab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2024-05-29 13:03:16.000000 splashlab-0.1.0/splashlab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:03:16.000000 splashlab-0.1.0/splashlab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-29 13:03:16.000000 splashlab-0.1.0/splashlab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 13:03:16.000000 splashlab-0.1.0/splashlab.egg-info/top_level.txt
```

### Comparing `splashlab-0.0.9/LICENSE` & `splashlab-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.9/setup.py` & `splashlab-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
   name = 'splashlab',         # How you named your package folder (MyLib)
   long_description = long_description,
   long_description_content_type = 'text/markdown',
-  packages = ['splashlab', 'splashlab.dimensional_analysis', 'splashlab.computer_vision'],   # Chose the same as "name"
-  version = 'v0.0.9',      # Start with a small number and increase it with every change you make
+  packages = ['splashlab', 'splashlab.dimensional_analysis', 'splashlab.data_management', 'splashlab.computer_vision'],   # Chose the same as "name"
+  version = 'v0.1.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A package for fluid mechanic experimentalists',   # Give a short description about your library
   author = 'Spencer Truman',                   # Type in your name
   author_email = 'trumans24@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/FluidsLab/SplashLab',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/FluidsLab/SplashLab/archive/refs/tags/v0.0.8.tar.gz',    # I explain this later on
   keywords = ['Fluid Dynamics', 'Experiment'],   # Keywords that define your package best
-  install_requires=[            # I get to this in a second
-          'numpy',
-          'pandas',
-          'sympy',
-          'matplotlib',
-          'opencv-python'
-      ],
+  install_requires=[
+      'numpy',
+      'pandas',
+      'sympy',
+      'matplotlib',
+      'opencv-python'
+  ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
-    'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
+    'Programming Language :: Python :: 3',      # Specify which python versions that you want to support
     'Programming Language :: Python :: 3.8',
   ],
 )
```

### Comparing `splashlab-0.0.9/splashlab/dimensional_analysis/convert.py` & `splashlab-0.1.0/splashlab/dimensional_analysis/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import numpy as np
 
 
 class Convert:
     def __init__(self):
-        # common constants
-        self.g = 9.81  # on earth
-        self.sg = 1000  # specific gravity
-
         # Length
         self.m = 1
         self.km = 1000 * self.m
         self.cm = 1 / 100 * self.m
         self.mm = 1 / 1000 * self.m
         self.inch = 2.54 * self.cm
         self.ft = 12 * self.inch
@@ -23,28 +19,32 @@
         self.hr = 60 * self.min
         self.day = 24 * self.hr
         self.week = 7 * self.day
         self.year = 365 * self.day
 
         # Mass
         self.kg = 1
+        self.kilogram = self.kg
+        self.g = 1 / 1000 * self.kg
         self.gram = 1 / 1000 * self.kg
         self.lbm = 1 / 2.2046 * self.kg
         self.slug = 14.594 * self.kg
 
         # Angle
         self.rad = 1
         self.deg = 3.141592653589793238462643383279/180 * self.rad
+        self.rev = 360 * self.deg
 
         # Force
         self.N = self.kg * self.m / self.s ** 2
         self.lbs = 4.448 * self.N
 
         # Energy
         self.J = self.N * self.m
+        self.kJ = 1000 * self.J
 
         # Pressure
         self.Pa = 1
         self.psi = 6.895e3 * self.Pa
 
         self.prefix = {
             'peta':  10 ** 15,
@@ -71,18 +71,18 @@
         return {name: 1 for name in dir(self) if '__' not in name}
 
 
 class ConvertTemperature:
     def __init__(self, temp):
         
         # Temperature
-        self.K = 1
+        self.K = 1 * temp
         self.C = (temp + 273.15) / temp
         self.F = ((temp - 32) * 5 / 9 + 273.15) / temp
-        self.Rankine = 0.556
+        self.Rankine = 0.556 * temp
 
 
 
 if __name__ == "__main__":
     c = Convert()
     print(c.get_conversion_factor())
     print(getattr(c, 'mm'))
```

### Comparing `splashlab-0.0.9/splashlab/dimensional_analysis/data_reader.py` & `splashlab-0.1.0/splashlab/dimensional_analysis/data_reader.py`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.9/splashlab/dimensional_analysis/group_of_parameter.py` & `splashlab-0.1.0/splashlab/dimensional_analysis/group_of_parameter.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     def __iter__(self):
         for elem in self.parameters:
             yield elem
 
     def __sub__(self, other):
         new = []
         for parameter_name in self:
-            if self[parameter_name] not in other:
+            if parameter_name not in other:
                 new.append(self[parameter_name])
         return GroupOfParameters(new)
 
     def __add__(self, other):
+        if isinstance(other, Parameter):
+            other = GroupOfParameters([other])
         new = [self[parameter] for parameter in self]
         for parameter in other:
             new.append(other[parameter])
         return GroupOfParameters(new)
 
     def _define_dimensional_matrix(self) -> sp.Matrix:
         m = []
```

### Comparing `splashlab-0.0.9/splashlab/dimensional_analysis/parameter.py` & `splashlab-0.1.0/splashlab/dimensional_analysis/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             if formula[param]:
                 name += f'({param.name}^{formula[param]})'  # if formula[param] != 1 else f'({param.name})'
                 units *= param.units ** formula[param]
                 values *= param.values ** formula[param]
                 new_formula |= {param: formula[param]}
         return Parameter(name=name, units=units, values=values, formula=new_formula)
     #
-    def __repr__(self) -> str:
-        return 'Parameter: ' + self.name
+    # def __repr__(self) -> str:
+    #     return 'Parameter: ' + self.name
 
     def __eq__(self, other) -> bool:
         # if self.name == other.name and (self.units != other.units or not (self.values == other.values).all()):
         #     raise Warning('Multiple parameters with the same name.')
         return self.name == other.name
 
     def __hash__(self) -> int:
```

### Comparing `splashlab-0.0.9/splashlab/dimensional_analysis/unit.py` & `splashlab-0.1.0/splashlab/dimensional_analysis/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 
 import warnings
 
-from util import Util
+from splashlab.dimensional_analysis.util import Util
 from splashlab.dimensional_analysis.convert import Convert
 
 
 class Unit:
     def __init__(self, value: float, display_units={2: 'Time', 3: 'Length', 5: 'Mass', 7: 'Temperature'}) -> None:
         self.value = value
         self.display_units = display_units
         self.factorization = Util.factorize(self.value)
         self.dimensions = {self.display_units[key]: self.factorization[0].count(key) - self.factorization[1].count(key)
                            for key in self.display_units}
 
     def __repr__(self) -> str:
         text = ''
         for key in self.dimensions:
-            # print(key, ': ', self.dimensions[key])
             if self.dimensions[key] != 0:
                 text += f'{key}^{self.dimensions[key]}*' if self.dimensions[key] != 1 else f'{key}*'
         return text.strip('*') if self.value != 1 else 'Nondimensional'
 
     def __eq__(self, other) -> bool:
         return self.value == other.value
 
@@ -225,7 +224,9 @@
 
 
 if __name__ == "__main__":
     print(Unit(2), Units.g * Units.volume / Units.voltage)
 
     text_unit = 'mm'
     print('eqn', unit_parser(text_unit, SIUnits))
+
+    print(unit_parser('m^2/m*s*psi'))
```

### Comparing `splashlab-0.0.9/splashlab.egg-info/SOURCES.txt` & `splashlab-0.1.0/splashlab.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 splashlab.egg-info/PKG-INFO
 splashlab.egg-info/SOURCES.txt
 splashlab.egg-info/dependency_links.txt
 splashlab.egg-info/requires.txt
 splashlab.egg-info/top_level.txt
 splashlab/computer_vision/__init__.py
 splashlab/computer_vision/image_util.py
+splashlab/data_management/experiment.py
 splashlab/dimensional_analysis/__init__.py
 splashlab/dimensional_analysis/convert.py
 splashlab/dimensional_analysis/data_reader.py
-splashlab/dimensional_analysis/fluid_types.py
 splashlab/dimensional_analysis/group_of_parameter.py
 splashlab/dimensional_analysis/parameter.py
 splashlab/dimensional_analysis/unit.py
+splashlab/dimensional_analysis/unit_dataframe.py
 splashlab/dimensional_analysis/util.py
```

