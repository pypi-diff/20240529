# Comparing `tmp/btgitserver-2.0.1.tar.gz` & `tmp/btgitserver-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btgitserver-2.0.1.tar", last modified: Sun May 26 18:57:36 2024, max compression
+gzip compressed data, was "btgitserver-3.1.0.tar", last modified: Wed May 29 21:00:20 2024, max compression
```

## Comparing `btgitserver-2.0.1.tar` & `btgitserver-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-26 18:57:36.112165 btgitserver-2.0.1/
--rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-2.0.1/.gitignore
--rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-2.0.1/Dockerfile
--rw-r--r--   0 etejeda    (501) staff       (20)     2893 2024-05-26 18:57:36.112462 btgitserver-2.0.1/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     2259 2024-05-26 06:26:27.000000 btgitserver-2.0.1/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2024-05-26 18:57:08.000000 btgitserver-2.0.1/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-26 18:57:36.107862 btgitserver-2.0.1/btgitserver/
--rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-2.0.1/btgitserver/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     8177 2024-05-26 06:20:33.000000 btgitserver-2.0.1/btgitserver/app.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2473 2024-05-26 18:55:58.000000 btgitserver-2.0.1/btgitserver/args.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-2.0.1/btgitserver/config.py
--rw-r--r--   0 etejeda    (501) staff       (20)      757 2024-05-26 06:05:54.000000 btgitserver-2.0.1/btgitserver/defaults.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-2.0.1/btgitserver/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-26 18:57:36.111269 btgitserver-2.0.1/btgitserver.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     2893 2024-05-26 18:57:35.000000 btgitserver-2.0.1/btgitserver.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      455 2024-05-26 18:57:36.000000 btgitserver-2.0.1/btgitserver.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2024-05-26 18:57:35.000000 btgitserver-2.0.1/btgitserver.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       55 2024-05-26 18:57:35.000000 btgitserver-2.0.1/btgitserver.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-2.0.1/btgitserver.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      173 2024-05-26 18:57:35.000000 btgitserver-2.0.1/btgitserver.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       12 2024-05-26 18:57:35.000000 btgitserver-2.0.1/btgitserver.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-26 18:57:36.111799 btgitserver-2.0.1/etc/
--rwx------   0 etejeda    (501) staff       (20)      197 2024-05-25 21:39:11.000000 btgitserver-2.0.1/etc/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)     1239 2024-05-26 18:57:36.114200 btgitserver-2.0.1/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-2.0.1/setup.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-29 21:00:20.727560 btgitserver-3.1.0/
+-rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-3.1.0/.gitignore
+-rwx------   0 etejeda    (501) staff       (20)      380 2024-05-26 20:17:48.000000 btgitserver-3.1.0/Dockerfile
+-rw-r--r--   0 etejeda    (501) staff       (20)     3265 2024-05-29 21:00:20.727823 btgitserver-3.1.0/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     2631 2024-05-29 18:17:16.000000 btgitserver-3.1.0/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2024-05-29 20:59:49.000000 btgitserver-3.1.0/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-29 21:00:20.723152 btgitserver-3.1.0/btgitserver/
+-rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-3.1.0/btgitserver/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     9876 2024-05-29 18:38:30.000000 btgitserver-3.1.0/btgitserver/app.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2984 2024-05-29 18:19:45.000000 btgitserver-3.1.0/btgitserver/args.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1043 2024-05-29 20:53:44.000000 btgitserver-3.1.0/btgitserver/config.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      904 2024-05-29 18:44:00.000000 btgitserver-3.1.0/btgitserver/defaults.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-3.1.0/btgitserver/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-29 21:00:20.726850 btgitserver-3.1.0/btgitserver.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3265 2024-05-29 21:00:20.000000 btgitserver-3.1.0/btgitserver.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      455 2024-05-29 21:00:20.000000 btgitserver-3.1.0/btgitserver.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2024-05-29 21:00:20.000000 btgitserver-3.1.0/btgitserver.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       60 2024-05-29 21:00:20.000000 btgitserver-3.1.0/btgitserver.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-3.1.0/btgitserver.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      204 2024-05-29 21:00:20.000000 btgitserver-3.1.0/btgitserver.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       12 2024-05-29 21:00:20.000000 btgitserver-3.1.0/btgitserver.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-29 21:00:20.727244 btgitserver-3.1.0/etc/
+-rwxr-xr-x   0 etejeda    (501) staff       (20)      279 2024-05-29 20:52:22.000000 btgitserver-3.1.0/etc/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)     1274 2024-05-29 21:00:20.730415 btgitserver-3.1.0/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-3.1.0/setup.py
```

### Comparing `btgitserver-2.0.1/.gitignore` & `btgitserver-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `btgitserver-2.0.1/PKG-INFO` & `btgitserver-3.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgitserver
-Version: 2.0.1
+Version: 3.1.0
 Summary: Python-based Git Server
 Home-page: https://github.com/berttejeda/bert.git-server
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -25,14 +25,15 @@
 Features:
 
 - Makes any git repository lying below the _search\_paths_ setting
   available for `git clone` and `git push` via HTTP using basic authentication
 - Application defaults can be overridden by specifying a configuration file<br />
   Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
 - On-demand repos: If you attempt to push a non-existing repo to the server, it will be created 
+- Employs process threading via [gunicorn](https://gunicorn.org/)
 
 ## Installation
 
 - Install from pypi.org: `pip install btgitserver`
 - Install directly from git repo: `pip install git+http://www.github.com/berttejeda/bert.gt-server.git`
 
 ## Usage
