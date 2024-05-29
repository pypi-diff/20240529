# Comparing `tmp/finecache-0.1.0.tar.gz` & `tmp/finecache-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finecache-0.1.0.tar", last modified: Tue May 28 11:57:19 2024, max compression
+gzip compressed data, was "finecache-0.1.1.tar", last modified: Wed May 29 18:45:48 2024, max compression
```

## Comparing `finecache-0.1.0.tar` & `finecache-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:57:19.381726 finecache-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:57:19.377726 finecache-0.1.0/FineCache/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-28 11:57:10.000000 finecache-0.1.0/FineCache/CachedCall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-28 11:57:10.000000 finecache-0.1.0/FineCache/FineCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 11:57:10.000000 finecache-0.1.0/FineCache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-28 11:57:10.000000 finecache-0.1.0/FineCache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:57:19.377726 finecache-0.1.0/FineCache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-28 11:57:19.000000 finecache-0.1.0/FineCache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 11:57:19.000000 finecache-0.1.0/FineCache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:57:19.000000 finecache-0.1.0/FineCache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 11:57:19.000000 finecache-0.1.0/FineCache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 11:57:10.000000 finecache-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-28 11:57:19.381726 finecache-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-28 11:57:10.000000 finecache-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:57:19.381726 finecache-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-28 11:57:10.000000 finecache-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:57:19.377726 finecache-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-28 11:57:10.000000 finecache-0.1.0/tests/test_cachelib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:45:48.585533 finecache-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:45:48.585533 finecache-0.1.1/FineCache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-29 18:45:44.000000 finecache-0.1.1/FineCache/CachedCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-05-29 18:45:44.000000 finecache-0.1.1/FineCache/FineCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 18:45:44.000000 finecache-0.1.1/FineCache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-29 18:45:44.000000 finecache-0.1.1/FineCache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:45:48.585533 finecache-0.1.1/FineCache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-29 18:45:48.000000 finecache-0.1.1/FineCache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-29 18:45:48.000000 finecache-0.1.1/FineCache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:45:48.000000 finecache-0.1.1/FineCache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 18:45:48.000000 finecache-0.1.1/FineCache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 18:45:44.000000 finecache-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-29 18:45:48.585533 finecache-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-29 18:45:44.000000 finecache-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:45:48.585533 finecache-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-29 18:45:44.000000 finecache-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:45:48.585533 finecache-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-29 18:45:44.000000 finecache-0.1.1/tests/test_cachelib.py
```

### Comparing `finecache-0.1.0/FineCache/CachedCall.py` & `finecache-0.1.1/FineCache/CachedCall.py`

 * *Files identical despite different names*

### Comparing `finecache-0.1.0/FineCache/FineCache.py` & `finecache-0.1.1/FineCache/FineCache.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,144 +17,156 @@
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
                     datefmt='%m-%d %H:%M:%S')
 logger = logging.getLogger(__name__)
 
 
 class FineCache:
-    def __init__(self, base_path=None, agent_class=PickleAgent, increment_dir: IncrementDir = None):
+    def __init__(self, base_path=None, ):
         """
         :param base_path: 保存的文件夹，默认为当前文件夹。
         """
         super().__init__()
         self.base_path = base_path if base_path else os.path.abspath(os.getcwd())
         os.makedirs(self.base_path, exist_ok=True)
