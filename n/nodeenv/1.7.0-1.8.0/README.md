# Comparing `tmp/nodeenv-1.7.0.tar.gz` & `tmp/nodeenv-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nodeenv-1.7.0.tar", last modified: Sat Jun 25 15:38:10 2022, max compression
+gzip compressed data, was "dist/nodeenv-1.8.0.tar", last modified: Fri May 12 08:09:48 2023, max compression
```

## Comparing `nodeenv-1.7.0.tar` & `nodeenv-1.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 shorrty  (783510019) LD\Domain Users (593637566)        0 2022-06-25 15:38:10.000000 nodeenv-1.7.0/
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)    27641 2022-06-25 15:38:10.000000 nodeenv-1.7.0/PKG-INFO
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1532 2022-04-21 19:26:06.000000 nodeenv-1.7.0/LICENSE
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1494 2022-06-25 15:33:52.000000 nodeenv-1.7.0/AUTHORS
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     4482 2022-06-25 15:30:36.000000 nodeenv-1.7.0/Makefile
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)    13332 2022-04-21 19:26:06.000000 nodeenv-1.7.0/CHANGES
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)      216 2022-04-21 19:26:06.000000 nodeenv-1.7.0/MANIFEST.in
-drwxr-xr-x   0 shorrty  (783510019) LD\Domain Users (593637566)        0 2022-06-25 15:38:10.000000 nodeenv-1.7.0/debian-upstream/
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)        2 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/compat
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1392 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/changelog
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)       53 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/nodeenv.links
--rwxr-xr-x   0 shorrty  (783510019) LD\Domain Users (593637566)      937 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/rules
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1532 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/copyright
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)      345 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/nodeenv.triggers
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)      752 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/control
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     7339 2022-06-25 14:04:36.000000 nodeenv-1.7.0/README
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1819 2022-04-21 19:26:06.000000 nodeenv-1.7.0/setup.py
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)    45789 2022-06-25 14:31:47.000000 nodeenv-1.7.0/nodeenv.py
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)       38 2022-06-25 15:38:10.000000 nodeenv-1.7.0/setup.cfg
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     7339 2022-06-25 14:04:36.000000 nodeenv-1.7.0/README.rst
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     6421 2022-04-21 19:26:06.000000 nodeenv-1.7.0/README.ru.rst
-drwxr-xr-x   0 shorrty  (783510019) LD\Domain Users (593637566)        0 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)    27641 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/PKG-INFO
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)        1 2022-06-25 15:21:40.000000 nodeenv-1.7.0/nodeenv.egg-info/not-zip-safe
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)      498 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/SOURCES.txt
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)       42 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/entry_points.txt
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)       11 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/requires.txt
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)        8 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/top_level.txt
--rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)        1 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/dependency_links.txt
+drwxr-xr-x   0 shorrty  (783510019) 593637566        0 2023-05-12 08:09:48.000000 nodeenv-1.8.0/
+-rw-r--r--   0 shorrty  (783510019) 593637566    27641 2023-05-12 08:09:48.000000 nodeenv-1.8.0/PKG-INFO
+-rw-r--r--   0 shorrty  (783510019) 593637566     1532 2022-04-21 19:26:06.000000 nodeenv-1.8.0/LICENSE
+-rw-r--r--   0 shorrty  (783510019) 593637566     1618 2023-05-12 08:02:08.000000 nodeenv-1.8.0/AUTHORS
+-rw-r--r--   0 shorrty  (783510019) 593637566     4482 2022-06-25 15:30:36.000000 nodeenv-1.8.0/Makefile
+-rw-r--r--   0 shorrty  (783510019) 593637566    13332 2022-04-21 19:26:06.000000 nodeenv-1.8.0/CHANGES
+-rw-r--r--   0 shorrty  (783510019) 593637566      216 2022-04-21 19:26:06.000000 nodeenv-1.8.0/MANIFEST.in
+drwxr-xr-x   0 shorrty  (783510019) 593637566        0 2023-05-12 08:09:48.000000 nodeenv-1.8.0/debian-upstream/
+-rw-r--r--   0 shorrty  (783510019) 593637566        2 2022-04-21 19:26:06.000000 nodeenv-1.8.0/debian-upstream/compat
+-rw-r--r--   0 shorrty  (783510019) 593637566     1392 2022-04-21 19:26:06.000000 nodeenv-1.8.0/debian-upstream/changelog
+-rw-r--r--   0 shorrty  (783510019) 593637566       53 2022-04-21 19:26:06.000000 nodeenv-1.8.0/debian-upstream/nodeenv.links
+-rwxr-xr-x   0 shorrty  (783510019) 593637566      937 2022-04-21 19:26:06.000000 nodeenv-1.8.0/debian-upstream/rules
+-rw-r--r--   0 shorrty  (783510019) 593637566     1532 2022-04-21 19:26:06.000000 nodeenv-1.8.0/debian-upstream/copyright
+-rw-r--r--   0 shorrty  (783510019) 593637566      345 2022-04-21 19:26:06.000000 nodeenv-1.8.0/debian-upstream/nodeenv.triggers
+-rw-r--r--   0 shorrty  (783510019) 593637566      752 2022-04-21 19:26:06.000000 nodeenv-1.8.0/debian-upstream/control
+-rw-r--r--   0 shorrty  (783510019) 593637566     7339 2022-06-25 14:04:36.000000 nodeenv-1.8.0/README
+-rw-r--r--   0 shorrty  (783510019) 593637566     1819 2022-04-21 19:26:06.000000 nodeenv-1.8.0/setup.py
+-rw-r--r--   0 shorrty  (783510019) 593637566    46439 2023-05-12 08:00:55.000000 nodeenv-1.8.0/nodeenv.py
+-rw-r--r--   0 shorrty  (783510019) 593637566       38 2023-05-12 08:09:48.000000 nodeenv-1.8.0/setup.cfg
+-rw-r--r--   0 shorrty  (783510019) 593637566     7339 2022-06-25 14:04:36.000000 nodeenv-1.8.0/README.rst
+-rw-r--r--   0 shorrty  (783510019) 593637566     6421 2022-04-21 19:26:06.000000 nodeenv-1.8.0/README.ru.rst
+drwxr-xr-x   0 shorrty  (783510019) 593637566        0 2023-05-12 08:09:48.000000 nodeenv-1.8.0/nodeenv.egg-info/
+-rw-r--r--   0 shorrty  (783510019) 593637566    27641 2023-05-12 08:09:48.000000 nodeenv-1.8.0/nodeenv.egg-info/PKG-INFO
+-rw-r--r--   0 shorrty  (783510019) 593637566        1 2022-06-25 15:21:40.000000 nodeenv-1.8.0/nodeenv.egg-info/not-zip-safe
+-rw-r--r--   0 shorrty  (783510019) 593637566      498 2023-05-12 08:09:48.000000 nodeenv-1.8.0/nodeenv.egg-info/SOURCES.txt
+-rw-r--r--   0 shorrty  (783510019) 593637566       42 2023-05-12 08:09:48.000000 nodeenv-1.8.0/nodeenv.egg-info/entry_points.txt
+-rw-r--r--   0 shorrty  (783510019) 593637566       11 2023-05-12 08:09:48.000000 nodeenv-1.8.0/nodeenv.egg-info/requires.txt
+-rw-r--r--   0 shorrty  (783510019) 593637566        8 2023-05-12 08:09:48.000000 nodeenv-1.8.0/nodeenv.egg-info/top_level.txt
+-rw-r--r--   0 shorrty  (783510019) 593637566        1 2023-05-12 08:09:48.000000 nodeenv-1.8.0/nodeenv.egg-info/dependency_links.txt
```

### Comparing `nodeenv-1.7.0/PKG-INFO` & `nodeenv-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nodeenv
-Version: 1.7.0
+Version: 1.8.0
 Summary: Node.js virtual environment builder
 Home-page: https://github.com/ekalinin/nodeenv
 Author: Eugene Kalinin
 Author-email: e.v.kalinin@gmail.com
 License: BSD
 Description: Node.js virtual environment
         ===========================
