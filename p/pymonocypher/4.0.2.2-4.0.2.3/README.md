# Comparing `tmp/pymonocypher-4.0.2.2.tar.gz` & `tmp/pymonocypher-4.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonocypher-4.0.2.2.tar", last modified: Fri May 10 15:21:37 2024, max compression
+gzip compressed data, was "pymonocypher-4.0.2.3.tar", last modified: Wed May 29 18:32:11 2024, max compression
```

## Comparing `pymonocypher-4.0.2.2.tar` & `pymonocypher-4.0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   755033 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/c_monocypher.c
--rw-r--r--   0 runner    (1001) docker     (127)   100271 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/monocypher.c
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/monocypher.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/pymonocypher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1873923 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/test/blake2-kat.json
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/test/test_monocypher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:32:11.518482 pymonocypher-4.0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-29 18:32:11.518482 pymonocypher-4.0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   768614 2024-05-29 18:32:11.000000 pymonocypher-4.0.2.3/c_monocypher.c
+-rw-r--r--   0 runner    (1001) docker     (127)   100271 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/monocypher.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/monocypher.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:32:11.518482 pymonocypher-4.0.2.3/pymonocypher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-29 18:32:11.000000 pymonocypher-4.0.2.3/pymonocypher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-29 18:32:11.000000 pymonocypher-4.0.2.3/pymonocypher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:32:11.000000 pymonocypher-4.0.2.3/pymonocypher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 18:32:11.000000 pymonocypher-4.0.2.3/pymonocypher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 18:32:11.000000 pymonocypher-4.0.2.3/pymonocypher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 18:32:11.518482 pymonocypher-4.0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:32:11.518482 pymonocypher-4.0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1873923 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/test/blake2-kat.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-29 18:32:05.000000 pymonocypher-4.0.2.3/test/test_monocypher.py
```

### Comparing `pymonocypher-4.0.2.2/LICENSE.txt` & `pymonocypher-4.0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.2/PKG-INFO` & `pymonocypher-4.0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonocypher
-Version: 4.0.2.2
+Version: 4.0.2.3
 Summary: Python ctypes bindings to the Monocypher library
 Home-page: https://github.com/jetperch/pymonocypher
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: BSD 2-clause
 Project-URL: Bug Reports, https://github.com/jetperch/pymonocypher/issues
 Project-URL: Source, https://github.com/jetperch/pymonocypher/
```

### Comparing `pymonocypher-4.0.2.2/README.md` & `pymonocypher-4.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.2/c_monocypher.c` & `pymonocypher-4.0.2.3/c_monocypher.c`

 * *Files 2% similar despite different names*

```diff
@@ -1507,28 +1507,28 @@
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10monocypher_IncrementalAuthenticatedEncryption;
 struct __pyx_obj_10monocypher_Blake2b;
 struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b;
 
-/* "monocypher.pyx":206
+/* "monocypher.pyx":205
  * 
  * 
  * cdef class IncrementalAuthenticatedEncryption:             # <<<<<<<<<<<<<<
  *     cdef crypto_aead_ctx _ctx
  * 
  */
 struct __pyx_obj_10monocypher_IncrementalAuthenticatedEncryption {
   PyObject_HEAD
   crypto_aead_ctx _ctx;
 };
 
 
