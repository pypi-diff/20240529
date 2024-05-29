# Comparing `tmp/ansar_connect-1.0.2.tar.gz` & `tmp/ansar_connect-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-1.0.2.tar", last modified: Mon May 27 05:44:54 2024, max compression
+gzip compressed data, was "ansar_connect-1.0.3.tar", last modified: Wed May 29 09:03:11 2024, max compression
```

## Comparing `ansar_connect-1.0.2.tar` & `ansar_connect-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:44:54.084343 ansar_connect-1.0.2/
--rw-rw-r--   0 scott     (1000) scott     (1000)      271 2024-05-27 03:58:46.000000 ansar_connect-1.0.2/CHANGES.rst
--rw-rw-r--   0 scott     (1000) scott     (1000)       32 2024-05-27 02:47:17.000000 ansar_connect-1.0.2/COPYRIGHT.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-1.0.2/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)      224 2024-05-27 02:47:17.000000 ansar_connect-1.0.2/MANIFEST.in
--rw-r--r--   0 scott     (1000) scott     (1000)     2407 2024-05-27 05:44:54.084343 ansar_connect-1.0.2/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      854 2024-05-27 03:59:46.000000 ansar_connect-1.0.2/README.rst
--rwxrwxr-x   0 scott     (1000) scott     (1000)     1429 2024-05-27 05:44:38.000000 ansar_connect-1.0.2/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-27 05:44:54.084343 ansar_connect-1.0.2/setup.cfg
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2615 2024-05-27 05:44:19.000000 ansar_connect-1.0.2/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:44:54.080343 ansar_connect-1.0.2/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:44:54.080343 ansar_connect-1.0.2/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:44:54.080343 ansar_connect-1.0.2/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-1.0.2/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-1.0.2/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9946 2024-05-26 20:11:05.000000 ansar_connect-1.0.2/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-1.0.2/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:44:54.084343 ansar_connect-1.0.2/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3003 2024-05-27 05:44:50.000000 ansar_connect-1.0.2/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14103 2024-05-26 20:11:05.000000 ansar_connect-1.0.2/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-1.0.2/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-1.0.2/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-1.0.2/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-1.0.2/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15870 2024-05-26 20:11:05.000000 ansar_connect-1.0.2/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-1.0.2/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23196 2024-05-26 20:11:05.000000 ansar_connect-1.0.2/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-1.0.2/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-26 07:36:57.000000 ansar_connect-1.0.2/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-1.0.2/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-1.0.2/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-1.0.2/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-1.0.2/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-1.0.2/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-1.0.2/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-1.0.2/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-1.0.2/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-27 05:44:54.084343 ansar_connect-1.0.2/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2407 2024-05-27 05:44:54.000000 ansar_connect-1.0.2/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1060 2024-05-27 05:44:54.000000 ansar_connect-1.0.2/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-27 05:44:54.000000 ansar_connect-1.0.2/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-27 05:44:54.000000 ansar_connect-1.0.2/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       47 2024-05-27 05:44:54.000000 ansar_connect-1.0.2/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-27 05:44:54.000000 ansar_connect-1.0.2/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-29 09:03:11.663064 ansar_connect-1.0.3/
+-rw-rw-r--   0 scott     (1000) scott     (1000)      271 2024-05-27 03:58:46.000000 ansar_connect-1.0.3/CHANGES.rst
+-rw-rw-r--   0 scott     (1000) scott     (1000)       32 2024-05-27 02:47:17.000000 ansar_connect-1.0.3/COPYRIGHT.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-1.0.3/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)      224 2024-05-27 02:47:17.000000 ansar_connect-1.0.3/MANIFEST.in
+-rw-r--r--   0 scott     (1000) scott     (1000)     2407 2024-05-29 09:03:11.663064 ansar_connect-1.0.3/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      854 2024-05-27 03:59:46.000000 ansar_connect-1.0.3/README.rst
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     1429 2024-05-27 05:44:38.000000 ansar_connect-1.0.3/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-29 09:03:11.663064 ansar_connect-1.0.3/setup.cfg
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2615 2024-05-27 05:44:19.000000 ansar_connect-1.0.3/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-29 09:03:11.663064 ansar_connect-1.0.3/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-29 09:03:11.663064 ansar_connect-1.0.3/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-29 09:03:11.663064 ansar_connect-1.0.3/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-1.0.3/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-1.0.3/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9946 2024-05-26 20:11:05.000000 ansar_connect-1.0.3/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-1.0.3/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-29 09:03:11.663064 ansar_connect-1.0.3/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3003 2024-05-29 09:03:08.000000 ansar_connect-1.0.3/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14103 2024-05-26 20:11:05.000000 ansar_connect-1.0.3/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-1.0.3/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-1.0.3/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-1.0.3/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-1.0.3/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15870 2024-05-26 20:11:05.000000 ansar_connect-1.0.3/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-1.0.3/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23196 2024-05-26 20:11:05.000000 ansar_connect-1.0.3/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-1.0.3/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-26 07:36:57.000000 ansar_connect-1.0.3/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-1.0.3/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-1.0.3/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-1.0.3/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-1.0.3/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-1.0.3/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-1.0.3/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-1.0.3/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-1.0.3/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-29 09:03:11.663064 ansar_connect-1.0.3/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2407 2024-05-29 09:03:11.000000 ansar_connect-1.0.3/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1060 2024-05-29 09:03:11.000000 ansar_connect-1.0.3/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-29 09:03:11.000000 ansar_connect-1.0.3/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-29 09:03:11.000000 ansar_connect-1.0.3/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       47 2024-05-29 09:03:11.000000 ansar_connect-1.0.3/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-29 09:03:11.000000 ansar_connect-1.0.3/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-1.0.2/LICENSE` & `ansar_connect-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/PKG-INFO` & `ansar_connect-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools and runtime for network messaging
 Author: Scott Woods
 Author-email: Scott Woods <ansar.library.management@gmail.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-1.0.2/README.rst` & `ansar_connect-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/pyproject.toml` & `ansar_connect-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/setup.py` & `ansar_connect-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/command/ansar_command.py` & `ansar_connect-1.0.3/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/command/ansar_directory.py` & `ansar_connect-1.0.3/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/command/ansar_group.py` & `ansar_connect-1.0.3/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/command/shared_directory.py` & `ansar_connect-1.0.3/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/__init__.py` & `ansar_connect-1.0.3/src/ansar/connect/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for network messaging.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 5da7d20d2635e525e46ffba86693bc69ed519a3f
