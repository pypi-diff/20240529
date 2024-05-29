# Comparing `tmp/wp_enhanced-0.8.9.tar.gz` & `tmp/wp_enhanced-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wp_enhanced-0.8.9.tar", max compression
+gzip compressed data, was "wp_enhanced-0.9.0.tar", max compression
```

## Comparing `wp_enhanced-0.8.9.tar` & `wp_enhanced-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,37 @@
--rw-r--r--   0        0        0      593 2024-03-19 11:00:28.048604 wp_enhanced-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     1975 2024-03-05 10:44:56.655179 wp_enhanced-0.8.9/README.md
--rw-r--r--   0        0        0     4711 2024-03-14 08:22:26.062624 wp_enhanced-0.8.9/src/wpe/cli.py
--rw-r--r--   0        0        0     6947 2024-03-19 10:42:30.989172 wp_enhanced-0.8.9/src/wpe/core.py
--rw-r--r--   0        0        0     1778 2024-03-19 10:33:46.953081 wp_enhanced-0.8.9/src/wpe/hook_processor.py
--rw-r--r--   0        0        0    17482 2024-03-14 07:44:27.317521 wp_enhanced-0.8.9/src/wpe/parameter.py
--rw-r--r--   0        0        0     2287 2024-03-14 03:45:45.269746 wp_enhanced-0.8.9/src/wpe/pathman.py
--rw-r--r--   0        0        0     3810 2024-03-19 10:53:13.200056 wp_enhanced-0.8.9/src/wpe/project_config.py
--rw-r--r--   0        0        0     1298 2023-11-16 06:38:22.015600 wp_enhanced-0.8.9/src/wpe/templates/.wpe/hooks/post_build.py
--rw-r--r--   0        0        0     1988 2024-03-19 07:55:45.477030 wp_enhanced-0.8.9/src/wpe/templates/.wpe/wpe_project.toml
--rw-r--r--   0        0        0     3525 2024-01-18 03:32:51.913897 wp_enhanced-0.8.9/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp
--rw-r--r--   0        0        0     3456 2024-01-18 03:31:38.067723 wp_enhanced-0.8.9/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h
--rw-r--r--   0        0        0     2591 2023-11-09 12:01:43.217512 wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectName.xml
--rw-r--r--   0        0        0     2619 2023-11-09 12:01:43.210512 wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp
--rw-r--r--   0        0        0     2212 2023-11-09 12:01:43.213515 wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h
--rw-r--r--   0        0        0      781 2023-08-31 03:15:55.810608 wp_enhanced-0.8.9/src/wpe/util.py
--rw-r--r--   0        0        0     5618 2024-03-19 10:51:33.313938 wp_enhanced-0.8.9/src/wpe/wp_patch/build.py
--rw-r--r--   0        0        0     2847 2024-03-19 03:42:12.795265 wp_enhanced-0.8.9/src/wpe/wp_patch/common/command/android.py
--rw-r--r--   0        0        0     1409 2024-03-19 03:38:23.562202 wp_enhanced-0.8.9/src/wpe/wp_patch/common/platform/android.py
--rw-r--r--   0        0        0    11282 2023-12-20 09:52:04.364880 wp_enhanced-0.8.9/src/wpe/wp_patch/package.py
--rw-r--r--   0        0        0     2560 2024-03-14 08:02:19.221827 wp_enhanced-0.8.9/src/wpe/wp_patch/premake.py
--rw-r--r--   0        0        0    12877 2024-03-15 09:30:41.524075 wp_enhanced-0.8.9/src/wpe/wp_patch/premakePlugins.lua
--rw-r--r--   0        0        0     3846 2024-03-19 10:51:33.314938 wp_enhanced-0.8.9/src/wpe/wp_wrapper.py
--rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 wp_enhanced-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0      629 2024-05-29 10:23:14.223279 wp_enhanced-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1975 2024-03-05 10:44:56.655179 wp_enhanced-0.9.0/README.md
+-rw-r--r--   0        0        0     5471 2024-05-29 08:37:52.344092 wp_enhanced-0.9.0/src/wpe/cli.py
+-rw-r--r--   0        0        0     3414 2024-05-20 06:36:07.243649 wp_enhanced-0.9.0/src/wpe/constants.py
+-rw-r--r--   0        0        0     9201 2024-05-29 09:55:00.869477 wp_enhanced-0.9.0/src/wpe/core.py
+-rw-r--r--   0        0        0     1778 2024-03-19 10:33:46.953081 wp_enhanced-0.9.0/src/wpe/hook_processor.py
+-rw-r--r--   0        0        0    22804 2024-05-24 09:25:52.692469 wp_enhanced-0.9.0/src/wpe/parameter.py
+-rw-r--r--   0        0        0     2557 2024-05-29 09:54:49.747133 wp_enhanced-0.9.0/src/wpe/pathman.py
+-rw-r--r--   0        0        0     4372 2024-05-20 08:48:15.544654 wp_enhanced-0.9.0/src/wpe/project_config.py
+-rw-r--r--   0        0        0     2536 2024-05-29 10:22:40.904327 wp_enhanced-0.9.0/src/wpe/renamer.py
+-rw-r--r--   0        0        0      529 2024-03-20 09:54:37.946663 wp_enhanced-0.9.0/src/wpe/templates/.wpe/hooks/post_build.py
+-rw-r--r--   0        0        0      570 2024-05-15 07:41:57.248430 wp_enhanced-0.9.0/src/wpe/templates/.wpe/hooks/pre_premake.py
+-rw-r--r--   0        0        0     2313 2024-05-24 09:16:35.575895 wp_enhanced-0.9.0/src/wpe/templates/.wpe/wpe_project.toml
+-rw-r--r--   0        0        0     3564 2024-05-15 10:45:20.195972 wp_enhanced-0.9.0/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp
+-rw-r--r--   0        0        0     3637 2024-05-15 10:45:01.387675 wp_enhanced-0.9.0/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h
+-rw-r--r--   0        0        0        7 2024-03-28 07:45:27.251336 wp_enhanced-0.9.0/src/wpe/templates/test/.gitignore
+-rw-r--r--   0        0        0      690 2024-03-28 10:50:17.608326 wp_enhanced-0.9.0/src/wpe/templates/test/CMakeLists.txt
+-rw-r--r--   0        0        0     1088 2024-03-28 10:27:22.354678 wp_enhanced-0.9.0/src/wpe/templates/test/main.cpp
+-rw-r--r--   0        0        0     3720 2024-03-28 10:20:00.582064 wp_enhanced-0.9.0/src/wpe/templates/test/util/test_mem_alloc.hpp
+-rw-r--r--   0        0        0      546 2024-03-28 10:23:24.722404 wp_enhanced-0.9.0/src/wpe/templates/test/util/test_util.hpp
+-rw-r--r--   0        0        0     2319 2024-05-21 07:17:38.787997 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectName.rc
+-rw-r--r--   0        0        0     2591 2023-11-09 12:01:43.217512 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectName.xml
+-rw-r--r--   0        0        0     2619 2023-11-09 12:01:43.210512 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp
+-rw-r--r--   0        0        0     2212 2023-11-09 12:01:43.213515 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h
+-rw-r--r--   0        0        0      502 2024-05-21 07:17:53.334293 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/resource.h
+-rw-r--r--   0        0        0     1649 2024-05-21 07:38:14.439284 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.cpp
+-rw-r--r--   0        0        0      865 2024-05-21 06:24:33.977130 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.h
+-rw-r--r--   0        0        0     4743 2024-03-28 10:59:21.634177 wp_enhanced-0.9.0/src/wpe/test_runner.py
+-rw-r--r--   0        0        0     3440 2024-05-29 10:11:26.069297 wp_enhanced-0.9.0/src/wpe/util.py
+-rw-r--r--   0        0        0     5618 2024-03-19 10:51:33.313938 wp_enhanced-0.9.0/src/wpe/wp_patch/build.py
+-rw-r--r--   0        0        0     2847 2024-03-19 03:42:12.795265 wp_enhanced-0.9.0/src/wpe/wp_patch/common/command/android.py
+-rw-r--r--   0        0        0     1409 2024-03-19 03:38:23.562202 wp_enhanced-0.9.0/src/wpe/wp_patch/common/platform/android.py
+-rw-r--r--   0        0        0    11092 2024-04-28 06:59:44.257676 wp_enhanced-0.9.0/src/wpe/wp_patch/package.py
+-rw-r--r--   0        0        0     2560 2024-03-14 08:02:19.221827 wp_enhanced-0.9.0/src/wpe/wp_patch/premake.py
+-rw-r--r--   0        0        0    12962 2024-03-20 09:54:02.989529 wp_enhanced-0.9.0/src/wpe/wp_patch/premakePlugins.lua
+-rw-r--r--   0        0        0     3846 2024-03-19 10:51:33.314938 wp_enhanced-0.9.0/src/wpe/wp_wrapper.py
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 wp_enhanced-0.9.0/PKG-INFO
```

### Comparing `wp_enhanced-0.8.9/README.md` & `wp_enhanced-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/cli.py` & `wp_enhanced-0.9.0/src/wpe/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,24 @@
         dest='build',
         default=False,
         required=False,
         help='Build project.'
     )
 
     command_group.add_argument(
+        '-t',
+        '--test',
+        action='store_true',
+        dest='test',
+        default=False,
+        required=False,
+        help='Test plugin with catch2 framework.'
+    )
+
+    command_group.add_argument(
         '-P',
         '--pack',
         action='store_true',
         dest='pack',
         default=False,
         required=False,
         help='Package plugin.'
@@ -97,14 +107,24 @@
         action='store_true',
         dest='bump',
         default=False,
         required=False,
         help='Bump wpe project version.'
     )
 