-/* "monocypher.pyx":286
+/* "monocypher.pyx":285
  * 
  * 
  * cdef class Blake2b:             # <<<<<<<<<<<<<<
  *     cdef crypto_blake2b_ctx _ctx
  *     cdef int _hash_size
  */
 struct __pyx_obj_10monocypher_Blake2b {
@@ -2268,28 +2268,29 @@
 extern int __pyx_module_is_main_monocypher;
 int __pyx_module_is_main_monocypher = 0;
 
 /* Implementation of "monocypher" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_TypeError;
+static PyObject *__pyx_builtin_DeprecationWarning;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_p[] = "p";
 static const char __pyx_k_16[] = " != 16";
 static const char __pyx_k_24[] = " != 24";
 static const char __pyx_k_32[] = " != 32";
 static const char __pyx_k__4[] = "";
 static const char __pyx_k_ad[] = "ad";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_rv[] = "rv";
-static const char __pyx_k__10[] = "*";
-static const char __pyx_k__60[] = "?";
+static const char __pyx_k__12[] = "*";
+static const char __pyx_k__62[] = "?";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_mac[] = "mac";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_sig[] = "sig";
 static const char __pyx_k_url[] = "__url__";
 static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_data[] = "data";
@@ -2298,14 +2299,15 @@
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_salt[] = "salt";
 static const char __pyx_k_seed[] = "seed";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
+static const char __pyx_k_warn[] = "warn";
 static const char __pyx_k_wipe[] = "wipe";
 static const char __pyx_k_wrap[] = "wrap";
 static const char __pyx_k_bytes[] = "bytes";
 static const char __pyx_k_curve[] = "curve";
 static const char __pyx_k_nonce[] = "nonce";
 static const char __pyx_k_title[] = "__title__";
 static const char __pyx_k_tweak[] = "tweak";
@@ -2323,24 +2325,23 @@
 static const char __pyx_k_public[] = "public";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_result[] = "result";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_secret[] = "secret";
 static const char __pyx_k_unlock[] = "unlock";
 static const char __pyx_k_update[] = "update";
-static const char __pyx_k_4_0_2_2[] = "4.0.2.2";
+static const char __pyx_k_4_0_2_3[] = "4.0.2.3";
 static const char __pyx_k_Blake2b[] = "Blake2b";
 static const char __pyx_k_blake2b[] = "blake2b";
 static const char __pyx_k_default[] = "default";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_license[] = "__license__";
 static const char __pyx_k_message[] = "message";
 static const char __pyx_k_secrets[] = "secrets";
 static const char __pyx_k_version[] = "__version__";
-static const char __pyx_k_binascii[] = "binascii";
 static const char __pyx_k_chacha20[] = "chacha20";
 static const char __pyx_k_finalize[] = "finalize";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_nb_block[] = "nb_block";
 static const char __pyx_k_nb_lanes[] = "nb_lanes";
 static const char __pyx_k_password[] = "password";
 static const char __pyx_k_randbits[] = "randbits";
@@ -2360,14 +2361,15 @@
 static const char __pyx_k_work_area[] = "work_area";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_argon2i_32[] = "argon2i_32";
 static const char __pyx_k_monocypher[] = "monocypher";
 static const char __pyx_k_plain_text[] = "plain_text";
 static const char __pyx_k_public_key[] = "public_key";
 static const char __pyx_k_secret_key[] = "secret_key";
+static const char __pyx_k_stacklevel[] = "stacklevel";
 static const char __pyx_k_cfunc_to_py[] = "cfunc.to_py";
 static const char __pyx_k_crypto_text[] = "crypto_text";
 static const char __pyx_k_description[] = "__description__";
 static const char __pyx_k_token_bytes[] = "token_bytes";
 static const char __pyx_k_BSD_2_clause[] = "BSD 2-clause";
 static const char __pyx_k_Jetperch_LLC[] = "Jetperch LLC";
 static const char __pyx_k_author_email[] = "__author_email__";
@@ -2387,38 +2389,41 @@
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_signature_check[] = "signature_check";
 static const char __pyx_k_your_secret_key[] = "your_secret_key";
 static const char __pyx_k_Blake2b_finalize[] = "Blake2b.finalize";
 static const char __pyx_k_c_monocypher_pyx[] = "c_monocypher.pyx";
 static const char __pyx_k_their_public_key[] = "their_public_key";
 static const char __pyx_k_tuple_bytes_bytes[] = "tuple[bytes, bytes]";
+static const char __pyx_k_DeprecationWarning[] = "DeprecationWarning";
 static const char __pyx_k_Invalid_key_length[] = "Invalid key length ";
 static const char __pyx_k_Invalid_mac_length[] = "Invalid mac length ";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_elligator_key_pair[] = "elligator_key_pair";
 static const char __pyx_k_Invalid_seed_length[] = "Invalid seed length ";
 static const char __pyx_k_Invalid_curve_length[] = "Invalid curve length ";
 static const char __pyx_k_Invalid_nonce_length[] = "Invalid nonce length ";
 static const char __pyx_k_invalid_nonce_length[] = "invalid nonce length";
 static const char __pyx_k_unsupported_method_s[] = "unsupported method: %s";
 static const char __pyx_k_Invalid_hidden_length[] = "Invalid hidden length ";
 static const char __pyx_k_Blake2b___reduce_cython[] = "Blake2b.__reduce_cython__";
 static const char __pyx_k_Blake2b___setstate_cython[] = "Blake2b.__setstate_cython__";
 static const char __pyx_k_generate_signing_key_pair[] = "generate_signing_key_pair";
+static const char __pyx_k_invalid_secret_key_length[] = "invalid secret key length";
 static const char __pyx_k_secret_key_length_invalid[] = "secret key length invalid";
 static const char __pyx_k_compute_signing_public_key[] = "compute_signing_public_key";
 static const char __pyx_k_joulescope_dev_jetperch_com[] = "joulescope-dev@jetperch.com";
 static const char __pyx_k_Pyx_CFunc_f5947c__10monocypher[] = "__Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b.<locals>.wrap";
 static const char __pyx_k_generate_key_exchange_key_pair[] = "generate_key_exchange_key_pair";
 static const char __pyx_k_Monocypher_library_Python_bindi[] = "\nMonocypher library Python bindings.\n\nMonocypher is an easy to use, easy to deploy, auditable crypto library\nwritten in portable C.\n";
 static const char __pyx_k_Pickling_of_struct_members_such[] = "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)";
 static const char __pyx_k_compute_key_exchange_public_key[] = "compute_key_exchange_public_key";
 static const char __pyx_k_Copyright_2018_2024_Jetperch_LLC[] = "Copyright 2018-2024 Jetperch LLC";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti[] = "IncrementalAuthenticatedEncryption";
+static const char __pyx_k_Provide_the_full_64_byte_key_fro[] = "Provide the full 64-byte key from generate_signing_key_pair()";
 static const char __pyx_k_Python_ctypes_bindings_to_the_Mo[] = "Python ctypes bindings to the Monocypher library";
 static const char __pyx_k_curve_point_is_unsuitable_for_hi[] = "curve point is unsuitable for hiding";
 static const char __pyx_k_https_github_com_jetperch_pymono[] = "https://github.com/jetperch/pymonocypher";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti_2[] = "IncrementalAuthenticatedEncryption.lock";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti_3[] = "IncrementalAuthenticatedEncryption.unlock";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti_4[] = "IncrementalAuthenticatedEncryption.__reduce_cython__";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti_5[] = "IncrementalAuthenticatedEncryption.__setstate_cython__";
@@ -2494,54 +2499,55 @@
   #endif
   PyTypeObject *__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption;
   PyTypeObject *__pyx_ptype_10monocypher_Blake2b;
   PyTypeObject *__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b;
   PyObject *__pyx_kp_u_16;
   PyObject *__pyx_kp_u_24;
   PyObject *__pyx_kp_u_32;
-  PyObject *__pyx_kp_u_4_0_2_2;
+  PyObject *__pyx_kp_u_4_0_2_3;
   PyObject *__pyx_kp_u_BSD_2_clause;
   PyObject *__pyx_n_s_Blake2b;
   PyObject *__pyx_n_s_Blake2b___reduce_cython;
   PyObject *__pyx_n_s_Blake2b___setstate_cython;
   PyObject *__pyx_n_s_Blake2b_finalize;
   PyObject *__pyx_n_s_Blake2b_update;
   PyObject *__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC;
+  PyObject *__pyx_n_s_DeprecationWarning;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti_2;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti_3;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti_4;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti_5;
   PyObject *__pyx_kp_u_Invalid_curve_length;
   PyObject *__pyx_kp_u_Invalid_hidden_length;
   PyObject *__pyx_kp_u_Invalid_key_length;
   PyObject *__pyx_kp_u_Invalid_mac_length;
   PyObject *__pyx_kp_u_Invalid_nonce_length;
   PyObject *__pyx_kp_u_Invalid_seed_length;
   PyObject *__pyx_kp_u_Jetperch_LLC;
   PyObject *__pyx_kp_s_Pickling_of_struct_members_such;
+  PyObject *__pyx_kp_u_Provide_the_full_64_byte_key_fro;
   PyObject *__pyx_kp_u_Python_ctypes_bindings_to_the_Mo;
   PyObject *__pyx_n_s_Pyx_CFunc_f5947c__10monocypher;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_ValueError;
-  PyObject *__pyx_n_s__10;
+  PyObject *__pyx_n_s__12;
   PyObject *__pyx_kp_b__4;
   PyObject *__pyx_kp_u__4;
-  PyObject *__pyx_n_s__60;
+  PyObject *__pyx_n_s__62;
   PyObject *__pyx_n_s_a;
   PyObject *__pyx_n_s_ad;
   PyObject *__pyx_n_u_ad;
   PyObject *__pyx_n_s_algorithm;
   PyObject *__pyx_n_s_argon2i_32;
   PyObject *__pyx_n_s_associated_data;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_author;
   PyObject *__pyx_n_s_author_email;
   PyObject *__pyx_n_s_b;
-  PyObject *__pyx_n_s_binascii;
   PyObject *__pyx_n_s_blake2b;
   PyObject *__pyx_n_s_bool;
   PyObject *__pyx_n_s_bytes;
   PyObject *__pyx_kp_s_c_monocypher_pyx;
   PyObject *__pyx_n_s_cfunc_to_py;
   PyObject *__pyx_n_s_chacha20;
   PyObject *__pyx_n_u_chacha20;
@@ -2573,14 +2579,15 @@
   PyObject *__pyx_n_s_hash_size;
   PyObject *__pyx_n_s_hidden;
   PyObject *__pyx_kp_u_https_github_com_jetperch_pymono;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_inputs;
   PyObject *__pyx_kp_u_invalid_nonce_length;
+  PyObject *__pyx_kp_u_invalid_secret_key_length;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_kp_u_joulescope_dev_jetperch_com;
   PyObject *__pyx_n_s_key;
   PyObject *__pyx_n_u_key;
   PyObject *__pyx_n_s_key_exchange;
   PyObject *__pyx_n_s_length;
@@ -2627,96 +2634,101 @@
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_sig;
   PyObject *__pyx_n_s_signature;
   PyObject *__pyx_n_s_signature_check;
   PyObject *__pyx_n_s_signature_sign;
   PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_stacklevel;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_their_public_key;
   PyObject *__pyx_n_s_title;
   PyObject *__pyx_n_s_token_bytes;
   PyObject *__pyx_kp_u_too_long;
   PyObject *__pyx_kp_s_tuple_bytes_bytes;
   PyObject *__pyx_n_s_tweak;
   PyObject *__pyx_n_s_unlock;
   PyObject *__pyx_kp_u_unsupported_method_s;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_url;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_version;
+  PyObject *__pyx_n_s_warn;
   PyObject *__pyx_n_s_warnings;
   PyObject *__pyx_n_s_wipe;
   PyObject *__pyx_n_s_work_area;
   PyObject *__pyx_n_s_wrap;
   PyObject *__pyx_n_s_your_secret_key;
+  PyObject *__pyx_int_2;
   PyObject *__pyx_int_8;
   PyObject *__pyx_int_16;
   PyObject *__pyx_int_24;
   PyObject *__pyx_int_32;
   PyObject *__pyx_int_64;
   PyObject *__pyx_int_4294967295;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__5;
   PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__7;
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__9;
+  PyObject *__pyx_tuple__10;
   PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__13;
   PyObject *__pyx_tuple__15;
-  PyObject *__pyx_tuple__16;
+  PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__18;
   PyObject *__pyx_tuple__20;
   PyObject *__pyx_tuple__22;
   PyObject *__pyx_tuple__24;
   PyObject *__pyx_tuple__26;
   PyObject *__pyx_tuple__28;
   PyObject *__pyx_tuple__30;
   PyObject *__pyx_tuple__32;
-  PyObject *__pyx_tuple__36;
+  PyObject *__pyx_tuple__34;
   PyObject *__pyx_tuple__38;
-  PyObject *__pyx_tuple__39;
+  PyObject *__pyx_tuple__40;
   PyObject *__pyx_tuple__41;
   PyObject *__pyx_tuple__43;
   PyObject *__pyx_tuple__45;
   PyObject *__pyx_tuple__47;
   PyObject *__pyx_tuple__49;
   PyObject *__pyx_tuple__51;
-  PyObject *__pyx_tuple__54;
+  PyObject *__pyx_tuple__53;
   PyObject *__pyx_tuple__56;
   PyObject *__pyx_tuple__58;
+  PyObject *__pyx_tuple__60;
   PyObject *__pyx_codeobj__2;
-  PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__14;
-  PyObject *__pyx_codeobj__17;
+  PyObject *__pyx_codeobj__16;
   PyObject *__pyx_codeobj__19;
   PyObject *__pyx_codeobj__21;
   PyObject *__pyx_codeobj__23;
   PyObject *__pyx_codeobj__25;
   PyObject *__pyx_codeobj__27;
   PyObject *__pyx_codeobj__29;
   PyObject *__pyx_codeobj__31;
   PyObject *__pyx_codeobj__33;
-  PyObject *__pyx_codeobj__34;
   PyObject *__pyx_codeobj__35;
+  PyObject *__pyx_codeobj__36;
   PyObject *__pyx_codeobj__37;
-  PyObject *__pyx_codeobj__40;
+  PyObject *__pyx_codeobj__39;
   PyObject *__pyx_codeobj__42;
   PyObject *__pyx_codeobj__44;
   PyObject *__pyx_codeobj__46;
   PyObject *__pyx_codeobj__48;
   PyObject *__pyx_codeobj__50;
   PyObject *__pyx_codeobj__52;
-  PyObject *__pyx_codeobj__53;
+  PyObject *__pyx_codeobj__54;
   PyObject *__pyx_codeobj__55;
   PyObject *__pyx_codeobj__57;
   PyObject *__pyx_codeobj__59;
+  PyObject *__pyx_codeobj__61;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2760,54 +2772,55 @@
   Py_CLEAR(clear_module_state->__pyx_ptype_10monocypher_Blake2b);
   Py_CLEAR(clear_module_state->__pyx_type_10monocypher_Blake2b);
   Py_CLEAR(clear_module_state->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b);
   Py_CLEAR(clear_module_state->__pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b);
   Py_CLEAR(clear_module_state->__pyx_kp_u_16);
   Py_CLEAR(clear_module_state->__pyx_kp_u_24);
   Py_CLEAR(clear_module_state->__pyx_kp_u_32);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_4_0_2_2);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_4_0_2_3);
   Py_CLEAR(clear_module_state->__pyx_kp_u_BSD_2_clause);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b_finalize);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b_update);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC);
+  Py_CLEAR(clear_module_state->__pyx_n_s_DeprecationWarning);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_3);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_4);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_5);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_curve_length);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_hidden_length);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_key_length);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_mac_length);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_nonce_length);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_seed_length);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Jetperch_LLC);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Pickling_of_struct_members_such);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Provide_the_full_64_byte_key_fro);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Python_ctypes_bindings_to_the_Mo);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pyx_CFunc_f5947c__10monocypher);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
-  Py_CLEAR(clear_module_state->__pyx_n_s__10);
+  Py_CLEAR(clear_module_state->__pyx_n_s__12);
   Py_CLEAR(clear_module_state->__pyx_kp_b__4);
   Py_CLEAR(clear_module_state->__pyx_kp_u__4);
-  Py_CLEAR(clear_module_state->__pyx_n_s__60);
+  Py_CLEAR(clear_module_state->__pyx_n_s__62);
   Py_CLEAR(clear_module_state->__pyx_n_s_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_ad);
   Py_CLEAR(clear_module_state->__pyx_n_u_ad);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithm);
   Py_CLEAR(clear_module_state->__pyx_n_s_argon2i_32);
   Py_CLEAR(clear_module_state->__pyx_n_s_associated_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_author);
   Py_CLEAR(clear_module_state->__pyx_n_s_author_email);
   Py_CLEAR(clear_module_state->__pyx_n_s_b);
-  Py_CLEAR(clear_module_state->__pyx_n_s_binascii);
   Py_CLEAR(clear_module_state->__pyx_n_s_blake2b);
   Py_CLEAR(clear_module_state->__pyx_n_s_bool);
   Py_CLEAR(clear_module_state->__pyx_n_s_bytes);
   Py_CLEAR(clear_module_state->__pyx_kp_s_c_monocypher_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_cfunc_to_py);
   Py_CLEAR(clear_module_state->__pyx_n_s_chacha20);
   Py_CLEAR(clear_module_state->__pyx_n_u_chacha20);
@@ -2839,14 +2852,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_hash_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_hidden);
   Py_CLEAR(clear_module_state->__pyx_kp_u_https_github_com_jetperch_pymono);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_inputs);
   Py_CLEAR(clear_module_state->__pyx_kp_u_invalid_nonce_length);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_invalid_secret_key_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_kp_u_joulescope_dev_jetperch_com);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
   Py_CLEAR(clear_module_state->__pyx_n_u_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_key_exchange);
   Py_CLEAR(clear_module_state->__pyx_n_s_length);
@@ -2893,96 +2907,101 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_sig);
   Py_CLEAR(clear_module_state->__pyx_n_s_signature);
   Py_CLEAR(clear_module_state->__pyx_n_s_signature_check);
   Py_CLEAR(clear_module_state->__pyx_n_s_signature_sign);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_stacklevel);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_their_public_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_title);
   Py_CLEAR(clear_module_state->__pyx_n_s_token_bytes);
   Py_CLEAR(clear_module_state->__pyx_kp_u_too_long);
   Py_CLEAR(clear_module_state->__pyx_kp_s_tuple_bytes_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_tweak);
   Py_CLEAR(clear_module_state->__pyx_n_s_unlock);
   Py_CLEAR(clear_module_state->__pyx_kp_u_unsupported_method_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_url);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_version);
+  Py_CLEAR(clear_module_state->__pyx_n_s_warn);
   Py_CLEAR(clear_module_state->__pyx_n_s_warnings);
   Py_CLEAR(clear_module_state->__pyx_n_s_wipe);
   Py_CLEAR(clear_module_state->__pyx_n_s_work_area);
   Py_CLEAR(clear_module_state->__pyx_n_s_wrap);
   Py_CLEAR(clear_module_state->__pyx_n_s_your_secret_key);
+  Py_CLEAR(clear_module_state->__pyx_int_2);
   Py_CLEAR(clear_module_state->__pyx_int_8);
   Py_CLEAR(clear_module_state->__pyx_int_16);
   Py_CLEAR(clear_module_state->__pyx_int_24);
   Py_CLEAR(clear_module_state->__pyx_int_32);
   Py_CLEAR(clear_module_state->__pyx_int_64);
   Py_CLEAR(clear_module_state->__pyx_int_4294967295);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
   Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__13);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
-  Py_CLEAR(clear_module_state->__pyx_tuple__16);
+  Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
   Py_CLEAR(clear_module_state->__pyx_tuple__20);
   Py_CLEAR(clear_module_state->__pyx_tuple__22);
   Py_CLEAR(clear_module_state->__pyx_tuple__24);
   Py_CLEAR(clear_module_state->__pyx_tuple__26);
   Py_CLEAR(clear_module_state->__pyx_tuple__28);
   Py_CLEAR(clear_module_state->__pyx_tuple__30);
   Py_CLEAR(clear_module_state->__pyx_tuple__32);
-  Py_CLEAR(clear_module_state->__pyx_tuple__36);
+  Py_CLEAR(clear_module_state->__pyx_tuple__34);
   Py_CLEAR(clear_module_state->__pyx_tuple__38);
-  Py_CLEAR(clear_module_state->__pyx_tuple__39);
+  Py_CLEAR(clear_module_state->__pyx_tuple__40);
   Py_CLEAR(clear_module_state->__pyx_tuple__41);
   Py_CLEAR(clear_module_state->__pyx_tuple__43);
   Py_CLEAR(clear_module_state->__pyx_tuple__45);
   Py_CLEAR(clear_module_state->__pyx_tuple__47);
   Py_CLEAR(clear_module_state->__pyx_tuple__49);
   Py_CLEAR(clear_module_state->__pyx_tuple__51);
-  Py_CLEAR(clear_module_state->__pyx_tuple__54);
+  Py_CLEAR(clear_module_state->__pyx_tuple__53);
   Py_CLEAR(clear_module_state->__pyx_tuple__56);
   Py_CLEAR(clear_module_state->__pyx_tuple__58);
+  Py_CLEAR(clear_module_state->__pyx_tuple__60);
   Py_CLEAR(clear_module_state->__pyx_codeobj__2);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__14);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__19);
   Py_CLEAR(clear_module_state->__pyx_codeobj__21);
   Py_CLEAR(clear_module_state->__pyx_codeobj__23);
   Py_CLEAR(clear_module_state->__pyx_codeobj__25);
   Py_CLEAR(clear_module_state->__pyx_codeobj__27);
   Py_CLEAR(clear_module_state->__pyx_codeobj__29);
   Py_CLEAR(clear_module_state->__pyx_codeobj__31);
   Py_CLEAR(clear_module_state->__pyx_codeobj__33);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__34);
   Py_CLEAR(clear_module_state->__pyx_codeobj__35);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__36);
   Py_CLEAR(clear_module_state->__pyx_codeobj__37);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__40);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__39);
   Py_CLEAR(clear_module_state->__pyx_codeobj__42);
   Py_CLEAR(clear_module_state->__pyx_codeobj__44);
   Py_CLEAR(clear_module_state->__pyx_codeobj__46);
   Py_CLEAR(clear_module_state->__pyx_codeobj__48);
   Py_CLEAR(clear_module_state->__pyx_codeobj__50);
   Py_CLEAR(clear_module_state->__pyx_codeobj__52);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__53);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__54);
   Py_CLEAR(clear_module_state->__pyx_codeobj__55);
   Py_CLEAR(clear_module_state->__pyx_codeobj__57);
   Py_CLEAR(clear_module_state->__pyx_codeobj__59);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__61);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3004,54 +3023,55 @@
   Py_VISIT(traverse_module_state->__pyx_ptype_10monocypher_Blake2b);
   Py_VISIT(traverse_module_state->__pyx_type_10monocypher_Blake2b);
   Py_VISIT(traverse_module_state->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b);
   Py_VISIT(traverse_module_state->__pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b);
   Py_VISIT(traverse_module_state->__pyx_kp_u_16);
   Py_VISIT(traverse_module_state->__pyx_kp_u_24);
   Py_VISIT(traverse_module_state->__pyx_kp_u_32);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_4_0_2_2);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_4_0_2_3);
   Py_VISIT(traverse_module_state->__pyx_kp_u_BSD_2_clause);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b_finalize);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b_update);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC);
+  Py_VISIT(traverse_module_state->__pyx_n_s_DeprecationWarning);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_3);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_4);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_5);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_curve_length);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_hidden_length);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_key_length);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_mac_length);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_nonce_length);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_seed_length);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Jetperch_LLC);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Pickling_of_struct_members_such);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Provide_the_full_64_byte_key_fro);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Python_ctypes_bindings_to_the_Mo);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pyx_CFunc_f5947c__10monocypher);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
-  Py_VISIT(traverse_module_state->__pyx_n_s__10);
+  Py_VISIT(traverse_module_state->__pyx_n_s__12);
   Py_VISIT(traverse_module_state->__pyx_kp_b__4);
   Py_VISIT(traverse_module_state->__pyx_kp_u__4);
-  Py_VISIT(traverse_module_state->__pyx_n_s__60);
+  Py_VISIT(traverse_module_state->__pyx_n_s__62);
   Py_VISIT(traverse_module_state->__pyx_n_s_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_ad);
   Py_VISIT(traverse_module_state->__pyx_n_u_ad);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithm);
   Py_VISIT(traverse_module_state->__pyx_n_s_argon2i_32);
   Py_VISIT(traverse_module_state->__pyx_n_s_associated_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_author);
   Py_VISIT(traverse_module_state->__pyx_n_s_author_email);
   Py_VISIT(traverse_module_state->__pyx_n_s_b);
-  Py_VISIT(traverse_module_state->__pyx_n_s_binascii);
   Py_VISIT(traverse_module_state->__pyx_n_s_blake2b);
   Py_VISIT(traverse_module_state->__pyx_n_s_bool);
   Py_VISIT(traverse_module_state->__pyx_n_s_bytes);
   Py_VISIT(traverse_module_state->__pyx_kp_s_c_monocypher_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_cfunc_to_py);
   Py_VISIT(traverse_module_state->__pyx_n_s_chacha20);
   Py_VISIT(traverse_module_state->__pyx_n_u_chacha20);
@@ -3083,14 +3103,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_hash_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_hidden);
   Py_VISIT(traverse_module_state->__pyx_kp_u_https_github_com_jetperch_pymono);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_inputs);
   Py_VISIT(traverse_module_state->__pyx_kp_u_invalid_nonce_length);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_invalid_secret_key_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_kp_u_joulescope_dev_jetperch_com);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
   Py_VISIT(traverse_module_state->__pyx_n_u_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_key_exchange);
   Py_VISIT(traverse_module_state->__pyx_n_s_length);
@@ -3137,96 +3158,101 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_sig);
   Py_VISIT(traverse_module_state->__pyx_n_s_signature);
   Py_VISIT(traverse_module_state->__pyx_n_s_signature_check);
   Py_VISIT(traverse_module_state->__pyx_n_s_signature_sign);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_stacklevel);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_their_public_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_title);
   Py_VISIT(traverse_module_state->__pyx_n_s_token_bytes);
   Py_VISIT(traverse_module_state->__pyx_kp_u_too_long);
   Py_VISIT(traverse_module_state->__pyx_kp_s_tuple_bytes_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_tweak);
   Py_VISIT(traverse_module_state->__pyx_n_s_unlock);
   Py_VISIT(traverse_module_state->__pyx_kp_u_unsupported_method_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_url);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_version);
+  Py_VISIT(traverse_module_state->__pyx_n_s_warn);
   Py_VISIT(traverse_module_state->__pyx_n_s_warnings);
   Py_VISIT(traverse_module_state->__pyx_n_s_wipe);
   Py_VISIT(traverse_module_state->__pyx_n_s_work_area);
   Py_VISIT(traverse_module_state->__pyx_n_s_wrap);
   Py_VISIT(traverse_module_state->__pyx_n_s_your_secret_key);
+  Py_VISIT(traverse_module_state->__pyx_int_2);
   Py_VISIT(traverse_module_state->__pyx_int_8);
   Py_VISIT(traverse_module_state->__pyx_int_16);
   Py_VISIT(traverse_module_state->__pyx_int_24);
   Py_VISIT(traverse_module_state->__pyx_int_32);
   Py_VISIT(traverse_module_state->__pyx_int_64);
   Py_VISIT(traverse_module_state->__pyx_int_4294967295);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
   Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__13);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
-  Py_VISIT(traverse_module_state->__pyx_tuple__16);
+  Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
   Py_VISIT(traverse_module_state->__pyx_tuple__20);
   Py_VISIT(traverse_module_state->__pyx_tuple__22);
   Py_VISIT(traverse_module_state->__pyx_tuple__24);
   Py_VISIT(traverse_module_state->__pyx_tuple__26);
   Py_VISIT(traverse_module_state->__pyx_tuple__28);
   Py_VISIT(traverse_module_state->__pyx_tuple__30);
   Py_VISIT(traverse_module_state->__pyx_tuple__32);
-  Py_VISIT(traverse_module_state->__pyx_tuple__36);
+  Py_VISIT(traverse_module_state->__pyx_tuple__34);
   Py_VISIT(traverse_module_state->__pyx_tuple__38);
-  Py_VISIT(traverse_module_state->__pyx_tuple__39);
+  Py_VISIT(traverse_module_state->__pyx_tuple__40);
   Py_VISIT(traverse_module_state->__pyx_tuple__41);
   Py_VISIT(traverse_module_state->__pyx_tuple__43);
   Py_VISIT(traverse_module_state->__pyx_tuple__45);
   Py_VISIT(traverse_module_state->__pyx_tuple__47);
   Py_VISIT(traverse_module_state->__pyx_tuple__49);
   Py_VISIT(traverse_module_state->__pyx_tuple__51);
-  Py_VISIT(traverse_module_state->__pyx_tuple__54);
+  Py_VISIT(traverse_module_state->__pyx_tuple__53);
   Py_VISIT(traverse_module_state->__pyx_tuple__56);
   Py_VISIT(traverse_module_state->__pyx_tuple__58);
+  Py_VISIT(traverse_module_state->__pyx_tuple__60);
   Py_VISIT(traverse_module_state->__pyx_codeobj__2);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__14);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__19);
   Py_VISIT(traverse_module_state->__pyx_codeobj__21);
   Py_VISIT(traverse_module_state->__pyx_codeobj__23);
   Py_VISIT(traverse_module_state->__pyx_codeobj__25);
   Py_VISIT(traverse_module_state->__pyx_codeobj__27);
   Py_VISIT(traverse_module_state->__pyx_codeobj__29);
   Py_VISIT(traverse_module_state->__pyx_codeobj__31);
   Py_VISIT(traverse_module_state->__pyx_codeobj__33);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__34);
   Py_VISIT(traverse_module_state->__pyx_codeobj__35);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__36);
   Py_VISIT(traverse_module_state->__pyx_codeobj__37);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__40);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__39);
   Py_VISIT(traverse_module_state->__pyx_codeobj__42);
   Py_VISIT(traverse_module_state->__pyx_codeobj__44);
   Py_VISIT(traverse_module_state->__pyx_codeobj__46);
   Py_VISIT(traverse_module_state->__pyx_codeobj__48);
   Py_VISIT(traverse_module_state->__pyx_codeobj__50);
   Py_VISIT(traverse_module_state->__pyx_codeobj__52);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__53);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__54);
   Py_VISIT(traverse_module_state->__pyx_codeobj__55);
   Py_VISIT(traverse_module_state->__pyx_codeobj__57);
   Py_VISIT(traverse_module_state->__pyx_codeobj__59);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__61);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3264,54 +3290,55 @@
 #endif
 #define __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption __pyx_mstate_global->__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption
 #define __pyx_ptype_10monocypher_Blake2b __pyx_mstate_global->__pyx_ptype_10monocypher_Blake2b
 #define __pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b __pyx_mstate_global->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b
 #define __pyx_kp_u_16 __pyx_mstate_global->__pyx_kp_u_16
 #define __pyx_kp_u_24 __pyx_mstate_global->__pyx_kp_u_24
 #define __pyx_kp_u_32 __pyx_mstate_global->__pyx_kp_u_32
-#define __pyx_kp_u_4_0_2_2 __pyx_mstate_global->__pyx_kp_u_4_0_2_2
+#define __pyx_kp_u_4_0_2_3 __pyx_mstate_global->__pyx_kp_u_4_0_2_3
 #define __pyx_kp_u_BSD_2_clause __pyx_mstate_global->__pyx_kp_u_BSD_2_clause
 #define __pyx_n_s_Blake2b __pyx_mstate_global->__pyx_n_s_Blake2b
 #define __pyx_n_s_Blake2b___reduce_cython __pyx_mstate_global->__pyx_n_s_Blake2b___reduce_cython
 #define __pyx_n_s_Blake2b___setstate_cython __pyx_mstate_global->__pyx_n_s_Blake2b___setstate_cython
 #define __pyx_n_s_Blake2b_finalize __pyx_mstate_global->__pyx_n_s_Blake2b_finalize
 #define __pyx_n_s_Blake2b_update __pyx_mstate_global->__pyx_n_s_Blake2b_update
 #define __pyx_kp_u_Copyright_2018_2024_Jetperch_LLC __pyx_mstate_global->__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC
+#define __pyx_n_s_DeprecationWarning __pyx_mstate_global->__pyx_n_s_DeprecationWarning
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti_2 __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti_2
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti_3 __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti_3
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti_4 __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti_4
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti_5 __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti_5
 #define __pyx_kp_u_Invalid_curve_length __pyx_mstate_global->__pyx_kp_u_Invalid_curve_length
 #define __pyx_kp_u_Invalid_hidden_length __pyx_mstate_global->__pyx_kp_u_Invalid_hidden_length
 #define __pyx_kp_u_Invalid_key_length __pyx_mstate_global->__pyx_kp_u_Invalid_key_length
 #define __pyx_kp_u_Invalid_mac_length __pyx_mstate_global->__pyx_kp_u_Invalid_mac_length
 #define __pyx_kp_u_Invalid_nonce_length __pyx_mstate_global->__pyx_kp_u_Invalid_nonce_length
 #define __pyx_kp_u_Invalid_seed_length __pyx_mstate_global->__pyx_kp_u_Invalid_seed_length
 #define __pyx_kp_u_Jetperch_LLC __pyx_mstate_global->__pyx_kp_u_Jetperch_LLC
 #define __pyx_kp_s_Pickling_of_struct_members_such __pyx_mstate_global->__pyx_kp_s_Pickling_of_struct_members_such
+#define __pyx_kp_u_Provide_the_full_64_byte_key_fro __pyx_mstate_global->__pyx_kp_u_Provide_the_full_64_byte_key_fro
 #define __pyx_kp_u_Python_ctypes_bindings_to_the_Mo __pyx_mstate_global->__pyx_kp_u_Python_ctypes_bindings_to_the_Mo
 #define __pyx_n_s_Pyx_CFunc_f5947c__10monocypher __pyx_mstate_global->__pyx_n_s_Pyx_CFunc_f5947c__10monocypher
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
-#define __pyx_n_s__10 __pyx_mstate_global->__pyx_n_s__10
+#define __pyx_n_s__12 __pyx_mstate_global->__pyx_n_s__12
 #define __pyx_kp_b__4 __pyx_mstate_global->__pyx_kp_b__4
 #define __pyx_kp_u__4 __pyx_mstate_global->__pyx_kp_u__4
-#define __pyx_n_s__60 __pyx_mstate_global->__pyx_n_s__60
+#define __pyx_n_s__62 __pyx_mstate_global->__pyx_n_s__62
 #define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
 #define __pyx_n_s_ad __pyx_mstate_global->__pyx_n_s_ad
 #define __pyx_n_u_ad __pyx_mstate_global->__pyx_n_u_ad
 #define __pyx_n_s_algorithm __pyx_mstate_global->__pyx_n_s_algorithm
 #define __pyx_n_s_argon2i_32 __pyx_mstate_global->__pyx_n_s_argon2i_32
 #define __pyx_n_s_associated_data __pyx_mstate_global->__pyx_n_s_associated_data
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_author __pyx_mstate_global->__pyx_n_s_author
 #define __pyx_n_s_author_email __pyx_mstate_global->__pyx_n_s_author_email
 #define __pyx_n_s_b __pyx_mstate_global->__pyx_n_s_b
-#define __pyx_n_s_binascii __pyx_mstate_global->__pyx_n_s_binascii
 #define __pyx_n_s_blake2b __pyx_mstate_global->__pyx_n_s_blake2b
 #define __pyx_n_s_bool __pyx_mstate_global->__pyx_n_s_bool
 #define __pyx_n_s_bytes __pyx_mstate_global->__pyx_n_s_bytes
 #define __pyx_kp_s_c_monocypher_pyx __pyx_mstate_global->__pyx_kp_s_c_monocypher_pyx
 #define __pyx_n_s_cfunc_to_py __pyx_mstate_global->__pyx_n_s_cfunc_to_py
 #define __pyx_n_s_chacha20 __pyx_mstate_global->__pyx_n_s_chacha20
 #define __pyx_n_u_chacha20 __pyx_mstate_global->__pyx_n_u_chacha20
@@ -3343,14 +3370,15 @@
 #define __pyx_n_s_hash_size __pyx_mstate_global->__pyx_n_s_hash_size
 #define __pyx_n_s_hidden __pyx_mstate_global->__pyx_n_s_hidden
 #define __pyx_kp_u_https_github_com_jetperch_pymono __pyx_mstate_global->__pyx_kp_u_https_github_com_jetperch_pymono
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_inputs __pyx_mstate_global->__pyx_n_s_inputs
 #define __pyx_kp_u_invalid_nonce_length __pyx_mstate_global->__pyx_kp_u_invalid_nonce_length
+#define __pyx_kp_u_invalid_secret_key_length __pyx_mstate_global->__pyx_kp_u_invalid_secret_key_length
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_kp_u_joulescope_dev_jetperch_com __pyx_mstate_global->__pyx_kp_u_joulescope_dev_jetperch_com
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
 #define __pyx_n_u_key __pyx_mstate_global->__pyx_n_u_key
 #define __pyx_n_s_key_exchange __pyx_mstate_global->__pyx_n_s_key_exchange
 #define __pyx_n_s_length __pyx_mstate_global->__pyx_n_s_length
@@ -3397,96 +3425,101 @@
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_sig __pyx_mstate_global->__pyx_n_s_sig
 #define __pyx_n_s_signature __pyx_mstate_global->__pyx_n_s_signature
 #define __pyx_n_s_signature_check __pyx_mstate_global->__pyx_n_s_signature_check
 #define __pyx_n_s_signature_sign __pyx_mstate_global->__pyx_n_s_signature_sign
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_stacklevel __pyx_mstate_global->__pyx_n_s_stacklevel
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_their_public_key __pyx_mstate_global->__pyx_n_s_their_public_key
 #define __pyx_n_s_title __pyx_mstate_global->__pyx_n_s_title
 #define __pyx_n_s_token_bytes __pyx_mstate_global->__pyx_n_s_token_bytes
 #define __pyx_kp_u_too_long __pyx_mstate_global->__pyx_kp_u_too_long
 #define __pyx_kp_s_tuple_bytes_bytes __pyx_mstate_global->__pyx_kp_s_tuple_bytes_bytes
 #define __pyx_n_s_tweak __pyx_mstate_global->__pyx_n_s_tweak
 #define __pyx_n_s_unlock __pyx_mstate_global->__pyx_n_s_unlock
 #define __pyx_kp_u_unsupported_method_s __pyx_mstate_global->__pyx_kp_u_unsupported_method_s
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_url __pyx_mstate_global->__pyx_n_s_url
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_version __pyx_mstate_global->__pyx_n_s_version
+#define __pyx_n_s_warn __pyx_mstate_global->__pyx_n_s_warn
 #define __pyx_n_s_warnings __pyx_mstate_global->__pyx_n_s_warnings
 #define __pyx_n_s_wipe __pyx_mstate_global->__pyx_n_s_wipe
 #define __pyx_n_s_work_area __pyx_mstate_global->__pyx_n_s_work_area
 #define __pyx_n_s_wrap __pyx_mstate_global->__pyx_n_s_wrap
 #define __pyx_n_s_your_secret_key __pyx_mstate_global->__pyx_n_s_your_secret_key
+#define __pyx_int_2 __pyx_mstate_global->__pyx_int_2
 #define __pyx_int_8 __pyx_mstate_global->__pyx_int_8
 #define __pyx_int_16 __pyx_mstate_global->__pyx_int_16
 #define __pyx_int_24 __pyx_mstate_global->__pyx_int_24
 #define __pyx_int_32 __pyx_mstate_global->__pyx_int_32
 #define __pyx_int_64 __pyx_mstate_global->__pyx_int_64
 #define __pyx_int_4294967295 __pyx_mstate_global->__pyx_int_4294967295
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
-#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
+#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
 #define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
 #define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
 #define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
 #define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
 #define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
 #define __pyx_tuple__30 __pyx_mstate_global->__pyx_tuple__30
 #define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
-#define __pyx_tuple__36 __pyx_mstate_global->__pyx_tuple__36
+#define __pyx_tuple__34 __pyx_mstate_global->__pyx_tuple__34
 #define __pyx_tuple__38 __pyx_mstate_global->__pyx_tuple__38
-#define __pyx_tuple__39 __pyx_mstate_global->__pyx_tuple__39
+#define __pyx_tuple__40 __pyx_mstate_global->__pyx_tuple__40
 #define __pyx_tuple__41 __pyx_mstate_global->__pyx_tuple__41
 #define __pyx_tuple__43 __pyx_mstate_global->__pyx_tuple__43
 #define __pyx_tuple__45 __pyx_mstate_global->__pyx_tuple__45
 #define __pyx_tuple__47 __pyx_mstate_global->__pyx_tuple__47
 #define __pyx_tuple__49 __pyx_mstate_global->__pyx_tuple__49
 #define __pyx_tuple__51 __pyx_mstate_global->__pyx_tuple__51
-#define __pyx_tuple__54 __pyx_mstate_global->__pyx_tuple__54
+#define __pyx_tuple__53 __pyx_mstate_global->__pyx_tuple__53
 #define __pyx_tuple__56 __pyx_mstate_global->__pyx_tuple__56
 #define __pyx_tuple__58 __pyx_mstate_global->__pyx_tuple__58
+#define __pyx_tuple__60 __pyx_mstate_global->__pyx_tuple__60
 #define __pyx_codeobj__2 __pyx_mstate_global->__pyx_codeobj__2
-#define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
-#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
+#define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
 #define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
-#define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
 #define __pyx_codeobj__35 __pyx_mstate_global->__pyx_codeobj__35
+#define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
 #define __pyx_codeobj__37 __pyx_mstate_global->__pyx_codeobj__37
-#define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
+#define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
 #define __pyx_codeobj__42 __pyx_mstate_global->__pyx_codeobj__42
 #define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
 #define __pyx_codeobj__46 __pyx_mstate_global->__pyx_codeobj__46
 #define __pyx_codeobj__48 __pyx_mstate_global->__pyx_codeobj__48
 #define __pyx_codeobj__50 __pyx_mstate_global->__pyx_codeobj__50
 #define __pyx_codeobj__52 __pyx_mstate_global->__pyx_codeobj__52
-#define __pyx_codeobj__53 __pyx_mstate_global->__pyx_codeobj__53
+#define __pyx_codeobj__54 __pyx_mstate_global->__pyx_codeobj__54
 #define __pyx_codeobj__55 __pyx_mstate_global->__pyx_codeobj__55
 #define __pyx_codeobj__57 __pyx_mstate_global->__pyx_codeobj__57
 #define __pyx_codeobj__59 __pyx_mstate_global->__pyx_codeobj__59
+#define __pyx_codeobj__61 __pyx_mstate_global->__pyx_codeobj__61
 /* #### Code section: module_code ### */
 
 /* "cfunc.to_py":67
  * @cname("__Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b")
  * cdef object __Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b(int (*f)(const uint8_t *, const uint8_t *) except *):
  *     def wrap(const uint8_t * a, const uint8_t * b):             # <<<<<<<<<<<<<<
  *         """wrap(a: 'const uint8_t *', b: 'const uint8_t *') -> 'int'"""
@@ -3722,15 +3755,15 @@
   __Pyx_XDECREF(__pyx_v_wrap);
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":156
+/* "monocypher.pyx":155
  * 
  * 
  * def wipe(data):             # <<<<<<<<<<<<<<
  *     """Wipe a bytes object from memory.
  * 
  */
 
@@ -3784,31 +3817,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 156, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 155, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "wipe") < 0)) __PYX_ERR(0, 156, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "wipe") < 0)) __PYX_ERR(0, 155, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_data = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("wipe", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 156, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("wipe", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 155, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -3837,26 +3870,26 @@
   uint8_t *__pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wipe", 1);
 
-  /* "monocypher.pyx":164
+  /* "monocypher.pyx":163
  *     data.  Ensure that the data to wipe is the only active reference!
  *     """
  *     crypto_wipe(data, len(data))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L1_error)
-  __pyx_t_2 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 163, __pyx_L1_error)
   crypto_wipe(__pyx_t_1, __pyx_t_2);
 
-  /* "monocypher.pyx":156
+  /* "monocypher.pyx":155
  * 
  * 
  * def wipe(data):             # <<<<<<<<<<<<<<
  *     """Wipe a bytes object from memory.
  * 
  */
 
@@ -3868,15 +3901,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":167
+/* "monocypher.pyx":166
  * 
  * 
  * def lock(key, nonce, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated encryption.
  * 
  */
 
@@ -3940,47 +3973,47 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nonce)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("lock", 0, 3, 4, 1); __PYX_ERR(0, 167, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("lock", 0, 3, 4, 1); __PYX_ERR(0, 166, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("lock", 0, 3, 4, 2); __PYX_ERR(0, 167, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("lock", 0, 3, 4, 2); __PYX_ERR(0, 166, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_associated_data);
           if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lock") < 0)) __PYX_ERR(0, 167, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lock") < 0)) __PYX_ERR(0, 166, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
@@ -3992,15 +4025,15 @@
     __pyx_v_key = values[0];
     __pyx_v_nonce = values[1];
     __pyx_v_message = values[2];
     __pyx_v_associated_data = values[3];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lock", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 167, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lock", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 166, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -4041,43 +4074,43 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lock", 0);
   __Pyx_INCREF(__pyx_v_associated_data);
 
-  /* "monocypher.pyx":179
+  /* "monocypher.pyx":178
  *         authentication code.  ciphertext is the encrypted message.
  *     """
  *     mac = bytes(16)             # <<<<<<<<<<<<<<
  *     crypto_text = bytes(len(message))
  *     associated_data = b'' if associated_data is None else associated_data
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_mac = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":180
+  /* "monocypher.pyx":179
  *     """
  *     mac = bytes(16)
  *     crypto_text = bytes(len(message))             # <<<<<<<<<<<<<<
  *     associated_data = b'' if associated_data is None else associated_data
  *     crypto_aead_lock(crypto_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))
  */
-  __pyx_t_2 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 180, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_crypto_text = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":181
+  /* "monocypher.pyx":180
  *     mac = bytes(16)
  *     crypto_text = bytes(len(message))
  *     associated_data = b'' if associated_data is None else associated_data             # <<<<<<<<<<<<<<
  *     crypto_aead_lock(crypto_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))
  *     return mac, crypto_text
  */
   __pyx_t_4 = (__pyx_v_associated_data == Py_None);
@@ -4087,52 +4120,52 @@
   } else {
     __Pyx_INCREF(__pyx_v_associated_data);
     __pyx_t_3 = __pyx_v_associated_data;
   }
   __Pyx_DECREF_SET(__pyx_v_associated_data, __pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":182
+  /* "monocypher.pyx":181
  *     crypto_text = bytes(len(message))
  *     associated_data = b'' if associated_data is None else associated_data
  *     crypto_aead_lock(crypto_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))             # <<<<<<<<<<<<<<
  *     return mac, crypto_text
  * 
  */
-  __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_crypto_text); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_v_mac); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_associated_data); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
-  __pyx_t_2 = PyObject_Length(__pyx_v_associated_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 182, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
-  __pyx_t_11 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_crypto_text); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_v_mac); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_associated_data); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_associated_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_11 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 181, __pyx_L1_error)
   crypto_aead_lock(__pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_2, __pyx_t_10, __pyx_t_11);
 