@@ -72,15 +73,15 @@
 git add .
 git commit -m 'Initial Commit'
 cd ~
 bt.git-server -r /tmp/repos
 ```
 
 **Note**: The `--repo-search-paths/-r` cli option allows specifying 
-multiple, space-delimitted search paths, e.g. `bt.git-server -r /tmp/repos /tmp/repos2`
+multiple, space-delimited search paths, e.g. `bt.git-server -r /tmp/repos /tmp/repos2`
 
 * Launch the standalone git server
 
 `bt.git-server`
 
 You should see output similar to:
 ```
@@ -106,7 +107,20 @@
 git remote add origin http://git-user:git-password@127.0.0.1:5000/contoso/foo-bar
 git checkout -b main
 touch test_file.txt
 git add .
 git commit -m 'Initial Commit'
 git push --set-upstream origin $(git rev-parse --abbrev-ref HEAD)
 ```
+
+## Docker
+
+For your convenience, a [Dockerfile](Dockerfile) has been provided,
+so feel free to build your own containerized instance of this app, or
+use the pre-built docker image:
+
+```bash
+mkdir /tmp/repos
+docker run -it --rm -p 5000:5000 \
+-v /tmp/repos:/opt/git-server/repos \
+berttejeda/git-server
+```
```

### Comparing `btgitserver-2.0.1/README.md` & `btgitserver-3.1.0/btgitserver.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,39 @@
+Metadata-Version: 2.1
+Name: btgitserver
+Version: 3.1.0
+Summary: Python-based Git Server
+Home-page: https://github.com/berttejeda/bert.git-server
+Author: Engelbert Tejeda
+Author-email: berttejeda@gmail.com
+Keywords: yaml,configuration,config,file,python,settings
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+
 ## Overview
 
 A git server implementation written in python.
 
 Based off the amazing work by Stewart Park in this gist: [https://gist.github.com/stewartpark/1b079dc0481c6213def9](https://gist.github.com/stewartpark/1b079dc0481c6213def9).
 
 Features:
 
 - Makes any git repository lying below the _search\_paths_ setting
   available for `git clone` and `git push` via HTTP using basic authentication
 - Application defaults can be overridden by specifying a configuration file<br />
   Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
 - On-demand repos: If you attempt to push a non-existing repo to the server, it will be created 
+- Employs process threading via [gunicorn](https://gunicorn.org/)
 
 ## Installation
 
 - Install from pypi.org: `pip install btgitserver`
 - Install directly from git repo: `pip install git+http://www.github.com/berttejeda/bert.gt-server.git`
 
 ## Usage
@@ -54,15 +73,15 @@
 git add .
 git commit -m 'Initial Commit'
 cd ~
 bt.git-server -r /tmp/repos
 ```
 
 **Note**: The `--repo-search-paths/-r` cli option allows specifying 
-multiple, space-delimitted search paths, e.g. `bt.git-server -r /tmp/repos /tmp/repos2`
+multiple, space-delimited search paths, e.g. `bt.git-server -r /tmp/repos /tmp/repos2`
 
 * Launch the standalone git server
 
 `bt.git-server`
 
 You should see output similar to:
 ```
@@ -87,8 +106,21 @@
 git init .
 git remote add origin http://git-user:git-password@127.0.0.1:5000/contoso/foo-bar
 git checkout -b main
 touch test_file.txt
 git add .
 git commit -m 'Initial Commit'
 git push --set-upstream origin $(git rev-parse --abbrev-ref HEAD)
-```
+```
+
+## Docker
+
+For your convenience, a [Dockerfile](Dockerfile) has been provided,
+so feel free to build your own containerized instance of this app, or
+use the pre-built docker image:
+
+```bash
+mkdir /tmp/repos
+docker run -it --rm -p 5000:5000 \
+-v /tmp/repos:/opt/git-server/repos \
+berttejeda/git-server
+```
```

### Comparing `btgitserver-2.0.1/btgitserver/app.py` & `btgitserver-3.1.0/btgitserver/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+import atexit
+import gunicorn.app.base
 import random
 import sys
 import subprocess
 
 from btgitserver.args import parse_args
 from btgitserver.config import AppConfig
-from btgitserver.defaults import default_app_port, \
+from btgitserver.defaults import \
 default_app_host_address, \
+default_app_port, \
+default_num_threads, \
+default_num_workers, \
+default_preload, \
 default_repo_search_paths, \
 default_ondemand_repo_search_paths, \
 default_verify_tls
 from btgitserver.logger import Logger
 
 from dulwich import repo
 from dulwich.pack import PackStreamReader
@@ -18,14 +24,15 @@
 from pathlib import Path
 
 if sys.version_info[0] == 2:
     from StringIO import StringIO
 if sys.version_info[0] >= 3:
     from io import BytesIO
 
+
 # Private variables
 __author__ = 'berttejeda'
 __original_author = 'stewartpark'
 
 # Read command-line args
 args = parse_args()
 
@@ -34,29 +41,51 @@
     logfile_path=args.logfile_path,
     logfile_write_mode=args.logfile_write_mode)
 logger = logger_obj.init_logger('app')
 
 verify_tls = args.no_verify_tls or default_verify_tls
 
 # Flask
-app = Flask(__name__)
 auth = HTTPBasicAuth()
 
 # Initialize Config Readers
 app_config = AppConfig().initialize(
   args=vars(args),
   verify_tls=verify_tls
 )
 
 git_ondemand_search_paths = args.ondemand_repo_search_paths or app_config.get('app.ondemand.search_paths', default_ondemand_repo_search_paths)
 git_search_paths = args.repo_search_paths or app_config.get('app.search_paths', default_repo_search_paths)
 git_search_paths = git_search_paths + git_ondemand_search_paths
+app_host_address = args.host_address or app_config.get('app.listen', default_app_host_address)
+app_port = args.port or app_config.get('app.port', default_app_port)
+gunicorn_preload = args.preload or app_config.get('app.gunicorn.preload', default_preload)
+gunicorn_threads = args.threads or app_config.get('app.gunicorn.threads', default_num_threads)
+gunicorn_workers = args.workers or app_config.get('app.gunicorn.workers', default_num_workers)
+
 authorized_users = app_config.auth.users
 users = [u[0] for u in authorized_users.items()]
 
+
+class StandaloneApplication(gunicorn.app.base.BaseApplication):
+
+    def __init__(self, app, options=None):
+        self.options = options or {}
+        self.application = app
+        super().__init__()
+
+    def load_config(self):
+        config = {key: value for key, value in self.options.items()
+                  if key in self.cfg.settings and value is not None}
+        for key, value in config.items():
+            self.cfg.set(key.lower(), value)
+
+    def load(self):
+        return self.application
+
 def get_repos(org, search_paths):
     repo_map = {}
 
     for git_search_path in search_paths:
         fq_git_search_path = Path(git_search_path).expanduser().joinpath(org)
         logger.debug(f'Building git repo map ...')
         logger.debug(f'Adding git repos under {fq_git_search_path}')
@@ -65,21 +94,28 @@
             if dotgit.is_dir():
                 git_directory = p.as_posix()
                 git_directory_name = p.name
                 if git_directory_name:
                     repo_map[git_directory_name] = git_directory
     logger.debug(f'Finished building git repo map!')
     numrepos = len(list(repo_map.keys()))
-    logger.info(f'Found {numrepos} repo(s)')
+    logger.debug(f'Found {numrepos} repo(s)')
     return repo_map
 
-def start_api():
+
+def interrupt():
+  logger.info("Stop API")
+
+def start_api(**kwargs):
   """API functions.
   This function defines the API routes and starts the API Process.
   """
+  app = Flask(__name__)
+  # app.config['MAX_CONTENT_LENGTH'] = 1600 * 1024 * 1024 # 16GB
+  # app.config['MAX_CONTENT_LENGTH'] = 16 * 1024 * 1024 # 16MB
 
   @auth.get_password
   def get_pw(username):
       if username in users:
           credential = authorized_users.get(username).password
           return credential
       else:
@@ -90,41 +126,46 @@
   def info_refs(org_name, project_name):
       git_repo_map = get_repos(org_name, git_search_paths)
       available_repos = list(git_repo_map.keys())
       service = request.args.get('service')
       if service[:4] != 'git-':
           abort(500)
 
+      logger.info(f'Receiving {org_name}/{project_name}')
+      
       if project_name in available_repos:
           return info_refs_header(
               git_repo_map=git_repo_map,
               project_name=project_name,
               service=service
           )
       else:
+          logger.info(f'Repo at {org_name}/{project_name} does not currently exist, processing as on-demand')
+          ondemand_search_path = random.choice(git_ondemand_search_paths)
+          ondemand_org_path = Path(ondemand_search_path).expanduser().joinpath(org_name)
           try:
-              ondemand_search_path = random.choice(git_ondemand_search_paths)
-              ondemand_org_path = Path(ondemand_search_path).expanduser().joinpath(org_name)
               if not ondemand_org_path.is_dir():
-                logger.info(f'Creating org path at {ondemand_org_path}')
-                ondemand_org_path.mkdir(parents=True)
+                  logger.info(f'Creating on-demand repo org path at {ondemand_org_path}')
+                  ondemand_org_path.mkdir(parents=True)
               ondemand_project_path = ondemand_org_path.joinpath(project_name).as_posix()
+              logger.info(f'Initializing on-demand repo {ondemand_project_path}')
               project_repo = repo.Repo.init(ondemand_project_path, mkdir=True)
               project_repo_config = project_repo.get_config()
               project_repo_config.set("receive", "denyCurrentBranch", "updateInstead")
               project_repo_config.write_to_path()
+              logger.info(f'Initialization complete for {ondemand_project_path}')
               git_repo_map = get_repos(org_name, git_search_paths)
               return info_refs_header(
                   git_repo_map=git_repo_map,
                   project_name=project_name,
                   service=service
               )
           except Exception as e:
-            logger.error(f"Could not create on-demand project path at {ondemand_project_path}, error was {e}")
-            abort(501)
+              logger.error(f"Could not create on-demand project path at {ondemand_project_path}, error was {e}")
+              abort(501)
 
   def info_refs_header(**kwargs):
     git_repo_map = kwargs['git_repo_map']
     project_name = kwargs['project_name']
     service = kwargs['service']
     project_path = [v for k, v in git_repo_map.items() if k == project_name][0]
     p = subprocess.Popen([service, '--stateless-rpc', '--advertise-refs', project_path], stdout=subprocess.PIPE)
@@ -169,14 +210,15 @@
           data_out = p.communicate()
           res = make_response(data_out)
           res.headers['Expires'] = 'Fri, 01 Jan 1980 00:00:00 GMT'
           res.headers['Pragma'] = 'no-cache'
           res.headers['Cache-Control'] = 'no-cache, max-age=0, must-revalidate'
           res.headers['Content-Type'] = 'application/x-git-receive-pack-result'
           p.wait()
+          logger.info(f'Finished receiving {org_name}/{project_name}')
           return res
       else:
           abort(501)
 
   @app.route('/<string:org_name>/<string:project_name>/git-upload-pack', methods=('POST',))
   @auth.login_required
   def git_upload_pack(org_name, project_name):
@@ -197,23 +239,22 @@
           p.wait()
           return res
       else:
           abort(501)
 
   logger.info("Start API")
 
-  app_port = args.port or app_config.get('app.port') or default_app_port
-  app_host_address = args.host_address or app_config.get('app.address') or default_app_host_address
-  app.run(host=app_host_address, port=app_port)
-
-  logger.info("Stop API")
-
-def main():
-  """The main entrypoint
-  """
-
-  start_api()
+  options = {
+      'bind': f'{app_host_address}:{app_port}',
+      'preload': gunicorn_preload,
+      'threads': gunicorn_threads,
+      'workers': gunicorn_workers,
+  }
+
+  atexit.register(interrupt)
+  if args.dev_server:
+    app.run(host=app_host_address, port=app_port)
+  else:
+    StandaloneApplication(app, options).run()    
 
 if __name__ == '__main__':
-  main()
-
-
+  start_api()
```

### Comparing `btgitserver-2.0.1/btgitserver/args.py` & `btgitserver-3.1.0/btgitserver/args.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,17 +46,22 @@
         help="Override number of gunicorn workers",
         metavar="ARG", required=False)    
     parser.add_argument('--no-verify-tls', '-notls',action='store_true', help='Verify SSL cert when downloading web content')
     parser.add_argument('--config-file', '-f', help="Path to config file override")
     parser.add_argument('--repo-search-paths', '-r', nargs='+', help="List of directories containing git repositories")
     parser.add_argument('--ondemand-repo-search-paths', '-odr', nargs='+', help="List of directories containing on-demand git repositories")
     parser.add_argument('--logfile-path', '-L', help="Path to logfile")
