# Comparing `tmp/latexminted-0.1.0b1.tar.gz` & `tmp/latexminted-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latexminted-0.1.0b1.tar", last modified: Sat May 25 14:41:44 2024, max compression
+gzip compressed data, was "latexminted-0.1.0b2.tar", last modified: Tue May 28 22:15:35 2024, max compression
```

## Comparing `latexminted-0.1.0b1.tar` & `latexminted-0.1.0b2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 14:41:44.659452 latexminted-0.1.0b1/
--rw-rw-rw-   0        0        0       83 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/CHANGELOG.md
--rw-rw-rw-   0        0        0      612 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/LICENSE.txt
--rw-rw-rw-   0        0        0     2641 2024-05-25 14:41:44.655453 latexminted-0.1.0b1/PKG-INFO
--rw-rw-rw-   0        0        0      852 2024-05-25 04:10:07.000000 latexminted-0.1.0b1/README.md
--rw-rw-rw-   0        0        0     6554 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/RESTRICTED_SHELL_ESCAPE.md
-drwxrwxrwx   0        0        0        0 2024-05-25 14:41:44.534398 latexminted-0.1.0b1/latexminted/
--rw-rw-rw-   0        0        0      262 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/__init__.py
--rw-rw-rw-   0        0        0     4967 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/cmdline.py
--rw-rw-rw-   0        0        0     2280 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/command_batch.py
--rw-rw-rw-   0        0        0     6247 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/command_clean.py
--rw-rw-rw-   0        0        0     2163 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/command_config.py
--rw-rw-rw-   0        0        0      638 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/command_delete.py
--rw-rw-rw-   0        0        0    14648 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/command_highlight.py
--rw-rw-rw-   0        0        0     1580 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/command_styledef.py
--rw-rw-rw-   0        0        0      905 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/err.py
--rw-rw-rw-   0        0        0     9062 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/fmtversion.py
--rw-rw-rw-   0        0        0     3093 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/load_data.py
--rw-rw-rw-   0        0        0     4462 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/messages.py
-drwxrwxrwx   0        0        0        0 2024-05-25 14:41:44.651454 latexminted-0.1.0b1/latexminted/restricted/
--rw-rw-rw-   0        0        0      568 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/restricted/__init__.py
--rw-rw-rw-   0        0        0     1724 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/restricted/_latexminted_config.py
--rw-rw-rw-   0        0        0      264 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/restricted/_lib.py
--rw-rw-rw-   0        0        0     2505 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/restricted/_load_custom_lexer.py
--rw-rw-rw-   0        0        0    11536 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/restricted/_restricted_pathlib.py
--rw-rw-rw-   0        0        0     3375 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/restricted/_restricted_subprocess.py
--rw-rw-rw-   0        0        0      325 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/restricted/_stdlib.py
--rw-rw-rw-   0        0        0      149 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/latexminted/version.py
-drwxrwxrwx   0        0        0        0 2024-05-25 14:41:44.653453 latexminted-0.1.0b1/latexminted.egg-info/
--rw-rw-rw-   0        0        0     2641 2024-05-25 14:41:44.000000 latexminted-0.1.0b1/latexminted.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2024-05-25 14:41:44.000000 latexminted-0.1.0b1/latexminted.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 14:41:44.000000 latexminted-0.1.0b1/latexminted.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-25 14:41:44.000000 latexminted-0.1.0b1/latexminted.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-25 14:41:44.000000 latexminted-0.1.0b1/latexminted.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-25 14:41:44.000000 latexminted-0.1.0b1/latexminted.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1370 2024-05-25 03:19:34.000000 latexminted-0.1.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 14:41:44.659452 latexminted-0.1.0b1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 22:15:35.181563 latexminted-0.1.0b2/
+-rw-rw-rw-   0        0        0       83 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/CHANGELOG.md
+-rw-rw-rw-   0        0        0      612 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2641 2024-05-28 22:15:35.174564 latexminted-0.1.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/README.md
+-rw-rw-rw-   0        0        0     6440 2024-05-28 21:27:51.000000 latexminted-0.1.0b2/RESTRICTED_SHELL_ESCAPE.md
+drwxrwxrwx   0        0        0        0 2024-05-28 22:15:35.078595 latexminted-0.1.0b2/latexminted/
+-rw-rw-rw-   0        0        0      262 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/__init__.py
+-rw-rw-rw-   0        0        0     4983 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/cmdline.py
+-rw-rw-rw-   0        0        0     2280 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/command_batch.py
+-rw-rw-rw-   0        0        0     6247 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/command_clean.py
+-rw-rw-rw-   0        0        0     2165 2024-05-28 21:53:57.000000 latexminted-0.1.0b2/latexminted/command_config.py
+-rw-rw-rw-   0        0        0      638 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/command_delete.py
+-rw-rw-rw-   0        0        0    14648 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/command_highlight.py
+-rw-rw-rw-   0        0        0     1580 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/command_styledef.py
+-rw-rw-rw-   0        0        0      905 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/err.py
+-rw-rw-rw-   0        0        0     9062 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/fmtversion.py
+-rw-rw-rw-   0        0        0     3093 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/load_data.py
+-rw-rw-rw-   0        0        0     4462 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-28 22:15:35.168567 latexminted-0.1.0b2/latexminted/restricted/
+-rw-rw-rw-   0        0        0      568 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/restricted/__init__.py
+-rw-rw-rw-   0        0        0     1724 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/restricted/_latexminted_config.py
+-rw-rw-rw-   0        0        0      264 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/restricted/_lib.py
+-rw-rw-rw-   0        0        0     2505 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/restricted/_load_custom_lexer.py
+-rw-rw-rw-   0        0        0    11927 2024-05-28 21:52:15.000000 latexminted-0.1.0b2/latexminted/restricted/_restricted_pathlib.py
+-rw-rw-rw-   0        0        0     3375 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/restricted/_restricted_subprocess.py
+-rw-rw-rw-   0        0        0      325 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/latexminted/restricted/_stdlib.py
+-rw-rw-rw-   0        0        0      149 2024-05-28 20:52:46.000000 latexminted-0.1.0b2/latexminted/version.py
+drwxrwxrwx   0        0        0        0 2024-05-28 22:15:35.172565 latexminted-0.1.0b2/latexminted.egg-info/
+-rw-rw-rw-   0        0        0     2641 2024-05-28 22:15:34.000000 latexminted-0.1.0b2/latexminted.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2024-05-28 22:15:34.000000 latexminted-0.1.0b2/latexminted.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 22:15:34.000000 latexminted-0.1.0b2/latexminted.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-28 22:15:34.000000 latexminted-0.1.0b2/latexminted.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-28 22:15:34.000000 latexminted-0.1.0b2/latexminted.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 22:15:34.000000 latexminted-0.1.0b2/latexminted.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1370 2024-05-25 23:21:31.000000 latexminted-0.1.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 22:15:35.181563 latexminted-0.1.0b2/setup.cfg
```

### Comparing `latexminted-0.1.0b1/LICENSE.txt` & `latexminted-0.1.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/PKG-INFO` & `latexminted-0.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latexminted
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Python executable for LaTeX minted package
 Author-email: "Geoffrey M. Poore" <gpoore@gmail.com>
 License: latexminted Python package
         Copyright (c) 2024 Geoffrey M. Poore
         
         This work may be distributed and/or modified under the
         conditions of the LaTeX Project Public License, either version 1.3c