-  /* "monocypher.pyx":183
+  /* "monocypher.pyx":182
  *     associated_data = b'' if associated_data is None else associated_data
  *     crypto_aead_lock(crypto_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))
  *     return mac, crypto_text             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_mac);
   __Pyx_GIVEREF(__pyx_v_mac);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_mac)) __PYX_ERR(0, 183, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_mac)) __PYX_ERR(0, 182, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_crypto_text);
   __Pyx_GIVEREF(__pyx_v_crypto_text);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_crypto_text)) __PYX_ERR(0, 183, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_crypto_text)) __PYX_ERR(0, 182, __pyx_L1_error);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":167
+  /* "monocypher.pyx":166
  * 
  * 
  * def lock(key, nonce, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated encryption.
  * 
  */
 
@@ -4147,15 +4180,15 @@
   __Pyx_XDECREF(__pyx_v_crypto_text);
   __Pyx_XDECREF(__pyx_v_associated_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":186
+/* "monocypher.pyx":185
  * 
  * 
  * def unlock(key, nonce, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated decryption.
  * 
  */
 
@@ -4222,57 +4255,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nonce)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("unlock", 0, 4, 5, 1); __PYX_ERR(0, 186, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("unlock", 0, 4, 5, 1); __PYX_ERR(0, 185, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mac)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("unlock", 0, 4, 5, 2); __PYX_ERR(0, 186, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("unlock", 0, 4, 5, 2); __PYX_ERR(0, 185, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("unlock", 0, 4, 5, 3); __PYX_ERR(0, 186, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("unlock", 0, 4, 5, 3); __PYX_ERR(0, 185, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_associated_data);
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "unlock") < 0)) __PYX_ERR(0, 186, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "unlock") < 0)) __PYX_ERR(0, 185, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -4286,15 +4319,15 @@
     __pyx_v_nonce = values[1];
     __pyx_v_mac = values[2];
     __pyx_v_message = values[3];
     __pyx_v_associated_data = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("unlock", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 186, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("unlock", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 185, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -4335,31 +4368,31 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unlock", 0);
   __Pyx_INCREF(__pyx_v_associated_data);
 
-  /* "monocypher.pyx":198
+  /* "monocypher.pyx":197
  *     :return: The secret message or None on authentication failure.
  *     """
  *     plain_text = bytearray(len(message))             # <<<<<<<<<<<<<<
  *     associated_data = b'' if associated_data is None else associated_data
  *     rv = crypto_aead_unlock(plain_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 198, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_plain_text = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":199
+  /* "monocypher.pyx":198
  *     """
  *     plain_text = bytearray(len(message))
  *     associated_data = b'' if associated_data is None else associated_data             # <<<<<<<<<<<<<<
  *     rv = crypto_aead_unlock(plain_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))
  *     if 0 != rv:
  */
   __pyx_t_4 = (__pyx_v_associated_data == Py_None);
@@ -4369,74 +4402,74 @@
   } else {
     __Pyx_INCREF(__pyx_v_associated_data);
     __pyx_t_3 = __pyx_v_associated_data;
   }
   __Pyx_DECREF_SET(__pyx_v_associated_data, __pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":200
+  /* "monocypher.pyx":199
  *     plain_text = bytearray(len(message))
  *     associated_data = b'' if associated_data is None else associated_data
  *     rv = crypto_aead_unlock(plain_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))             # <<<<<<<<<<<<<<
  *     if 0 != rv:
  *         return None
  */
-  __pyx_t_5 = __Pyx_PyObject_AsWritableUString(__pyx_v_plain_text); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_AsUString(__pyx_v_mac); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_associated_data); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_t_1 = PyObject_Length(__pyx_v_associated_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_t_11 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsWritableUString(__pyx_v_plain_text); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsUString(__pyx_v_mac); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_associated_data); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_associated_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_11 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 199, __pyx_L1_error)
   __pyx_v_rv = crypto_aead_unlock(__pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_1, __pyx_t_10, __pyx_t_11);
 
-  /* "monocypher.pyx":201
+  /* "monocypher.pyx":200
  *     associated_data = b'' if associated_data is None else associated_data
  *     rv = crypto_aead_unlock(plain_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))
  *     if 0 != rv:             # <<<<<<<<<<<<<<
  *         return None
  *     return plain_text
  */
   __pyx_t_4 = (0 != __pyx_v_rv);
   if (__pyx_t_4) {
 
-    /* "monocypher.pyx":202
+    /* "monocypher.pyx":201
  *     rv = crypto_aead_unlock(plain_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))
  *     if 0 != rv:
  *         return None             # <<<<<<<<<<<<<<
  *     return plain_text
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "monocypher.pyx":201
+    /* "monocypher.pyx":200
  *     associated_data = b'' if associated_data is None else associated_data
  *     rv = crypto_aead_unlock(plain_text, mac, key, nonce, associated_data, len(associated_data), message, len(message))
  *     if 0 != rv:             # <<<<<<<<<<<<<<
  *         return None
  *     return plain_text
  */
   }
 
-  /* "monocypher.pyx":203
+  /* "monocypher.pyx":202
  *     if 0 != rv:
  *         return None
  *     return plain_text             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_plain_text);
   __pyx_r = __pyx_v_plain_text;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":186
+  /* "monocypher.pyx":185
  * 
  * 
  * def unlock(key, nonce, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated decryption.
  * 
  */
 
@@ -4450,15 +4483,15 @@
   __Pyx_XDECREF(__pyx_v_plain_text);
   __Pyx_XDECREF(__pyx_v_associated_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":214
+/* "monocypher.pyx":213
  *     :param nonce: The 24-byte number, used only once with any given session key.
  *     """
  *     def __init__(self, key, nonce):             # <<<<<<<<<<<<<<
  *         if len(key) != 32:
  *             raise ValueError(f'Invalid key length {len(key)} != 32')
  */
 
@@ -4497,43 +4530,43 @@
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nonce)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 214, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 213, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 214, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 213, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
       values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
     }
     __pyx_v_key = values[0];
     __pyx_v_nonce = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 214, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 213, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
@@ -4568,138 +4601,138 @@
   uint8_t const *__pyx_t_7;
   uint8_t const *__pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "monocypher.pyx":215
+  /* "monocypher.pyx":214
  *     """
  *     def __init__(self, key, nonce):
  *         if len(key) != 32:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid key length {len(key)} != 32')
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 214, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 32);
   if (unlikely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":216
+    /* "monocypher.pyx":215
  *     def __init__(self, key, nonce):
  *         if len(key) != 32:
  *             raise ValueError(f'Invalid key length {len(key)} != 32')             # <<<<<<<<<<<<<<
  * 
  *         if len(nonce) != 24:
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = 0;
     __pyx_t_4 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_key_length);
     __pyx_t_1 += 19;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_key_length);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Invalid_key_length);
-    __pyx_t_5 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 216, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_1 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_kp_u_32);
     __pyx_t_1 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_32);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_32);
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 216, __pyx_L1_error)
+    __PYX_ERR(0, 215, __pyx_L1_error)
 
-    /* "monocypher.pyx":215
+    /* "monocypher.pyx":214
  *     """
  *     def __init__(self, key, nonce):
  *         if len(key) != 32:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid key length {len(key)} != 32')
  * 
  */
   }
 
-  /* "monocypher.pyx":218
+  /* "monocypher.pyx":217
  *             raise ValueError(f'Invalid key length {len(key)} != 32')
  * 
  *         if len(nonce) != 24:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid nonce length {len(key)} != 24')
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_nonce); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_nonce); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 217, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 24);
   if (unlikely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":219
+    /* "monocypher.pyx":218
  * 
  *         if len(nonce) != 24:
  *             raise ValueError(f'Invalid nonce length {len(key)} != 24')             # <<<<<<<<<<<<<<
  * 
  *         crypto_aead_init_x(&self._ctx, key, nonce)
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = 0;
     __pyx_t_4 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_nonce_length);
     __pyx_t_1 += 21;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_nonce_length);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Invalid_nonce_length);
-    __pyx_t_5 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 219, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_1 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_kp_u_24);
     __pyx_t_1 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_24);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_24);
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 219, __pyx_L1_error)
+    __PYX_ERR(0, 218, __pyx_L1_error)
 
-    /* "monocypher.pyx":218
+    /* "monocypher.pyx":217
  *             raise ValueError(f'Invalid key length {len(key)} != 32')
  * 
  *         if len(nonce) != 24:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid nonce length {len(key)} != 24')
  * 
  */
   }
 
-  /* "monocypher.pyx":221
+  /* "monocypher.pyx":220
  *             raise ValueError(f'Invalid nonce length {len(key)} != 24')
  * 
  *         crypto_aead_init_x(&self._ctx, key, nonce)             # <<<<<<<<<<<<<<
  * 
  *     def lock(self, message, associated_data=None):
  */
-  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 221, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L1_error)
   crypto_aead_init_x((&__pyx_v_self->_ctx), __pyx_t_7, __pyx_t_8);
 
-  /* "monocypher.pyx":214
+  /* "monocypher.pyx":213
  *     :param nonce: The 24-byte number, used only once with any given session key.
  *     """
  *     def __init__(self, key, nonce):             # <<<<<<<<<<<<<<
  *         if len(key) != 32:
  *             raise ValueError(f'Invalid key length {len(key)} != 32')
  */
 
@@ -4712,15 +4745,15 @@
   __Pyx_AddTraceback("monocypher.IncrementalAuthenticatedEncryption.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":223
+/* "monocypher.pyx":222
  *         crypto_aead_init_x(&self._ctx, key, nonce)
  * 
  *     def lock(self, message, associated_data=None):             # <<<<<<<<<<<<<<
  *         """Perform authenticated encryption.
  * 
  */
 
@@ -4778,27 +4811,27 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_associated_data);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lock") < 0)) __PYX_ERR(0, 223, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lock") < 0)) __PYX_ERR(0, 222, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
@@ -4806,15 +4839,15 @@
       }
     }
     __pyx_v_message = values[0];
     __pyx_v_associated_data = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lock", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 223, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lock", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 222, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -4853,43 +4886,43 @@
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lock", 0);
   __Pyx_INCREF(__pyx_v_associated_data);
 
-  /* "monocypher.pyx":232
+  /* "monocypher.pyx":231
  *             authentication code.  ciphertext is the encrypted message.
  *         """
  *         mac = bytes(16)             # <<<<<<<<<<<<<<
  *         crypto_text = bytes(len(message))
  *         associated_data = b'' if associated_data is None else associated_data
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_mac = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":233
+  /* "monocypher.pyx":232
  *         """
  *         mac = bytes(16)
  *         crypto_text = bytes(len(message))             # <<<<<<<<<<<<<<
  *         associated_data = b'' if associated_data is None else associated_data
  *         crypto_aead_write(&self._ctx, crypto_text, mac, associated_data, len(associated_data), message, len(message))
  */
-  __pyx_t_2 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 233, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_crypto_text = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":234
+  /* "monocypher.pyx":233
  *         mac = bytes(16)
  *         crypto_text = bytes(len(message))
  *         associated_data = b'' if associated_data is None else associated_data             # <<<<<<<<<<<<<<
  *         crypto_aead_write(&self._ctx, crypto_text, mac, associated_data, len(associated_data), message, len(message))
  *         return mac, crypto_text
  */
   __pyx_t_4 = (__pyx_v_associated_data == Py_None);
@@ -4899,50 +4932,50 @@
   } else {
     __Pyx_INCREF(__pyx_v_associated_data);
     __pyx_t_3 = __pyx_v_associated_data;
   }
   __Pyx_DECREF_SET(__pyx_v_associated_data, __pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":235
+  /* "monocypher.pyx":234
  *         crypto_text = bytes(len(message))
  *         associated_data = b'' if associated_data is None else associated_data
  *         crypto_aead_write(&self._ctx, crypto_text, mac, associated_data, len(associated_data), message, len(message))             # <<<<<<<<<<<<<<
  *         return mac, crypto_text
  * 
  */
-  __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_crypto_text); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_v_mac); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_associated_data); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
-  __pyx_t_2 = PyObject_Length(__pyx_v_associated_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
-  __pyx_t_9 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_crypto_text); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_v_mac); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_associated_data); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_associated_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_9 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 234, __pyx_L1_error)
   crypto_aead_write((&__pyx_v_self->_ctx), __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_2, __pyx_t_8, __pyx_t_9);
 
-  /* "monocypher.pyx":236
+  /* "monocypher.pyx":235
  *         associated_data = b'' if associated_data is None else associated_data
  *         crypto_aead_write(&self._ctx, crypto_text, mac, associated_data, len(associated_data), message, len(message))
  *         return mac, crypto_text             # <<<<<<<<<<<<<<
  * 
  *     def unlock(self, mac, message, associated_data=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_mac);
   __Pyx_GIVEREF(__pyx_v_mac);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_mac)) __PYX_ERR(0, 236, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_mac)) __PYX_ERR(0, 235, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_crypto_text);
   __Pyx_GIVEREF(__pyx_v_crypto_text);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_crypto_text)) __PYX_ERR(0, 236, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_crypto_text)) __PYX_ERR(0, 235, __pyx_L1_error);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":223
+  /* "monocypher.pyx":222
  *         crypto_aead_init_x(&self._ctx, key, nonce)
  * 
  *     def lock(self, message, associated_data=None):             # <<<<<<<<<<<<<<
  *         """Perform authenticated encryption.
  * 
  */
 
@@ -4957,15 +4990,15 @@
   __Pyx_XDECREF(__pyx_v_crypto_text);
   __Pyx_XDECREF(__pyx_v_associated_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":238
+/* "monocypher.pyx":237
  *         return mac, crypto_text
  * 
  *     def unlock(self, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *         """Perform authenticated decryption.
  * 
  */
 
@@ -5026,37 +5059,37 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mac)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 237, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 237, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("unlock", 0, 2, 3, 1); __PYX_ERR(0, 238, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("unlock", 0, 2, 3, 1); __PYX_ERR(0, 237, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_associated_data);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 237, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "unlock") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "unlock") < 0)) __PYX_ERR(0, 237, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -5066,15 +5099,15 @@
     }
     __pyx_v_mac = values[0];
     __pyx_v_message = values[1];
     __pyx_v_associated_data = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("unlock", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 238, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("unlock", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 237, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5114,87 +5147,87 @@
   uint8_t const *__pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unlock", 0);
   __Pyx_INCREF(__pyx_v_associated_data);
 
-  /* "monocypher.pyx":247
+  /* "monocypher.pyx":246
  *         :return: The secret message or None on authentication failure.
  *         """
  *         if len(mac) != 16:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid mac length {len(mac)} != 16')
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_mac); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_mac); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 246, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 16);
   if (unlikely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":248
+    /* "monocypher.pyx":247
  *         """
  *         if len(mac) != 16:
  *             raise ValueError(f'Invalid mac length {len(mac)} != 16')             # <<<<<<<<<<<<<<
  * 
  *         plain_text = bytearray(len(message))
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = 0;
     __pyx_t_4 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_mac_length);
     __pyx_t_1 += 19;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_mac_length);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Invalid_mac_length);
-    __pyx_t_5 = PyObject_Length(__pyx_v_mac); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 248, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_mac); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_1 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_kp_u_16);
     __pyx_t_1 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_16);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_16);
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 248, __pyx_L1_error)
+    __PYX_ERR(0, 247, __pyx_L1_error)
 
-    /* "monocypher.pyx":247
+    /* "monocypher.pyx":246
  *         :return: The secret message or None on authentication failure.
  *         """
  *         if len(mac) != 16:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid mac length {len(mac)} != 16')
  * 
  */
   }
 
-  /* "monocypher.pyx":250
+  /* "monocypher.pyx":249
  *             raise ValueError(f'Invalid mac length {len(mac)} != 16')
  * 
  *         plain_text = bytearray(len(message))             # <<<<<<<<<<<<<<
  *         associated_data = b'' if associated_data is None else associated_data
  *         rv = crypto_aead_read(&self._ctx, plain_text, mac, associated_data, len(associated_data), message, len(message))
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 250, __pyx_L1_error)
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_plain_text = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "monocypher.pyx":251
+  /* "monocypher.pyx":250
  * 
  *         plain_text = bytearray(len(message))
  *         associated_data = b'' if associated_data is None else associated_data             # <<<<<<<<<<<<<<
  *         rv = crypto_aead_read(&self._ctx, plain_text, mac, associated_data, len(associated_data), message, len(message))
  *         if 0 != rv:
  */
   __pyx_t_2 = (__pyx_v_associated_data == Py_None);
@@ -5204,72 +5237,72 @@
   } else {
     __Pyx_INCREF(__pyx_v_associated_data);
     __pyx_t_6 = __pyx_v_associated_data;
   }
   __Pyx_DECREF_SET(__pyx_v_associated_data, __pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "monocypher.pyx":252
+  /* "monocypher.pyx":251
  *         plain_text = bytearray(len(message))
  *         associated_data = b'' if associated_data is None else associated_data
  *         rv = crypto_aead_read(&self._ctx, plain_text, mac, associated_data, len(associated_data), message, len(message))             # <<<<<<<<<<<<<<
  *         if 0 != rv:
  *             return None
  */
-  __pyx_t_7 = __Pyx_PyObject_AsWritableUString(__pyx_v_plain_text); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_mac); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_associated_data); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L1_error)
-  __pyx_t_1 = PyObject_Length(__pyx_v_associated_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 252, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L1_error)
-  __pyx_t_5 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsWritableUString(__pyx_v_plain_text); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_mac); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_associated_data); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_associated_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 251, __pyx_L1_error)
   __pyx_v_rv = crypto_aead_read((&__pyx_v_self->_ctx), __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_1, __pyx_t_10, __pyx_t_5);
 
-  /* "monocypher.pyx":253
+  /* "monocypher.pyx":252
  *         associated_data = b'' if associated_data is None else associated_data
  *         rv = crypto_aead_read(&self._ctx, plain_text, mac, associated_data, len(associated_data), message, len(message))
  *         if 0 != rv:             # <<<<<<<<<<<<<<
  *             return None
  *         return plain_text
  */
   __pyx_t_2 = (0 != __pyx_v_rv);
   if (__pyx_t_2) {
 
-    /* "monocypher.pyx":254
+    /* "monocypher.pyx":253
  *         rv = crypto_aead_read(&self._ctx, plain_text, mac, associated_data, len(associated_data), message, len(message))
  *         if 0 != rv:
  *             return None             # <<<<<<<<<<<<<<
  *         return plain_text
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "monocypher.pyx":253
+    /* "monocypher.pyx":252
  *         associated_data = b'' if associated_data is None else associated_data
  *         rv = crypto_aead_read(&self._ctx, plain_text, mac, associated_data, len(associated_data), message, len(message))
  *         if 0 != rv:             # <<<<<<<<<<<<<<
  *             return None
  *         return plain_text
  */
   }
 
-  /* "monocypher.pyx":255
+  /* "monocypher.pyx":254
  *         if 0 != rv:
  *             return None
  *         return plain_text             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_plain_text);
   __pyx_r = __pyx_v_plain_text;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":238
+  /* "monocypher.pyx":237
  *         return mac, crypto_text
  * 
  *     def unlock(self, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *         """Perform authenticated decryption.
  * 
  */
 
@@ -5497,15 +5530,15 @@
   __Pyx_AddTraceback("monocypher.IncrementalAuthenticatedEncryption.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":258
+/* "monocypher.pyx":257
  * 
  * 
  * def chacha20(key, nonce, message):             # <<<<<<<<<<<<<<
  *     """Encrypt/Decrypt a message with ChaCha20.
  * 
  */
 
@@ -5565,55 +5598,55 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 258, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 257, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nonce)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 258, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 257, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("chacha20", 1, 3, 3, 1); __PYX_ERR(0, 258, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("chacha20", 1, 3, 3, 1); __PYX_ERR(0, 257, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 258, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 257, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("chacha20", 1, 3, 3, 2); __PYX_ERR(0, 258, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("chacha20", 1, 3, 3, 2); __PYX_ERR(0, 257, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "chacha20") < 0)) __PYX_ERR(0, 258, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "chacha20") < 0)) __PYX_ERR(0, 257, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_key = values[0];
     __pyx_v_nonce = values[1];
     __pyx_v_message = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("chacha20", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 258, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("chacha20", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 257, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5652,129 +5685,129 @@
   uint8_t const *__pyx_t_10;
   uint8_t const *__pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chacha20", 1);
 
-  /* "monocypher.pyx":266
+  /* "monocypher.pyx":265
  *     :return: The message XOR'ed with the ChaCha20 stream.
  *     """
  *     result = bytes(len(message))             # <<<<<<<<<<<<<<
  *     if 24 == len(nonce):
  *         crypto_chacha20_x(result, message, len(message), key, nonce, 0)
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 266, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":267
+  /* "monocypher.pyx":266
  *     """
  *     result = bytes(len(message))
  *     if 24 == len(nonce):             # <<<<<<<<<<<<<<
  *         crypto_chacha20_x(result, message, len(message), key, nonce, 0)
  *     elif 8 == len(nonce):
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_nonce); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_nonce); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 266, __pyx_L1_error)
   __pyx_t_4 = (24 == __pyx_t_1);
   if (__pyx_t_4) {
 
-    /* "monocypher.pyx":268
+    /* "monocypher.pyx":267
  *     result = bytes(len(message))
  *     if 24 == len(nonce):
  *         crypto_chacha20_x(result, message, len(message), key, nonce, 0)             # <<<<<<<<<<<<<<
  *     elif 8 == len(nonce):
  *         crypto_chacha20_djb(result, message, len(message), key, nonce, 0)
  */
-    __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_result); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L1_error)
-    __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 268, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_result); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 267, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 267, __pyx_L1_error)
+    __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 267, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 267, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 267, __pyx_L1_error)
     (void)(crypto_chacha20_x(__pyx_t_5, __pyx_t_6, __pyx_t_1, __pyx_t_7, __pyx_t_8, 0));
 