-    parser.add_argument('--logfile-write-mode', '-Lw', default='w', choices=['a', 'w'], help="File mode when writing to log file, 'a' to append, 'w' to overwrite")    
+    parser.add_argument('--threads', '-t', default=8, help="Number of concurrent threads")
+    parser.add_argument('--timeout', '-T', default=0, help="Timeout")
+    parser.add_argument('--num-workers', type=int, default=5, help="Number of worker processes")
+    parser.add_argument('--logfile-write-mode', '-Lw', default='w', choices=['a', 'w'], help="File mode when writing to log file, 'a' to append, 'w' to overwrite")
+    parser.add_argument('--preload', action='store_true', help="Load application code before the worker processes are forked")
     parser.add_argument('--debug', action='store_true')
+    parser.add_argument('--dev-server', action='store_true', help="Start app in Flask dev server mode")
     parser.add_argument('--version', action='version', version=f'%(prog)s {__version__}')
     parser.add_argument(
         "-v",
         "--verbose",
         help="increase output verbosity",
         action="store_true")
-    
-    return parser.parse_args()
+    args, unknown = parser.parse_known_args()
+    return args
```

### Comparing `btgitserver-2.0.1/btgitserver/config.py` & `btgitserver-3.1.0/btgitserver/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,13 +27,14 @@
     logger.info(f"Config file URI is {config_file_uri}")
     # Initialize App Config
     config = Config(
         config_file_uri=config_file_uri,
         default_value=default_settings,
         initial_data=initial_data,
         args=args,
+        warn_if_config_not_found=True,
         verify_tls=verify_tls
     )
 
     settings = config.read()
 
     return settings