```

### Comparing `nodeenv-1.7.0/LICENSE` & `nodeenv-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/AUTHORS` & `nodeenv-1.8.0/AUTHORS`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 -  Anthony Sottile
 -  anatoly techtonik
 -  ivan hilkov
 -  Vincent Bernat
 -  Kyle P Davis
 -  Kefu Chai
 -  Elias Kunnas
+-  Avimitin
 -  Adam Johnson
 -  Pierre Le Marre
 -  Eashwar Ranganathan
 -  Doug Turnbull
 -  Anton Parkhomenko
 -  syndbg
 -  Vyacheslav Levit
@@ -24,22 +25,24 @@
 -  Lucas Cimon
 -  Lispython
 -  Leonardo Fedalto
 -  Kyle P Davis
 -  Jon Winn
 -  Duncan Bellamy
 -  Dennis Flanigan
+-  Christian Clauss
 -  Chris Beaven
 -  Cerem Cem ASLAN
 -  Bruno Oliveira
 -  Andrzej Pragacz
 -  Andrey Mishchenko
 -  Alex Couper
 -  0Xellos
 -  zjeuhpiung liu
+-  zbw
 -  urbandove
 -  sam
 -  rely10
 -  rachmadaniHaryono
 -  proItheus
 -  michael
 -  jiho
@@ -50,14 +53,15 @@
 -  Yi-Feng Tzeng
 -  Willem Jan Withagen
 -  Walter dos Santos Filho
 -  Vladimír Gorej
 -  Vincent Bernat
 -  Uman Shahzad
 -  Tom Whitwell
+-  Tom Parker-Shemilt
 -  Tim Gates
 -  Thomas Bechtold
 -  Terseus
 -  Stan Seibert
 -  Shubhang Mani
 -  Rik
 -  Philipp Dieter
@@ -72,19 +76,22 @@
 -  Laust Rud Jacobsen
 -  Ken Struys
 -  Kai Weber
 -  Josh Soref
 -  Joby Harding
 -  Jesse Dhillon
 -  Jeremy Banks
+-  Jelle van der Waa
 -  Geoffrey Huntley
 -  Fabricio C Zuardi
+-  Eashwar Ranganathan
 -  Duncan Bellamy
 -  Dennis Flanigan
 -  Dan North
 -  Dan Fuchs
 -  Damien Nozay
 -  Brian Jacobel
 -  Ben Davis
+-  Bastien Gérard
 -  Augusto Andreoli
 -  Andreas Wirooks
 -  Alexey Poryadin
```