-        self.agent = agent_class()
-        self.increment_dir = increment_dir if increment_dir else IncrementDir(self.base_path)
+
+        # record current changes immediately
+        # 在代码初始化的时刻就记录代码的改动，否则运行时间较长时，将导致记录错误的记录。
+        self.commit_hash, self.project_root, self.patch_content = self.record_changes()
+        self.patch_time = str(datetime.now())
+
+    @staticmethod
+    def record_changes():
+        # 获取当前的commit hash
+        result = subprocess.run(['git', 'rev-parse', 'HEAD', '--show-toplevel'], stdout=subprocess.PIPE,
+                                encoding='utf-8', text=True)
+        commit_hash, project_root = result.stdout.strip().split('\n')
+
+        # 创建一个patch文件，包含当前改动内容
+        result = subprocess.run(['git', 'diff', 'HEAD'], stdout=subprocess.PIPE,
+                                encoding='utf-8', text=True)
+        patch_content = result.stdout
+        return commit_hash, project_root, patch_content
 
     def cache(self, args_hash: List[Callable[[Any], str]] = None,
               kwargs_hash: List[Callable[[str, Any], Tuple[str, str]]] = None,
-              config: CacheFilenameConfig = CacheFilenameConfig()):
+              config: CacheFilenameConfig = CacheFilenameConfig(),
+              agent=PickleAgent()):
         """
         缓存装饰函数的调用结果。每次调用时，检查是否存在已缓存结果，如果存在则直接给出缓存结果。
 
         :param args_hash:
         :param kwargs_hash:
         :param config:
+        :param agent:
         :return:
         """
 
         def _cache(func: Callable) -> Callable:
             @wraps(func)
             def _get_result(*args, **kwargs):
                 call = CachedCall(func, args, kwargs)
                 filename = config.get_filename(call, args_hash=args_hash, kwargs_hash=kwargs_hash)
                 cache_filename = os.path.join(self.base_path, filename)
                 if os.path.exists(cache_filename) and os.path.isfile(cache_filename):
                     # 从缓存文件获取结果
-                    return self.agent.get(call, cache_filename)
+                    return agent.get(call, cache_filename)
                 else:
                     # 将运行结果缓存到缓存文件中
                     result = call.result
-                    self.agent.set(call, result, cache_filename)
+                    agent.set(call, result, cache_filename)
                     return result
 
             return _get_result
 
         return _cache
 
-    def record(self, comment: str = "", tracking_files: List[str] = None, save_output: bool = True):
-        """
-        保存装饰的函数运行时的代码变更.
-
-        :param comment:
-        :param tracking_files:
-        :param save_output:
-        :return:
+    @contextmanager
+    def record_context(self, inc_dir: IncrementDir, comment: str, tracking_files: List[str] = None,
+                       save_output: bool = True):
+        """
+        :param comment: 注释
+        :param tracking_files: 保存的追踪文件
+        :param save_output: 是否保存输出到单独文件
         """
 
         class Tee:
-            """模仿Linux的tee命令，同时向两个流写入数据"""
-
             def __init__(self, stdout, file):
                 self.stdout = stdout
                 self.file = file
 
             def write(self, data):
+                """"模仿Linux的tee命令，同时向两个流写入数据"""
                 self.stdout.write(data)
                 self.file.write(data)
 
             def flush(self):
                 self.stdout.flush()
                 self.file.flush()
 
-        @contextmanager
-        def duplicate_stdout(file_path):
-            with open(file_path, 'a', encoding='utf-8') as f:
-                old_stdout = sys.stdout
-                sys.stdout = Tee(old_stdout, f)
-                try:
-                    yield
-                finally:
-                    sys.stdout = old_stdout
+        increment_dir = inc_dir if inc_dir else IncrementDir(self.base_path)
+        record_dir = increment_dir.create_new_dir(comment)
+        if save_output:
+            log_filename = os.path.join(record_dir, 'console.log')
+            log_fp = open(log_filename, 'a', encoding='utf-8')
+            old_stdout = sys.stdout
+            sys.stdout = Tee(old_stdout, log_fp)
 
+        # 将追踪的文件复制到相应位置
         tracking_files = [] if tracking_files is None else tracking_files
