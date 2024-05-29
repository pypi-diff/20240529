# Comparing `tmp/scuba-2.8.0.tar.gz` & `tmp/scuba-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scuba-2.8.0.tar", last modified: Wed Aug 18 06:32:31 2021, max compression
+gzip compressed data, was "scuba-2.9.0.tar", last modified: Thu Sep 16 02:04:49 2021, max compression
```

## Comparing `scuba-2.8.0.tar` & `scuba-2.9.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 06:32:31.044879 scuba-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     8481 2021-08-18 06:31:56.000000 scuba-2.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-08-18 06:31:56.000000 scuba-2.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-08-18 06:31:56.000000 scuba-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-08-18 06:31:56.000000 scuba-2.8.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-08-18 06:32:31.044879 scuba-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      987 2021-08-18 06:31:56.000000 scuba-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 06:32:31.044879 scuba-2.8.0/scuba/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-08-18 06:31:56.000000 scuba-2.8.0/scuba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16724 2021-08-18 06:31:56.000000 scuba-2.8.0/scuba/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14126 2021-08-18 06:31:56.000000 scuba-2.8.0/scuba/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-08-18 06:31:56.000000 scuba-2.8.0/scuba/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2021-08-18 06:31:56.000000 scuba-2.8.0/scuba/dockerutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2021-08-18 06:31:56.000000 scuba-2.8.0/scuba/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2259 2021-08-18 06:31:56.000000 scuba-2.8.0/scuba/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 06:32:31.044879 scuba-2.8.0/scuba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-08-18 06:32:30.000000 scuba-2.8.0/scuba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-08-18 06:32:30.000000 scuba-2.8.0/scuba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-18 06:32:30.000000 scuba-2.8.0/scuba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-08-18 06:32:30.000000 scuba-2.8.0/scuba.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-18 06:32:30.000000 scuba-2.8.0/scuba.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-08-18 06:32:30.000000 scuba-2.8.0/scuba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-18 06:32:30.000000 scuba-2.8.0/scuba.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 06:32:31.044879 scuba-2.8.0/scubainit/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-08-18 06:31:56.000000 scuba-2.8.0/scubainit/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-08-18 06:31:56.000000 scuba-2.8.0/scubainit/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    16196 2021-08-18 06:31:56.000000 scuba-2.8.0/scubainit/scubainit.c
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-18 06:32:31.044879 scuba-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2021-08-18 06:31:56.000000 scuba-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 02:04:49.293736 scuba-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     8650 2021-09-16 02:04:05.000000 scuba-2.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-09-16 02:04:05.000000 scuba-2.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-09-16 02:04:05.000000 scuba-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-09-16 02:04:05.000000 scuba-2.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2021-09-16 02:04:49.293736 scuba-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2021-09-16 02:04:05.000000 scuba-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 02:04:49.293736 scuba-2.9.0/scuba/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-09-16 02:04:05.000000 scuba-2.9.0/scuba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5396 2021-09-16 02:04:05.000000 scuba-2.9.0/scuba/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12792 2021-09-16 02:04:05.000000 scuba-2.9.0/scuba/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-09-16 02:04:05.000000 scuba-2.9.0/scuba/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2021-09-16 02:04:05.000000 scuba-2.9.0/scuba/dockerutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15152 2021-09-16 02:04:05.000000 scuba-2.9.0/scuba/scuba.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1982 2021-09-16 02:04:05.000000 scuba-2.9.0/scuba/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2259 2021-09-16 02:04:05.000000 scuba-2.9.0/scuba/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 02:04:49.293736 scuba-2.9.0/scuba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2021-09-16 02:04:48.000000 scuba-2.9.0/scuba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2021-09-16 02:04:49.000000 scuba-2.9.0/scuba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-16 02:04:48.000000 scuba-2.9.0/scuba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-09-16 02:04:48.000000 scuba-2.9.0/scuba.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-16 02:04:48.000000 scuba-2.9.0/scuba.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-09-16 02:04:48.000000 scuba-2.9.0/scuba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-16 02:04:48.000000 scuba-2.9.0/scuba.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 02:04:49.293736 scuba-2.9.0/scubainit/
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-16 02:04:05.000000 scuba-2.9.0/scubainit/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-09-16 02:04:05.000000 scuba-2.9.0/scubainit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    16196 2021-09-16 02:04:05.000000 scuba-2.9.0/scubainit/scubainit.c
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-16 02:04:49.293736 scuba-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2021-09-16 02:04:05.000000 scuba-2.9.0/setup.py
```

### Comparing `scuba-2.8.0/CHANGELOG.md` & `scuba-2.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
+## [2.9.0] - 2021-09-15
+### Added
+- Add ability to specify volumes in `.scuba.yml` (#186)
+
+
 ## [2.8.0] - 2021-08-18
 ### Added
 - Add ability to specify additional docker arguments in `.scuba.yml` (#177)
 
 ### Changed
 - Switched testing framework from from `nose` to `pytest`
 
@@ -37,15 +42,15 @@
 ## [2.5.0] - 2020-03-05
 ### Changed
 - Use username/groupname of invoking user inside container (#153)
 - Ignore already existing UID/GIDs (#139)
 - Allow top-level `image` to be omitted in `.scuba.yml` (#158)
 
 ### Fixed
-- Fixed deprecation error with collections.Mapping (#156)
+- Fixed deprecation error with `collections.Mapping` (#156)
 
 ### Removed
 - Drop support for Python 2 (#154)
 
 
 ## [2.4.2] - 2020-02-24
 ### Changed
@@ -148,15 +153,15 @@
 
 
 ## [1.5.0] - 2016-02-01
 ### Added
 - Add `-r` option to run container as root
 - Add automated testing (both unit and system tests)
 - Add support for Python 2.6 - 3.5
-- Added to PyPi
+- Added to PyPI
 
 ### Changed
 - Scuba is now a package, and setup.py installs it as such, including an
   auto-generated `console_script` wrapper.
 - `--dry-run` output now shows an actual docker command-line.
 - Only pass `--tty` to docker if scuba's stdout is a TTY.
 
@@ -227,15 +232,16 @@
 - Check for and reject extraneous nodes in `.scuba.yml`
 
 
 ## 0.1.0 - 2015-12-09
 First versioned release
 
 
-[Unreleased]: https://github.com/JonathonReinhart/scuba/compare/v2.8.0...HEAD
+[Unreleased]: https://github.com/JonathonReinhart/scuba/compare/v2.9.0...HEAD
+[2.9.0]: https://github.com/JonathonReinhart/scuba/compare/v2.8.0...v2.9.0
 [2.8.0]: https://github.com/JonathonReinhart/scuba/compare/v2.7.0...v2.8.0
 [2.7.0]: https://github.com/JonathonReinhart/scuba/compare/v2.6.1...v2.7.0
 [2.6.1]: https://github.com/JonathonReinhart/scuba/compare/v2.6.0...v2.6.1
 [2.6.0]: https://github.com/JonathonReinhart/scuba/compare/v2.5.0...v2.6.0
 [2.5.0]: https://github.com/JonathonReinhart/scuba/compare/v2.4.2...v2.5.0
 [2.4.2]: https://github.com/JonathonReinhart/scuba/compare/v2.4.1...v2.4.2
 [2.4.1]: https://github.com/JonathonReinhart/scuba/compare/v2.4.0...v2.4.1
```

### Comparing `scuba-2.8.0/LICENSE.txt` & `scuba-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scuba-2.8.0/PKG-INFO` & `scuba-2.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: scuba
-Version: 2.8.0
+Version: 2.9.0
 Summary: Simplify use of Docker containers for building software
 Home-page: https://github.com/JonathonReinhart/scuba
 Author: Jonathon Reinhart
 Author-email: jonathon.reinhart@gmail.com
 License: MIT
-Description: SCUBA  [![Build Status](https://github.com/JonathonReinhart/scuba/actions/workflows/build-test.yml/badge.svg)](https://github.com/JonathonReinhart/scuba/actions/workflows/build-test.yml) [![codecov.io](https://codecov.io/github/JonathonReinhart/scuba/coverage.svg?branch=master)](https://codecov.io/github/JonathonReinhart/scuba?branch=master) [![PyPI](https://img.shields.io/pypi/v/scuba.svg)](https://pypi.python.org/pypi/scuba) [![Docs](https://readthedocs.org/projects/scuba/badge/?version=latest)](https://scuba.readthedocs.io/)
-        -----
-        
-        Simple Container-Utilizing Build Apparatus
-        
-        Scuba makes it easier to use Docker containers in everyday development. It is
-        intended to be used by developers with `make` or `scons`-based build systems,
-        where the entire build environment is encapsulated in a Docker container.
-        
-        For more information, [Read the Docs](https://scuba.readthedocs.io/).
-        
-        ## License
-        
-        This software is released under the [MIT License](https://opensource.org/licenses/MIT).
-        
 Keywords: docker
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: argcomplete
+License-File: LICENSE.txt
+
+SCUBA  [![Build Status](https://github.com/JonathonReinhart/scuba/actions/workflows/build-test.yml/badge.svg)](https://github.com/JonathonReinhart/scuba/actions/workflows/build-test.yml) [![codecov.io](https://codecov.io/github/JonathonReinhart/scuba/coverage.svg?branch=master)](https://codecov.io/github/JonathonReinhart/scuba?branch=master) [![PyPI](https://img.shields.io/pypi/v/scuba.svg)](https://pypi.python.org/pypi/scuba) [![Docs](https://readthedocs.org/projects/scuba/badge/?version=latest)](https://scuba.readthedocs.io/)
+-----
+
+Simple Container-Utilizing Build Apparatus
+
+Scuba makes it easier to use Docker containers in everyday development. It is
+intended to be used by developers with `make` or `scons`-based build systems,
+where the entire build environment is encapsulated in a Docker container.
+
+For more information, [Read the Docs](https://scuba.readthedocs.io/).
+
+## License
+
+This software is released under the [MIT License](https://opensource.org/licenses/MIT).
+
+
```

### Comparing `scuba-2.8.0/README.md` & `scuba-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `scuba-2.8.0/scuba/__main__.py` & `scuba-2.9.0/scuba/scuba.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,169 +1,105 @@
-# SCUBA - Simple Container-Utilizing Build Architecture
-# (C) 2015 Jonathon Reinhart
-# https://github.com/JonathonReinhart/scuba
-# PYTHON_ARGCOMPLETE_OK
-
-import os.path
-from pwd import getpwuid
-from grp import getgrgid
+import os
+import shutil
 import sys
-import shlex
-import itertools
-import argparse
-try:
-    import argcomplete
-except ImportError:
-    class argcomplete:
-        @staticmethod
-        def autocomplete(*_, **__):
-            pass
 import tempfile
-import shutil
 from collections.abc import Mapping
+from grp import getgrgid
 from io import StringIO
+from pwd import getpwuid
 
-from .constants import *
-from .config import find_config, load_config, ScubaConfig, \
-        ConfigError, ConfigNotFoundError
-from .utils import *
-from .version import __version__
-from .dockerutil import get_image_command, get_image_entrypoint, make_vol_opt, \
-        DockerError, DockerExecuteError
-from . import dockerutil
-
-# This is the path where all scuba-related things will be bind-mounted into the
-# container.
-SCUBA_DIR = '/.scuba'
-
-def appmsg(fmt, *args):
-    print('scuba: ' + fmt.format(*args), file=sys.stderr)
-
-def verbose_msg(fmt, *args):
-    if g_verbose:
-        appmsg(fmt, *args)
-
-def get_umask():
-    # Same logic as bash/builtins/umask.def
-    val = os.umask(0o22)
-    os.umask(val)
-    return val
-
-def writeln(f, line):
-    f.write(line + '\n')
-
-
-def parse_scuba_args(argv):
-
-    def _list_images_completer(**_):
-        return dockerutil.get_images()
-
-    def _list_aliases_completer(parsed_args, **_):
-        # We don't want to try to complete any aliases if one was already given
-        if parsed_args.command:
-            return []
-
-        try:
-            _, _, config = find_config()
-            return sorted(config.aliases)
-        except (ConfigNotFoundError, ConfigError):
-            argcomplete.warn('No or invalid config found.  Cannot auto-complete aliases.')
-            return []
-
-    ap = argparse.ArgumentParser(description='Simple Container-Utilizing Build Apparatus')
-    ap.add_argument('-d', '--docker-arg', dest='docker_args', action='append',
-            type=lambda x: shlex.split(x), default=[],
-            help="Pass additional arguments to 'docker run'")
-    ap.add_argument('-e', '--env', dest='env_vars', action='append',
-            type=parse_env_var, default=[],
-            help='Environment variables to pass to docker')
-    ap.add_argument('--entrypoint',
-            help='Override the default ENTRYPOINT of the image')
-    ap.add_argument('--image', help='Override Docker image').completer = _list_images_completer
-    ap.add_argument('--shell', help='Override shell used in Docker container')
-    ap.add_argument('-n', '--dry-run', action='store_true',
-            help="Don't actually invoke docker; just print the docker cmdline")
-    ap.add_argument('-r', '--root', action='store_true',
-            help="Run container as root (don't create scubauser)")
-    ap.add_argument('-v', '--version', action='version', version='scuba ' + __version__)
-    ap.add_argument('-V', '--verbose', action='store_true',
-            help="Be verbose")
-    ap.add_argument('command', nargs=argparse.REMAINDER,
-            help="Command (and arguments) to run in the container").completer = _list_aliases_completer
-
-    argcomplete.autocomplete(ap, always_complete_options=False)
-    args = ap.parse_args(argv)
-
-    # Flatten docker arguments into single list
-    args.docker_args = list(itertools.chain.from_iterable(args.docker_args))
-
-    # Convert env var tuples into a dict, forbidding duplicates
-    env = dict()
-    for k,v in args.env_vars:
-        if k in env:
-            ap.error("Duplicate env var {}".format(k))
-        env[k] = v
-    args.env_vars = env
-
-    global g_verbose
-    g_verbose = args.verbose
-
-    return args
+from .config import find_config, ScubaConfig, OverrideMixin
+from .config import ConfigError, ConfigNotFoundError
+from .dockerutil import get_image_command
+from .dockerutil import get_image_entrypoint
+from .dockerutil import make_vol_opt
+from .utils import shell_quote_cmd, flatten_list, get_umask, writeln
 
 
 class ScubaError(Exception):
     pass
 
 class ScubaDive:
-    def __init__(self, user_command, docker_args=None, env=None, as_root=False, verbose=False,
-            image_override=None, entrypoint=None, shell_override=None):
+    def __init__(self, user_command, config, top_path, top_rel,
+            docker_args=None, env=None, as_root=False, verbose=False,
+            image_override=None, entrypoint=None, shell_override=None, keep_tempfiles=False):
 
         env = env or {}
         if not isinstance(env, Mapping):
             raise ValueError('Argument env must be dict-like')
 
-        self.user_command = user_command
         self.as_root = as_root
         self.verbose = verbose
-        self.image_override = image_override
         self.entrypoint_override = entrypoint
-        self.shell_override = shell_override
+        self.keep_tempfiles = keep_tempfiles
 
         # These will be added to docker run cmdline
         self.env_vars = env
         self.volumes = []
         self.options = []
         self.docker_args = docker_args or []
         self.workdir = None
 
-        self.__locate_scubainit()
-        self.__load_config()
+        self.__scubadir_hostpath = None
+        self.__scubadir_contpath = None
+        self.config = config
 
 
-    def prepare(self):
-        '''Prepare to run the docker command'''
-        self.__make_scubadir()
+        # Mount scuba root directory at the same path in the container...
+        self.add_volume(top_path, top_path)
 
-        if self.is_remote_docker:
-            '''
-            Docker is running remotely (e.g. boot2docker on OSX).
-            We don't need to do any user setup whatsoever.
+        # ...and set the working dir relative to it
+        self.set_workdir(os.path.join(top_path, top_rel))
 
-            TODO: For now, remote instances won't have any .scubainit
+        self.add_env('SCUBA_ROOT', top_path)
 
-            See:
-            https://github.com/JonathonReinhart/scuba/issues/17
-            '''
-            raise ScubaError('Remote docker not supported (DOCKER_HOST is set)')
 
-        # Docker is running natively
-        self.__setup_native_run()
+        try:
 
-        # Apply environment vars from .scuba.yml
-        self.env_vars.update(self.context.environment)
+            # Process any aliases
+            self.context = ScubaContext.process_command(
+                                      cfg = self.config,
+                                      command = user_command,
+                                      image = image_override,
+                                      shell = shell_override,
+                                      )
+
+            # Apply environment vars from .scuba.yml
+            self.env_vars.update(self.context.environment)
+
+            self.__make_scubadir()
+
+            if self.is_remote_docker:
+                '''
+                Docker is running remotely (e.g. boot2docker on OSX).
+                We don't need to do any user setup whatsoever.
+
+                TODO: For now, remote instances won't have any .scubainit
+
+                See:
+                https://github.com/JonathonReinhart/scuba/issues/17
+                '''
+                raise ScubaError('Remote docker not supported (DOCKER_HOST is set)')
+
+            # Docker is running natively
+            self.__setup_native_run()
+        except:
+            self._cleanup()
+            raise
+
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *exc_info):
+        self._cleanup()
+
+    def _cleanup(self):
+        if self.__scubadir_hostpath and not self.keep_tempfiles:
+            shutil.rmtree(self.__scubadir_hostpath)
 
     def __str__(self):
         s = StringIO()
 
         indent = '  '
         level = 0
 
@@ -184,26 +120,24 @@
 
         writelist('options', self.options)
         writelist('docker_args', self.docker_args)
         writelist('env_vars', ('{}={}'.format(*e) for e in self.env_vars.items()))
         writelist('volumes', ('{} => {} {}'.format(hp, cp, opt)
                               for hp, cp, opt in self.__get_vol_opts()))
 
-        writescl('user_command', self.user_command)
         writescl('context')
         level += 1
         writescl('script', self.context.script)
         writescl('image', self.context.image)
         writelist('docker_args', self.context.docker_args)
+        writelist('volumes', self.context.volumes)
 
         return s.getvalue()
 
 
-    def cleanup_tempfiles(self):
-        shutil.rmtree(self.__scubadir_hostpath)
 
 
     @property
     def is_remote_docker(self):
         return 'DOCKER_HOST' in os.environ
 
     def add_env(self, name, val):
@@ -229,137 +163,101 @@
         self.workdir = workdir
 
     def __locate_scubainit(self):
         '''Determine path to scubainit binary
         '''
         pkg_path = os.path.dirname(__file__)
 
-        self.scubainit_path = os.path.join(pkg_path, 'scubainit')
-        if not os.path.isfile(self.scubainit_path):
-            raise ScubaError('scubainit not found at "{}"'.format(self.scubainit_path))
-
-    def __load_config(self):
-        '''Find and load .scuba.yml
-        '''
-
-        # top_path is where .scuba.yml is found, and becomes the top of our bind mount.
-        # top_rel is the relative path from top_path to the current working directory,
-        # and is where we'll set the working directory in the container (relative to
-        # the bind mount point).
-        try:
-            top_path, top_rel, self.config = find_config()
-        except ConfigNotFoundError as cfgerr:
-            # SCUBA_YML can be missing if --image was given.
-            # In this case, we assume a default config
-            if not self.image_override:
-                raise ScubaError(str(cfgerr))
-            top_path, top_rel = os.getcwd(), ''
-            self.config = ScubaConfig(image=None)
-        except ConfigError as cfgerr:
-            raise ScubaError(str(cfgerr))
-
-        # Mount scuba root directory at the same path in the container...
-        self.add_volume(top_path, top_path)
-
-        # ...and set the working dir relative to it
-        self.set_workdir(os.path.join(top_path, top_rel))
-
-        self.add_env('SCUBA_ROOT', top_path)
+        scubainit_path = os.path.join(pkg_path, 'scubainit')
+        if not os.path.isfile(scubainit_path):
+            raise ScubaError('scubainit not found at "{}"'.format(scubainit_path))
+        return scubainit_path
 
     def __make_scubadir(self):
         '''Make temp directory where all ancillary files are bind-mounted
         '''
         self.__scubadir_hostpath = tempfile.mkdtemp(prefix='scubadir')
         self.__scubadir_contpath = '/.scuba'
         self.add_volume(self.__scubadir_hostpath, self.__scubadir_contpath)
 
     def __setup_native_run(self):
         # These options are appended to mounted volume arguments
         # NOTE: This tells Docker to re-label the directory for compatibility
         # with SELinux. See `man docker-run` for more information.
         self.vol_opts = ['z']
 
-        # Process any aliases
-        context = self.config.process_command(self.user_command,
-                image=self.image_override, shell=self.shell_override)
-
         # Pass variables to scubainit
         self.add_env('SCUBAINIT_UMASK', '{:04o}'.format(get_umask()))
 
         # Check if the CLI args specify "run as root", or if the command (alias) does
-        if not self.as_root and not context.as_root:
+        if not self.as_root and not self.context.as_root:
             uid = os.getuid()
             gid = os.getgid()
             self.add_env('SCUBAINIT_UID', uid)
             self.add_env('SCUBAINIT_GID', gid)
             self.add_env('SCUBAINIT_USER', getpwuid(uid).pw_name)
             self.add_env('SCUBAINIT_GROUP', getgrgid(gid).gr_name)
 
         if self.verbose:
             self.add_env('SCUBAINIT_VERBOSE', 1)
 
 
         # Copy scubainit into the container
         # We make a copy because Docker 1.13 gets pissed if we try to re-label
         # /usr, and Fedora 28 gives an AVC denial.
-        scubainit_cpath = self.copy_scubadir_file('scubainit', self.scubainit_path)
+        scubainit_cpath = self.copy_scubadir_file('scubainit', self.__locate_scubainit())
 
         # Hooks
         for name in ('root', 'user', ):
-            self.__generate_hook_script(name, context.shell)
+            self.__generate_hook_script(name, self.context.shell)
 
         # allocate TTY if scuba's output is going to a terminal
         # and stdin is not redirected
         if sys.stdout.isatty() and sys.stdin.isatty():
             self.add_option('--tty')
 
 
         '''
         Normally, if the user provides no command to "docker run", the image's
         default CMD is run. Because we set the entrypiont, scuba must emulate the
         default behavior itself.
         '''
-        if not context.script:
+        if not self.context.script:
             # No user-provided command; we want to run the image's default command
-            verbose_msg('No user command; getting command from image')
-            default_cmd = get_image_command(context.image)
+            default_cmd = get_image_command(self.context.image)
             if not default_cmd:
                 raise ScubaError('No command given and no image-specified command')
-            verbose_msg('{} Cmd: "{}"'.format(context.image, default_cmd))
-            context.script = [shell_quote_cmd(default_cmd)]
+            self.context.script = [shell_quote_cmd(default_cmd)]
 
         # Make scubainit the real entrypoint, and use the defined entrypoint as
         # the docker command (if it exists)
         self.add_option('--entrypoint={}'.format(scubainit_cpath))
 
         self.docker_cmd = []
         if self.entrypoint_override is not None:
             # --entrypoint takes precedence
             if self.entrypoint_override != '':
                 self.docker_cmd = [self.entrypoint_override]
-        elif context.entrypoint is not None:
+        elif self.context.entrypoint is not None:
             # then .scuba.yml
-            if context.entrypoint != '':
-                self.docker_cmd = [context.entrypoint]
+            if self.context.entrypoint != '':
+                self.docker_cmd = [self.context.entrypoint]
         else:
-            ep = get_image_entrypoint(context.image)
+            ep = get_image_entrypoint(self.context.image)
             if ep:
                 self.docker_cmd = ep
 
         # The user command is executed via a generated shell script
         with self.open_scubadir_file('command.sh', 'wt') as f:
-            self.docker_cmd += [context.shell, f.container_path]
+            self.docker_cmd += [self.context.shell, f.container_path]
             writeln(f, '# Auto-generated from scuba')
             writeln(f, 'set -e')
-            for cmd in context.script:
+            for cmd in self.context.script:
                 writeln(f, cmd)
 
-        self.context = context
-
-
 
     def open_scubadir_file(self, name, mode):
         '''Opens a file in the 'scubadir'
 
         This file will automatically be bind-mounted into the container,
         at a path given by the 'container_path' property on the returned file object.
         '''
@@ -417,14 +315,17 @@
 
         for name,val in self.env_vars.items():
             args.append('--env={}={}'.format(name, val))
 
         for hostpath, contpath, options in self.__get_vol_opts():
             args.append(make_vol_opt(hostpath, contpath, options))
 
+        for _, vol in self.context.volumes.items():
+            args.append(vol.get_vol_opt())
+
         if self.workdir:
             args += ['-w', self.workdir]
 
         args += self.options
 
         # .scuba.yml (top-level or alias)
         if self.context.docker_args is not None:
@@ -439,67 +340,99 @@
 
         # Command to run in container
         args += self.docker_cmd
 
         return args
 
 
-def run_scuba(scuba_args):
-    dive = ScubaDive(
-        scuba_args.command,
-        docker_args = scuba_args.docker_args,
-        env = scuba_args.env_vars,
-        as_root = scuba_args.root,
-        verbose = scuba_args.verbose,
-        image_override = scuba_args.image,
-        entrypoint = scuba_args.entrypoint,
-        shell_override = scuba_args.shell,
-        )
-
-    try:
-        dive.prepare()
-        run_args = dive.get_docker_cmdline()
-
-        if g_verbose or scuba_args.dry_run:
-            print(str(dive))
-            print()
-
-            appmsg('Docker command line:')
-            print('$ ' + format_cmdline(run_args))
-
-        if scuba_args.dry_run:
-            sys.exit(42)
-
-        # Explicitly pass sys.stdin/stdout/stderr so they apply to the
-        # child process if overridden (by tests).
-        return dockerutil.call(
-                args = run_args,
-                stdin = sys.stdin,
-                stdout = sys.stdout,
-                stderr = sys.stderr,
+class ScubaContext:
+    def __init__(self, image=None, script=None, entrypoint=None, environment=None, shell=None, docker_args=None, volumes=None):
+        self.image = image
+        self.script = script
+        self.as_root = False
+        self.entrypoint = entrypoint
+        self.environment = environment
+        self.shell = shell
+        self.docker_args = docker_args
+        self.volumes = volumes or {}
+
+    @classmethod
+    def process_command(cls, cfg, command, image=None, shell=None):
+        '''Processes a user command using aliases
+
+        Arguments:
+            cfg         ScubaConfig object
+            command     A user command list (e.g. argv)
+            image       Override the image from .scuba.yml
+            shell       Override the shell from .scuba.yml
+
+        Returns: A ScubaContext object with the following attributes:
+            script: a list of command line strings
+            image: the docker image name to use
+        '''
+        result = cls(
+                entrypoint = cfg.entrypoint,
+                environment = cfg.environment.copy(),
+                shell = cfg.shell,
+                docker_args = cfg.docker_args,
+                volumes = cfg.volumes,
                 )
 
-    finally:
-        if scuba_args.dry_run:
-            appmsg("Temp files not cleaned up")
-        else:
-            dive.cleanup_tempfiles()
-
-
-def main(argv=None):
-    scuba_args = parse_scuba_args(argv)
-
-    try:
-        rc = run_scuba(scuba_args) or 0
-        sys.exit(rc)
-    except ConfigError as e:
-        appmsg("Config error: " + str(e))
-        sys.exit(128)
-    except DockerExecuteError as e:
-        appmsg(str(e))
-        sys.exit(2)
-    except (ScubaError, DockerError) as e:
-        appmsg(str(e))
-        sys.exit(128)
+        if command:
+            alias = cfg.aliases.get(command[0])
+            if not alias:
+                # Command is not an alias; use it as-is.
+                result.script = [shell_quote_cmd(command)]
+            else:
+                # Using an alias
+                # Does this alias override the image and/or entrypoint?
+                if alias.image:
+                    result.image = alias.image
+                if alias.entrypoint is not None:
+                    result.entrypoint = alias.entrypoint
+                if alias.shell is not None:
+                    result.shell = alias.shell
+                if alias.as_root:
+                    result.as_root = True
+
+                if isinstance(alias.docker_args, OverrideMixin) or result.docker_args is None:
+                    result.docker_args = alias.docker_args
+                elif alias.docker_args is not None:
+                    result.docker_args.extend(alias.docker_args)
+
+                if alias.volumes is not None:
+                    result.volumes.update(alias.volumes)
+
+                # Merge/override the environment
+                if alias.environment:
+                    result.environment.update(alias.environment)
+
+                if len(alias.script) > 1:
+                    # Alias is a multiline script; no additional
+                    # arguments are allowed in the scuba invocation.
+                    if len(command) > 1:
+                        raise ConfigError('Additional arguments not allowed with multi-line aliases')
+                    result.script = alias.script
+
+                else:
+                    # Alias is a single-line script; perform substituion
+                    # and add user arguments.
+                    command.pop(0)
+                    result.script = [alias.script[0] + ' ' + shell_quote_cmd(command)]
+
+            result.script = flatten_list(result.script)
+
+        # If a shell was given on the CLI, it should override the shell set by
+        # the alias or top-level config
+        if shell:
+            result.shell = shell
+
+        # If an image was given, it overrides what might have been set by an alias
+        if image:
+            result.image = image
+
+        # If the image was still not set, then try to get it from the confg,
+        # which will raise a ConfigError if it is not set
+        if not result.image:
+            result.image = cfg.image
 
-if __name__ == '__main__':
-    main()
+        return result
```

### Comparing `scuba-2.8.0/scuba/config.py` & `scuba-2.9.0/scuba/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import yaml
 import re
 import shlex
 
 from .constants import *
 from .utils import *
+from .dockerutil import make_vol_opt
 
 class ConfigError(Exception):
     pass
 
 class ConfigNotFoundError(ConfigError):
     pass
 
@@ -235,201 +236,168 @@
         override = isinstance(args, OverrideMixin)
         args = shlex.split(args)
         if override:
             args = OverrideList(args)
 
     return args
 
+def _get_typed_val(data, key, type_):
+    v = data.get(key)
+    if v is not None and not isinstance(v, type_):
+        raise ConfigError("'{}' must be a {}, not {}".format(
+                key, type_.__name__, type(v).__name__))
+    return v
+
+def _get_dict(data, key):
+    return _get_typed_val(data, key, dict)
+
+def _get_delimited_str_list(data, key, sep):
+    s = _get_typed_val(data, key, str)
+    return s.split(sep) if s else []
+
+def _get_volumes(data):
+    voldata = _get_dict(data, 'volumes')
+    if voldata is None:
+        return None
+
+    vols = {}
+    for cpath, v in voldata.items():
+        vols[cpath] = ScubaVolume.from_dict(cpath, v)
+    return vols
+
+class ScubaVolume:
+    def __init__(self, container_path, host_path=None, options=None):
+        self.container_path = container_path
+        self.host_path = host_path
+        self.options = options or []
+
+    @classmethod
+    def from_dict(cls, cpath, node):
+        # Treat a null node as an empty dict
+        if node is None:
+            node = {}
+
+        # Simple form:
+        # volumes:
+        #   /foo: /host/foo
+        if isinstance(node, str):
+            return cls(
+                container_path = cpath,
+                host_path = node,
+                )
+
+        # Complex form
+        # volumes:
+        #   /foo:
+        #     hostpath: /host/foo
+        #     options: ro,z
+        if isinstance(node, dict):
+            hpath = node.get('hostpath')
+            if hpath is None:
+                raise ConfigError("Volume {} must have a 'hostpath' subkey".format(cpath))
+            return cls(
+                container_path = cpath,
+                host_path = hpath,
+                options = _get_delimited_str_list(node, 'options', ','),
+                )
+
+        raise ConfigError("{}: must be string or dict".format(cpath))
+
+    def get_vol_opt(self):
+        if not self.host_path:
+            raise NotImplementedError("No anonymous volumes for now")
+        return make_vol_opt(self.host_path, self.container_path, self.options)
+
+
 class ScubaAlias:
-    def __init__(self, name, script, image, entrypoint, environment, shell, as_root, docker_args):
+    def __init__(self, name, script, image=None, entrypoint=None,
+            environment=None, shell=None, as_root=None, docker_args=None,
+            volumes=None):
         self.name = name
         self.script = script
         self.image = image
         self.entrypoint = entrypoint
         self.environment = environment
         self.shell = shell
-        self.as_root = as_root
+        self.as_root = bool(as_root)
         self.docker_args = docker_args
+        self.volumes = volumes
 
     @classmethod
     def from_dict(cls, name, node):
         script = _process_script_node(node, name)
-        image = None
-        entrypoint = None
-        environment = None
-        shell = None
-        as_root = False
-        docker_args = None
 
         if isinstance(node, dict):  # Rich alias
-            image = node.get('image')
-            docker_args = _get_docker_args(node)
-            entrypoint = _get_entrypoint(node)
-            environment = _process_environment(
-                    node.get('environment'),
-                    '{}.{}'.format(name, 'environment'))
-            shell = node.get('shell')
-            as_root = node.get('root', as_root)
+            return cls(
+                name = name,
+                script = script,
+                image = node.get('image'),
+                entrypoint = _get_entrypoint(node),
+                environment = _process_environment(
+                        node.get('environment'),
+                        '{}.{}'.format(name, 'environment')),
+                shell = node.get('shell'),
+                as_root = node.get('root'),
+                docker_args = _get_docker_args(node),
+                volumes = _get_volumes(node),
+                )
 
-        return cls(name, script, image, entrypoint, environment, shell, as_root, docker_args)
+        return cls(name=name, script=script)
 
-class ScubaContext:
-    pass
 
 class ScubaConfig:
     def __init__(self, **data):
-        optional_nodes = ('image','aliases','hooks','entrypoint','environment','shell','docker_args')
+        optional_nodes = (
+            'image', 'aliases', 'hooks', 'entrypoint', 'environment', 'shell',
+            'docker_args', 'volumes',
+        )
 
         # Check for unrecognized nodes
         extra = [n for n in data if not n in optional_nodes]
         if extra:
             raise ConfigError('{}: Unrecognized node{}: {}'.format(SCUBA_YML,
                     's' if len(extra) > 1 else '', ', '.join(extra)))
 
         self._image = data.get('image')
-        self._shell = data.get('shell', DEFAULT_SHELL)
-        self._entrypoint = _get_entrypoint(data)
-        self._docker_args = _get_docker_args(data)
+        self.shell = data.get('shell', DEFAULT_SHELL)
+        self.entrypoint = _get_entrypoint(data)
+        self.docker_args = _get_docker_args(data)
+        self.volumes = _get_volumes(data)
         self._load_aliases(data)
         self._load_hooks(data)
-        self._environment = self._load_environment(data)
-
-
+        self._load_environment(data)
 
 
     def _load_aliases(self, data):
-        self._aliases = {}
+        self.aliases = {}
 
         for name, node in data.get('aliases', {}).items():
             if ' ' in name:
                 raise ConfigError('Alias names cannot contain spaces')
-            self._aliases[name] = ScubaAlias.from_dict(name, node)
-
+            self.aliases[name] = ScubaAlias.from_dict(name, node)
 
     def _load_hooks(self, data):
-        self._hooks = {}
+        self.hooks = {}
 
         for name in ('user', 'root',):
             node = data.get('hooks', {}).get(name)
             if node:
                 hook = _process_script_node(node, name)
-                self._hooks[name] = hook
+                self.hooks[name] = hook
 
     def _load_environment(self, data):
-         return _process_environment(data.get('environment'), 'environment')
+        self.environment = _process_environment(data.get('environment'), 'environment')
 
 
     @property
     def image(self):
         if not self._image:
             raise ConfigError("Top-level 'image' not set")
         return self._image
 
-    @property
-    def entrypoint(self):
-        return self._entrypoint
-
-    @property
-    def aliases(self):
-        return self._aliases
-
-    @property
-    def hooks(self):
-        return self._hooks
-
-    @property
-    def environment(self):
-        return self._environment
-
-    @property
-    def shell(self):
-        return self._shell
-
-    @property
-    def docker_args(self):
-        return self._docker_args
-
-
-    def process_command(self, command, image=None, shell=None):
-        '''Processes a user command using aliases
-
-        Arguments:
-            command     A user command list (e.g. argv)
-            image       Override the image from .scuba.yml
-            shell       Override the shell from .scuba.yml
-
-        Returns: A ScubaContext object with the following attributes:
-            script: a list of command line strings
-            image: the docker image name to use
-        '''
-        result = ScubaContext()
-        result.script = None
-        result.image = None
-        result.entrypoint = self.entrypoint
-        result.environment = self.environment.copy()
-        result.shell = self.shell
-        result.as_root = False
-        result.docker_args = self.docker_args
-
-        if command:
-            alias = self.aliases.get(command[0])
-            if not alias:
-                # Command is not an alias; use it as-is.
-                result.script = [shell_quote_cmd(command)]
-            else:
-                # Using an alias
-                # Does this alias override the image and/or entrypoint?
-                if alias.image:
-                    result.image = alias.image
-                if alias.entrypoint is not None:
-                    result.entrypoint = alias.entrypoint
-                if alias.shell is not None:
-                    result.shell = alias.shell
-                if alias.as_root:
-                    result.as_root = True
-
-                if isinstance(alias.docker_args, OverrideMixin) or result.docker_args is None:
-                    result.docker_args = alias.docker_args
-                elif alias.docker_args is not None:
-                    result.docker_args.extend(alias.docker_args)
-
-                # Merge/override the environment
-                if alias.environment:
-                    result.environment.update(alias.environment)
-
-                if len(alias.script) > 1:
-                    # Alias is a multiline script; no additional
-                    # arguments are allowed in the scuba invocation.
-                    if len(command) > 1:
-                        raise ConfigError('Additional arguments not allowed with multi-line aliases')
-                    result.script = alias.script
-
-                else:
-                    # Alias is a single-line script; perform substituion
-                    # and add user arguments.
-                    command.pop(0)
-                    result.script = [alias.script[0] + ' ' + shell_quote_cmd(command)]
-
-            result.script = flatten_list(result.script)
-
-        # If a shell was given on the CLI, it should override the shell set by
-        # the alias or top-level config
-        if shell:
-            result.shell = shell
-
-        # If an image was given, it overrides what might have been set by an alias
-        if image:
-            result.image = image
-
-        # If the image was still not set, then try to get it from the confg,
-        # which will raise a ConfigError if it is not set
-        if not result.image:
-            result.image = self.image
-
-        return result
 
 
 def load_config(path):
     try:
         with open(path, 'r') as f:
             data = yaml.load(f, Loader)
     except IOError as e:
```

### Comparing `scuba-2.8.0/scuba/dockerutil.py` & `scuba-2.9.0/scuba/dockerutil.py`

 * *Files identical despite different names*

### Comparing `scuba-2.8.0/scuba/utils.py` & `scuba-2.9.0/scuba/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,7 +64,18 @@
     for i in x:
         if isinstance(i, list):
             for j in flatten_list(i):
                 result.append(j)
         else:
             result.append(i)
     return result
+
+
+def get_umask():
+    # Same logic as bash/builtins/umask.def
+    val = os.umask(0o22)
+    os.umask(val)
+    return val
+
+
+def writeln(f, line):
+    f.write(line + '\n')
```

### Comparing `scuba-2.8.0/scuba/version.py` & `scuba-2.9.0/scuba/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 PACKAGEPATH = abspath(dirname(__file__))
 PROJPATH = dirname(PACKAGEPATH)
 
 DIST_SPEC = 'scuba'
 
 # Base version, which will be augmented with Git information
-BASE_VERSION = '2.8.0'
+BASE_VERSION = '2.9.0'
 
 # This string will be replaced by `git-archive`
 # with the abbreviated commit hash
 git_archive_rev = "$Format:%h$"
 
 def git_describe():
     from subprocess import check_call, check_output
```

### Comparing `scuba-2.8.0/scuba.egg-info/PKG-INFO` & `scuba-2.9.0/scuba.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: scuba
-Version: 2.8.0
+Version: 2.9.0
 Summary: Simplify use of Docker containers for building software
 Home-page: https://github.com/JonathonReinhart/scuba
 Author: Jonathon Reinhart
 Author-email: jonathon.reinhart@gmail.com
 License: MIT
-Description: SCUBA  [![Build Status](https://github.com/JonathonReinhart/scuba/actions/workflows/build-test.yml/badge.svg)](https://github.com/JonathonReinhart/scuba/actions/workflows/build-test.yml) [![codecov.io](https://codecov.io/github/JonathonReinhart/scuba/coverage.svg?branch=master)](https://codecov.io/github/JonathonReinhart/scuba?branch=master) [![PyPI](https://img.shields.io/pypi/v/scuba.svg)](https://pypi.python.org/pypi/scuba) [![Docs](https://readthedocs.org/projects/scuba/badge/?version=latest)](https://scuba.readthedocs.io/)
-        -----
-        
-        Simple Container-Utilizing Build Apparatus
-        
-        Scuba makes it easier to use Docker containers in everyday development. It is
-        intended to be used by developers with `make` or `scons`-based build systems,
-        where the entire build environment is encapsulated in a Docker container.
-        
-        For more information, [Read the Docs](https://scuba.readthedocs.io/).
-        
-        ## License
-        
-        This software is released under the [MIT License](https://opensource.org/licenses/MIT).
-        
 Keywords: docker
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: argcomplete
+License-File: LICENSE.txt
+
+SCUBA  [![Build Status](https://github.com/JonathonReinhart/scuba/actions/workflows/build-test.yml/badge.svg)](https://github.com/JonathonReinhart/scuba/actions/workflows/build-test.yml) [![codecov.io](https://codecov.io/github/JonathonReinhart/scuba/coverage.svg?branch=master)](https://codecov.io/github/JonathonReinhart/scuba?branch=master) [![PyPI](https://img.shields.io/pypi/v/scuba.svg)](https://pypi.python.org/pypi/scuba) [![Docs](https://readthedocs.org/projects/scuba/badge/?version=latest)](https://scuba.readthedocs.io/)
+-----
+
+Simple Container-Utilizing Build Apparatus
+
+Scuba makes it easier to use Docker containers in everyday development. It is
+intended to be used by developers with `make` or `scons`-based build systems,
+where the entire build environment is encapsulated in a Docker container.
+
+For more information, [Read the Docs](https://scuba.readthedocs.io/).
+
+## License
+
+This software is released under the [MIT License](https://opensource.org/licenses/MIT).
+
+
```

### Comparing `scuba-2.8.0/scubainit/scubainit.c` & `scuba-2.9.0/scubainit/scubainit.c`

 * *Files identical despite different names*

### Comparing `scuba-2.8.0/setup.py` & `scuba-2.9.0/setup.py`

 * *Files identical despite different names*