```

### Comparing `btgitserver-2.0.1/btgitserver/defaults.py` & `btgitserver-3.1.0/btgitserver/defaults.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 # Flask app settings
 debug = False
 app_name = "Python Git Server"
 default_app_port = 5000
 default_config_file_name = 'config.yaml'
 default_app_host_address = '0.0.0.0'
-default_repo_search_paths = ['~/repos']
-default_ondemand_repo_search_paths = ['~/repos.ondemand']
-default_num_workers = 4 # not yet implemented
+default_repo_search_paths = ['~/git-server/repos']
+default_ondemand_repo_search_paths = ['~/git-server/repos.ondemand']
+default_num_workers = 4
+default_num_threads = 8
+default_preload = True
 default_settings = {
   "auth": {
     "users": {
       "git-user": {
         "password": "git-password"
       }
     }
@@ -24,10 +26,14 @@
     "debug": debug,
     "listen": default_app_host_address,
     "port": default_app_port,
     "search_paths": default_repo_search_paths,
     "ondemand": {
       "search_paths": default_ondemand_repo_search_paths
     },
-    "workers": default_num_workers
+    "gunicorn": {
+      "workers": default_num_workers, 
+      "threads": default_num_threads, 
+      "preload": default_preload
+    }
   }
 }
```

### Comparing `btgitserver-2.0.1/btgitserver/logger.py` & `btgitserver-3.1.0/btgitserver/logger.py`

 * *Files identical despite different names*

### Comparing `btgitserver-2.0.1/setup.cfg` & `btgitserver-3.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -39,32 +39,31 @@
 	wheel >= 0.31
 packages = find:
 zip_safe = False
 scripts = 
 install_requires = 
 	btconfig>=4.4.4,<5.0.0
 	coloredlogs>=15.0.0,<16.0
-	flask>=2.0.0,<3.0
 	setuptools
-	dulwich==0.19.5
-	Flask
-	Flask-HTTPAuth
-	gunicorn
+	dulwich>=0.22.1,<1.0
+	flask>=3.0.3,<4.0.0
+	Flask-HTTPAuth>=4.8.0,<5.0.0
+	gunicorn>=20.1.0,<21.0.0
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-cov
 	coveralls
 	flake8
 	mypy
 
 [options.entry_points]
 console_scripts = 
-	bt.git-server=btgitserver.app:main
+	bt.git-server=btgitserver.app:start_api
 
 [options.data_files]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `btgitserver-2.0.1/setup.py` & `btgitserver-3.1.0/setup.py`

 * *Files identical despite different names*

