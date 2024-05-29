# Comparing `tmp/reldplayer-0.0.1a2.tar.gz` & `tmp/reldplayer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "reldplayer-0.1.0.tar", max compression
```

## Comparing `reldplayer-0.0.1a2.tar` & `reldplayer-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/.gitattributes
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/.python-version
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/LICENSE
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/requirements.lock
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/__main__.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/autogui.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/console.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/main.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/metaMgr.py
--rw-r--r--   0        0        0    16417 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/rawconsole.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/wndMgr.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/models/__init__.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/models/file.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/utils/screen.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/src/reldplayer/utils/wip.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/.gitignore
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/README.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 reldplayer-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-24 18:23:11.481172 reldplayer-0.1.0/LICENSE
+-rw-r--r--   0        0        0      660 2024-05-29 04:30:53.154679 reldplayer-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      196 2024-05-29 06:36:12.051597 reldplayer-0.1.0/README.md
+-rw-r--r--   0        0        0      133 2024-05-29 06:16:57.355155 reldplayer-0.1.0/src/reldplayer/__init__.py
+-rw-r--r--   0        0        0     5396 2024-05-29 07:32:11.755121 reldplayer-0.1.0/src/reldplayer/core/config.py
+-rw-r--r--   0        0        0      260 2024-05-29 06:33:01.769341 reldplayer-0.1.0/src/reldplayer/core/ctx.py
+-rw-r--r--   0        0        0     4131 2024-05-29 07:08:02.426804 reldplayer-0.1.0/src/reldplayer/core/player.py
+-rw-r--r--   0        0        0    17332 2024-05-29 06:58:10.584313 reldplayer-0.1.0/src/reldplayer/extensions/console.py
+-rw-r--r--   0        0        0     4689 2024-05-29 07:25:44.867782 reldplayer-0.1.0/src/reldplayer/extensions/manage_config.py
+-rw-r--r--   0        0        0     1600 2024-05-29 07:31:29.614717 reldplayer-0.1.0/src/reldplayer/extensions/manage_macro.py
+-rw-r--r--   0        0        0     2665 2024-05-29 07:29:32.088119 reldplayer-0.1.0/src/reldplayer/extensions/manage_window.py
+-rw-r--r--   0        0        0     2213 2024-05-29 07:29:32.083243 reldplayer-0.1.0/src/reldplayer/extensions/window_auto.py
+-rw-r--r--   0        0        0      234 2024-05-29 07:27:24.897770 reldplayer-0.1.0/src/reldplayer/internal/__init__.py
+-rw-r--r--   0        0        0     9140 2024-05-29 06:16:57.497197 reldplayer-0.1.0/src/reldplayer/internal/iconsole.py
+-rw-r--r--   0        0        0     1190 2024-05-29 07:19:26.633455 reldplayer-0.1.0/src/reldplayer/internal/model_config.py
+-rw-r--r--   0        0        0     3938 2024-05-29 06:16:57.449282 reldplayer-0.1.0/src/reldplayer/internal/model_mps.py
+-rw-r--r--   0        0        0     2318 2024-05-29 06:16:57.433803 reldplayer-0.1.0/src/reldplayer/internal/model_profile_config.py
+-rw-r--r--   0        0        0      855 2024-05-29 07:32:17.889778 reldplayer-0.1.0/src/reldplayer/internal/model_record.py
+-rw-r--r--   0        0        0      209 2024-05-29 06:16:57.423889 reldplayer-0.1.0/src/reldplayer/internal/typedicts.py
+-rw-r--r--   0        0        0      140 2024-05-29 06:16:57.434776 reldplayer-0.1.0/src/reldplayer/objs/query.py
+-rw-r--r--   0        0        0     1281 2024-05-29 06:16:57.444826 reldplayer-0.1.0/src/reldplayer/objs/wnd_instance.py
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 reldplayer-0.1.0/PKG-INFO
```

### Comparing `reldplayer-0.0.1a2/LICENSE` & `reldplayer-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `reldplayer-0.0.1a2/src/reldplayer/rawconsole.py` & `reldplayer-0.1.0/src/reldplayer/extensions/console.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,227 +1,201 @@
-
-import os
-import subprocess
+from functools import cached_property
+import json
+from time import sleep
+from zrcl4.subprocess import exec_command as _exec, query, query_raw
 import typing
-from .models import ConsoleInterface, InstanceDict
+import os
+
+from reldplayer.core.ctx import PlayerCtx
+from reldplayer.core.config import PlayerConfig
+from reldplayer.internal.iconsole import IConsole, list_of_id_funcs
+from reldplayer.internal.typedicts import InstanceMeta
+
 
-class Rawconsole(ConsoleInterface):
-    def __init__(self, path : str):
-        if not os.path.exists(path):
-            raise FileNotFoundError
-        
-        if not path.endswith("ldconsole.exe"):
-            raise ValueError("path must end with ldconsole.exe")
-        
-        self.path = path
+class Console(IConsole):
 
-    def __argument_id(self, mnq_name : str, mnq_idx : int, arglist :list):
+    def __init__(self, player, rawconsole: bool = False):
+        self.__rawconsole = rawconsole
+        self.__player = player
+
+    @property
+    def __config(self) -> PlayerConfig:
+        return self.__player._config
+
+    @property
+    def __ctx(self) -> PlayerCtx:
+        if self.__rawconsole:
+            return None
+        return self.__player._ctx
+
+    @cached_property
+    def __ldconsole__(self):
+        return os.path.join(self.__config.path, "ldconsole.exe")
+
+    def __argument_id(
+        self,
+        mnq_name: typing.Optional[str],
+        mnq_idx: typing.Optional[int],
+        arglist: list,
+    ):
         if mnq_name is None and mnq_idx is None:
             raise ValueError("mnq_name and mnq_idx cannot both be None")
 
         if isinstance(mnq_name, int):
             arglist.extend(["--index", str(mnq_name)])
         elif mnq_name is not None:
             arglist.extend(["--name", mnq_name])
         else:
             arglist.extend(["--index", str(mnq_idx)])
 
-    def __argument_check_range(self, value :int, low :int, high :int):
+    def __argument_check_range(self, value: int, low: int, high: int):
         if value < low or value > high:
             raise ValueError(f"value must be between {low} and {high}")
-        
-    # ANCHOR subporcess
-    def _exec(self, *args):
-        """
-        Execute a subprocess with the given arguments.
-
-        Args:
-            *args: Variable length argument list.
-
-        Returns:
-            None
-        """
-        subprocess.Popen( # noqa
-        [self.path, *(str(arg) for arg in args)],
-        stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-        creationflags=
-            subprocess.DETACHED_PROCESS |
-            subprocess.CREATE_NEW_PROCESS_GROUP | 
-            subprocess.CREATE_BREAKAWAY_FROM_JOB
-    )
-
-    def _queryRaw(self, *args, timeout : int = 5):
-        """
-        Executes a raw query using the specified arguments and a timeout.
-
-        Args:
-            *args: Any additional arguments for the query.
-            timeout (int): The maximum time to wait for the query to complete (default is 5).
-
-        Returns:
-            bytes: The output of the query execution.
-        """
-        try:
-            if not len(args):
-                queryed = [self.path]
-            else:
-                queryed = [self.path, *(str(arg) for arg in args)]
-
-            proc : subprocess.CompletedProcess = subprocess.run(
-                queryed,
-                capture_output=True,
-                timeout=timeout
-            )
-            comm : bytes = proc.stdout
 
-        except subprocess.TimeoutExpired as e:
-            raise e
-        except subprocess.CalledProcessError as e:
-            raise e
-        
-        return comm
-    
-    def _query(
-        self, 
-        *args, 
-        timeout: int = 5, 
-        raw: bool = False, 
-        decodeOrder: typing.List[str] = ["utf-8", "gbk"], 
-        toList: bool = False,
-        stripNullLines : bool = False
-    ):
-        """
-        Perform a query with optional parameters for timeout, raw output, return context, decoding order, conversion to list, and stripping null lines.
-
-        Args:
-            *args: Variable length argument list.
-            timeout (int): Timeout duration in seconds (default is 5).
-            raw (bool): Flag to indicate whether to return raw output (default is False).
-            decodeOrder (List[str]): List of encoding orders to decode raw output (default is ["utf-8", "gbk"]).
-            toList (bool): Flag to indicate whether to convert the output to a list (default is False).
-            stripNullLines (bool): Flag to indicate whether to strip null lines from the output (default is False).
-
-        Returns:
-            str: The processed query output
-        """
-        rawProcess = self._queryRaw(*args, timeout=timeout)
-
-        if raw:
-            return rawProcess
-        
-        for decoder in decodeOrder:
-            try:
-                decoded = rawProcess.decode(decoder)
-            except: #noqa
-                continue
-
-            ret = decoded
-
-        if toList:
-            ret = ret.strip().split("\r\n")
-        
-            if stripNullLines:
-                ret = list(filter(None, ret))
-                ret = list(map(lambda x: x.strip(), ret))
-        
-        return ret
+    def _exec(self, cmd: str, *args):
+        _exec(self.__ldconsole__, cmd, *args)
+
+    def _query(self, cmd: str, *args, **kwargs):
+        return query(self.__ldconsole__, cmd, *args, **kwargs)
+
+    def _query_raw(self, cmd: str, *args):
+        return query_raw(self.__ldconsole__, cmd, *args)
 
-    # ANCHOR commands
-    def quit(self, mnq_name : str = None, mnq_idx : int = None):
+    # commands
+    def quit(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         self._exec("quit", *arglist)
 
     def quitall(self):
         self._exec("quitall")
 
-    def launch(self, mnq_name : str = None, mnq_idx : int = None):
+    def launch(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         self._exec("launch", *arglist)
 
-    def reboot(self, mnq_name : str = None, mnq_idx : int = None):
+    def reboot(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         self._exec("reboot", *arglist)
 
     def list(self):
         return self._query("list")
 
     def runninglist(self):
         return self._query("runninglist")
 
-    def isrunning(self, mnq_name : str = None, mnq_idx : int = None):
+    def isrunning(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         return self._query("isrunning", *arglist) == "running"
 
-    def list2(self) -> typing.List[InstanceDict]:
-        raw = self._query("list2", toList=True)
+    def list2(self) -> typing.List[InstanceMeta]:
+        raw = self._query("list2", to_list=True)
+        assert isinstance(raw, list)
         ret = []
         for item in raw:
-            item : str
+            item: str
             splitted = item.split(",")
 
-            ret.append(InstanceDict(
-                id=int(splitted[0]),
-                name=splitted[1],
-                top_window_handle=int(splitted[2]),
-                bind_window_handle=int(splitted[3]),
-                android_started_int=int(splitted[4]),
-                pid=int(splitted[5]),
-                pid_of_vbox=int(splitted[6]),
-            ))
-        
+            ret.append(
+                InstanceMeta(
+                    id=int(splitted[0]),
+                    name=splitted[1],
+                    top_window_handle=int(splitted[2]),
+                    bind_window_handle=int(splitted[3]),
+                    android_started_int=int(splitted[4]),
+                    pid=int(splitted[5]),
+                    pid_of_vbox=int(splitted[6]),
+                )
+            )
+
         return ret
-    
-    def add(self, mnq_name : str = None):
+
+    def add(self, mnq_name: typing.Optional[str] = None):
         arglist = ["--name", mnq_name] if mnq_name is not None else []
         self._exec("add", *arglist)
 
-    def copy(self, mnq_name : str = None, mnq_idx : int = None, to : str = None):
+    def copy(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        to: typing.Optional[str] = None,
+    ):
         if not mnq_name and not mnq_idx:
             raise ValueError("mnq_name and mnq_idx cannot both be None")
-        arglist = ["--from", mnq_name] if mnq_name is not None else ["--from", str(mnq_idx), "--to", to]
+        arglist = (
+            ["--from", mnq_name]
+            if mnq_name is not None
+            else ["--from", str(mnq_idx), "--to", to]
+        )
 
         if to is not None:
             arglist = ["--name", to] + arglist
 
         self._exec("copy", *arglist)
 
-    def remove(self, mnq_name : str = None, mnq_idx : int = None):
+    def remove(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         self._exec("remove", *arglist)
 
-    def rename(self, mnq_name : str = None, mnq_idx : int = None, title : str = None):
+    def rename(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        title: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         if title is not None:
-            arglist.extend(["--title", title]) 
+            arglist.extend(["--title", title])
         self._exec("rename", *arglist)
 
     def modify(
         self,
-        mnq_name : str = None, 
-        mnq_idx : int = None, 
-        resolution : str = None,
-        cpu : typing.Literal[1,2,3,4] = None,
-        memory : typing.Literal[256, 512,768,1024, 2048, 4096, 8192] = None,
-        manufacturer : str = None,
-        model : str = None,
-        pnumber : int = None,
-        imei : typing.Union[typing.Literal["auto"], str] = None,
-        imsi : typing.Union[typing.Literal["auto"], str] = None,
-        simserial : typing.Union[typing.Literal["auto"], str] = None,
-        androidid : typing.Union[typing.Literal["auto"], str] = None,
-        mac : typing.Union[typing.Literal["auto"], str] = None,
-        autorotate : bool = None,
-        lockwindow : bool = None,
-        root : bool = None
+        mnq_name: typing.Optional[typing.Optional[str]] = None,
+        mnq_idx: typing.Optional[typing.Optional[int]] = None,
+        resolution: typing.Optional[str] = None,
+        cpu: typing.Optional[typing.Literal[1, 2, 3, 4]] = None,
+        memory: typing.Optional[
+            typing.Literal[256, 512, 768, 1024, 2048, 4096, 8192]
+        ] = None,
+        manufacturer: typing.Optional[str] = None,
+        model: typing.Optional[str] = None,
+        pnumber: typing.Optional[int] = None,
+        imei: typing.Optional[typing.Union[typing.Literal["auto"], str]] = None,
+        imsi: typing.Optional[typing.Union[typing.Literal["auto"], str]] = None,
+        simserial: typing.Optional[typing.Union[typing.Literal["auto"], str]] = None,
+        androidid: typing.Optional[typing.Union[typing.Literal["auto"], str]] = None,
+        mac: typing.Optional[typing.Union[typing.Literal["auto"], str]] = None,
+        autorotate: typing.Optional[bool] = None,
+        lockwindow: typing.Optional[bool] = None,
+        root: typing.Optional[bool] = None,
     ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         if resolution is not None:
             arglist.extend(["--resolution", resolution])
         if cpu is not None:
             arglist.extend(["--cpu", str(cpu)])
@@ -247,89 +221,159 @@
             arglist.extend(["--autorotate", 1 if autorotate else 0])
         if lockwindow is not None:
             arglist.extend(["--lockwindow", 1 if lockwindow else 0])
         if root is not None:
             arglist.extend(["--root", 1 if root else 0])
         self._exec("modify", *arglist)
 
-    def installapp(self, mnq_name : str = None, mnq_idx : int = None, apk_file_name : str = None):
+    def installapp(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        apk_file_name: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--filename", apk_file_name])
         self._exec("installapp", *arglist)
 
-    def uninstallapp(self, mnq_name : str = None, mnq_idx : int = None, apk_package_name : str = None):
+    def uninstallapp(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        apk_package_name: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--packagename", apk_package_name])
         self._exec("uninstallapp", *arglist)
 
-    def runapp(self, mnq_name : str = None, mnq_idx : int = None, apk_package_name : str = None):
+    def runapp(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        apk_package_name: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--packagename", apk_package_name])
         self._exec("runapp", *arglist)
 
-    def killapp(self, mnq_name : str = None, mnq_idx : int = None, apk_package_name : str = None):
+    def killapp(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        apk_package_name: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--packagename", apk_package_name])
         self._exec("killapp", *arglist)
 
-    def locate(self, mnq_name : str = None, mnq_idx : int = None, lng : float = None, lat : float = None):
+    def locate(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        lng: typing.Optional[float] = None,
+        lat: typing.Optional[float] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
-        arglist.extend["--LLI", f"{lat},{lng}"]
+        arglist.extend(["--LLI", f"{str(lat)},{str(lng)}"])
         self._exec("locate", *arglist)
 
-    def adb(self, mnq_name : str = None, mnq_idx : int = None, cmd_str : str = None):
+    def adb(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        cmd_str: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--command", cmd_str])
         self._exec("adb", *arglist)
 
-    def setprop(self, mnq_name : str = None, mnq_idx : int = None, key : str = None, value : str = None):
+    def setprop(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        key: typing.Optional[str] = None,
+        value: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--key", key, "--value", value])
         self._exec("setprop", *arglist)
 
-    def getprop(self, mnq_name : str = None, mnq_idx : int = None, key : str = None):
+    def getprop(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        key: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         if key is not None:
             arglist.extend(["--key", key])
         self._exec("getprop", *arglist)
 
-    def downcpu(self, mnq_name : str = None, mnq_idx : int = None, rate : int = None):
+    def downcpu(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        rate: typing.Optional[int] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
+        if rate is None:
+            rate = 100
         self.__argument_check_range(rate, 0, 100)
         arglist.extend(["--rate", str(rate)])
         self._exec("downcpu", *arglist)
 
-    def backup(self, mnq_name : str = None, mnq_idx : int = None, filepath : str = None):
+    def backup(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        filepath: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--file", filepath])
         self._exec("backup", *arglist)
 
-    def restore(self, mnq_name : str = None, mnq_idx : int = None, filepath : str = None):
+    def restore(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        filepath: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--file", filepath])
         self._exec("restore", *arglist)
 
-    def action(self, mnq_name : str = None, mnq_idx : int = None, name :str = None, value : str = None):
+    def action(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        name: typing.Optional[str] = None,
+        value: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--name", name, "--value", value])
         self._exec("action", *arglist)
 
-    def scan(self, mnq_name : str = None, mnq_idx : int = None, filepath : str = None):
+    def scan(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        filepath: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--file", filepath])
         self._exec("scan", *arglist)
 
     def sortWnd(self):
         self._exec("sortWnd")
@@ -339,92 +383,136 @@
 
     def zoomOut(self):
         self._exec("zoomOut")
 
     def rock(self):
         self._exec("rock")
 
-    def pull(self, mnq_name : str = None, mnq_idx : int = None, remote : str = None, local : str = None):
+    def pull(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        remote: typing.Optional[str] = None,
+        local: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--remote", remote, "--local", local])
         self._exec("pull", *arglist)
-    
-    def push(self, mnq_name : str = None, mnq_idx : int = None, remote : str = None, local : str = None):
+
+    def push(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        remote: typing.Optional[str] = None,
+        local: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--remote", remote, "--local", local])
         self._exec("push", *arglist)
 
-    def backupapp(self, mnq_name : str = None, mnq_idx : int = None, apk_package_name : str = None, filepath : str = None):
+    def backupapp(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        apk_package_name: typing.Optional[str] = None,
+        filepath: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--packagename", apk_package_name, "--file", filepath])
         self._exec("backupapp", *arglist)
 
-    def restoreapp(self, mnq_name : str = None, mnq_idx : int = None, apk_package_name : str = None, filepath : str = None):
+    def restoreapp(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        apk_package_name: typing.Optional[str] = None,
+        filepath: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--packagename", apk_package_name, "--file", filepath])
         self._exec("restoreapp", *arglist)
 
     def globalsetting(
         self,
-        fps : int = None,
-        audio : bool = None,
-        fastplay : bool = None,
-        cleanmode : bool = None
+        fps: typing.Optional[int] = None,
+        audio: typing.Optional[bool] = None,
+        fastplay: typing.Optional[bool] = None,
+        cleanmode: typing.Optional[bool] = None,
     ):
         arglist = []
         if fps is not None:
             arglist.extend(["--fps", str(fps)])
         if audio is not None:
             arglist.extend(["--audio", 1 if audio else 0])
         if fastplay is not None:
             arglist.extend(["--fastplay", 1 if fastplay else 0])
         if cleanmode is not None:
             arglist.extend(["--cleanmode", 1 if cleanmode else 0])
         self._exec("globalsetting", *arglist)
 
-    def launchex(self, mnq_name : str = None, mnq_idx : int = None, apk_package_name : str = None):
+    def launchex(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        apk_package_name: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--packagename", apk_package_name])
         self._exec("launchex", *arglist)
 
-    def operatelist(self, mnq_name : str = None, mnq_idx : int = None):
+    def operatelist(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
-        self._query("operatelist", *arglist)
+        raw = self._query("operatelist", *arglist)
+        return json.loads(raw)
 
-    def operateinfo(self, mnq_name : str = None, mnq_idx : int = None, filepath : str = None):
+    def operateinfo(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        filepath: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--file", filepath])
-        self._query("operateinfo", *arglist)
+        raw = self._query("operateinfo", *arglist)
+        assert isinstance(raw, str)
+        return json.loads(raw)
 
-    def operaterecord(self, mnq_name : str = None, mnq_idx : int = None, jsonstring : str = None):
+    def operaterecord(
+        self,
+        mnq_name: typing.Optional[str] = None,
+        mnq_idx: typing.Optional[int] = None,
+        jsonstring: typing.Optional[str] = None,
+    ):
         arglist = []
         self.__argument_id(mnq_name, mnq_idx, arglist)
         arglist.extend(["--content", jsonstring])
         self._exec("operaterecord", *arglist)
 
-    #
-    def get(self, mnq_name : str = None, mnq_idx : int = None):
-        if isinstance(mnq_name, int):
-            mnq_idx = mnq_name
-        for item in self.list2():
-            if item["name"] == mnq_name or item["id"] == mnq_idx:
-                return item
-            
-    def query(self, qrystr : str, returnIds : bool = False):
-        evalfunc = eval(f"lambda q : {qrystr}")
-        matched = []
-
-        for item in self.list2():
-            if evalfunc(item):
-                matched.append(item)
+    def __getattribute__(self, name: str) -> typing.Any:
+        if (
+            name.startswith("_")
+            or not self.__ctx
+            or name not in list_of_id_funcs
+            or not self.__ctx.selected
+        ):
+            return super().__getattribute__(name)
+
+        func = super().__getattribute__(name)
+
+        def wrapper(*args, **kwargs):
+
+            for idx in self.__ctx.selected:
+                func(mnq_idx=idx, *args, **kwargs)
+                sleep(self.__config.SYNC_DELAY)
 
-        if returnIds:
-            return [item["id"] for item in matched]
-        else:
-            return matched
+        return wrapper
```

