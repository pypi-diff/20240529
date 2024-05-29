# Comparing `tmp/metrit-0.0.1.tar.gz` & `tmp/metrit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrit-0.0.1.tar", last modified: Tue May 28 19:30:38 2024, max compression
+gzip compressed data, was "metrit-0.0.3.tar", last modified: Wed May 29 09:40:13 2024, max compression
```

## Comparing `metrit-0.0.1.tar` & `metrit-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 19:30:38.780327 metrit-0.0.1/
--rw-rw-rw-   0        0        0     1069 2024-05-23 17:02:02.000000 metrit-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    11409 2024-05-28 19:30:38.779060 metrit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10784 2024-05-28 19:22:57.000000 metrit-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 19:30:38.749009 metrit-0.0.1/metrit/
--rw-rw-rw-   0        0        0    10816 2024-05-28 17:43:00.000000 metrit-0.0.1/metrit/Monitoring.py
--rw-rw-rw-   0        0        0    15508 2024-05-28 17:13:01.000000 metrit-0.0.1/metrit/StatCollector.py
--rw-rw-rw-   0        0        0      839 2024-05-27 18:36:05.000000 metrit-0.0.1/metrit/Stats.py
--rw-rw-rw-   0        0        0       80 2024-05-26 05:45:09.000000 metrit-0.0.1/metrit/__init__.py
--rw-rw-rw-   0        0        0    10267 2024-05-28 19:19:40.000000 metrit-0.0.1/metrit/core.py
--rw-rw-rw-   0        0        0     2848 2024-05-28 19:19:52.000000 metrit-0.0.1/metrit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 19:30:38.775230 metrit-0.0.1/metrit.egg-info/
--rw-rw-rw-   0        0        0    11409 2024-05-28 19:30:38.000000 metrit-0.0.1/metrit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-05-28 19:30:38.000000 metrit-0.0.1/metrit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 19:30:38.000000 metrit-0.0.1/metrit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-28 19:30:38.000000 metrit-0.0.1/metrit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-28 19:30:38.000000 metrit-0.0.1/metrit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 19:30:38.780327 metrit-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-05-28 19:27:44.000000 metrit-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 19:30:38.774234 metrit-0.0.1/tests/
--rw-rw-rw-   0        0        0     9264 2024-05-28 17:26:03.000000 metrit-0.0.1/tests/test_StatsCollector.py
--rw-rw-rw-   0        0        0     3074 2024-05-28 17:33:22.000000 metrit-0.0.1/tests/test_metrit.py
--rw-rw-rw-   0        0        0     6906 2024-05-28 17:30:46.000000 metrit-0.0.1/tests/test_metrit_deactivated.py
--rw-rw-rw-   0        0        0     3606 2024-05-28 17:31:51.000000 metrit-0.0.1/tests/test_metrit_with_args.py
--rw-rw-rw-   0        0        0      745 2024-05-28 17:04:00.000000 metrit-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:13.659616 metrit-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 09:40:02.000000 metrit-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 09:40:13.659616 metrit-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-29 09:40:02.000000 metrit-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:13.655616 metrit-0.0.3/metrit/
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/Monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/StatCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/Stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:13.659616 metrit-0.0.3/metrit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:40:13.659616 metrit-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 09:40:10.000000 metrit-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:13.659616 metrit-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_StatsCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_metrit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_metrit_deactivated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_metrit_with_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_utils.py
```

### Comparing `metrit-0.0.1/LICENSE` & `metrit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metrit-0.0.1/PKG-INFO` & `metrit-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-Metadata-Version: 2.1
-Name: metrit
-Version: 0.0.1
-Summary: A dead simple resources monitoring decorator
-Home-page: https://github.com/mcrespoae/metrit
-Author: mcrespoae
-Author-email: info@mariocrespo.es
-Keywords: metrit
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: psutil==5.9.8
-Requires-Dist: multiprocess==0.70.16
-
-
-# metrit
-
-![PyPI](https://img.shields.io/pypi/v/metrit?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/metrit)
-
-## Overview
-
-`metrit` is a Python package designed to simplify the process of measuring the execution resources of your functions through a straightforward decorator.
-
-## Installation
-
-You can install `metrit` using pip:
-
-```bash
-pip install metrit
-```
-
-## Usage
-
-Utilizing the `metrit` decorator is simple and intuitive. Follow this section to learn how to make the most of its capabilities.
-
-### Basic Usage
-
-Below are some examples demonstrating `metrit`'s usage:
-
-```python
-from metrit import metrit
-
-@metrit
-def my_function():
-    # Normal code of your function
-    pass
-
-my_function()
-```
-
-This will output something like:
-
-```text
-Function 'my_function'    24.00KB avg of memory     0.00% avg of CPU     239B IO reads   2.05KB IO writes.
-```
-
-### Advanced Usage
-
-You can customize the behavior of the `metrit` decorator using various [Parameters](#parameters). Here is an example:
-
-```python
-from metrit import metrit
-@metrit(verbose=True, find_children=True, isolate=True)
-def my_function_with_args(a:int = 1, b:int = 2):
-    return a + b
-
-result = my_function_with_args(1, b=2)
-```
-
-This will provide detailed output:
-
-```text
-***** metrit data for function my_function_with_args: *****
-    Args: (1,).
-    Kwargs: {'b': 2}.
-    Maximum CPU usage: 0.00%.
-    Average CPU usage: 0.00%.
-    Average memory usage: 0.00%.
-    Maximum RSS memory usage: 112.00KB.
-    Average RSS memory usage: 112.00KB.
-    Maximum VMS memory usage: 68.00KB.
-    Average VMS memory usage: 68.00KB.
-    IO read count: 5.
-    IO writes count: 2.
-    IO read bytes: 239B.
-    IO write bytes: 2.01KB.
-***** End of metrit data. *****
-```
-
-More examples can be found in the [examples.py](https://github.com/mcrespoae/metrit/blob/main/examples/examples.py) script.
-
-### Metrit in Production Environments
-
-The `metrit` decorator is designed **exclusively for benchmarking and is not suitable for use in production code**. You can globally deactivate the `metrit` feature by setting the `MetrittConfig.ACTIVE` flag to false at the top of your imports. While this will skip the decoration of callables, there may still be a minimal CPU overhead. For production-grade applications, it's recommended to manually remove the decorators and `metrit` imports to maintain optimal performance.
-
-```python
-from metrit import MetritConfig, metrit
-MetritConfig.ACTIVE = False  # Deactivates the decorator
-```
-
-## Features
-
-- Simplified usage.
-- Accurate measurement of function resources.
-- Ability to isolate the execution of the function for more accurate measurement.
-- Support for functions, methods, `classmethod` and `staticmethods`.
-- Human-readable data formatting.
-- Optional verbose mode for detailed information.
-- Ability to globally deactivate the `metrit` decorator.
-- Optional check children processes' resources as well.
-- Automatic recursion detection.
-
-## Parameters
-
-Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
-
-- `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
-- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
-- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
-
-## Best Practices
-
-The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
-
-- For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
-
-- Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
-
-- Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
-
-## Recursive Functions
-
-Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
-
-### Using the Auto-Recursion Feature
-
-The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
-
-This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
-
-```python
-@metrit
-def recursive_func(n):
-    if n == 0:
-        return 0
-    else:
-        return n + recursive_func(n - 1)
-
-
-# This will trigger the auto-recursion feature
-result = recursive_func(3)
-```
-
-### Encapsulating the Recursive Function
-
-The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
-
-```python
-@metrit
-def encapsulated_recursive_function(n):
-    """A non-verbose wrapper for the recursive function."""
-    def recursive_func(n):
-        if n == 0:
-            return 0
-        else:
-            return n + recursive_func(n - 1)
-
-    return recursive_func(n)
-
-# Encapsulating the recursive function
-result = encapsulated_recursive_function(3)
-```
-
-This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
-
-## Isolate
-
-The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
-
-## Limitations
-
-While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
-
-### Isolate Limitations
-
-While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
-
-- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
-- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
-
-### Why is Class Decoration Bypassed?
-
-When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
-
-This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
-
-### MacOs Limitations
-
-This package relies on the `psutil` package for retrieving data. Unfortunately, macOS and `psutil` do not support IO data per process, so IO data will not be shown on macOS.
-
-### CPU Percentage Over 100
-
-As noted in the psutil documentation:
-> Note: the returned value can be > 100.0 in case of a process running multiple threads on different CPU cores.
-
-Additionally, if `find_children` is set to `True`, the CPU percentage of all child processes will be added to the main process. This can easily result in the max and average CPU percentages exceeding 100%.
-
-## Error Management and Warnings
-
-### Errors
-
-If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
-
-### Warnings
-
-- Deprecation warnings will be added before removing a feature.
-- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
-
-## Contributing
-
-Contributions are welcome! Please follow these guidelines when contributing:
-
-1. Fork the repository.
-2. Use `make install` to install all dependencies.
-3. Create a new branch for your changes.
-4. Implement your changes and commit them.
-5. Push your changes to your forked repository.
-6. Submit a pull request.
-
-You can also open an issue if you find a bug or have a suggestion.
-
-You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/metrit/blob/main/Makefile) to know more about commands.
-
-## Testing
-
-The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/metrit/tree/main/tests).
-
-## License
-
-This project is licensed under the [MIT License](https://github.com/mcrespoae/metrit/blob/main/LICENSE).
-
-## Contributors
-
-- [Mario Crespo](https://github.com/mcrespoae)
+Metadata-Version: 2.1
+Name: metrit
+Version: 0.0.3
+Summary: A dead simple resources monitoring decorator
+Home-page: https://github.com/mcrespoae/metrit
+Author: mcrespoae
+Author-email: info@mariocrespo.es
+Keywords: metrit
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: psutil==5.9.8
+Requires-Dist: multiprocess==0.70.16
+
+
+# metrit
+
+![PyPI](https://img.shields.io/pypi/v/metrit?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/metrit)
+
+## Overview
+
+`metrit` is a Python package designed to simplify the process of measuring the execution resources of your functions through a straightforward decorator.
+
+## Installation
+
+You can install `metrit` using pip:
+
+```bash
+pip install metrit
+```
+
+## Usage
+
+Utilizing the `metrit` decorator is simple and intuitive. Follow this section to learn how to make the most of its capabilities.
+
+### Basic Usage
+
+Below are some examples demonstrating `metrit`'s usage:
+
+```python
+from metrit import metrit
+
+@metrit
+def my_function():
+    # Normal code of your function
+    pass
+
+my_function()
+```
+
+This will output something like:
+
+```text
+Function 'my_function'    24.00KB avg of memory     0.00% avg of CPU     239B IO reads   2.05KB IO writes.
+```
+
+### Advanced Usage
+
+You can customize the behavior of the `metrit` decorator using various [Parameters](#parameters). Here is an example:
+
+```python
+from metrit import metrit
+@metrit(verbose=True, find_children=True, isolate=True)
+def my_function_with_args(a:int = 1, b:int = 2):
+    return a + b
+
+result = my_function_with_args(1, b=2)
+```
+
+This will provide detailed output:
+
+```text
+***** metrit data for function my_function_with_args: *****
+    Args: (1,).
+    Kwargs: {'b': 2}.
+    Maximum CPU usage: 0.00%.
+    Average CPU usage: 0.00%.
+    Average memory usage: 0.00%.
+    Maximum RSS memory usage: 112.00KB.
+    Average RSS memory usage: 112.00KB.
+    Maximum VMS memory usage: 68.00KB.
+    Average VMS memory usage: 68.00KB.
+    IO read count: 5.
+    IO writes count: 2.
+    IO read bytes: 239B.
+    IO write bytes: 2.01KB.
+***** End of metrit data. *****
+```
+
+More examples can be found in the [examples.py](https://github.com/mcrespoae/metrit/blob/main/examples/examples.py) script.
+
+### Metrit in Production Environments
+
+The `metrit` decorator is designed **exclusively for benchmarking and is not suitable for use in production code**. You can globally deactivate the `metrit` feature by setting the `MetrittConfig.ACTIVE` flag to false at the top of your imports. While this will skip the decoration of callables, there may still be a minimal CPU overhead. For production-grade applications, it's recommended to manually remove the decorators and `metrit` imports to maintain optimal performance.
+
+```python
+from metrit import MetritConfig, metrit
+MetritConfig.ACTIVE = False  # Deactivates the decorator
+```
+
+## Features
+
+- Simplified usage.
+- Accurate measurement of function resources.
+- Ability to isolate the execution of the function for more accurate measurement.
+- Support for functions, methods, `classmethod` and `staticmethods`.
+- Human-readable data formatting.
+- Optional verbose mode for detailed information.
+- Ability to globally deactivate the `metrit` decorator.
+- Optional check children processes' resources as well.
+- Automatic recursion detection.
+
+## Parameters
+
+Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
+
+- `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
+- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
+- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
+
+## Best Practices
+
+The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
+
+- For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
+
+- Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
+
+- Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
+
+## Recursive Functions
+
+Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
+
+### Using the Auto-Recursion Feature
+
+The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
+
+This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
+
+```python
+@metrit
+def recursive_func(n):
+    if n == 0:
+        return 0
+    else:
+        return n + recursive_func(n - 1)
+
+
+# This will trigger the auto-recursion feature
+result = recursive_func(3)
+```
+
+### Encapsulating the Recursive Function
+
+The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
+
+```python
+@metrit
+def encapsulated_recursive_function(n):
+    """A non-verbose wrapper for the recursive function."""
+    def recursive_func(n):
+        if n == 0:
+            return 0
+        else:
+            return n + recursive_func(n - 1)
+
+    return recursive_func(n)
+
+# Encapsulating the recursive function
+result = encapsulated_recursive_function(3)
+```
+
+This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+
+## Isolate
+
+The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
+
+## Limitations
+
+While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
+
+### Isolate Limitations
+
+While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
+
+- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
+- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
+
+### Why is Class Decoration Bypassed?
+
+When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
+
+This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
+
+### MacOs Limitations
+
+This package relies on the `psutil` package for retrieving data. Unfortunately, macOS and `psutil` do not support IO data per process, so IO data will not be shown on macOS.
+
+### CPU Percentage Over 100
+
+As noted in the psutil documentation:
+> Note: the returned value can be > 100.0 in case of a process running multiple threads on different CPU cores.
+
+Additionally, if `find_children` is set to `True`, the CPU percentage of all child processes will be added to the main process. This can easily result in the max and average CPU percentages exceeding 100%.
+
+## Error Management and Warnings
+
+### Errors
+
+If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
+
+### Warnings
+
+- Deprecation warnings will be added before removing a feature.
+- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
+
+## Contributing
+
+Contributions are welcome! Please follow these guidelines when contributing:
+
+1. Fork the repository.
+2. Use `make install` to install all dependencies.
+3. Create a new branch for your changes.
+4. Implement your changes and commit them.
+5. Push your changes to your forked repository.
+6. Submit a pull request.
+
+You can also open an issue if you find a bug or have a suggestion.
+
+You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/metrit/blob/main/Makefile) to know more about commands.
+
+## Testing
+
+The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/metrit/tree/main/tests).
+
+## License
+
+This project is licensed under the [MIT License](https://github.com/mcrespoae/metrit/blob/main/LICENSE).
+
+## Contributors
+
+- [Mario Crespo](https://github.com/mcrespoae)
```

### Comparing `metrit-0.0.1/README.md` & `metrit-0.0.3/metrit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,231 +1,250 @@
-
-# metrit
-
-![PyPI](https://img.shields.io/pypi/v/metrit?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/metrit)
-
-## Overview
-
-`metrit` is a Python package designed to simplify the process of measuring the execution resources of your functions through a straightforward decorator.
-
-## Installation
-
-You can install `metrit` using pip:
-
-```bash
-pip install metrit
-```
-
-## Usage
-
-Utilizing the `metrit` decorator is simple and intuitive. Follow this section to learn how to make the most of its capabilities.
-
-### Basic Usage
-
-Below are some examples demonstrating `metrit`'s usage:
-
-```python
-from metrit import metrit
-
-@metrit
-def my_function():
-    # Normal code of your function
-    pass
-
-my_function()
-```
-
-This will output something like:
-
-```text
-Function 'my_function'    24.00KB avg of memory     0.00% avg of CPU     239B IO reads   2.05KB IO writes.
-```
-
-### Advanced Usage
-
-You can customize the behavior of the `metrit` decorator using various [Parameters](#parameters). Here is an example:
-
-```python
-from metrit import metrit
-@metrit(verbose=True, find_children=True, isolate=True)
-def my_function_with_args(a:int = 1, b:int = 2):
-    return a + b
-
-result = my_function_with_args(1, b=2)
-```
-
-This will provide detailed output:
-
-```text
-***** metrit data for function my_function_with_args: *****
-    Args: (1,).
-    Kwargs: {'b': 2}.
-    Maximum CPU usage: 0.00%.
-    Average CPU usage: 0.00%.
-    Average memory usage: 0.00%.
-    Maximum RSS memory usage: 112.00KB.
-    Average RSS memory usage: 112.00KB.
-    Maximum VMS memory usage: 68.00KB.
-    Average VMS memory usage: 68.00KB.
-    IO read count: 5.
-    IO writes count: 2.
-    IO read bytes: 239B.
-    IO write bytes: 2.01KB.
-***** End of metrit data. *****
-```
-
-More examples can be found in the [examples.py](https://github.com/mcrespoae/metrit/blob/main/examples/examples.py) script.
-
-### Metrit in Production Environments
-
-The `metrit` decorator is designed **exclusively for benchmarking and is not suitable for use in production code**. You can globally deactivate the `metrit` feature by setting the `MetrittConfig.ACTIVE` flag to false at the top of your imports. While this will skip the decoration of callables, there may still be a minimal CPU overhead. For production-grade applications, it's recommended to manually remove the decorators and `metrit` imports to maintain optimal performance.
-
-```python
-from metrit import MetritConfig, metrit
-MetritConfig.ACTIVE = False  # Deactivates the decorator
-```
-
-## Features
-
-- Simplified usage.
-- Accurate measurement of function resources.
-- Ability to isolate the execution of the function for more accurate measurement.
-- Support for functions, methods, `classmethod` and `staticmethods`.
-- Human-readable data formatting.
-- Optional verbose mode for detailed information.
-- Ability to globally deactivate the `metrit` decorator.
-- Optional check children processes' resources as well.
-- Automatic recursion detection.
-
-## Parameters
-
-Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
-
-- `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
-- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
-- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
-
-## Best Practices
-
-The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
-
-- For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
-
-- Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
-
-- Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
-
-## Recursive Functions
-
-Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
-
-### Using the Auto-Recursion Feature
-
-The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
-
-This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
-
-```python
-@metrit
-def recursive_func(n):
-    if n == 0:
-        return 0
-    else:
-        return n + recursive_func(n - 1)
-
-
-# This will trigger the auto-recursion feature
-result = recursive_func(3)
-```
-
-### Encapsulating the Recursive Function
-
-The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
-
-```python
-@metrit
-def encapsulated_recursive_function(n):
-    """A non-verbose wrapper for the recursive function."""
-    def recursive_func(n):
-        if n == 0:
-            return 0
-        else:
-            return n + recursive_func(n - 1)
-
-    return recursive_func(n)
-
-# Encapsulating the recursive function
-result = encapsulated_recursive_function(3)
-```
-
-This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
-
-## Isolate
-
-The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
-
-## Limitations
-
-While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
-
-### Isolate Limitations
-
-While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
-
-- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
-- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
-
-### Why is Class Decoration Bypassed?
-
-When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
-
-This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
-
-### MacOs Limitations
-
-This package relies on the `psutil` package for retrieving data. Unfortunately, macOS and `psutil` do not support IO data per process, so IO data will not be shown on macOS.
-
-### CPU Percentage Over 100
-
-As noted in the psutil documentation:
-> Note: the returned value can be > 100.0 in case of a process running multiple threads on different CPU cores.
-
-Additionally, if `find_children` is set to `True`, the CPU percentage of all child processes will be added to the main process. This can easily result in the max and average CPU percentages exceeding 100%.
-
-## Error Management and Warnings
-
-### Errors
-
-If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
-
-### Warnings
-
-- Deprecation warnings will be added before removing a feature.
-- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
-
-## Contributing
-
-Contributions are welcome! Please follow these guidelines when contributing:
-
-1. Fork the repository.
-2. Use `make install` to install all dependencies.
-3. Create a new branch for your changes.
-4. Implement your changes and commit them.
-5. Push your changes to your forked repository.
-6. Submit a pull request.
-
-You can also open an issue if you find a bug or have a suggestion.
-
-You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/metrit/blob/main/Makefile) to know more about commands.
-
-## Testing
-
-The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/metrit/tree/main/tests).
-
-## License
-
-This project is licensed under the [MIT License](https://github.com/mcrespoae/metrit/blob/main/LICENSE).
-
-## Contributors
-
-- [Mario Crespo](https://github.com/mcrespoae)
+Metadata-Version: 2.1
+Name: metrit
+Version: 0.0.3
+Summary: A dead simple resources monitoring decorator
+Home-page: https://github.com/mcrespoae/metrit
+Author: mcrespoae
+Author-email: info@mariocrespo.es
+Keywords: metrit
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: psutil==5.9.8
+Requires-Dist: multiprocess==0.70.16
+
+
+# metrit
+
+![PyPI](https://img.shields.io/pypi/v/metrit?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/metrit)
+
+## Overview
+
+`metrit` is a Python package designed to simplify the process of measuring the execution resources of your functions through a straightforward decorator.
+
+## Installation
+
+You can install `metrit` using pip:
+
+```bash
+pip install metrit
+```
+
+## Usage
+
+Utilizing the `metrit` decorator is simple and intuitive. Follow this section to learn how to make the most of its capabilities.
+
+### Basic Usage
+
+Below are some examples demonstrating `metrit`'s usage:
+
+```python
+from metrit import metrit
+
+@metrit
+def my_function():
+    # Normal code of your function
+    pass
+
+my_function()
+```
+
+This will output something like:
+
+```text
+Function 'my_function'    24.00KB avg of memory     0.00% avg of CPU     239B IO reads   2.05KB IO writes.
+```
+
+### Advanced Usage
+
+You can customize the behavior of the `metrit` decorator using various [Parameters](#parameters). Here is an example:
+
+```python
+from metrit import metrit
+@metrit(verbose=True, find_children=True, isolate=True)
+def my_function_with_args(a:int = 1, b:int = 2):
+    return a + b
+
+result = my_function_with_args(1, b=2)
+```
+
+This will provide detailed output:
+
+```text
+***** metrit data for function my_function_with_args: *****
+    Args: (1,).
+    Kwargs: {'b': 2}.
+    Maximum CPU usage: 0.00%.
+    Average CPU usage: 0.00%.
+    Average memory usage: 0.00%.
+    Maximum RSS memory usage: 112.00KB.
+    Average RSS memory usage: 112.00KB.
+    Maximum VMS memory usage: 68.00KB.
+    Average VMS memory usage: 68.00KB.
+    IO read count: 5.
+    IO writes count: 2.
+    IO read bytes: 239B.
+    IO write bytes: 2.01KB.
+***** End of metrit data. *****
+```
+
+More examples can be found in the [examples.py](https://github.com/mcrespoae/metrit/blob/main/examples/examples.py) script.
+
+### Metrit in Production Environments
+
+The `metrit` decorator is designed **exclusively for benchmarking and is not suitable for use in production code**. You can globally deactivate the `metrit` feature by setting the `MetrittConfig.ACTIVE` flag to false at the top of your imports. While this will skip the decoration of callables, there may still be a minimal CPU overhead. For production-grade applications, it's recommended to manually remove the decorators and `metrit` imports to maintain optimal performance.
+
+```python
+from metrit import MetritConfig, metrit
+MetritConfig.ACTIVE = False  # Deactivates the decorator
+```
+
+## Features
+
+- Simplified usage.
+- Accurate measurement of function resources.
+- Ability to isolate the execution of the function for more accurate measurement.
+- Support for functions, methods, `classmethod` and `staticmethods`.
+- Human-readable data formatting.
+- Optional verbose mode for detailed information.
+- Ability to globally deactivate the `metrit` decorator.
+- Optional check children processes' resources as well.
+- Automatic recursion detection.
+
+## Parameters
+
+Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
+
+- `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
+- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
+- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
+
+## Best Practices
+
+The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
+
+- For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
+
+- Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
+
+- Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
+
+## Recursive Functions
+
+Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
+
+### Using the Auto-Recursion Feature
+
+The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
+
+This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
+
+```python
+@metrit
+def recursive_func(n):
+    if n == 0:
+        return 0
+    else:
+        return n + recursive_func(n - 1)
+
+
+# This will trigger the auto-recursion feature
+result = recursive_func(3)
+```
+
+### Encapsulating the Recursive Function
+
+The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
+
+```python
+@metrit
+def encapsulated_recursive_function(n):
+    """A non-verbose wrapper for the recursive function."""
+    def recursive_func(n):
+        if n == 0:
+            return 0
+        else:
+            return n + recursive_func(n - 1)
+
+    return recursive_func(n)
+
+# Encapsulating the recursive function
+result = encapsulated_recursive_function(3)
+```
+
+This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+
+## Isolate
+
+The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
+
+## Limitations
+
+While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
+
+### Isolate Limitations
+
+While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
+
+- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
+- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
+
+### Why is Class Decoration Bypassed?
+
+When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
+
+This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
+
+### MacOs Limitations
+
+This package relies on the `psutil` package for retrieving data. Unfortunately, macOS and `psutil` do not support IO data per process, so IO data will not be shown on macOS.
+
+### CPU Percentage Over 100
+
+As noted in the psutil documentation:
+> Note: the returned value can be > 100.0 in case of a process running multiple threads on different CPU cores.
+
+Additionally, if `find_children` is set to `True`, the CPU percentage of all child processes will be added to the main process. This can easily result in the max and average CPU percentages exceeding 100%.
+
+## Error Management and Warnings
+
+### Errors
+
+If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
+
+### Warnings
+
+- Deprecation warnings will be added before removing a feature.
+- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
+
+## Contributing
+
+Contributions are welcome! Please follow these guidelines when contributing:
+
+1. Fork the repository.
+2. Use `make install` to install all dependencies.
+3. Create a new branch for your changes.
+4. Implement your changes and commit them.
+5. Push your changes to your forked repository.
+6. Submit a pull request.
+
+You can also open an issue if you find a bug or have a suggestion.
+
+You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/metrit/blob/main/Makefile) to know more about commands.
+
+## Testing
+
+The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/metrit/tree/main/tests).
+
+## License
+
+This project is licensed under the [MIT License](https://github.com/mcrespoae/metrit/blob/main/LICENSE).
+
+## Contributors
+
+- [Mario Crespo](https://github.com/mcrespoae)
```

### Comparing `metrit-0.0.1/metrit/Monitoring.py` & `metrit-0.0.3/metrit/Monitoring.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-import time
-from sys import platform
-from typing import Dict, Self
-
-from multiprocess import Process, Queue, current_process
-
-from .StatCollector import StatCollector
-from .Stats import RawStats, Stats
-from .utils import format_size
-
-
-class Monitoring:
-    def __init__(self, find_children: bool = False):
-        """
-        Initializes a new instance of the Monitoring class.
-
-        Args:
-            find_children (bool, optional): If True, the monitoring process will also monitor child processes spawned by the main process. Defaults to False.
-
-        Returns:
-            None
-        """
-        self.pid: int = current_process().pid  # type: ignore
-        self.find_children: bool = find_children
-        self.stat_collector: StatCollector = StatCollector(self.pid)
-        self.stats_per_pid: Dict[int, Stats] = {}
-        self.formated_stats: Stats = Stats()
-
-    @staticmethod
-    def has_process_crashed(queue: Queue) -> bool:
-        """
-        Checks if the process has crashed based on the given queue.
-
-        Args:
-            queue (Queue): The queue containing the process status.
-
-        Returns:
-            bool: True if the process has crashed, False otherwise.
-        """
-        while not queue.empty():
-            if not queue.get():
-                return True
-        return False
-
-    def take_snapshot(self):
-        """
-        Takes a snapshot of RAM and IO stats for the process and its children.
-        Saves the result in `self.stats_per_pid` in the form of Dict[int, Stats].
-        """
-
-        self.pre_success_queue = Queue()
-        self.pre_data_queue = Queue()
-
-        # Take a snapshot of RAM and IO stats for the process and its children
-        try:
-            take_snapshot_process: Process = Process(target=self.collect_snapshot_stats, args=())
-            take_snapshot_process.start()
-            take_snapshot_process.join()  # Ensure process termination
-            has_process_crashed: bool = self.has_process_crashed(self.pre_success_queue)
-            if has_process_crashed:
-                print("Process snapshot has crashed")
-                take_snapshot_process.terminate()
-            raw_snapshot_stats: Dict[int, RawStats] = self.pre_data_queue.get()
-
-        except Exception:
-            raw_snapshot_stats = {}  # Avoid hanging the process if something goes wrong
-
-        self.stats_per_pid: Dict[int, Stats] = self.stat_collector.calculate_statistics_from_data(raw_snapshot_stats)
-
-        # Clear queues
-        self.pre_data_queue.close()
-        self.pre_success_queue.close()
-        delattr(self, "pre_data_queue")
-        delattr(self, "pre_success_queue")
-
-    def collect_snapshot_stats(self):
-        """
-        Collects CPU and RAM statistics for the process and its children, and IO counters.
-        The result is added to the queue.
-        It uses queues to pass the data:
-            pre_data_queue (Queue): A queue to store the collected statistics.
-            success_queue (Queue): A queue to communicate success or failure.
-        """
-        refresh_rate: float = 0.0
-        raw_stats: Dict[int, RawStats] = {}
-
-        cpu_memory_stats = self.stat_collector.collect_cpu_ram_stats(
-            raw_stats, self.find_children, refresh_rate, self.pre_success_queue
-        )
-
-        raw_stats = self.stat_collector.collect_io_counters(
-            cpu_memory_stats, self.find_children, self.pre_success_queue
-        )
-
-        self.pre_data_queue.put(raw_stats)
-
-    def start_monitoring(self):
-        """
-        Initializes the monitoring process by creating queues and starting the pooling process.
-        This function initializes the monitoring process by creating the necessary queues for communication between the main process and the pooling process.
-        """
-
-        self.stop_queue = Queue()
-        self.data_pool_queue = Queue()
-        self.success_queue = Queue()
-        self.pooling_raw_stats: Dict | None = None
-
-        # Start the monitoring process
-        self.pooling_process = Process(target=self.pool_stats, args=())
-        self.pooling_process.start()
-
-    def stop_monitoring(self):
-        """
-        Stops the monitoring process by sending a signal to stop the pooling process.
-        This function sends a signal to stop the pooling process by putting the string "STOP" into the `stop_queue`.
-        It then waits for the pooling process to terminate using the `join()` method.
-        If the pooling process has crashed, it prints a message and terminates the process using the `terminate()` method.
-        After that, it retrieves the raw statistics from the `data_pool_queue` and calculates the statistics per PID using the `calculate_statistics_from_data()` method of the `stat_collector` object.
-        The object stats_per_pid is a dict of Stats objects, where the keys are the PIDs and the values are the corresponding Stats objects.
-        """
-        # Send a signal to stop the pooling process
-        self.stop_queue.put("STOP")
-        self.pooling_process.join()  # type: ignore
-        has_process_crashed = self.has_process_crashed(self.success_queue)
-        if has_process_crashed:
-            print("Process pooling has crashed")
-            self.pooling_process.terminate()  # type: ignore
-
-        pooling_raw_stats: Dict[int, RawStats] = self.data_pool_queue.get()
-
-        self.stats_per_pid = self.stat_collector.calculate_statistics_from_data(pooling_raw_stats)
-
-        # Clean queues and process
-        self.stop_queue.close()
-        self.data_pool_queue.close()
-        self.success_queue.close()
-        delattr(self, "stop_queue")
-        delattr(self, "data_pool_queue")
-        delattr(self, "success_queue")
-        delattr(self, "pooling_process")
-
-    def pool_stats(self):
-        """
-        Collects statistics about CPU and RAM usage and IO counters for the process and its children.
-        It uses queues to pass the data:
-            data_pool_queue (Queue): A queue to store the collected statistics as a dict of RawStats.
-            stop_queue (Queue): A queue to receive stop signals.
-            success_queue (Queue): A queue to communicate success or failure.
-        """
-        refresh_rate: float = 0.1  # Initial refresh rate
-        max_refresh_rate: int = 5  # Maximum refresh rate
-        time_elapsed: float = 0.0
-        stats: Dict[int, RawStats] = {}
-
-        while True:
-
-            stats = self.stat_collector.collect_cpu_ram_stats(
-                stats, self.find_children, refresh_rate, self.success_queue
-            )
-            if not self.stop_queue.empty():
-                message = self.stop_queue.get()
-                if message == "STOP":
-                    stats = self.stat_collector.collect_io_counters(stats, self.find_children, self.success_queue)
-                    self.data_pool_queue.put(stats)
-                    break
-            time.sleep(refresh_rate)
-            time_elapsed += refresh_rate
-            if time_elapsed > 10:
-                if refresh_rate < max_refresh_rate:
-                    refresh_rate = min(refresh_rate * 2, max_refresh_rate)
-                    # Double the refresh rate, but do not exceed max_refresh_rate
-                time_elapsed = 0.0
-
-    def calculate_delta(self, other: Self):
-        """
-        Calculate the difference between the current instance's stats_per_pid and another instance's stats_per_pid.
-
-        Args:
-            other (Self): The other instance to compare stats_per_pid with.
-        """
-        subtracted_stats: Dict[int, Stats] = self.stat_collector.subtract_stats(self.stats_per_pid, other.stats_per_pid)
-        self.formated_stats: Stats = self.stat_collector.get_final_stats(subtracted_stats)
-
-    def get_data(self):
-        """
-        Retrieves the formatted statistics from the `formated_stats` attribute of the current instance.
-        Returns:
-            The formatted statistics as a `Stats` object.
-        """
-        return self.formated_stats
-
-    def print(self, verbose: bool, func_name: str, args: tuple, kwargs: dict) -> None:
-        """
-        Prints the metrit data for a given function.
-
-        Parameters:
-            verbose (bool): If True, prints detailed information about the metrit data. If False, prints a concise summary.
-            func_name (str): The name of the function.
-            args (tuple): The positional arguments passed to the function.
-            kwargs (dict): The keyword arguments passed to the function.
-
-        Returns:
-            None
-        """
-        data: Stats = self.formated_stats
-        if verbose:
-            print("*" * 5, f"metrit data for function {func_name}:", "*" * 5)
-            print(f"\tArgs: {args}.")
-            print(f"\tKwargs: {kwargs}.")
-            print(f"Maximum CPU usage: {data.cpu_percentage_max:.2f}%.")
-            print(f"Average CPU usage: {data.cpu_percentage_avg:.2f}%.")
-            print(f"Average memory usage: {data.memory_percentage_avg:.2f}%.")
-            print(f"Maximum RSS memory usage: {format_size(data.rss_bytes_max)}.")
-            print(f"Average RSS memory usage: {format_size(data.rss_bytes_avg)}.")
-            print(f"Maximum VMS memory usage: {format_size(data.vms_bytes_max)}.")
-            print(f"Average VMS memory usage: {format_size(data.vms_bytes_avg)}.")
-
-            if platform != "darwin":
-                print(f"IO read count: {data.read_count}.")
-                print(f"IO writes count: {data.write_count}.")
-                print(f"IO read bytes: {format_size(data.read_bytes)}.")
-                print(f"IO write bytes: {format_size(data.write_bytes)}.")
-            print("*" * 5, "End of metrit data.", "*" * 5)
-        else:
-            func_name_spacing = 30
-            func_name = f"'{func_name}'"
-            if len(func_name) > func_name_spacing:
-                func_name = func_name[: func_name_spacing - 4] + "..." + "'"
-            if platform != "darwin":
-                output_format = "Function {:30} {:>8} avg of memory {:>8.2f}% avg of CPU {:>8} IO reads {:>8} IO writes"
-                output = output_format.format(
-                    func_name,
-                    format_size(data.rss_bytes_avg),
-                    data.cpu_percentage_avg,
-                    format_size(data.read_bytes),
-                    format_size(data.write_bytes),
-                )
-            else:
-                output_format = "Function {:30} {:>8} avg of memory {:>8.2f}% avg of CPU"
-                output = output_format.format(func_name, format_size(data.rss_bytes_avg), data.cpu_percentage_avg)
-            print(output)
+import time
+from sys import platform
+from typing import Dict, Self
+
+from multiprocess import Process, Queue, current_process
+
+from .StatCollector import StatCollector
+from .Stats import RawStats, Stats
+from .utils import format_size
+
+
+class Monitoring:
+    def __init__(self, find_children: bool = False):
+        """
+        Initializes a new instance of the Monitoring class.
+
+        Args:
+            find_children (bool, optional): If True, the monitoring process will also monitor child processes spawned by the main process. Defaults to False.
+
+        Returns:
+            None
+        """
+        self.pid: int = current_process().pid  # type: ignore
+        self.find_children: bool = find_children
+        self.stat_collector: StatCollector = StatCollector(self.pid)
+        self.stats_per_pid: Dict[int, Stats] = {}
+        self.formated_stats: Stats = Stats()
+
+    @staticmethod
+    def has_process_crashed(queue: Queue) -> bool:
+        """
+        Checks if the process has crashed based on the given queue.
+
+        Args:
+            queue (Queue): The queue containing the process status.
+
+        Returns:
+            bool: True if the process has crashed, False otherwise.
+        """
+        while not queue.empty():
+            if not queue.get():
+                return True
+        return False
+
+    def take_snapshot(self):
+        """
+        Takes a snapshot of RAM and IO stats for the process and its children.
+        Saves the result in `self.stats_per_pid` in the form of Dict[int, Stats].
+        """
+
+        self.pre_success_queue = Queue()
+        self.pre_data_queue = Queue()
+
+        # Take a snapshot of RAM and IO stats for the process and its children
+        try:
+            take_snapshot_process: Process = Process(target=self.collect_snapshot_stats, args=())
+            take_snapshot_process.start()
+            take_snapshot_process.join()  # Ensure process termination
+            has_process_crashed: bool = self.has_process_crashed(self.pre_success_queue)
+            if has_process_crashed:
+                print("Process snapshot has crashed")
+                take_snapshot_process.terminate()
+            raw_snapshot_stats: Dict[int, RawStats] = self.pre_data_queue.get()
+
+        except Exception:
+            raw_snapshot_stats = {}  # Avoid hanging the process if something goes wrong
+
+        self.stats_per_pid: Dict[int, Stats] = self.stat_collector.calculate_statistics_from_data(raw_snapshot_stats)
+
+        # Clear queues
+        self.pre_data_queue.close()
+        self.pre_success_queue.close()
+        delattr(self, "pre_data_queue")
+        delattr(self, "pre_success_queue")
+
+    def collect_snapshot_stats(self):
+        """
+        Collects CPU and RAM statistics for the process and its children, and IO counters.
+        The result is added to the queue.
+        It uses queues to pass the data:
+            pre_data_queue (Queue): A queue to store the collected statistics.
+            success_queue (Queue): A queue to communicate success or failure.
+        """
+        refresh_rate: float = 0.0
+        raw_stats: Dict[int, RawStats] = {}
+
+        cpu_memory_stats = self.stat_collector.collect_cpu_ram_stats(
+            raw_stats, self.find_children, refresh_rate, self.pre_success_queue
+        )
+
+        raw_stats = self.stat_collector.collect_io_counters(
+            cpu_memory_stats, self.find_children, self.pre_success_queue
+        )
+
+        self.pre_data_queue.put(raw_stats)
+
+    def start_monitoring(self):
+        """
+        Initializes the monitoring process by creating queues and starting the pooling process.
+        This function initializes the monitoring process by creating the necessary queues for communication between the main process and the pooling process.
+        """
+
+        self.stop_queue = Queue()
+        self.data_pool_queue = Queue()
+        self.success_queue = Queue()
+        self.pooling_raw_stats: Dict | None = None
+
+        # Start the monitoring process
+        self.pooling_process = Process(target=self.pool_stats, args=())
+        self.pooling_process.start()
+
+    def stop_monitoring(self):
+        """
+        Stops the monitoring process by sending a signal to stop the pooling process.
+        This function sends a signal to stop the pooling process by putting the string "STOP" into the `stop_queue`.
+        It then waits for the pooling process to terminate using the `join()` method.
+        If the pooling process has crashed, it prints a message and terminates the process using the `terminate()` method.
+        After that, it retrieves the raw statistics from the `data_pool_queue` and calculates the statistics per PID using the `calculate_statistics_from_data()` method of the `stat_collector` object.
+        The object stats_per_pid is a dict of Stats objects, where the keys are the PIDs and the values are the corresponding Stats objects.
+        """
+        # Send a signal to stop the pooling process
+        self.stop_queue.put("STOP")
+        self.pooling_process.join()  # type: ignore
+        has_process_crashed = self.has_process_crashed(self.success_queue)
+        if has_process_crashed:
+            print("Process pooling has crashed")
+            self.pooling_process.terminate()  # type: ignore
+
+        pooling_raw_stats: Dict[int, RawStats] = self.data_pool_queue.get()
+
+        self.stats_per_pid = self.stat_collector.calculate_statistics_from_data(pooling_raw_stats)
+
+        # Clean queues and process
+        self.stop_queue.close()
+        self.data_pool_queue.close()
+        self.success_queue.close()
+        delattr(self, "stop_queue")
+        delattr(self, "data_pool_queue")
+        delattr(self, "success_queue")
+        delattr(self, "pooling_process")
+
+    def pool_stats(self):
+        """
+        Collects statistics about CPU and RAM usage and IO counters for the process and its children.
+        It uses queues to pass the data:
+            data_pool_queue (Queue): A queue to store the collected statistics as a dict of RawStats.
+            stop_queue (Queue): A queue to receive stop signals.
+            success_queue (Queue): A queue to communicate success or failure.
+        """
+        refresh_rate: float = 0.1  # Initial refresh rate
+        max_refresh_rate: int = 5  # Maximum refresh rate
+        time_elapsed: float = 0.0
+        stats: Dict[int, RawStats] = {}
+
+        while True:
+
+            stats = self.stat_collector.collect_cpu_ram_stats(
+                stats, self.find_children, refresh_rate, self.success_queue
+            )
+            if not self.stop_queue.empty():
+                message = self.stop_queue.get()
+                if message == "STOP":
+                    stats = self.stat_collector.collect_io_counters(stats, self.find_children, self.success_queue)
+                    self.data_pool_queue.put(stats)
+                    break
+            time.sleep(refresh_rate)
+            time_elapsed += refresh_rate
+            if time_elapsed > 10:
+                if refresh_rate < max_refresh_rate:
+                    refresh_rate = min(refresh_rate * 2, max_refresh_rate)
+                    # Double the refresh rate, but do not exceed max_refresh_rate
+                time_elapsed = 0.0
+
+    def calculate_delta(self, other: Self):
+        """
+        Calculate the difference between the current instance's stats_per_pid and another instance's stats_per_pid.
+
+        Args:
+            other (Self): The other instance to compare stats_per_pid with.
+        """
+        subtracted_stats: Dict[int, Stats] = self.stat_collector.subtract_stats(self.stats_per_pid, other.stats_per_pid)
+        self.formated_stats: Stats = self.stat_collector.get_final_stats(subtracted_stats)
+
+    def get_data(self):
+        """
+        Retrieves the formatted statistics from the `formated_stats` attribute of the current instance.
+        Returns:
+            The formatted statistics as a `Stats` object.
+        """
+        return self.formated_stats
+
+    def print(self, verbose: bool, func_name: str, args: tuple, kwargs: dict) -> None:
+        """
+        Prints the metrit data for a given function.
+
+        Parameters:
+            verbose (bool): If True, prints detailed information about the metrit data. If False, prints a concise summary.
+            func_name (str): The name of the function.
+            args (tuple): The positional arguments passed to the function.
+            kwargs (dict): The keyword arguments passed to the function.
+
+        Returns:
+            None
+        """
+        data: Stats = self.formated_stats
+        if verbose:
+            print("*" * 5, f"metrit data for function {func_name}:", "*" * 5)
+            print(f"\tArgs: {args}.")
+            print(f"\tKwargs: {kwargs}.")
+            print(f"Maximum CPU usage: {data.cpu_percentage_max:.2f}%.")
+            print(f"Average CPU usage: {data.cpu_percentage_avg:.2f}%.")
+            print(f"Average memory usage: {data.memory_percentage_avg:.2f}%.")
+            print(f"Maximum RSS memory usage: {format_size(data.rss_bytes_max)}.")
+            print(f"Average RSS memory usage: {format_size(data.rss_bytes_avg)}.")
+            print(f"Maximum VMS memory usage: {format_size(data.vms_bytes_max)}.")
+            print(f"Average VMS memory usage: {format_size(data.vms_bytes_avg)}.")
+
+            if platform != "darwin":
+                print(f"IO read count: {data.read_count}.")
+                print(f"IO writes count: {data.write_count}.")
+                print(f"IO read bytes: {format_size(data.read_bytes)}.")
+                print(f"IO write bytes: {format_size(data.write_bytes)}.")
+            print("*" * 5, "End of metrit data.", "*" * 5)
+        else:
+            func_name_spacing = 30
+            func_name = f"'{func_name}'"
+            if len(func_name) > func_name_spacing:
+                func_name = func_name[: func_name_spacing - 4] + "..." + "'"
+            if platform != "darwin":
+                output_format = "Function {:30} {:>8} avg of memory {:>8.2f}% avg of CPU {:>8} IO reads {:>8} IO writes"
+                output = output_format.format(
+                    func_name,
+                    format_size(data.rss_bytes_avg),
+                    data.cpu_percentage_avg,
+                    format_size(data.read_bytes),
+                    format_size(data.write_bytes),
+                )
+            else:
+                output_format = "Function {:30} {:>8} avg of memory {:>8.2f}% avg of CPU"
+                output = output_format.format(func_name, format_size(data.rss_bytes_avg), data.cpu_percentage_avg)
+            print(output)
```

### Comparing `metrit-0.0.1/metrit/StatCollector.py` & `metrit-0.0.3/metrit/StatCollector.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-from statistics import mean
-from sys import platform
-from typing import Dict, Tuple
-
-import psutil
-from multiprocess import Queue, current_process
-
-from .Stats import RawStats, Stats
-
-
-class StatCollector:
-    def __init__(self, pid):
-        """
-        Initializes a new instance of the StatCollector class.
-        Args:
-            pid (int): The process ID of the process to collect stats for.
-        Returns:
-            None
-        """
-        self.pid = pid
-        self.stats = {}
-
-    def collect_cpu_ram_stats(
-        self, stats: Dict, find_children: bool, refresh_rate: float, sucesss_queue: Queue
-    ) -> Dict[int, RawStats]:
-        """
-        Collects current CPU and RAM stats for the process and its children.
-
-        Args:
-            stats (Dict): A dictionary to store the collected stats as {pid: RawStats}.
-            find_children (bool): Whether to collect stats for the process's children.
-            refresh_rate (float): The refresh rate for collecting stats.
-            sucesss_queue (Queue): A queue to indicate the success of stats collection.
-
-        Returns:
-            Dict: The updated dictionary containing the collected stats as {pid: RawStats}.
-
-        Raises:
-            Exception: If there is an error collecting the stats.
-        """
-        # Collect current CPU and RAM stats for the process and its children
-        try:
-            cpu_percent, memory_percent, rss_bytes, vms_bytes = self.get_current_stats(self.pid, refresh_rate)
-            if self.pid not in stats:
-                stats[self.pid] = RawStats()
-            stats[self.pid].cpu_percent.append(cpu_percent)
-            stats[self.pid].memory_percent.append(memory_percent)
-            stats[self.pid].rss_bytes.append(rss_bytes)
-            stats[self.pid].vms_bytes.append(vms_bytes)
-            if find_children:
-
-                for child in psutil.Process(self.pid).children(recursive=True):
-                    try:
-                        if child.pid == current_process().pid:  # Avoid counting the current process
-                            continue
-                        cpu_percent, memory_percent, rss_bytes, vms_bytes = self.get_current_stats(
-                            child.pid, refresh_rate
-                        )
-                        if child.pid not in stats:
-                            stats[child.pid] = RawStats()
-                        stats[child.pid].cpu_percent.append(cpu_percent)
-                        stats[child.pid].memory_percent.append(memory_percent)
-                        stats[child.pid].rss_bytes.append(rss_bytes)
-                        stats[child.pid].vms_bytes.append(vms_bytes)
-                    except Exception:
-                        if child.pid in stats:
-                            del stats[child.pid]
-                        continue  # It is possible for some children processes to not exist, so we skip them
-
-            sucesss_queue.put(True)
-        except Exception as e:
-            print(f"Error collecting cpu and ram stats: {e}")
-            sucesss_queue.put(False)
-        finally:
-            return stats
-
-    @staticmethod
-    def get_current_stats(pid: int, refresh_rate: float) -> Tuple[float, float, int, int]:
-        """
-        Get the current CPU and memory usage statistics for a given process ID (PID).
-
-        Parameters:
-            pid (int): The process ID (PID) of the process to get the stats for.
-            refresh_rate (float): The interval (in seconds) to refresh the CPU usage.
-
-        Returns:
-            Tuple[float, float, int, int]: A tuple containing the CPU percentage, memory percentage, RSS (resident set size) in bytes, and VMS (virtual memory size) in bytes.
-
-         Note:
-            - The CPU percentage is calculated using `psutil.Process.cpu_percent()` with the given `refresh_rate`.
-            - The memory information is obtained using `psutil.Process.as_dict()` with the attributes "memory_info" and "memory_percent".
-            - If there is an error getting the stats, the function returns 0.0 for CPU and memory percentages, and 0 for RSS and VMS.
-        """
-        # Use psutil to get the stats for a given PID
-        try:
-            p = psutil.Process(pid)
-            cpu_percent = p.cpu_percent(interval=refresh_rate)
-            memory_info = p.as_dict(attrs=["memory_info", "memory_percent"])
-            memory_percent = memory_info["memory_percent"]
-            rss_bytes = memory_info["memory_info"].rss
-            vms_bytes = memory_info["memory_info"].vms
-        except Exception:
-            # print(f"Error getting cpu and ram stats for PID {pid}. {e}")
-            return 0.0, 0.0, 0, 0
-        return cpu_percent, memory_percent, rss_bytes, vms_bytes
-
-    def collect_io_counters(self, stats, find_children: bool, sucesss_queue: Queue) -> Dict[int, RawStats]:
-        """
-        Collects IO stats for the process and its children.
-
-        Args:
-            stats (Dict): A dictionary to store the collected stats.
-            find_children (bool): Whether to collect stats for the process's children.
-            sucesss_queue (Queue): A queue to communicate success or failure.
-
-        Returns:
-            Dict: The updated stats dictionary in form of {pid: RawStats}.
-
-        Note:
-            - If the platform is "darwin" (macos), the function returns the stats dictionary as is since IO stats are not supported for macOS.
-            - The IO stats for the process and its children are collected using `self.get_io_counters()`.
-            - The stats are stored in the `stats` dictionary with the process ID as the key.
-            - If `find_children` is True, the function iterates over the process's children and collects their IO stats.
-            - If a child process does not exist, it is skipped.
-            - The function puts True in the `sucesss_queue` if the stats collection is successful, False otherwise.
-            - If there is an exception during the stats an error message is printed and False is put in the `sucesss_queue`.
-        """
-        if platform == "darwin":
-            return stats
-        # Collect IO stats for the process and its children
-        try:
-            io_read_count, io_write_count, io_read_bytes, io_write_bytes = self.get_io_counters(self.pid)
-            if self.pid not in stats:
-                stats[self.pid] = RawStats()
-            stats[self.pid].io_read_count = io_read_count
-            stats[self.pid].io_write_count = io_write_count
-            stats[self.pid].io_read_bytes = io_read_bytes
-            stats[self.pid].io_write_bytes = io_write_bytes
-
-            if find_children:
-                for child in psutil.Process(self.pid).children(recursive=True):
-                    try:
-                        if child.pid == current_process().pid:  # Avoid counting the current process
-                            continue
-                        io_read_count, io_write_count, io_read_bytes, io_write_bytes = self.get_io_counters(child.pid)
-                        if child.pid not in stats:
-                            stats[child.pid] = RawStats()
-                        stats[child.pid].io_read_count = io_read_count
-                        stats[child.pid].io_write_count = io_write_count
-                        stats[child.pid].io_read_bytes = io_read_bytes
-                        stats[child.pid].io_write_bytes = io_write_bytes
-                    except Exception:
-                        if child.pid in stats:
-                            del stats[child.pid]
-                        continue  # It is possible for some children processes to not exist, so we skip them
-
-            sucesss_queue.put(True)
-        except Exception as e:
-            print(f"Error collecting io stats: {e}")
-            sucesss_queue.put(False)
-        finally:
-            return stats
-
-    @staticmethod
-    def get_io_counters(pid: int) -> Tuple[int, int, int, int]:
-        """
-        Get the IO counters for a given process ID.
-
-        Args:
-            pid (int): The process ID of the process to get the IO counters for.
-
-        Returns:
-            Tuple[int, int, int, int]: A tuple containing the read count, write count, read bytes, and write bytes of the process's IO counters.
-
-        Note:
-            If there is an error getting the stats for the process ID, the function returns 0 for all counters.
-        """
-        try:
-            p = psutil.Process(pid)
-        except Exception:
-            print(f"Error getting stats for PID {pid}")
-            return 0, 0, 0, 0
-        io_counters = p.io_counters()  # type: ignore
-        return io_counters.read_count, io_counters.write_count, io_counters.read_bytes, io_counters.write_bytes
-
-    def calculate_statistics_from_data(self, raw_stats: Dict[int, RawStats]) -> Dict[int, Stats]:
-        """
-        Calculate statistics from the given raw statistics data.
-        Args:
-            raw_stats (Dict[int, RawStats]): A dictionary containing the raw statistics data, where the keys are process IDs and the values are RawStats objects.
-        Returns:
-            Dict[int, Stats]: A dictionary containing the calculated statistics, where the keys are process IDs and the values are Stats objects. Only the statistics for non-empty RawStats objects are included.
-        """
-        return {pid: self.calculate_statistics(pid_data) for pid, pid_data in raw_stats.items() if pid_data}
-
-    @staticmethod
-    def calculate_statistics(data: RawStats) -> Stats:
-        """
-        Calculates the maximum CPU percentage, average CPU percentage, average memory percentage, average RSS bytes,
-        maximum RSS bytes, average VMS bytes, maximum VMS bytes, write count, read count, write bytes,
-        and read bytes from the given RawStats object.
-
-        Args:
-            data (RawStats): The data to calculate statistics from.
-
-        Returns:
-            Stats: The calculated statistics.
-
-        """
-        return Stats(
-            cpu_percentage_max=max(data.cpu_percent) if data.cpu_percent else 0.0,
-            cpu_percentage_avg=mean(data.cpu_percent) if data.cpu_percent else 0.0,
-            memory_percentage_avg=mean(data.memory_percent) if data.memory_percent else 0.0,
-            rss_bytes_avg=mean(data.rss_bytes) if data.rss_bytes else 0.0,
-            rss_bytes_max=max(data.rss_bytes) if data.rss_bytes else 0,
-            vms_bytes_avg=mean(data.vms_bytes) if data.vms_bytes else 0.0,
-            vms_bytes_max=max(data.vms_bytes) if data.vms_bytes else 0,
-            write_count=data.io_write_count if data.io_write_count is not None else 0,
-            read_count=data.io_read_count if data.io_read_count is not None else 0,
-            write_bytes=data.io_write_bytes if data.io_write_bytes is not None else 0,
-            read_bytes=data.io_read_bytes if data.io_read_bytes is not None else 0,
-        )
-
-    @staticmethod
-    def subtract_stats(main: Dict[int, Stats], other: Dict[int, Stats]) -> Dict[int, Stats]:
-        """
-        Subtracts the statistics from the `other` dictionary from the statistics in the `main` dictionary.
-
-        Args:
-            main (Dict[int, Stats]): A dictionary mapping process IDs to their respective statistics.
-            other (Dict[int, Stats]): A dictionary mapping process IDs to their respective statistics.
-
-        Returns:
-            Dict[int, Stats]: A dictionary mapping process IDs to their respective statistics after subtraction.
-
-        The function subtracts the statistics from the `other` dictionary from the statistics in the `main` dictionary.
-        It iterates over the process IDs in the `main` dictionary and checks if the corresponding process ID exists in the `other` dictionary.
-        If it does, it subtracts the statistics from the `other` dictionary from the statistics in the `main` dictionary.
-        The resulting statistics are stored in the `result` dictionary.
-        If the corresponding process ID does not exist in the `other` dictionary, the statistics from the `main` dictionary are copied to the `result` dictionary.
-        Finally, the function returns the `result` dictionary.
-
-        Note:
-            - The CPU statistics are not subtracted.
-            - The statistics are subtracted element-wise, and the resulting values are capped at 0.0 for floating-point values and 0 for integer values.
-        """
-        result = {}
-        if not main:
-            return result
-        for pid, stats_main in main.items():
-            if pid in other:
-                stats_b = other[pid]
-                subtracted_stats = Stats(
-                    # cpu is not subtracted
-                    cpu_percentage_max=stats_main.cpu_percentage_max,
-                    cpu_percentage_avg=stats_main.cpu_percentage_avg,
-                    memory_percentage_avg=max(stats_main.memory_percentage_avg - stats_b.memory_percentage_avg, 0.0),
-                    rss_bytes_avg=max(stats_main.rss_bytes_avg - stats_b.rss_bytes_avg, 0.0),
-                    rss_bytes_max=max(stats_main.rss_bytes_max - stats_b.rss_bytes_max, 0),
-                    vms_bytes_avg=max(stats_main.vms_bytes_avg - stats_b.vms_bytes_avg, 0.0),
-                    vms_bytes_max=max(stats_main.vms_bytes_max - stats_b.vms_bytes_max, 0),
-                    write_count=max(stats_main.write_count - stats_b.write_count, 0),
-                    read_count=max(stats_main.read_count - stats_b.read_count, 0),
-                    write_bytes=max(stats_main.write_bytes - stats_b.write_bytes, 0),
-                    read_bytes=max(stats_main.read_bytes - stats_b.read_bytes, 0),
-                )
-                result[pid] = subtracted_stats
-            else:
-                result[pid] = stats_main
-
-        return result
-
-    @staticmethod
-    def get_final_stats(stats: Dict[int, Stats]):
-        """
-        Calculates the final statistics by summing up the statistics of all processes.
-        Args:
-            stats (Dict[int, Stats]): A dictionary mapping process IDs to their respective statistics.
-        Returns:
-            Stats: The final statistics.
-        This function iterates over all the statistics in the `stats` dictionary and sums up their respective values.
-        The final statistics are stored in the `final_stats` object, which is then returned.
-        If the `stats` dictionary is empty, an empty `Stats` object is returned.
-        """
-        final_stats = Stats()
-        if not stats:
-            return final_stats
-        for _, stat in stats.items():
-            final_stats.cpu_percentage_max += stat.cpu_percentage_max
-            final_stats.cpu_percentage_avg += stat.cpu_percentage_avg
-            final_stats.memory_percentage_avg += stat.memory_percentage_avg
-            final_stats.rss_bytes_avg += stat.rss_bytes_avg
-            final_stats.rss_bytes_max += stat.rss_bytes_max
-            final_stats.vms_bytes_avg += stat.vms_bytes_avg
-            final_stats.vms_bytes_max += stat.vms_bytes_max
-            final_stats.write_count += stat.write_count
-            final_stats.read_count += stat.read_count
-            final_stats.write_bytes += stat.write_bytes
-            final_stats.read_bytes += stat.read_bytes
-        return final_stats
+from statistics import mean
+from sys import platform
+from typing import Dict, Tuple
+
+import psutil
+from multiprocess import Queue, current_process
+
+from .Stats import RawStats, Stats
+
+
+class StatCollector:
+    def __init__(self, pid):
+        """
+        Initializes a new instance of the StatCollector class.
+        Args:
+            pid (int): The process ID of the process to collect stats for.
+        Returns:
+            None
+        """
+        self.pid = pid
+        self.stats = {}
+
+    def collect_cpu_ram_stats(
+        self, stats: Dict, find_children: bool, refresh_rate: float, sucesss_queue: Queue
+    ) -> Dict[int, RawStats]:
+        """
+        Collects current CPU and RAM stats for the process and its children.
+
+        Args:
+            stats (Dict): A dictionary to store the collected stats as {pid: RawStats}.
+            find_children (bool): Whether to collect stats for the process's children.
+            refresh_rate (float): The refresh rate for collecting stats.
+            sucesss_queue (Queue): A queue to indicate the success of stats collection.
+
+        Returns:
+            Dict: The updated dictionary containing the collected stats as {pid: RawStats}.
+
+        Raises:
+            Exception: If there is an error collecting the stats.
+        """
+        # Collect current CPU and RAM stats for the process and its children
+        try:
+            cpu_percent, memory_percent, rss_bytes, vms_bytes = self.get_current_stats(self.pid, refresh_rate)
+            if self.pid not in stats:
+                stats[self.pid] = RawStats()
+            stats[self.pid].cpu_percent.append(cpu_percent)
+            stats[self.pid].memory_percent.append(memory_percent)
+            stats[self.pid].rss_bytes.append(rss_bytes)
+            stats[self.pid].vms_bytes.append(vms_bytes)
+            if find_children:
+
+                for child in psutil.Process(self.pid).children(recursive=True):
+                    try:
+                        if child.pid == current_process().pid:  # Avoid counting the current process
+                            continue
+                        cpu_percent, memory_percent, rss_bytes, vms_bytes = self.get_current_stats(
+                            child.pid, refresh_rate
+                        )
+                        if child.pid not in stats:
+                            stats[child.pid] = RawStats()
+                        stats[child.pid].cpu_percent.append(cpu_percent)
+                        stats[child.pid].memory_percent.append(memory_percent)
+                        stats[child.pid].rss_bytes.append(rss_bytes)
+                        stats[child.pid].vms_bytes.append(vms_bytes)
+                    except Exception:
+                        if child.pid in stats:
+                            del stats[child.pid]
+                        continue  # It is possible for some children processes to not exist, so we skip them
+
+            sucesss_queue.put(True)
+        except Exception as e:
+            print(f"Error collecting cpu and ram stats: {e}")
+            sucesss_queue.put(False)
+        finally:
+            return stats
+
+    @staticmethod
+    def get_current_stats(pid: int, refresh_rate: float) -> Tuple[float, float, int, int]:
+        """
+        Get the current CPU and memory usage statistics for a given process ID (PID).
+
+        Parameters:
+            pid (int): The process ID (PID) of the process to get the stats for.
+            refresh_rate (float): The interval (in seconds) to refresh the CPU usage.
+
+        Returns:
+            Tuple[float, float, int, int]: A tuple containing the CPU percentage, memory percentage, RSS (resident set size) in bytes, and VMS (virtual memory size) in bytes.
+
+         Note:
+            - The CPU percentage is calculated using `psutil.Process.cpu_percent()` with the given `refresh_rate`.
+            - The memory information is obtained using `psutil.Process.as_dict()` with the attributes "memory_info" and "memory_percent".
+            - If there is an error getting the stats, the function returns 0.0 for CPU and memory percentages, and 0 for RSS and VMS.
+        """
+        # Use psutil to get the stats for a given PID
+        try:
+            p = psutil.Process(pid)
+            cpu_percent = p.cpu_percent(interval=refresh_rate)
+            memory_info = p.as_dict(attrs=["memory_info", "memory_percent"])
+            memory_percent = memory_info["memory_percent"]
+            rss_bytes = memory_info["memory_info"].rss
+            vms_bytes = memory_info["memory_info"].vms
+        except Exception:
+            # print(f"Error getting cpu and ram stats for PID {pid}. {e}")
+            return 0.0, 0.0, 0, 0
+        return cpu_percent, memory_percent, rss_bytes, vms_bytes
+
+    def collect_io_counters(self, stats, find_children: bool, sucesss_queue: Queue) -> Dict[int, RawStats]:
+        """
+        Collects IO stats for the process and its children.
+
+        Args:
+            stats (Dict): A dictionary to store the collected stats.
+            find_children (bool): Whether to collect stats for the process's children.
+            sucesss_queue (Queue): A queue to communicate success or failure.
+
+        Returns:
+            Dict: The updated stats dictionary in form of {pid: RawStats}.
+
+        Note:
+            - If the platform is "darwin" (macos), the function returns the stats dictionary as is since IO stats are not supported for macOS.
+            - The IO stats for the process and its children are collected using `self.get_io_counters()`.
+            - The stats are stored in the `stats` dictionary with the process ID as the key.
+            - If `find_children` is True, the function iterates over the process's children and collects their IO stats.
+            - If a child process does not exist, it is skipped.
+            - The function puts True in the `sucesss_queue` if the stats collection is successful, False otherwise.
+            - If there is an exception during the stats an error message is printed and False is put in the `sucesss_queue`.
+        """
+        if platform == "darwin":
+            return stats
+        # Collect IO stats for the process and its children
+        try:
+            io_read_count, io_write_count, io_read_bytes, io_write_bytes = self.get_io_counters(self.pid)
+            if self.pid not in stats:
+                stats[self.pid] = RawStats()
+            stats[self.pid].io_read_count = io_read_count
+            stats[self.pid].io_write_count = io_write_count
+            stats[self.pid].io_read_bytes = io_read_bytes
+            stats[self.pid].io_write_bytes = io_write_bytes
+
+            if find_children:
+                for child in psutil.Process(self.pid).children(recursive=True):
+                    try:
+                        if child.pid == current_process().pid:  # Avoid counting the current process
+                            continue
+                        io_read_count, io_write_count, io_read_bytes, io_write_bytes = self.get_io_counters(child.pid)
+                        if child.pid not in stats:
+                            stats[child.pid] = RawStats()
+                        stats[child.pid].io_read_count = io_read_count
+                        stats[child.pid].io_write_count = io_write_count
+                        stats[child.pid].io_read_bytes = io_read_bytes
+                        stats[child.pid].io_write_bytes = io_write_bytes
+                    except Exception:
+                        if child.pid in stats:
+                            del stats[child.pid]
+                        continue  # It is possible for some children processes to not exist, so we skip them
+
+            sucesss_queue.put(True)
+        except Exception as e:
+            print(f"Error collecting io stats: {e}")
+            sucesss_queue.put(False)
+        finally:
+            return stats
+
+    @staticmethod
+    def get_io_counters(pid: int) -> Tuple[int, int, int, int]:
+        """
+        Get the IO counters for a given process ID.
+
+        Args:
+            pid (int): The process ID of the process to get the IO counters for.
+
+        Returns:
+            Tuple[int, int, int, int]: A tuple containing the read count, write count, read bytes, and write bytes of the process's IO counters.
+
+        Note:
+            If there is an error getting the stats for the process ID, the function returns 0 for all counters.
+        """
+        try:
+            p = psutil.Process(pid)
+        except Exception:
+            print(f"Error getting stats for PID {pid}")
+            return 0, 0, 0, 0
+        io_counters = p.io_counters()  # type: ignore
+        return io_counters.read_count, io_counters.write_count, io_counters.read_bytes, io_counters.write_bytes
+
+    def calculate_statistics_from_data(self, raw_stats: Dict[int, RawStats]) -> Dict[int, Stats]:
+        """
+        Calculate statistics from the given raw statistics data.
+        Args:
+            raw_stats (Dict[int, RawStats]): A dictionary containing the raw statistics data, where the keys are process IDs and the values are RawStats objects.
+        Returns:
+            Dict[int, Stats]: A dictionary containing the calculated statistics, where the keys are process IDs and the values are Stats objects. Only the statistics for non-empty RawStats objects are included.
+        """
+        return {pid: self.calculate_statistics(pid_data) for pid, pid_data in raw_stats.items() if pid_data}
+
+    @staticmethod
+    def calculate_statistics(data: RawStats) -> Stats:
+        """
+        Calculates the maximum CPU percentage, average CPU percentage, average memory percentage, average RSS bytes,
+        maximum RSS bytes, average VMS bytes, maximum VMS bytes, write count, read count, write bytes,
+        and read bytes from the given RawStats object.
+
+        Args:
+            data (RawStats): The data to calculate statistics from.
+
+        Returns:
+            Stats: The calculated statistics.
+
+        """
+        return Stats(
+            cpu_percentage_max=max(data.cpu_percent) if data.cpu_percent else 0.0,
+            cpu_percentage_avg=mean(data.cpu_percent) if data.cpu_percent else 0.0,
+            memory_percentage_avg=mean(data.memory_percent) if data.memory_percent else 0.0,
+            rss_bytes_avg=mean(data.rss_bytes) if data.rss_bytes else 0.0,
+            rss_bytes_max=max(data.rss_bytes) if data.rss_bytes else 0,
+            vms_bytes_avg=mean(data.vms_bytes) if data.vms_bytes else 0.0,
+            vms_bytes_max=max(data.vms_bytes) if data.vms_bytes else 0,
+            write_count=data.io_write_count if data.io_write_count is not None else 0,
+            read_count=data.io_read_count if data.io_read_count is not None else 0,
+            write_bytes=data.io_write_bytes if data.io_write_bytes is not None else 0,
+            read_bytes=data.io_read_bytes if data.io_read_bytes is not None else 0,
+        )
+
+    @staticmethod
+    def subtract_stats(main: Dict[int, Stats], other: Dict[int, Stats]) -> Dict[int, Stats]:
+        """
+        Subtracts the statistics from the `other` dictionary from the statistics in the `main` dictionary.
+
+        Args:
+            main (Dict[int, Stats]): A dictionary mapping process IDs to their respective statistics.
+            other (Dict[int, Stats]): A dictionary mapping process IDs to their respective statistics.
+
+        Returns:
+            Dict[int, Stats]: A dictionary mapping process IDs to their respective statistics after subtraction.
+
+        The function subtracts the statistics from the `other` dictionary from the statistics in the `main` dictionary.
+        It iterates over the process IDs in the `main` dictionary and checks if the corresponding process ID exists in the `other` dictionary.
+        If it does, it subtracts the statistics from the `other` dictionary from the statistics in the `main` dictionary.
+        The resulting statistics are stored in the `result` dictionary.
+        If the corresponding process ID does not exist in the `other` dictionary, the statistics from the `main` dictionary are copied to the `result` dictionary.
+        Finally, the function returns the `result` dictionary.
+
+        Note:
+            - The CPU statistics are not subtracted.
+            - The statistics are subtracted element-wise, and the resulting values are capped at 0.0 for floating-point values and 0 for integer values.
+        """
+        result = {}
+        if not main:
+            return result
+        for pid, stats_main in main.items():
+            if pid in other:
+                stats_b = other[pid]
+                subtracted_stats = Stats(
+                    # cpu is not subtracted
+                    cpu_percentage_max=stats_main.cpu_percentage_max,
+                    cpu_percentage_avg=stats_main.cpu_percentage_avg,
+                    memory_percentage_avg=max(stats_main.memory_percentage_avg - stats_b.memory_percentage_avg, 0.0),
+                    rss_bytes_avg=max(stats_main.rss_bytes_avg - stats_b.rss_bytes_avg, 0.0),
+                    rss_bytes_max=max(stats_main.rss_bytes_max - stats_b.rss_bytes_max, 0),
+                    vms_bytes_avg=max(stats_main.vms_bytes_avg - stats_b.vms_bytes_avg, 0.0),
+                    vms_bytes_max=max(stats_main.vms_bytes_max - stats_b.vms_bytes_max, 0),
+                    write_count=max(stats_main.write_count - stats_b.write_count, 0),
+                    read_count=max(stats_main.read_count - stats_b.read_count, 0),
+                    write_bytes=max(stats_main.write_bytes - stats_b.write_bytes, 0),
+                    read_bytes=max(stats_main.read_bytes - stats_b.read_bytes, 0),
+                )
+                result[pid] = subtracted_stats
+            else:
+                result[pid] = stats_main
+
+        return result
+
+    @staticmethod
+    def get_final_stats(stats: Dict[int, Stats]):
+        """
+        Calculates the final statistics by summing up the statistics of all processes.
+        Args:
+            stats (Dict[int, Stats]): A dictionary mapping process IDs to their respective statistics.
+        Returns:
+            Stats: The final statistics.
+        This function iterates over all the statistics in the `stats` dictionary and sums up their respective values.
+        The final statistics are stored in the `final_stats` object, which is then returned.
+        If the `stats` dictionary is empty, an empty `Stats` object is returned.
+        """
+        final_stats = Stats()
+        if not stats:
+            return final_stats
+        for _, stat in stats.items():
+            final_stats.cpu_percentage_max += stat.cpu_percentage_max
+            final_stats.cpu_percentage_avg += stat.cpu_percentage_avg
+            final_stats.memory_percentage_avg += stat.memory_percentage_avg
+            final_stats.rss_bytes_avg += stat.rss_bytes_avg
+            final_stats.rss_bytes_max += stat.rss_bytes_max
+            final_stats.vms_bytes_avg += stat.vms_bytes_avg
+            final_stats.vms_bytes_max += stat.vms_bytes_max
+            final_stats.write_count += stat.write_count
+            final_stats.read_count += stat.read_count
+            final_stats.write_bytes += stat.write_bytes
+            final_stats.read_bytes += stat.read_bytes
+        return final_stats
```

### Comparing `metrit-0.0.1/metrit/core.py` & `metrit-0.0.3/metrit/core.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,254 +1,254 @@
-import inspect
-from collections import deque
-from functools import partial, wraps
-from typing import Any, Callable, Dict, Tuple
-
-from metrit.Monitoring import Monitoring
-from metrit.utils import check_is_recursive_func, extract_callable_and_args_if_method
-
-
-class MetritConfig:
-    ACTIVE: bool = True
-
-
-def metrit(*args: Any, verbose: bool = False, find_children: bool = False, isolate: bool = False) -> Callable:
-    """
-    Decorator function that measures the cpu, ram and io footprint of a given function in the current process. It can be called like @metrit or using arguments @metrit(...)
-
-    Args:
-        args: contains the function to be decorated if no arguments are provided when calling the decorator
-        verbose (bool, optional): Whether to print detailed information after execution. Defaults to False.
-        isolate (bool, optional): If True, encapsulates the function in its own process. Defaults to False.
-
-    Returns:
-        Callable: The decorated function if arguments are provided, otherwise a partial function.
-                    If the callable is a class it will be returned unmodified and will not be decorated.
-                    If the MetritConfig ACTIVE flag is set to false, the callable will be returned without modification and will not be decorated.
-
-    Raises:
-        Exception: If the function crashes, it will raise the exception given by the user's function.
-
-    Notes:
-        - Processes spawned inside the decorated function won't be measured
-        - This decorator also checks for recursion automatically even though is better to wrap the recursive function in another function and apply the @metrit decorator to the new function.
-        - Recursive functions shouldn't use the isolate argument since recursion cannot be measured.
-        - Classes will be returned unmodified and will not be decorated.
-        - If the function is a methods won't be isolated.
-        - If isolate==True and it crashes in the process, it will be tried again in the main process.
-
-
-
-    Example:
-        @metrit(verbose=True)
-        def my_function(arg1, arg2):
-            # function body
-
-        @metrit
-        def my_function(arg1, arg2):
-            # function body
-
-        # The decorated function can be used as usual
-        result = my_function(arg1_value, arg2_value)
-    """
-    if not MetritConfig.ACTIVE:
-        # Return the callable unmodified if MetritConfig.ACTIVE is set to False
-        if args:
-            return args[0]
-        else:
-            return lambda f: f
-    if args:  # If arguments are provided, return the decorated function
-        return _decorator(*args)
-    else:
-        return partial(_decorator, verbose=verbose, find_children=find_children, isolate=isolate)
-
-
-def _decorator(func: Callable, verbose: bool = False, find_children: bool = False, isolate: bool = False) -> Callable:
-    """
-    Decorator function that measures the memory and time of a given function.
-    Args:
-        func (Callable): The function to be decorated.
-        verbose (bool, optional): If True, prints detailed information about the function execution. Defaults to False.
-        find_children (bool, optional): If True, measures the memory and time of all child processes spawned by the function. Defaults to False.
-        isolate (bool, optional): If True, encapsulates the function in its own process. Defaults to False.
-
-    Returns:
-        Callable: The decorated function.
-    Raises:
-        Exception: If the function crashes, it will raise the exception given by the user's function.
-    """
-    if inspect.isclass(func):
-        # If a class is found, return the class inmediatly since it could raise an exception if triggered from other processes
-        return func
-
-    potential_recursion_func_stack: deque[Callable] = deque()
-
-    @wraps(func)
-    def metrit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
-        nonlocal potential_recursion_func_stack
-        is_recursive: bool = check_is_recursive_func(func, potential_recursion_func_stack)
-
-        callable_func, args, args_to_print, is_method = extract_callable_and_args_if_method(func, *args)
-        if is_recursive:
-            return handle_recursive_call(callable_func, potential_recursion_func_stack, *args, **kwargs)
-
-        crashed: bool = False
-        # Get the memory footprint before the function is called
-        if isolate and not is_method:
-            try:
-                result, pool_monitor_data = isolate_function(find_children, callable_func, *args, **kwargs)
-            except Exception:
-                crashed = True
-
-        if crashed or not isolate or is_method:
-            result, pool_monitor_data = call_func(find_children, callable_func, *args, **kwargs)
-
-        potential_recursion_func_stack.pop()
-        if not potential_recursion_func_stack:
-            pool_monitor_data.print(verbose, callable_func.__name__, args_to_print, kwargs)
-
-        return result
-
-    return metrit_wrapper
-
-
-def handle_recursive_call(func: Callable, potential_recursion_func_stack: deque, *args: Tuple, **kwargs: Dict) -> Any:
-    """
-    Handle a recursive call by executing the given function with the provided arguments and keyword arguments.
-
-    Parameters:
-        func (Callable): The function to be executed.
-        potential_recursion_func_stack (deque): A stack of potential recursive functions.
-        *args: Variable length argument list.
-        **kwargs: Arbitrary keyword arguments.
-
-    Returns:
-        Any: The result of executing the function.
-    """
-    result: Any = func(*args, **kwargs)
-    potential_recursion_func_stack.pop()
-    return result
-
-
-def call_func(find_children: bool, func: Callable, *args: Tuple, **kwargs: Dict) -> Tuple[Any, Monitoring]:
-    """
-    Calls the given function with the provided arguments and keyword arguments.
-    Monitor the resources used by the function.
-    Returns the result along with the monitoring data.
-
-    Args:
-        find_children (bool): Whether to find children processes.
-        func (Callable): The function to be executed.
-        *args: Variable length argument list.
-        **kwargs: Arbitrary keyword arguments.
-
-    Returns:
-        Tuple[Any, Monitoring]: A tuple containing the result of the function and the monitoring data.
-
-    Raises:
-        Exception: If an exception occurs during the execution of the function.
-    """
-
-    pre_monitor_data = Monitoring(find_children=find_children)
-    pre_monitor_data.take_snapshot()
-
-    pool_monitor_data = Monitoring(find_children=find_children)
-    pool_monitor_data.start_monitoring()
-    try:
-        result: Any = func(*args, **kwargs)
-    except Exception as e:
-        pool_monitor_data.stop_monitoring()
-        import traceback
-
-        traceback.print_exc()
-        raise e
-
-    pool_monitor_data.stop_monitoring()
-    pool_monitor_data.calculate_delta(pre_monitor_data)
-    return result, pool_monitor_data
-
-
-def isolate_function(find_children: bool, func: Callable, *args: Tuple, **kwargs: Dict) -> Tuple[Any, Monitoring]:
-    """
-    Isolates the given function in a separate process and monitors its resource usage.
-    Args:
-        find_children (bool): Whether to find children processes.
-        func (Callable): The function to be executed.
-        *args: Variable length argument list.
-        **kwargs: Arbitrary keyword arguments.
-    Returns:
-        Tuple[Any, Monitoring]: A tuple containing the result of the function and the monitoring data.
-    Raises:
-        Exception: If an exception occurs during the execution of the function.
-        This exception will be handled in the main process and try again the execution and measurement of the function in the main process.
-    """
-    from multiprocess import Process, Queue
-
-    data_queue = Queue()
-    result_queue = Queue()
-    error_queue = Queue()
-    try:
-
-        func_process: Process = Process(
-            target=call_func_isolated,
-            args=(find_children, func, data_queue, result_queue, error_queue, args),
-            kwargs=kwargs,
-        )
-
-        func_process.start()
-        func_process.join()
-        if not error_queue.empty():
-            raise error_queue.get()
-
-        pool_monitor_data = data_queue.get()
-        result = result_queue.get()
-        result_queue.close()
-        data_queue.close()
-
-        return result, pool_monitor_data
-
-    except Exception as e:
-        func_process.join()
-        func_process.terminate()
-        print("Error trying to isolate the process. Trying it again in main process:", e)
-        raise e
-
-
-def call_func_isolated(
-    find_children: bool, func: Callable, data_queue, result_queue, error_queue, args: Tuple, **kwargs: Dict
-):
-    """
-    Executes the given function in a separate process and monitors its resource usage.
-
-    Args:
-        find_children (bool): Whether to find child processes.
-        func (Callable): The function to be executed.
-        data_queue (Queue): The queue to store the monitoring data.
-        result_queue (Queue): The queue to store the result of the function.
-        error_queue (Queue): The queue to store any exceptions that occur during execution.
-        args (Tuple): The positional arguments to be passed to the function.
-        **kwargs (Dict): The keyword arguments to be passed to the function.
-
-    Returns:
-        None
-
-    Raises:
-        Exception: If an exception occurs during the execution of the function.
-            The exception is put into the error_queue.
-
-    """
-    pre_monitor_data = Monitoring(find_children=find_children)
-    pre_monitor_data.take_snapshot()
-    pool_monitor_data = Monitoring(find_children=find_children)
-    pool_monitor_data.start_monitoring()
-
-    try:
-        result: Any = func(*args, **kwargs)
-    except Exception as e:
-        pool_monitor_data.stop_monitoring()
-        error_queue.put(e)
-        return
-
-    pool_monitor_data.stop_monitoring()
-    pool_monitor_data.calculate_delta(pre_monitor_data)
-    data_queue.put(pool_monitor_data)
-    result_queue.put(result)
+import inspect
+from collections import deque
+from functools import partial, wraps
+from typing import Any, Callable, Dict, Tuple
+
+from metrit.Monitoring import Monitoring
+from metrit.utils import check_is_recursive_func, extract_callable_and_args_if_method
+
+
+class MetritConfig:
+    ACTIVE: bool = True
+
+
+def metrit(*args: Any, verbose: bool = False, find_children: bool = False, isolate: bool = False) -> Callable:
+    """
+    Decorator function that measures the cpu, ram and io footprint of a given function in the current process. It can be called like @metrit or using arguments @metrit(...)
+
+    Args:
+        args: contains the function to be decorated if no arguments are provided when calling the decorator
+        verbose (bool, optional): Whether to print detailed information after execution. Defaults to False.
+        isolate (bool, optional): If True, encapsulates the function in its own process. Defaults to False.
+
+    Returns:
+        Callable: The decorated function if arguments are provided, otherwise a partial function.
+                    If the callable is a class it will be returned unmodified and will not be decorated.
+                    If the MetritConfig ACTIVE flag is set to false, the callable will be returned without modification and will not be decorated.
+
+    Raises:
+        Exception: If the function crashes, it will raise the exception given by the user's function.
+
+    Notes:
+        - Processes spawned inside the decorated function won't be measured
+        - This decorator also checks for recursion automatically even though is better to wrap the recursive function in another function and apply the @metrit decorator to the new function.
+        - Recursive functions shouldn't use the isolate argument since recursion cannot be measured.
+        - Classes will be returned unmodified and will not be decorated.
+        - If the function is a methods won't be isolated.
+        - If isolate==True and it crashes in the process, it will be tried again in the main process.
+
+
+
+    Example:
+        @metrit(verbose=True)
+        def my_function(arg1, arg2):
+            # function body
+
+        @metrit
+        def my_function(arg1, arg2):
+            # function body
+
+        # The decorated function can be used as usual
+        result = my_function(arg1_value, arg2_value)
+    """
+    if not MetritConfig.ACTIVE:
+        # Return the callable unmodified if MetritConfig.ACTIVE is set to False
+        if args:
+            return args[0]
+        else:
+            return lambda f: f
+    if args:  # If arguments are provided, return the decorated function
+        return _decorator(*args)
+    else:
+        return partial(_decorator, verbose=verbose, find_children=find_children, isolate=isolate)
+
+
+def _decorator(func: Callable, verbose: bool = False, find_children: bool = False, isolate: bool = False) -> Callable:
+    """
+    Decorator function that measures the memory and time of a given function.
+    Args:
+        func (Callable): The function to be decorated.
+        verbose (bool, optional): If True, prints detailed information about the function execution. Defaults to False.
+        find_children (bool, optional): If True, measures the memory and time of all child processes spawned by the function. Defaults to False.
+        isolate (bool, optional): If True, encapsulates the function in its own process. Defaults to False.
+
+    Returns:
+        Callable: The decorated function.
+    Raises:
+        Exception: If the function crashes, it will raise the exception given by the user's function.
+    """
+    if inspect.isclass(func):
+        # If a class is found, return the class inmediatly since it could raise an exception if triggered from other processes
+        return func
+
+    potential_recursion_func_stack: deque[Callable] = deque()
+
+    @wraps(func)
+    def metrit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
+        nonlocal potential_recursion_func_stack
+        is_recursive: bool = check_is_recursive_func(func, potential_recursion_func_stack)
+
+        callable_func, args, args_to_print, is_method = extract_callable_and_args_if_method(func, *args)
+        if is_recursive:
+            return handle_recursive_call(callable_func, potential_recursion_func_stack, *args, **kwargs)
+
+        crashed: bool = False
+        # Get the memory footprint before the function is called
+        if isolate and not is_method:
+            try:
+                result, pool_monitor_data = isolate_function(find_children, callable_func, *args, **kwargs)
+            except Exception:
+                crashed = True
+
+        if crashed or not isolate or is_method:
+            result, pool_monitor_data = call_func(find_children, callable_func, *args, **kwargs)
+
+        potential_recursion_func_stack.pop()
+        if not potential_recursion_func_stack:
+            pool_monitor_data.print(verbose, callable_func.__name__, args_to_print, kwargs)
+
+        return result
+
+    return metrit_wrapper
+
+
+def handle_recursive_call(func: Callable, potential_recursion_func_stack: deque, *args: Tuple, **kwargs: Dict) -> Any:
+    """
+    Handle a recursive call by executing the given function with the provided arguments and keyword arguments.
+
+    Parameters:
+        func (Callable): The function to be executed.
+        potential_recursion_func_stack (deque): A stack of potential recursive functions.
+        *args: Variable length argument list.
+        **kwargs: Arbitrary keyword arguments.
+
+    Returns:
+        Any: The result of executing the function.
+    """
+    result: Any = func(*args, **kwargs)
+    potential_recursion_func_stack.pop()
+    return result
+
+
+def call_func(find_children: bool, func: Callable, *args: Tuple, **kwargs: Dict) -> Tuple[Any, Monitoring]:
+    """
+    Calls the given function with the provided arguments and keyword arguments.
+    Monitor the resources used by the function.
+    Returns the result along with the monitoring data.
+
+    Args:
+        find_children (bool): Whether to find children processes.
+        func (Callable): The function to be executed.
+        *args: Variable length argument list.
+        **kwargs: Arbitrary keyword arguments.
+
+    Returns:
+        Tuple[Any, Monitoring]: A tuple containing the result of the function and the monitoring data.
+
+    Raises:
+        Exception: If an exception occurs during the execution of the function.
+    """
+
+    pre_monitor_data = Monitoring(find_children=find_children)
+    pre_monitor_data.take_snapshot()
+
+    pool_monitor_data = Monitoring(find_children=find_children)
+    pool_monitor_data.start_monitoring()
+    try:
+        result: Any = func(*args, **kwargs)
+    except Exception as e:
+        pool_monitor_data.stop_monitoring()
+        import traceback
+
+        traceback.print_exc()
+        raise e
+
+    pool_monitor_data.stop_monitoring()
+    pool_monitor_data.calculate_delta(pre_monitor_data)
+    return result, pool_monitor_data
+
+
+def isolate_function(find_children: bool, func: Callable, *args: Tuple, **kwargs: Dict) -> Tuple[Any, Monitoring]:
+    """
+    Isolates the given function in a separate process and monitors its resource usage.
+    Args:
+        find_children (bool): Whether to find children processes.
+        func (Callable): The function to be executed.
+        *args: Variable length argument list.
+        **kwargs: Arbitrary keyword arguments.
+    Returns:
+        Tuple[Any, Monitoring]: A tuple containing the result of the function and the monitoring data.
+    Raises:
+        Exception: If an exception occurs during the execution of the function.
+        This exception will be handled in the main process and try again the execution and measurement of the function in the main process.
+    """
+    from multiprocess import Process, Queue
+
+    data_queue = Queue()
+    result_queue = Queue()
+    error_queue = Queue()
+    try:
+
+        func_process: Process = Process(
+            target=call_func_isolated,
+            args=(find_children, func, data_queue, result_queue, error_queue, args),
+            kwargs=kwargs,
+        )
+
+        func_process.start()
+        func_process.join()
+        if not error_queue.empty():
+            raise error_queue.get()
+
+        pool_monitor_data = data_queue.get()
+        result = result_queue.get()
+        result_queue.close()
+        data_queue.close()
+
+        return result, pool_monitor_data
+
+    except Exception as e:
+        func_process.join()
+        func_process.terminate()
+        print("Error trying to isolate the process. Trying it again in main process:", e)
+        raise e
+
+
+def call_func_isolated(
+    find_children: bool, func: Callable, data_queue, result_queue, error_queue, args: Tuple, **kwargs: Dict
+):
+    """
+    Executes the given function in a separate process and monitors its resource usage.
+
+    Args:
+        find_children (bool): Whether to find child processes.
+        func (Callable): The function to be executed.
+        data_queue (Queue): The queue to store the monitoring data.
+        result_queue (Queue): The queue to store the result of the function.
+        error_queue (Queue): The queue to store any exceptions that occur during execution.
+        args (Tuple): The positional arguments to be passed to the function.
+        **kwargs (Dict): The keyword arguments to be passed to the function.
+
+    Returns:
+        None
+
+    Raises:
+        Exception: If an exception occurs during the execution of the function.
+            The exception is put into the error_queue.
+
+    """
+    pre_monitor_data = Monitoring(find_children=find_children)
+    pre_monitor_data.take_snapshot()
+    pool_monitor_data = Monitoring(find_children=find_children)
+    pool_monitor_data.start_monitoring()
+
+    try:
+        result: Any = func(*args, **kwargs)
+    except Exception as e:
+        pool_monitor_data.stop_monitoring()
+        error_queue.put(e)
+        return
+
+    pool_monitor_data.stop_monitoring()
+    pool_monitor_data.calculate_delta(pre_monitor_data)
+    data_queue.put(pool_monitor_data)
+    result_queue.put(result)
```

### Comparing `metrit-0.0.1/metrit/utils.py` & `metrit-0.0.3/metrit/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from collections import deque
-from typing import Callable, Tuple
-from warnings import warn
-
-
-def format_size(bytes_size: int | float) -> str:
-    """
-    Converts a size in bytes to a human-readable format.
-    Parameters:
-        bytes_size (int | float): The size in bytes to be converted.
-    Returns:
-        str: The human-read
-    """
-    for unit in ["B", "KB", "MB", "GB", "TB"]:
-        if bytes_size < 1024:
-            if unit == "B":
-                return f"{bytes_size:.0f}{unit}"
-            return f"{bytes_size:.2f}{unit}"
-        bytes_size /= 1024
-    return f"{bytes_size:.2f}PB"  # If it exceeds TB, convert to petabytes
-
-
-def extract_callable_and_args_if_method(func: Callable, *args: Tuple) -> Tuple[Callable, Tuple, Tuple, bool]:
-    """
-    Extracts the callable function and arguments from a given function, if it is a method.
-    Args:
-        func (Callable): The function to extract the callable from.
-        *args: Variable length argument list.
-    Returns:
-        Tuple[Callable, Tuple, Tuple]: A tuple containing the extracted callable function, the modified arguments,
-        and the arguments to be printed.
-    """
-
-    callable_func: Callable = func
-    args_to_print: Tuple = args
-    is_method: bool = hasattr(args[0], func.__name__) if args else False
-
-    if is_method:
-        args_to_print = args[1:]
-        if isinstance(func, classmethod):
-            args = (args[0].__class__,) + args[1:]  # type: ignore
-            callable_func = func.__func__
-        elif isinstance(func, staticmethod):
-            args = args[1:]
-    return callable_func, args, args_to_print, is_method
-
-
-def check_is_recursive_func(func: Callable, potential_recursion_func_stack: deque[Callable]) -> bool:
-    """
-    Checks if the function is being called recursively by checking the stack of called functions.
-    It will send a warning if the function is being called recursively.
-    Args:
-        func (Callable): The function to check for recursion.
-        potential_recursion_func_stack (deque[Callable]): A stack of potential recursive functions.
-    Returns:
-        bool: True if the function is being called recursively, False otherwise.
-
-    """
-
-    if potential_recursion_func_stack and potential_recursion_func_stack[-1] == func:
-        potential_recursion_func_stack.append(func)
-        # Check if the function is being called recursively by checking the object identity. This is way faster than using getFrameInfo
-        warning_msg = "Recursive function detected. This process may be slow. Consider wrapping the recursive function in another function and applying the @metrit decorator to the new function."
-        warn(warning_msg, stacklevel=3)
-        return True
-    potential_recursion_func_stack.append(func)
-    return False
+from collections import deque
+from typing import Callable, Tuple
+from warnings import warn
+
+
+def format_size(bytes_size: int | float) -> str:
+    """
+    Converts a size in bytes to a human-readable format.
+    Parameters:
+        bytes_size (int | float): The size in bytes to be converted.
+    Returns:
+        str: The human-read
+    """
+    for unit in ["B", "KB", "MB", "GB", "TB"]:
+        if bytes_size < 1024:
+            if unit == "B":
+                return f"{bytes_size:.0f}{unit}"
+            return f"{bytes_size:.2f}{unit}"
+        bytes_size /= 1024
+    return f"{bytes_size:.2f}PB"  # If it exceeds TB, convert to petabytes
+
+
+def extract_callable_and_args_if_method(func: Callable, *args: Tuple) -> Tuple[Callable, Tuple, Tuple, bool]:
+    """
+    Extracts the callable function and arguments from a given function, if it is a method.
+    Args:
+        func (Callable): The function to extract the callable from.
+        *args: Variable length argument list.
+    Returns:
+        Tuple[Callable, Tuple, Tuple]: A tuple containing the extracted callable function, the modified arguments,
+        and the arguments to be printed.
+    """
+
+    callable_func: Callable = func
+    args_to_print: Tuple = args
+    is_method: bool = hasattr(args[0], func.__name__) if args else False
+
+    if is_method:
+        args_to_print = args[1:]
+        if isinstance(func, classmethod):
+            args = (args[0].__class__,) + args[1:]  # type: ignore
+            callable_func = func.__func__
+        elif isinstance(func, staticmethod):
+            args = args[1:]
+    return callable_func, args, args_to_print, is_method
+
+
+def check_is_recursive_func(func: Callable, potential_recursion_func_stack: deque[Callable]) -> bool:
+    """
+    Checks if the function is being called recursively by checking the stack of called functions.
+    It will send a warning if the function is being called recursively.
+    Args:
+        func (Callable): The function to check for recursion.
+        potential_recursion_func_stack (deque[Callable]): A stack of potential recursive functions.
+    Returns:
+        bool: True if the function is being called recursively, False otherwise.
+
+    """
+
+    if potential_recursion_func_stack and potential_recursion_func_stack[-1] == func:
+        potential_recursion_func_stack.append(func)
+        # Check if the function is being called recursively by checking the object identity. This is way faster than using getFrameInfo
+        warning_msg = "Recursive function detected. This process may be slow. Consider wrapping the recursive function in another function and applying the @metrit decorator to the new function."
+        warn(warning_msg, stacklevel=3)
+        return True
+    potential_recursion_func_stack.append(func)
+    return False
```

### Comparing `metrit-0.0.1/metrit.egg-info/PKG-INFO` & `metrit-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,250 +1,231 @@
-Metadata-Version: 2.1
-Name: metrit
-Version: 0.0.1
-Summary: A dead simple resources monitoring decorator
-Home-page: https://github.com/mcrespoae/metrit
-Author: mcrespoae
-Author-email: info@mariocrespo.es
-Keywords: metrit
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: psutil==5.9.8
-Requires-Dist: multiprocess==0.70.16
-
-
-# metrit
-
-![PyPI](https://img.shields.io/pypi/v/metrit?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/metrit)
-
-## Overview
-
-`metrit` is a Python package designed to simplify the process of measuring the execution resources of your functions through a straightforward decorator.
-
-## Installation
-
-You can install `metrit` using pip:
-
-```bash
-pip install metrit
-```
-
-## Usage
-
-Utilizing the `metrit` decorator is simple and intuitive. Follow this section to learn how to make the most of its capabilities.
-
-### Basic Usage
-
-Below are some examples demonstrating `metrit`'s usage:
-
-```python
-from metrit import metrit
-
-@metrit
-def my_function():
-    # Normal code of your function
-    pass
-
-my_function()
-```
-
-This will output something like:
-
-```text
-Function 'my_function'    24.00KB avg of memory     0.00% avg of CPU     239B IO reads   2.05KB IO writes.
-```
-
-### Advanced Usage
-
-You can customize the behavior of the `metrit` decorator using various [Parameters](#parameters). Here is an example:
-
-```python
-from metrit import metrit
-@metrit(verbose=True, find_children=True, isolate=True)
-def my_function_with_args(a:int = 1, b:int = 2):
-    return a + b
-
-result = my_function_with_args(1, b=2)
-```
-
-This will provide detailed output:
-
-```text
-***** metrit data for function my_function_with_args: *****
-    Args: (1,).
-    Kwargs: {'b': 2}.
-    Maximum CPU usage: 0.00%.
-    Average CPU usage: 0.00%.
-    Average memory usage: 0.00%.
-    Maximum RSS memory usage: 112.00KB.
-    Average RSS memory usage: 112.00KB.
-    Maximum VMS memory usage: 68.00KB.
-    Average VMS memory usage: 68.00KB.
-    IO read count: 5.
-    IO writes count: 2.
-    IO read bytes: 239B.
-    IO write bytes: 2.01KB.
-***** End of metrit data. *****
-```
-
-More examples can be found in the [examples.py](https://github.com/mcrespoae/metrit/blob/main/examples/examples.py) script.
-
-### Metrit in Production Environments
-
-The `metrit` decorator is designed **exclusively for benchmarking and is not suitable for use in production code**. You can globally deactivate the `metrit` feature by setting the `MetrittConfig.ACTIVE` flag to false at the top of your imports. While this will skip the decoration of callables, there may still be a minimal CPU overhead. For production-grade applications, it's recommended to manually remove the decorators and `metrit` imports to maintain optimal performance.
-
-```python
-from metrit import MetritConfig, metrit
-MetritConfig.ACTIVE = False  # Deactivates the decorator
-```
-
-## Features
-
-- Simplified usage.
-- Accurate measurement of function resources.
-- Ability to isolate the execution of the function for more accurate measurement.
-- Support for functions, methods, `classmethod` and `staticmethods`.
-- Human-readable data formatting.
-- Optional verbose mode for detailed information.
-- Ability to globally deactivate the `metrit` decorator.
-- Optional check children processes' resources as well.
-- Automatic recursion detection.
-
-## Parameters
-
-Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
-
-- `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
-- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
-- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
-
-## Best Practices
-
-The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
-
-- For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
-
-- Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
-
-- Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
-
-## Recursive Functions
-
-Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
-
-### Using the Auto-Recursion Feature
-
-The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
-
-This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
-
-```python
-@metrit
-def recursive_func(n):
-    if n == 0:
-        return 0
-    else:
-        return n + recursive_func(n - 1)
-
-
-# This will trigger the auto-recursion feature
-result = recursive_func(3)
-```
-
-### Encapsulating the Recursive Function
-
-The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
-
-```python
-@metrit
-def encapsulated_recursive_function(n):
-    """A non-verbose wrapper for the recursive function."""
-    def recursive_func(n):
-        if n == 0:
-            return 0
-        else:
-            return n + recursive_func(n - 1)
-
-    return recursive_func(n)
-
-# Encapsulating the recursive function
-result = encapsulated_recursive_function(3)
-```
-
-This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
-
-## Isolate
-
-The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
-
-## Limitations
-
-While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
-
-### Isolate Limitations
-
-While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
-
-- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
-- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
-
-### Why is Class Decoration Bypassed?
-
-When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
-
-This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
-
-### MacOs Limitations
-
-This package relies on the `psutil` package for retrieving data. Unfortunately, macOS and `psutil` do not support IO data per process, so IO data will not be shown on macOS.
-
-### CPU Percentage Over 100
-
-As noted in the psutil documentation:
-> Note: the returned value can be > 100.0 in case of a process running multiple threads on different CPU cores.
-
-Additionally, if `find_children` is set to `True`, the CPU percentage of all child processes will be added to the main process. This can easily result in the max and average CPU percentages exceeding 100%.
-
-## Error Management and Warnings
-
-### Errors
-
-If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
-
-### Warnings
-
-- Deprecation warnings will be added before removing a feature.
-- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
-
-## Contributing
-
-Contributions are welcome! Please follow these guidelines when contributing:
-
-1. Fork the repository.
-2. Use `make install` to install all dependencies.
-3. Create a new branch for your changes.
-4. Implement your changes and commit them.
-5. Push your changes to your forked repository.
-6. Submit a pull request.
-
-You can also open an issue if you find a bug or have a suggestion.
-
-You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/metrit/blob/main/Makefile) to know more about commands.
-
-## Testing
-
-The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/metrit/tree/main/tests).
-
-## License
-
-This project is licensed under the [MIT License](https://github.com/mcrespoae/metrit/blob/main/LICENSE).
-
-## Contributors
-
-- [Mario Crespo](https://github.com/mcrespoae)
+
+# metrit
+
+![PyPI](https://img.shields.io/pypi/v/metrit?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/metrit)
+
+## Overview
+
+`metrit` is a Python package designed to simplify the process of measuring the execution resources of your functions through a straightforward decorator.
+
+## Installation
+
+You can install `metrit` using pip:
+
+```bash
+pip install metrit
+```
+
+## Usage
+
+Utilizing the `metrit` decorator is simple and intuitive. Follow this section to learn how to make the most of its capabilities.
+
+### Basic Usage
+
+Below are some examples demonstrating `metrit`'s usage:
+
+```python
+from metrit import metrit
+
+@metrit
+def my_function():
+    # Normal code of your function
+    pass
+
+my_function()
+```
+
+This will output something like:
+
+```text
+Function 'my_function'    24.00KB avg of memory     0.00% avg of CPU     239B IO reads   2.05KB IO writes.
+```
+
+### Advanced Usage
+
+You can customize the behavior of the `metrit` decorator using various [Parameters](#parameters). Here is an example:
+
+```python
+from metrit import metrit
+@metrit(verbose=True, find_children=True, isolate=True)
+def my_function_with_args(a:int = 1, b:int = 2):
+    return a + b
+
+result = my_function_with_args(1, b=2)
+```
+
+This will provide detailed output:
+
+```text
+***** metrit data for function my_function_with_args: *****
+    Args: (1,).
+    Kwargs: {'b': 2}.
+    Maximum CPU usage: 0.00%.
+    Average CPU usage: 0.00%.
+    Average memory usage: 0.00%.
+    Maximum RSS memory usage: 112.00KB.
+    Average RSS memory usage: 112.00KB.
+    Maximum VMS memory usage: 68.00KB.
+    Average VMS memory usage: 68.00KB.
+    IO read count: 5.
+    IO writes count: 2.
+    IO read bytes: 239B.
+    IO write bytes: 2.01KB.
+***** End of metrit data. *****
+```
+
+More examples can be found in the [examples.py](https://github.com/mcrespoae/metrit/blob/main/examples/examples.py) script.
+
+### Metrit in Production Environments
+
+The `metrit` decorator is designed **exclusively for benchmarking and is not suitable for use in production code**. You can globally deactivate the `metrit` feature by setting the `MetrittConfig.ACTIVE` flag to false at the top of your imports. While this will skip the decoration of callables, there may still be a minimal CPU overhead. For production-grade applications, it's recommended to manually remove the decorators and `metrit` imports to maintain optimal performance.
+
+```python
+from metrit import MetritConfig, metrit
+MetritConfig.ACTIVE = False  # Deactivates the decorator
+```
+
+## Features
+
+- Simplified usage.
+- Accurate measurement of function resources.
+- Ability to isolate the execution of the function for more accurate measurement.
+- Support for functions, methods, `classmethod` and `staticmethods`.
+- Human-readable data formatting.
+- Optional verbose mode for detailed information.
+- Ability to globally deactivate the `metrit` decorator.
+- Optional check children processes' resources as well.
+- Automatic recursion detection.
+
+## Parameters
+
+Using the decorator `@metrit` without any parameters executes the function once and displays the resources. However, you can enhance the experience using the following arguments:
+
+- `find_children` (bool, optional): Specifies if the monitoring system should look for children processes as well. Defaults to False.
+- `isolate` (bool, optional): Determines if the execution of the function is done in a separate process for more accurate results. See the [Isolate limitations](#isolate-limitations) for more details. Defaults to False.
+- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
+
+## Best Practices
+
+The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
+
+- For more precise measurements, it is recommended to set `isolate` to `True`. Please see the [Isolate](#isolate) section to understand the limitations of this approach.
+
+- Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more.
+
+- Decorating classes will return the class unmodified and will not be decorated. For more information about this decision, see the [Why is class decoration bypassed](#why-is-class-decoration-bypassed) in the [Limitations](#limitations) section.
+
+## Recursive Functions
+
+Measuring the resources of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended [encapsulating the recursive function](#encapsulating-the-recursive-function) within another function for cleaner, more precise, and safer results. Using recursive functions with `isolate = True` will not trigger the automatic recursion checker, making bad measurements, slowing time and making a too verbose output.
+
+### Using the Auto-Recursion Feature
+
+The auto-recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the measures taken to run the appropriate function, plus a small overhead. It is not recommended to rely on this feature intentionally since the collected data might not be as accurate.
+
+This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
+
+```python
+@metrit
+def recursive_func(n):
+    if n == 0:
+        return 0
+    else:
+        return n + recursive_func(n - 1)
+
+
+# This will trigger the auto-recursion feature
+result = recursive_func(3)
+```
+
+### Encapsulating the Recursive Function
+
+The recommended option is to encapsulate the recursive function within another function and then, decorate and call the parent function. Here's an example:
+
+```python
+@metrit
+def encapsulated_recursive_function(n):
+    """A non-verbose wrapper for the recursive function."""
+    def recursive_func(n):
+        if n == 0:
+            return 0
+        else:
+            return n + recursive_func(n - 1)
+
+    return recursive_func(n)
+
+# Encapsulating the recursive function
+result = encapsulated_recursive_function(3)
+```
+
+This approach enhances readability without incurring any performance penalties, even if `isolate = True`. However, it requires modifying your code to measure this type of function.
+
+## Isolate
+
+The isolation feature works by encapsulating the decorated function in a separate process and then monitoring that process from another process to avoid interfering with the function's execution. If any part of this process fails, `metrit` will retry running the function in the original process.
+
+## Limitations
+
+While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `metrit` decorator could lead to unexpected behavior.
+
+### Isolate Limitations
+
+While the `isolate` feature is powerful and recommended for precise measurements, it can lead to unexpected results. Here are the main limitations:
+
+- Using it in a non-wrapped recursive function will generate a process for each recursive call, wasting resources, performing inaccurate measurements, and generating verbose output. Ensure you are not using it directly with a recursive function.
+- Methods are not affected by the `isolate` parameter and will be executed as if it were `False`. This is because encapsulating a method in a separate process from its object can lead to issues. When methods are called, they rely on the state of the object they belong to. Isolating a method would require serializing (pickling) the entire object state and then deserializing it in a new process. This process can be complex and error-prone, leading to potential errors and inconsistencies. Therefore, to avoid these issues, `metrit` does not apply the isolate parameter to methods, ensuring they run in the same process as their object.
+
+### Why is Class Decoration Bypassed?
+
+When a class is decorated using `metrit`, it remains unmodified and is not decorated. If the user intends to measure the time of `__init__` or any other constructor, it can be done directly on those methods.
+
+This design decision was made due to a potential issue that arises when a decorated class is used in conjunction with spawning a new process. Specifically, if a class decorated with `metrit` is pickled for use in a separate process and then a method is called within that new process, it may result in a `PicklingError`.
+
+### MacOs Limitations
+
+This package relies on the `psutil` package for retrieving data. Unfortunately, macOS and `psutil` do not support IO data per process, so IO data will not be shown on macOS.
+
+### CPU Percentage Over 100
+
+As noted in the psutil documentation:
+> Note: the returned value can be > 100.0 in case of a process running multiple threads on different CPU cores.
+
+Additionally, if `find_children` is set to `True`, the CPU percentage of all child processes will be added to the main process. This can easily result in the max and average CPU percentages exceeding 100%.
+
+## Error Management and Warnings
+
+### Errors
+
+If an error occurs while executing the decorated function in non-isolated mode or within a recursively decorated function, the error will be propagated to the user's function.
+
+### Warnings
+
+- Deprecation warnings will be added before removing a feature.
+- If recursion is detected, a warning will be prompted. In such cases, refer to the [Recursive functions](#recursive-functions) section.
+
+## Contributing
+
+Contributions are welcome! Please follow these guidelines when contributing:
+
+1. Fork the repository.
+2. Use `make install` to install all dependencies.
+3. Create a new branch for your changes.
+4. Implement your changes and commit them.
+5. Push your changes to your forked repository.
+6. Submit a pull request.
+
+You can also open an issue if you find a bug or have a suggestion.
+
+You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/metrit/blob/main/Makefile) to know more about commands.
+
+## Testing
+
+The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/metrit/tree/main/tests).
+
+## License
+
+This project is licensed under the [MIT License](https://github.com/mcrespoae/metrit/blob/main/LICENSE).
+
+## Contributors
+
+- [Mario Crespo](https://github.com/mcrespoae)
```

### Comparing `metrit-0.0.1/tests/test_metrit.py` & `metrit-0.0.3/tests/test_metrit.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import os
-import unittest
-from time import sleep
-
-from metrit.core import MetritConfig, metrit
-
-IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
-
-MetritConfig.ACTIVE = True
-
-
-@metrit
-class MetritTestClassWithArgs:
-    @metrit
-    def __init__(self, a: int = 1, b: int = 2):
-        self.sum = a + b
-
-
-@metrit
-class MetritTestClass:
-    @metrit
-    def metrit_basic(self, a: int = 1, b: int = 2):
-        return a + b
-
-    @metrit
-    @staticmethod
-    def static_method(a: int = 1, b: int = 2):
-        return a + b
-
-    @metrit
-    @classmethod
-    def class_method(cls, a: int = 1, b: int = 2):
-        return cls.__name__, a + b
-
-
-@metrit
-def fill_ram(size_in_mb, duration_in_seconds):
-    size_in_bytes = int(size_in_mb * 1024 * 1024)
-    _ = bytearray(size_in_bytes)
-    sleep(duration_in_seconds)
-    return 1 + 2
-
-
-@metrit()
-def cpu_intensive(a: int = 1, b: int = 2) -> int:
-    for _ in range(2):
-        for _ in range(1_000):
-            pass  # Simulate some work
-    return a + b
-
-
-@metrit
-def recursive_func(n):
-    if n < 2:
-        return n
-    return recursive_func(n - 2) + recursive_func(n - 1)
-
-
-def fib(n):
-    if n < 2:
-        return n
-    return fib(n - 2) + fib(n - 1)
-
-
-@metrit
-def wrapped_recursive_func(n):
-    return fib(n)
-
-
-@metrit
-def simulate_writes_and_reads(num_writes=5_000, data_size=1024):
-    file = ".temp_file"
-    with open(file, "wb") as f:
-        for _ in range(num_writes):
-            f.write(b"a" * data_size)
-            f.flush()
-
-    with open(file, "rb") as f:
-        f.read()
-    os.remove(file)
-
-
-class TestMetritFunctions(unittest.TestCase):
-    def setUp(self):
-        MetritConfig.ACTIVE = True
-
-    def test_MetritTestClassWithArgs(self):
-        obj = MetritTestClassWithArgs(3, b=6)
-        self.assertEqual(obj.sum, 9)
-
-    def test_metrit_basic(self):
-        obj = MetritTestClass()
-        result = obj.metrit_basic()
-        self.assertEqual(result, 3)
-
-    def test_static_method(self):
-        result = MetritTestClass.static_method()
-        self.assertEqual(result, 3)
-
-    def test_class_method(self):
-        obj = MetritTestClass()
-        class_name, result = obj.class_method(3, b=4)
-        self.assertEqual(result, 7)
-        self.assertEqual(class_name, "MetritTestClass")
-
-    def test_fill_ram(self):
-        result = fill_ram(0.5, 0.1)  # 0.5 MB for 0.1 second
-        self.assertEqual(result, 3)
-
-    def test_cpu_intensive(self):
-        result = cpu_intensive(3, b=4)
-        self.assertEqual(result, 7)
-
-    def test_recursive_func(self):
-        result = recursive_func(5)
-        self.assertEqual(result, 5)  # fib(5) is 5
-
-    def test_wrapped_recursive_func(self):
-        result = wrapped_recursive_func(5)
-        self.assertEqual(result, 5)  # fib(5) is 5
-
-    def test_simulate_writes_and_reads(self):
-        simulate_writes_and_reads(100, 1024)  # Smaller number of writes for testing purposes
-
-
-if __name__ == "__main__":
-    unittest.main()
+import os
+import unittest
+from time import sleep
+
+from metrit.core import MetritConfig, metrit
+
+IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
+
+MetritConfig.ACTIVE = True
+
+
+@metrit
+class MetritTestClassWithArgs:
+    @metrit
+    def __init__(self, a: int = 1, b: int = 2):
+        self.sum = a + b
+
+
+@metrit
+class MetritTestClass:
+    @metrit
+    def metrit_basic(self, a: int = 1, b: int = 2):
+        return a + b
+
+    @metrit
+    @staticmethod
+    def static_method(a: int = 1, b: int = 2):
+        return a + b
+
+    @metrit
+    @classmethod
+    def class_method(cls, a: int = 1, b: int = 2):
+        return cls.__name__, a + b
+
+
+@metrit
+def fill_ram(size_in_mb, duration_in_seconds):
+    size_in_bytes = int(size_in_mb * 1024 * 1024)
+    _ = bytearray(size_in_bytes)
+    sleep(duration_in_seconds)
+    return 1 + 2
+
+
+@metrit()
+def cpu_intensive(a: int = 1, b: int = 2) -> int:
+    for _ in range(2):
+        for _ in range(1_000):
+            pass  # Simulate some work
+    return a + b
+
+
+@metrit
+def recursive_func(n):
+    if n < 2:
+        return n
+    return recursive_func(n - 2) + recursive_func(n - 1)
+
+
+def fib(n):
+    if n < 2:
+        return n
+    return fib(n - 2) + fib(n - 1)
+
+
+@metrit
+def wrapped_recursive_func(n):
+    return fib(n)
+
+
+@metrit
+def simulate_writes_and_reads(num_writes=5_000, data_size=1024):
+    file = ".temp_file"
+    with open(file, "wb") as f:
+        for _ in range(num_writes):
+            f.write(b"a" * data_size)
+            f.flush()
+
+    with open(file, "rb") as f:
+        f.read()
+    os.remove(file)
+
+
+class TestMetritFunctions(unittest.TestCase):
+    def setUp(self):
+        MetritConfig.ACTIVE = True
+
+    def test_MetritTestClassWithArgs(self):
+        obj = MetritTestClassWithArgs(3, b=6)
+        self.assertEqual(obj.sum, 9)
+
+    def test_metrit_basic(self):
+        obj = MetritTestClass()
+        result = obj.metrit_basic()
+        self.assertEqual(result, 3)
+
+    def test_static_method(self):
+        result = MetritTestClass.static_method()
+        self.assertEqual(result, 3)
+
+    def test_class_method(self):
+        obj = MetritTestClass()
+        class_name, result = obj.class_method(3, b=4)
+        self.assertEqual(result, 7)
+        self.assertEqual(class_name, "MetritTestClass")
+
+    def test_fill_ram(self):
+        result = fill_ram(0.5, 0.1)  # 0.5 MB for 0.1 second
+        self.assertEqual(result, 3)
+
+    def test_cpu_intensive(self):
+        result = cpu_intensive(3, b=4)
+        self.assertEqual(result, 7)
+
+    def test_recursive_func(self):
+        result = recursive_func(5)
+        self.assertEqual(result, 5)  # fib(5) is 5
+
+    def test_wrapped_recursive_func(self):
+        result = wrapped_recursive_func(5)
+        self.assertEqual(result, 5)  # fib(5) is 5
+
+    def test_simulate_writes_and_reads(self):
+        simulate_writes_and_reads(100, 1024)  # Smaller number of writes for testing purposes
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `metrit-0.0.1/tests/test_metrit_deactivated.py` & `metrit-0.0.3/tests/test_metrit_deactivated.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-import os
-import unittest
-from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
-
-from metrit.core import MetritConfig, metrit
-
-IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
-MetritConfig.ACTIVE = False
-
-
-class MetritTestClassDeactivated:
-
-    @metrit()
-    def metrit_basic(self, a: int = 0, b: int = 1):
-        return a + b
-
-    @metrit
-    def metrit_basic_no_parenthesis(self, a: int = 0, b: int = 1):
-        return a + b
-
-    def sum(self, a: int = 1, b: int = 2):
-        return a + b
-
-    @metrit(verbose=True, find_children=True)
-    def test_metrit_args(self, a: int = 0, b: int = 1):
-        return self.sum(a, b)
-
-    @metrit(isolate=True)
-    @staticmethod
-    def static_method(a: int = 0, b: int = 1):
-        return a + b
-
-    @metrit
-    @classmethod
-    def class_method(cls, a: int = 0, b: int = 1):
-        return cls.__name__, a + b
-
-
-class TestmetritDecoratorClassDeactivated(unittest.TestCase):
-    def setUp(self):
-        self.test_class = MetritTestClassDeactivated()
-
-    def test_metrit_basic(self):
-        result_1 = self.test_class.metrit_basic(1, b=2)
-        result_2 = self.test_class.metrit_basic()
-        self.assertEqual(result_1, 3)
-        self.assertEqual(result_2, 1)
-
-    def test_metrit_basic_no_parenthesis(self):
-        result_1 = self.test_class.metrit_basic_no_parenthesis(1, b=2)
-        result_2 = self.test_class.metrit_basic_no_parenthesis()
-        self.assertEqual(result_1, 3)
-        self.assertEqual(result_2, 1)
-
-    def test_metrit_args(self):
-        result_1 = self.test_class.test_metrit_args(1, b=2)
-        result_2 = self.test_class.test_metrit_args()
-        self.assertEqual(result_1, 3)
-        self.assertEqual(result_2, 1)
-
-    def test_metrit_static_method(self):
-        result_1 = self.test_class.static_method(1, b=2)
-        result_2 = self.test_class.static_method()
-        self.assertEqual(result_1, 3)
-        self.assertEqual(result_2, 1)
-
-    def test_metrit_class_method(self):
-        class_name_1, result_1 = self.test_class.class_method(1, b=2)
-        class_name_2, result_2 = self.test_class.class_method()
-        self.assertEqual(class_name_1, "MetritTestClassDeactivated")
-        self.assertEqual(result_1, 3)
-        self.assertEqual(class_name_2, "MetritTestClassDeactivated")
-        self.assertEqual(result_2, 1)
-
-    def test_metrit_run_from_other_thread(self):
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.test_metrit_args, 1, b=2)
-            result = future.result()
-
-        self.assertEqual(result, 3)
-
-    def test_metrit_run_from_other_process(self):
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.test_metrit_args, 1, b=2)
-            result = future.result()
-
-        self.assertEqual(result, 3)
-
-    def test_metrit_class_method_from_other_thread(self):
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.class_method, 1, b=2)
-            class_name, result = future.result()
-
-        self.assertEqual(class_name, "MetritTestClassDeactivated")
-        self.assertEqual(result, 3)
-
-    def test_metrit_class_method_run_from_other_process(self):
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.class_method, 2, b=6)
-            class_name, result = future.result()
-
-        self.assertEqual(class_name, "MetritTestClassDeactivated")
-        self.assertEqual(result, 8)
-
-    def test_metrit_static_method_from_other_thread(self):
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.static_method, 4, b=5)
-            result = future.result()
-
-        self.assertEqual(result, 9)
-
-    def test_metrit_static_method_run_from_other_process(self):
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.static_method, 1, b=2)
-            result = future.result()
-
-        self.assertEqual(result, 3)
-
-
-class TestMetritDeactivated(unittest.TestCase):
-    MetritConfig.ACTIVE = False
-
-    def setUp(self):
-        MetritConfig.ACTIVE = False
-
-    def test_metrit_basic_deactivated(self):
-        @metrit
-        def my_function(a: int = 0, b: int = 1):
-            return a + b
-
-        self.assertEqual(my_function(1, b=2), 3)
-        self.assertEqual(my_function(), 1)
-
-    def test_metrit_with_args_deactivated(self):
-        @metrit(verbose=True)
-        def my_function(a: int = 0, b: int = 1):
-            return a + b
-
-        self.assertEqual(my_function(1, b=2), 3)
-        self.assertEqual(my_function(), 1)
-
-    def test_run_from_other_process(self):
-
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future_1 = executor.submit(my_process_function_deactivated, 1, b=2)
-            result_1 = future_1.result()
-            future_2 = executor.submit(my_process_function_deactivated)
-            result_2 = future_2.result()
-            future_3 = executor.submit(my_process_function_no_args_deactivated, 1, b=2)
-            result_3 = future_3.result()
-            future_4 = executor.submit(my_process_function_no_args_deactivated)
-            result_4 = future_4.result()
-
-        self.assertEqual(result_1, 3)
-        self.assertEqual(result_2, 1)
-        self.assertEqual(result_3, 3)
-        self.assertEqual(result_4, 1)
-
-    def test_run_from_other_thread(self):
-        @metrit()
-        def my_thread_function(a=0, b=1):
-            return a + b
-
-        @metrit
-        def my_thread_no_args_function(a=0, b=1):
-            return a + b
-
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future_1 = executor.submit(my_thread_function, 1, b=2)
-            result_1 = future_1.result()
-            future_2 = executor.submit(my_thread_function)
-            result_2 = future_2.result()
-            future_3 = executor.submit(my_thread_no_args_function, 1, b=2)
-            result_3 = future_3.result()
-            future_4 = executor.submit(my_thread_no_args_function)
-            result_4 = future_4.result()
-
-        self.assertEqual(result_1, 3)
-        self.assertEqual(result_2, 1)
-        self.assertEqual(result_3, 3)
-        self.assertEqual(result_4, 1)
-
-
-# Added here since calling a function from another process inside a test method doesn't work
-@metrit(find_children=True, isolate=True, verbose=True)
-def my_process_function_deactivated(a: int = 0, b: int = 1):
-    return a + b
-
-
-@metrit
-def my_process_function_no_args_deactivated(a: int = 0, b: int = 1):
-    return a + b
-
-
-if __name__ == "__main__":
-    unittest.main()
+import os
+import unittest
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+
+from metrit.core import MetritConfig, metrit
+
+IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
+MetritConfig.ACTIVE = False
+
+
+class MetritTestClassDeactivated:
+
+    @metrit()
+    def metrit_basic(self, a: int = 0, b: int = 1):
+        return a + b
+
+    @metrit
+    def metrit_basic_no_parenthesis(self, a: int = 0, b: int = 1):
+        return a + b
+
+    def sum(self, a: int = 1, b: int = 2):
+        return a + b
+
+    @metrit(verbose=True, find_children=True)
+    def test_metrit_args(self, a: int = 0, b: int = 1):
+        return self.sum(a, b)
+
+    @metrit(isolate=True)
+    @staticmethod
+    def static_method(a: int = 0, b: int = 1):
+        return a + b
+
+    @metrit
+    @classmethod
+    def class_method(cls, a: int = 0, b: int = 1):
+        return cls.__name__, a + b
+
+
+class TestmetritDecoratorClassDeactivated(unittest.TestCase):
+    def setUp(self):
+        self.test_class = MetritTestClassDeactivated()
+
+    def test_metrit_basic(self):
+        result_1 = self.test_class.metrit_basic(1, b=2)
+        result_2 = self.test_class.metrit_basic()
+        self.assertEqual(result_1, 3)
+        self.assertEqual(result_2, 1)
+
+    def test_metrit_basic_no_parenthesis(self):
+        result_1 = self.test_class.metrit_basic_no_parenthesis(1, b=2)
+        result_2 = self.test_class.metrit_basic_no_parenthesis()
+        self.assertEqual(result_1, 3)
+        self.assertEqual(result_2, 1)
+
+    def test_metrit_args(self):
+        result_1 = self.test_class.test_metrit_args(1, b=2)
+        result_2 = self.test_class.test_metrit_args()
+        self.assertEqual(result_1, 3)
+        self.assertEqual(result_2, 1)
+
+    def test_metrit_static_method(self):
+        result_1 = self.test_class.static_method(1, b=2)
+        result_2 = self.test_class.static_method()
+        self.assertEqual(result_1, 3)
+        self.assertEqual(result_2, 1)
+
+    def test_metrit_class_method(self):
+        class_name_1, result_1 = self.test_class.class_method(1, b=2)
+        class_name_2, result_2 = self.test_class.class_method()
+        self.assertEqual(class_name_1, "MetritTestClassDeactivated")
+        self.assertEqual(result_1, 3)
+        self.assertEqual(class_name_2, "MetritTestClassDeactivated")
+        self.assertEqual(result_2, 1)
+
+    def test_metrit_run_from_other_thread(self):
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.test_metrit_args, 1, b=2)
+            result = future.result()
+
+        self.assertEqual(result, 3)
+
+    def test_metrit_run_from_other_process(self):
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.test_metrit_args, 1, b=2)
+            result = future.result()
+
+        self.assertEqual(result, 3)
+
+    def test_metrit_class_method_from_other_thread(self):
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.class_method, 1, b=2)
+            class_name, result = future.result()
+
+        self.assertEqual(class_name, "MetritTestClassDeactivated")
+        self.assertEqual(result, 3)
+
+    def test_metrit_class_method_run_from_other_process(self):
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.class_method, 2, b=6)
+            class_name, result = future.result()
+
+        self.assertEqual(class_name, "MetritTestClassDeactivated")
+        self.assertEqual(result, 8)
+
+    def test_metrit_static_method_from_other_thread(self):
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.static_method, 4, b=5)
+            result = future.result()
+
+        self.assertEqual(result, 9)
+
+    def test_metrit_static_method_run_from_other_process(self):
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.static_method, 1, b=2)
+            result = future.result()
+
+        self.assertEqual(result, 3)
+
+
+class TestMetritDeactivated(unittest.TestCase):
+    MetritConfig.ACTIVE = False
+
+    def setUp(self):
+        MetritConfig.ACTIVE = False
+
+    def test_metrit_basic_deactivated(self):
+        @metrit
+        def my_function(a: int = 0, b: int = 1):
+            return a + b
+
+        self.assertEqual(my_function(1, b=2), 3)
+        self.assertEqual(my_function(), 1)
+
+    def test_metrit_with_args_deactivated(self):
+        @metrit(verbose=True)
+        def my_function(a: int = 0, b: int = 1):
+            return a + b
+
+        self.assertEqual(my_function(1, b=2), 3)
+        self.assertEqual(my_function(), 1)
+
+    def test_run_from_other_process(self):
+
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future_1 = executor.submit(my_process_function_deactivated, 1, b=2)
+            result_1 = future_1.result()
+            future_2 = executor.submit(my_process_function_deactivated)
+            result_2 = future_2.result()
+            future_3 = executor.submit(my_process_function_no_args_deactivated, 1, b=2)
+            result_3 = future_3.result()
+            future_4 = executor.submit(my_process_function_no_args_deactivated)
+            result_4 = future_4.result()
+
+        self.assertEqual(result_1, 3)
+        self.assertEqual(result_2, 1)
+        self.assertEqual(result_3, 3)
+        self.assertEqual(result_4, 1)
+
+    def test_run_from_other_thread(self):
+        @metrit()
+        def my_thread_function(a=0, b=1):
+            return a + b
+
+        @metrit
+        def my_thread_no_args_function(a=0, b=1):
+            return a + b
+
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future_1 = executor.submit(my_thread_function, 1, b=2)
+            result_1 = future_1.result()
+            future_2 = executor.submit(my_thread_function)
+            result_2 = future_2.result()
+            future_3 = executor.submit(my_thread_no_args_function, 1, b=2)
+            result_3 = future_3.result()
+            future_4 = executor.submit(my_thread_no_args_function)
+            result_4 = future_4.result()
+
+        self.assertEqual(result_1, 3)
+        self.assertEqual(result_2, 1)
+        self.assertEqual(result_3, 3)
+        self.assertEqual(result_4, 1)
+
+
+# Added here since calling a function from another process inside a test method doesn't work
+@metrit(find_children=True, isolate=True, verbose=True)
+def my_process_function_deactivated(a: int = 0, b: int = 1):
+    return a + b
+
+
+@metrit
+def my_process_function_no_args_deactivated(a: int = 0, b: int = 1):
+    return a + b
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `metrit-0.0.1/tests/test_utils.py` & `metrit-0.0.3/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import unittest
-
-from metrit.utils import format_size
-
-
-class TestFormatSize(unittest.TestCase):
-
-    def test_bytes(self):
-        self.assertEqual(format_size(10), "10B")
-
-    def test_kilobytes(self):
-        self.assertEqual(format_size(1024), "1.00KB")
-
-    def test_megabytes(self):
-        self.assertEqual(format_size(1024 * 1024), "1.00MB")
-
-    def test_gigabytes(self):
-        self.assertEqual(format_size(1024 * 1024 * 1024), "1.00GB")
-
-    def test_terabytes(self):
-        self.assertEqual(format_size(1024 * 1024 * 1024 * 1024), "1.00TB")
-
-    def test_petabytes(self):
-        self.assertEqual(format_size(1024 * 1024 * 1024 * 1024 * 1024), "1.00PB")
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+
+from metrit.utils import format_size
+
+
+class TestFormatSize(unittest.TestCase):
+
+    def test_bytes(self):
+        self.assertEqual(format_size(10), "10B")
+
+    def test_kilobytes(self):
+        self.assertEqual(format_size(1024), "1.00KB")
+
+    def test_megabytes(self):
+        self.assertEqual(format_size(1024 * 1024), "1.00MB")
+
+    def test_gigabytes(self):
+        self.assertEqual(format_size(1024 * 1024 * 1024), "1.00GB")
+
+    def test_terabytes(self):
+        self.assertEqual(format_size(1024 * 1024 * 1024 * 1024), "1.00TB")
+
+    def test_petabytes(self):
+        self.assertEqual(format_size(1024 * 1024 * 1024 * 1024 * 1024), "1.00PB")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