-    /* "monocypher.pyx":267
+    /* "monocypher.pyx":266
  *     """
  *     result = bytes(len(message))
  *     if 24 == len(nonce):             # <<<<<<<<<<<<<<
  *         crypto_chacha20_x(result, message, len(message), key, nonce, 0)
  *     elif 8 == len(nonce):
  */
     goto __pyx_L3;
   }
 
-  /* "monocypher.pyx":269
+  /* "monocypher.pyx":268
  *     if 24 == len(nonce):
  *         crypto_chacha20_x(result, message, len(message), key, nonce, 0)
  *     elif 8 == len(nonce):             # <<<<<<<<<<<<<<
  *         crypto_chacha20_djb(result, message, len(message), key, nonce, 0)
  *         pass
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_nonce); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_nonce); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 268, __pyx_L1_error)
   __pyx_t_4 = (8 == __pyx_t_1);
   if (likely(__pyx_t_4)) {
 
-    /* "monocypher.pyx":270
+    /* "monocypher.pyx":269
  *         crypto_chacha20_x(result, message, len(message), key, nonce, 0)
  *     elif 8 == len(nonce):
  *         crypto_chacha20_djb(result, message, len(message), key, nonce, 0)             # <<<<<<<<<<<<<<
  *         pass
  *     else:
  */
-    __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_result); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 270, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 270, __pyx_L1_error)
-    __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 270, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 270, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 270, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_result); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_1 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_AsUString(__pyx_v_nonce); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L1_error)
     (void)(crypto_chacha20_djb(__pyx_t_5, __pyx_t_9, __pyx_t_1, __pyx_t_10, __pyx_t_11, 0));
 
-    /* "monocypher.pyx":269
+    /* "monocypher.pyx":268
  *     if 24 == len(nonce):
  *         crypto_chacha20_x(result, message, len(message), key, nonce, 0)
  *     elif 8 == len(nonce):             # <<<<<<<<<<<<<<
  *         crypto_chacha20_djb(result, message, len(message), key, nonce, 0)
  *         pass
  */
     goto __pyx_L3;
   }
 
-  /* "monocypher.pyx":273
+  /* "monocypher.pyx":272
  *         pass
  *     else:
  *         raise ValueError('invalid nonce length')             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 273, __pyx_L1_error)
+    __PYX_ERR(0, 272, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "monocypher.pyx":274
+  /* "monocypher.pyx":273
  *     else:
  *         raise ValueError('invalid nonce length')
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":258
+  /* "monocypher.pyx":257
  * 
  * 
  * def chacha20(key, nonce, message):             # <<<<<<<<<<<<<<
  *     """Encrypt/Decrypt a message with ChaCha20.
  * 
  */
 
@@ -5787,15 +5820,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":277
+/* "monocypher.pyx":276
  * 
  * 
  * def blake2b(msg, key=None):             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     if isinstance(msg, str):
  */
 
@@ -5852,27 +5885,27 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_msg)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 277, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 276, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 277, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 276, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "blake2b") < 0)) __PYX_ERR(0, 277, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "blake2b") < 0)) __PYX_ERR(0, 276, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
@@ -5880,15 +5913,15 @@
       }
     }
     __pyx_v_msg = values[0];
     __pyx_v_key = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("blake2b", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 277, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("blake2b", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 276, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5929,15 +5962,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("blake2b", 0);
   __Pyx_INCREF(__pyx_v_msg);
   __Pyx_INCREF(__pyx_v_key);
 
-  /* "monocypher.pyx":278
+  /* "monocypher.pyx":277
  * 
  * def blake2b(msg, key=None):
  *     key = b'' if key is None else key             # <<<<<<<<<<<<<<
  *     if isinstance(msg, str):
  *         msg = msg.encode('utf-8')
  */
   __pyx_t_2 = (__pyx_v_key == Py_None);
@@ -5947,32 +5980,32 @@
   } else {
     __Pyx_INCREF(__pyx_v_key);
     __pyx_t_1 = __pyx_v_key;
   }
   __Pyx_DECREF_SET(__pyx_v_key, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":279
+  /* "monocypher.pyx":278
  * def blake2b(msg, key=None):
  *     key = b'' if key is None else key
  *     if isinstance(msg, str):             # <<<<<<<<<<<<<<
  *         msg = msg.encode('utf-8')
  *     hash = bytes(64)
  */
   __pyx_t_2 = PyUnicode_Check(__pyx_v_msg); 
   if (__pyx_t_2) {
 
-    /* "monocypher.pyx":280
+    /* "monocypher.pyx":279
  *     key = b'' if key is None else key
  *     if isinstance(msg, str):
  *         msg = msg.encode('utf-8')             # <<<<<<<<<<<<<<
  *     hash = bytes(64)
  *     crypto_blake2b_keyed(hash, len(hash), key, len(key), msg, len(msg))
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 280, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 279, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -5984,70 +6017,70 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_u_utf_8};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_msg, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":279
+    /* "monocypher.pyx":278
  * def blake2b(msg, key=None):
  *     key = b'' if key is None else key
  *     if isinstance(msg, str):             # <<<<<<<<<<<<<<
  *         msg = msg.encode('utf-8')
  *     hash = bytes(64)
  */
   }
 
-  /* "monocypher.pyx":281
+  /* "monocypher.pyx":280
  *     if isinstance(msg, str):
  *         msg = msg.encode('utf-8')
  *     hash = bytes(64)             # <<<<<<<<<<<<<<
  *     crypto_blake2b_keyed(hash, len(hash), key, len(key), msg, len(msg))
  *     return hash
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_hash = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":282
+  /* "monocypher.pyx":281
  *         msg = msg.encode('utf-8')
  *     hash = bytes(64)
  *     crypto_blake2b_keyed(hash, len(hash), key, len(key), msg, len(msg))             # <<<<<<<<<<<<<<
  *     return hash
  * 
  */
-  __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hash); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hash); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 282, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L1_error)
-  __pyx_t_9 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 282, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_msg); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L1_error)
-  __pyx_t_11 = PyObject_Length(__pyx_v_msg); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hash); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hash); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_9 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_AsUString(__pyx_v_msg); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_11 = PyObject_Length(__pyx_v_msg); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
   crypto_blake2b_keyed(__pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11);
 
-  /* "monocypher.pyx":283
+  /* "monocypher.pyx":282
  *     hash = bytes(64)
  *     crypto_blake2b_keyed(hash, len(hash), key, len(key), msg, len(msg))
  *     return hash             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_hash);
   __pyx_r = __pyx_v_hash;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":277
+  /* "monocypher.pyx":276
  * 
  * 
  * def blake2b(msg, key=None):             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     if isinstance(msg, str):
  */
 
@@ -6063,15 +6096,15 @@
   __Pyx_XDECREF(__pyx_v_msg);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":295
+/* "monocypher.pyx":294
  *     :param hash_size: The resulting hash size.  None (default) is 64.
  *     """
  *     def __init__(self, key=None, hash_size=None):             # <<<<<<<<<<<<<<
  *         key = b'' if key is None else key
  *         self._hash_size = 64 if hash_size is None else hash_size
  */
 
@@ -6111,27 +6144,27 @@
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 295, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_hash_size);
           if (value) { values[1] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 295, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 295, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 294, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -6140,15 +6173,15 @@
       }
     }
     __pyx_v_key = values[0];
     __pyx_v_hash_size = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 295, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 294, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
@@ -6182,15 +6215,15 @@
   Py_ssize_t __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __Pyx_INCREF(__pyx_v_key);
 
-  /* "monocypher.pyx":296
+  /* "monocypher.pyx":295
  *     """
  *     def __init__(self, key=None, hash_size=None):
  *         key = b'' if key is None else key             # <<<<<<<<<<<<<<
  *         self._hash_size = 64 if hash_size is None else hash_size
  *         crypto_blake2b_keyed_init(&self._ctx, self._hash_size, key, len(key))
  */
   __pyx_t_2 = (__pyx_v_key == Py_None);
@@ -6200,42 +6233,42 @@
   } else {
     __Pyx_INCREF(__pyx_v_key);
     __pyx_t_1 = __pyx_v_key;
   }
   __Pyx_DECREF_SET(__pyx_v_key, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":297
+  /* "monocypher.pyx":296
  *     def __init__(self, key=None, hash_size=None):
  *         key = b'' if key is None else key
  *         self._hash_size = 64 if hash_size is None else hash_size             # <<<<<<<<<<<<<<
  *         crypto_blake2b_keyed_init(&self._ctx, self._hash_size, key, len(key))
  * 
  */
   __pyx_t_2 = (__pyx_v_hash_size == Py_None);
   if (__pyx_t_2) {
     __pyx_t_3 = 64;
   } else {
-    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_v_hash_size); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_v_hash_size); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 296, __pyx_L1_error)
     __pyx_t_3 = __pyx_t_4;
   }
   __pyx_v_self->_hash_size = __pyx_t_3;
 
-  /* "monocypher.pyx":298
+  /* "monocypher.pyx":297
  *         key = b'' if key is None else key
  *         self._hash_size = 64 if hash_size is None else hash_size
  *         crypto_blake2b_keyed_init(&self._ctx, self._hash_size, key, len(key))             # <<<<<<<<<<<<<<
  * 
  *     def update(self, message):
  */
-  __pyx_t_5 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 298, __pyx_L1_error)
-  __pyx_t_6 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 297, __pyx_L1_error)
   crypto_blake2b_keyed_init((&__pyx_v_self->_ctx), __pyx_v_self->_hash_size, __pyx_t_5, __pyx_t_6);
 
-  /* "monocypher.pyx":295
+  /* "monocypher.pyx":294
  *     :param hash_size: The resulting hash size.  None (default) is 64.
  *     """
  *     def __init__(self, key=None, hash_size=None):             # <<<<<<<<<<<<<<
  *         key = b'' if key is None else key
  *         self._hash_size = 64 if hash_size is None else hash_size
  */
 
@@ -6248,15 +6281,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":300
+/* "monocypher.pyx":299
  *         crypto_blake2b_keyed_init(&self._ctx, self._hash_size, key, len(key))
  * 
  *     def update(self, message):             # <<<<<<<<<<<<<<
  *         """Add new data to the hash.
  * 
  */
 
@@ -6310,31 +6343,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 300, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 299, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "update") < 0)) __PYX_ERR(0, 300, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "update") < 0)) __PYX_ERR(0, 299, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_message = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("update", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 300, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("update", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 299, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6363,26 +6396,26 @@
   uint8_t const *__pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("update", 1);
 
-  /* "monocypher.pyx":305
+  /* "monocypher.pyx":304
  *         :param message: Additional data to hash.
  *         """
  *         crypto_blake2b_update(&self._ctx, message, len(message))             # <<<<<<<<<<<<<<
  * 
  *     def finalize(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 305, __pyx_L1_error)
-  __pyx_t_2 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 305, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 304, __pyx_L1_error)
   crypto_blake2b_update((&__pyx_v_self->_ctx), __pyx_t_1, __pyx_t_2);
 
-  /* "monocypher.pyx":300
+  /* "monocypher.pyx":299
  *         crypto_blake2b_keyed_init(&self._ctx, self._hash_size, key, len(key))
  * 
  *     def update(self, message):             # <<<<<<<<<<<<<<
  *         """Add new data to the hash.
  * 
  */
 
@@ -6394,15 +6427,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":307
+/* "monocypher.pyx":306
  *         crypto_blake2b_update(&self._ctx, message, len(message))
  * 
  *     def finalize(self):             # <<<<<<<<<<<<<<
  *         """Finalize and return the computed hash.
  * 
  */
 
@@ -6456,52 +6489,52 @@
   PyObject *__pyx_t_2 = NULL;
   uint8_t *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("finalize", 1);
 
-  /* "monocypher.pyx":312
+  /* "monocypher.pyx":311
  *         :return: The hash.
  *         """
  *         hash = bytes(self._hash_size)             # <<<<<<<<<<<<<<
  *         crypto_blake2b_final(&self._ctx, hash)
  *         return hash
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_hash_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_hash_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_hash = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":313
+  /* "monocypher.pyx":312
  *         """
  *         hash = bytes(self._hash_size)
  *         crypto_blake2b_final(&self._ctx, hash)             # <<<<<<<<<<<<<<
  *         return hash
  * 
  */
-  __pyx_t_3 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hash); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hash); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 312, __pyx_L1_error)
   crypto_blake2b_final((&__pyx_v_self->_ctx), __pyx_t_3);
 
-  /* "monocypher.pyx":314
+  /* "monocypher.pyx":313
  *         hash = bytes(self._hash_size)
  *         crypto_blake2b_final(&self._ctx, hash)
  *         return hash             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_hash);
   __pyx_r = __pyx_v_hash;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":307
+  /* "monocypher.pyx":306
  *         crypto_blake2b_update(&self._ctx, message, len(message))
  * 
  *     def finalize(self):             # <<<<<<<<<<<<<<
  *         """Finalize and return the computed hash.
  * 
  */
 
@@ -6728,15 +6761,15 @@
   __Pyx_AddTraceback("monocypher.Blake2b.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":317
+/* "monocypher.pyx":316
  * 
  * 
  * cdef uint32_t _validate_u32(variable_name, value):             # <<<<<<<<<<<<<<
  *     if value > 0xffff_ffff:
  *         raise ValueError(f'{variable_name} too long: {value}')
  */
 
@@ -6750,86 +6783,86 @@
   PyObject *__pyx_t_5 = NULL;
   uint32_t __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_validate_u32", 1);
 
-  /* "monocypher.pyx":318
+  /* "monocypher.pyx":317
  * 
  * cdef uint32_t _validate_u32(variable_name, value):
  *     if value > 0xffff_ffff:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'{variable_name} too long: {value}')
  *     return <uint32_t> value
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_4294967295, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_4294967295, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":319
+    /* "monocypher.pyx":318
  * cdef uint32_t _validate_u32(variable_name, value):
  *     if value > 0xffff_ffff:
  *         raise ValueError(f'{variable_name} too long: {value}')             # <<<<<<<<<<<<<<
  *     return <uint32_t> value
  * 
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = 0;
     __pyx_t_4 = 127;
-    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_variable_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_variable_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_4 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_4) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_4;
     __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_INCREF(__pyx_kp_u_too_long);
     __pyx_t_3 += 11;
     __Pyx_GIVEREF(__pyx_kp_u_too_long);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_too_long);
-    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_value, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_value, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_4 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_4) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_4;
     __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 319, __pyx_L1_error)
+    __PYX_ERR(0, 318, __pyx_L1_error)
 
-    /* "monocypher.pyx":318
+    /* "monocypher.pyx":317
  * 
  * cdef uint32_t _validate_u32(variable_name, value):
  *     if value > 0xffff_ffff:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'{variable_name} too long: {value}')
  *     return <uint32_t> value
  */
   }
 
-  /* "monocypher.pyx":320
+  /* "monocypher.pyx":319
  *     if value > 0xffff_ffff:
  *         raise ValueError(f'{variable_name} too long: {value}')
  *     return <uint32_t> value             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_v_value); if (unlikely((__pyx_t_6 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_v_value); if (unlikely((__pyx_t_6 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L1_error)
   __pyx_r = ((uint32_t)__pyx_t_6);
   goto __pyx_L0;
 
-  /* "monocypher.pyx":317
+  /* "monocypher.pyx":316
  * 
  * 
  * cdef uint32_t _validate_u32(variable_name, value):             # <<<<<<<<<<<<<<
  *     if value > 0xffff_ffff:
  *         raise ValueError(f'{variable_name} too long: {value}')
  */
 
@@ -6840,15 +6873,15 @@
   __Pyx_AddTraceback("monocypher._validate_u32", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":323
+/* "monocypher.pyx":322
  * 
  * 
  * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
 
@@ -6918,64 +6951,64 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nb_blocks)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nb_iterations)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 1); __PYX_ERR(0, 323, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 1); __PYX_ERR(0, 322, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_password)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 2); __PYX_ERR(0, 323, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 2); __PYX_ERR(0, 322, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_salt)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 3); __PYX_ERR(0, 323, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 3); __PYX_ERR(0, 322, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ad);
           if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "argon2i_32") < 0)) __PYX_ERR(0, 323, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "argon2i_32") < 0)) __PYX_ERR(0, 322, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
@@ -6992,15 +7025,15 @@
     __pyx_v_password = values[2];
     __pyx_v_salt = values[3];
     __pyx_v_key = values[4];
     __pyx_v_ad = values[5];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, __pyx_nargs); __PYX_ERR(0, 323, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, __pyx_nargs); __PYX_ERR(0, 322, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -7053,15 +7086,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("argon2i_32", 0);
   __Pyx_INCREF(__pyx_v_key);
   __Pyx_INCREF(__pyx_v_ad);
 
-  /* "monocypher.pyx":324
+  /* "monocypher.pyx":323
  * 
  * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:
  *     key = b'' if key is None else key             # <<<<<<<<<<<<<<
  *     ad = b'' if ad is None else ad
  * 
  */
   __pyx_t_2 = (__pyx_v_key == Py_None);
@@ -7071,15 +7104,15 @@
   } else {
     __Pyx_INCREF(__pyx_v_key);
     __pyx_t_1 = __pyx_v_key;
   }
   __Pyx_DECREF_SET(__pyx_v_key, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":325
+  /* "monocypher.pyx":324
  * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad             # <<<<<<<<<<<<<<
  * 
  *     cdef crypto_argon2_config config;
  */
   __pyx_t_2 = (__pyx_v_ad == Py_None);
@@ -7089,194 +7122,194 @@
   } else {
     __Pyx_INCREF(__pyx_v_ad);
     __pyx_t_1 = __pyx_v_ad;
   }
   __Pyx_DECREF_SET(__pyx_v_ad, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":328
+  /* "monocypher.pyx":327
  * 
  *     cdef crypto_argon2_config config;
  *     config.algorithm = 1             # <<<<<<<<<<<<<<
  *     config.nb_block = nb_blocks
  *     config.nb_passes = nb_iterations
  */
   __pyx_v_config.algorithm = 1;
 
-  /* "monocypher.pyx":329
+  /* "monocypher.pyx":328
  *     cdef crypto_argon2_config config;
  *     config.algorithm = 1
  *     config.nb_block = nb_blocks             # <<<<<<<<<<<<<<
  *     config.nb_passes = nb_iterations
  *     config.nb_lanes = 1
  */
-  __pyx_t_1 = __pyx_convert__to_py_crypto_argon2_config(__pyx_v_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert__to_py_crypto_argon2_config(__pyx_v_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_nb_block, __pyx_v_nb_blocks) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_nb_block, __pyx_v_nb_blocks) < 0) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":330
+  /* "monocypher.pyx":329
  *     config.algorithm = 1
  *     config.nb_block = nb_blocks
  *     config.nb_passes = nb_iterations             # <<<<<<<<<<<<<<
  *     config.nb_lanes = 1
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_nb_iterations); if (unlikely((__pyx_t_3 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_nb_iterations); if (unlikely((__pyx_t_3 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L1_error)
   __pyx_v_config.nb_passes = __pyx_t_3;
 
-  /* "monocypher.pyx":331
+  /* "monocypher.pyx":330
  *     config.nb_block = nb_blocks
  *     config.nb_passes = nb_iterations
  *     config.nb_lanes = 1             # <<<<<<<<<<<<<<
  * 
  *     cdef crypto_argon2_inputs inputs;
  */
   __pyx_v_config.nb_lanes = 1;
 
-  /* "monocypher.pyx":334
+  /* "monocypher.pyx":333
  * 
  *     cdef crypto_argon2_inputs inputs;
  *     inputs.pass_ = password             # <<<<<<<<<<<<<<
  *     inputs.pass_size = _validate_u32('password', len(password))
  *     inputs.salt = salt
  */
-  __pyx_t_4 = __Pyx_PyObject_AsUString(__pyx_v_password); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_AsUString(__pyx_v_password); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 333, __pyx_L1_error)
   __pyx_v_inputs.pass = __pyx_t_4;
 
-  /* "monocypher.pyx":335
+  /* "monocypher.pyx":334
  *     cdef crypto_argon2_inputs inputs;
  *     inputs.pass_ = password
  *     inputs.pass_size = _validate_u32('password', len(password))             # <<<<<<<<<<<<<<
  *     inputs.salt = salt
  *     inputs.salt_size = _validate_u32('salt', len(salt))
  */
-  __pyx_t_5 = PyObject_Length(__pyx_v_password); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 335, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_password); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_password, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_password, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_inputs.pass_size = __pyx_t_3;
 
-  /* "monocypher.pyx":336
+  /* "monocypher.pyx":335
  *     inputs.pass_ = password
  *     inputs.pass_size = _validate_u32('password', len(password))
  *     inputs.salt = salt             # <<<<<<<<<<<<<<
  *     inputs.salt_size = _validate_u32('salt', len(salt))
  * 
  */
-  __pyx_t_6 = __Pyx_PyObject_AsUString(__pyx_v_salt); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsUString(__pyx_v_salt); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
   __pyx_v_inputs.salt = __pyx_t_6;
 
-  /* "monocypher.pyx":337
+  /* "monocypher.pyx":336
  *     inputs.pass_size = _validate_u32('password', len(password))
  *     inputs.salt = salt
  *     inputs.salt_size = _validate_u32('salt', len(salt))             # <<<<<<<<<<<<<<
  * 
  *     cdef crypto_argon2_extras extras;
  */
-  __pyx_t_5 = PyObject_Length(__pyx_v_salt); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 337, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_salt); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_salt, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_salt, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_inputs.salt_size = __pyx_t_3;
 
-  /* "monocypher.pyx":340
+  /* "monocypher.pyx":339
  * 
  *     cdef crypto_argon2_extras extras;
  *     extras.key = key             # <<<<<<<<<<<<<<
  *     extras.key_size = _validate_u32('key', len(key))
  *     extras.ad = ad
  */
-  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 339, __pyx_L1_error)
   __pyx_v_extras.key = __pyx_t_7;
 
-  /* "monocypher.pyx":341
+  /* "monocypher.pyx":340
  *     cdef crypto_argon2_extras extras;
  *     extras.key = key
  *     extras.key_size = _validate_u32('key', len(key))             # <<<<<<<<<<<<<<
  *     extras.ad = ad
  *     extras.ad_size = _validate_u32('ad', len(ad))
  */
-  __pyx_t_5 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 341, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_key, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_key, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_extras.key_size = __pyx_t_3;
 
-  /* "monocypher.pyx":342
+  /* "monocypher.pyx":341
  *     extras.key = key
  *     extras.key_size = _validate_u32('key', len(key))
  *     extras.ad = ad             # <<<<<<<<<<<<<<
  *     extras.ad_size = _validate_u32('ad', len(ad))
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_ad); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_ad); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
   __pyx_v_extras.ad = __pyx_t_8;
 
-  /* "monocypher.pyx":343
+  /* "monocypher.pyx":342
  *     extras.key_size = _validate_u32('key', len(key))
  *     extras.ad = ad
  *     extras.ad_size = _validate_u32('ad', len(ad))             # <<<<<<<<<<<<<<
  * 
  *     hash = bytes(32)
  */
