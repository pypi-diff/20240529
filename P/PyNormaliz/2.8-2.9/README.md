# Comparing `tmp/PyNormaliz-2.8.tar.gz` & `tmp/PyNormaliz-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyNormaliz-2.8.tar", last modified: Sun Jun  9 10:17:24 2019, max compression
+gzip compressed data, was "dist/PyNormaliz-2.9.tar", last modified: Sat Feb  8 14:45:39 2020, max compression
```

## Comparing `PyNormaliz-2.8.tar` & `PyNormaliz-2.9.tar`

### file list

```diff
@@ -1,46 +1,43 @@
-drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2019-06-09 10:17:24.000000 PyNormaliz-2.8/
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      744 2016-10-28 22:08:05.000000 PyNormaliz-2.8/COPYING
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)    18092 2010-03-23 23:34:05.000000 PyNormaliz-2.8/GPLv2
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)    73398 2019-06-07 10:11:24.000000 PyNormaliz-2.8/NormalizModule.cpp
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     3695 2019-06-09 10:17:24.000000 PyNormaliz-2.8/PKG-INFO
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)    24123 2019-04-23 09:34:43.000000 PyNormaliz-2.8/PyNormaliz.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     2748 2019-06-02 20:10:15.000000 PyNormaliz-2.8/Readme.md
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)       52 2019-04-28 18:50:11.000000 PyNormaliz-2.8/config.py.in
--rwxr-xr-x   0 sebastian  (1000) sebastian  (1000)   121777 2019-04-28 18:54:26.000000 PyNormaliz-2.8/configure
-drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2019-06-09 10:17:24.000000 PyNormaliz-2.8/doc/
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)    18936 2017-05-04 15:35:32.000000 PyNormaliz-2.8/doc/PyNormaliz_Tutorial.ipynb
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)   137933 2017-05-04 15:35:32.000000 PyNormaliz-2.8/doc/PyNormaliz_Tutorial.pdf
-drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2019-06-09 10:17:24.000000 PyNormaliz-2.8/examples/
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      485 2018-07-03 08:48:00.000000 PyNormaliz-2.8/examples/4x4.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1131 2019-04-23 07:14:56.000000 PyNormaliz-2.8/examples/first.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      578 2019-04-16 08:34:53.000000 PyNormaliz-2.8/examples/first_enf.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1151 2019-04-23 07:21:41.000000 PyNormaliz-2.8/examples/first_long.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1123 2017-12-06 09:43:28.000000 PyNormaliz-2.8/examples/first_rational.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1249 2018-04-13 21:10:28.000000 PyNormaliz-2.8/examples/getters.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      394 2017-12-06 09:43:28.000000 PyNormaliz-2.8/examples/j462.py
--rwxr-xr-x   0 sebastian  (1000) sebastian  (1000)      118 2019-04-22 11:58:57.000000 PyNormaliz-2.8/examples/runexamples.sh
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      270 2019-04-01 10:13:23.000000 PyNormaliz-2.8/examples/simple.py
-drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2019-06-09 10:17:24.000000 PyNormaliz-2.8/m4/
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)    19246 2019-04-28 18:50:11.000000 PyNormaliz-2.8/m4/ax_cxx_compile_stdcxx.m4
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)       40 2019-06-02 20:07:11.000000 PyNormaliz-2.8/setup.cfg
--rwxr-xr-x   0 sebastian  (1000) sebastian  (1000)     3157 2019-06-07 10:11:24.000000 PyNormaliz-2.8/setup.py
-drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2019-06-09 10:17:24.000000 PyNormaliz-2.8/tests/
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      994 2019-06-04 17:04:04.000000 PyNormaliz-2.8/tests/assertion.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      959 2019-06-04 17:02:50.000000 PyNormaliz-2.8/tests/assertion.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      402 2019-06-05 07:52:51.000000 PyNormaliz-2.8/tests/autom.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      330 2019-04-26 13:24:32.000000 PyNormaliz-2.8/tests/equation-41.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     9153 2019-06-04 18:16:09.000000 PyNormaliz-2.8/tests/generic_test.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     8400 2019-06-05 07:53:59.000000 PyNormaliz-2.8/tests/generic_test.pyc
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      281 2019-06-07 10:11:24.000000 PyNormaliz-2.8/tests/modify_cone.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      389 2019-06-07 10:11:24.000000 PyNormaliz-2.8/tests/modify_cone_renf.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      244 2019-04-26 13:24:32.000000 PyNormaliz-2.8/tests/must_be_matrices-39.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      462 2019-04-26 13:24:32.000000 PyNormaliz-2.8/tests/quasi_poly-36.txt
--rwxr-xr-x   0 sebastian  (1000) sebastian  (1000)     1483 2019-06-07 10:11:24.000000 PyNormaliz-2.8/tests/runtests.py
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      517 2019-04-25 09:13:32.000000 PyNormaliz-2.8/tests/segfault-23.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      433 2019-04-28 14:19:11.000000 PyNormaliz-2.8/tests/segfault-27.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      286 2019-04-26 13:24:32.000000 PyNormaliz-2.8/tests/segfault-35.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      312 2019-04-26 13:24:32.000000 PyNormaliz-2.8/tests/segfault-45.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     2205 2019-05-01 16:58:20.000000 PyNormaliz-2.8/tests/test_rational_cones.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      286 2019-04-26 13:24:32.000000 PyNormaliz-2.8/tests/vertex_denom-37.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      407 2019-04-26 13:24:32.000000 PyNormaliz-2.8/tests/volume_20.txt
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)      251 2019-04-26 13:24:32.000000 PyNormaliz-2.8/tests/volume_22.txt
+drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2020-02-08 14:45:39.000000 PyNormaliz-2.9/
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      744 2016-10-28 22:08:05.000000 PyNormaliz-2.9/COPYING
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)    18092 2010-03-23 23:34:05.000000 PyNormaliz-2.9/GPLv2
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)    71166 2020-02-08 14:43:04.000000 PyNormaliz-2.9/NormalizModule.cpp
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     4667 2020-02-08 14:45:39.000000 PyNormaliz-2.9/PKG-INFO
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     9484 2020-02-08 14:43:04.000000 PyNormaliz-2.9/PyNormaliz.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     3544 2020-02-08 14:43:04.000000 PyNormaliz-2.9/README.md
+drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2020-02-08 14:45:39.000000 PyNormaliz-2.9/doc/
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)    18936 2017-05-04 15:35:32.000000 PyNormaliz-2.9/doc/PyNormaliz_Tutorial.ipynb
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)   137933 2017-05-04 15:35:32.000000 PyNormaliz-2.9/doc/PyNormaliz_Tutorial.pdf
+drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2020-02-08 14:45:39.000000 PyNormaliz-2.9/examples/
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      485 2018-07-03 08:48:00.000000 PyNormaliz-2.9/examples/4x4.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1131 2019-04-23 07:14:56.000000 PyNormaliz-2.9/examples/first.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      578 2019-04-16 08:34:53.000000 PyNormaliz-2.9/examples/first_enf.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1151 2019-04-23 07:21:41.000000 PyNormaliz-2.9/examples/first_long.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1123 2017-12-06 09:43:28.000000 PyNormaliz-2.9/examples/first_rational.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1249 2018-04-13 21:10:28.000000 PyNormaliz-2.9/examples/getters.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      394 2017-12-06 09:43:28.000000 PyNormaliz-2.9/examples/j462.py
+-rwxr-xr-x   0 sebastian  (1000) sebastian  (1000)      118 2019-04-22 11:58:57.000000 PyNormaliz-2.9/examples/runexamples.sh
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      270 2019-04-01 10:13:23.000000 PyNormaliz-2.9/examples/simple.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)       40 2020-02-08 14:43:04.000000 PyNormaliz-2.9/setup.cfg
+-rwxr-xr-x   0 sebastian  (1000) sebastian  (1000)     1458 2020-02-08 14:45:00.000000 PyNormaliz-2.9/setup.py
+drwxr-xr-x   0 sebastian  (1000) sebastian  (1000)        0 2020-02-08 14:45:39.000000 PyNormaliz-2.9/tests/
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      994 2019-06-04 17:04:04.000000 PyNormaliz-2.9/tests/assertion.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      959 2019-06-04 17:02:50.000000 PyNormaliz-2.9/tests/assertion.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      402 2019-06-05 07:52:51.000000 PyNormaliz-2.9/tests/autom.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      330 2019-04-26 13:24:32.000000 PyNormaliz-2.9/tests/equation-41.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     9318 2020-02-08 14:43:04.000000 PyNormaliz-2.9/tests/generic_test.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     8400 2019-06-05 07:53:59.000000 PyNormaliz-2.9/tests/generic_test.pyc
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      281 2019-06-07 10:11:24.000000 PyNormaliz-2.9/tests/modify_cone.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      389 2019-06-07 10:11:24.000000 PyNormaliz-2.9/tests/modify_cone_renf.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      244 2019-04-26 13:24:32.000000 PyNormaliz-2.9/tests/must_be_matrices-39.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      462 2019-04-26 13:24:32.000000 PyNormaliz-2.9/tests/quasi_poly-36.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      457 2020-02-08 14:43:04.000000 PyNormaliz-2.9/tests/rational.txt
+-rwxr-xr-x   0 sebastian  (1000) sebastian  (1000)     1537 2020-02-08 14:43:04.000000 PyNormaliz-2.9/tests/runtests.py
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      517 2019-04-25 09:13:32.000000 PyNormaliz-2.9/tests/segfault-23.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      433 2019-04-28 14:19:11.000000 PyNormaliz-2.9/tests/segfault-27.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      286 2019-04-26 13:24:32.000000 PyNormaliz-2.9/tests/segfault-35.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      312 2019-04-26 13:24:32.000000 PyNormaliz-2.9/tests/segfault-45.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     2205 2019-05-01 16:58:20.000000 PyNormaliz-2.9/tests/test_rational_cones.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      286 2019-04-26 13:24:32.000000 PyNormaliz-2.9/tests/vertex_denom-37.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      407 2019-04-26 13:24:32.000000 PyNormaliz-2.9/tests/volume_20.txt
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)      251 2019-04-26 13:24:32.000000 PyNormaliz-2.9/tests/volume_22.txt
```

### Comparing `PyNormaliz-2.8/COPYING` & `PyNormaliz-2.9/COPYING`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/GPLv2` & `PyNormaliz-2.9/GPLv2`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/NormalizModule.cpp` & `PyNormaliz-2.9/NormalizModule.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 /***************************************************************************
  *
  * Include
  *
  ***************************************************************************/
 
 #include <Python.h>