```

### Comparing `latexminted-0.1.0b1/README.md` & `latexminted-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/RESTRICTED_SHELL_ESCAPE.md` & `latexminted-0.1.0b2/RESTRICTED_SHELL_ESCAPE.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,57 +15,56 @@
 version 3 uses a new Python executable that is part of the `latexminted`
 Python package.  This executable is designed to be accepted as one of the
 trusted programs that TeX distributions allow to run by default, without
 needing `-shell-escape`.  This is referred to as "restricted shell scape,"
 shell escape but only for trusted executables.
 
 
-## `latexminted` and the filesystem
+## `latexminted` and the file system
 
-Restricted access to the filesystem is one aspect of the requirements for
+Restricted access to the file system is one aspect of the requirements for
 restricted shell escape.  The restrictions may be summarized as follows, based on the TeX Live configuration file
 [`texmf.cnf`](https://tug.org/svn/texlive/trunk/Build/source/texk/kpathsea/texmf.cnf?revision=70942&view=markup#l634)
 plus the changelog for `kpathsea` which mentions the new environment
 variable
 [`TEXMF_OUTPUT_DIRECTORY`](https://www.tug.org/svn/texlive/trunk/Build/source/texk/kpathsea/NEWS?view=markup).
 
-  * Reading:  Disallow reading dotfiles.
+  * Reading:  No restrictions.
 
-  * Writing:  Restrict writing to the current working directory, `$TEXMFOUT`,
-    and `$TEXMF_OUTPUT_DIRECTORY`, plus their subdirectories.
+  * Writing:  Prohibit writing dotfiles.  Restrict writing to the current
+    working directory, `$TEXMFOUT`, and `$TEXMF_OUTPUT_DIRECTORY`, plus their
+    subdirectories.
 
 The exact way that these restrictions are described in the TeX Live sources is
 somewhat different (for example, disallowing going to parent directories), but
 this is the overall effect of the restrictions.
 
 Python provides a number of ways to read and write files, including the
 [`open()`](https://docs.python.org/3/library/functions.html#open) function,
 the [`io`](https://docs.python.org/3/library/io.html) module, and the
 [`pathlib`](https://docs.python.org/3/library/pathlib.html) module.  The
-`latexminted` library restricts access to the filesystem as follows.
+`latexminted` library restricts access to the file system as follows.
 
-1.  All security-related functionality, including filesystem access, is
+1.  All security-related functionality, including file system access, is
     provided through the `restricted` subpackage.  This makes it easier to see
     whether commits modify any code with security implications.
 
 2.  Within the `restricted` subpackage, there is a `RestrictedPath` class that
     is a subclass of `pathlib.Path`.  All file path objects that are created
     in response to user data from LaTeX are instances of `RestrictedPath`.
-    Filesystem operations are initiated using instances of `RestrictedPath`,
+    File system operations are initiated using instances of `RestrictedPath`,
     including creating directories and reading and writing files.
 
-    Before an instance of `RestrictedPath` can access the filesystem, it is
+    Before an instance of `RestrictedPath` can access the file system, it is
     resolved
     ([`.resolve()`](https://docs.python.org/3/library/pathlib.html#pathlib.Path.resolve))
     to create an absolute path with no symlinks.  Then this resolved path is
     checked against the current working directory, `$TEXMFOUT`,
     and `$TEXMF_OUTPUT_DIRECTORY` to ensure that the location and type of
-    filesystem operation is allowed.  If not, an error is raised.
-
-    Reading files is currently further restricted to files within the user's home directory.  This restriction may be relaxed in the future.
+    file system operation is allowed.  If not, an error is raised.
 
     Writing/deleting files is further restricted beyond file location to files
     with names matching this regular expression:
     ```
     [0-9a-zA-Z_-]+\.(?:config|data|errlog|highlight|index|message|style)\.minted
     ```
     All temp files and cache files created by the `minted` LaTeX package and
```

### Comparing `latexminted-0.1.0b1/latexminted/cmdline.py` & `latexminted-0.1.0b2/latexminted/cmdline.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,30 +26,30 @@
 from .command_styledef import styledef
 from .load_data import load_data
 from .messages import Messages
 
 
 
 
-def main(latexmintedwin=None):
+def main(latexmintedwindows=None):
     parser = argparse.ArgumentParser(prog='latexminted', allow_abbrev=False)
     parser.set_defaults(func=lambda **x: parser.print_help())
-    if latexmintedwin is None:
+    if latexmintedwindows is None:
         library_version = ', '.join([
             f'latex2pydata {latex2pydata_version}',
             f'pygments {pygments_version}'
         ])
         version = f'latexminted {__version__} (libraries: {library_version})'
     else:
         library_version = ', '.join([
             f'latexminted {__version__}',
             f'latex2pydata {latex2pydata_version}',
             f'pygments {pygments_version}',
         ])
-        version = f'latexmintedwin {latexmintedwin} (libraries: {library_version})'
+        version = f'latexmintedwindows {latexmintedwindows} (libraries: {library_version})'
     parser.add_argument('--version', action='version', version=version)
     subparsers = parser.add_subparsers(dest='subparser_name')
 
     parser_batch = subparsers.add_parser('batch', help='Batch process highlight, styledef, and clean')
     parser_batch.set_defaults(func=batch)
     parser_batch.add_argument('--timestamp', help='LaTeX compile timestamp', required=True)
     parser_batch.add_argument('md5', help=r'MD5 hash based \jobname')
```

### Comparing `latexminted-0.1.0b1/latexminted/command_batch.py` & `latexminted-0.1.0b2/latexminted/command_batch.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/command_clean.py` & `latexminted-0.1.0b2/latexminted/command_clean.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/command_config.py` & `latexminted-0.1.0b2/latexminted/command_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     config_lines.append(rf'\gdef\minted@executable@version{{{minted_executable_version}}}%')
     config_lines.append(rf'\gdef\minted@executable@timestamp{{{timestamp}}}%')
     if data is not None:
         tex_timestamp: str = data['timestamp']
         config_lines.append(rf'\gdef\minted@config@timestamp{{{tex_timestamp}}}%')
         tex_cachepath: str
         tex_cachedir: str = data['cachedir']
-        if RestrictedPath(tex_cachedir).absolute() or not input_tempfiledir_path_str:
+        if RestrictedPath(tex_cachedir).is_absolute() or not input_tempfiledir_path_str:
             tex_cachepath = tex_cachedir
         else:
             if tex_cachedir.startswith('./'):
                 tex_cachedir = tex_cachedir[2:]
-            tex_cachepath = f'{input_tempfiledir_path_str}/{tex_cachedir}'
+            tex_cachepath = f'{input_tempfiledir_path_str}{tex_cachedir}'
         if not tex_cachepath.endswith('/'):
             tex_cachepath += '/'
         config_lines.append(rf'\gdef\minted@config@cachepath{{{tex_cachepath}}}%')
 
     try:
         (tempfiledir_path / config_file_name).write_text('\n'.join(config_lines))
     except PermissionError:
```

### Comparing `latexminted-0.1.0b1/latexminted/command_delete.py` & `latexminted-0.1.0b2/latexminted/command_delete.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/command_highlight.py` & `latexminted-0.1.0b2/latexminted/command_highlight.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/command_styledef.py` & `latexminted-0.1.0b2/latexminted/command_styledef.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/err.py` & `latexminted-0.1.0b2/latexminted/err.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/fmtversion.py` & `latexminted-0.1.0b2/latexminted/fmtversion.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/load_data.py` & `latexminted-0.1.0b2/latexminted/load_data.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/messages.py` & `latexminted-0.1.0b2/latexminted/messages.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/restricted/__init__.py` & `latexminted-0.1.0b2/latexminted/restricted/__init__.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/restricted/_latexminted_config.py` & `latexminted-0.1.0b2/latexminted/restricted/_latexminted_config.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/restricted/_load_custom_lexer.py` & `latexminted-0.1.0b2/latexminted/restricted/_load_custom_lexer.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted/restricted/_restricted_pathlib.py` & `latexminted-0.1.0b2/latexminted/restricted/_restricted_pathlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,15 @@
     Subclass of `pathlib.Path` (which is system-dependent) that restricts file
     operations to be consistent with TeX restricted shell escape security
     requirements.  For this to be effective, all file operations must go
     through this class; it must not be bypassed with other modules such as
     `os` and `shutil` or functions such as `open()`.
 
      *  Reading:  Restricted to `.read_text()`, `.read_bytes()`, and
-        `.open()`.  No reading dot files.  No reading files outside the user
-        home directory.
+        `.open()`.
 
      *  Writing:  Restricted to `.write_text()` and `.open()`.  Restricted to
         files under the current working directory, $TEXMFOUTPUT, and
         $TEXMF_OUTPUT_DIRECTORY that have names matching the regular
         expression for minted temp files or cache files.
 
      *  Deleting files:  Restricted to `.unlink()`.  Restricted to files under
@@ -58,16 +57,22 @@
          -  `.rename()`
          -  `.replace()`
          -  `.symlink_to()`
          -  `.hardlink_to()`
          -  `.touch()`
     '''
 
+    # There are currently no restrictions on reading locations, but the
+    # implementation allows this to be added.  This is equivalent to
+    # TeX Live's `openin_any = a`; see
+    # https://tug.org/svn/texlive/trunk/Build/source/texk/kpathsea/texmf.cnf?revision=70942&view=markup#l634.
     _fs_read_roots: set[pathlib.Path] = set()
-    _fs_read_roots.add(pathlib.Path.home().resolve())
+    # Similarly, there are no restrictions on reading dotfiles, but the
+    # implementation allows this to be added.
+    _fs_read_dotfiles: bool = True
 
     _fs_write_roots: set[pathlib.Path] = set()
     _fs_write_roots.add(pathlib.Path.cwd().resolve())
     for variable in ('TEXMFOUTPUT', 'TEXMF_OUTPUT_DIRECTORY'):
         value = os.getenv(variable)
         if value:
             value_path = pathlib.Path(value).resolve()
@@ -94,27 +99,27 @@
 
     _checked_executable_file_location_set: set[RestrictedPath] = set()
     _is_executable_file_location_set: set[RestrictedPath] = set()
 
     def is_readable_dir(self) -> bool:
         if self not in self._checked_readable_dir_set:
             self_resolved = self.resolve()
-            if not any(self_resolved.is_relative_to(p) for p in self._fs_read_roots):
+            if self._fs_read_roots and not any(self_resolved.is_relative_to(p) for p in self._fs_read_roots):
                 pass
             else:
                 self._is_readable_dir_set.add(self)
             self._checked_readable_dir_set.add(self)
         return self in self._is_readable_dir_set
 
     def is_readable_file(self) -> bool:
         if self not in self._checked_readable_file_set:
             self_resolved = self.resolve()
-            if not any(self_resolved.is_relative_to(p) for p in self._fs_read_roots):
+            if self._fs_read_roots and not any(self_resolved.is_relative_to(p) for p in self._fs_read_roots):
                 pass
-            elif self_resolved.name.startswith('.'):
+            elif not self._fs_read_dotfiles and self_resolved.name.startswith('.'):
                 pass
             else:
                 self._is_readable_file_set.add(self)
             self._checked_readable_file_set.add(self)
         return self in self._is_readable_file_set
 
     def is_writable_dir(self) -> bool:
```

### Comparing `latexminted-0.1.0b1/latexminted/restricted/_restricted_subprocess.py` & `latexminted-0.1.0b2/latexminted/restricted/_restricted_subprocess.py`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/latexminted.egg-info/PKG-INFO` & `latexminted-0.1.0b2/latexminted.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latexminted
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Python executable for LaTeX minted package
 Author-email: "Geoffrey M. Poore" <gpoore@gmail.com>
 License: latexminted Python package
         Copyright (c) 2024 Geoffrey M. Poore
         
         This work may be distributed and/or modified under the
         conditions of the LaTeX Project Public License, either version 1.3c
```

### Comparing `latexminted-0.1.0b1/latexminted.egg-info/SOURCES.txt` & `latexminted-0.1.0b2/latexminted.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latexminted-0.1.0b1/pyproject.toml` & `latexminted-0.1.0b2/pyproject.toml`

 * *Files identical despite different names*