-  __pyx_t_5 = PyObject_Length(__pyx_v_ad); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 343, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_ad); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_ad, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_ad, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_extras.ad_size = __pyx_t_3;
 
-  /* "monocypher.pyx":345
+  /* "monocypher.pyx":344
  *     extras.ad_size = _validate_u32('ad', len(ad))
  * 
  *     hash = bytes(32)             # <<<<<<<<<<<<<<
  *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))
  *     try:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_hash = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":346
+  /* "monocypher.pyx":345
  * 
  *     hash = bytes(32)
  *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))             # <<<<<<<<<<<<<<
  *     try:
  *         crypto_argon2(hash, <uint32_t> len(hash), work_area, config, inputs, extras)
  */
-  __pyx_t_9 = __Pyx_PyInt_As_size_t(__pyx_v_nb_blocks); if (unlikely((__pyx_t_9 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_size_t(__pyx_v_nb_blocks); if (unlikely((__pyx_t_9 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
   __pyx_v_work_area = malloc((((size_t)__pyx_t_9) * ((size_t)0x400)));
 
-  /* "monocypher.pyx":347
+  /* "monocypher.pyx":346
  *     hash = bytes(32)
  *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))
  *     try:             # <<<<<<<<<<<<<<
  *         crypto_argon2(hash, <uint32_t> len(hash), work_area, config, inputs, extras)
  *     finally:
  */
   /*try:*/ {
 
-    /* "monocypher.pyx":348
+    /* "monocypher.pyx":347
  *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))
  *     try:
  *         crypto_argon2(hash, <uint32_t> len(hash), work_area, config, inputs, extras)             # <<<<<<<<<<<<<<
  *     finally:
  *         free(work_area)
  */
-    __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hash); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L4_error)
-    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hash); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 348, __pyx_L4_error)
+    __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hash); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 347, __pyx_L4_error)
+    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hash); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 347, __pyx_L4_error)
     crypto_argon2(__pyx_t_10, ((uint32_t)__pyx_t_5), __pyx_v_work_area, __pyx_v_config, __pyx_v_inputs, __pyx_v_extras);
   }
 
-  /* "monocypher.pyx":350
+  /* "monocypher.pyx":349
  *         crypto_argon2(hash, <uint32_t> len(hash), work_area, config, inputs, extras)
  *     finally:
  *         free(work_area)             # <<<<<<<<<<<<<<
  *     crypto_wipe(password, len(password))
  *     return hash
  */
   /*finally:*/ {
@@ -7315,38 +7348,38 @@
       __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
       __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_12; __pyx_filename = __pyx_t_13;
       goto __pyx_L1_error;
     }
     __pyx_L5:;
   }
 
-  /* "monocypher.pyx":351
+  /* "monocypher.pyx":350
  *     finally:
  *         free(work_area)
  *     crypto_wipe(password, len(password))             # <<<<<<<<<<<<<<
  *     return hash
  * 
  */
-  __pyx_t_10 = __Pyx_PyObject_AsWritableUString(__pyx_v_password); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
-  __pyx_t_5 = PyObject_Length(__pyx_v_password); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_AsWritableUString(__pyx_v_password); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_password); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 350, __pyx_L1_error)
   crypto_wipe(__pyx_t_10, __pyx_t_5);
 
-  /* "monocypher.pyx":352
+  /* "monocypher.pyx":351
  *         free(work_area)
  *     crypto_wipe(password, len(password))
  *     return hash             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_hash);
   __pyx_r = __pyx_v_hash;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":323
+  /* "monocypher.pyx":322
  * 
  * 
  * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
 
@@ -7360,15 +7393,15 @@
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_ad);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":355
+/* "monocypher.pyx":354
  * 
  * 
  * def compute_key_exchange_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
 
@@ -7422,45 +7455,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_secret_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 354, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_key_exchange_public_key") < 0)) __PYX_ERR(0, 355, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_key_exchange_public_key") < 0)) __PYX_ERR(0, 354, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_secret_key = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compute_key_exchange_public_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 355, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compute_key_exchange_public_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 354, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.compute_key_exchange_public_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 355, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 354, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_12compute_key_exchange_public_key(__pyx_self, __pyx_v_secret_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7482,50 +7515,50 @@
   uint8_t *__pyx_t_2;
   uint8_t const *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compute_key_exchange_public_key", 1);
 
-  /* "monocypher.pyx":361
+  /* "monocypher.pyx":360
  *     :return: The 32-byte public key for :func:`key_exchange`.
  *     """
  *     public_key = bytes(32)             # <<<<<<<<<<<<<<
  *     crypto_x25519_public_key(public_key, secret_key)
  *     return public_key
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_public_key = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":362
+  /* "monocypher.pyx":361
  *     """
  *     public_key = bytes(32)
  *     crypto_x25519_public_key(public_key, secret_key)             # <<<<<<<<<<<<<<
  *     return public_key
  * 
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public_key); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyBytes_AsUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public_key); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L1_error)
   crypto_x25519_public_key(__pyx_t_2, __pyx_t_3);
 
-  /* "monocypher.pyx":363
+  /* "monocypher.pyx":362
  *     public_key = bytes(32)
  *     crypto_x25519_public_key(public_key, secret_key)
  *     return public_key             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_public_key);
   __pyx_r = __pyx_v_public_key;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":355
+  /* "monocypher.pyx":354
  * 
  * 
  * def compute_key_exchange_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
 
@@ -7537,15 +7570,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_public_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":366
+/* "monocypher.pyx":365
  * 
  * 
  * def key_exchange(your_secret_key: bytes, their_public_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
 
@@ -7602,58 +7635,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_your_secret_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_their_public_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("key_exchange", 1, 2, 2, 1); __PYX_ERR(0, 366, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("key_exchange", 1, 2, 2, 1); __PYX_ERR(0, 365, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "key_exchange") < 0)) __PYX_ERR(0, 366, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "key_exchange") < 0)) __PYX_ERR(0, 365, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_your_secret_key = ((PyObject*)values[0]);
     __pyx_v_their_public_key = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("key_exchange", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 366, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("key_exchange", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 365, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.key_exchange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_your_secret_key), (&PyBytes_Type), 0, "your_secret_key", 1))) __PYX_ERR(0, 366, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_their_public_key), (&PyBytes_Type), 0, "their_public_key", 1))) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_your_secret_key), (&PyBytes_Type), 0, "your_secret_key", 1))) __PYX_ERR(0, 365, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_their_public_key), (&PyBytes_Type), 0, "their_public_key", 1))) __PYX_ERR(0, 365, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_14key_exchange(__pyx_self, __pyx_v_your_secret_key, __pyx_v_their_public_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7676,51 +7709,51 @@
   uint8_t const *__pyx_t_3;
   uint8_t const *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("key_exchange", 1);
 
-  /* "monocypher.pyx":374
+  /* "monocypher.pyx":373
  *         computed using their_secret_key and your_public_key.
  *     """
  *     p = bytes(32)             # <<<<<<<<<<<<<<
  *     crypto_x25519(p, your_secret_key, their_public_key)
  *     return p
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_p = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":375
+  /* "monocypher.pyx":374
  *     """
  *     p = bytes(32)
  *     crypto_x25519(p, your_secret_key, their_public_key)             # <<<<<<<<<<<<<<
  *     return p
  * 
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_p); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 375, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyBytes_AsUString(__pyx_v_your_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 375, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyBytes_AsUString(__pyx_v_their_public_key); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_p); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsUString(__pyx_v_your_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_AsUString(__pyx_v_their_public_key); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 374, __pyx_L1_error)
   crypto_x25519(__pyx_t_2, __pyx_t_3, __pyx_t_4);
 
-  /* "monocypher.pyx":376
+  /* "monocypher.pyx":375
  *     p = bytes(32)
  *     crypto_x25519(p, your_secret_key, their_public_key)
  *     return p             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_p);
   __pyx_r = __pyx_v_p;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":366
+  /* "monocypher.pyx":365
  * 
  * 
  * def key_exchange(your_secret_key: bytes, their_public_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
 
@@ -7732,15 +7765,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_p);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":379
+/* "monocypher.pyx":378
  * 
  * 
  * def compute_signing_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
 
@@ -7794,45 +7827,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_secret_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 379, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 378, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_signing_public_key") < 0)) __PYX_ERR(0, 379, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_signing_public_key") < 0)) __PYX_ERR(0, 378, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_secret_key = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compute_signing_public_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 379, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compute_signing_public_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 378, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.compute_signing_public_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 378, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_16compute_signing_public_key(__pyx_self, __pyx_v_secret_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7843,107 +7876,226 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_10monocypher_16compute_signing_public_key(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_secret_key) {
+  PyObject *__pyx_v_secret = NULL;
+  PyObject *__pyx_v_public = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  uint8_t *__pyx_t_6;
+  uint8_t *__pyx_t_7;
+  uint8_t *__pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("compute_signing_public_key", 1);
+  __Pyx_RefNannySetupContext("compute_signing_public_key", 0);
+  __Pyx_INCREF(__pyx_v_secret_key);
 
-  /* "monocypher.pyx":385
+  /* "monocypher.pyx":384
+ *     :return: The 32-byte public key.
+ *     """
+ *     if len(secret_key) == 32:             # <<<<<<<<<<<<<<
+ *         warnings.warn('Provide the full 64-byte key from generate_signing_key_pair()',
+ *                       DeprecationWarning, stacklevel=2)
+ */
+  __pyx_t_1 = __Pyx_PyBytes_GET_SIZE(__pyx_v_secret_key); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_t_1 == 32);
+  if (__pyx_t_2) {
+
+    /* "monocypher.pyx":385
+ *     """
+ *     if len(secret_key) == 32:
+ *         warnings.warn('Provide the full 64-byte key from generate_signing_key_pair()',             # <<<<<<<<<<<<<<
+ *                       DeprecationWarning, stacklevel=2)
+ *         secret = bytes(64)
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_warnings); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_warn); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "monocypher.pyx":386
+ *     if len(secret_key) == 32:
+ *         warnings.warn('Provide the full 64-byte key from generate_signing_key_pair()',
+ *                       DeprecationWarning, stacklevel=2)             # <<<<<<<<<<<<<<
+ *         secret = bytes(64)
+ *         public = bytes(32)
+ */
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_stacklevel, __pyx_int_2) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
+
+    /* "monocypher.pyx":385
+ *     """
+ *     if len(secret_key) == 32:
+ *         warnings.warn('Provide the full 64-byte key from generate_signing_key_pair()',             # <<<<<<<<<<<<<<
+ *                       DeprecationWarning, stacklevel=2)
+ *         secret = bytes(64)
+ */
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__8, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    /* "monocypher.pyx":387
+ *         warnings.warn('Provide the full 64-byte key from generate_signing_key_pair()',
+ *                       DeprecationWarning, stacklevel=2)
+ *         secret = bytes(64)             # <<<<<<<<<<<<<<
+ *         public = bytes(32)
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ */
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_v_secret = ((PyObject*)__pyx_t_5);
+    __pyx_t_5 = 0;
+
+    /* "monocypher.pyx":388
+ *                       DeprecationWarning, stacklevel=2)
+ *         secret = bytes(64)
+ *         public = bytes(32)             # <<<<<<<<<<<<<<
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ *         secret_key = secret
+ */
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_v_public = ((PyObject*)__pyx_t_5);
+    __pyx_t_5 = 0;
+
+    /* "monocypher.pyx":389
+ *         secret = bytes(64)
+ *         public = bytes(32)
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))             # <<<<<<<<<<<<<<
+ *         secret_key = secret
+ *     if len(secret_key) != 64:
+ */
+    __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_secret_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_8 = __Pyx_PyBytes_AsWritableUString(__pyx_t_5); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L1_error)
+    crypto_eddsa_key_pair(__pyx_t_6, __pyx_t_7, __pyx_t_8);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    /* "monocypher.pyx":390
+ *         public = bytes(32)
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ *         secret_key = secret             # <<<<<<<<<<<<<<
+ *     if len(secret_key) != 64:
+ *         raise ValueError('secret key length invalid')
+ */
+    __Pyx_INCREF(__pyx_v_secret);
+    __Pyx_DECREF_SET(__pyx_v_secret_key, __pyx_v_secret);
+
+    /* "monocypher.pyx":384
  *     :return: The 32-byte public key.
  *     """
+ *     if len(secret_key) == 32:             # <<<<<<<<<<<<<<
+ *         warnings.warn('Provide the full 64-byte key from generate_signing_key_pair()',
+ *                       DeprecationWarning, stacklevel=2)
+ */
+  }
+
+  /* "monocypher.pyx":391
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ *         secret_key = secret
  *     if len(secret_key) != 64:             # <<<<<<<<<<<<<<
  *         raise ValueError('secret key length invalid')
  *     return secret_key[32:]
  */
-  __pyx_t_1 = __Pyx_PyBytes_GET_SIZE(__pyx_v_secret_key); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_GET_SIZE(__pyx_v_secret_key); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 391, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 64);
   if (unlikely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":386
- *     """
+    /* "monocypher.pyx":392
+ *         secret_key = secret
  *     if len(secret_key) != 64:
  *         raise ValueError('secret key length invalid')             # <<<<<<<<<<<<<<
  *     return secret_key[32:]
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_Raise(__pyx_t_5, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __PYX_ERR(0, 392, __pyx_L1_error)
 
-    /* "monocypher.pyx":385
- *     :return: The 32-byte public key.
- *     """
+    /* "monocypher.pyx":391
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ *         secret_key = secret
  *     if len(secret_key) != 64:             # <<<<<<<<<<<<<<
  *         raise ValueError('secret key length invalid')
  *     return secret_key[32:]
  */
   }
 