-using namespace std;
-
-#ifdef ENFNORMALIZ
-#include <e-antic/renfxx.h>
-#endif
-
-#include <iostream>
-using std::cerr;
-using std::cout;
-using std::endl;
 
 #include <string>
 using std::string;
 
 #include <libnormaliz/cone.h>
 #include <libnormaliz/map_operations.h>
 #include <libnormaliz/vector_operations.h>
@@ -27,14 +17,20 @@
 using libnormaliz::Cone;
 // using libnormaliz::ConeProperty;
 using libnormaliz::ConeProperties;
 using libnormaliz::Sublattice_Representation;
 using libnormaliz::Type::InputType;
 using libnormaliz::AutomorphismGroup;
 
+#ifdef LIBNORMALIZ_DYNAMIC_BITSET_H
+using libnormaliz::dynamic_bitset;
+#else
+typedef boost::dynamic_bitset<> dynamic_bitset;
+#endif
+
 #include <vector>
 using std::map;
 using std::pair;
 using std::vector;
 
 #include <csignal>
 
@@ -48,31 +44,28 @@
 
 #define FUNC_BEGIN try {
 
 #define FUNC_END                                                             \
     }                                                                        \
     catch (libnormaliz::InterruptException & e)                              \
     {                                                                        \
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);             \
         libnormaliz::nmz_interrupted = false;                                \
         PyErr_SetString(PyExc_KeyboardInterrupt,                             \
                         "interrupted Normaliz Computation");                 \
         PyErr_SetInterrupt();                                                \
         PyErr_CheckSignals();                                                \
         return NULL;                                                         \
     }                                                                        \
     catch (libnormaliz::NormalizException & e)                               \
     {                                                                        \
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);             \
         PyErr_SetString(NormalizError, e.what());                            \
         return NULL;                                                         \
     }                                                                        \
-    catch (exception & e)                                                    \
+    catch (std::exception & e)                                               \
     {                                                                        \
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);             \
         PyErr_SetString(PyNormaliz_cppError, e.what());                      \
         return NULL;                                                         \
     }
 
 
 class PyNormalizInputException : public std::exception {
   private:
@@ -98,39 +91,47 @@
 
 /***************************************************************************
  *
  * Signal handling
  *
  ***************************************************************************/
 
-void signal_handler(int signal)
+static void signal_handler(int signal)
 {
     libnormaliz::nmz_interrupted = true;
 }
 
+// helper class implementing RAII pattern for our custom SIGINT handler;
+// it helps ensure we *always* restore the signal handler inside a
+// FUNC_BEGIN / FUNC_END block.
+class TempSignalHandler {
+    PyOS_sighandler_t original_handler;
+public:
+    TempSignalHandler() {
+        original_handler = PyOS_setsig(SIGINT, signal_handler);
+    }
+
+    ~TempSignalHandler() {
+        PyOS_setsig(SIGINT, original_handler);
+    }
+};
+
 /***************************************************************************
  *
  * Static objects
  *
  ***************************************************************************/
 
 
 static PyObject*   NormalizError;
 static PyObject*   PyNormaliz_cppError;
 static const char* cone_name = "Cone";
 static const char* cone_name_long = "Cone<long long>";
 static const char* cone_name_renf = "Cone<renf_elem>";
 
-static string cone_name_str(cone_name);
-static string cone_name_str_long(cone_name_long);
-static string cone_name_str_renf(cone_name_renf);
-
-
-static PyOS_sighandler_t current_interpreter_sigint_handler;
-
 static PyObject* RationalHandler = NULL;
 
 #ifdef ENFNORMALIZ
 static PyObject* NumberfieldElementHandler = NULL;
 #endif
 
 static PyObject* VectorHandler = NULL;
@@ -138,15 +139,15 @@
 
 /***************************************************************************
  *
  * Call func on one argument
  *
  ***************************************************************************/
 
-PyObject* CallPythonFuncOnOneArg(PyObject* function, PyObject* single_arg)
+static PyObject* CallPythonFuncOnOneArg(PyObject* function, PyObject* single_arg)
 {
     PyObject* single_arg_tuple = PyTuple_Pack(1, single_arg);
     PyObject* return_obj = PyObject_CallObject(function, single_arg_tuple);
     Py_DecRef(single_arg);
     Py_DecRef(single_arg_tuple);
     return return_obj;
 }
@@ -159,50 +160,31 @@
 
 #if PY_MAJOR_VERSION >= 3
 #define string_check PyUnicode_Check
 #else
 #define string_check PyString_Check
 #endif
 
-// Hacky 64-bit check. Works for windows and gcc, probably not clang.
-// Check windows
-#if _WIN32 || _WIN64
-#if _WIN64
-#define ENVIRONMENT64
-#else
-#define ENVIRONMENT32
-#endif
-#endif
-
-// Check GCC
-#if __GNUC__
-#if __x86_64__ || __ppc64__ || __aarch64__
-#define ENVIRONMENT64
-#else
-#define ENVIRONMENT32
-#endif
-#endif
-
 #ifndef NMZ_RELEASE
 static_assert(
     false,
-    "Your Normaliz version (unknown) is to old! Update to 3.7.0 or newer.");
+    "Your Normaliz version (unknown) is to old! Update to 3.8.3 or newer.");
 #endif
 #if NMZ_RELEASE < 30700
 static_assert(false,
-              "Your Normaliz version is to old! Update to 3.7.0 or newer.");
+              "Your Normaliz version is to old! Update to 3.8.3 or newer.");
 #endif
 
 /***************************************************************************
  *
  * Python-C data conversion functions
  *
  ***************************************************************************/
 
-string PyUnicodeToString(PyObject* in)
+static string PyUnicodeToString(PyObject* in)
 {
     if (!string_check(in)) {
         throw PyNormalizInputException("input must be a string");
         return NULL;
     }
 #if PY_MAJOR_VERSION >= 3
     string out = "";
@@ -213,37 +195,37 @@
     return out;
 #else
     char* out = PyString_AsString(in);
     return string(out);
 #endif
 }
 
-PyObject* StringToPyUnicode(string in)
+static PyObject* StringToPyUnicode(const string &in)
 {
 #if PY_MAJOR_VERSION >= 3
     return PyUnicode_FromString(in.c_str());
 #else
     return PyString_FromString(in.c_str());
 #endif
 }
 
 // Boolean conversion
 
-inline PyObject* BoolToPyBool(bool in)
+static inline PyObject* BoolToPyBool(bool in)
 {
     if (in)
         Py_RETURN_TRUE;
     Py_RETURN_FALSE;
 }
 
 // Converting MPZ's to PyLong and back via strings. Worst possible solution
 // ever.
-bool PyNumberToNmz(PyObject*, mpz_class&);
+static bool PyNumberToNmz(PyObject*, mpz_class&);
 
-bool PyNumberToNmz(PyObject* in, mpq_class& out)
+static bool PyNumberToNmz(PyObject* in, mpq_class& out)
 {
     if (PyFloat_Check(in)) {
         out = mpq_class(PyFloat_AsDouble(in));
         return true;
     }
 #if PY_MAJOR_VERSION < 3
     if (PyInt_Check(in)) {
@@ -272,25 +254,24 @@
             return false;
         }
         out = mpq_class(num, denom);
         return true;
     }
     PyObject*   in_as_string = PyObject_Str(in);
     string      s = PyUnicodeToString(in_as_string);
-    const char* in_as_c_string = s.c_str();
-    int         check = out.set_str(in_as_c_string, 10);
+    int         check = out.set_str(s.c_str(), 10);
     if (check == -1) {
         throw PyNormalizInputException(
             "coefficient in matrix must be PyFloat, PyInt, PyLong, Sequence, "
             "must be able to be converted to a valid gmp input string");
     }
     return true;
 }
 
