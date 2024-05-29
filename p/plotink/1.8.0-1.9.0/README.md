# Comparing `tmp/plotink-1.8.0.tar.gz` & `tmp/plotink-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotink-1.8.0.tar", last modified: Sun Dec 11 19:29:14 2022, max compression
+gzip compressed data, was "plotink-1.9.0.tar", last modified: Sat Dec  2 20:43:29 2023, max compression
```

## Comparing `plotink-1.8.0.tar` & `plotink-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 oskay      (504) staff       (20)        0 2022-12-11 19:29:14.138553 plotink-1.8.0/
--rw-r--r--   0 oskay      (504) staff       (20)     1098 2022-01-04 02:39:32.000000 plotink-1.8.0/LICENSE
--rw-r--r--   0 oskay      (504) staff       (20)     2777 2022-12-11 19:29:14.138417 plotink-1.8.0/PKG-INFO
--rw-r--r--   0 oskay      (504) staff       (20)     2126 2022-06-13 01:44:06.000000 plotink-1.8.0/README.md
-drwxr-xr-x   0 oskay      (504) staff       (20)        0 2022-12-11 19:29:14.137375 plotink-1.8.0/plotink/
--rw-r--r--   0 oskay      (504) staff       (20)        0 2019-09-28 22:35:55.000000 plotink-1.8.0/plotink/__init__.py
--rw-r--r--   0 oskay      (504) staff       (20)    18950 2022-10-31 08:49:19.000000 plotink-1.8.0/plotink/ebb_motion.py
--rw-r--r--   0 oskay      (504) staff       (20)    16075 2022-10-31 08:49:19.000000 plotink-1.8.0/plotink/ebb_serial.py
--rw-r--r--   0 oskay      (504) staff       (20)    29877 2022-12-11 07:06:59.000000 plotink-1.8.0/plotink/plot_utils.py
--rw-r--r--   0 oskay      (504) staff       (20)     1906 2019-11-11 19:46:38.000000 plotink-1.8.0/plotink/plot_utils_import.py
--rw-r--r--   0 oskay      (504) staff       (20)     4158 2022-01-04 02:39:32.000000 plotink-1.8.0/plotink/rtree.py
--rw-r--r--   0 oskay      (504) staff       (20)    10521 2022-01-04 02:39:32.000000 plotink-1.8.0/plotink/spatial_grid.py
--rw-r--r--   0 oskay      (504) staff       (20)     3113 2021-12-14 22:44:34.000000 plotink-1.8.0/plotink/text_utils.py
-drwxr-xr-x   0 oskay      (504) staff       (20)        0 2022-12-11 19:29:14.138221 plotink-1.8.0/plotink.egg-info/
--rw-r--r--   0 oskay      (504) staff       (20)     2777 2022-12-11 19:29:14.000000 plotink-1.8.0/plotink.egg-info/PKG-INFO
--rw-r--r--   0 oskay      (504) staff       (20)      358 2022-12-11 19:29:14.000000 plotink-1.8.0/plotink.egg-info/SOURCES.txt
--rw-r--r--   0 oskay      (504) staff       (20)        1 2022-12-11 19:29:14.000000 plotink-1.8.0/plotink.egg-info/dependency_links.txt
--rw-r--r--   0 oskay      (504) staff       (20)       69 2022-12-11 19:29:14.000000 plotink-1.8.0/plotink.egg-info/requires.txt
--rw-r--r--   0 oskay      (504) staff       (20)        8 2022-12-11 19:29:14.000000 plotink-1.8.0/plotink.egg-info/top_level.txt
--rw-r--r--   0 oskay      (504) staff       (20)       38 2022-12-11 19:29:14.138595 plotink-1.8.0/setup.cfg
--rw-r--r--   0 oskay      (504) staff       (20)     1318 2022-12-11 07:15:17.000000 plotink-1.8.0/setup.py
+drwxr-xr-x   0 oskay      (504) staff       (20)        0 2023-12-02 20:43:29.945861 plotink-1.9.0/
+-rw-r--r--   0 oskay      (504) staff       (20)     1098 2022-01-04 02:39:32.000000 plotink-1.9.0/LICENSE
+-rw-r--r--   0 oskay      (504) staff       (20)     2936 2023-12-02 20:43:29.945659 plotink-1.9.0/PKG-INFO
+-rw-r--r--   0 oskay      (504) staff       (20)     2126 2022-06-13 01:44:06.000000 plotink-1.9.0/README.md
+drwxr-xr-x   0 oskay      (504) staff       (20)        0 2023-12-02 20:43:29.944460 plotink-1.9.0/plotink/
+-rw-r--r--   0 oskay      (504) staff       (20)        0 2019-09-28 22:35:55.000000 plotink-1.9.0/plotink/__init__.py
+-rw-r--r--   0 oskay      (504) staff       (20)    14815 2023-12-02 20:40:08.000000 plotink-1.9.0/plotink/ebb_calc.py
+-rw-r--r--   0 oskay      (504) staff       (20)    16218 2023-12-02 20:39:22.000000 plotink-1.9.0/plotink/ebb_motion.py
+-rw-r--r--   0 oskay      (504) staff       (20)    16075 2023-12-02 19:39:29.000000 plotink-1.9.0/plotink/ebb_serial.py
+-rw-r--r--   0 oskay      (504) staff       (20)    29877 2023-12-02 19:39:33.000000 plotink-1.9.0/plotink/plot_utils.py
+-rw-r--r--   0 oskay      (504) staff       (20)     1906 2019-11-11 19:46:38.000000 plotink-1.9.0/plotink/plot_utils_import.py
+-rw-r--r--   0 oskay      (504) staff       (20)     4158 2022-01-04 02:39:32.000000 plotink-1.9.0/plotink/rtree.py
+-rw-r--r--   0 oskay      (504) staff       (20)    10521 2022-01-04 02:39:32.000000 plotink-1.9.0/plotink/spatial_grid.py
+-rw-r--r--   0 oskay      (504) staff       (20)     3113 2021-12-14 22:44:34.000000 plotink-1.9.0/plotink/text_utils.py
+drwxr-xr-x   0 oskay      (504) staff       (20)        0 2023-12-02 20:43:29.945397 plotink-1.9.0/plotink.egg-info/
+-rw-r--r--   0 oskay      (504) staff       (20)     2936 2023-12-02 20:43:29.000000 plotink-1.9.0/plotink.egg-info/PKG-INFO
+-rw-r--r--   0 oskay      (504) staff       (20)      378 2023-12-02 20:43:29.000000 plotink-1.9.0/plotink.egg-info/SOURCES.txt
+-rw-r--r--   0 oskay      (504) staff       (20)        1 2023-12-02 20:43:29.000000 plotink-1.9.0/plotink.egg-info/dependency_links.txt
+-rw-r--r--   0 oskay      (504) staff       (20)       83 2023-12-02 20:43:29.000000 plotink-1.9.0/plotink.egg-info/requires.txt
+-rw-r--r--   0 oskay      (504) staff       (20)        8 2023-12-02 20:43:29.000000 plotink-1.9.0/plotink.egg-info/top_level.txt
+-rw-r--r--   0 oskay      (504) staff       (20)       38 2023-12-02 20:43:29.946038 plotink-1.9.0/setup.cfg
+-rw-r--r--   0 oskay      (504) staff       (20)     1343 2023-12-02 20:39:22.000000 plotink-1.9.0/setup.py
```

### Comparing `plotink-1.8.0/LICENSE` & `plotink-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plotink-1.8.0/PKG-INFO` & `plotink-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: plotink
-Version: 1.8.0
+Version: 1.9.0
 Summary: Helper routines for use with plotters
 Home-page: https://github.com/evil-mad/plotink
 Author: Evil Mad Scientist Laboratories
 Author-email: contact@evilmadscientist.com
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ink_extensions
+Requires-Dist: mpmath>=1.3.0
+Requires-Dist: packaging>=21.0
+Requires-Dist: pyserial>=3.5
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
 
 # plotink
 Python helper routines for driving AxiDraw, EggBot, WaterColorBot, and similar plotter-based machines.
 
 Source code and issue tracker are hosted [at github](https://github.com/evil-mad/plotink).
```

### Comparing `plotink-1.8.0/README.md` & `plotink-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `plotink-1.8.0/plotink/ebb_motion.py` & `plotink-1.9.0/plotink/ebb_motion.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Intended to provide some common interfaces that can be used by
 EggBot, WaterColorBot, AxiDraw, and similar machines.
 
 See version() below for version number.
 
 The MIT License (MIT)
 
-Copyright (c) 2022 Windell H. Oskay, Evil Mad Scientist Laboratories
+Copyright (c) 2023 Windell H. Oskay, Evil Mad Scientist Laboratories
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -29,21 +29,20 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import math
 from . import ebb_serial
+from . import ebb_calc
 
 def version():  # Report version number for this document
     ''' Return version number '''
-    return "0.25"  # Dated 2022-10-05
-
+    return "0.26"  # Dated 2023-05-04
 
 def doABMove(port_name, delta_a, delta_b, duration, verbose=True):
     '''
     Issue command to move A/B axes as: "XM,<move_duration>,<axisA>,<axisB><CR>"
     Then, <Axis1> moves by <AxisA> + <AxisB>, and <Axis2> as <AxisA> - <AxisB>
     '''
     if port_name is not None:
@@ -121,134 +120,44 @@
         else:
             str_output = 'HM,{0}\r'.format(rate)
         ebb_serial.command(port_name, str_output, verbose)
 
 
 def moveDistLM(rate_in, accel_in, time_ticks):
     '''
-    Calculate the number of motor steps taken using the LM command,
-    with rate factor r, acceleration accel_in, and in a given number
-    of 40 us time_ticks. Calculation is for one axis only.
-    Step distance moved after T time ticks is given by:
-        S = floor(( 2 * R * T + A * T^2 )/ 2^32 )
-
-    This calculation is valid for the revised LM command as of
-    version 2.7 of the EBB firmware.
-    '''
-    time = int(time_ticks)  # Ensure that the inputs are integral.
-    rate_r0 = int(rate_in)
-    accel = int(accel_in)
-    if time == 0:
-        return 0
-    return (2 * rate_r0 * time + accel * time * time) >> 32
-
+    Deprecated function as of v 0.26, and will be removed in a future version.
+    Same as ebb_calc.move_dist_lt(), but does not accept or return accumulator value.
+    (This function was removed because without knowing the initial accumulator value,
+        it is possible to get the wrong distance.)
 
-def moveDistLMA(rate_in, accel_in, time_ticks, accum_in):
+    Calls to this function may be replaced as per the example here, but it is better to
+        use ebb_calc.move_dist_lt() *with* an initial accumulator value.
     '''
-    Calculate motor step count and final accumulator "remainder"
-    after a certain number of time ticks, using the LM or LT
-    command. Calculation is for one axis only.
+    dist, _accum = ebb_calc.move_dist_lt(rate_in, accel_in, time_ticks, 0)
+    return dist
 
-    Inputs: Rate factor rate_in, acceleration accel_in, initial
-    accumulator value accum_in, and 40 us intervals time_ticks.
 
-    Accumulator value T time ticks is given by:
-        Accum = R * T + 0.5 * accel_in * T^2 + accum_in
-        Steps = floor (Accum / 2^31)
-        Remainder = Accum - 2^31 * Steps
-
-    Return Steps, Remainder
-    This calculation is valid for version 2.7+ of the EBB firmware.
+def moveDistLMA(rate_in, accel_in, time_ticks, accum_in):
     '''
-    time = int(time_ticks)  # Ensure that the inputs are integral.
-    rate_r0 = int(rate_in)
-    accel = int(accel_in)
-    accum_0 = int(accum_in)
-    if time == 0:
-        return 0, 0
-
-    # TWICE the accumulator value, before dividing:
-    accum_end = (2 * accum_0 + 2 * rate_r0 * time + accel * time * time) >> 1
-    step_count = accum_end >> 31
-    rems = (accum_end) - (step_count << 31)
-
-    return step_count, rems
+    Deprecated function as of v 0.26, and will be removed in a future version.
+    Function renamed to: move_dist_lt().
+    '''
+    return ebb_calc.move_dist_lt(rate_in, accel_in, time_ticks, accum_in)
 
 
-def moveTimeLM(rate_in, steps, accel_in):
+def moveTimeLM(rate, steps, accel):
     """
-    Calculate how long, in 40 us ISR intervals, the LM command will take to move one axis.
+    Deprecated function as of v 0.26, and will be removed in a future version.
 
-    First: Distance in steps moved after T time ticks is given by
-      the formula: S = floor(( 2 * R * T + A * T^2 )/ 2^32 )
-    Use the quadratic formula to solve for possible values of time T,
-    the number of time ticks needed to travel the through distance of steps.
-
-    As this is a floating point result, we will round down the output, and
-    then move one time step forward until we find the result.
-
-    This calculation is valid for the revised LM command as of
-    version 2.7 of the EBB firmware.
+    Calculate how long, in 40 us ISR intervals, the LM command will take to move one axis.
+    Older version, for firmware 2.7+
     """
 
-    steps = abs(steps)
-    rate = float(rate_in)
-    accel = float(accel_in)
-
-    if steps == 0:
-        return 0  # No steps to take, so takes zero time.
-
-    if accel_in == 0:
-        if rate_in == 0:
-            return 0  # No move will be made if rate_in and accel_in are both zero.
-
-        # Case of no acceleration: Simple to get actual movement time, since
-        # Steps = floor(rate * Time / 2^31)
-        # Thus, Time = ceil(Steps * 2^31 / rate)
-
-        scaled_f = int(steps) << 31
-        return int(math.ceil(scaled_f / rate))
-
-    # Otherwise, accel_in is not zero.
-
-    # Solve quadratic for T
-    # S = floor(( 2 * R * T + A * T^2 )/ 2^32 )
-    # -> (1/2)A T^2 + R T - 2^31 S = 0
-    # a = A/2
-    # b = R
-    # c = -2^31 S
-    #
-    # T = (-b +/- sqrt(b^2 - 4 a c)) / 2 a
-
-    # factors:
-    a_fact = accel / 2.0
-    b_fact = rate
-    c_fact = -2147483648.0 * steps
-
-    root_factor = b_fact * b_fact - 4 * a_fact * c_fact
-
-    if root_factor < 0:
-        root_factor = 0
-    root = math.sqrt(root_factor)
-
-    result1 = int(math.ceil((- b_fact + root) / accel))
-    result2 = int(math.ceil((- b_fact - root) / accel))
-
-    if result1 < 0 and result2 < 0:
-        return -1  # No plausible roots; movement time must be positive
-
-    if result1 < 0:
-        time_ticks = result2  # Pick the positive root
-    elif result2 < 0:
-        time_ticks = result1  # Pick the positive root
-    elif result2 < result1:  # If both are valid, pick the smaller value.
-        time_ticks = result2
-    else:
-        time_ticks = result1
-    return time_ticks
+    time, _dist, _accum = ebb_calc.calculate_lm(steps, rate, accel, accum="clear")
+    return time
 
 
 def QueryPenUp(port_name, verbose=True):
     """ Check if the pen is up, using QP. """
     if port_name is not None:
         pen_status = ebb_serial.query(port_name, 'QP\r', verbose)
         if pen_status[0] == '0':
```

### Comparing `plotink-1.8.0/plotink/ebb_serial.py` & `plotink-1.9.0/plotink/ebb_serial.py`

 * *Files identical despite different names*

### Comparing `plotink-1.8.0/plotink/plot_utils.py` & `plotink-1.9.0/plotink/plot_utils.py`

 * *Files identical despite different names*

### Comparing `plotink-1.8.0/plotink/plot_utils_import.py` & `plotink-1.9.0/plotink/plot_utils_import.py`

 * *Files identical despite different names*

### Comparing `plotink-1.8.0/plotink/rtree.py` & `plotink-1.9.0/plotink/rtree.py`

 * *Files identical despite different names*

### Comparing `plotink-1.8.0/plotink/spatial_grid.py` & `plotink-1.9.0/plotink/spatial_grid.py`

 * *Files identical despite different names*

### Comparing `plotink-1.8.0/plotink/text_utils.py` & `plotink-1.9.0/plotink/text_utils.py`

 * *Files identical despite different names*

### Comparing `plotink-1.8.0/plotink.egg-info/PKG-INFO` & `plotink-1.9.0/plotink.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: plotink
-Version: 1.8.0
+Version: 1.9.0
 Summary: Helper routines for use with plotters
 Home-page: https://github.com/evil-mad/plotink
 Author: Evil Mad Scientist Laboratories
 Author-email: contact@evilmadscientist.com
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ink_extensions
+Requires-Dist: mpmath>=1.3.0
+Requires-Dist: packaging>=21.0
+Requires-Dist: pyserial>=3.5
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
 
 # plotink
 Python helper routines for driving AxiDraw, EggBot, WaterColorBot, and similar plotter-based machines.
 
 Source code and issue tracker are hosted [at github](https://github.com/evil-mad/plotink).
```

### Comparing `plotink-1.8.0/setup.py` & `plotink-1.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='plotink',
-    version='1.8.0',
+    version='1.9.0',
     python_requires='>=3.6.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/evil-mad/plotink',
     author='Evil Mad Scientist Laboratories',
     author_email='contact@evilmadscientist.com',
     description="Helper routines for use with plotters",
@@ -32,14 +32,15 @@
         "Natural Language :: English",
         "Intended Audience :: Developers",
     ],
 
     packages=find_packages(exclude=['contrib', 'docs', 'test', 'test.*']),
     install_requires=[
         'ink_extensions',
+        'mpmath>=1.3.0',
         'packaging>=21.0',
         'pyserial>=3.5',
     ],
     extras_require={
         'dev': ['coverage'],
         'test': [],
     },
```