-  /* "monocypher.pyx":387
+  /* "monocypher.pyx":393
  *     if len(secret_key) != 64:
  *         raise ValueError('secret key length invalid')
  *     return secret_key[32:]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PySequence_GetSlice(__pyx_v_secret_key, 32, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_r = ((PyObject*)__pyx_t_3);
-  __pyx_t_3 = 0;
+  __pyx_t_5 = PySequence_GetSlice(__pyx_v_secret_key, 32, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_r = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":379
+  /* "monocypher.pyx":378
  * 
  * 
  * def compute_signing_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("monocypher.compute_signing_public_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_secret);
+  __Pyx_XDECREF(__pyx_v_public);
+  __Pyx_XDECREF(__pyx_v_secret_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":390
+/* "monocypher.pyx":396
  * 
  * 
  * def signature_sign(secret_key: bytes, message: bytes) -> bytes:             # <<<<<<<<<<<<<<
- *     """Cryptographically sign a messge.
+ *     """Cryptographically sign a message.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_19signature_sign(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_10monocypher_18signature_sign, "Cryptographically sign a messge.\n\n    :param secret_key: Your 64-byte secret key.\n    :param message: The message to sign.\n    :return: The 64-byte signature of message.\n\n    For a quick description of the signing process, see the bottom of\n    https://pynacl.readthedocs.io/en/stable/signing/.\n    ");
+PyDoc_STRVAR(__pyx_doc_10monocypher_18signature_sign, "Cryptographically sign a message.\n\n    :param secret_key: Your 64-byte secret key.\n    :param message: The message to sign.\n    :return: The 64-byte signature of message.\n\n    For a quick description of the signing process, see the bottom of\n    https://pynacl.readthedocs.io/en/stable/signing/.\n    ");
 static PyMethodDef __pyx_mdef_10monocypher_19signature_sign = {"signature_sign", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10monocypher_19signature_sign, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_10monocypher_18signature_sign};
 static PyObject *__pyx_pw_10monocypher_19signature_sign(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -7984,58 +8136,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_secret_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 396, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 396, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("signature_sign", 1, 2, 2, 1); __PYX_ERR(0, 390, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature_sign", 1, 2, 2, 1); __PYX_ERR(0, 396, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "signature_sign") < 0)) __PYX_ERR(0, 390, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "signature_sign") < 0)) __PYX_ERR(0, 396, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_secret_key = ((PyObject*)values[0]);
     __pyx_v_message = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("signature_sign", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 390, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("signature_sign", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 396, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.signature_sign", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 390, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_message), (&PyBytes_Type), 0, "message", 1))) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 396, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_message), (&PyBytes_Type), 0, "message", 1))) __PYX_ERR(0, 396, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_18signature_sign(__pyx_self, __pyx_v_secret_key, __pyx_v_message);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8046,85 +8198,198 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_10monocypher_18signature_sign(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_secret_key, PyObject *__pyx_v_message) {
+  PyObject *__pyx_v_secret = NULL;
+  PyObject *__pyx_v_public = NULL;
   PyObject *__pyx_v_sig = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  uint8_t *__pyx_t_2;
-  uint8_t const *__pyx_t_3;
-  uint8_t const *__pyx_t_4;
-  Py_ssize_t __pyx_t_5;
+  Py_ssize_t __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  uint8_t *__pyx_t_4;
+  uint8_t *__pyx_t_5;
+  uint8_t *__pyx_t_6;
+  uint8_t const *__pyx_t_7;
+  uint8_t const *__pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("signature_sign", 1);
+  __Pyx_RefNannySetupContext("signature_sign", 0);
+  __Pyx_INCREF(__pyx_v_secret_key);
 
-  /* "monocypher.pyx":400
+  /* "monocypher.pyx":406
  *     https://pynacl.readthedocs.io/en/stable/signing/.
  *     """
+ *     if len(secret_key) == 32:             # <<<<<<<<<<<<<<
+ *         secret = bytes(64)
+ *         public = bytes(32)
+ */
+  __pyx_t_1 = __Pyx_PyBytes_GET_SIZE(__pyx_v_secret_key); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_t_1 == 32);
+  if (__pyx_t_2) {
+
+    /* "monocypher.pyx":407
+ *     """
+ *     if len(secret_key) == 32:
+ *         secret = bytes(64)             # <<<<<<<<<<<<<<
+ *         public = bytes(32)
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ */
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_v_secret = ((PyObject*)__pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "monocypher.pyx":408
+ *     if len(secret_key) == 32:
+ *         secret = bytes(64)
+ *         public = bytes(32)             # <<<<<<<<<<<<<<
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ *         secret_key = secret
+ */
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_v_public = ((PyObject*)__pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "monocypher.pyx":409
+ *         secret = bytes(64)
+ *         public = bytes(32)
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))             # <<<<<<<<<<<<<<
+ *         secret_key = secret
+ *     elif len(secret_key) != 64:
+ */
+    __pyx_t_4 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_secret_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_t_3); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 409, __pyx_L1_error)
+    crypto_eddsa_key_pair(__pyx_t_4, __pyx_t_5, __pyx_t_6);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "monocypher.pyx":410
+ *         public = bytes(32)
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ *         secret_key = secret             # <<<<<<<<<<<<<<
+ *     elif len(secret_key) != 64:
+ *         raise ValueError('invalid secret key length')
+ */
+    __Pyx_INCREF(__pyx_v_secret);
+    __Pyx_DECREF_SET(__pyx_v_secret_key, __pyx_v_secret);
+
+    /* "monocypher.pyx":406
+ *     https://pynacl.readthedocs.io/en/stable/signing/.
+ *     """
+ *     if len(secret_key) == 32:             # <<<<<<<<<<<<<<
+ *         secret = bytes(64)
+ *         public = bytes(32)
+ */
+    goto __pyx_L3;
+  }
+
+  /* "monocypher.pyx":411
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ *         secret_key = secret
+ *     elif len(secret_key) != 64:             # <<<<<<<<<<<<<<
+ *         raise ValueError('invalid secret key length')
+ *     sig = bytes(64)
+ */
+  __pyx_t_1 = __Pyx_PyBytes_GET_SIZE(__pyx_v_secret_key); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_t_1 != 64);
+  if (unlikely(__pyx_t_2)) {
+
+    /* "monocypher.pyx":412
+ *         secret_key = secret
+ *     elif len(secret_key) != 64:
+ *         raise ValueError('invalid secret key length')             # <<<<<<<<<<<<<<
+ *     sig = bytes(64)
+ *     crypto_eddsa_sign(sig, secret_key, message, len(message))
+ */
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __PYX_ERR(0, 412, __pyx_L1_error)
+
+    /* "monocypher.pyx":411
+ *         crypto_eddsa_key_pair(secret, public, bytes(secret_key))
+ *         secret_key = secret
+ *     elif len(secret_key) != 64:             # <<<<<<<<<<<<<<
+ *         raise ValueError('invalid secret key length')
+ *     sig = bytes(64)
+ */
+  }
+  __pyx_L3:;
+
+  /* "monocypher.pyx":413
+ *     elif len(secret_key) != 64:
+ *         raise ValueError('invalid secret key length')
  *     sig = bytes(64)             # <<<<<<<<<<<<<<
  *     crypto_eddsa_sign(sig, secret_key, message, len(message))
  *     return sig
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_sig = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_v_sig = ((PyObject*)__pyx_t_3);
+  __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":401
- *     """
+  /* "monocypher.pyx":414
+ *         raise ValueError('invalid secret key length')
  *     sig = bytes(64)
  *     crypto_eddsa_sign(sig, secret_key, message, len(message))             # <<<<<<<<<<<<<<
  *     return sig
  * 
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_sig); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyBytes_AsUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyBytes_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_message); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 401, __pyx_L1_error)
-  crypto_eddsa_sign(__pyx_t_2, __pyx_t_3, __pyx_t_4, __pyx_t_5);
+  __pyx_t_6 = __Pyx_PyBytes_AsWritableUString(__pyx_v_sig); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_AsUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyBytes_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_GET_SIZE(__pyx_v_message); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 414, __pyx_L1_error)
+  crypto_eddsa_sign(__pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_1);
 
-  /* "monocypher.pyx":402
+  /* "monocypher.pyx":415
  *     sig = bytes(64)
  *     crypto_eddsa_sign(sig, secret_key, message, len(message))
  *     return sig             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_sig);
   __pyx_r = __pyx_v_sig;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":390
+  /* "monocypher.pyx":396
  * 
  * 
  * def signature_sign(secret_key: bytes, message: bytes) -> bytes:             # <<<<<<<<<<<<<<
- *     """Cryptographically sign a messge.
+ *     """Cryptographically sign a message.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("monocypher.signature_sign", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_secret);
+  __Pyx_XDECREF(__pyx_v_public);
   __Pyx_XDECREF(__pyx_v_sig);
+  __Pyx_XDECREF(__pyx_v_secret_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":405
+/* "monocypher.pyx":418
  * 
  * 
  * def signature_check(signature, public_key, message) -> bool:             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
 
@@ -8184,55 +8449,55 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_signature)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 405, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_public_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 405, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, 1); __PYX_ERR(0, 405, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, 1); __PYX_ERR(0, 418, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 405, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, 2); __PYX_ERR(0, 405, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, 2); __PYX_ERR(0, 418, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "signature_check") < 0)) __PYX_ERR(0, 405, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "signature_check") < 0)) __PYX_ERR(0, 418, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_signature = values[0];
     __pyx_v_public_key = values[1];
     __pyx_v_message = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 405, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 418, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -8264,33 +8529,33 @@
   Py_ssize_t __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signature_check", 1);
 
-  /* "monocypher.pyx":415
+  /* "monocypher.pyx":428
  *         fails verification.
  *     """
  *     return 0 == crypto_eddsa_check(signature, public_key, message, len(message))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_AsUString(__pyx_v_signature); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_AsUString(__pyx_v_public_key); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
-  __pyx_t_4 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 415, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyBool_FromLong((0 == crypto_eddsa_check(__pyx_t_1, __pyx_t_2, __pyx_t_3, __pyx_t_4))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_AsUString(__pyx_v_signature); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_AsUString(__pyx_v_public_key); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBool_FromLong((0 == crypto_eddsa_check(__pyx_t_1, __pyx_t_2, __pyx_t_3, __pyx_t_4))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":405
+  /* "monocypher.pyx":418
  * 
  * 
  * def signature_check(signature, public_key, message) -> bool:             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
 
@@ -8301,15 +8566,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":418
+/* "monocypher.pyx":431
  * 
  * 
  * def generate_key(length=None, method=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
 
@@ -8367,27 +8632,27 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_length);
           if (value) { values[0] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_method);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "generate_key") < 0)) __PYX_ERR(0, 418, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "generate_key") < 0)) __PYX_ERR(0, 431, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -8396,15 +8661,15 @@
       }
     }
     __pyx_v_length = values[0];
     __pyx_v_method = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("generate_key", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 418, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("generate_key", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 431, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -8441,80 +8706,80 @@
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("generate_key", 0);
   __Pyx_INCREF(__pyx_v_length);
 
-  /* "monocypher.pyx":435
+  /* "monocypher.pyx":448
  *     specific crypto usage.
  *     """
  *     length = 32 if length is None else int(length)             # <<<<<<<<<<<<<<
  *     if method in ['chacha20', None, '', 'default']:
  *         # Do not entirely trust the platform's random number generator
  */
   __pyx_t_2 = (__pyx_v_length == Py_None);
   if (__pyx_t_2) {
     __Pyx_INCREF(__pyx_int_32);
     __pyx_t_1 = __pyx_int_32;
   } else {
-    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 435, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   }
   __Pyx_DECREF_SET(__pyx_v_length, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":436
+  /* "monocypher.pyx":449
  *     """
  *     length = 32 if length is None else int(length)
  *     if method in ['chacha20', None, '', 'default']:             # <<<<<<<<<<<<<<
  *         # Do not entirely trust the platform's random number generator
  *         key = secrets.token_bytes(32)
  */
   __Pyx_INCREF(__pyx_v_method);
   __pyx_t_1 = __pyx_v_method;
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_chacha20, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_chacha20, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 449, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, Py_None, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, Py_None, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (!__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__4, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__4, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 449, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_default, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_default, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 449, __pyx_L1_error)
   __pyx_t_2 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = __pyx_t_2;
   if (__pyx_t_4) {
 
-    /* "monocypher.pyx":438
+    /* "monocypher.pyx":451
  *     if method in ['chacha20', None, '', 'default']:
  *         # Do not entirely trust the platform's random number generator
  *         key = secrets.token_bytes(32)             # <<<<<<<<<<<<<<
  *         nonce = secrets.token_bytes(24)
  *         message = secrets.token_bytes(length)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
@@ -8527,31 +8792,31 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_int_32};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 438, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 451, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_v_key = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":439
+    /* "monocypher.pyx":452
  *         # Do not entirely trust the platform's random number generator
  *         key = secrets.token_bytes(32)
  *         nonce = secrets.token_bytes(24)             # <<<<<<<<<<<<<<
  *         message = secrets.token_bytes(length)
  *         key = chacha20(key, nonce, message)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_secrets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_secrets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8564,31 +8829,31 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_int_24};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 452, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_v_nonce = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":440
+    /* "monocypher.pyx":453
  *         key = secrets.token_bytes(32)
  *         nonce = secrets.token_bytes(24)
  *         message = secrets.token_bytes(length)             # <<<<<<<<<<<<<<
  *         key = chacha20(key, nonce, message)
  *     elif method in ['os', 'secrets']:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 440, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
@@ -8601,29 +8866,29 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_length};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 453, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_v_message = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":441
+    /* "monocypher.pyx":454
  *         nonce = secrets.token_bytes(24)
  *         message = secrets.token_bytes(length)
  *         key = chacha20(key, nonce, message)             # <<<<<<<<<<<<<<
  *     elif method in ['os', 'secrets']:
  *         key = secrets.token_bytes(length)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_chacha20); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_chacha20); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 454, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_3 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_3)) {
@@ -8635,63 +8900,63 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_v_key, __pyx_v_nonce, __pyx_v_message};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 3+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 441, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_key, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":436
+    /* "monocypher.pyx":449
  *     """
  *     length = 32 if length is None else int(length)
  *     if method in ['chacha20', None, '', 'default']:             # <<<<<<<<<<<<<<
  *         # Do not entirely trust the platform's random number generator
  *         key = secrets.token_bytes(32)
  */
     goto __pyx_L3;
   }
 
-  /* "monocypher.pyx":442
+  /* "monocypher.pyx":455
  *         message = secrets.token_bytes(length)
  *         key = chacha20(key, nonce, message)
  *     elif method in ['os', 'secrets']:             # <<<<<<<<<<<<<<
  *         key = secrets.token_bytes(length)
  *     else:
  */
   __Pyx_INCREF(__pyx_v_method);
   __pyx_t_1 = __pyx_v_method;
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_os, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_os, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 455, __pyx_L1_error)
   if (!__pyx_t_2) {
   } else {
     __pyx_t_4 = __pyx_t_2;
     goto __pyx_L8_bool_binop_done;
   }
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_secrets, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_secrets, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 455, __pyx_L1_error)
   __pyx_t_4 = __pyx_t_2;
   __pyx_L8_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_2 = __pyx_t_4;
   if (likely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":443
+    /* "monocypher.pyx":456
  *         key = chacha20(key, nonce, message)
  *     elif method in ['os', 'secrets']:
  *         key = secrets.token_bytes(length)             # <<<<<<<<<<<<<<
  *     else:
  *         raise ValueError('unsupported method: %s' % method)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_secrets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_secrets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 456, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 456, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8704,64 +8969,64 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_v_length};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 456, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_v_key = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":442
+    /* "monocypher.pyx":455
  *         message = secrets.token_bytes(length)
  *         key = chacha20(key, nonce, message)
  *     elif method in ['os', 'secrets']:             # <<<<<<<<<<<<<<
  *         key = secrets.token_bytes(length)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "monocypher.pyx":445
+  /* "monocypher.pyx":458
  *         key = secrets.token_bytes(length)
  *     else:
  *         raise ValueError('unsupported method: %s' % method)             # <<<<<<<<<<<<<<
  *     return key
  * 
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unsupported_method_s, __pyx_v_method); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unsupported_method_s, __pyx_v_method); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 445, __pyx_L1_error)
+    __PYX_ERR(0, 458, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "monocypher.pyx":446
+  /* "monocypher.pyx":459
  *     else:
  *         raise ValueError('unsupported method: %s' % method)
  *     return key             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  if (!(likely(PyBytes_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_key))) __PYX_ERR(0, 446, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_key))) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_INCREF(__pyx_v_key);
   __pyx_r = ((PyObject*)__pyx_v_key);
   goto __pyx_L0;
 
-  /* "monocypher.pyx":418
+  /* "monocypher.pyx":431
  * 
  * 
  * def generate_key(length=None, method=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
 
@@ -8778,15 +9043,15 @@
   __Pyx_XDECREF(__pyx_v_message);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":449
+/* "monocypher.pyx":462
  * 
  * 
  * def generate_signing_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
 
@@ -8820,48 +9085,48 @@
   int __pyx_t_6;
   uint8_t *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("generate_signing_key_pair", 1);
 
-  /* "monocypher.pyx":459
+  /* "monocypher.pyx":472
  *         print(binascii.hexlify(key))
  *     """
  *     secret = bytes(64)             # <<<<<<<<<<<<<<
  *     public = bytes(32)
  *     crypto_eddsa_key_pair(secret, public, generate_key())
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_secret = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":460
+  /* "monocypher.pyx":473
  *     """
  *     secret = bytes(64)
  *     public = bytes(32)             # <<<<<<<<<<<<<<
  *     crypto_eddsa_key_pair(secret, public, generate_key())
  *     return secret, public
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 473, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_public = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":461
+  /* "monocypher.pyx":474
  *     secret = bytes(64)
  *     public = bytes(32)
  *     crypto_eddsa_key_pair(secret, public, generate_key())             # <<<<<<<<<<<<<<
  *     return secret, public
  * 
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_generate_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_generate_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
@@ -8873,43 +9138,43 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_7 = __Pyx_PyObject_AsWritableUString(__pyx_t_1); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsWritableUString(__pyx_t_1); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L1_error)
   crypto_eddsa_key_pair(__pyx_t_2, __pyx_t_3, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":462
+  /* "monocypher.pyx":475
  *     public = bytes(32)
  *     crypto_eddsa_key_pair(secret, public, generate_key())
  *     return secret, public             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_secret);
   __Pyx_GIVEREF(__pyx_v_secret);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret)) __PYX_ERR(0, 462, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret)) __PYX_ERR(0, 475, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_public);
   __Pyx_GIVEREF(__pyx_v_public);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_public)) __PYX_ERR(0, 462, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_public)) __PYX_ERR(0, 475, __pyx_L1_error);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":449
+  /* "monocypher.pyx":462
  * 
  * 
  * def generate_signing_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
 
@@ -8924,15 +9189,15 @@
   __Pyx_XDECREF(__pyx_v_secret);
   __Pyx_XDECREF(__pyx_v_public);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":465
+/* "monocypher.pyx":478
  * 
  * 
  * def generate_key_exchange_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
 
@@ -8963,22 +9228,22 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("generate_key_exchange_key_pair", 1);
 
-  /* "monocypher.pyx":470
+  /* "monocypher.pyx":483
  *     :return: (secret, public)
  *     """
  *     secret = generate_key()             # <<<<<<<<<<<<<<
  *     public = compute_key_exchange_public_key(secret)
  *     return secret, public
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_generate_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_generate_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -8990,29 +9255,29 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 470, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 483, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_secret = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":471
+  /* "monocypher.pyx":484
  *     """
  *     secret = generate_key()
  *     public = compute_key_exchange_public_key(secret)             # <<<<<<<<<<<<<<
  *     return secret, public
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_compute_key_exchange_public_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_compute_key_exchange_public_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -9024,42 +9289,42 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_secret};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 471, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_public = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":472
+  /* "monocypher.pyx":485
  *     secret = generate_key()
  *     public = compute_key_exchange_public_key(secret)
  *     return secret, public             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_secret);
   __Pyx_GIVEREF(__pyx_v_secret);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret)) __PYX_ERR(0, 472, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret)) __PYX_ERR(0, 485, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_public);
   __Pyx_GIVEREF(__pyx_v_public);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_public)) __PYX_ERR(0, 472, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_public)) __PYX_ERR(0, 485, __pyx_L1_error);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":465
+  /* "monocypher.pyx":478
  * 
  * 
  * def generate_key_exchange_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
 
@@ -9074,15 +9339,15 @@
   __Pyx_XDECREF(__pyx_v_secret);
   __Pyx_XDECREF(__pyx_v_public);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":478
+/* "monocypher.pyx":491
  * 
  * 
  * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the point corresponding to a representative.
  * 
  */
 
@@ -9136,45 +9401,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_hidden)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 478, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 491, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_map") < 0)) __PYX_ERR(0, 478, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_map") < 0)) __PYX_ERR(0, 491, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_hidden = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("elligator_map", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 478, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("elligator_map", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 491, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.elligator_map", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_hidden), (&PyBytes_Type), 0, "hidden", 1))) __PYX_ERR(0, 478, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_hidden), (&PyBytes_Type), 0, "hidden", 1))) __PYX_ERR(0, 491, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_28elligator_map(__pyx_self, __pyx_v_hidden);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9201,106 +9466,106 @@
   uint8_t *__pyx_t_7;
   uint8_t const *__pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("elligator_map", 1);
 
-  /* "monocypher.pyx":486
+  /* "monocypher.pyx":499
  *         the two most significant bits are ignored.
  *     """
  *     curve = bytes(32)             # <<<<<<<<<<<<<<
  *     if len(hidden) != 32:
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_curve = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":487
+  /* "monocypher.pyx":500
  *     """
  *     curve = bytes(32)
  *     if len(hidden) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  *     crypto_elligator_map(curve, hidden)
  */
-  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 487, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 500, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 32);
   if (unlikely(__pyx_t_3)) {
 
-    /* "monocypher.pyx":488
+    /* "monocypher.pyx":501
  *     curve = bytes(32)
  *     if len(hidden) != 32:
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')             # <<<<<<<<<<<<<<
  *     crypto_elligator_map(curve, hidden)
  *     return curve
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 501, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_4 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_hidden_length);
     __pyx_t_2 += 22;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_hidden_length);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_hidden_length);
-    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 488, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 501, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 501, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_kp_u_32);
     __pyx_t_2 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_32);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 501, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 501, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 488, __pyx_L1_error)
+    __PYX_ERR(0, 501, __pyx_L1_error)
 
-    /* "monocypher.pyx":487
+    /* "monocypher.pyx":500
  *     """
  *     curve = bytes(32)
  *     if len(hidden) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  *     crypto_elligator_map(curve, hidden)
  */
   }
 
-  /* "monocypher.pyx":489
+  /* "monocypher.pyx":502
  *     if len(hidden) != 32:
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  *     crypto_elligator_map(curve, hidden)             # <<<<<<<<<<<<<<
  *     return curve
  * 
  */
-  __pyx_t_7 = __Pyx_PyBytes_AsWritableUString(__pyx_v_curve); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 489, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyBytes_AsUString(__pyx_v_hidden); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_AsWritableUString(__pyx_v_curve); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyBytes_AsUString(__pyx_v_hidden); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 502, __pyx_L1_error)
   crypto_elligator_map(__pyx_t_7, __pyx_t_8);
 
-  /* "monocypher.pyx":490
+  /* "monocypher.pyx":503
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  *     crypto_elligator_map(curve, hidden)
  *     return curve             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_curve);
   __pyx_r = __pyx_v_curve;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":478
+  /* "monocypher.pyx":491
  * 
  * 
  * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the point corresponding to a representative.
  * 
  */
 
@@ -9313,15 +9578,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_curve);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":493
+/* "monocypher.pyx":506
  * 
  * 
  * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the representative of a point.
  * 
  */
 