-bool PyNumberToNmz(PyObject* in, mpz_class& out)
+static bool PyNumberToNmz(PyObject* in, mpz_class& out)
 {
 #if PY_MAJOR_VERSION < 3
     if (PyInt_Check(in)) {
         out = PyInt_AsLong(in);
         return true;
     }
 #endif
@@ -302,88 +283,87 @@
     long input_long = PyLong_AsLongAndOverflow(in, &overflow);
     if (overflow == 0) {
         out = mpz_class(input_long);
         return true;
     }
     PyObject*   in_as_string = PyObject_Str(in);
     string      s = PyUnicodeToString(in_as_string);
-    const char* in_as_c_string = s.c_str();
-    out.set_str(in_as_c_string, 10);
+    out.set_str(s.c_str(), 10);
     return true;
 }
 
-PyObject* NmzToPyNumber(const mpz_class in)
+static PyObject* NmzToPyNumber(const mpz_class in)
 {
     if (in.fits_slong_p()) {
         return PyLong_FromLong(in.get_si());
     }
-    string    mpz_as_string = in.get_str();
+
+    // in Python 2, the first argument to PyLong_FromString is not const, thus
+    // we need to perform a const cast here.
+    string    mpz_as_string = in.get_str(16);
     char*     mpz_as_c_string = const_cast< char* >(mpz_as_string.c_str());
-    PyObject* ret_val = PyLong_FromString(mpz_as_c_string, NULL, 10);
-    return ret_val;
+    return PyLong_FromString(mpz_as_c_string, NULL, 16);
 }
 
-PyObject* NmzToPyNumber(const mpq_class in)
+static PyObject* NmzToPyNumber(const mpq_class in)
 {
     PyObject* out_list = PyList_New(2);
     PyList_SetItem(out_list, 0, NmzToPyNumber(in.get_num()));
     PyList_SetItem(out_list, 1, NmzToPyNumber(in.get_den()));
     if (RationalHandler != NULL)
         out_list = CallPythonFuncOnOneArg(RationalHandler, out_list);
     return out_list;
 }
 
-bool PyNumberToNmz(PyObject* in, long long& out)
+static bool PyNumberToNmz(PyObject* in, long long& out)
 {
     int overflow;
     out = PyLong_AsLongLongAndOverflow(in, &overflow);
     if (overflow == -1)
         throw PyNormalizInputException(
             "Cannot store input coefficient in long long");
     return true;
 }
 
-PyObject* NmzToPyNumber(long long in)
+static PyObject* NmzToPyNumber(unsigned int in)
 {
-    return PyLong_FromLongLong(in);
+    return PyLong_FromUnsignedLong(in);
 }
 
-PyObject* NmzToPyNumber(libnormaliz::key_t in)
+static PyObject* NmzToPyNumber(unsigned long in)
 {
-    return PyLong_FromLong(in);
+    return PyLong_FromUnsignedLong(in);
 }
 
-#ifdef ENVIRONMENT64
-PyObject* NmzToPyNumber(size_t in)
+static PyObject* NmzToPyNumber(int in)
 {
     return PyLong_FromLong(in);
 }
-#endif
 
-PyObject* NmzToPyNumber(int in)
+static PyObject* NmzToPyNumber(long in)
 {
     return PyLong_FromLong(in);
 }
 
-PyObject* NmzToPyNumber(long in)
+static PyObject* NmzToPyNumber(long long in)
 {
-    return PyLong_FromLong(in);
+    return PyLong_FromLongLong(in);
 }
 
-PyObject* NmzToPyNumber(double in)
+static PyObject* NmzToPyNumber(double in)
 {
     return PyFloat_FromDouble(in);
 }
 
 template < typename Integer >
