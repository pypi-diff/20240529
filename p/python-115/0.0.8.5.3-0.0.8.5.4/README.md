# Comparing `tmp/python_115-0.0.8.5.3.tar.gz` & `tmp/python_115-0.0.8.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.5.3.tar", max compression
+gzip compressed data, was "python_115-0.0.8.5.4.tar", max compression
```

## Comparing `python_115-0.0.8.5.3.tar` & `python_115-0.0.8.5.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.5.3/LICENSE
--rwxr-xr-x   0        0        0      475 2024-05-28 12:42:36.566609 python_115-0.0.8.5.3/p115/__init__.py
--rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.5.3/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.5.3/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.5.3/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.5.3/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.5.3/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     2024 2024-05-28 08:51:24.074103 python_115-0.0.8.5.3/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.5.3/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.5.3/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.5.3/p115/component/cipher.py
--rwxr-xr-x   0        0        0   244560 2024-05-28 12:12:17.132740 python_115-0.0.8.5.3/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.5.3/p115/component/exception.py
--rwxr-xr-x   0        0        0    65841 2024-05-28 08:52:45.311883 python_115-0.0.8.5.3/p115/component/fs.py
--rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.5.3/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.5.3/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.5.3/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.5.3/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.5.3/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.5.3/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.5.3/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.5.3/p115/py.typed
--rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.5.3/p115/tool/__init__.py
--rw-r--r--   0        0        0     1681 2024-05-28 12:42:44.494644 python_115-0.0.8.5.3/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.5.3/readme.md
--rw-r--r--   0        0        0    36399 1970-01-01 00:00:00.000000 python_115-0.0.8.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.5.4/LICENSE
+-rwxr-xr-x   0        0        0      475 2024-05-28 12:42:57.024793 python_115-0.0.8.5.4/p115/__init__.py
+-rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.5.4/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.5.4/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.5.4/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.4/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.4/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.4/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.5.4/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.5.4/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2024 2024-05-28 08:51:24.074103 python_115-0.0.8.5.4/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.5.4/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.4/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.4/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.4/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.4/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.5.4/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.5.4/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   244629 2024-05-28 14:00:15.740836 python_115-0.0.8.5.4/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.5.4/p115/component/exception.py
+-rwxr-xr-x   0        0        0    66130 2024-05-28 15:26:11.565966 python_115-0.0.8.5.4/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48262 2024-05-28 15:24:40.699422 python_115-0.0.8.5.4/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.5.4/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.5.4/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.5.4/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.5.4/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.5.4/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.5.4/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.5.4/p115/py.typed
+-rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.5.4/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1681 2024-05-28 15:26:24.284780 python_115-0.0.8.5.4/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.5.4/readme.md
+-rw-r--r--   0        0        0    36399 1970-01-01 00:00:00.000000 python_115-0.0.8.5.4/PKG-INFO
```

### Comparing `python_115-0.0.8.5.3/LICENSE` & `python_115-0.0.8.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/cmd/check.py` & `python_115-0.0.8.5.4/p115/cmd/check.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/cmd/iterdir.py` & `python_115-0.0.8.5.4/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/cmd/qrcode.py` & `python_115-0.0.8.5.4/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/component/__init__.py` & `python_115-0.0.8.5.4/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/component/cipher.py` & `python_115-0.0.8.5.4/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/component/client.py` & `python_115-0.0.8.5.4/p115/component/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1324,15 +1324,15 @@
         ...
     def user_points_sign_post(
         self, 
         /,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
-        """每日签到
+        """每日签到（注意：不要用 web，即浏览器，的 cookies，会失败）
         POST https://proapi.115.com/android/2.0/user/points_sign
         """
         api = "https://proapi.115.com/android/2.0/user/points_sign"
         t = int(time())
         request_kwargs["data"] = {
             "token": sha1(b"%d-Points_Sign@#115-%d" % (self.user_id, t)).hexdigest(), 
             "token_time": t,
```

### Comparing `python_115-0.0.8.5.3/p115/component/fs.py` & `python_115-0.0.8.5.4/p115/component/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
     def copy(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
         overwrite: bool = False, 
-        onerror: bool | Callable[[OSError], bool] = True, 
+        onerror: None | bool | Callable[[OSError], bool] = True, 
     ) -> None | Self:
         attr = self.fs.copy(
             self, 
             dst_path, 
             pid=pid, 
             overwrite=overwrite, 
             onerror=onerror, 
@@ -779,15 +779,15 @@
                 resp = get_files(payload)
                 dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
                 if path_to_id is not None:
                     path_to_id[dirname] = id
                 count = resp["count"]
                 for attr in resp["data"]:
                     yield normalize_attr(attr, dirname, fs=self)
-                for offset in range(page_size, count, 1 << 10):
+                for offset in range(page_size, count, page_size):
                     payload["offset"] = offset
                     resp = get_files(payload)
                     if resp["count"] != count:
                         raise RuntimeError(f"{id} detected count changes during iteration")
                     for attr in resp["data"]:
                         yield normalize_attr(attr, dirname, fs=self)
             if attr_cache is None:
@@ -803,15 +803,15 @@
     def copy(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
         overwrite: bool = False, 
-        onerror: bool | Callable[[OSError], bool] = True, 
+        onerror: None | bool | Callable[[OSError], bool] = True, 
         recursive: bool = False, 
     ) -> None | AttrDict:
         "复制文件"
         try:
             src_attr = self.attr(src_path, pid)
             src_path = cast(str, src_attr["path"])
             if src_attr["is_directory"]:
@@ -893,30 +893,30 @@
                     self.fs_move(dst_id, dst_pid)
                 finally:
                     self.fs_delete(tempdir_id)
                 return self.attr(dst_id)
         except OSError as e:
             if onerror is True:
                 raise
-            elif onerror is False:
+            elif onerror is False or onerror is None:
                 pass
             else:
                 onerror(e)
             return None
 
     # TODO: 使用 fs_batch_* 方法，尽量加快执行速度，但是如果任务数过大（大于 5 万）而报错，则尝试对任务进行拆分
     # TODO: 删除、还原、复制、移动等操作均遵此例，也就是尽量用 batch 方法
     def copytree(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType = "", 
         pid: None | int = None, 
         overwrite: bool = False, 
-        onerror: bool | Callable[[OSError], bool] = True, 
+        onerror: None | bool | Callable[[OSError], bool] = True, 
     ) -> None | AttrDict:
         "复制路径"
         try:
             src_attr = self.attr(src_path, pid)
             if not src_attr["is_directory"]:
                 return self.copy(
                     src_attr, 
@@ -968,15 +968,15 @@
                     )
                 dst_attrs_map = {a["name"]: a for a in self.listdir_attr(dst_id)}
 
             src_attrs = self.listdir_attr(src_id)
         except OSError as e:
             if onerror is True:
                 raise
-            elif onerror is False:
+            elif onerror is False or onerror is None:
                 pass
             else:
                 onerror(e)
             return None
 
         src_files: list[int] = []
         payload: dict = dict(pid=dst_id, overwrite=overwrite, onerror=onerror)
@@ -1296,15 +1296,16 @@
             return self.rename(src_attr, [src_attr["name"]], pid=dst_attr["id"])
         raise FileExistsError(
             errno.EEXIST, 
             f"destination already exists: {src_path!r} -> {dst_path!r}", 
         )
 
     # TODO: 由于 115 网盘不支持删除里面有超过 5 万个文件等目录，因此执行失败时需要拆分任务
-    # TODO: 就算删除和还原执行返回成功，后台可能依然在执行，需要等待前一批完成再执行下一批
+    # TODO: 就算删除和还原执行返回成功，后台可能依然在执行，需要等待几秒钟，前一批完成再执行下一批
+    #       {'state': False, 'error': '删除[...]操作尚未执行完成，请稍后再试！', 'errno': 990009, 'errtype': 'war'}
     def remove(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
         recursive: bool = False, 
     ) -> AttrDict:
@@ -1721,15 +1722,15 @@
         local_path: str | PathLike[str] = ".", 
         path: IDOrPathType = "", 
         pid: None | int = None, 
         no_root: bool = False, 
         overwrite: bool = False, 
         remove_done: bool = False, 
         predicate: None | Callable[[Path], bool] = None, 
-        onerror: bool | Callable[[OSError], bool] = True, 
+        onerror: None | bool | Callable[[OSError], bool] = True, 
     ) -> Iterator[AttrDict]:
         "上传到路径"
         remote_path_attr_map: None | dict[str, dict] = None
         try:
             attr = self.attr(path, pid)
         except FileNotFoundError:
             if isinstance(path, int):
@@ -1761,15 +1762,15 @@
                         pid=pid, 
                         overwrite=overwrite, 
                         remove_done=remove_done, 
                     )
                 except OSError as e:
                     if onerror is True:
                         raise e
-                    elif onerror is False:
+                    elif onerror is False or onerror is None:
                         pass
                     else:
                         onerror(e)
                     return
             if not no_root:
                 attr = self.makedirs(
                     [ospath.basename(local_path)], 
@@ -1779,15 +1780,15 @@
                 pid = attr["id"]
                 remote_path_attr_map = {}
             elif remote_path_attr_map is None:
                 remote_path_attr_map = {a["name"]: a for a in self.iterdir(pid)}
         except OSError as e:
             if onerror is True:
                 raise e
-            elif onerror is False:
+            elif onerror is False or onerror is None:
                 pass
             else:
                 onerror(e)
             return
 
         for entry in subpaths:
             name = entry.name
@@ -1795,15 +1796,15 @@
             remote_path_attr = remote_path_attr_map.get(name)
             if remote_path_attr and isdir != remote_path_attr["is_directory"]:
                 if onerror is True:
                     raise FileExistsError(
                         errno.EEXIST, 
                         f"remote path {remote_path_attr['path']!r} already exists", 
                     )
-                elif onerror is False:
+                elif onerror is False or onerror is None:
                     pass
                 else:
                     onerror(FileExistsError(
                         errno.EEXIST, 
                         f"remote path {remote_path_attr['path']!r} already exists"), 
                     )
                 return
@@ -1848,15 +1849,15 @@
                             remote_path_attr, 
                             overwrite=overwrite, 
                             remove_done=remove_done, 
                         )
                 except OSError as e:
                     if onerror is True:
                         raise e
-                    elif onerror is False:
+                    elif onerror is False or onerror is None:
                         pass
                     else:
                         onerror(e)
 
     unlink = remove
 
     def write_bytes(
```

### Comparing `python_115-0.0.8.5.3/p115/component/fs_base.py` & `python_115-0.0.8.5.4/p115/component/fs_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,15 +464,15 @@
 
     def walk(
         self, 
         /, 
         topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
-        onerror: None | bool | Callable = None, 
+        onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[str], list[str]]]:
         return self.fs.walk(
             self, 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
@@ -482,15 +482,15 @@
 
     def walk_attr(
         self, 
         /, 
         topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
-        onerror: None | bool | Callable = None, 
+        onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         return self.fs.walk_attr(
             self, 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
@@ -500,15 +500,15 @@
 
     def walk_path(
         self, 
         /, 
         topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
-        onerror: None | bool | Callable = None, 
+        onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[Self], list[Self]]]:
         return self.fs.walk_path(
             self, 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
@@ -1354,15 +1354,15 @@
     def _walk_bfs(
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         min_depth: int = 0, 
         max_depth: int = -1, 
-        onerror: None | bool | Callable = None, 
+        onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         dq: deque[tuple[int, AttrDict]] = deque()
         push, pop = dq.append, dq.popleft
         push((0, self.attr(top, pid)))
         while dq:
             depth, parent = pop()
@@ -1394,15 +1394,15 @@
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         topdown: bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
-        onerror: None | bool | Callable = None, 
+        onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         if not max_depth:
             return
         if min_depth > 0:
             min_depth -= 1
         if max_depth > 0:
@@ -1438,15 +1438,15 @@
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
-        onerror: None | bool | Callable = None, 
+        onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[str], list[str]]]:
         for path, dirs, files in self.walk_attr(
             top, 
             pid, 
             topdown=topdown, 
             min_depth=min_depth, 
@@ -1460,15 +1460,15 @@
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
-        onerror: None | bool | Callable = None, 
+        onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         if topdown is None:
             return self._walk_bfs(
                 top, 
                 pid, 
                 min_depth=min_depth, 
@@ -1491,15 +1491,15 @@
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         topdown: Optional[bool] = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
-        onerror: None | bool | Callable = None, 
+        onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[P115PathType], list[P115PathType]]]:
         path_class = type(self).path_class
         for path, dirs, files in self.walk_attr(
             top, 
             pid, 
             topdown=topdown,
```

### Comparing `python_115-0.0.8.5.3/p115/component/fs_share.py` & `python_115-0.0.8.5.4/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/component/fs_zip.py` & `python_115-0.0.8.5.4/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/component/labellist.py` & `python_115-0.0.8.5.4/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/component/offline.py` & `python_115-0.0.8.5.4/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/component/recyclebin.py` & `python_115-0.0.8.5.4/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/component/sharing.py` & `python_115-0.0.8.5.4/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/p115/tool/__init__.py` & `python_115-0.0.8.5.4/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/pyproject.toml` & `python_115-0.0.8.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.5.3"
+version = "0.0.8.5.4"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.5.3/readme.md` & `python_115-0.0.8.5.4/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.3/PKG-INFO` & `python_115-0.0.8.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.5.3
+Version: 0.0.8.5.4
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