### Comparing `nodeenv-1.7.0/Makefile` & `nodeenv-1.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/CHANGES` & `nodeenv-1.8.0/CHANGES`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/debian-upstream/changelog` & `nodeenv-1.8.0/debian-upstream/changelog`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/debian-upstream/rules` & `nodeenv-1.8.0/debian-upstream/rules`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/debian-upstream/copyright` & `nodeenv-1.8.0/debian-upstream/copyright`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/debian-upstream/control` & `nodeenv-1.8.0/debian-upstream/control`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/README` & `nodeenv-1.8.0/README`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/setup.py` & `nodeenv-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/nodeenv.py` & `nodeenv-1.8.0/nodeenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     import urllib.request as urllib2
     iteritems = operator.methodcaller('items')
     import http
     IncompleteRead = http.client.IncompleteRead
 
 from pkg_resources import parse_version
 
-nodeenv_version = '1.7.0'
+nodeenv_version = '1.8.0'
 
 join = os.path.join
 abspath = os.path.abspath
 src_base_url = None
 
 is_PY3 = sys.version_info[0] >= 3
 is_WIN = platform.system() == 'Windows'
@@ -526,14 +526,18 @@
         return src_base_url
 
 
 def is_x86_64_musl():
     return sysconfig.get_config_var('HOST_GNU_TYPE') == 'x86_64-pc-linux-musl'
 
 
+def is_riscv64():
+    return platform.machine() == 'riscv64'
+
+
 def get_node_bin_url(version):
     archmap = {
         'x86':    'x86',  # Windows Vista 32
         'i686':   'x86',
         'x86_64': 'x64',  # Linux Ubuntu 64
         'amd64':  'x64',  # FreeBSD 64bits
         'AMD64':  'x64',  # Windows Server 2012 R2 (x64)
@@ -543,14 +547,15 @@
         'aarch64': 'arm64',
         'arm64': 'arm64',
         'arm64/v8': 'arm64',
         'armv8': 'arm64',
         'armv8.4': 'arm64',
         'ppc64le': 'ppc64le',   # Power PC
         's390x': 's390x',       # IBM S390x
+        'riscv64': 'riscv64',   # RISCV 64
     }
     sysinfo = {
         'system': platform.system().lower(),
         'arch': archmap[platform.machine()],
     }
     if is_WIN or is_CYGWIN:
         postfix = '-win-%(arch)s.zip' % sysinfo
@@ -573,25 +578,36 @@
     tf = tarfile.open(*args, **kwargs)
     try:
         yield tf
     finally:
         tf.close()
 
 