-Version: 1.0.1 (2024-05-27@17:44:50+NZST)
+Commit: e2552ecf4b5ccf74b6098715adf52faea1e20bed
+Version: 1.0.2 (2024-05-29@21:03:08+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-1.0.2/src/ansar/connect/connect_directory.py` & `ansar_connect-1.0.3/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/directory.py` & `ansar_connect-1.0.3/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/directory_if.py` & `ansar_connect-1.0.3/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/foh_if.py` & `ansar_connect-1.0.3/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/group_if.py` & `ansar_connect-1.0.3/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/grouping.py` & `ansar_connect-1.0.3/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/moving.py` & `ansar_connect-1.0.3/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/networking.py` & `ansar_connect-1.0.3/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/networking_if.py` & `ansar_connect-1.0.3/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/node.py` & `ansar_connect-1.0.3/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/plumbing.py` & `ansar_connect-1.0.3/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/procedure.py` & `ansar_connect-1.0.3/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/product.py` & `ansar_connect-1.0.3/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/socketry.py` & `ansar_connect-1.0.3/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/standard.py` & `ansar_connect-1.0.3/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/transporting.py` & `ansar_connect-1.0.3/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/transporting_if.py` & `ansar_connect-1.0.3/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar/connect/wan.py` & `ansar_connect-1.0.3/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-1.0.2/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-1.0.3/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools and runtime for network messaging
 Author: Scott Woods
 Author-email: Scott Woods <ansar.library.management@gmail.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-1.0.2/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-1.0.3/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