+        patterns = [re.compile(p) for p in tracking_files]
+        tracking_records = defaultdict(list)
+        for root, dirs, files in os.walk(self.project_root):
+            for file in files:
+                # 构建完整的文件路径
+                full_path = os.path.join(root, file)
+                relative_path = os.path.relpath(full_path, self.project_root)
+                for pattern in patterns:
+                    # 检查是否匹配正则表达式
+                    if pattern.search(file):
+                        # 记录匹配文件的位置
+                        tracking_records[pattern].append(relative_path)
+                        # 复制文件
+                        shutil.copy(full_path, record_dir)
+                        logger.debug(f'Recording {full_path} to {record_dir}')
+
+        # 记录改动及信息
+        patch_location = os.path.join(record_dir, 'current_changes.patch')
+        with open(patch_location, 'w', encoding='utf-8') as patch_file:
+            patch_file.write(self.patch_content)
+        information = {
+            'commit': self.commit_hash,
+            'run_time': str(datetime.now()),
+            'patch_time': self.patch_time,
+            'project_root': self.project_root
+        }
+        if len(tracking_records.keys()) > 0:
+            information['tracking_records'] = tracking_records
+        try:
+            yield information  # 允许修改information内容
+        finally:
+            if save_output:
+                # 关闭文件接口；恢复stdout
+                log_fp.close()
+                sys.stdout = old_stdout
+            information_filename = os.path.join(record_dir, 'information.json')
+            with open(information_filename, 'w', encoding='utf-8') as fp:
+                json.dump(information, fp)
+
+    def record(self, increment_dir: IncrementDir = None, comment: str = "", tracking_files: List[str] = None,
+               save_output: bool = True):
+        """
+        保存装饰的函数运行时的代码变更.
+        """
 
         def record_decorator(func):
             @wraps(func)
             def new_func(*args, **kwargs):
-                record_dir = self.increment_dir.create_new_dir(comment)
-                # 保存输出至文件
-                if save_output:
-                    log_filename = os.path.join(record_dir, 'console.log')
-                    with duplicate_stdout(log_filename):
-                        res = func(*args, **kwargs)
-                else:
+                with self.record_context(increment_dir, comment, tracking_files, save_output) as information:
                     res = func(*args, **kwargs)
-
-                # 获取当前的commit hash
-                result = subprocess.run(['git', 'rev-parse', 'HEAD', '--show-toplevel'], stdout=subprocess.PIPE,
-                                        encoding='utf-8', text=True)
-                commit_hash, project_root = result.stdout.strip().split('\n')
-
-                # 创建一个patch文件，包含当前改动内容
-                result = subprocess.run(['git', 'diff', 'HEAD'], stdout=subprocess.PIPE,
-                                        encoding='utf-8', text=True)
-                patch_content = result.stdout
-                patch_location = os.path.join(record_dir, 'current_changes.patch')
-                with open(patch_location, 'w', encoding='utf-8') as patch_file:
-                    patch_file.write(patch_content)
-
-                # 将追踪的文件复制到相应位置
-                tracking_records = defaultdict(list)
-                for root, dirs, files in os.walk(project_root):
-                    for file in files:
-                        # 构建完整的文件路径
-                        full_path = os.path.join(root, file)
-                        relative_path = os.path.relpath(full_path, project_root)
-                        for file_pattern in tracking_files:
-                            # 检查是否匹配正则表达式
-                            pattern = re.compile(file_pattern)
-                            if pattern.search(file):
-                                # 记录匹配文件的位置
-                                tracking_records[pattern].append(relative_path)
-                                # 复制文件
-                                shutil.copy(full_path, record_dir)
-                                logger.debug(f'Recording {full_path} to {record_dir}')
-
-                # 记录信息：
-                information = {
-                    'commit': commit_hash,
-                    'runtime': str(datetime.now()),
-                    'record_function': func.__qualname__,
-                    'project_root': project_root
-                }
-                if len(tracking_records.keys()) > 0:
-                    information['tracking_records'] = tracking_records
-                information_filename = os.path.join(record_dir, 'information.json')
-                with open(information_filename, 'w', encoding='utf-8') as fp:
-                    json.dump(information, fp)
+                    information['record_function'] = func.__qualname__
+                    information['run_end_time'] = str(datetime.now())
                 return res
 
             return new_func
 
         return record_decorator
```

### Comparing `finecache-0.1.0/FineCache/utils.py` & `finecache-0.1.1/FineCache/utils.py`

 * *Files identical despite different names*

### Comparing `finecache-0.1.0/FineCache.egg-info/PKG-INFO` & `finecache-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: FineCache
-Version: 0.1.0
-Summary: 科研项目缓存中间结果和实验变动记录工具
-Home-page: https://github.com/ciaranchen/FineCache
-Author: Ciaran Chen
-Author-email: ciaranchen@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FineCache
 
 科研项目缓存中间结果和实验变动记录工具。主要提供两个装饰器：
 
 - `FineCache.cache` : 缓存函数的运行结果和参数，并且在下次以相同的参数调用时取出返回结果。
 - `FineCache.record`: 记录实验进行时的代码改动、配置文件及运行信息。
 