+    command_group.add_argument(
+        '--rename',
+        action='store',
+        type=str,
+        dest='rename',
+        default='',
+        required=False,
+        help='Rename plugin.'
+    )
+
     parser.add_argument(
         '-H',
         '--with-hooks',
         action='store',
         dest='withHooks',
         nargs='*',
         default=[],
@@ -116,21 +136,24 @@
   - proj_root: project root path
   - build_config: build configuration (Debug, Profile, Release)
   - plugin_name: plugin name, which is used to glob plugin files'''
     )
 
     parser.add_argument(
         '-plt',
-        '--platform',
+        '--platforms',
         action='store',
-        choices=('', 'Android', 'Authoring', 'Authoring_Windows', 'Authoring_Linux', 'Authoring_Mac', 'iOS', 'Linux', 'LinuxAuto', 'Mac', 'NX', 'PS4', 'PS5', 'QNX', 'tvOS', 'Windows_vc160', 'Windows_vc170', 'WinGC', 'XboxOneGC', 'XboxSeriesX'),
-        dest='platform',
-        default='',
+        choices=['Android', 'Authoring', 'Authoring_Windows', 'Authoring_Linux', 'Authoring_Mac', 'iOS', 'Linux',
+                 'LinuxAuto', 'Mac', 'NX', 'PS4', 'PS5', 'QNX', 'tvOS', 'Windows_vc140', 'Windows_vc150',
+                 'Windows_vc160', 'Windows_vc170', 'WinGC', 'XboxOneGC', 'XboxSeriesX'],
+        dest='platforms',
+        default=[],
+        nargs='*',
         required=False,
-        help='Platform to premake/build. Leave empty to premake/build all platforms defined in `wpe_project.toml`.'
+        help='Platforms to premake/build. Leave empty to premake/build all platforms defined in `wpe_project.toml`.'
     )
     parser.add_argument(
         '-c',
         '--configuration',
         action='store',
         choices=('Debug', 'Profile', 'Release'),
         dest='configuration',
@@ -145,15 +168,24 @@
         dest='force',
         required=False,
         default=False,
         help='''Force operation. This argument is compatible with -gp or -b.
     For -gp, it will overwrite existing source files.
     For -b, it will terminate Wwise process and copy plugin files, then reopen Wwise.'''
     )
+    parser.add_argument(
+        '-g',
+        '--gui',
+        action='store_true',
+        dest='gui',
+        required=False,
+        default=False,
+        help='Effective when -gp is specified. Generate GUI resources.'
+    )
 
     parsed_args = parser.parse_args()
-    worker = Worker.get_platform_worker(parsed_args)
+    worker = Worker.create_platform(parsed_args)
     worker.main()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `wp_enhanced-0.8.9/src/wpe/core.py` & `wp_enhanced-0.9.0/src/wpe/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,167 @@
 import logging
 import os.path as osp
 import platform
 import subprocess
 import glob
+from typing import Optional
 
 # 3rd party
 import kkpyutil as util
 
 # project
 import wpe.util as wpe_util
 from wpe.pathman import PathMan
 from wpe.wp_wrapper import WpWrapper
 from wpe.parameter import ParameterGenerator
 from wpe.hook_processor import HookProcessor
 from wpe.project_config import ProjectConfig, PlatformTarget
+from wpe.test_runner import TestRunner
+from wpe.renamer import Renamer
+from wpe import constants
 
 
 class Worker:
     def __init__(self, args, path_man=None):
         self.args = args
 
         self.wpWrapper = WpWrapper()
 
         # lazy inits
-        self.pathMan = path_man
-        self.projConfig = None
+        self.pathMan: Optional[PathMan] = path_man
+        self.projConfig: Optional[ProjectConfig] = None
         self.targetPlatforms: list[PlatformTarget] = []
 
         self.wwiseProcName = ''
         self.terminatedWwise = False
 
     @staticmethod
-    def get_platform_worker(args):
+    def create_platform(args):
         system = platform.system()
         if system == 'Windows':
             return WindowsWorker(args)
         if system == 'Darwin':
             return MacWorker(args)
         raise NotImplementedError(f'Not implemented for this platform: {system}')
 
-    def _lazy_init_pathman(self):
+    def _lazy_load_configs(self):
         self.pathMan = self.pathMan or PathMan()
         self.projConfig = ProjectConfig(self.pathMan)
         self.targetPlatforms = self.projConfig.target_platforms()
-        if self.args.platform:
-            self.targetPlatforms = [plt for plt in self.targetPlatforms if plt.platform == self.args.platform]
+        if self.args.platforms:
+            self.targetPlatforms = [plt for plt in self.targetPlatforms if plt.platform in self.args.platforms]
         HookProcessor().init(self.pathMan, self.args.configuration, self.args.withHooks)
 
     def main(self):
         self.wpWrapper.validate_env()
 
         if self.args.wp:
             return self.wp()
 
         if self.args.new:
             return self.new()
 
-        self._lazy_init_pathman()
+        self._lazy_load_configs()
 
         if self.args.initWpe:
             return self.init_wpe()
 
         if self.args.premake:
             self.premake()
 
         if self.args.generateParameters:
             self.generate_parameters()
 
         if self.args.build:
             self.build()
 
+        if self.args.test:
+            self.test()
+
         if self.args.pack:
             self.pack()
 
         if self.args.fullPack:
             self.full_pack()
 
         if self.args.bump:
             self.bump()
 
+        if self.args.rename:
+            self.rename()
+
     def wp(self):
         logging.info('Run wp.py')
         self.wpWrapper.wp(self.args.wp)
 
     def new(self):
+        def _copy_win32_gui_resource():
+            wpe_util.copy_template('WwisePlugin/ProjectName.rc', self.pathMan)
+            wpe_util.copy_template('WwisePlugin/resource.h', self.pathMan)
+            wpe_util.copy_template('WwisePlugin/Win32/ProjectNamePluginGUI.h', self.pathMan)
+            wpe_util.copy_template('WwisePlugin/Win32/ProjectNamePluginGUI.cpp', self.pathMan)
+
         logging.info('Create new project')
         self.wpWrapper.new()
         self.init_wpe()
+        self._lazy_load_configs()
+        _copy_win32_gui_resource()
         self.premake()
         logging.info('Next step: implement your plugin, build with hooks by command: wpe -b -H')
 
     def init_wpe(self):
+        def _append_to_gitignore():
+            gitignore = osp.join(self.pathMan.root, '.gitignore')
+            if osp.exists(gitignore):
+                with open(gitignore, 'a') as f:
+                    f.write(constants.extra_gitignore)
         logging.info('Initialize wpe project config')
-        self._lazy_init_pathman()
-
+        self.pathMan = self.pathMan or PathMan()
+        HookProcessor().init(self.pathMan, self.args.configuration, self.args.withHooks)
+        _append_to_gitignore()
         wpe_util.overwrite_copy(
             osp.join(self.pathMan.templatesDir, '.wpe'),
             osp.join(self.pathMan.configDir)
         )
 
     @HookProcessor().register('premake')
     def premake(self):
         logging.info('Premake project')
         platforms = set([plt.platform for plt in self.targetPlatforms])
         for plt in platforms:
             self.wpWrapper.premake(plt)
 
     @HookProcessor().register('generate_parameters')
     def generate_parameters(self):
-        parameter_manager = ParameterGenerator(self.pathMan, is_forced=self.args.force)
+        def clear_existing_doc():
+            util.remove_tree(self.pathMan.docsDir)
+            util.remove_tree(self.pathMan.htmlDocsDir)
+        clear_existing_doc()
+        parameter_manager = ParameterGenerator(self.pathMan,
+                                               is_forced=self.args.force,
+                                               generate_gui_resource=self.args.gui)
         parameter_manager.main()
         self.wpWrapper.build('Documentation')
 
     @HookProcessor().register('build')
     def build(self):
         self._terminate_wwise()
         self._build()
         self._reopen_wwise()
 
+    @HookProcessor().register('test')
+    def test(self):
+        # self.args.configuration = 'Release'
+        # self.targetPlatforms = [PlatformTarget({
+        #     'platform': 'Windows_vc160',
+        #     'architectures': ['x64'],
+        # })]
+        # self.build()
+        TestRunner.create_platform(self.pathMan).main()
+
     @HookProcessor().register('pack')
     def pack(self):
         def _collect_packages(_output_dir):
             util.remove_tree(_output_dir)
             for pkg in glob.iglob(osp.join(self.pathMan.root, f'{self.pathMan.pluginName}*.tar.xz')):
                 util.move_file(pkg, _output_dir, isdstdir=True)
             util.move_file(osp.join(self.pathMan.root, 'bundle.json'), _output_dir, isdstdir=True)
@@ -133,16 +173,16 @@
         version_code, build_number = self.wpWrapper.wwiseVersion.rsplit('.', 1)
         build_number = self.projConfig.version()
 
         plugin_version = f'{version_code}.{build_number}'
         output_dir = osp.join(self.pathMan.distDir, f'{self.pathMan.pluginName}_v{version_code}_Build{build_number}')
         self.wpWrapper.package('Common', '-v', plugin_version)
         self.wpWrapper.package('Documentation', '-v', plugin_version)
-        for plt in self.targetPlatforms:
-            self.wpWrapper.package(plt.platform, '-v', plugin_version)
+        for plt in self.projConfig.all_platforms():
+            self.wpWrapper.package(plt, '-v', plugin_version)
         self.wpWrapper.generate_bundle('-v', plugin_version)
         _collect_packages(output_dir)
         _zip_bundle(output_dir)
         logging.info(f'Saved to {output_dir}')
 
     def full_pack(self):
         HookProcessor().process_pre_hook('build')
@@ -160,14 +200,24 @@
 
     @HookProcessor().register('bump')
     def bump(self):
         logging.info('Bump wpe project version')
         self.projConfig.bump()
         logging.info(f'Version bumped to {self.projConfig.version()}')
 
+    @HookProcessor().register('rename')
+    def rename(self):
+        logging.info(f'Rename plugin from {self.pathMan.pluginName} to {self.args.rename}.')
+        res = input('Commit your changes before renaming is recommended. Continue? [y/n]') == 'y'
+        if not res:
+            return
+        Renamer(self.args.rename, self.pathMan, self.projConfig).main()
+        self.premake()
+        logging.info('Rename completed, check your changes with git status.')
+
     def _build(self):
         logging.info('Build plugin')
         for plt in self.targetPlatforms:
             args = [plt.platform, '-c', self.args.configuration, '-x'] + plt.architectures
             if plt.need_toolset():
                 args.extend(['-t', plt.toolset()])
             self.wpWrapper.build(*args)
```

### Comparing `wp_enhanced-0.8.9/src/wpe/hook_processor.py` & `wp_enhanced-0.9.0/src/wpe/hook_processor.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/parameter.py` & `wp_enhanced-0.9.0/src/wpe/parameter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,151 @@
 import copy
-import logging
-import os.path as osp
 from typing import Any, Optional
 from dataclasses import dataclass, field
 import xml.etree.ElementTree as ET
+from collections import OrderedDict
 
-import kkpyutil as util
 
 # project
 from wpe.util import *
 from wpe.project_config import ProjectConfig, PluginInfo
 
 _type_prefix_map = {
     'float': 'f',
     'int': 'i',
+    'uint': 'u',
     'bool': 'b',
 }
 
 _wwise_type_name_map = {
     'float': 'AkReal32',
     'int': 'AkInt32',
+    'uint': 'AkUInt32',
     'bool': 'bool',
 }
 
 _xml_type_name_map = {
     'float': 'Real32',
     'int': 'int32',
+    'uint': 'Uint32',
     'bool': 'bool',
 }
 
+_supported_rtpc_types = {'Additive', 'Multiplicative', 'Exclusive', 'Boolean'}
 
-def auto_add_line_end(lines: list[str]):
-    for i, line in enumerate(lines):
-        if not line.endswith('\n'):
-            lines[i] += '\n'
-    return lines
+
+@dataclass
+class InnerType:
+    name: str
+    fields: list['Parameter']
+
+    def __post_init__(self):
+        self.structName = util.convert_compound_cases(self.name)
+
+    @staticmethod
+    def create(name, dict_define: dict[str, Any]):
+        instance = InnerType(
+            name=name,
+            fields=[Parameter.create(name, defines) for name, defines in dict_define.items()],
+        )
+        return instance
+
+    def generate_struct_defines(self):
+        return f'''struct {self.structName}
+{{
+    {self.__generate_field_lines()}
+}};'''
+
+    def __generate_field_lines(self):
+        lines = []
+        for type_field in self.fields:
+            type_field.generate_names()
+            lines.append(type_field.generate_declaration())
+        return '\n    '.join(lines)
 
 
 @dataclass
 class Parameter:
     name: str
     type_: str
-    rtpc: bool
+    rtpc_type: str
     defaultValue: Any
     minValue: Any
     maxValue: Any
+    data_meaning: str = ''
     description: list[dict] = field(default_factory=list)
     dependencies: list[dict] = field(default_factory=list)
     displayName: str = ''
     enumeration: list[dict] = field(default_factory=list)
     userInterface: dict = field(default_factory=dict)
     id: int = 0
+    parent: Optional[InnerType] = None
+    basename: str = ''
+    suffix: str = ''
 
     def __post_init__(self):
+        if self.type_ not in _wwise_type_name_map:
+            raise ValueError(f'Unsupported type: {self.type_} in parameter "{self.name}". Expected one of {_wwise_type_name_map.keys()}.')
+
+        if self.rtpc_type and self.rtpc_type not in _supported_rtpc_types:
+            raise ValueError(f'Unsupported rtpc type: {self.rtpc_type} in parameter "{self.name}". Expected one of {_supported_rtpc_types}.')
+
+    def generate_names(self):
         if self.type_ == 'bool':
             self.defaultValue = str(self.defaultValue).lower()
             self.minValue = 'false'
             self.maxValue = 'true'
         self.propertyName = util.convert_compound_cases(self.name)
-        self.cppVariableName = _type_prefix_map[self.type_] + self.propertyName
+        self.cppVariableName = _type_prefix_map[self.type_] + util.convert_compound_cases(self.basename or self.propertyName)
         self.paramIDName = f'PARAM_{self.name.upper()}_ID'
         self.typeName = _wwise_type_name_map[self.type_]
         self.xmlTypeName = _xml_type_name_map[self.type_]
-        self.struct = 'RTPC' if self.rtpc else 'NonRTPC'
+        self.struct = 'InnerType' if self.parent else ('RTPC' if self.rtpc_type else 'NonRTPC')
         self.displayName = self.displayName or util.convert_compound_cases(self.name, style='title')
+        self.nameSpace = f'{self.struct}.{self.parent.name}{self.suffix}' if self.parent else self.struct
 
     def assign_id(self, _id: int):
         self.id = _id
 
     @staticmethod
     def create(name, dict_define: dict[str, Any]):
         return Parameter(
             name=name,
             type_=dict_define['type'],
-            rtpc=dict_define['rtpc'],
+            rtpc_type=dict_define.get('rtpc_type', 'Exclusive' if dict_define.get('rtpc') else ''),
             defaultValue=dict_define['default_value'],
             minValue=dict_define.get('min_value', None),
             maxValue=dict_define.get('max_value', None),
+            data_meaning=dict_define.get('data_meaning', ''),
             description=dict_define.get('description', []),
-            dependencies=dict_define.get('dependencies', []),
+            dependencies=copy.deepcopy(dict_define.get('dependencies', [])),
             displayName=dict_define.get('display_name', ''),
             enumeration=dict_define.get('enumeration', []),
             userInterface=dict_define.get('user_interface', '')
         )
 
     def generate_param_id(self) -> str:
         return f'static constexpr AkPluginParamID {self.paramIDName} = {self.id};'
 
     def generate_declaration(self) -> str:
+        if self.parent:
+            return f'{self.parent.structName} {self.parent.name}{self.suffix};'
         return f'{self.typeName} {self.cppVariableName};'
 
     def generate_init(self) -> str:
-        return f'{self.struct}.{self.cppVariableName} = {self.defaultValue};'
+        return f'{self.nameSpace}.{self.cppVariableName} = {self.defaultValue};'
 
     def generate_read_bank_data(self) -> str:
-        return f'{self.struct}.{self.cppVariableName} = READBANKDATA({self.typeName}, pParamsBlock, in_ulBlockSize);'
+        return f'{self.nameSpace}.{self.cppVariableName} = READBANKDATA({self.typeName}, pParamsBlock, in_ulBlockSize);'
 
     def generate_set_parameter(self) -> str:
-        need_reinterpret = self.typeName != 'AkReal32' and self.rtpc
+        need_reinterpret = self.typeName != 'AkReal32' and bool(self.rtpc_type)
         interpret_pointer = f'static_cast<{self.typeName}>(*(AkReal32*)in_pValue)' if need_reinterpret else f'*(({self.typeName}*)in_pValue)'
         return f'''    case {self.paramIDName}:
-        {self.struct}.{self.cppVariableName} = {interpret_pointer};
+        {self.nameSpace}.{self.cppVariableName} = {interpret_pointer};
         m_paramChangeHandler.SetParamChange({self.paramIDName});
         break;'''
 
     def generate_property_name_declaration(self) -> str:
         return f'extern const char* const sz{self.propertyName};'
 
     def generate_property_name_definition(self) -> str:
@@ -136,43 +177,48 @@
                     range_.attrib['Type'] = dep['obj'].xmlTypeName
                     min_value = ET.SubElement(range_, 'Min')
                     min_value.text = str(dep['min'])
                     max_value = ET.SubElement(range_, 'Max')
                     max_value.text = str(dep['max'])
             ET.indent(dependencies_element)
             return '\n' + ET.tostring(dependencies_element).decode(util.TXT_CODEC)
-        support_rtpc_type = 'SupportRTPCType="Exclusive"' if self.rtpc else ''
+        support_rtpc_type = f'SupportRTPCType="{self.rtpc_type}"' if self.rtpc_type else ''
+        data_meaning = f'DataMeaning="{self.data_meaning}"' if self.data_meaning else ''
 
         def _generate_bool_gui_lines():
-            return f'''<Property Name="{self.propertyName}" Type="{self.xmlTypeName}" {support_rtpc_type} DisplayName="{self.displayName}">
+            return f'''<Property Name="{self.propertyName}" Type="{self.xmlTypeName}" {support_rtpc_type} {data_meaning} DisplayName="{self.displayName}">
   <DefaultValue>{self.defaultValue}</DefaultValue>
   <AudioEnginePropertyID>{self.id}</AudioEnginePropertyID>{_generate_dependencies()}
 </Property>'''.splitlines()
 
         def _generate_int_gui_lines():
             user_interface = self.userInterface
             if not self.enumeration:
-                raise ValueError(f'Parameter "{self.name}" is int type but no enumeration provided. Please provide enumeration field with string list.')
+                return f'''<Property Name="{self.propertyName}" Type="{self.xmlTypeName}" {support_rtpc_type} {data_meaning} DisplayName="{self.displayName}">
+                  <UserInterface {user_interface} />
+                  <DefaultValue>{self.defaultValue}</DefaultValue>
+                  <AudioEnginePropertyID>{self.id}</AudioEnginePropertyID>
+                </Property>'''.splitlines()
             options = '\n        '.join(['<Value DisplayName="{}">{}</Value>'.format(opt['displayName'], opt['value']) for opt in self.enumeration])
-            return f'''<Property Name="{self.propertyName}" Type="{self.xmlTypeName}" {support_rtpc_type} DisplayName="{self.displayName}">
+            return f'''<Property Name="{self.propertyName}" Type="{self.xmlTypeName}" {support_rtpc_type} {data_meaning} DisplayName="{self.displayName}">
   <UserInterface {user_interface} />
   <DefaultValue>{self.defaultValue}</DefaultValue>
   <AudioEnginePropertyID>{self.id}</AudioEnginePropertyID>
   <Restrictions>
     <ValueRestriction>
       <Enumeration Type="{self.xmlTypeName}"> 
         {options}
       </Enumeration>
     </ValueRestriction>
   </Restrictions>{_generate_dependencies()}
 </Property>'''.splitlines()
 
         def _generate_float_gui_lines():
             user_interface = self.userInterface or f'Step="0.1" Fine="0.001" Decimals="3" UIMax="{self.maxValue}"'
-            return f'''<Property Name="{self.propertyName}" Type="{self.xmlTypeName}" {support_rtpc_type} DisplayName="{self.displayName}">
+            return f'''<Property Name="{self.propertyName}" Type="{self.xmlTypeName}" {support_rtpc_type} {data_meaning} DisplayName="{self.displayName}">
   <UserInterface {user_interface} />
   <DefaultValue>{self.defaultValue}</DefaultValue>
   <AudioEnginePropertyID>{self.id}</AudioEnginePropertyID>
   <Restrictions>
     <ValueRestriction>
       <Range Type="{self.xmlTypeName}">
         <Min>{self.minValue}</Min>
@@ -181,15 +227,15 @@
     </ValueRestriction>
   </Restrictions>{_generate_dependencies()}
 </Property>'''.splitlines()
 
         if self.type_ == 'bool':
             return _generate_bool_gui_lines()
 
-        if self.type_ == 'int':
+        if self.type_ == 'int' or self.type_ == 'uint':
             return _generate_int_gui_lines()
 
         if self.type_ == 'float':
             return _generate_float_gui_lines()
 
         raise NotImplementedError(f'Parameter type "{self.type_}" not supported.')
 
@@ -199,19 +245,40 @@
             doc_str = f'''##{self.displayName}
 
 {lang['text']}
 
 Range: {self.minValue} - {self.maxValue} <br/>'''
             util.save_text(output_path, doc_str)
 
+    def generate_win32_controls(self) -> list[str]:
+        row_height = 18
+        vertical_pos = row_height * self.id + 6
+        title = f'LTEXT "{self.displayName}",IDC_STATIC,0,{vertical_pos + 2},48,10'
+        control_pos = f'48,{vertical_pos},64,12'
+        if self.type_ == 'bool':
+            control = f'CONTROL "{self.propertyName}",IDC_{self.propertyName},"Button",BS_AUTOCHECKBOX | WS_TABSTOP,' + control_pos
+        elif self.type_ == 'int':
+            if self.enumeration:
+                options = ', '.join([f'{opt["value"]}:{opt["displayName"]}' for opt in self.enumeration])
+                control = f'LTEXT "Class=Combo;Prop={self.propertyName};Options={options}",IDC_{self.propertyName},' + control_pos
+            else:
+                control = f'LTEXT "Class=Spinner;Prop={self.propertyName};Min={self.minValue};Max={self.maxValue}",IDC_{self.propertyName},' + control_pos
+        elif self.type_ == 'float':
+            control = f'LTEXT "Class=SuperRange;Prop={self.propertyName}",IDC_{self.propertyName},' + control_pos
+        else:
+            raise ValueError(f'Unknown type: {self.type_}')
+        return [title, control]
+
 
 class ParameterGenerator:
-    def __init__(self, path_man, is_forced=False):
+    def __init__(self, path_man, is_forced=False, generate_gui_resource=False):
         self.pathMan = path_man
         self.isForced = is_forced
+        self.generateGuiResource = generate_gui_resource
+        self.innerTypes: dict[str, InnerType] = {}
         self.parameters: dict[str, Parameter] = {}
         self.pluginInfo: Optional[PluginInfo] = None
 
     def main(self):
         self.load_parameter_config()
         self._generate()
 
@@ -224,137 +291,144 @@
         # load parameters
         if not proj_config.has_parameters():
             return
         for name, define in proj_config.parameter_defines().items():
             self.parameters[name] = Parameter.create(name, define)
         for instance in proj_config.parameter_from_templates():
             self.__load_with_template(instance, proj_config.parameter_templates())
+        self.innerTypes = {name: InnerType.create(name, dict_define) for name, dict_define in proj_config.parameter_inner_types().items()}
         for instance in proj_config.parameter_from_inner_types():
-            self.__load_with_inner_type(instance, proj_config.parameter_inner_types())
-        # link parameter dependency
+            self.__load_with_inner_type(instance)
+
         for i, param in enumerate(self.parameters.values()):
             param.assign_id(i)
+            param.generate_names()
+            # link parameter dependency
             for dep in param.dependencies:
                 dep['obj'] = self.parameters[dep['name']]
 
     def _generate(self):
-        def _copy_template(relative):
-            def _need_overwrite(_dst):
-                if self.isForced:
-                    return True
-                if osp.isfile(_dst):
-                    content = util.load_text(_dst)
-                    return '[wp-enhanced template]' not in content
-                return True
-
-            src = osp.join(self.pathMan.templatesDir, relative)
-            dst = replace_in_basename(osp.join(self.pathMan.root, relative), 'ProjectName', self.pathMan.pluginName)
-            if not _need_overwrite(dst):
-                logging.info(f'Skip copying template "{osp.basename(src)}". Use -f to force overwrite.')
-                return dst
-            if osp.isfile(src):
-                overwrite_copy(src, dst)
-                util.substitute_keywords_in_file(dst,
-                                                 {
-                                                     'name': self.pathMan.pluginName,
-                                                     'display_name': self.pathMan.pluginName,
-                                                     'plugin_id': self.pathMan.pluginId,
-                                                 })
-                return dst
-            else:
-                raise FileNotFoundError(f'File not found: {src}')
-
         def _generate_fx_params_h():
             target = 'SoundEnginePlugin/ProjectNameFXParams.h'
-            dst = _copy_template(target)
+            dst = copy_template(target, self.pathMan, self.isForced)
             util.substitute_lines_in_file(self.__generate_ids(), dst, '// [ParameterID]', '// [/ParameterID]')
-            util.substitute_lines_in_file(self.__generate_declarations(rtpc=True), dst, '// [RTPCDeclaration]',
+            util.substitute_lines_in_file(self.__generate_inner_types(), dst, '// [InnerTypes]', '// [/InnerTypes]')
+            util.substitute_lines_in_file(self.__generate_declarations(struct='InnerType'), dst, '// [InnerTypeDeclaration]',
+                                          '// [/InnerTypeDeclaration]')
+            util.substitute_lines_in_file(self.__generate_declarations(struct='RTPC'), dst, '// [RTPCDeclaration]',
                                           '// [/RTPCDeclaration]')
-            util.substitute_lines_in_file(self.__generate_declarations(rtpc=False), dst, '// [NonRTPCDeclaration]',
+            util.substitute_lines_in_file(self.__generate_declarations(struct='NonRTPC'), dst, '// [NonRTPCDeclaration]',
                                           '// [/NonRTPCDeclaration]')
 
         def _generate_fx_params_cpp():
             target = 'SoundEnginePlugin/ProjectNameFXParams.cpp'
-            dst = _copy_template(target)
+            dst = copy_template(target, self.pathMan, self.isForced)
             util.substitute_lines_in_file(self.__generate_init(), dst, '// [ParameterInitialization]',
                                           '// [/ParameterInitialization]')
             util.substitute_lines_in_file(self.__generate_read_bank_data(), dst, '// [ReadBankData]',
                                           '// [/ReadBankData]')
             util.substitute_lines_in_file(self.__generate_set_parameter(), dst, '// [SetParameters]',
                                           '// [/SetParameters]', withindent=False)
 
         def _generate_wwise_plugin_h():
             target = 'WwisePlugin/ProjectNamePlugin.h'
-            dst = _copy_template(target)
+            dst = copy_template(target, self.pathMan, self.isForced)
             util.substitute_lines_in_file(self.__generate_property_name_declaration(), dst, '// [PropertyNames]',
                                           '// [/PropertyNames]')
 
         def _generate_wwise_plugin_cpp():
             target = 'WwisePlugin/ProjectNamePlugin.cpp'
-            dst = _copy_template(target)
+            dst = copy_template(target, self.pathMan, self.isForced)
             util.substitute_lines_in_file(self.__generate_property_name_definition(), dst, '// [PropertyNames]',
                                           '// [/PropertyNames]')
             util.substitute_lines_in_file(self.__generate_write_bank_data(), dst, '// [WriteBankData]',
                                           '// [/WriteBankData]')
 
         def _generate_wwise_xml():
             target = 'WwisePlugin/ProjectName.xml'
-            dst = _copy_template(target)
+            dst = copy_template(target, self.pathMan, self.isForced)
             util.substitute_lines_in_file(self.__generate_parameter_gui(), dst, '<!-- [ParameterGui] -->',
                                           '<!-- [/ParameterGui] -->')
             util.substitute_lines_in_file(self.__generate_platform_support(), dst, '<!-- [PlatformSupport] -->',
                                           '<!-- [/PlatformSupport] -->')
+            util.substitute_lines_in_file(self.__generate_plugin_info(), dst, '<!-- [PluginInfo] -->',
+                                          '<!-- [/PluginInfo] -->')
 
         def _generate_doc():
             for param in self.parameters.values():
                 param.dump_parameter_doc(self.pathMan.docsDir)
 
+        def _generate_win32_gui_resource():
+            target = 'WwisePlugin/ProjectName.rc'
+            dst = copy_template(target, self.pathMan, self.isForced)
+            util.substitute_lines_in_file(self.__generate_win32_controls(), dst, '// [Controls]', '// [/Controls]')
+            target = 'WwisePlugin/resource.h'
+            dst = copy_template(target, self.pathMan, self.isForced)
+            util.substitute_lines_in_file(self.__generate_win32_idc(), dst, '// [IDC]', '// [/IDC]')
+            target = 'WwisePlugin/Win32/ProjectNamePluginGUI.cpp'
+            dst = copy_template(target, self.pathMan, self.isForced)
+            util.substitute_lines_in_file(self.__generate_win32_property_table(), dst, '// [PropertyTable]', '// [/PropertyTable]')
+
         _generate_fx_params_h()
         _generate_fx_params_cpp()
         _generate_wwise_plugin_h()
         _generate_wwise_plugin_cpp()
         _generate_wwise_xml()
         _generate_doc()
+        if self.generateGuiResource:
+            _generate_win32_gui_resource()
 
     def __generate_ids(self):
         lines = []
         for i, param in enumerate(self.parameters.values()):
             lines.append(param.generate_param_id())
         lines.append(f'static constexpr AkUInt32 NUM_PARAMS = {len(self.parameters)};')
         return auto_add_line_end(lines)
 
+    def __generate_inner_types(self):
+        lines = []
+        for i, inner_type in enumerate(self.innerTypes.values()):
+            lines.append(inner_type.generate_struct_defines())
+        return auto_add_line_end(lines)
+
     def __load_with_template(self, instance, templates):
         template = copy.deepcopy(templates[instance['template']])
         for key, value in instance.get('override', {}).items():
             template[key] = value
         for dep in template.get('dependencies', []):
             dep['name'] = dep['name'] % {'suffix': instance['suffix']}
 
         name = f"{instance['template']}_{instance['suffix']}"
         self.parameters[name] = Parameter.create(name, template)
 
-    def __load_with_inner_type(self, instance, inner_types):
-        inner_type = inner_types[instance['inner_type']]
-        overrides = instance.get('overrides', {})
-
-        for field_name, template in inner_type.items():
-            template = copy.deepcopy(template)
+    def __load_with_inner_type(self, define):
+        inner_type = self.innerTypes[define['inner_type']]
+        overrides = define.get('overrides', {})
+
+        for type_field in inner_type.fields:
+            field_name = type_field.name
+            instance = copy.deepcopy(type_field)
             if field_name in overrides:
-                template['default_value'] = overrides[field_name]
-            for dep in template.get('dependencies', []):
-                dep['name'] = f"{instance['inner_type']}_{dep['name'] % {'suffix': instance['suffix']}}"
-
-            name = f"{instance['inner_type']}_{field_name}_{instance['suffix']}"
-            self.parameters[name] = Parameter.create(name, template)
+                instance.defaultValue = overrides[field_name]
+            for dep in instance.dependencies:
+                dep['name'] = f"{inner_type.name}_{dep['name'] % {'suffix': define['suffix']}}"
+
+            instance.name = f"{inner_type.name}_{field_name}_{define['suffix']}"
+            instance.basename = field_name
+            instance.parent = inner_type
+            instance.suffix = define['suffix']
+            self.parameters[instance.name] = instance
 
-    def __generate_declarations(self, rtpc=True):
+    def __generate_declarations(self, struct):
         lines = []
         for param in self.parameters.values():
-            if param.rtpc == rtpc:
+            if param.struct == struct:
                 lines.append(param.generate_declaration())
+        # remove duplicate lines(when inner type is used)
+        lines = list(OrderedDict.fromkeys(lines).keys())
         return auto_add_line_end(lines)
 
     def __generate_init(self):
         lines = []
         for param in self.parameters.values():
             lines.append(param.generate_init())
         return auto_add_line_end(lines)
@@ -392,8 +466,32 @@
     def __generate_parameter_gui(self):
         lines = []
         for param in self.parameters.values():
             lines.extend(param.generate_parameter_gui())
         return auto_add_line_end(lines)
 
     def __generate_platform_support(self):
+        logging.warning('Deprecated tag: "PlatformSupport", please migrate to "PluginInfo" instead.')
         return auto_add_line_end(self.pluginInfo.generate_platform_support())
+
+    def __generate_plugin_info(self):
+        return auto_add_line_end(self.pluginInfo.generate_plugin_info())
+
+    def __generate_win32_controls(self):
+        lines = []
+        for param in self.parameters.values():
+            lines.extend(param.generate_win32_controls())
+        return auto_add_line_end(lines)
+
+    def __generate_win32_idc(self):
+        lines = []
+        for i, param in enumerate(self.parameters.values()):
+            lines.append(f'#define IDC_{param.propertyName} {i + 1001}')
+        return auto_add_line_end(lines)
+
+    def __generate_win32_property_table(self):
+        lines = []
+        for param in self.parameters.values():
+            if param.type_ != 'bool':
+                continue
+            lines.append(f'    AK_WWISE_PLUGIN_GUI_WINDOWS_POP_ITEM(IDC_{param.propertyName}, sz{param.propertyName})')
+        return auto_add_line_end(lines)
```

### Comparing `wp_enhanced-0.8.9/src/wpe/pathman.py` & `wp_enhanced-0.9.0/src/wpe/pathman.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 
 import kkpyutil as util
 
 
 class PathMan:
     def __init__(self, cwd=None):
         self.templatesDir = osp.join(osp.dirname(__file__), 'templates')
+        self.testUtilDir = osp.join(osp.dirname(__file__), 'test', 'util')
         self.premakePluginLua = self.find_premake_plugin_lua_in_ancestor_and_update_root(cwd or os.getcwd())
         self.root = osp.dirname(self.premakePluginLua)
         os.chdir(self.root)
         self.pluginName = self.parse_plugin_name()
         self.pluginConfigHeader = osp.join(self.root, f'{self.pluginName}Config.h')
         self.pluginId = self.parse_plugin_id()
         self.configDir = osp.join(self.root, '.wpe')
         self.projConfig = osp.join(self.configDir, 'wpe_project.toml')
         # compatible with old version
         self.parameterConfig = osp.join(self.configDir, 'wpe_parameters.toml')
         self.docsDir = osp.join(self.root, 'WwisePlugin/res/Md')
+        self.htmlDocsDir = osp.join(self.root, 'WwisePlugin/res/Html')
         self.distDir = osp.join(self.root, 'dist')
+        self.testDir = osp.join(self.root, 'test')
         self.hooksDir = osp.join(self.configDir, 'hooks')
 
     @staticmethod
     def find_premake_plugin_lua_in_ancestor_and_update_root(cwd):
         premake_script_filename = 'PremakePlugin.lua'
         while cwd:
             lua = osp.join(cwd, premake_script_filename)
@@ -46,7 +49,10 @@
     def parse_plugin_id(self):
         lines = util.load_lines(self.pluginConfigHeader, rmlineend=True)
         prefix = '    static const unsigned short PluginID = '
         name_define_pattern = rf'{prefix}\d+'
         for line in lines:
             if matched := re.match(name_define_pattern, line):
                 return int(matched.group().lstrip(prefix))
+
+    def refresh_paths(self, cwd=None):
+        self.__init__(cwd)
```

### Comparing `wp_enhanced-0.8.9/src/wpe/project_config.py` & `wp_enhanced-0.9.0/src/wpe/wp_wrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import logging
+import os
 import os.path as osp
 import platform
 
 import kkpyutil as util
 
-# project
-from wpe.util import *
-from wpe.pathman import PathMan
-
-
-class PluginInfo:
-    def __init__(self, info_dict: dict):
-        self.infoDict = info_dict
-        self.defaultPlatformSupport = '''<Platform Name="Any">
-  <CanBeInsertOnBusses>true</CanBeInsertOnBusses>
-  <CanBeInsertOnAudioObjects>true</CanBeInsertOnAudioObjects>
-  <CanBeRendered>true</CanBeRendered>
-</Platform>'''
-
-    def generate_platform_support(self) -> list[str]:
-        if not self.infoDict['platform_support']:
-            return self.defaultPlatformSupport.splitlines()
-        lines = []
-        for platform, config in self.infoDict['platform_support'].items():
-            lines.append(f'<Platform Name="{platform}">')
-            for key, value in config.items():
-                lines.append(f'  <{key}>{str(value).lower()}</{key}>')
-            lines.append('</Platform>')
-        return lines
-
-
-class PlatformTarget:
-    def __init__(self, target_dict: dict):
-        self.targetDict = target_dict
-        self.platform: str = target_dict['platform']
-        self.architectures: list[str] = target_dict['architectures']
-
-    def is_windows(self) -> bool:
-        return self.platform.startswith('Windows')
-
-    def is_authoring(self) -> bool:
-        return self.platform == 'Authoring'
-
-    def need_toolset(self) -> bool:
-        return self.is_windows() or self.is_authoring()
-
-    def toolset(self):
-        if ts := self.targetDict.get('toolset'):
-            return ts
-        return self.platform.split('_')[1] if self.is_windows() else None
-
-
-class ProjectConfig:
-    def __init__(self, path_man: PathMan):
-        self.pathMan = path_man
-        self.config = None
-        self.load()
-
-    def load(self):
-        if osp.isfile(self.pathMan.projConfig):
-            self.config = load_toml(self.pathMan.projConfig)
-            return
-
-        if osp.isfile(self.pathMan.parameterConfig):
-            self.config = load_toml(self.pathMan.parameterConfig)
-            logging.warning('wpe_parameters.toml is deprecated. Please rename it to wpe_project.toml.')
-            return
-
-        raise FileNotFoundError(f'wpe project config not found: {self.pathMan.projConfig}')
-
-    def bump(self):
-        new_version = self.version() + 1
-        config_lines = util.load_lines(self.pathMan.projConfig)
-        for i, line in enumerate(config_lines):
-            if line.startswith('version = '):
-                config_lines[i] = f'version = {new_version}\n'
-                break
-        util.save_lines(self.pathMan.projConfig, config_lines)
-        self.load()
-
-    def target_platforms(self) -> list[PlatformTarget]:
-        platform_targets_key = 'win_targets' if platform.system() == 'Windows' else 'mac_targets'
-        return [PlatformTarget(target) for target in self.config['project'][platform_targets_key]]
-
-    def plugin_info(self) -> PluginInfo:
-        return PluginInfo(self.config['plugin_info'])
-
-    def has_parameters(self) -> bool:
-        return 'parameters' in self.config
-
-    def parameter_defines(self) -> dict:
-        return self.config['parameters'].get('defines', {})
-
-    def parameter_templates(self) -> dict:
-        return self.config['parameters'].get('templates', {})
-
-    def parameter_inner_types(self) -> dict:
-        return self.config['parameters'].get('inner_types', {})
 
-    def parameter_from_templates(self) -> list:
-        return self.config['parameters'].get('from_templates', [])
-
-    def parameter_from_inner_types(self) -> list:
-        return self.config['parameters'].get('from_inner_types', [])
-
-    def version(self) -> int:
-        return self.config['project']['version']
+def create_sdk_symlink(wwise_sdk):
+    temp_sdk_dir = 'C:\\temp\\wpe\\WWISESDK' if platform.system() == 'Windows' else osp.expanduser(
+        '~/temp/wpe/WWISESDK')
+    if osp.exists(temp_sdk_dir):
+        if osp.islink(temp_sdk_dir):
+            os.remove(temp_sdk_dir)
+        else:
+            raise FileExistsError(f'{temp_sdk_dir} exists and is not a symlink to WWISESDK')
+    os.makedirs(osp.dirname(temp_sdk_dir), exist_ok=True)
+    os.symlink(wwise_sdk, temp_sdk_dir)
+    return temp_sdk_dir
+
+
+def inject_wwise_sdk_for_android(func):
+    def wrapper(*args, **kwargs):
+        plt = args[0] if args else ''
+        if plt != 'Android':
+            return func(*args, **kwargs)
+        org_sdk_dir = os.getenv('WWISESDK')
+        temp_sdk_dir = create_sdk_symlink(org_sdk_dir)
+        os.environ['WWISESDK'] = temp_sdk_dir
+        res = func(*args, **kwargs)
+        os.environ['WWISESDK'] = org_sdk_dir
+        return res
+    return wrapper
+
+
+class WpWrapper:
+    def __init__(self):
+        self.wwiseRoot: str = os.getenv('WWISEROOT')
+        self.wwiseSDKRoot: str = os.getenv('WWISESDK')
+        self.wwiseVersion: str = self._load_wwise_version()
+        self.wpScriptDir = osp.join(self.wwiseRoot, 'Scripts/Build/Plugins')
+        util.lazy_prepend_sys_path([self.wpScriptDir])
+
+        self.subcommands = (
+            'build',
+            'generate_bundle',
+            'new',
+            'package',
+            'premake',
+        )
+
+    def _load_wwise_version(self) -> str:
+        install_entry = util.load_json(osp.join(self.wwiseRoot, 'install-entry.json'))
+        version = install_entry['bundle']['version']
+        return f'{version["year"]}.{version["major"]}.{version["minor"]}.{version["build"]}'
+
+    def validate_env(self):
+        if self.wwiseRoot is None:
+            raise EnvironmentError(f'Unknown env variable: WWISEROOT\n  - Try setting environment variables in Wwise '
+                                   f'Launcher')
+
+        if self.wwiseSDKRoot is None:
+            raise EnvironmentError(f'Unknown env variable: WWISESDK\n  - Try setting environment variables in Wwise '
+                                   f'Launcher')
+
+        if not osp.isfile((wp := osp.join(self.wpScriptDir, 'wp.py'))):
+            raise FileNotFoundError(f'"{wp}" not found.')
+
+        for subcommand in self.subcommands:
+            if not osp.isfile((subcommand_file := osp.join(self.wpScriptDir, f'{subcommand}.py'))):
+                raise FileNotFoundError(f'Subcommand "{subcommand_file}" not found.')
+
+    def wp(self, args):
+        subcommand = args[0]
+        if subcommand not in self.subcommands:
+            raise ValueError(f'Unknown subcommand: {subcommand}')
+        return self.run(subcommand, *args[1:])
+
+    @staticmethod
+    @inject_wwise_sdk_for_android
+    def build(*args):
+        import wpe.wp_patch.build as wpe_build
+        res = wpe_build.run(args)
+        if res != 0:
+            raise RuntimeError(f'Build failed. Exit code: {res}')
+        return res
+
+    def generate_bundle(self, *args):
+        return self.run('generate_bundle', *args)
+
+    def new(self, *args):
+        return self.run('new', *args)
+
+    @staticmethod
+    def package(*args):
+        import wpe.wp_patch.package as wpe_package
+        res = wpe_package.run(args)
+        return res
+
+    @staticmethod
+    @inject_wwise_sdk_for_android
+    def premake(*args):
+        import wpe.wp_patch.premake as wpe_premake
+        res = wpe_premake.run(args)
+        return res
+
+    def run(self, subcommand, *args):
+        subcommand_module = util.safe_import_module(osp.basename(subcommand), self.wpScriptDir)
+        return subcommand_module.run(args)
```

### Comparing `wp_enhanced-0.8.9/src/wpe/templates/.wpe/wpe_project.toml` & `wp_enhanced-0.9.0/src/wpe/templates/.wpe/wpe_project.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [project]
 version = 1
-targets = [
+win_targets = [
     { platform = 'Authoring', architectures = ['x64'], toolset = 'vc160' },
     { platform = 'Windows_vc160', architectures = ['x64'] },
     { platform = 'Android', architectures = ['arm64-v8a', 'armeabi-v7a'] },
+]
+mac_targets = [
+    { platform = 'Authoring', architectures = ['universal'] },
     { platform = 'iOS', architectures = ['iOS'] },
 ]
 
-[plugin_info.platform_support]
+[plugin_info]
+MenuPath = 'custom'
+
 [plugin_info.platform_support.Any]
 CanBeInsertOnBusses = true
 CanBeInsertOnAudioObjects = true
 CanBeRendered = true
 
 
 [parameters.defines.bool_param_as_checkbox]
 type = 'bool'
-rtpc = false
 default_value = true
 
 
 [parameters.defines.int_param_as_combo_box] # snake_case_name
 # int/float/bool are supported
 type = 'int'
-rtpc = true
+# Additive/Multiplicative/Exclusive/Boolean are supported
+rtpc_type = 'Exclusive'
 default_value = 0
 
 # Fields below are optional
 # Description displayed in Wwise UI. Refer to: https://www.audiokinetic.com/zh/library/edge/?source=SDK&id=effectplugin_tools_property_help.html
 description = [
     { language = 'en', text = 'This is a description for this parameter' },
     { language = 'zh', text = '这是一个参数的描述' }
@@ -43,15 +48,17 @@
 dependencies = [
     { name = 'bool_param_as_checkbox', condition = 'Enumeration', values = [true] },
 ]
 
 
 [parameters.defines.float_param_as_slider]
 type = 'float'
-rtpc = true
+rtpc_type = 'Exclusive'
+# Optional, Refer to `DataMeaning` section in: https://www.audiokinetic.com/zh/library/edge/?source=SDK&id=plugin_xml_properties.html
+data_meaning = 'Decibels'
 default_value = 0
 min_value = -96
 max_value = 24
 
 description = [
     { language = 'en', text = 'This is a description for this parameter' },
     { language = 'zh', text = '这是一个参数的描述' }
```

### Comparing `wp_enhanced-0.8.9/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp` & `wp_enhanced-0.9.0/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 %(name)sFXParams::~%(name)sFXParams()
 {
 }
 
 %(name)sFXParams::%(name)sFXParams(const %(name)sFXParams& in_rParams)
 {
+    InnerType = in_rParams.InnerType;
     RTPC = in_rParams.RTPC;
     NonRTPC = in_rParams.NonRTPC;
     m_paramChangeHandler.SetAllParamChanges();
 }
 
 AK::IAkPluginParam* %(name)sFXParams::Clone(AK::IAkPluginMemAlloc* in_pAllocator)
 {
```

### Comparing `wp_enhanced-0.8.9/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h` & `wp_enhanced-0.9.0/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,23 @@
 // Add parameters IDs here, those IDs should map to the AudioEnginePropertyID
 // attributes in the xml property definition.
 // [ParameterID]
 static const AkPluginParamID PARAM_PLACEHOLDER_ID = 0;
 static const AkUInt32 NUM_PARAMS = 1;
 // [/ParameterID]
 
+// [InnerTypes]
+// [/InnerTypes]
+
+struct %(name)sInnerTypeParams
+{
+    // [InnerTypeDeclaration]
+    // [/InnerTypeDeclaration]
+};
+
 struct %(name)sRTPCParams
 {
     // [RTPCDeclaration]
     AkReal32 fPlaceholder;
     // [/RTPCDeclaration]
 };
 
@@ -73,14 +82,15 @@
     AKRESULT SetParamsBlock(const void* in_pParamsBlock, AkUInt32 in_ulBlockSize) override;
 
     /// Update a single parameter at a time and perform the necessary actions on the parameter changes.
     AKRESULT SetParam(AkPluginParamID in_paramID, const void* in_pValue, AkUInt32 in_ulParamSize) override;
 
     AK::AkFXParameterChangeHandler<NUM_PARAMS>* GetParamChangeHandler() { return &m_paramChangeHandler; }
 
+    %(name)sInnerTypeParams InnerType;
     %(name)sRTPCParams RTPC;
     %(name)sNonRTPCParams NonRTPC;
 
 private:
     AK::AkFXParameterChangeHandler<NUM_PARAMS> m_paramChangeHandler;
 };
```

### Comparing `wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectName.xml` & `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectName.xml`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp` & `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h` & `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/wp_patch/build.py` & `wp_enhanced-0.9.0/src/wpe/wp_patch/build.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/wp_patch/common/command/android.py` & `wp_enhanced-0.9.0/src/wpe/wp_patch/common/command/android.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/wp_patch/common/platform/android.py` & `wp_enhanced-0.9.0/src/wpe/wp_patch/common/platform/android.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/wp_patch/package.py` & `wp_enhanced-0.9.0/src/wpe/wp_patch/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,21 +36,18 @@
 
 def find_artifacts(args):
     # search for artifacts using the glob patterns
     artifacts_found = []
     artifacts_found_in_project = []
 
     platform_info = platform_registry.get(args.platform)
-    # [wp-enhanced] exclude pdb and debug artifacts
-    debug_artifacts_folders = {'Debug', 'Debug(StaticCRT)', 'Debug-iphoneos', 'Debug-iphonesimulator'}
+    # [wp-enhanced] exclude pdb
     for artifact_glob in (pattern for pattern in platform_info.package.artifacts if not pattern.endswith(".pdb")):
         for artifact in glob(os.path.join(WWISE_ROOT, artifact_glob.format(plugin_name=PLUGIN_NAME))):
             sections = set(artifact.split(os.path.sep))
-            if sections & debug_artifacts_folders:
-                continue
             artifacts_found.append(artifact)
             print("Found {}".format(artifact))
     # [/wp-enhanced]
 
     # validate additional artifacts
     for artifact_glob in args.additional_artifacts:
         artifacts = glob(os.path.join(WWISE_ROOT, os.path.normpath(artifact_glob)))
@@ -126,15 +123,16 @@
         if not args.version:
             exit_with_error("'Version' argument needs to be specified using -v or --version, -h for more details.")
 
         print("Packaging {} for {}...".format(PLUGIN_NAME, platform_info.name))
 
         artifacts_found, artifacts_found_in_project = find_artifacts(args)
         if not artifacts_found and not artifacts_found_in_project:
-            exit_with_error("Nothing to package!")
+            print("Nothing to package!")
+            return 0
 
         formatted_plugin_version = "v{}.{}.{}_Build{}".format(
             args.version.year, args.version.major, args.version.minor, args.version.build)
 
         if is_documentation(platform_info.name):
             formatted_platforms = ["Authoring.{}".format(platform_info.name)]
         elif is_authoring_target(platform_info.name):
```

### Comparing `wp_enhanced-0.8.9/src/wpe/wp_patch/premake.py` & `wp_enhanced-0.9.0/src/wpe/wp_patch/premake.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.9/src/wpe/wp_patch/premakePlugins.lua` & `wp_enhanced-0.9.0/src/wpe/wp_patch/premakePlugins.lua`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,17 @@
 end
 
 function PremakePlugins.CreateAuthoring()
 	local platform = AK.Platform
 	local authoringLocation = AkRelativeToCwd(projectPath) .. "WwisePlugin/"
 	local authoringOutput = AkRelativeToCwd(_AK_WWISE_ROOT .. "Authoring/")
 	local authoringFileName = plugin.name .. "_Authoring_" .. platform.name .. actionsuffix
-	local targetDir = authoringOutput .. "$(Platform)/$(Configuration)/" .. "bin/Plugins"
+-- 	[wp-enhanced patch] Always output to release dir for authoring
+	local targetDir = authoringOutput .. "$(Platform)/Release/" .. "bin/Plugins"
+-- 	[/wp-enhanced patch]
 
 	PremakePlugins.CreateProject(plugin.name, authoringFileName, plugin.authoring, authoringLocation, "SharedLib")
 
 	filter { "system:windows" }
 		for _,cfg in pairs(plugin.configurations) do
 			filter (cfg)
 				targetdir (targetDir)
```

### Comparing `wp_enhanced-0.8.9/PKG-INFO` & `wp_enhanced-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: wp-enhanced
-Version: 0.8.9
+Version: 0.9.0
 Summary: Wrapper of `wp.py`. Easy to premake, build, and deploy wwise plugins.
 Home-page: https://github.com/tgalpha/wp-enhanced
 License: MIT
 Author: tgalpha
 Author-email: tanalpha.zhy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: kkpyutil (>=0.154.6,<0.155.0)
+Requires-Dist: kkpyutil (>=1.33.5,<2.0.0)
+Requires-Dist: lupa (>=2.1,<3.0)
 Requires-Dist: markdown (>=3.4.4,<4.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/tgalpha/wp-enhanced
 Description-Content-Type: text/markdown
 
 # wp-enhanced
 Wrapper of `wp.py`. Easy to premake, build, deploy and distribute wwise plugins.
 
 # Installation
```