@@ -9379,27 +9644,27 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_curve)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 493, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 506, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_tweak);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 493, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 506, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_rev") < 0)) __PYX_ERR(0, 493, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_rev") < 0)) __PYX_ERR(0, 506, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
@@ -9407,29 +9672,29 @@
       }
     }
     __pyx_v_curve = ((PyObject*)values[0]);
     __pyx_v_tweak = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("elligator_rev", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 493, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("elligator_rev", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 506, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.elligator_rev", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_curve), (&PyBytes_Type), 0, "curve", 1))) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_curve), (&PyBytes_Type), 0, "curve", 1))) __PYX_ERR(0, 506, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_30elligator_rev(__pyx_self, __pyx_v_curve, __pyx_v_tweak);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9461,102 +9726,102 @@
   uint8_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("elligator_rev", 0);
   __Pyx_INCREF(__pyx_v_tweak);
 
-  /* "monocypher.pyx":504
+  /* "monocypher.pyx":517
  *         and try again.
  *     """
  *     hidden = bytes(32)             # <<<<<<<<<<<<<<
  *     if len(curve) != 32:
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_hidden = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":505
+  /* "monocypher.pyx":518
  *     """
  *     hidden = bytes(32)
  *     if len(curve) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:
  */
-  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 518, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 32);
   if (unlikely(__pyx_t_3)) {
 
-    /* "monocypher.pyx":506
+    /* "monocypher.pyx":519
  *     hidden = bytes(32)
  *     if len(curve) != 32:
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')             # <<<<<<<<<<<<<<
  *     if tweak is None:
  *         tweak = secrets.randbits(8)
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 519, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_4 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_curve_length);
     __pyx_t_2 += 21;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_curve_length);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_curve_length);
-    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 506, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 506, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 519, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 519, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_kp_u_32);
     __pyx_t_2 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_32);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 506, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 519, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 519, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 506, __pyx_L1_error)
+    __PYX_ERR(0, 519, __pyx_L1_error)
 
-    /* "monocypher.pyx":505
+    /* "monocypher.pyx":518
  *     """
  *     hidden = bytes(32)
  *     if len(curve) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:
  */
   }
 
-  /* "monocypher.pyx":507
+  /* "monocypher.pyx":520
  *     if len(curve) != 32:
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:             # <<<<<<<<<<<<<<
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  */
   __pyx_t_3 = (__pyx_v_tweak == Py_None);
   if (__pyx_t_3) {
 
-    /* "monocypher.pyx":508
+    /* "monocypher.pyx":521
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:
  *         tweak = secrets.randbits(8)             # <<<<<<<<<<<<<<
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_secrets); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 508, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_secrets); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_randbits); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 508, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_randbits); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     __pyx_t_8 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
@@ -9569,87 +9834,87 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_int_8};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 508, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_tweak, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":507
+    /* "monocypher.pyx":520
  *     if len(curve) != 32:
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:             # <<<<<<<<<<<<<<
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  */
   }
 
-  /* "monocypher.pyx":509
+  /* "monocypher.pyx":522
  *     if tweak is None:
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)             # <<<<<<<<<<<<<<
  *     if rv:
  *         raise ValueError('curve point is unsuitable for hiding')
  */
-  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyBytes_AsUString(__pyx_v_curve); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_PyInt_As_uint8_t(__pyx_v_tweak); if (unlikely((__pyx_t_11 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 522, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyBytes_AsUString(__pyx_v_curve); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 522, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_uint8_t(__pyx_v_tweak); if (unlikely((__pyx_t_11 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 522, __pyx_L1_error)
   __pyx_v_rv = crypto_elligator_rev(__pyx_t_9, __pyx_t_10, __pyx_t_11);
 
-  /* "monocypher.pyx":510
+  /* "monocypher.pyx":523
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:             # <<<<<<<<<<<<<<
  *         raise ValueError('curve point is unsuitable for hiding')
  *     return hidden
  */
   __pyx_t_3 = (__pyx_v_rv != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "monocypher.pyx":511
+    /* "monocypher.pyx":524
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:
  *         raise ValueError('curve point is unsuitable for hiding')             # <<<<<<<<<<<<<<
  *     return hidden
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 524, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 511, __pyx_L1_error)
+    __PYX_ERR(0, 524, __pyx_L1_error)
 
-    /* "monocypher.pyx":510
+    /* "monocypher.pyx":523
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:             # <<<<<<<<<<<<<<
  *         raise ValueError('curve point is unsuitable for hiding')
  *     return hidden
  */
   }
 
-  /* "monocypher.pyx":512
+  /* "monocypher.pyx":525
  *     if rv:
  *         raise ValueError('curve point is unsuitable for hiding')
  *     return hidden             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_hidden);
   __pyx_r = __pyx_v_hidden;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":493
+  /* "monocypher.pyx":506
  * 
  * 
  * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the representative of a point.
  * 
  */
 
@@ -9664,15 +9929,15 @@
   __Pyx_XDECREF(__pyx_v_hidden);
   __Pyx_XDECREF(__pyx_v_tweak);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":515
+/* "monocypher.pyx":528
  * 
  * 
  * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a key pair.
  * 
  */
 
@@ -9726,48 +9991,48 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_seed);
           if (value) { values[0] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 515, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 528, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_key_pair") < 0)) __PYX_ERR(0, 515, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_key_pair") < 0)) __PYX_ERR(0, 528, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_seed = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("elligator_key_pair", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 515, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("elligator_key_pair", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 528, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.elligator_key_pair", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seed), (&PyBytes_Type), 1, "seed", 1))) __PYX_ERR(0, 515, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seed), (&PyBytes_Type), 1, "seed", 1))) __PYX_ERR(0, 528, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_32elligator_key_pair(__pyx_self, __pyx_v_seed);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9799,58 +10064,58 @@
   uint8_t *__pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("elligator_key_pair", 0);
   __Pyx_INCREF(__pyx_v_seed);
 
-  /* "monocypher.pyx":525
+  /* "monocypher.pyx":538
  *         * secret_key: The generated 32-byte little endian secret key.
  *     """
  *     hidden = bytes(32)             # <<<<<<<<<<<<<<
  *     secret_key = bytes(32)
  *     if seed is None:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_hidden = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":526
+  /* "monocypher.pyx":539
  *     """
  *     hidden = bytes(32)
  *     secret_key = bytes(32)             # <<<<<<<<<<<<<<
  *     if seed is None:
  *         seed = secrets.token_bytes(32)
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 526, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_secret_key = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":527
+  /* "monocypher.pyx":540
  *     hidden = bytes(32)
  *     secret_key = bytes(32)
  *     if seed is None:             # <<<<<<<<<<<<<<
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:
  */
   __pyx_t_2 = (__pyx_v_seed == ((PyObject*)Py_None));
   if (__pyx_t_2) {
 
-    /* "monocypher.pyx":528
+    /* "monocypher.pyx":541
  *     secret_key = bytes(32)
  *     if seed is None:
  *         seed = secrets.token_bytes(32)             # <<<<<<<<<<<<<<
  *     elif len(seed) != 32:
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 528, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 541, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 528, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 541, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
@@ -9863,131 +10128,131 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_int_32};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 528, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 541, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_1))) __PYX_ERR(0, 528, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_1))) __PYX_ERR(0, 541, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_seed, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":527
+    /* "monocypher.pyx":540
  *     hidden = bytes(32)
  *     secret_key = bytes(32)
  *     if seed is None:             # <<<<<<<<<<<<<<
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:
  */
     goto __pyx_L3;
   }
 
-  /* "monocypher.pyx":529
+  /* "monocypher.pyx":542
  *     if seed is None:
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  *     crypto_elligator_key_pair(hidden, secret_key, seed)
  */
   if (unlikely(__pyx_v_seed == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 529, __pyx_L1_error)
+    __PYX_ERR(0, 542, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 529, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 542, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_6 != 32);
   if (unlikely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":530
+    /* "monocypher.pyx":543
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')             # <<<<<<<<<<<<<<
  *     crypto_elligator_key_pair(hidden, secret_key, seed)
  *     return hidden, secret_key
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 530, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_seed_length);
     __pyx_t_6 += 20;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_seed_length);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_seed_length);
     if (unlikely(__pyx_v_seed == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 530, __pyx_L1_error)
+      __PYX_ERR(0, 543, __pyx_L1_error)
     }
-    __pyx_t_8 = __Pyx_PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 530, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_8, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 530, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 543, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_8, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_INCREF(__pyx_kp_u_32);
     __pyx_t_6 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_32);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
-    __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 530, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 530, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 530, __pyx_L1_error)
+    __PYX_ERR(0, 543, __pyx_L1_error)
 
-    /* "monocypher.pyx":529
+    /* "monocypher.pyx":542
  *     if seed is None:
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  *     crypto_elligator_key_pair(hidden, secret_key, seed)
  */
   }
   __pyx_L3:;
 
-  /* "monocypher.pyx":531
+  /* "monocypher.pyx":544
  *     elif len(seed) != 32:
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  *     crypto_elligator_key_pair(hidden, secret_key, seed)             # <<<<<<<<<<<<<<
  *     return hidden, secret_key
  */
-  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 544, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 544, __pyx_L1_error)
   if (unlikely(__pyx_v_seed == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 531, __pyx_L1_error)
+    __PYX_ERR(0, 544, __pyx_L1_error)
   }
-  __pyx_t_11 = __Pyx_PyBytes_AsWritableUString(__pyx_v_seed); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyBytes_AsWritableUString(__pyx_v_seed); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 544, __pyx_L1_error)
   crypto_elligator_key_pair(__pyx_t_9, __pyx_t_10, __pyx_t_11);
 
-  /* "monocypher.pyx":532
+  /* "monocypher.pyx":545
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  *     crypto_elligator_key_pair(hidden, secret_key, seed)
  *     return hidden, secret_key             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_hidden);
   __Pyx_GIVEREF(__pyx_v_hidden);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_hidden)) __PYX_ERR(0, 532, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_hidden)) __PYX_ERR(0, 545, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_secret_key);
   __Pyx_GIVEREF(__pyx_v_secret_key);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_secret_key)) __PYX_ERR(0, 532, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_secret_key)) __PYX_ERR(0, 545, __pyx_L1_error);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":515
+  /* "monocypher.pyx":528
  * 
  * 
  * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a key pair.
  * 
  */
 
@@ -10449,54 +10714,55 @@
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_kp_u_16, __pyx_k_16, sizeof(__pyx_k_16), 0, 1, 0, 0},
     {&__pyx_kp_u_24, __pyx_k_24, sizeof(__pyx_k_24), 0, 1, 0, 0},
     {&__pyx_kp_u_32, __pyx_k_32, sizeof(__pyx_k_32), 0, 1, 0, 0},
-    {&__pyx_kp_u_4_0_2_2, __pyx_k_4_0_2_2, sizeof(__pyx_k_4_0_2_2), 0, 1, 0, 0},
+    {&__pyx_kp_u_4_0_2_3, __pyx_k_4_0_2_3, sizeof(__pyx_k_4_0_2_3), 0, 1, 0, 0},
     {&__pyx_kp_u_BSD_2_clause, __pyx_k_BSD_2_clause, sizeof(__pyx_k_BSD_2_clause), 0, 1, 0, 0},
     {&__pyx_n_s_Blake2b, __pyx_k_Blake2b, sizeof(__pyx_k_Blake2b), 0, 0, 1, 1},
     {&__pyx_n_s_Blake2b___reduce_cython, __pyx_k_Blake2b___reduce_cython, sizeof(__pyx_k_Blake2b___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Blake2b___setstate_cython, __pyx_k_Blake2b___setstate_cython, sizeof(__pyx_k_Blake2b___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Blake2b_finalize, __pyx_k_Blake2b_finalize, sizeof(__pyx_k_Blake2b_finalize), 0, 0, 1, 1},
     {&__pyx_n_s_Blake2b_update, __pyx_k_Blake2b_update, sizeof(__pyx_k_Blake2b_update), 0, 0, 1, 1},
     {&__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC, __pyx_k_Copyright_2018_2024_Jetperch_LLC, sizeof(__pyx_k_Copyright_2018_2024_Jetperch_LLC), 0, 1, 0, 0},
+    {&__pyx_n_s_DeprecationWarning, __pyx_k_DeprecationWarning, sizeof(__pyx_k_DeprecationWarning), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti, __pyx_k_IncrementalAuthenticatedEncrypti, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti_2, __pyx_k_IncrementalAuthenticatedEncrypti_2, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti_2), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti_3, __pyx_k_IncrementalAuthenticatedEncrypti_3, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti_3), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti_4, __pyx_k_IncrementalAuthenticatedEncrypti_4, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti_4), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti_5, __pyx_k_IncrementalAuthenticatedEncrypti_5, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti_5), 0, 0, 1, 1},
     {&__pyx_kp_u_Invalid_curve_length, __pyx_k_Invalid_curve_length, sizeof(__pyx_k_Invalid_curve_length), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_hidden_length, __pyx_k_Invalid_hidden_length, sizeof(__pyx_k_Invalid_hidden_length), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_key_length, __pyx_k_Invalid_key_length, sizeof(__pyx_k_Invalid_key_length), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_mac_length, __pyx_k_Invalid_mac_length, sizeof(__pyx_k_Invalid_mac_length), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_nonce_length, __pyx_k_Invalid_nonce_length, sizeof(__pyx_k_Invalid_nonce_length), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_seed_length, __pyx_k_Invalid_seed_length, sizeof(__pyx_k_Invalid_seed_length), 0, 1, 0, 0},
     {&__pyx_kp_u_Jetperch_LLC, __pyx_k_Jetperch_LLC, sizeof(__pyx_k_Jetperch_LLC), 0, 1, 0, 0},
     {&__pyx_kp_s_Pickling_of_struct_members_such, __pyx_k_Pickling_of_struct_members_such, sizeof(__pyx_k_Pickling_of_struct_members_such), 0, 0, 1, 0},
+    {&__pyx_kp_u_Provide_the_full_64_byte_key_fro, __pyx_k_Provide_the_full_64_byte_key_fro, sizeof(__pyx_k_Provide_the_full_64_byte_key_fro), 0, 1, 0, 0},
     {&__pyx_kp_u_Python_ctypes_bindings_to_the_Mo, __pyx_k_Python_ctypes_bindings_to_the_Mo, sizeof(__pyx_k_Python_ctypes_bindings_to_the_Mo), 0, 1, 0, 0},
     {&__pyx_n_s_Pyx_CFunc_f5947c__10monocypher, __pyx_k_Pyx_CFunc_f5947c__10monocypher, sizeof(__pyx_k_Pyx_CFunc_f5947c__10monocypher), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-    {&__pyx_n_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 1},
+    {&__pyx_n_s__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 0, 1, 1},
     {&__pyx_kp_b__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 0, 0, 0},
     {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
-    {&__pyx_n_s__60, __pyx_k__60, sizeof(__pyx_k__60), 0, 0, 1, 1},
+    {&__pyx_n_s__62, __pyx_k__62, sizeof(__pyx_k__62), 0, 0, 1, 1},
     {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
     {&__pyx_n_s_ad, __pyx_k_ad, sizeof(__pyx_k_ad), 0, 0, 1, 1},
     {&__pyx_n_u_ad, __pyx_k_ad, sizeof(__pyx_k_ad), 0, 1, 0, 1},
     {&__pyx_n_s_algorithm, __pyx_k_algorithm, sizeof(__pyx_k_algorithm), 0, 0, 1, 1},
     {&__pyx_n_s_argon2i_32, __pyx_k_argon2i_32, sizeof(__pyx_k_argon2i_32), 0, 0, 1, 1},
     {&__pyx_n_s_associated_data, __pyx_k_associated_data, sizeof(__pyx_k_associated_data), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_author, __pyx_k_author, sizeof(__pyx_k_author), 0, 0, 1, 1},
     {&__pyx_n_s_author_email, __pyx_k_author_email, sizeof(__pyx_k_author_email), 0, 0, 1, 1},
     {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
-    {&__pyx_n_s_binascii, __pyx_k_binascii, sizeof(__pyx_k_binascii), 0, 0, 1, 1},
     {&__pyx_n_s_blake2b, __pyx_k_blake2b, sizeof(__pyx_k_blake2b), 0, 0, 1, 1},
     {&__pyx_n_s_bool, __pyx_k_bool, sizeof(__pyx_k_bool), 0, 0, 1, 1},
     {&__pyx_n_s_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
     {&__pyx_kp_s_c_monocypher_pyx, __pyx_k_c_monocypher_pyx, sizeof(__pyx_k_c_monocypher_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_cfunc_to_py, __pyx_k_cfunc_to_py, sizeof(__pyx_k_cfunc_to_py), 0, 0, 1, 1},
     {&__pyx_n_s_chacha20, __pyx_k_chacha20, sizeof(__pyx_k_chacha20), 0, 0, 1, 1},
     {&__pyx_n_u_chacha20, __pyx_k_chacha20, sizeof(__pyx_k_chacha20), 0, 1, 0, 1},
@@ -10528,14 +10794,15 @@
     {&__pyx_n_s_hash_size, __pyx_k_hash_size, sizeof(__pyx_k_hash_size), 0, 0, 1, 1},
     {&__pyx_n_s_hidden, __pyx_k_hidden, sizeof(__pyx_k_hidden), 0, 0, 1, 1},
     {&__pyx_kp_u_https_github_com_jetperch_pymono, __pyx_k_https_github_com_jetperch_pymono, sizeof(__pyx_k_https_github_com_jetperch_pymono), 0, 1, 0, 0},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_inputs, __pyx_k_inputs, sizeof(__pyx_k_inputs), 0, 0, 1, 1},
     {&__pyx_kp_u_invalid_nonce_length, __pyx_k_invalid_nonce_length, sizeof(__pyx_k_invalid_nonce_length), 0, 1, 0, 0},
+    {&__pyx_kp_u_invalid_secret_key_length, __pyx_k_invalid_secret_key_length, sizeof(__pyx_k_invalid_secret_key_length), 0, 1, 0, 0},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_kp_u_joulescope_dev_jetperch_com, __pyx_k_joulescope_dev_jetperch_com, sizeof(__pyx_k_joulescope_dev_jetperch_com), 0, 1, 0, 0},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
     {&__pyx_n_u_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 1, 0, 1},
     {&__pyx_n_s_key_exchange, __pyx_k_key_exchange, sizeof(__pyx_k_key_exchange), 0, 0, 1, 1},
     {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
@@ -10582,41 +10849,44 @@
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_sig, __pyx_k_sig, sizeof(__pyx_k_sig), 0, 0, 1, 1},
     {&__pyx_n_s_signature, __pyx_k_signature, sizeof(__pyx_k_signature), 0, 0, 1, 1},
     {&__pyx_n_s_signature_check, __pyx_k_signature_check, sizeof(__pyx_k_signature_check), 0, 0, 1, 1},
     {&__pyx_n_s_signature_sign, __pyx_k_signature_sign, sizeof(__pyx_k_signature_sign), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_stacklevel, __pyx_k_stacklevel, sizeof(__pyx_k_stacklevel), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_their_public_key, __pyx_k_their_public_key, sizeof(__pyx_k_their_public_key), 0, 0, 1, 1},
     {&__pyx_n_s_title, __pyx_k_title, sizeof(__pyx_k_title), 0, 0, 1, 1},
     {&__pyx_n_s_token_bytes, __pyx_k_token_bytes, sizeof(__pyx_k_token_bytes), 0, 0, 1, 1},
     {&__pyx_kp_u_too_long, __pyx_k_too_long, sizeof(__pyx_k_too_long), 0, 1, 0, 0},
     {&__pyx_kp_s_tuple_bytes_bytes, __pyx_k_tuple_bytes_bytes, sizeof(__pyx_k_tuple_bytes_bytes), 0, 0, 1, 0},
     {&__pyx_n_s_tweak, __pyx_k_tweak, sizeof(__pyx_k_tweak), 0, 0, 1, 1},
     {&__pyx_n_s_unlock, __pyx_k_unlock, sizeof(__pyx_k_unlock), 0, 0, 1, 1},
     {&__pyx_kp_u_unsupported_method_s, __pyx_k_unsupported_method_s, sizeof(__pyx_k_unsupported_method_s), 0, 1, 0, 0},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
+    {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
     {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
     {&__pyx_n_s_wipe, __pyx_k_wipe, sizeof(__pyx_k_wipe), 0, 0, 1, 1},
     {&__pyx_n_s_work_area, __pyx_k_work_area, sizeof(__pyx_k_work_area), 0, 0, 1, 1},
     {&__pyx_n_s_wrap, __pyx_k_wrap, sizeof(__pyx_k_wrap), 0, 0, 1, 1},
     {&__pyx_n_s_your_secret_key, __pyx_k_your_secret_key, sizeof(__pyx_k_your_secret_key), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 215, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_builtin_DeprecationWarning = __Pyx_GetBuiltinName(__pyx_n_s_DeprecationWarning); if (!__pyx_builtin_DeprecationWarning) __PYX_ERR(0, 386, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -10631,380 +10901,403 @@
  *         return f(a, b)
  */
   __pyx_tuple_ = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
   __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(1, 67, __pyx_L1_error)
 
-  /* "monocypher.pyx":179
+  /* "monocypher.pyx":178
  *         authentication code.  ciphertext is the encrypted message.
  *     """
  *     mac = bytes(16)             # <<<<<<<<<<<<<<
  *     crypto_text = bytes(len(message))
  *     associated_data = b'' if associated_data is None else associated_data
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_int_16); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_int_16); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "monocypher.pyx":273
+  /* "monocypher.pyx":272
  *         pass
  *     else:
  *         raise ValueError('invalid nonce length')             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_invalid_nonce_length); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_invalid_nonce_length); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "monocypher.pyx":281
+  /* "monocypher.pyx":280
  *     if isinstance(msg, str):
  *         msg = msg.encode('utf-8')
  *     hash = bytes(64)             # <<<<<<<<<<<<<<
  *     crypto_blake2b_keyed(hash, len(hash), key, len(key), msg, len(msg))
  *     return hash
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_int_64); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_int_64); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "monocypher.pyx":345
+  /* "monocypher.pyx":344
  *     extras.ad_size = _validate_u32('ad', len(ad))
  * 
  *     hash = bytes(32)             # <<<<<<<<<<<<<<
  *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))
  *     try:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_int_32); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_int_32); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "monocypher.pyx":386
+  /* "monocypher.pyx":385
  *     """
+ *     if len(secret_key) == 32:
+ *         warnings.warn('Provide the full 64-byte key from generate_signing_key_pair()',             # <<<<<<<<<<<<<<
+ *                       DeprecationWarning, stacklevel=2)
+ *         secret = bytes(64)
+ */
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_kp_u_Provide_the_full_64_byte_key_fro, __pyx_builtin_DeprecationWarning); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+
+  /* "monocypher.pyx":392
+ *         secret_key = secret
  *     if len(secret_key) != 64:
  *         raise ValueError('secret key length invalid')             # <<<<<<<<<<<<<<
  *     return secret_key[32:]
  * 
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_secret_key_length_invalid); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 386, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_secret_key_length_invalid); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "monocypher.pyx":511
+  /* "monocypher.pyx":412
+ *         secret_key = secret
+ *     elif len(secret_key) != 64:
+ *         raise ValueError('invalid secret key length')             # <<<<<<<<<<<<<<
+ *     sig = bytes(64)
+ *     crypto_eddsa_sign(sig, secret_key, message, len(message))
+ */
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_invalid_secret_key_length); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+
+  /* "monocypher.pyx":524
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:
  *         raise ValueError('curve point is unsuitable for hiding')             # <<<<<<<<<<<<<<
  *     return hidden
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_curve_point_is_unsuitable_for_hi); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 511, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_curve_point_is_unsuitable_for_hi); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 524, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "monocypher.pyx":156
+  /* "monocypher.pyx":155
  * 
  * 
  * def wipe(data):             # <<<<<<<<<<<<<<
  *     """Wipe a bytes object from memory.
  * 
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_data); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 156, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_wipe, 156, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_n_s_data); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_wipe, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 155, __pyx_L1_error)
 
-  /* "monocypher.pyx":167
+  /* "monocypher.pyx":166
  * 
  * 
  * def lock(key, nonce, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated encryption.
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(6, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_mac, __pyx_n_s_crypto_text); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_lock, 167, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __pyx_tuple__15 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(6, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_mac, __pyx_n_s_crypto_text); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_lock, 166, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "monocypher.pyx":186
+  /* "monocypher.pyx":185
  * 
  * 
  * def unlock(key, nonce, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated decryption.
  * 
  */
-  __pyx_tuple__16 = PyTuple_Pack(7, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_mac, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_plain_text, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 186, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_unlock, 186, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(7, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_mac, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_plain_text, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_unlock, 185, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 185, __pyx_L1_error)
 
-  /* "monocypher.pyx":223
+  /* "monocypher.pyx":222
  *         crypto_aead_init_x(&self._ctx, key, nonce)
  * 
  *     def lock(self, message, associated_data=None):             # <<<<<<<<<<<<<<
  *         """Perform authenticated encryption.
  * 
  */
-  __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_mac, __pyx_n_s_crypto_text); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 223, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_lock, 223, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_mac, __pyx_n_s_crypto_text); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_lock, 222, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 222, __pyx_L1_error)
 
-  /* "monocypher.pyx":238
+  /* "monocypher.pyx":237
  *         return mac, crypto_text
  * 
  *     def unlock(self, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *         """Perform authenticated decryption.
  * 
  */
-  __pyx_tuple__20 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_mac, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_plain_text, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 238, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_unlock, 238, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_mac, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_plain_text, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_unlock, 237, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 237, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  */
-  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 3, __pyx_L1_error)
 
-  /* "monocypher.pyx":258
+  /* "monocypher.pyx":257
  * 
  * 
  * def chacha20(key, nonce, message):             # <<<<<<<<<<<<<<
  *     """Encrypt/Decrypt a message with ChaCha20.
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message, __pyx_n_s_result); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 258, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_chacha20, 258, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(4, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message, __pyx_n_s_result); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 257, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_chacha20, 257, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 257, __pyx_L1_error)
 
-  /* "monocypher.pyx":277
+  /* "monocypher.pyx":276
  * 
  * 
  * def blake2b(msg, key=None):             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     if isinstance(msg, str):
  */
-  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_msg, __pyx_n_s_key, __pyx_n_s_hash); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 277, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_blake2b, 277, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(3, __pyx_n_s_msg, __pyx_n_s_key, __pyx_n_s_hash); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_blake2b, 276, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 276, __pyx_L1_error)
 
-  /* "monocypher.pyx":300
+  /* "monocypher.pyx":299
  *         crypto_blake2b_keyed_init(&self._ctx, self._hash_size, key, len(key))
  * 
  *     def update(self, message):             # <<<<<<<<<<<<<<
  *         """Add new data to the hash.
  * 
  */
-  __pyx_tuple__30 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_message); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 300, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_update, 300, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_message); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_update, 299, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 299, __pyx_L1_error)
 
-  /* "monocypher.pyx":307
+  /* "monocypher.pyx":306
  *         crypto_blake2b_update(&self._ctx, message, len(message))
  * 
  *     def finalize(self):             # <<<<<<<<<<<<<<
  *         """Finalize and return the computed hash.
  * 
  */
-  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_hash); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 307, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_finalize, 307, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_hash); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_finalize, 306, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 306, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  */
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(1, 3, __pyx_L1_error)
 
-  /* "monocypher.pyx":323
+  /* "monocypher.pyx":322
  * 
  * 
  * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
-  __pyx_tuple__36 = PyTuple_Pack(11, __pyx_n_s_nb_blocks, __pyx_n_s_nb_iterations, __pyx_n_s_password, __pyx_n_s_salt, __pyx_n_s_key, __pyx_n_s_ad, __pyx_n_s_config, __pyx_n_s_inputs, __pyx_n_s_extras, __pyx_n_s_hash, __pyx_n_s_work_area); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 323, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_argon2i_32, 323, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 323, __pyx_L1_error)
-  __pyx_tuple__38 = PyTuple_Pack(2, Py_None, Py_None); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(11, __pyx_n_s_nb_blocks, __pyx_n_s_nb_iterations, __pyx_n_s_password, __pyx_n_s_salt, __pyx_n_s_key, __pyx_n_s_ad, __pyx_n_s_config, __pyx_n_s_inputs, __pyx_n_s_extras, __pyx_n_s_hash, __pyx_n_s_work_area); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_argon2i_32, 322, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(2, Py_None, Py_None); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
 
-  /* "monocypher.pyx":355
+  /* "monocypher.pyx":354
  * 
  * 
  * def compute_key_exchange_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
-  __pyx_tuple__39 = PyTuple_Pack(2, __pyx_n_s_secret_key, __pyx_n_s_public_key); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 355, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_key_exchange_public_key, 355, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(2, __pyx_n_s_secret_key, __pyx_n_s_public_key); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_key_exchange_public_key, 354, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 354, __pyx_L1_error)
 
-  /* "monocypher.pyx":366
+  /* "monocypher.pyx":365
  * 
  * 
  * def key_exchange(your_secret_key: bytes, their_public_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
-  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_n_s_your_secret_key, __pyx_n_s_their_public_key, __pyx_n_s_p); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 366, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_key_exchange, 366, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(3, __pyx_n_s_your_secret_key, __pyx_n_s_their_public_key, __pyx_n_s_p); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_key_exchange, 365, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 365, __pyx_L1_error)
 
-  /* "monocypher.pyx":379
+  /* "monocypher.pyx":378
  * 
  * 
  * def compute_signing_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
-  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 379, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_signing_public_key, 379, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_n_s_secret_key, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_signing_public_key, 378, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 378, __pyx_L1_error)
 
-  /* "monocypher.pyx":390
+  /* "monocypher.pyx":396
  * 
  * 
  * def signature_sign(secret_key: bytes, message: bytes) -> bytes:             # <<<<<<<<<<<<<<
- *     """Cryptographically sign a messge.
+ *     """Cryptographically sign a message.
  * 
  */
-  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_n_s_secret_key, __pyx_n_s_message, __pyx_n_s_sig); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 390, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_sign, 390, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(5, __pyx_n_s_secret_key, __pyx_n_s_message, __pyx_n_s_secret, __pyx_n_s_public, __pyx_n_s_sig); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__47);
+  __Pyx_GIVEREF(__pyx_tuple__47);
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_sign, 396, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 396, __pyx_L1_error)
 
-  /* "monocypher.pyx":405
+  /* "monocypher.pyx":418
  * 
  * 
  * def signature_check(signature, public_key, message) -> bool:             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
-  __pyx_tuple__47 = PyTuple_Pack(3, __pyx_n_s_signature, __pyx_n_s_public_key, __pyx_n_s_message); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 405, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__47);
-  __Pyx_GIVEREF(__pyx_tuple__47);
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_check, 405, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_tuple__49 = PyTuple_Pack(3, __pyx_n_s_signature, __pyx_n_s_public_key, __pyx_n_s_message); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__49);
+  __Pyx_GIVEREF(__pyx_tuple__49);
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_check, 418, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 418, __pyx_L1_error)
 
-  /* "monocypher.pyx":418
+  /* "monocypher.pyx":431
  * 
  * 
  * def generate_key(length=None, method=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
-  __pyx_tuple__49 = PyTuple_Pack(5, __pyx_n_s_length, __pyx_n_s_method, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 418, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__49);
-  __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key, 418, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_tuple__51 = PyTuple_Pack(5, __pyx_n_s_length, __pyx_n_s_method, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 431, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__51);
+  __Pyx_GIVEREF(__pyx_tuple__51);
+  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key, 431, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 431, __pyx_L1_error)
 
-  /* "monocypher.pyx":449
+  /* "monocypher.pyx":462
  * 
  * 
  * def generate_signing_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
-  __pyx_tuple__51 = PyTuple_Pack(2, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 449, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__51);
-  __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_signing_key_pair, 449, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_tuple__53 = PyTuple_Pack(2, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 462, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__53);
+  __Pyx_GIVEREF(__pyx_tuple__53);
+  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_signing_key_pair, 462, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 462, __pyx_L1_error)
 
-  /* "monocypher.pyx":465
+  /* "monocypher.pyx":478
  * 
  * 
  * def generate_key_exchange_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
-  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key_exchange_key_pair, 465, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key_exchange_key_pair, 478, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 478, __pyx_L1_error)
 
-  /* "monocypher.pyx":478
+  /* "monocypher.pyx":491
  * 
  * 
  * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the point corresponding to a representative.
  * 
  */
-  __pyx_tuple__54 = PyTuple_Pack(2, __pyx_n_s_hidden, __pyx_n_s_curve); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 478, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__54);
-  __Pyx_GIVEREF(__pyx_tuple__54);
-  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_map, 478, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(2, __pyx_n_s_hidden, __pyx_n_s_curve); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_map, 491, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 491, __pyx_L1_error)
 
-  /* "monocypher.pyx":493
+  /* "monocypher.pyx":506
  * 
  * 
  * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the representative of a point.
  * 
  */
-  __pyx_tuple__56 = PyTuple_Pack(4, __pyx_n_s_curve, __pyx_n_s_tweak, __pyx_n_s_hidden, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 493, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__56);
-  __Pyx_GIVEREF(__pyx_tuple__56);
-  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_rev, 493, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(4, __pyx_n_s_curve, __pyx_n_s_tweak, __pyx_n_s_hidden, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__58);
+  __Pyx_GIVEREF(__pyx_tuple__58);
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_rev, 506, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 506, __pyx_L1_error)
 
-  /* "monocypher.pyx":515
+  /* "monocypher.pyx":528
  * 
  * 
  * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a key pair.
  * 
  */
