# Comparing `tmp/Miraheze_PyUtils-0.0.2-py3-none-any.whl.zip` & `tmp/Miraheze_PyUtils-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,30 @@
-Zip file size: 18098 bytes, number of entries: 15
--rw-r--r--  2.0 unx       13 b- defN 24-May-18 14:48 miraheze/__init__.py
--rw-r--r--  2.0 unx       18 b- defN 24-May-18 14:48 miraheze/version.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-18 14:48 miraheze/salt/__init__.py
--rw-r--r--  2.0 unx     1836 b- defN 24-May-18 14:48 miraheze/salt/utils.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-18 14:48 miraheze/salt/mwcli/__init__.py
--rw-r--r--  2.0 unx     1182 b- defN 24-May-18 14:48 miraheze/salt/mwcli/partial_reset_wiki.py
--rw-r--r--  2.0 unx     1575 b- defN 24-May-18 14:48 miraheze/salt/mwcli/rename_wiki.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-18 14:48 miraheze/swift/__init__.py
--rw-r--r--  2.0 unx     1090 b- defN 24-May-18 14:48 miraheze/swift/fix_container_permissions.py
--rw-r--r--  2.0 unx    35149 b- defN 24-May-18 14:49 Miraheze_PyUtils-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      671 b- defN 24-May-18 14:49 Miraheze_PyUtils-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-18 14:49 Miraheze_PyUtils-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      202 b- defN 24-May-18 14:49 Miraheze_PyUtils-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-18 14:49 Miraheze_PyUtils-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1296 b- defN 24-May-18 14:49 Miraheze_PyUtils-0.0.2.dist-info/RECORD
-15 files, 43136 bytes uncompressed, 15908 bytes compressed:  63.1%
+Zip file size: 36413 bytes, number of entries: 28
+-rw-r--r--  2.0 unx       13 b- defN 24-May-29 18:51 miraheze/__init__.py
+-rw-r--r--  2.0 unx       18 b- defN 24-May-29 18:51 miraheze/version.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 18:51 miraheze/mediawiki/__init__.py
+-rw-r--r--  2.0 unx      413 b- defN 24-May-29 18:51 miraheze/mediawiki/check_read_only.py
+-rw-r--r--  2.0 unx     3262 b- defN 24-May-29 18:51 miraheze/mediawiki/iaupload.py
+-rw-r--r--  2.0 unx    34233 b- defN 24-May-29 18:51 miraheze/mediawiki/mwdeploy.py
+-rw-r--r--  2.0 unx     5779 b- defN 24-May-29 18:51 miraheze/mediawiki/mwscript.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 18:51 miraheze/puppet/__init__.py
+-rw-r--r--  2.0 unx      182 b- defN 24-May-29 18:51 miraheze/puppet/cycle_puppet.py
+-rw-r--r--  2.0 unx      291 b- defN 24-May-29 18:51 miraheze/puppet/disable_puppet.py
+-rw-r--r--  2.0 unx      239 b- defN 24-May-29 18:51 miraheze/puppet/enable_puppet.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 18:51 miraheze/salt/__init__.py
+-rw-r--r--  2.0 unx     1836 b- defN 24-May-29 18:51 miraheze/salt/utils.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 18:51 miraheze/salt/mwcli/__init__.py
+-rw-r--r--  2.0 unx     1182 b- defN 24-May-29 18:51 miraheze/salt/mwcli/partial_reset_wiki.py
+-rw-r--r--  2.0 unx     1575 b- defN 24-May-29 18:51 miraheze/salt/mwcli/rename_wiki.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 18:51 miraheze/swift/__init__.py
+-rw-r--r--  2.0 unx     1090 b- defN 24-May-29 18:51 miraheze/swift/fix_container_permissions.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 18:51 tests/__init__.py
+-rw-r--r--  2.0 unx     2042 b- defN 24-May-29 18:51 tests/test_iaupload.py
+-rw-r--r--  2.0 unx    15950 b- defN 24-May-29 18:51 tests/test_mwdeploy.py
+-rw-r--r--  2.0 unx     9519 b- defN 24-May-29 18:51 tests/test_mwscript.py
+-rw-r--r--  2.0 unx    35149 b- defN 24-May-29 18:51 Miraheze_PyUtils-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1713 b- defN 24-May-29 18:51 Miraheze_PyUtils-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 18:51 Miraheze_PyUtils-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      202 b- defN 24-May-29 18:51 Miraheze_PyUtils-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 24-May-29 18:51 Miraheze_PyUtils-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2391 b- defN 24-May-29 18:51 Miraheze_PyUtils-0.0.3.dist-info/RECORD
+28 files, 117192 bytes uncompressed, 32509 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -1,13 +1,40 @@
 Filename: miraheze/__init__.py
 Comment: 
 
 Filename: miraheze/version.py
 Comment: 
 
+Filename: miraheze/mediawiki/__init__.py
+Comment: 
+
+Filename: miraheze/mediawiki/check_read_only.py
+Comment: 
+
+Filename: miraheze/mediawiki/iaupload.py
+Comment: 
+
+Filename: miraheze/mediawiki/mwdeploy.py
+Comment: 
+
+Filename: miraheze/mediawiki/mwscript.py
+Comment: 
+
+Filename: miraheze/puppet/__init__.py
+Comment: 
+
+Filename: miraheze/puppet/cycle_puppet.py
+Comment: 
+
+Filename: miraheze/puppet/disable_puppet.py
+Comment: 
+
+Filename: miraheze/puppet/enable_puppet.py
+Comment: 
+
 Filename: miraheze/salt/__init__.py
 Comment: 
 
 Filename: miraheze/salt/utils.py
 Comment: 
 
 Filename: miraheze/salt/mwcli/__init__.py
@@ -21,26 +48,38 @@
 
 Filename: miraheze/swift/__init__.py
 Comment: 
 
 Filename: miraheze/swift/fix_container_permissions.py
 Comment: 
 
-Filename: Miraheze_PyUtils-0.0.2.dist-info/LICENSE
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/test_iaupload.py
+Comment: 
+
+Filename: tests/test_mwdeploy.py
+Comment: 
+
+Filename: tests/test_mwscript.py
+Comment: 
+
+Filename: Miraheze_PyUtils-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: Miraheze_PyUtils-0.0.2.dist-info/METADATA
+Filename: Miraheze_PyUtils-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: Miraheze_PyUtils-0.0.2.dist-info/WHEEL
+Filename: Miraheze_PyUtils-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: Miraheze_PyUtils-0.0.2.dist-info/entry_points.txt
+Filename: Miraheze_PyUtils-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: Miraheze_PyUtils-0.0.2.dist-info/top_level.txt
+Filename: Miraheze_PyUtils-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: Miraheze_PyUtils-0.0.2.dist-info/RECORD
+Filename: Miraheze_PyUtils-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## miraheze/version.py

```diff
@@ -1 +1 @@
-VERSION = '0.0.2'
+VERSION = '0.0.3'
```

## Comparing `Miraheze_PyUtils-0.0.2.dist-info/LICENSE` & `Miraheze_PyUtils-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