@@ -44,20 +31,17 @@
 
 
 func(3, a2=4, k2='v3')
 ```
 
 ### 详细说明
 
-#### FineCache(base_path: str, agent_class: PickleAgent, increment_dir: IncrementDir)
+#### FineCache(base_path: str, agent_class: PickleAgent)
 
 - base_path。基础缓存目录，默认为当前目录。cache的缓存会生成文件。record将会在目录中生成多个文件夹。
-- agent_class。为cache所使用的缓存格式，目前仅支持Pickle。（对于不支持pickle的函数参数，将会跳过存储；对于不支持pickle
-  的函数运行结果，将会报错。）
-- increment_dir。为record使用的自增目录类。参见 `IncrementDir` 说明。
 
 #### FineCache.cache(self, args_hash, kwargs_hash, config = CacheFilenameConfig())
 
 在科研项目（尤其是涉及机器学习的项目）中，通常都需要对通用的数据集进行预处理；进行预处理的结果不应该永久保存，而且又应该避免重复调用繁琐的预处理流程。
 
 这个装饰器能缓存函数的运行结果和参数，并且在下次以相同的参数调用时取出返回结果。
 
@@ -78,33 +62,54 @@
 
 - `config` 定义了缓存文件的文件名生成方式。实际上缓存文件名的生成方式是这样调用的。
 
 ```python
 config.get_filename(call, args_hash, kwargs_hash)
 ```
 
-#### FineCache.record(self, comment: str = "", tracking_files: List[str] = None, save_output: bool = True)
+- `agent`。为cache所使用的缓存格式，目前仅支持PickleAgent。（对于不支持pickle的函数参数，将会跳过存储；对于不支持pickle
+  的函数运行结果，将会报错。）
+
+#### FineCache.record_context(self, increment_dir: IncrementDir = None, comment: str = "", tracking_files: List[str] = None, save_output: bool = True)
 
 在进行研究的过程中，尝尝出现需要调整参数或者方法的情况，这时就需要保存函数的原始代码。每一次运行的过程改动可能都不大，每次都进行git
 commit来存储当然不现实。
 
-这个装饰器能记录实验进行时的代码改动、配置文件及运行信息。参数说明如下。
+此上下文管理器能记录实验进行时的代码改动、配置文件及运行信息。参数说明如下。
 
-- comment: 本次实验的注释。将会影响在base_path下生成文件夹的文件名。
-- tracking_files: 需要保存的配置文件，或任何其它文件。可以使用正则表达式。
-- save_output: 是否记录当前装饰函数的stdout。这不会影响原有输出。
-
-装饰器将在被装饰的函数运行时，在base_path下生成一个文件夹。文件夹中将包含：
-
-- `information.json`: 必要的信息。包含 记录的时间、记录时HEAD的commit ID。
+- `increment_dir`。为record使用的自增目录类，默认为`IncrementDir(self.base_path)`。参见 `IncrementDir` 说明。
+- `comment`: 本次实验的注释。将会影响在base_path下生成文件夹的文件名。
+- `tracking_files`: 需要保存的配置文件，或任何其它文件。可以使用正则表达式。
+- `save_output`: 是否记录当前装饰函数的stdout。这不会影响原有输出。
+
+上下文管理器在进入和离开时，将在base_path下生成一个文件夹。文件夹中将包含：
+
+- `information.json`: 必要的信息。包含以下字段。
+    - `commit`: HEAD的commit ID。
+    - `project_root`: git项目的根目录。
+    - `patch_time`: 记录current changes的时间
+    - `tracking_records`: 额外记录的文件名列表（相对于项目根目录的路径）。
 - `console.log`: 记录的被装饰函数的输出。
 - `current_changes.patch`: 与HEAD的差距patch。
 - `其它tracking_fiels中记录的文件`。
 
+上下文管理器的使用例子如下。可以在`info`字典中添加自定义的内容，将会在离开上下文时被一同写入`information.json`。
+
+```python
+with fc.record_context as info:
+    pass  # do something.
+```
+
+> 注意：为了防止运行时间过长导致运行到上下文处时代码已经做了变更。我们将会在FineCache初始化时就记录代码的patch，只是在上下文运行时才写入文件。
+
+#### FineCache.record
+
+此装饰器与record的参数定义完全一致。只是提供不同的使用方式。在`information.json`中会额外写入调用的函数名称及运行结束的时间。
+
 ### 其它说明
 
 #### IncrementDir(base_path: str, dir_prefix: str = "")
 
-- base_path: 基础缓存目录。
-- dir_prefix: 生成文件夹名称的前缀。
+- `base_path`: 基础缓存目录。
+- `dir_prefix`: 生成文件夹名称的前缀。
 
 其生成的文件夹名称为 `{dir_prefix}{num}` 或 `{dir_prefix}{num}-{comment}`。
```