-PyObject* NmzVectorToPyList(const vector< Integer >& in,
+static PyObject* NmzVectorToPyList(const vector< Integer >& in,
                             bool                     do_callback = true);
 
 #ifdef ENFNORMALIZ
-PyObject* NmzToPyNumber(renf_elem_class in)
+static PyObject* NmzToPyNumber(const renf_elem_class &in)
 {
     vector< mpz_class > output_nums = in.get_num_vector();
     mpz_class           output_den = in.get_den();
     PyObject*           denom_py = NmzToPyNumber(output_den);
     PyObject*           out_list = PyList_New(output_nums.size());
     for (size_t i = 0; i < output_nums.size(); i++) {
         PyObject* current = PyList_New(2);
@@ -398,14 +378,24 @@
     if (NumberfieldElementHandler != NULL)
         out_list =
             CallPythonFuncOnOneArg(NumberfieldElementHandler, out_list);
     return out_list;
 }
 #endif
 
+PyObject* NmzToPyNumber(const dynamic_bitset& in)
+{
+    size_t    len = in.size();
+    PyObject* result = PyList_New(len);
+    for (size_t i = 0; i < len; i++) {
+        PyList_SetItem(result, i, NmzToPyNumber(in[i] ? 1 : 0));
+    }
+    return result;
+}
+
 template < typename Integer >
 static bool PyListToNmz(vector< Integer >& out, PyObject* in)
 {
     if (!PySequence_Check(in))
         throw PyNormalizInputException("Input list is not a sequence");
     const int n = PySequence_Size(in);
     out.resize(n);
@@ -430,15 +420,15 @@
             return false;
     }
     return true;
 }
 
 #ifdef ENFNORMALIZ
 template < typename NumberField, typename NumberFieldElem >
-bool prepare_nf_input(vector< vector< NumberFieldElem > >& out,
+static bool prepare_nf_input(vector< vector< NumberFieldElem > >& out,
                       PyObject*                            in,
                       NumberField*                         nf)
 {
     if (!PySequence_Check(in))
         throw PyNormalizInputException("Number field data is not a list");
     const int nr = PySequence_Size(in);
     out.resize(nr);
@@ -482,85 +472,53 @@
     return true;
 }
 #endif
 
 template < typename Integer >
 static bool PyInputToNmz(vector< vector< Integer > >& out, PyObject* in)
 {
-    bool check_input;
-    check_input = PyIntMatrixToNmz(out, in);
-    if (check_input)
+    if (PyIntMatrixToNmz(out, in))
         return true;
     out.resize(1);
-    check_input = PyListToNmz(out[0], in);
-    if (check_input) {
+    if (PyListToNmz(out[0], in)) {
         return true;
     }
     throw PyNormalizInputException(
         "Input could not be converted to vector or list");
 }
 
 template < typename Integer >
-PyObject* NmzVectorToPyList(const vector< Integer >& in, bool do_callback)
+static PyObject* NmzVectorToPyList(const vector< Integer >& in, bool do_callback)
 {
     PyObject*    vector;
     const size_t n = in.size();
     vector = PyList_New(n);
     for (size_t i = 0; i < n; ++i) {
         PyList_SetItem(vector, i, NmzToPyNumber(in[i]));
     }
     if (do_callback && VectorHandler != NULL)
         vector = CallPythonFuncOnOneArg(VectorHandler, vector);
     return vector;
 }
 
-template PyObject* NmzVectorToPyList(const vector< mpq_class >& in,
-                                     bool                       do_callback);
-
-PyObject* NmzBoolVectorToPyList(const vector< bool >& in)
-{
-    PyObject*    vector;
-    const size_t n = in.size();
-    vector = PyList_New(n);
-    for (size_t i = 0; i < n; ++i) {
-        PyList_SetItem(vector, i, BoolToPyBool(in[i]));
-    }
-    if (VectorHandler != NULL)
-        vector = CallPythonFuncOnOneArg(VectorHandler, vector);
-    return vector;
-}
-
-PyObject* NmzBoolMatrixToPyList(const vector< vector< bool > >& in)
-{
-    PyObject*    matrix;
-    const size_t n = in.size();
-    matrix = PyList_New(n);
-    for (size_t i = 0; i < n; ++i) {
-        PyList_SetItem(matrix, i, NmzBoolVectorToPyList(in[i]));
-    }
-    if (MatrixHandler != NULL)
-        matrix = CallPythonFuncOnOneArg(MatrixHandler, matrix);
-    return matrix;
-}
-
 template < typename Integer >
-PyObject* NmzMatrixToPyList(const vector< vector< Integer > >& in)
+static PyObject* NmzMatrixToPyList(const vector< vector< Integer > >& in)
 {
     PyObject*    matrix;
     const size_t n = in.size();
     matrix = PyList_New(n);
     for (size_t i = 0; i < n; ++i) {
         PyList_SetItem(matrix, i, NmzVectorToPyList(in[i]));
     }
     if (MatrixHandler != NULL)
         matrix = CallPythonFuncOnOneArg(MatrixHandler, matrix);
     return matrix;
 }
 
-PyObject* NmzHilbertSeriesToPyList(const libnormaliz::HilbertSeries& HS,
+static PyObject* NmzHilbertSeriesToPyList(const libnormaliz::HilbertSeries& HS,
                                    bool                              is_HSOP)
 {
     PyObject* return_list = PyList_New(3);
     if (is_HSOP) {
         PyList_SetItem(return_list, 0, NmzVectorToPyList(HS.getHSOPNum()));
         PyList_SetItem(
             return_list, 1,
@@ -574,44 +532,44 @@
             NmzVectorToPyList(libnormaliz::to_vector(HS.getDenom())));
         PyList_SetItem(return_list, 2, NmzToPyNumber(HS.getShift()));
     }
     return return_list;
 }
 
 template < typename Integer >
-PyObject* NmzWeightedEhrhartSeriesToPyList(
+static PyObject* NmzWeightedEhrhartSeriesToPyList(
     const std::pair< libnormaliz::HilbertSeries, Integer >& HS)
 {
     PyObject* return_list = PyList_New(4);
     PyList_SetItem(return_list, 0, NmzVectorToPyList(HS.first.getNum()));
     PyList_SetItem(
         return_list, 1,
         NmzVectorToPyList(libnormaliz::to_vector(HS.first.getDenom())));
     PyList_SetItem(return_list, 2, NmzToPyNumber(HS.first.getShift()));
     PyList_SetItem(return_list, 3, NmzToPyNumber(HS.second));
     return return_list;
 }
 
 template < typename Integer >
-PyObject*
+static PyObject*
 NmzHilbertQuasiPolynomialToPyList(const libnormaliz::HilbertSeries& HS)
 {
     vector< vector< Integer > > HQ = HS.getHilbertQuasiPolynomial();
     const size_t                n = HS.getPeriod();
     PyObject*                   return_list = PyList_New(n + 1);
     for (size_t i = 0; i < n; ++i) {
         PyList_SetItem(return_list, i, NmzVectorToPyList(HQ[i]));
     }
     PyList_SetItem(return_list, n,
                    NmzToPyNumber(HS.getHilbertQuasiPolynomialDenom()));
     return return_list;
 }
 
 template < typename Integer >
-PyObject* NmzWeightedEhrhartQuasiPolynomialToPyList(
+static PyObject* NmzWeightedEhrhartQuasiPolynomialToPyList(
     const libnormaliz::IntegrationData& int_data)
 {
     vector< vector< Integer > > ehrhart_qp =
         int_data.getWeightedEhrhartQuasiPolynomial();
     const size_t n = ehrhart_qp.size();
     PyObject*    return_list = PyList_New(n + 1);
     for (size_t i = 0; i < n; ++i) {
@@ -620,15 +578,15 @@
     PyList_SetItem(
         return_list, n,
         NmzToPyNumber(int_data.getWeightedEhrhartQuasiPolynomialDenom()));
     return return_list;
 }
 
 template < typename Integer >
-PyObject* NmzTriangleListToPyList(
+static PyObject* NmzTriangleListToPyList(
     const vector< pair< vector< libnormaliz::key_t >, Integer > >& in)
 {
     const size_t n = in.size();
     PyObject*    M = PyList_New(n);
     for (size_t i = 0; i < n; ++i) {
         // convert the pair
         PyObject* pair = PyList_New(2);
@@ -637,32 +595,32 @@
         PyList_SetItem(pair, 1, NmzToPyNumber(in[i].second));
         PyList_SetItem(M, i, pair);
     }
     return M;
 }
 
 template < typename Integer >
-PyObject*
+static PyObject*
 NmzStanleyDataToPyList(const libnormaliz::STANLEYDATA< Integer >& StanleyData)
 {
     PyObject* pair = PyList_New(2);
     PyList_SetItem(pair, 0,
                    NmzVectorToPyList< libnormaliz::key_t >(StanleyData.key));
     PyList_SetItem(pair, 1,
                    NmzMatrixToPyList(StanleyData.offsets.get_elements()));
     return pair;
 }
 
 template < typename Integer >
-PyObject* NmzStanleyDecToPyList(
-    const list< libnormaliz::STANLEYDATA< Integer > >& StanleyDec)
+static PyObject* NmzStanleyDecToPyList(
+    const std::list< libnormaliz::STANLEYDATA< Integer > >& StanleyDec)
 {
     const size_t n = StanleyDec.size();
     PyObject*    M = PyList_New(n);
-    typename list< libnormaliz::STANLEYDATA< Integer > >::const_iterator S =
+    typename std::list< libnormaliz::STANLEYDATA< Integer > >::const_iterator S =
         StanleyDec.begin();
     for (size_t i = 0; i < n; ++i) {
         PyList_SetItem(M, i, NmzStanleyDataToPyList(*S));
         ++S;
     }
     return M;
 }
@@ -677,33 +635,23 @@
     PyList_SetItem(res, 1, NmzMatrixToPyList(bc.getProjection()));
     PyList_SetItem(res, 2, NmzToPyNumber(bc.getAnnihilator()));
     // Dim, Rank, Equations and Congruences are already covered by special
     // functions ditto ExternalIndex
     return res;
 }
 
-static PyObject* NmzBitsetToPyList(const boost::dynamic_bitset<>& bits)
-{
-    ssize_t   len = bits.size();
-    PyObject* list = PyList_New(len);
-    for (ssize_t i = 0; i < len; i++) {
-        PyList_SetItem(list, i, BoolToPyBool(bits[i]));
-    }
-    return list;
-}
-
 static PyObject*
-NmzFacelatticeToPython(const map< boost::dynamic_bitset<>, int >& lattice)
+NmzFacelatticeToPython(const map<dynamic_bitset, int>& lattice)
 {
     ssize_t   len = lattice.size();
     PyObject* list = PyList_New(len);
     ssize_t   curr = 0;
     for (auto it = lattice.begin(); it != lattice.end(); it++) {
         PyObject* list_int = PyList_New(2);
-        PyList_SetItem(list_int, 0, NmzBitsetToPyList(it->first));
+        PyList_SetItem(list_int, 0, NmzToPyNumber(it->first));
         PyList_SetItem(list_int, 1, NmzToPyNumber(it->second));
         PyList_SetItem(list, curr, list_int);
         curr++;
     }
     return list;
 }
 
@@ -745,132 +693,127 @@
 #ifdef ENFNORMALIZ
 struct NumberFieldCone {
     renf_class*              nf;
     Cone< renf_elem_class >* cone;
 };
 #endif
 
-void delete_cone_mpz(PyObject* cone)
+static void delete_cone_mpz(PyObject* cone)
 {
     Cone< mpz_class >* cone_ptr = reinterpret_cast< Cone< mpz_class >* >(
         PyCapsule_GetPointer(cone, cone_name));
     delete cone_ptr;
 }
 
-void delete_cone_long(PyObject* cone)
+static void delete_cone_long(PyObject* cone)
 {
     Cone< long long >* cone_ptr = reinterpret_cast< Cone< long long >* >(
         PyCapsule_GetPointer(cone, cone_name_long));
     delete cone_ptr;
 }
 
 #ifdef ENFNORMALIZ
-void delete_cone_renf(PyObject* cone)
+static void delete_cone_renf(PyObject* cone)
 {
     NumberFieldCone* cone_ptr = reinterpret_cast< NumberFieldCone* >(
         PyCapsule_GetPointer(cone, cone_name_renf));
     delete cone_ptr->cone;
     // delete cone_ptr->nf;
 }
 #endif
 
-Cone< long long >* get_cone_long(PyObject* cone)
+static Cone< long long >* get_cone_long(PyObject* cone)
 {
     return reinterpret_cast< Cone< long long >* >(
         PyCapsule_GetPointer(cone, cone_name_long));
 }
 
-Cone< mpz_class >* get_cone_mpz(PyObject* cone)
+static Cone< mpz_class >* get_cone_mpz(PyObject* cone)
 {
     return reinterpret_cast< Cone< mpz_class >* >(
         PyCapsule_GetPointer(cone, cone_name));
 }
 
 #ifdef ENFNORMALIZ
-Cone< renf_elem_class >* get_cone_renf(PyObject* cone)
+static Cone< renf_elem_class >* get_cone_renf(PyObject* cone)
 {
     NumberFieldCone* cone_ptr = reinterpret_cast< NumberFieldCone* >(
         PyCapsule_GetPointer(cone, cone_name_renf));
     return cone_ptr->cone;
 }
 
-renf_class* get_cone_renf_renf(PyObject* cone)
+static renf_class* get_cone_renf_renf(PyObject* cone)
 {
     NumberFieldCone* cone_ptr = reinterpret_cast< NumberFieldCone* >(
         PyCapsule_GetPointer(cone, cone_name_renf));
     return cone_ptr->nf;
 }
 #endif
 
-PyObject* pack_cone(Cone< mpz_class >* C, void* dummy = nullptr)
+static PyObject* pack_cone(Cone< mpz_class >* C, void* dummy = nullptr)
 {
     return PyCapsule_New(reinterpret_cast< void* >(C), cone_name,
                          &delete_cone_mpz);
 }
 
-PyObject* pack_cone(Cone< long long >* C, void* dummy = nullptr)
+static PyObject* pack_cone(Cone< long long >* C, void* dummy = nullptr)
 {
     return PyCapsule_New(reinterpret_cast< void* >(C), cone_name_long,
                          &delete_cone_long);
 }
 
 #ifdef ENFNORMALIZ
-PyObject* pack_cone(Cone< renf_elem_class >* C, void* nf = nullptr)
+static PyObject* pack_cone(Cone< renf_elem_class >* C, void* nf)
 {
     NumberFieldCone* cone_ptr = new NumberFieldCone();
     cone_ptr->nf = reinterpret_cast< renf_class* >(nf);
     cone_ptr->cone = C;
     return PyCapsule_New(reinterpret_cast< void* >(cone_ptr), cone_name_renf,
                          &delete_cone_renf);
 }
-
-PyObject* pack_cone(Cone< renf_elem_class >* C)
-{
-    PyErr_SetString(PyNormaliz_cppError,
-                    "Trying to pack renf cone without number field");
-    return NULL;
-}
 #endif
 
-bool is_cone(PyObject* cone)
+static bool is_cone(PyObject* cone)
 {
     if (PyCapsule_CheckExact(cone)) {
-        string current = string(PyCapsule_GetName(cone));
-        return cone_name_str == current || cone_name_str_long == current ||
-               cone_name_str_renf == current;
+        const char *name = PyCapsule_GetName(cone);
+        return !strcmp(name, cone_name) || !strcmp(name, cone_name_long) ||
+               !strcmp(name, cone_name_renf);
     }
     return false;
 }
 
-bool is_cone_mpz(PyObject* cone)
+static bool is_cone_mpz(PyObject* cone)
 {
     if (PyCapsule_CheckExact(cone)) {
-        string current = string(PyCapsule_GetName(cone));
-        return current == cone_name_str;
+        const char *name = PyCapsule_GetName(cone);
+        return !strcmp(name, cone_name);
     }
     return false;
 }
 
-bool is_cone_long(PyObject* cone)
+static bool is_cone_long(PyObject* cone)
 {
     if (PyCapsule_CheckExact(cone)) {
-        string current = string(PyCapsule_GetName(cone));
-        return current == cone_name_str_long;
+        const char *name = PyCapsule_GetName(cone);
+        return !strcmp(name, cone_name_long);
     }
     return false;
 }
 
-bool is_cone_renf(PyObject* cone)
+#ifdef ENFNORMALIZ
+static bool is_cone_renf(PyObject* cone)
 {
     if (PyCapsule_CheckExact(cone)) {
-        string current = string(PyCapsule_GetName(cone));
-        return current == cone_name_str_renf;
+        const char *name = PyCapsule_GetName(cone);
+        return !strcmp(name, cone_name_renf);
     }
     return false;
 }
+#endif
 
 /***************************************************************************
  *
  * Cone property list
  *
  ***************************************************************************/
 
@@ -891,22 +834,17 @@
 */
 static PyObject* NmzListConeProperties(PyObject* args)
 {
     FUNC_BEGIN
 
     PyObject* return_list = PyList_New(2);
 
-    ConeProperties props;
-    for (int i = 0; i < libnormaliz::ConeProperty::EnumSize; i++) {
-        props.set(static_cast< libnormaliz::ConeProperty::Enum >(i));
-    }
-
-    ConeProperties goals = props.goals();
-    ConeProperties options = props.options();
-
+    ConeProperties goals = libnormaliz::all_goals();
+    ConeProperties options = libnormaliz::all_options();
+    
     int number_goals = goals.count();
     int number_options = options.count();
 
     PyObject* goal_list = PyList_New(number_goals);
     PyObject* option_list = PyList_New(number_options);
 
     PyList_SetItem(return_list, 0, goal_list);
@@ -1135,15 +1073,15 @@
 Normaliz input types, and the values for the keys matrices
 (consisting of either Longs, Floats, or strings for rationals),
 lists for single vector input types, or bools for boolean input type.
 Special cases are a string describing a polynomial for the polynomial
 input type, and the CreateAsLongLong keyword to restrict normaliz computations
 to machine integers instead of arbitrary precision numbers.
 */
-PyObject* _NmzCone(PyObject* self, PyObject* args, PyObject* kwargs)
+static PyObject* _NmzCone(PyObject* self, PyObject* args, PyObject* kwargs)
 {
     FUNC_BEGIN
 
     static const char* string_for_long = "CreateAsLongLong";
     PyObject* create_as_long_long = StringToPyUnicode(string_for_long);
 #ifdef ENFNORMALIZ
     static const char* string_for_renf = "number_field";
@@ -1167,37 +1105,35 @@
 
 /*
 @Name NmzConeCopy
 @Arguments Cone
 @Description
 Returns a copy of the cone.
 */
-PyObject* _NmzConeCopy(PyObject* self, PyObject* args)
+static PyObject* _NmzConeCopy(PyObject* self, PyObject* args)
 {
     FUNC_BEGIN
     PyObject* cone = PyTuple_GetItem(args, 0);
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
 
-    string current_name = string(PyCapsule_GetName(cone));
-
-    if (cone_name_str == current_name) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         Cone< mpz_class >* new_cone = new Cone< mpz_class >(*cone_ptr);
         return pack_cone(new_cone);
     }
-    else if (cone_name_str_long == current_name) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         Cone< long long >* new_cone = new Cone< long long >(*cone_ptr);
         return pack_cone(new_cone);
     }
 #ifdef ENFNORMALIZ
-    else {
+    else if (is_cone_renf(cone)) {
         Cone< renf_elem_class >* cone_ptr = get_cone_renf(cone);
         Cone< renf_elem_class >* new_cone =
             new Cone< renf_elem_class >(*cone_ptr);
         return pack_cone(new_cone, get_cone_renf_renf(cone));
     }
 #endif
     Py_RETURN_NONE;
@@ -1207,15 +1143,15 @@
 /***************************************************************************
  *
  * NmzHilbertSeries
  *
  ***************************************************************************/
 
 template < typename Integer >
-PyObject* NmzHilbertSeries(Cone< Integer >* C, PyObject* args)
+static PyObject* NmzHilbertSeries(Cone< Integer >* C, PyObject* args)
 {
     FUNC_BEGIN
 
     const int arg_len = PyTuple_Size(args);
 
     if (arg_len == 1) {
         bool is_HSOP = C->isComputed(libnormaliz::ConeProperty::HSOP);
@@ -1232,42 +1168,37 @@
     else {
         return NmzHilbertSeriesToPyList(C->getHilbertSeries(), false);
     }
     FUNC_END
 }
 
 
-PyObject* NmzHilbertSeries_Outer(PyObject* self, PyObject* args)
+static PyObject* NmzHilbertSeries_Outer(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
     PyObject* cone = PyTuple_GetItem(args, 0);
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
 
-    current_interpreter_sigint_handler = PyOS_setsig(SIGINT, signal_handler);
-    string current_name = string(PyCapsule_GetName(cone));
-    if (cone_name_str == current_name) {
+    TempSignalHandler tmpHandler; // use custom signal handler
+
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
-        PyObject*          return_value = NmzHilbertSeries(cone_ptr, args);
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-        return return_value;
+        return NmzHilbertSeries(cone_ptr, args);
     }
-    else if (cone_name_str_long == current_name) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
-        PyObject*          return_value = NmzHilbertSeries(cone_ptr, args);
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-        return return_value;
+        return NmzHilbertSeries(cone_ptr, args);
     }
     else {
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
         PyErr_SetString(PyNormaliz_cppError,
                         "Hilbert series not available for renf cone");
         return NULL;
     }
     FUNC_END
 }
 
@@ -1275,15 +1206,15 @@
  *
  * NmzCompute
  *
  ***************************************************************************/
 
 
 template < typename Integer >
-PyObject* _NmzCompute(Cone< Integer >* C, PyObject* args)
+static PyObject* _NmzCompute(Cone< Integer >* C, PyObject* args)
 {
     FUNC_BEGIN
 
     const int arg_len = PyTuple_Size(args);
 
     PyObject* to_compute;
 
@@ -1303,15 +1234,15 @@
                 return NULL;
             }
         }
     }
     else {
         to_compute = PyList_New(arg_len - 1);
         for (int i = 1; i < arg_len; i++) {
-            PyList_SetItem(to_compute, i, PyTuple_GetItem(args, i));
+            PyList_SetItem(to_compute, i-1, PyTuple_GetItem(args, i));
         }
     }
 
     ConeProperties propsToCompute;
     const int      n = PySequence_Size(to_compute);
 
     for (int i = 0; i < n; ++i) {
@@ -1332,47 +1263,45 @@
     // we return a bool, true when everything requested was computed
     Py_DecRef(to_compute);
     return BoolToPyBool(notComputed.goals().none());
     FUNC_END
 }
 
 
-PyObject* _NmzCompute_Outer(PyObject* self, PyObject* args)
+static PyObject* _NmzCompute_Outer(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
-    current_interpreter_sigint_handler = PyOS_setsig(SIGINT, signal_handler);
-
     PyObject* cone = PyTuple_GetItem(args, 0);
 
     PyObject* result = NULL;
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    TempSignalHandler tmpHandler; // use custom signal handler
+
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         result = _NmzCompute(cone_ptr, args);
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         result = _NmzCompute(cone_ptr, args);
     }
 #ifdef ENFNORMALIZ
-    else {
+    else if (is_cone_renf(cone)) {
         Cone< renf_elem_class >* cone_ptr = get_cone_renf(cone);
         result = _NmzCompute(cone_ptr, args);
     }
 #endif
 
-    PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-
     return result;
 
     FUNC_END
 }
 
 /***************************************************************************
  *
@@ -1410,41 +1339,39 @@
 #endif
 
 PyObject* _NmzModify_Outer(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
-    current_interpreter_sigint_handler = PyOS_setsig(SIGINT, signal_handler);
-
     PyObject* cone = PyTuple_GetItem(args, 0);
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    TempSignalHandler tmpHandler; // use custom signal handler
+
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         return _NmzModify(cone_ptr, args);
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         return _NmzModify(cone_ptr, args);
     }
 #ifdef ENFNORMALIZ
-    else {
+    else if (is_cone_renf(cone)) {
         Cone< renf_elem_class >* cone_ptr = get_cone_renf(cone);
         renf_class* nf = get_cone_renf_renf(cone);
         return _NmzModify_Renf(cone_ptr, nf, args);
     }
 #endif
 
-    PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-
     Py_RETURN_TRUE;
 
     FUNC_END
 }
 
 /***************************************************************************
  *
@@ -1455,48 +1382,48 @@
 /*
 @Name NmzIsComputed
 @Arguments <cone>, <property_string>
 @Desctiption
 Returns if the cone property <property_string> is computed in the cone <cone>.
 */
 template < typename Integer >
-PyObject* NmzIsComputed(Cone< Integer >* C, PyObject* prop)
+static PyObject* NmzIsComputed(Cone< Integer >* C, PyObject* prop)
 {
     FUNC_BEGIN
 
     libnormaliz::ConeProperty::Enum p =
         libnormaliz::toConeProperty(PyUnicodeToString(prop));
 
     return BoolToPyBool(C->isComputed(p));
 
     FUNC_END
 }
 
-PyObject* NmzIsComputed_Outer(PyObject* self, PyObject* args)
+static PyObject* NmzIsComputed_Outer(PyObject* self, PyObject* args)
 {
     FUNC_BEGIN
 
     PyObject* cone = PyTuple_GetItem(args, 0);
     PyObject* to_compute = PyTuple_GetItem(args, 1);
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         return NmzIsComputed(cone_ptr, to_compute);
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         return NmzIsComputed(cone_ptr, to_compute);
     }
 #ifdef ENFNORMALIZ
-    else {
+    else if (is_cone_renf(cone)) {
         Cone< renf_elem_class >* cone_ptr = get_cone_renf(cone);
         return NmzIsComputed(cone_ptr, to_compute);
     }
 #endif
     Py_RETURN_FALSE;
 
     FUNC_END
@@ -1505,37 +1432,37 @@
 /***************************************************************************
  *
  * NmzSetGrading
  *
  ***************************************************************************/
 
 template < typename Integer >
-PyObject* NmzSetGrading_inner(Cone< Integer >* cone, PyObject* list)
+static PyObject* NmzSetGrading_inner(Cone< Integer >* cone, PyObject* list)
 {
     vector< Integer > list_c;
     bool              result = PyListToNmz(list_c, list);
     if (!result) {
         PyErr_SetString(PyNormaliz_cppError,
                         "grading argument is not an integer list");
         return NULL;
     }
     cone->resetGrading(list_c);
     Py_RETURN_NONE;
 }
 
-PyObject* NmzSetGrading(PyObject* self, PyObject* args)
+static PyObject* NmzSetGrading(PyObject* self, PyObject* args)
 {
     FUNC_BEGIN
     PyObject* cone = PyTuple_GetItem(args, 0);
     PyObject* grading_py = PyTuple_GetItem(args, 1);
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         return NmzSetGrading_inner(cone_ptr, grading_py);
     }
     else {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         return NmzSetGrading_inner(cone_ptr, grading_py);
     }
@@ -1570,25 +1497,27 @@
 * IntegerHull and ProjectCone return new cones.
 * StanleyDec
   Returns a list containing the Stanley decomposition. All entries are
 2-tuples. First entry in the tuple is the key, second the decomposition data.
 */
 
 template < typename Integer >
-PyObject*
+static PyObject*
 _NmzResultImpl(Cone< Integer >* C, PyObject* prop_obj, void* nf = nullptr)
 {
 
     string prop = PyUnicodeToString(prop_obj);
 
     libnormaliz::ConeProperty::Enum p = libnormaliz::toConeProperty(prop);
 
-    current_interpreter_sigint_handler = PyOS_setsig(SIGINT, signal_handler);
-    ConeProperties notComputed = C->compute(ConeProperties(p));
-    PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
+    ConeProperties notComputed;
+    {
+    TempSignalHandler tmpHandler; // use custom signal handler
+    notComputed = C->compute(ConeProperties(p));
+    }
 
     if (notComputed.goals().any()) {
         Py_RETURN_NONE;
     }
 
     // Handle standard cases
     libnormaliz::OutputType::Enum outputtype = libnormaliz::output_type(p);
@@ -1608,15 +1537,17 @@
             return NmzHilbertSeriesToPyList(C->getEhrhartSeries(), is_HSOP);
         }
 
         case libnormaliz::ConeProperty::WeightedEhrhartSeries:
             return NmzWeightedEhrhartSeriesToPyList(
                 C->getWeightedEhrhartSeries());
 
-
+        // though Grading has the return type vector<Integer> we make it
+        // a complex struture within PyNormaliz since we want to combine it
+        // with the grading denominator
         case libnormaliz::ConeProperty::Grading: {
             vector< Integer > grad = C->getGrading();
             Integer           denom = C->getGradingDenom();
             PyObject*         return_list = PyList_New(2);
             PyList_SetItem(return_list, 0, NmzVectorToPyList(grad));
             PyList_SetItem(return_list, 1, NmzToPyNumber(denom));
             return return_list;
@@ -1625,19 +1556,21 @@
         case libnormaliz::ConeProperty::StanleyDec:
             return NmzStanleyDecToPyList(C->getStanleyDec());
 
         case libnormaliz::ConeProperty::InclusionExclusionData:
             return NmzTriangleListToPyList< long >(
                 C->getInclusionExclusionData());
 
+        /* returned as a matrix, no need to make it a complex property
         case libnormaliz::ConeProperty::Equations:
             return NmzMatrixToPyList(C->getSublattice().getEquations());
 
         case libnormaliz::ConeProperty::Congruences:
             return NmzMatrixToPyList(C->getSublattice().getCongruences());
+        */
 
         case libnormaliz::ConeProperty::Sublattice:
             return _NmzBasisChangeIntern(C);
 
         case libnormaliz::ConeProperty::ExternalIndex:
             return NmzToPyNumber(C->getSublattice().getExternalIndex());
 
@@ -1660,14 +1593,17 @@
         case libnormaliz::ConeProperty::EhrhartQuasiPolynomial:
             return NmzHilbertQuasiPolynomialToPyList< mpz_class >(
                 C->getEhrhartSeries());
 
         case libnormaliz::ConeProperty::WeightedEhrhartQuasiPolynomial:
             return NmzWeightedEhrhartQuasiPolynomialToPyList< mpz_class >(
                 C->getIntData());
+            
+        case libnormaliz::ConeProperty::ClassGroup:
+            return NmzVectorToPyList(C->getClassGroup());
 
         case libnormaliz::ConeProperty::FVector:
             return NmzVectorToPyList(C->getFVector());
 
         case libnormaliz::ConeProperty::FaceLattice:
             return NmzFacelatticeToPython(C->getFaceLattice());
 
@@ -1687,14 +1623,17 @@
             return NmzAutomorphismsToPython(C->getAutomorphismGroup(
                 libnormaliz::ConeProperty::RationalAutomorphisms));
 
         case libnormaliz::ConeProperty::EuclideanAutomorphisms:
             return NmzAutomorphismsToPython(C->getAutomorphismGroup(
                 libnormaliz::ConeProperty::EuclideanAutomorphisms));
 
+        case libnormaliz::ConeProperty::Incidence:
+            return NmzVectorToPyList(C->getIncidence());
+
         default: {
             switch (outputtype) {
                 case libnormaliz::OutputType::Matrix:
                     return NmzMatrixToPyList(C->getMatrixConeProperty(p));
                 case libnormaliz::OutputType::MatrixFloat:
                     return NmzMatrixToPyList(
                         C->getFloatMatrixConeProperty(p));
@@ -1726,18 +1665,23 @@
                 }
             }
         }
     }
     Py_RETURN_NONE;
 }
 
-PyObject* _NmzResult(PyObject* self, PyObject* args, PyObject* kwargs)
+static PyObject* _NmzResult(PyObject* self, PyObject* args, PyObject* kwargs)
 {
 
     FUNC_BEGIN
+    
+    if(PyTuple_Size(args)!=2){
+        PyErr_SetString(PyNormaliz_cppError, "Exactly one computation goal required for NmzResult");
+        return NULL;        
+    }
 
     PyObject* cone = PyTuple_GetItem(args, 0);
     PyObject* prop = PyTuple_GetItem(args, 1);
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
@@ -1757,24 +1701,24 @@
 #endif
         VectorHandler = PyDict_GetItemString(kwargs, "VectorHandler");
         MatrixHandler = PyDict_GetItemString(kwargs, "MatrixHandler");
     }
 
     PyObject* result = NULL;
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         result = _NmzResultImpl(cone_ptr, prop);
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         result = _NmzResultImpl(cone_ptr, prop);
     }
 #ifdef ENFNORMALIZ
-    else {
+    else if (is_cone_renf(cone)) {
         Cone< renf_elem_class >* cone_ptr = get_cone_renf(cone);
         result = _NmzResultImpl(
             cone_ptr, prop,
             reinterpret_cast< void* >(get_cone_renf_renf(cone)));
     }
 #endif
 
@@ -1792,38 +1736,36 @@
 
 /***************************************************************************
  *
  * Python verbosity
  *
  ***************************************************************************/
 
-PyObject* NmzSetVerboseDefault(PyObject* self, PyObject* args)
+static PyObject* NmzSetVerboseDefault(PyObject* self, PyObject* args)
 {
     FUNC_BEGIN
     PyObject* value = PyTuple_GetItem(args, 0);
     if (value != Py_True && value != Py_False) {
         PyErr_SetString(PyNormaliz_cppError,
                         "Argument must be True or False");
         return NULL;
     }
     return BoolToPyBool(libnormaliz::setVerboseDefault(value == Py_True));
     FUNC_END
 }
 
 template < typename Integer >
-PyObject* NmzSetVerbose(Cone< Integer >* C, PyObject* value)
+static PyObject* NmzSetVerbose(Cone< Integer >* C, PyObject* value)
 {
     FUNC_BEGIN
-    bool old_value;
-    old_value = C->setVerbose(value == Py_True);
-    return BoolToPyBool(old_value);
+    return BoolToPyBool(C->setVerbose(value == Py_True));
     FUNC_END
 }
 
-PyObject* NmzSetVerbose_Outer(PyObject* self, PyObject* args)
+static PyObject* NmzSetVerbose_Outer(PyObject* self, PyObject* args)
 {
     FUNC_BEGIN
 
     PyObject* cone = PyTuple_GetItem(args, 0);
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
@@ -1833,24 +1775,24 @@
     PyObject* value = PyTuple_GetItem(args, 1);
     if (value != Py_True && value != Py_False) {
         PyErr_SetString(PyNormaliz_cppError,
                         "Second argument must be True or False");
         return NULL;
     }
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         return NmzSetVerbose(cone_ptr, value);
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         return NmzSetVerbose(cone_ptr, value);
     }
 #ifdef ENFNORMALIZ
-    else {
+    else if (is_cone_renf(cone)) {
         Cone< renf_elem_class >* cone_ptr = get_cone_renf(cone);
         return NmzSetVerbose(cone_ptr, value);
     }
 #endif
     Py_RETURN_NONE;
 
     FUNC_END
@@ -1858,151 +1800,134 @@
 
 /***************************************************************************
  *
  * Get Polynomial
  *
  ***************************************************************************/
 
-PyObject* NmzGetPolynomial(PyObject* self, PyObject* args)
+static PyObject* NmzGetPolynomial(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
     PyObject* cone = PyTuple_GetItem(args, 0);
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
 
-    current_interpreter_sigint_handler = PyOS_setsig(SIGINT, signal_handler);
+    TempSignalHandler tmpHandler; // use custom signal handler
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
-        PyObject*          return_value =
-            StringToPyUnicode((cone_ptr->getIntData()).getPolynomial());
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-        return return_value;
+        return StringToPyUnicode((cone_ptr->getIntData()).getPolynomial());
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
-        PyObject*          return_value =
-            StringToPyUnicode((cone_ptr->getIntData()).getPolynomial());
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-        return return_value;
+        return StringToPyUnicode((cone_ptr->getIntData()).getPolynomial());
     }
     else {
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
         PyErr_SetString(PyNormaliz_cppError,
                         "Polynomial not available for renf cone");
         return NULL;
     }
 
     FUNC_END
 }
 
 /***************************************************************************
  *
  * NrCoeffQuasiPol
  *
  ***************************************************************************/
 
-PyObject* NmzSetNrCoeffQuasiPol(PyObject* self, PyObject* args)
+static PyObject* NmzSetNrCoeffQuasiPol(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
     PyObject* cone = PyTuple_GetItem(args, 0);
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
 
     PyObject* bound_py = PyTuple_GetItem(args, 1);
 
+    TempSignalHandler tmpHandler; // use custom signal handler
+
     int  overflow;
     long bound = PyLong_AsLongLongAndOverflow(bound_py, &overflow);
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         cone_ptr->setNrCoeffQuasiPol(bound);
         Py_RETURN_TRUE;
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         cone_ptr->setNrCoeffQuasiPol(bound);
         Py_RETURN_TRUE;
     }
     else {
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
         PyErr_SetString(PyNormaliz_cppError,
                         "Cannot set quasi polynomial coeffs for renf cone");
         return NULL;
     }
 
     FUNC_END
 }
 
 /***************************************************************************
  *
  * Get Symmetrized cone
  *
  ***************************************************************************/
 
-PyObject* NmzSymmetrizedCone(PyObject* self, PyObject* args)
+static PyObject* NmzSymmetrizedCone(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
     PyObject* cone = PyTuple_GetItem(args, 0);
 
     if (!is_cone(cone)) {
         PyErr_SetString(PyNormaliz_cppError, "First argument must be a cone");
         return NULL;
     }
 
-    current_interpreter_sigint_handler = PyOS_setsig(SIGINT, signal_handler);
+    TempSignalHandler tmpHandler; // use custom signal handler
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
-        Cone< mpz_class >* symm_cone = &(cone_ptr->getSymmetrizedCone());
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-        if (symm_cone == 0) {
-            Py_RETURN_NONE;
-        }
-        symm_cone = new Cone< mpz_class >(*symm_cone);
-        return pack_cone(symm_cone);
+        Cone< mpz_class >& symm_cone = cone_ptr->getSymmetrizedCone();
+        return pack_cone(new Cone< mpz_class >(symm_cone));
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
-        Cone< long long >* symm_cone = &(cone_ptr->getSymmetrizedCone());
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-        if (symm_cone == 0) {
-            Py_RETURN_NONE;
-        }
-        symm_cone = new Cone< long long >(*symm_cone);
-        return pack_cone(symm_cone);
+        Cone< long long >& symm_cone = cone_ptr->getSymmetrizedCone();
+        return pack_cone(new Cone< long long >(symm_cone));
     }
     else {
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
         PyErr_SetString(PyNormaliz_cppError,
                         "Symmetrized cone not available for renf cone");
         return NULL;
     }
 
     FUNC_END
 }
 
 /***************************************************************************
  *
  * Get expanded hilbert series
  *
  ***************************************************************************/
 
-PyObject* NmzGetHilbertSeriesExpansion(PyObject* self, PyObject* args)
+static PyObject* NmzGetHilbertSeriesExpansion(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
     PyObject* cone = PyTuple_GetItem(args, 0);
     PyObject* py_degree = PyTuple_GetItem(args, 1);
 
@@ -2015,43 +1940,39 @@
         PyErr_SetString(PyNormaliz_cppError,
                         "Second argument must be a long");
         return NULL;
     }
 
     long                       degree = PyLong_AsLong(py_degree);
     libnormaliz::HilbertSeries HS;
-    current_interpreter_sigint_handler = PyOS_setsig(SIGINT, signal_handler);
+    TempSignalHandler tmpHandler; // use custom signal handler
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         HS = cone_ptr->getHilbertSeries();
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         HS = cone_ptr->getHilbertSeries();
     }
     else {
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
         PyErr_SetString(
             PyNormaliz_cppError,
             "Hilbert series expansion not available for renf cone");
         return NULL;
     }
 
     HS.set_expansion_degree(degree);
-    PyObject* result = NmzVectorToPyList(HS.getExpansion());
-    PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-
-    return result;
+    return NmzVectorToPyList(HS.getExpansion());
 
     FUNC_END
 }
 
 
-PyObject* NmzGetWeightedEhrhartSeriesExpansion(PyObject* self, PyObject* args)
+static PyObject* NmzGetWeightedEhrhartSeriesExpansion(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
     PyObject* cone = PyTuple_GetItem(args, 0);
     PyObject* py_degree = PyTuple_GetItem(args, 1);
 
@@ -2064,48 +1985,44 @@
         PyErr_SetString(PyNormaliz_cppError,
                         "Second argument must be a long");
         return NULL;
     }
 
     long degree = PyLong_AsLong(py_degree);
     pair< libnormaliz::HilbertSeries, mpz_class > ES;
-    current_interpreter_sigint_handler = PyOS_setsig(SIGINT, signal_handler);
+    TempSignalHandler tmpHandler; // use custom signal handler
 
-    if (cone_name_str == string(PyCapsule_GetName(cone))) {
+    if (is_cone_mpz(cone)) {
         Cone< mpz_class >* cone_ptr = get_cone_mpz(cone);
         ES = cone_ptr->getWeightedEhrhartSeries();
     }
-    else if (cone_name_str_long == string(PyCapsule_GetName(cone))) {
+    else if (is_cone_long(cone)) {
         Cone< long long >* cone_ptr = get_cone_long(cone);
         ES = cone_ptr->getWeightedEhrhartSeries();
     }
     else {
-        PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
         PyErr_SetString(
             PyNormaliz_cppError,
             "Ehrhart series expansion not available for renf cone");
         return NULL;
     }
 
     ES.first.set_expansion_degree(degree);
-    PyObject* result = NmzVectorToPyList(ES.first.getExpansion());
-    PyOS_setsig(SIGINT, current_interpreter_sigint_handler);
-
-    return result;
+    return NmzVectorToPyList(ES.first.getExpansion());
 
     FUNC_END
 }
 
 /***************************************************************************
  *
  * Set number of threads
  *
  ***************************************************************************/
 
-PyObject* NmzSetNumberOfNormalizThreads(PyObject* self, PyObject* args)
+static PyObject* NmzSetNumberOfNormalizThreads(PyObject* self, PyObject* args)
 {
 
     FUNC_BEGIN
 
     PyObject* num_threads = PyTuple_GetItem(args, 0);
 
     long num_threads_long;
@@ -2128,34 +2045,61 @@
     return PyLong_FromLong(num_threads_long);
 
     FUNC_END
 }
 
 /***************************************************************************
  *
- * Check for ENFNormaliz
+ * Check for various features
  *
  ***************************************************************************/
 
-PyObject* NmzHasEAntic(PyObject* self)
+static PyObject* NmzHasEAntic(PyObject* self)
 {
 #ifdef ENFNORMALIZ
     Py_RETURN_TRUE;
 #else
     Py_RETURN_FALSE;
 #endif
 }
 
+static PyObject* NmzHasNauty(PyObject* self)
+{
+#ifdef NMZ_NAUTY
+    Py_RETURN_TRUE;
+#else
+    Py_RETURN_FALSE;
+#endif
+}
+
+static PyObject* NmzHasFlint(PyObject* self)
+{
+#ifdef NMZ_FLINT
+    Py_RETURN_TRUE;
+#else
+    Py_RETURN_FALSE;
+#endif
+}
+
+static PyObject* NmzHasCocoa(PyObject* self)
+{
+#ifdef NMZ_COCOA
+    Py_RETURN_TRUE;
+#else
+    Py_RETURN_FALSE;
+#endif
+}
+
 /***************************************************************************
  *
  * Write output file
  *
  ***************************************************************************/
 
-PyObject* NmzWriteOutputFile(PyObject* self, PyObject* args)
+static PyObject* NmzWriteOutputFile(PyObject* self, PyObject* args)
 {
     FUNC_BEGIN
 
     if ((!PyTuple_Check(args)) || (PyTuple_Size(args) != 2)) {
         throw PyNormalizInputException(
             "The arguments must be a cone and a string");
         return NULL;
@@ -2190,15 +2134,15 @@
 
 /***************************************************************************
  *
  * Get renf precision
  *
  ***************************************************************************/
 
-PyObject* NmzGetRenfInfo(PyObject* self, PyObject* args)
+static PyObject* NmzGetRenfInfo(PyObject* self, PyObject* args)
 {
     FUNC_BEGIN
 #ifdef ENFNORMALIZ
     if( (!PyTuple_Check(args)) || (PyTuple_Size(args) != 1) ){
         throw PyNormalizInputException(
             "Only one argument allowed"
         );
@@ -2282,16 +2226,24 @@
      METH_VARARGS, "Sets the period bound for the quasi-polynomial"},
     {"NmzGetHilbertSeriesExpansion",
      (PyCFunction)NmzGetHilbertSeriesExpansion, METH_VARARGS,
      "Returns expansion of the hilbert series"},
     {"NmzGetWeightedEhrhartSeriesExpansion",
      (PyCFunction)NmzGetWeightedEhrhartSeriesExpansion, METH_VARARGS,
      "Returns expansion of the weighted Ehrhart series"},
+
     {"NmzHasEAntic", (PyCFunction)NmzHasEAntic, METH_NOARGS,
      "Returns true if (Py)Normaliz was compiled with e-antic support"},
+    {"NmzHasNauty", (PyCFunction)NmzHasNauty, METH_NOARGS,
+     "Returns true if (Py)Normaliz was compiled with nauty support"},
+    {"NmzHasFlint", (PyCFunction)NmzHasFlint, METH_NOARGS,
+     "Returns true if (Py)Normaliz was compiled with Flint support"},
+    {"NmzHasCocoa", (PyCFunction)NmzHasCocoa, METH_NOARGS,
+     "Returns true if (Py)Normaliz was compiled with CoCoA support"},
+
     {"NmzWriteOutputFile", (PyCFunction)NmzWriteOutputFile, METH_VARARGS,
      "Prints the Normaliz cone output into a file"},
     {"NmzGetRenfInfo", (PyCFunction)NmzGetRenfInfo, METH_VARARGS,
      "Outputs info of the number field associated to a renf cone"},
     {"NmzModifyCone", (PyCFunction)_NmzModify_Outer, METH_VARARGS,
      "Modifies a given input property of a cone using a new matrix"},
     {
@@ -2354,13 +2306,11 @@
         const_cast< char* >("PyNormaliz_cpp.NormalizInterfaceError"), NULL,
         NULL);
     Py_INCREF(PyNormaliz_cppError);
 
     PyModule_AddObject(module, "normaliz_error", NormalizError);
     PyModule_AddObject(module, "pynormaliz_error", PyNormaliz_cppError);
 
-    current_interpreter_sigint_handler = PyOS_getsig(SIGINT);
-
 #if PY_MAJOR_VERSION >= 3
     return module;
 #endif
 }
```

### Comparing `PyNormaliz-2.8/doc/PyNormaliz_Tutorial.ipynb` & `PyNormaliz-2.9/doc/PyNormaliz_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/doc/PyNormaliz_Tutorial.pdf` & `PyNormaliz-2.9/doc/PyNormaliz_Tutorial.pdf`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/examples/first.py` & `PyNormaliz-2.9/examples/first.py`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/examples/first_enf.py` & `PyNormaliz-2.9/examples/first_enf.py`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/examples/first_long.py` & `PyNormaliz-2.9/examples/first_long.py`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/examples/first_rational.py` & `PyNormaliz-2.9/examples/first_rational.py`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/examples/getters.py` & `PyNormaliz-2.9/examples/getters.py`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/tests/assertion.py` & `PyNormaliz-2.9/tests/assertion.py`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/tests/assertion.txt` & `PyNormaliz-2.9/tests/assertion.txt`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/tests/generic_test.py` & `PyNormaliz-2.9/tests/generic_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from PyNormaliz import NmzCone, NmzResult, normaliz_error
 
 from itertools import product
 from random import shuffle
 
 methods = [
          "AffineDim",
+         "Automorphisms",
          "Congruences",
          "Dehomogenization",
          "Equations",
          "EmbeddingDim",
 # NOTE: floating point value
 #         "EuclideanVolume",
          "EhrhartQuasiPolynomial",
@@ -143,14 +144,16 @@
                         print("*"*50)
                         stdout.flush()
                         failed += 1
                     elif self.verbosity >= 3:
                         print("pass")
                         stdout.flush()
 
+        return failed
+
 class Test1(GenericPyNormalizTest):
     init_data = {"vertices": [(-3,-2,-1,1), (-1,1,-1,2), (1,1,-1,1), (1,1,1,1)]}
 
     # expected results
     AffineDim = 3
     Congruences = []
     Dehomogenization = [0,0,0,1]
@@ -188,14 +191,15 @@
 class Test2(GenericPyNormalizTest):
     "A cube in a subspace"
 
     init_data = {"vertices": list((2,) + p+(-2,1,) for p in product([-1,0,1],repeat=2))}
 
     # expected results
     AffineDim = 2
+    Automorphisms = [8, [[[],[]],[]], [[[0,2,1,3], [1,0,3,2]], [[0,1,2,3]]], [[[1,0,3,2], [0,2,1,3]], [[0,1,2,3]]]]
     Congruences = []
     Dehomogenization = normaliz_error
     EmbeddingDim = 5
     EhrhartQuasiPolynomial = [[1,4,4],1]
     Equations = [[1,0,0,0,-2],[0,0,0,1,2]]
     ExcludedFaces = normaliz_error
     ExternalIndex = 1
```

### Comparing `PyNormaliz-2.8/tests/generic_test.pyc` & `PyNormaliz-2.9/tests/generic_test.pyc`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/tests/runtests.py` & `PyNormaliz-2.9/tests/runtests.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     skip.add("segfault-27.txt")
     skip.add("segfault-35.txt")
     skip.add("vertex_denom-37.txt")
     skip.add("modify_cone_renf.txt")
 
 # run doctests
 attempted = failed = 0
-for filename in os.listdir(os.curdir):
+dir = os.path.dirname(os.path.realpath(__file__))
+for filename in os.listdir(dir):
     if filename.endswith('.txt'):
         if filename in skip:
             print("Skip {}".format(filename))
             continue
 
         print("Doctest {}".format(filename))
         result = doctest.testfile(filename, 
@@ -40,10 +41,10 @@
         attempted += result[1]
 
 
 # unit tests
 from generic_test import tests
 
 for test in tests:
-    test(verbosity=2).run(repeat=10)
+    failed += test(verbosity=2).run(repeat=10)
 
 sys.exit(failed)
```

### Comparing `PyNormaliz-2.8/tests/segfault-23.txt` & `PyNormaliz-2.9/tests/segfault-23.txt`

 * *Files identical despite different names*

### Comparing `PyNormaliz-2.8/tests/test_rational_cones.txt` & `PyNormaliz-2.9/tests/test_rational_cones.txt`

 * *Files identical despite different names*