-  __pyx_tuple__58 = PyTuple_Pack(3, __pyx_n_s_seed, __pyx_n_s_hidden, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 515, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__58);
-  __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_key_pair, 515, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(3, __pyx_n_s_seed, __pyx_n_s_hidden, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__60);
+  __Pyx_GIVEREF(__pyx_tuple__60);
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_key_pair, 528, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_24 = PyInt_FromLong(24); if (unlikely(!__pyx_int_24)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_32 = PyInt_FromLong(32); if (unlikely(!__pyx_int_32)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4294967295 = PyInt_FromString((char *)"4294967295", 0, 0); if (unlikely(!__pyx_int_4294967295)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -11054,58 +11347,58 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10monocypher_IncrementalAuthenticatedEncryption_spec, NULL); if (unlikely(!__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption)) __PYX_ERR(0, 206, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10monocypher_IncrementalAuthenticatedEncryption_spec, __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10monocypher_IncrementalAuthenticatedEncryption_spec, NULL); if (unlikely(!__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption)) __PYX_ERR(0, 205, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10monocypher_IncrementalAuthenticatedEncryption_spec, __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
   #else
   __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption = &__pyx_type_10monocypher_IncrementalAuthenticatedEncryption;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption->tp_dictoffset && __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_IncrementalAuthenticatedEncrypti, (PyObject *) __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_IncrementalAuthenticatedEncrypti, (PyObject *) __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_10monocypher_Blake2b = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10monocypher_Blake2b_spec, NULL); if (unlikely(!__pyx_ptype_10monocypher_Blake2b)) __PYX_ERR(0, 286, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10monocypher_Blake2b_spec, __pyx_ptype_10monocypher_Blake2b) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_ptype_10monocypher_Blake2b = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10monocypher_Blake2b_spec, NULL); if (unlikely(!__pyx_ptype_10monocypher_Blake2b)) __PYX_ERR(0, 285, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10monocypher_Blake2b_spec, __pyx_ptype_10monocypher_Blake2b) < 0) __PYX_ERR(0, 285, __pyx_L1_error)
   #else
   __pyx_ptype_10monocypher_Blake2b = &__pyx_type_10monocypher_Blake2b;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_10monocypher_Blake2b) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_10monocypher_Blake2b) < 0) __PYX_ERR(0, 285, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_10monocypher_Blake2b->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_10monocypher_Blake2b->tp_dictoffset && __pyx_ptype_10monocypher_Blake2b->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_10monocypher_Blake2b->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Blake2b, (PyObject *) __pyx_ptype_10monocypher_Blake2b) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Blake2b, (PyObject *) __pyx_ptype_10monocypher_Blake2b) < 0) __PYX_ERR(0, 285, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_10monocypher_Blake2b) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_10monocypher_Blake2b) < 0) __PYX_ERR(0, 285, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
   __pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b_spec, NULL); if (unlikely(!__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b)) __PYX_ERR(1, 66, __pyx_L1_error)
   if (__Pyx_fix_up_extension_type_from_spec(&__pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b_spec, __pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b) < 0) __PYX_ERR(1, 66, __pyx_L1_error)
   #else
   __pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b = &__pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b;
   #endif
@@ -11431,493 +11724,481 @@
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "monocypher.pyx":10
  * from libc.stdint cimport uint8_t, uint32_t, uint64_t
  * from libc.stdlib cimport malloc, free
- * import binascii             # <<<<<<<<<<<<<<
- * import secrets
- * import warnings
- */
-  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_binascii, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_binascii, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "monocypher.pyx":11
- * from libc.stdlib cimport malloc, free
- * import binascii
  * import secrets             # <<<<<<<<<<<<<<
  * import warnings
  * 
  */
-  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_secrets, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_secrets, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_secrets, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_secrets, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":12
- * import binascii
+  /* "monocypher.pyx":11
+ * from libc.stdlib cimport malloc, free
  * import secrets
  * import warnings             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_warnings, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_warnings, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_2) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":16
+  /* "monocypher.pyx":15
  * 
  * # also edit setup.py
- * __version__ = '4.0.2.2'   # also change setup.py             # <<<<<<<<<<<<<<
+ * __version__ = '4.0.2.3'   # also change setup.py             # <<<<<<<<<<<<<<
  * __title__ = 'pymonocypher'
  * __description__ = 'Python ctypes bindings to the Monocypher library'
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_4_0_2_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_4_0_2_3) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
 
-  /* "monocypher.pyx":17
+  /* "monocypher.pyx":16
  * # also edit setup.py
- * __version__ = '4.0.2.2'   # also change setup.py
+ * __version__ = '4.0.2.3'   # also change setup.py
  * __title__ = 'pymonocypher'             # <<<<<<<<<<<<<<
  * __description__ = 'Python ctypes bindings to the Monocypher library'
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_title, __pyx_n_u_pymonocypher) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_title, __pyx_n_u_pymonocypher) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
 
-  /* "monocypher.pyx":18
- * __version__ = '4.0.2.2'   # also change setup.py
+  /* "monocypher.pyx":17
+ * __version__ = '4.0.2.3'   # also change setup.py
  * __title__ = 'pymonocypher'
  * __description__ = 'Python ctypes bindings to the Monocypher library'             # <<<<<<<<<<<<<<
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  * __author__ = 'Jetperch LLC'
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_description, __pyx_kp_u_Python_ctypes_bindings_to_the_Mo) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_description, __pyx_kp_u_Python_ctypes_bindings_to_the_Mo) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
 
-  /* "monocypher.pyx":19
+  /* "monocypher.pyx":18
  * __title__ = 'pymonocypher'
  * __description__ = 'Python ctypes bindings to the Monocypher library'
  * __url__ = 'https://github.com/jetperch/pymonocypher'             # <<<<<<<<<<<<<<
  * __author__ = 'Jetperch LLC'
  * __author_email__ = 'joulescope-dev@jetperch.com'
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_url, __pyx_kp_u_https_github_com_jetperch_pymono) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_url, __pyx_kp_u_https_github_com_jetperch_pymono) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
 
-  /* "monocypher.pyx":20
+  /* "monocypher.pyx":19
  * __description__ = 'Python ctypes bindings to the Monocypher library'
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  * __author__ = 'Jetperch LLC'             # <<<<<<<<<<<<<<
  * __author_email__ = 'joulescope-dev@jetperch.com'
  * __license__ = 'BSD 2-clause'
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_author, __pyx_kp_u_Jetperch_LLC) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_author, __pyx_kp_u_Jetperch_LLC) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
 
-  /* "monocypher.pyx":21
+  /* "monocypher.pyx":20
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  * __author__ = 'Jetperch LLC'
  * __author_email__ = 'joulescope-dev@jetperch.com'             # <<<<<<<<<<<<<<
  * __license__ = 'BSD 2-clause'
  * __copyright__ = 'Copyright 2018-2024 Jetperch LLC'
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_author_email, __pyx_kp_u_joulescope_dev_jetperch_com) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_author_email, __pyx_kp_u_joulescope_dev_jetperch_com) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
 
-  /* "monocypher.pyx":22
+  /* "monocypher.pyx":21
  * __author__ = 'Jetperch LLC'
  * __author_email__ = 'joulescope-dev@jetperch.com'
  * __license__ = 'BSD 2-clause'             # <<<<<<<<<<<<<<
  * __copyright__ = 'Copyright 2018-2024 Jetperch LLC'
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_license, __pyx_kp_u_BSD_2_clause) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_license, __pyx_kp_u_BSD_2_clause) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
 
-  /* "monocypher.pyx":23
+  /* "monocypher.pyx":22
  * __author_email__ = 'joulescope-dev@jetperch.com'
  * __license__ = 'BSD 2-clause'
  * __copyright__ = 'Copyright 2018-2024 Jetperch LLC'             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_copyright, __pyx_kp_u_Copyright_2018_2024_Jetperch_LLC) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_copyright, __pyx_kp_u_Copyright_2018_2024_Jetperch_LLC) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
 
-  /* "monocypher.pyx":156
+  /* "monocypher.pyx":155
  * 
  * 
  * def wipe(data):             # <<<<<<<<<<<<<<
  *     """Wipe a bytes object from memory.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_1wipe, 0, __pyx_n_s_wipe, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_1wipe, 0, __pyx_n_s_wipe, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_wipe, __pyx_t_2) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_wipe, __pyx_t_2) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":167
+  /* "monocypher.pyx":166
  * 
  * 
  * def lock(key, nonce, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated encryption.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_3lock, 0, __pyx_n_s_lock, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_3lock, 0, __pyx_n_s_lock, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__15);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lock, __pyx_t_2) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__17);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lock, __pyx_t_2) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":186
+  /* "monocypher.pyx":185
  * 
  * 
  * def unlock(key, nonce, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated decryption.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_5unlock, 0, __pyx_n_s_unlock, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_5unlock, 0, __pyx_n_s_unlock, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__15);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_unlock, __pyx_t_2) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__17);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_unlock, __pyx_t_2) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":223
+  /* "monocypher.pyx":222
  *         crypto_aead_init_x(&self._ctx, key, nonce)
  * 
  *     def lock(self, message, associated_data=None):             # <<<<<<<<<<<<<<
  *         """Perform authenticated encryption.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_34IncrementalAuthenticatedEncryption_3lock, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IncrementalAuthenticatedEncrypti_2, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_34IncrementalAuthenticatedEncryption_3lock, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IncrementalAuthenticatedEncrypti_2, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__15);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption, __pyx_n_s_lock, __pyx_t_2) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__17);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption, __pyx_n_s_lock, __pyx_t_2) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption);
 
-  /* "monocypher.pyx":238
+  /* "monocypher.pyx":237
  *         return mac, crypto_text
  * 
  *     def unlock(self, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *         """Perform authenticated decryption.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_34IncrementalAuthenticatedEncryption_5unlock, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IncrementalAuthenticatedEncrypti_3, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_34IncrementalAuthenticatedEncryption_5unlock, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IncrementalAuthenticatedEncrypti_3, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__15);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption, __pyx_n_s_unlock, __pyx_t_2) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__17);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption, __pyx_n_s_unlock, __pyx_t_2) < 0) __PYX_ERR(0, 237, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_34IncrementalAuthenticatedEncryption_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IncrementalAuthenticatedEncrypti_4, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_34IncrementalAuthenticatedEncryption_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IncrementalAuthenticatedEncrypti_4, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_34IncrementalAuthenticatedEncryption_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IncrementalAuthenticatedEncrypti_5, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_34IncrementalAuthenticatedEncryption_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IncrementalAuthenticatedEncrypti_5, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":258
+  /* "monocypher.pyx":257
  * 
  * 
  * def chacha20(key, nonce, message):             # <<<<<<<<<<<<<<
  *     """Encrypt/Decrypt a message with ChaCha20.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7chacha20, 0, __pyx_n_s_chacha20, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7chacha20, 0, __pyx_n_s_chacha20, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_chacha20, __pyx_t_2) < 0) __PYX_ERR(0, 258, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_chacha20, __pyx_t_2) < 0) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":277
+  /* "monocypher.pyx":276
  * 
  * 
  * def blake2b(msg, key=None):             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     if isinstance(msg, str):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_9blake2b, 0, __pyx_n_s_blake2b, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_9blake2b, 0, __pyx_n_s_blake2b, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__15);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_blake2b, __pyx_t_2) < 0) __PYX_ERR(0, 277, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__17);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_blake2b, __pyx_t_2) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":300
+  /* "monocypher.pyx":299
  *         crypto_blake2b_keyed_init(&self._ctx, self._hash_size, key, len(key))
  * 
  *     def update(self, message):             # <<<<<<<<<<<<<<
  *         """Add new data to the hash.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_3update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b_update, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_3update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b_update, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_10monocypher_Blake2b, __pyx_n_s_update, __pyx_t_2) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_10monocypher_Blake2b, __pyx_n_s_update, __pyx_t_2) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_10monocypher_Blake2b);
 
-  /* "monocypher.pyx":307
+  /* "monocypher.pyx":306
  *         crypto_blake2b_update(&self._ctx, message, len(message))
  * 
  *     def finalize(self):             # <<<<<<<<<<<<<<
  *         """Finalize and return the computed hash.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_5finalize, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b_finalize, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_5finalize, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b_finalize, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_10monocypher_Blake2b, __pyx_n_s_finalize, __pyx_t_2) < 0) __PYX_ERR(0, 307, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_10monocypher_Blake2b, __pyx_n_s_finalize, __pyx_t_2) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_10monocypher_Blake2b);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b___reduce_cython, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b___reduce_cython, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b___setstate_cython, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b___setstate_cython, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":323
+  /* "monocypher.pyx":322
  * 
  * 
  * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_11argon2i_32, 0, __pyx_n_s_argon2i_32, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_11argon2i_32, 0, __pyx_n_s_argon2i_32, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__38);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__40);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_argon2i_32, __pyx_t_3) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_argon2i_32, __pyx_t_3) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":355
+  /* "monocypher.pyx":354
  * 
  * 
  * def compute_key_exchange_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 355, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 355, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_13compute_key_exchange_public_key, 0, __pyx_n_s_compute_key_exchange_public_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 354, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_13compute_key_exchange_public_key, 0, __pyx_n_s_compute_key_exchange_public_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_key_exchange_public_key, __pyx_t_2) < 0) __PYX_ERR(0, 355, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_key_exchange_public_key, __pyx_t_2) < 0) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":366
+  /* "monocypher.pyx":365
  * 
  * 
  * def key_exchange(your_secret_key: bytes, their_public_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_your_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_their_public_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_15key_exchange, 0, __pyx_n_s_key_exchange, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_your_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 365, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_their_public_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 365, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_15key_exchange, 0, __pyx_n_s_key_exchange, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_key_exchange, __pyx_t_3) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_key_exchange, __pyx_t_3) < 0) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":379
+  /* "monocypher.pyx":378
  * 
  * 
  * def compute_signing_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_17compute_signing_public_key, 0, __pyx_n_s_compute_signing_public_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_17compute_signing_public_key, 0, __pyx_n_s_compute_signing_public_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_signing_public_key, __pyx_t_2) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_signing_public_key, __pyx_t_2) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":390
+  /* "monocypher.pyx":396
  * 
  * 
  * def signature_sign(secret_key: bytes, message: bytes) -> bytes:             # <<<<<<<<<<<<<<
- *     """Cryptographically sign a messge.
+ *     """Cryptographically sign a message.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_message, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_19signature_sign, 0, __pyx_n_s_signature_sign, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_message, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_19signature_sign, 0, __pyx_n_s_signature_sign, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_signature_sign, __pyx_t_3) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_signature_sign, __pyx_t_3) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":405
+  /* "monocypher.pyx":418
  * 
  * 
  * def signature_check(signature, public_key, message) -> bool:             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(0, 405, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_21signature_check, 0, __pyx_n_s_signature_check, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_21signature_check, 0, __pyx_n_s_signature_check, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_signature_check, __pyx_t_2) < 0) __PYX_ERR(0, 405, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_signature_check, __pyx_t_2) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":418
+  /* "monocypher.pyx":431
  * 
  * 
  * def generate_key(length=None, method=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_23generate_key, 0, __pyx_n_s_generate_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_23generate_key, 0, __pyx_n_s_generate_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__38);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__40);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key, __pyx_t_3) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key, __pyx_t_3) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":449
+  /* "monocypher.pyx":462
  * 
  * 
  * def generate_signing_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_25generate_signing_key_pair, 0, __pyx_n_s_generate_signing_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 449, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_25generate_signing_key_pair, 0, __pyx_n_s_generate_signing_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_signing_key_pair, __pyx_t_2) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_signing_key_pair, __pyx_t_2) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":465
+  /* "monocypher.pyx":478
  * 
  * 
  * def generate_key_exchange_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 465, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_27generate_key_exchange_key_pair, 0, __pyx_n_s_generate_key_exchange_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_27generate_key_exchange_key_pair, 0, __pyx_n_s_generate_key_exchange_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key_exchange_key_pair, __pyx_t_3) < 0) __PYX_ERR(0, 465, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key_exchange_key_pair, __pyx_t_3) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":478
+  /* "monocypher.pyx":491
  * 
  * 
  * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the point corresponding to a representative.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_hidden, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_29elligator_map, 0, __pyx_n_s_elligator_map, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 478, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_hidden, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 491, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_29elligator_map, 0, __pyx_n_s_elligator_map, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_map, __pyx_t_2) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_map, __pyx_t_2) < 0) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":493
+  /* "monocypher.pyx":506
  * 
  * 
  * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the representative of a point.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_curve, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_31elligator_rev, 0, __pyx_n_s_elligator_rev, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_curve, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_31elligator_rev, 0, __pyx_n_s_elligator_rev, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__15);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__17);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_rev, __pyx_t_3) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_rev, __pyx_t_3) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":515
+  /* "monocypher.pyx":528
  * 
  * 
  * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a key pair.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_seed, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_33elligator_key_pair, 0, __pyx_n_s_elligator_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_seed, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_33elligator_key_pair, 0, __pyx_n_s_elligator_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__15);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__17);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_key_pair, __pyx_t_2) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_key_pair, __pyx_t_2) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "monocypher.pyx":1
  * """             # <<<<<<<<<<<<<<
  * Monocypher library Python bindings.
  * 
  */
@@ -11925,26 +12206,26 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
   {
     PyObject* wrapped = __Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b(crypto_verify16);
-    if (unlikely(!wrapped)) __PYX_ERR(0, 28, __pyx_L1_error)
-    if (PyObject_SetAttrString(__pyx_m, "crypto_verify16", wrapped) < 0) __PYX_ERR(0, 28, __pyx_L1_error);
+    if (unlikely(!wrapped)) __PYX_ERR(0, 27, __pyx_L1_error)
+    if (PyObject_SetAttrString(__pyx_m, "crypto_verify16", wrapped) < 0) __PYX_ERR(0, 27, __pyx_L1_error);
   }
   {
     PyObject* wrapped = __Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b(crypto_verify32);
-    if (unlikely(!wrapped)) __PYX_ERR(0, 30, __pyx_L1_error)
-    if (PyObject_SetAttrString(__pyx_m, "crypto_verify32", wrapped) < 0) __PYX_ERR(0, 30, __pyx_L1_error);
+    if (unlikely(!wrapped)) __PYX_ERR(0, 29, __pyx_L1_error)
+    if (PyObject_SetAttrString(__pyx_m, "crypto_verify32", wrapped) < 0) __PYX_ERR(0, 29, __pyx_L1_error);
   }
   {
     PyObject* wrapped = __Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b(crypto_verify64);
-    if (unlikely(!wrapped)) __PYX_ERR(0, 32, __pyx_L1_error)
-    if (PyObject_SetAttrString(__pyx_m, "crypto_verify64", wrapped) < 0) __PYX_ERR(0, 32, __pyx_L1_error);
+    if (unlikely(!wrapped)) __PYX_ERR(0, 31, __pyx_L1_error)
+    if (PyObject_SetAttrString(__pyx_m, "crypto_verify64", wrapped) < 0) __PYX_ERR(0, 31, __pyx_L1_error);
   }
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   if (__pyx_m) {
@@ -15513,15 +15794,15 @@
         return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
     }
     return module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__10;
+    PyObject *module, *from_list, *star = __pyx_n_s__12;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -17154,15 +17435,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__60);
+        name = __Pyx_NewRef(__pyx_n_s__62);
     }
     return name;
 }
 #endif
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
```

### Comparing `pymonocypher-4.0.2.2/monocypher.c` & `pymonocypher-4.0.2.3/monocypher.c`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.2/monocypher.h` & `pymonocypher-4.0.2.3/monocypher.h`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.2/pymonocypher.egg-info/PKG-INFO` & `pymonocypher-4.0.2.3/pymonocypher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonocypher
-Version: 4.0.2.2
+Version: 4.0.2.3
 Summary: Python ctypes bindings to the Monocypher library
 Home-page: https://github.com/jetperch/pymonocypher
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: BSD 2-clause
 Project-URL: Bug Reports, https://github.com/jetperch/pymonocypher/issues
 Project-URL: Source, https://github.com/jetperch/pymonocypher/
```

### Comparing `pymonocypher-4.0.2.2/pyproject.toml` & `pymonocypher-4.0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.2/setup.py` & `pymonocypher-4.0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # https://github.com/pypa/sampleproject
 
 
 import setuptools
 import os
 
 MYPATH = os.path.abspath(os.path.dirname(__file__))
-VERSION = '4.0.2.2'  # also change c_monocypher.pyx
+VERSION = '4.0.2.3'  # also change c_monocypher.pyx
 
 
 try:
     from Cython.Build import cythonize
     USE_CYTHON = os.path.isfile(os.path.join(MYPATH, 'c_monocypher.pyx'))
 except ImportError:
     USE_CYTHON = False
```

### Comparing `pymonocypher-4.0.2.2/test/blake2-kat.json` & `pymonocypher-4.0.2.3/test/blake2-kat.json`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.2/test/test_monocypher.py` & `pymonocypher-4.0.2.3/test/test_monocypher.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,20 +104,34 @@
         random = np.random.RandomState(seed=1)
         for i in range(100):
             length = random.randint(1, 4096)
             secret_key, expected_public_key = monocypher.generate_signing_key_pair()
             msg = bytes(random.randint(0, 256, length, dtype=np.uint8))
             public_key = monocypher.compute_signing_public_key(secret_key)
             self.assertEqual(expected_public_key, public_key)
+            public_key = monocypher.compute_signing_public_key(secret_key[:32])
+            self.assertEqual(expected_public_key, public_key)
             sig = monocypher.signature_sign(secret_key, msg)
             self.assertTrue(monocypher.signature_check(sig, public_key, msg))
             self.assertFalse(monocypher.signature_check(sig, public_key, msg + b'0'))
             sig2 = sig[:10] + bytes([(sig[10] + 1) & 0xff]) + sig[11:]
             self.assertFalse(monocypher.signature_check(sig2, public_key, msg))
 
+    def test_sign_secret32_deprecated(self):
+        random = np.random.RandomState(seed=1)
+        for i in range(100):
+            length = random.randint(1, 4096)
+            secret_key, public_key = monocypher.generate_signing_key_pair()
+            msg = bytes(random.randint(0, 256, length, dtype=np.uint8))
+            sig = monocypher.signature_sign(secret_key[:32], msg)
+            self.assertTrue(monocypher.signature_check(sig, public_key, msg))
+            self.assertFalse(monocypher.signature_check(sig, public_key, msg + b'0'))
+            sig2 = sig[:10] + bytes([(sig[10] + 1) & 0xff]) + sig[11:]
+            self.assertFalse(monocypher.signature_check(sig2, public_key, msg))
+
     def test_key_exchange_static(self):
         expect = b'l#\x84\xf2\xc0\xf1:\x8f\xf3\xce\xeeU\x07U@w\x8c\xd9\xf9C\x83\x17\x887\xae$\xf9\xf4\x19\xc1-{'
         your_secret_key = bytes(range(32))
         their_public_key = bytes(range(32, 64))
         shared_key = monocypher.key_exchange(your_secret_key, their_public_key)
         self.assertEqual(expect, shared_key)
 
@@ -128,16 +142,19 @@
         a_shared_secret = monocypher.key_exchange(a_private_secret, b_public_secret)
         self.assertEqual(a_shared_secret, b_shared_secret)
 
     def test_generate_key(self):
         self.assertEqual(32, len(monocypher.generate_key()))
 
     def test_compute_signing_public_key(self):
-        with self.assertRaises(ValueError):
-            monocypher.compute_signing_public_key(monocypher.generate_key())
+        secret, public = monocypher.generate_signing_key_pair()
+        p1 = monocypher.compute_signing_public_key(bytes(secret))
+        self.assertEqual(public, p1)
+        p2 = monocypher.compute_signing_public_key(bytes(secret[:32]))
+        self.assertEqual(public, p2)
 
     def test_elligator(self):
         hidden1, secret = monocypher.elligator_key_pair()
         curve1 = monocypher.elligator_map(hidden1)
         while True:
             try:
                 hidden2 = monocypher.elligator_rev(curve1)
```