### Comparing `finecache-0.1.0/LICENSE` & `finecache-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finecache-0.1.0/PKG-INFO` & `finecache-0.1.1/FineCache.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FineCache
-Version: 0.1.0
+Version: 0.1.1
 Summary: 科研项目缓存中间结果和实验变动记录工具
 Home-page: https://github.com/ciaranchen/FineCache
 Author: Ciaran Chen
 Author-email: ciaranchen@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,20 +44,17 @@
 
 
 func(3, a2=4, k2='v3')
 ```
 
 ### 详细说明
 
-#### FineCache(base_path: str, agent_class: PickleAgent, increment_dir: IncrementDir)
+#### FineCache(base_path: str, agent_class: PickleAgent)
 
 - base_path。基础缓存目录，默认为当前目录。cache的缓存会生成文件。record将会在目录中生成多个文件夹。
-- agent_class。为cache所使用的缓存格式，目前仅支持Pickle。（对于不支持pickle的函数参数，将会跳过存储；对于不支持pickle
-  的函数运行结果，将会报错。）
-- increment_dir。为record使用的自增目录类。参见 `IncrementDir` 说明。
 
 #### FineCache.cache(self, args_hash, kwargs_hash, config = CacheFilenameConfig())
 
 在科研项目（尤其是涉及机器学习的项目）中，通常都需要对通用的数据集进行预处理；进行预处理的结果不应该永久保存，而且又应该避免重复调用繁琐的预处理流程。
 
 这个装饰器能缓存函数的运行结果和参数，并且在下次以相同的参数调用时取出返回结果。
 
@@ -78,33 +75,54 @@
 
 - `config` 定义了缓存文件的文件名生成方式。实际上缓存文件名的生成方式是这样调用的。
 
 ```python
 config.get_filename(call, args_hash, kwargs_hash)
 ```
 
-#### FineCache.record(self, comment: str = "", tracking_files: List[str] = None, save_output: bool = True)
+- `agent`。为cache所使用的缓存格式，目前仅支持PickleAgent。（对于不支持pickle的函数参数，将会跳过存储；对于不支持pickle
+  的函数运行结果，将会报错。）
+
+#### FineCache.record_context(self, increment_dir: IncrementDir = None, comment: str = "", tracking_files: List[str] = None, save_output: bool = True)
 
 在进行研究的过程中，尝尝出现需要调整参数或者方法的情况，这时就需要保存函数的原始代码。每一次运行的过程改动可能都不大，每次都进行git
 commit来存储当然不现实。
 
-这个装饰器能记录实验进行时的代码改动、配置文件及运行信息。参数说明如下。
+此上下文管理器能记录实验进行时的代码改动、配置文件及运行信息。参数说明如下。
 
-- comment: 本次实验的注释。将会影响在base_path下生成文件夹的文件名。
-- tracking_files: 需要保存的配置文件，或任何其它文件。可以使用正则表达式。
-- save_output: 是否记录当前装饰函数的stdout。这不会影响原有输出。
-
-装饰器将在被装饰的函数运行时，在base_path下生成一个文件夹。文件夹中将包含：
-
-- `information.json`: 必要的信息。包含 记录的时间、记录时HEAD的commit ID。
+- `increment_dir`。为record使用的自增目录类，默认为`IncrementDir(self.base_path)`。参见 `IncrementDir` 说明。
+- `comment`: 本次实验的注释。将会影响在base_path下生成文件夹的文件名。
+- `tracking_files`: 需要保存的配置文件，或任何其它文件。可以使用正则表达式。
+- `save_output`: 是否记录当前装饰函数的stdout。这不会影响原有输出。
+
+上下文管理器在进入和离开时，将在base_path下生成一个文件夹。文件夹中将包含：
+
+- `information.json`: 必要的信息。包含以下字段。
+    - `commit`: HEAD的commit ID。
+    - `project_root`: git项目的根目录。
+    - `patch_time`: 记录current changes的时间
+    - `tracking_records`: 额外记录的文件名列表（相对于项目根目录的路径）。
 - `console.log`: 记录的被装饰函数的输出。
 - `current_changes.patch`: 与HEAD的差距patch。
 - `其它tracking_fiels中记录的文件`。
 
+上下文管理器的使用例子如下。可以在`info`字典中添加自定义的内容，将会在离开上下文时被一同写入`information.json`。
+
+```python
+with fc.record_context as info:
+    pass  # do something.
+```
+
+> 注意：为了防止运行时间过长导致运行到上下文处时代码已经做了变更。我们将会在FineCache初始化时就记录代码的patch，只是在上下文运行时才写入文件。
+
+#### FineCache.record
+
+此装饰器与record的参数定义完全一致。只是提供不同的使用方式。在`information.json`中会额外写入调用的函数名称及运行结束的时间。
+
 ### 其它说明
 
 #### IncrementDir(base_path: str, dir_prefix: str = "")
 
-- base_path: 基础缓存目录。
-- dir_prefix: 生成文件夹名称的前缀。
+- `base_path`: 基础缓存目录。
+- `dir_prefix`: 生成文件夹名称的前缀。
 
 其生成的文件夹名称为 `{dir_prefix}{num}` 或 `{dir_prefix}{num}-{comment}`。
```