+def _download_node_file(node_url, n_attempt=3):
+    """Do multiple attempts to avoid incomplete data in case
+    of unstable network"""
+    while n_attempt > 0:
+        try:
+            return io.BytesIO(urlopen(node_url).read())
+        except IncompleteRead as e:
+            logger.warning(
+                'Incomplete read while reading'
+                'from {} - {}'.format(node_url, e)
+            )
+            n_attempt -= 1
+            if n_attempt == 0:
+                raise e
+
+
 def download_node_src(node_url, src_dir, args):
     """
     Download source code
     """
     logger.info('.', extra=dict(continued=True))
-    try:
-        dl_contents = io.BytesIO(urlopen(node_url).read())
-    except IncompleteRead as e:
-        logger.warning('Incomplete read while reading'
-                       'from {}'.format(node_url))
-        dl_contents = e.partial
+    dl_contents = _download_node_file(node_url)
     logger.info('.', extra=dict(continued=True))
 
     if is_WIN or is_CYGWIN:
         ctx = zipfile.ZipFile(dl_contents)
         members = operator.methodcaller('namelist')
         member_name = lambda s: s  # noqa: E731
     else:
@@ -761,14 +777,16 @@
         try:
             download_node_src(node_url, src_dir, args)
         except urllib2.HTTPError:
             if "arm64" in node_url:
                 # if arm64 not found, try x64
                 download_node_src(node_url.replace('arm64', 'x64'),
                                   src_dir, args)
+            else:
+                logger.warning('Failed to download from %s' % node_url)
 
     logger.info('.', extra=dict(continued=True))
 
     if args.prebuilt:
         copy_node_from_prebuilt(env_dir, src_dir, args.node)
     else:
         build_node_from_src(env_dir, src_dir, node_src_dir, args)
@@ -1078,15 +1096,15 @@
     src_domain = None
     if args.mirror:
         if '://' in args.mirror:
             src_base_url = args.mirror
         else:
             src_domain = args.mirror
     # use unofficial builds only if musl and no explicitly chosen mirror
-    elif is_x86_64_musl():
+    elif is_x86_64_musl() or is_riscv64():
         src_domain = 'unofficial-builds.nodejs.org'
     else:
         src_domain = 'nodejs.org'
     if src_base_url is None:
         src_base_url = 'https://%s/download/release' % src_domain
 
     if not args.node or args.node.lower() == 'latest':
@@ -1393,18 +1411,21 @@
     end
 
     if test -n "$_OLD_NODE_FISH_PROMPT_OVERRIDE"
         # Set an empty local `$fish_function_path` to allow the removal of
         # `fish_prompt` using `functions -e`.
         set -l fish_function_path
 
-        # Erase virtualenv's `fish_prompt` and restore the original.
-        functions -e fish_prompt
-        functions -c _node_old_fish_prompt fish_prompt
-        functions -e _node_old_fish_prompt
+        # Prevents error when using nested fish instances
+        if functions -q _node_old_fish_prompt
+            # Erase virtualenv's `fish_prompt` and restore the original.
+            functions -e fish_prompt
+            functions -c _node_old_fish_prompt fish_prompt
+            functions -e _node_old_fish_prompt
+        end
         set -e _OLD_NODE_FISH_PROMPT_OVERRIDE
     end
 
     set -e NODE_VIRTUAL_ENV
 
     if test (count $argv) = 0 -o "$argv[1]" != "nondestructive"
         # Self destruct!
@@ -1488,15 +1509,15 @@
             printf '%s%s ' "__NODE_VIRTUAL_PROMPT__" (set_color normal)
         else
             printf '%s(%s) ' (set_color normal) (basename "$NODE_VIRTUAL_ENV")
         end
 
         # Restore the original $status
         echo "exit $old_status" | source
-        _old_fish_prompt
+        _node_old_fish_prompt
     end
 
     set -gx _OLD_NODE_FISH_PROMPT_OVERRIDE "$NODE_VIRTUAL_ENV"
 end
 """  # noqa: E501
 
 PREDEACTIVATE_SH = """
```

### Comparing `nodeenv-1.7.0/README.rst` & `nodeenv-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/README.ru.rst` & `nodeenv-1.8.0/README.ru.rst`

 * *Files identical despite different names*

### Comparing `nodeenv-1.7.0/nodeenv.egg-info/PKG-INFO` & `nodeenv-1.8.0/nodeenv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nodeenv
-Version: 1.7.0
+Version: 1.8.0
 Summary: Node.js virtual environment builder
 Home-page: https://github.com/ekalinin/nodeenv
 Author: Eugene Kalinin
 Author-email: e.v.kalinin@gmail.com
 License: BSD
 Description: Node.js virtual environment
         ===========================
```