### Comparing `finecache-0.1.0/README.md` & `finecache-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: FineCache
+Version: 0.1.1
+Summary: 科研项目缓存中间结果和实验变动记录工具
+Home-page: https://github.com/ciaranchen/FineCache
+Author: Ciaran Chen
+Author-email: ciaranchen@qq.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # FineCache
 
 科研项目缓存中间结果和实验变动记录工具。主要提供两个装饰器：
 
 - `FineCache.cache` : 缓存函数的运行结果和参数，并且在下次以相同的参数调用时取出返回结果。
 - `FineCache.record`: 记录实验进行时的代码改动、配置文件及运行信息。
 
@@ -31,20 +44,17 @@
 
 
 func(3, a2=4, k2='v3')
 ```
 
 ### 详细说明
 
-#### FineCache(base_path: str, agent_class: PickleAgent, increment_dir: IncrementDir)
+#### FineCache(base_path: str, agent_class: PickleAgent)
 
 - base_path。基础缓存目录，默认为当前目录。cache的缓存会生成文件。record将会在目录中生成多个文件夹。
-- agent_class。为cache所使用的缓存格式，目前仅支持Pickle。（对于不支持pickle的函数参数，将会跳过存储；对于不支持pickle
-  的函数运行结果，将会报错。）
-- increment_dir。为record使用的自增目录类。参见 `IncrementDir` 说明。
 
 #### FineCache.cache(self, args_hash, kwargs_hash, config = CacheFilenameConfig())
 
 在科研项目（尤其是涉及机器学习的项目）中，通常都需要对通用的数据集进行预处理；进行预处理的结果不应该永久保存，而且又应该避免重复调用繁琐的预处理流程。
 
 这个装饰器能缓存函数的运行结果和参数，并且在下次以相同的参数调用时取出返回结果。
 
@@ -65,33 +75,54 @@
 
 - `config` 定义了缓存文件的文件名生成方式。实际上缓存文件名的生成方式是这样调用的。
 
 ```python
 config.get_filename(call, args_hash, kwargs_hash)
 ```
 
-#### FineCache.record(self, comment: str = "", tracking_files: List[str] = None, save_output: bool = True)
+- `agent`。为cache所使用的缓存格式，目前仅支持PickleAgent。（对于不支持pickle的函数参数，将会跳过存储；对于不支持pickle
+  的函数运行结果，将会报错。）
+
+#### FineCache.record_context(self, increment_dir: IncrementDir = None, comment: str = "", tracking_files: List[str] = None, save_output: bool = True)
 
 在进行研究的过程中，尝尝出现需要调整参数或者方法的情况，这时就需要保存函数的原始代码。每一次运行的过程改动可能都不大，每次都进行git
 commit来存储当然不现实。
 
-这个装饰器能记录实验进行时的代码改动、配置文件及运行信息。参数说明如下。
+此上下文管理器能记录实验进行时的代码改动、配置文件及运行信息。参数说明如下。
 
-- comment: 本次实验的注释。将会影响在base_path下生成文件夹的文件名。
-- tracking_files: 需要保存的配置文件，或任何其它文件。可以使用正则表达式。
-- save_output: 是否记录当前装饰函数的stdout。这不会影响原有输出。
-
-装饰器将在被装饰的函数运行时，在base_path下生成一个文件夹。文件夹中将包含：
-
-- `information.json`: 必要的信息。包含 记录的时间、记录时HEAD的commit ID。
+- `increment_dir`。为record使用的自增目录类，默认为`IncrementDir(self.base_path)`。参见 `IncrementDir` 说明。
+- `comment`: 本次实验的注释。将会影响在base_path下生成文件夹的文件名。
+- `tracking_files`: 需要保存的配置文件，或任何其它文件。可以使用正则表达式。
+- `save_output`: 是否记录当前装饰函数的stdout。这不会影响原有输出。
+
+上下文管理器在进入和离开时，将在base_path下生成一个文件夹。文件夹中将包含：
+
+- `information.json`: 必要的信息。包含以下字段。
+    - `commit`: HEAD的commit ID。
+    - `project_root`: git项目的根目录。
+    - `patch_time`: 记录current changes的时间
+    - `tracking_records`: 额外记录的文件名列表（相对于项目根目录的路径）。
 - `console.log`: 记录的被装饰函数的输出。
 - `current_changes.patch`: 与HEAD的差距patch。
 - `其它tracking_fiels中记录的文件`。
 
+上下文管理器的使用例子如下。可以在`info`字典中添加自定义的内容，将会在离开上下文时被一同写入`information.json`。
+
+```python
+with fc.record_context as info:
+    pass  # do something.
+```
+
+> 注意：为了防止运行时间过长导致运行到上下文处时代码已经做了变更。我们将会在FineCache初始化时就记录代码的patch，只是在上下文运行时才写入文件。
+
+#### FineCache.record
+
+此装饰器与record的参数定义完全一致。只是提供不同的使用方式。在`information.json`中会额外写入调用的函数名称及运行结束的时间。
+
 ### 其它说明
 
 #### IncrementDir(base_path: str, dir_prefix: str = "")
 
-- base_path: 基础缓存目录。
-- dir_prefix: 生成文件夹名称的前缀。
+- `base_path`: 基础缓存目录。
+- `dir_prefix`: 生成文件夹名称的前缀。
 
 其生成的文件夹名称为 `{dir_prefix}{num}` 或 `{dir_prefix}{num}-{comment}`。
```

### Comparing `finecache-0.1.0/setup.py` & `finecache-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="FineCache",
-  version="0.1.0",
+  version="0.1.1",
   author="Ciaran Chen",
   author_email="ciaranchen@qq.com",
   description="科研项目缓存中间结果和实验变动记录工具",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ciaranchen/FineCache",
   packages=setuptools.find_packages(),
```

### Comparing `finecache-0.1.0/tests/test_cachelib.py` & `finecache-0.1.1/tests/test_cachelib.py`

 * *Files identical despite different names*

