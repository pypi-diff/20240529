# Comparing `tmp/pre_commit_update-0.3.1.post2.tar.gz` & `tmp/pre_commit_update-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_update-0.3.1.post2.tar", max compression
+gzip compressed data, was "pre_commit_update-0.3.2.tar", max compression
```

## Comparing `pre_commit_update-0.3.1.post2.tar` & `pre_commit_update-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/LICENSE
--rw-r--r--   0        0        0     6594 2024-04-26 20:49:14.183951 pre_commit_update-0.3.1.post2/README.md
--rw-r--r--   0        0        0     1680 2024-04-29 13:16:49.324994 pre_commit_update-0.3.1.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/__init__.py
--rw-r--r--   0        0        0     3167 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/cli.py
--rw-r--r--   0        0        0      229 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/__init__.py
--rw-r--r--   0        0        0      685 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/env.py
--rw-r--r--   0        0        0     3116 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/message.py
--rw-r--r--   0        0        0     4526 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/repo.py
--rw-r--r--   0        0        0      800 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/yaml.py
--rw-r--r--   0        0        0        0 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/py.typed
--rw-r--r--   0        0        0     2151 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/repo.py
--rw-r--r--   0        0        0      759 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1.post2/src/pre_commit_update/utils.py
--rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 pre_commit_update-0.3.1.post2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-04-26 20:43:34.039297 pre_commit_update-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6831 2024-05-28 23:39:28.839485 pre_commit_update-0.3.2/README.md
+-rw-r--r--   0        0        0     1675 2024-05-28 23:39:28.839485 pre_commit_update-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 20:43:34.039297 pre_commit_update-0.3.2/src/pre_commit_update/__init__.py
+-rw-r--r--   0        0        0     4830 2024-05-28 23:39:28.839485 pre_commit_update-0.3.2/src/pre_commit_update/cli.py
+-rw-r--r--   0        0        0      229 2024-04-26 20:43:34.039297 pre_commit_update-0.3.2/src/pre_commit_update/managers/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-26 20:43:34.039297 pre_commit_update-0.3.2/src/pre_commit_update/managers/env.py
+-rw-r--r--   0        0        0     3647 2024-05-28 23:39:28.839485 pre_commit_update-0.3.2/src/pre_commit_update/managers/message.py
+-rw-r--r--   0        0        0     4724 2024-05-28 23:39:28.839485 pre_commit_update-0.3.2/src/pre_commit_update/managers/repo.py
+-rw-r--r--   0        0        0      800 2024-04-26 20:43:34.039297 pre_commit_update-0.3.2/src/pre_commit_update/managers/yaml.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:43:34.039297 pre_commit_update-0.3.2/src/pre_commit_update/py.typed
+-rw-r--r--   0        0        0     2255 2024-05-28 23:39:28.842818 pre_commit_update-0.3.2/src/pre_commit_update/repo.py
+-rw-r--r--   0        0        0      861 2024-05-28 23:39:28.842818 pre_commit_update-0.3.2/src/pre_commit_update/utils.py
+-rw-r--r--   0        0        0     8395 1970-01-01 00:00:00.000000 pre_commit_update-0.3.2/PKG-INFO
```

### Comparing `pre_commit_update-0.3.1.post2/LICENSE` & `pre_commit_update-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post2/README.md` & `pre_commit_update-0.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 1. [ Reasoning ](#1-reasoning)
 2. [ Features ](#2-features)
 3. [ Installation ](#3-installation)
 4. [ Usage ](#4-usage)
     1. [ Pipeline usage example ](#1-pipeline-usage-example)
        1. [ GitLab job ](#a-gitlab-job)
     2. [ pre-commit hook usage example ](#2-pre-commit-hook-usage-example)
-    3. [ pyproject.toml usage example ](#3-pyprojecttoml-usage-example)
+5. [ Configuration ](#5-configuration)
 
 ## 1. Reasoning
 
 `pre-commit` is a nice little tool that helps you polish your code before releasing it into the wild.
 It is fairly easy to use. A single `pre-commit-config.yaml` file can hold multiple hooks (checks) that will go through
 your code or repository and do certain checks. The problem is that the file is static and once you pin your hook versions
 after a while they get outdated.
@@ -54,15 +54,14 @@
 
 ## 3. Installation
 
 `pre-commit-update` is available on PyPI:
 ```console 
 $ python -m pip install pre-commit-update
 ```
-Python >= 3.8 is supported.
 
 **NOTE:** Please make sure that `git` is installed.
 
 
 ## 4. Usage
 
 `pre-commit-update` CLI can be used as below:
@@ -70,14 +69,15 @@
 ```console
 Usage: pre-commit-update [OPTIONS]
 
 Options:
   -d, --dry-run / -nd, --no-dry-run             Dry run only checks for the new versions without updating  [default: nd]
   -a, --all-versions / -na, --no-all-versions   Include the alpha/beta versions when updating  [default: na]
   -v, --verbose / -nv, --no-verbose             Display the complete output  [default: nv]
+  -p, --preview / -np, --no-preview             Previews the cli configuration values by overwriting order (disables the actual cli work if enabled!)  [default: np]
   -e, --exclude REPO_URL_TRIM                   Exclude specific repo(s) by the `repo` url trim
   -k, --keep REPO_URL_TRIM                      Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)
   -h, --help                                    Show this message and exit.
 ```
 
 If you want to just check for updates (without updating `pre-commit-config.yaml`), for example, you would use:
 ```console
@@ -115,35 +115,38 @@
 
 ### 2) pre-commit hook usage example
 
 You can also use `pre-commit-update` as a hook in your `pre-commit` hooks:
 
 ```yaml
 - repo: https://gitlab.com/vojko.pribudic.foss/pre-commit-update
-  rev: v0.3.1  # Insert the latest tag here
+  rev: v0.3.2  # Insert the latest tag here
   hooks:
     - id: pre-commit-update
       args: [--dry-run, --exclude, black, --keep, isort]
 ```
 
-### 3) pyproject.toml usage example
+## 5. Configuration
 
 You can configure `pre-commit-update` in your `pyproject.toml` as below (feel free to do your own configuration):
 
 ```toml
 [tool.pre-commit-update]
 dry_run = true
 all_versions = false
 verbose = true
+preview = false
 exclude = ["isort"]
 keep = ["black"]
 ```
 
 **NOTE:** If some of the options are missing (for example `exclude` option), `pre-commit-update`
 will use default value for that option (default for `exclude` option would be an empty list).
 
 ***IMPORTANT*** If you invoke `pre-commit-update` with any arguments (e.g. `pre-commit-update -d`),
 `pyproject.toml` configuration will be **overridden**. This means that all the arguments passed while
-calling `pre-commit-update` will have priority over configuration defined inside `pyproject.toml`.
+calling `pre-commit-update` will have priority over the configuration defined inside `pyproject.toml`.
 If you want to override boolean flags, you can do so by passing the negative flag value.
 For example, given the configuration above, to override `verbose` flag from `pyproject.toml`, you
 would invoke `pre-commit-update` with either `--no-verbose` or `-nv`.
+
+You can always check the configuration overrides (priorities) by running `pre-commit-update -p` / `pre-commit-update --preview`
```

#### html2text {}

```diff
@@ -14,64 +14,67 @@
               grade/e727532ea95341b18ffd963e77605c2b?logo=codacy)
   _[_k_o_f_i_]pprree--ccoommmmiitt--uuppddaattee is a simple CLI tool to check and update pre-commit
                                     hooks.
 ## Table of contents 1. [ Reasoning ](#1-reasoning) 2. [ Features ](#2-
 features) 3. [ Installation ](#3-installation) 4. [ Usage ](#4-usage) 1.
 [ Pipeline usage example ](#1-pipeline-usage-example) 1. [ GitLab job ](#a-
 gitlab-job) 2. [ pre-commit hook usage example ](#2-pre-commit-hook-usage-
-example) 3. [ pyproject.toml usage example ](#3-pyprojecttoml-usage-example) ##
-1. Reasoning `pre-commit` is a nice little tool that helps you polish your code
-before releasing it into the wild. It is fairly easy to use. A single `pre-
-commit-config.yaml` file can hold multiple hooks (checks) that will go through
-your code or repository and do certain checks. The problem is that the file is
-static and once you pin your hook versions after a while they get outdated.
-`pre-commit-update` was created because there is no easy way to update your
-hooks by using `pre-commit autoupdate` as it is not versatile enough. ## 2.
-Features | Feature | pre-commit-update | pre-commit autoupdate | |:------------
---------------------------------------:|:-----------------:|:------------------
--------------------------:| | Dry run (checks for updates, does not update) |
-Yes | No | | Stable versions only | Yes | No | | Exclude repo(s) from update
-check | Yes | Workaround (updates only specified repo(s)) | | Keep repo(s)
-(checks for updates, does not update) | Yes | No | | Update by hash instead of
-tag | Yes | Yes | | Can be used as a pre-commit hook | Yes | No | | Can be
-configured in `pyproject.toml` | Yes | No | ## 3. Installation `pre-commit-
-update` is available on PyPI: ```console $ python -m pip install pre-commit-
-update ``` Python >= 3.8 is supported. **NOTE:** Please make sure that `git` is
-installed. ## 4. Usage `pre-commit-update` CLI can be used as below: ```console
-Usage: pre-commit-update [OPTIONS] Options: -d, --dry-run / -nd, --no-dry-run
-Dry run only checks for the new versions without updating [default: nd] -a, --
-all-versions / -na, --no-all-versions Include the alpha/beta versions when
-updating [default: na] -v, --verbose / -nv, --no-verbose Display the complete
-output [default: nv] -e, --exclude REPO_URL_TRIM Exclude specific repo(s) by
-the `repo` url trim -k, --keep REPO_URL_TRIM Keep the version of specific repo
-(s) by the `repo` url trim (still checks for the new versions) -h, --help Show
-this message and exit. ``` If you want to just check for updates (without
-updating `pre-commit-config.yaml`), for example, you would use: ```console $
-pre-commit-update -d ``` or ```console $ pre-commit-update --dry-run ```
-**NOTE:** If you are to use the `exclude` or `keep` options, please pass the
-repo url trim as a parameter. Keep in mind that if you have multiple hooks
-(id's) configured for a single repo and you `exclude` that repo, **NONE** of
-the hooks will be updated, whole repo will be excluded. Example of repo url
-trim: https://github.com/ambv/black -> `black` (you will only pass `black` as a
-parameter to `exclude` or `keep`) ### 1) Pipeline usage example #### a) GitLab
-job: ```yaml pre-commit-hooks-update: stage: update script: # install git if
-not present in the image - pip install pre-commit-update - pre-commit-update --
-dry-run except: - main when: manual allow_failure: true ``` **NOTE:** This is
-just an example, feel free to do your own configuration ### 2) pre-commit hook
-usage example You can also use `pre-commit-update` as a hook in your `pre-
-commit` hooks: ```yaml - repo: https://gitlab.com/vojko.pribudic.foss/pre-
-commit-update rev: v0.3.1 # Insert the latest tag here hooks: - id: pre-commit-
-update args: [--dry-run, --exclude, black, --keep, isort] ``` ### 3)
-pyproject.toml usage example You can configure `pre-commit-update` in your
-`pyproject.toml` as below (feel free to do your own configuration): ```toml
-[tool.pre-commit-update] dry_run = true all_versions = false verbose = true
-exclude = ["isort"] keep = ["black"] ``` **NOTE:** If some of the options are
-missing (for example `exclude` option), `pre-commit-update` will use default
-value for that option (default for `exclude` option would be an empty list).
-***IMPORTANT*** If you invoke `pre-commit-update` with any arguments (e.g.
-`pre-commit-update -d`), `pyproject.toml` configuration will be **overridden**.
-This means that all the arguments passed while calling `pre-commit-update` will
-have priority over configuration defined inside `pyproject.toml`. If you want
-to override boolean flags, you can do so by passing the negative flag value.
-For example, given the configuration above, to override `verbose` flag from
-`pyproject.toml`, you would invoke `pre-commit-update` with either `--no-
-verbose` or `-nv`.
+example) 5. [ Configuration ](#5-configuration) ## 1. Reasoning `pre-commit` is
+a nice little tool that helps you polish your code before releasing it into the
+wild. It is fairly easy to use. A single `pre-commit-config.yaml` file can hold
+multiple hooks (checks) that will go through your code or repository and do
+certain checks. The problem is that the file is static and once you pin your
+hook versions after a while they get outdated. `pre-commit-update` was created
+because there is no easy way to update your hooks by using `pre-commit
+autoupdate` as it is not versatile enough. ## 2. Features | Feature | pre-
+commit-update | pre-commit autoupdate | |:-------------------------------------
+-------------:|:-----------------:|:------------------------------------------
+-:| | Dry run (checks for updates, does not update) | Yes | No | | Stable
+versions only | Yes | No | | Exclude repo(s) from update check | Yes |
+Workaround (updates only specified repo(s)) | | Keep repo(s) (checks for
+updates, does not update) | Yes | No | | Update by hash instead of tag | Yes |
+Yes | | Can be used as a pre-commit hook | Yes | No | | Can be configured in
+`pyproject.toml` | Yes | No | ## 3. Installation `pre-commit-update` is
+available on PyPI: ```console $ python -m pip install pre-commit-update ```
+**NOTE:** Please make sure that `git` is installed. ## 4. Usage `pre-commit-
+update` CLI can be used as below: ```console Usage: pre-commit-update [OPTIONS]
+Options: -d, --dry-run / -nd, --no-dry-run Dry run only checks for the new
+versions without updating [default: nd] -a, --all-versions / -na, --no-all-
+versions Include the alpha/beta versions when updating [default: na] -v, --
+verbose / -nv, --no-verbose Display the complete output [default: nv] -p, --
+preview / -np, --no-preview Previews the cli configuration values by
+overwriting order (disables the actual cli work if enabled!) [default: np] -e,
+--exclude REPO_URL_TRIM Exclude specific repo(s) by the `repo` url trim -k, --
+keep REPO_URL_TRIM Keep the version of specific repo(s) by the `repo` url trim
+(still checks for the new versions) -h, --help Show this message and exit. ```
+If you want to just check for updates (without updating `pre-commit-
+config.yaml`), for example, you would use: ```console $ pre-commit-update -
+d ``` or ```console $ pre-commit-update --dry-run ``` **NOTE:** If you are to
+use the `exclude` or `keep` options, please pass the repo url trim as a
+parameter. Keep in mind that if you have multiple hooks (id's) configured for a
+single repo and you `exclude` that repo, **NONE** of the hooks will be updated,
+whole repo will be excluded. Example of repo url trim: https://github.com/ambv/
+black -> `black` (you will only pass `black` as a parameter to `exclude` or
+`keep`) ### 1) Pipeline usage example #### a) GitLab job: ```yaml pre-commit-
+hooks-update: stage: update script: # install git if not present in the image -
+pip install pre-commit-update - pre-commit-update --dry-run except: - main
+when: manual allow_failure: true ``` **NOTE:** This is just an example, feel
+free to do your own configuration ### 2) pre-commit hook usage example You can
+also use `pre-commit-update` as a hook in your `pre-commit` hooks: ```yaml -
+repo: https://gitlab.com/vojko.pribudic.foss/pre-commit-update rev: v0.3.2 #
+Insert the latest tag here hooks: - id: pre-commit-update args: [--dry-run, --
+exclude, black, --keep, isort] ``` ## 5. Configuration You can configure `pre-
+commit-update` in your `pyproject.toml` as below (feel free to do your own
+configuration): ```toml [tool.pre-commit-update] dry_run = true all_versions =
+false verbose = true preview = false exclude = ["isort"] keep = ["black"] ```
+**NOTE:** If some of the options are missing (for example `exclude` option),
+`pre-commit-update` will use default value for that option (default for
+`exclude` option would be an empty list). ***IMPORTANT*** If you invoke `pre-
+commit-update` with any arguments (e.g. `pre-commit-update -d`),
+`pyproject.toml` configuration will be **overridden**. This means that all the
+arguments passed while calling `pre-commit-update` will have priority over the
+configuration defined inside `pyproject.toml`. If you want to override boolean
+flags, you can do so by passing the negative flag value. For example, given the
+configuration above, to override `verbose` flag from `pyproject.toml`, you
+would invoke `pre-commit-update` with either `--no-verbose` or `-nv`. You can
+always check the configuration overrides (priorities) by running `pre-commit-
+update -p` / `pre-commit-update --preview`
```

### Comparing `pre_commit_update-0.3.1.post2/pyproject.toml` & `pre_commit_update-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pre-commit-update"
-version = "0.3.1post2"
+version = "0.3.2"
 description = "Simple CLI tool to check and update pre-commit hooks."
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = ["Vojko Pribudić <dmanthing@gmail.com>"]
 repository = "https://gitlab.com/vojko.pribudic.foss/pre-commit-update"
 readme = "README.md"
 license = "MIT"
 classifiers = [
```

### Comparing `pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/env.py` & `pre_commit_update-0.3.2/src/pre_commit_update/managers/env.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/message.py` & `pre_commit_update-0.3.2/src/pre_commit_update/managers/message.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class MessageManager:
     def __init__(self) -> None:
         self._to_update: MessageType = []
         self._no_update: MessageType = []
         self._excluded: MessageType = []
         self._kept: MessageType = []
+        self._warning: MessageType = []
 
     @property
     def to_update(self) -> MessageType:
         return self._to_update
 
     @property
     def no_update(self) -> MessageType:
@@ -35,14 +36,18 @@
     def excluded(self) -> MessageType:
         return self._excluded
 
     @property
     def kept(self) -> MessageType:
         return self._kept
 
+    @property
+    def warning(self) -> MessageType:
+        return self._warning
+
     def add_to_update_message(
         self, name: str, current_version: str, latest_version: str
     ) -> None:
         to_update_message: str = (
             f"{name} - {get_color(current_version, 'yellow')} -> {get_color(latest_version, 'red')}"
         )
         self._to_update.append(
@@ -94,14 +99,26 @@
                 icon="◉",
                 icon_alt="●",
                 text="[kept]",
                 color="blue",
             )
         )
 
+    def add_warning_message(self, name: str, version: str, reason: str) -> None:
+        warning_message: str = f"{name} - {get_color(version, 'yellow')} ({reason})"
+        self._warning.append(
+            Message(
+                message=warning_message,
+                icon="⚠",
+                icon_alt="▲",
+                text="[warning]",
+                color="yellow",
+            )
+        )
+
     @staticmethod
     def output_messages(messages: MessageType) -> None:
         for message in messages:
             for symbol in (message["icon"], message["icon_alt"], message["text"]):
                 try:
                     click.echo(
                         f"{message['message']} {get_color(click.style(symbol, bold=True), message['color'])}"
```

### Comparing `pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/repo.py` & `pre_commit_update-0.3.2/src/pre_commit_update/managers/repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,14 +101,19 @@
     def _is_repo_kept(self, repo: Repo) -> bool:
         return repo.name in self._keep
 
     def get_updates(self, messages: MessageManager) -> None:
         for i, repo in enumerate(self._repos_list):
             if repo.is_local:
                 continue
+            if not repo.has_git_tags:
+                messages.add_warning_message(
+                    repo.name, repo.current_version, "no-tags-fetched"
+                )
+                continue
             if self._is_repo_excluded(repo):
                 messages.add_excluded_message(repo.name, repo.current_version)
                 continue
             if self._is_repo_kept(repo):
                 messages.add_kept_message(
                     repo.name, repo.current_version, repo.latest_version
                 )
```

### Comparing `pre_commit_update-0.3.1.post2/src/pre_commit_update/managers/yaml.py` & `pre_commit_update-0.3.2/src/pre_commit_update/managers/yaml.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post2/src/pre_commit_update/repo.py` & `pre_commit_update-0.3.2/src/pre_commit_update/repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
             )
 
     @property
     def is_local(self) -> bool:
         return not self._url.startswith("http")
 
     @property
+    def has_git_tags(self) -> bool:
+        return len(self._git_tags) > 0
+
+    @property
     def name(self) -> str:
         return self._name
 
     @property
     def current_version(self) -> str:
         return self._current_version
 
@@ -54,12 +58,12 @@
     def _get_latest_hash(self) -> str:
         return git.cmd.Git().ls_remote("--exit-code", self._url, "HEAD").split()[0]
 
     def _get_latest_version(self, all_versions: bool) -> str:
         try:
             parse_version(self._current_version)
             return self._get_latest_tag(all_versions)
-        except InvalidVersion:
+        except (InvalidVersion, IndexError):
             pass
         if self._is_hash:
             return self._get_latest_hash()
         return self._current_version
```

### Comparing `pre_commit_update-0.3.1.post2/src/pre_commit_update/utils.py` & `pre_commit_update-0.3.2/src/pre_commit_update/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,7 +25,11 @@
     try:
         toml_file: PyProject = PyProject.load(
             os.path.join(os.getcwd(), "pyproject.toml")
         )
         return {**defaults, **toml_file.tool["pre-commit-update"]}
     except (FileNotFoundError, KeyError):
         return defaults
+
+
+def get_dict_diffs(d1: Dict, d2: Dict) -> Dict:
+    return {k: d2[k] for k in d2 if d2[k] != d1[k]}
```

### Comparing `pre_commit_update-0.3.1.post2/PKG-INFO` & `pre_commit_update-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit-update
-Version: 0.3.1.post2
+Version: 0.3.2
 Summary: Simple CLI tool to check and update pre-commit hooks.
 Home-page: https://gitlab.com/vojko.pribudic.foss/pre-commit-update
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
@@ -58,15 +58,15 @@
 1. [ Reasoning ](#1-reasoning)
 2. [ Features ](#2-features)
 3. [ Installation ](#3-installation)
 4. [ Usage ](#4-usage)
     1. [ Pipeline usage example ](#1-pipeline-usage-example)
        1. [ GitLab job ](#a-gitlab-job)
     2. [ pre-commit hook usage example ](#2-pre-commit-hook-usage-example)
-    3. [ pyproject.toml usage example ](#3-pyprojecttoml-usage-example)
+5. [ Configuration ](#5-configuration)
 
 ## 1. Reasoning
 
 `pre-commit` is a nice little tool that helps you polish your code before releasing it into the wild.
 It is fairly easy to use. A single `pre-commit-config.yaml` file can hold multiple hooks (checks) that will go through
 your code or repository and do certain checks. The problem is that the file is static and once you pin your hook versions
 after a while they get outdated.
@@ -90,15 +90,14 @@
 
 ## 3. Installation
 
 `pre-commit-update` is available on PyPI:
 ```console 
 $ python -m pip install pre-commit-update
 ```
-Python >= 3.8 is supported.
 
 **NOTE:** Please make sure that `git` is installed.
 
 
 ## 4. Usage
 
 `pre-commit-update` CLI can be used as below:
@@ -106,14 +105,15 @@
 ```console
 Usage: pre-commit-update [OPTIONS]
 
 Options:
   -d, --dry-run / -nd, --no-dry-run             Dry run only checks for the new versions without updating  [default: nd]
   -a, --all-versions / -na, --no-all-versions   Include the alpha/beta versions when updating  [default: na]
   -v, --verbose / -nv, --no-verbose             Display the complete output  [default: nv]
+  -p, --preview / -np, --no-preview             Previews the cli configuration values by overwriting order (disables the actual cli work if enabled!)  [default: np]
   -e, --exclude REPO_URL_TRIM                   Exclude specific repo(s) by the `repo` url trim
   -k, --keep REPO_URL_TRIM                      Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)
   -h, --help                                    Show this message and exit.
 ```
 
 If you want to just check for updates (without updating `pre-commit-config.yaml`), for example, you would use:
 ```console
@@ -151,36 +151,39 @@
 
 ### 2) pre-commit hook usage example
 
 You can also use `pre-commit-update` as a hook in your `pre-commit` hooks:
 
 ```yaml
 - repo: https://gitlab.com/vojko.pribudic.foss/pre-commit-update
-  rev: v0.3.1  # Insert the latest tag here
+  rev: v0.3.2  # Insert the latest tag here
   hooks:
     - id: pre-commit-update
       args: [--dry-run, --exclude, black, --keep, isort]
 ```
 
-### 3) pyproject.toml usage example
+## 5. Configuration
 
 You can configure `pre-commit-update` in your `pyproject.toml` as below (feel free to do your own configuration):
 
 ```toml
 [tool.pre-commit-update]
 dry_run = true
 all_versions = false
 verbose = true
+preview = false
 exclude = ["isort"]
 keep = ["black"]
 ```
 
 **NOTE:** If some of the options are missing (for example `exclude` option), `pre-commit-update`
 will use default value for that option (default for `exclude` option would be an empty list).
 
 ***IMPORTANT*** If you invoke `pre-commit-update` with any arguments (e.g. `pre-commit-update -d`),
 `pyproject.toml` configuration will be **overridden**. This means that all the arguments passed while
-calling `pre-commit-update` will have priority over configuration defined inside `pyproject.toml`.
+calling `pre-commit-update` will have priority over the configuration defined inside `pyproject.toml`.
 If you want to override boolean flags, you can do so by passing the negative flag value.
 For example, given the configuration above, to override `verbose` flag from `pyproject.toml`, you
 would invoke `pre-commit-update` with either `--no-verbose` or `-nv`.
 
+You can always check the configuration overrides (priorities) by running `pre-commit-update -p` / `pre-commit-update --preview`
+
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: pre-commit-update Version: 0.3.1.post2 Summary:
-Simple CLI tool to check and update pre-commit hooks. Home-page: https://
-gitlab.com/vojko.pribudic.foss/pre-commit-update License: MIT Author: Vojko
-PribudiÄ Author-email: dmanthing@gmail.com Maintainer: Vojko PribudiÄ
-Maintainer-email: dmanthing@gmail.com Requires-Python: >=3.8 Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Web
-Environment Classifier: Intended Audience :: Developers Classifier: License ::
-OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
-Software Development :: Libraries Requires-Dist: GitPython (>=3.1) Requires-
-Dist: click (>=8.1) Requires-Dist: packaging (>=23.2) Requires-Dist: pyproject-
-parser (>=0.9) Requires-Dist: ruamel.yaml (>=0.18) Project-URL: Changelog,
-https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/releases Project-
-URL: Repository, https://gitlab.com/vojko.pribudic.foss/pre-commit-update
-Project-URL: Tracker, https://gitlab.com/vojko.pribudic.foss/pre-commit-update/
--/issues Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: pre-commit-update Version: 0.3.2 Summary: Simple
+CLI tool to check and update pre-commit hooks. Home-page: https://gitlab.com/
+vojko.pribudic.foss/pre-commit-update License: MIT Author: Vojko PribudiÄ
+Author-email: dmanthing@gmail.com Maintainer: Vojko PribudiÄ Maintainer-email:
+dmanthing@gmail.com Requires-Python: >=3.8 Classifier: Development Status :: 5
+- Production/Stable Classifier: Environment :: Web Environment Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Topic :: Software
+Development :: Libraries Requires-Dist: GitPython (>=3.1) Requires-Dist: click
+(>=8.1) Requires-Dist: packaging (>=23.2) Requires-Dist: pyproject-parser
+(>=0.9) Requires-Dist: ruamel.yaml (>=0.18) Project-URL: Changelog, https://
+gitlab.com/vojko.pribudic.foss/pre-commit-update/-/releases Project-URL:
+Repository, https://gitlab.com/vojko.pribudic.foss/pre-commit-update Project-
+URL: Tracker, https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/issues
+Description-Content-Type: text/markdown
                         ************ pprree--ccoommmmiitt--uuppddaattee ************
   ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update) ![PePy -
 Downloads](https://pepy.tech/badge/pre-commit-update) ![Gitlab Pipeline Status]
    (https://img.shields.io/gitlab/pipeline-status/vojko.pribudic.foss%2Fpre-
       commit-update?branch=main&label=pipeline) ![GitLab Issues](https://
  img.shields.io/gitlab/issues/open/vojko.pribudic.foss%2Fpre-commit-update) !
         [GitLab Last Commit](https://img.shields.io/gitlab/last-commit/
@@ -35,64 +35,67 @@
               grade/e727532ea95341b18ffd963e77605c2b?logo=codacy)
   _[_k_o_f_i_]pprree--ccoommmmiitt--uuppddaattee is a simple CLI tool to check and update pre-commit
                                     hooks.
 ## Table of contents 1. [ Reasoning ](#1-reasoning) 2. [ Features ](#2-
 features) 3. [ Installation ](#3-installation) 4. [ Usage ](#4-usage) 1.
 [ Pipeline usage example ](#1-pipeline-usage-example) 1. [ GitLab job ](#a-
 gitlab-job) 2. [ pre-commit hook usage example ](#2-pre-commit-hook-usage-
-example) 3. [ pyproject.toml usage example ](#3-pyprojecttoml-usage-example) ##
-1. Reasoning `pre-commit` is a nice little tool that helps you polish your code
-before releasing it into the wild. It is fairly easy to use. A single `pre-
-commit-config.yaml` file can hold multiple hooks (checks) that will go through
-your code or repository and do certain checks. The problem is that the file is
-static and once you pin your hook versions after a while they get outdated.
-`pre-commit-update` was created because there is no easy way to update your
-hooks by using `pre-commit autoupdate` as it is not versatile enough. ## 2.
-Features | Feature | pre-commit-update | pre-commit autoupdate | |:------------
---------------------------------------:|:-----------------:|:------------------
--------------------------:| | Dry run (checks for updates, does not update) |
-Yes | No | | Stable versions only | Yes | No | | Exclude repo(s) from update
-check | Yes | Workaround (updates only specified repo(s)) | | Keep repo(s)
-(checks for updates, does not update) | Yes | No | | Update by hash instead of
-tag | Yes | Yes | | Can be used as a pre-commit hook | Yes | No | | Can be
-configured in `pyproject.toml` | Yes | No | ## 3. Installation `pre-commit-
-update` is available on PyPI: ```console $ python -m pip install pre-commit-
-update ``` Python >= 3.8 is supported. **NOTE:** Please make sure that `git` is
-installed. ## 4. Usage `pre-commit-update` CLI can be used as below: ```console
-Usage: pre-commit-update [OPTIONS] Options: -d, --dry-run / -nd, --no-dry-run
-Dry run only checks for the new versions without updating [default: nd] -a, --
-all-versions / -na, --no-all-versions Include the alpha/beta versions when
-updating [default: na] -v, --verbose / -nv, --no-verbose Display the complete
-output [default: nv] -e, --exclude REPO_URL_TRIM Exclude specific repo(s) by
-the `repo` url trim -k, --keep REPO_URL_TRIM Keep the version of specific repo
-(s) by the `repo` url trim (still checks for the new versions) -h, --help Show
-this message and exit. ``` If you want to just check for updates (without
-updating `pre-commit-config.yaml`), for example, you would use: ```console $
-pre-commit-update -d ``` or ```console $ pre-commit-update --dry-run ```
-**NOTE:** If you are to use the `exclude` or `keep` options, please pass the
-repo url trim as a parameter. Keep in mind that if you have multiple hooks
-(id's) configured for a single repo and you `exclude` that repo, **NONE** of
-the hooks will be updated, whole repo will be excluded. Example of repo url
-trim: https://github.com/ambv/black -> `black` (you will only pass `black` as a
-parameter to `exclude` or `keep`) ### 1) Pipeline usage example #### a) GitLab
-job: ```yaml pre-commit-hooks-update: stage: update script: # install git if
-not present in the image - pip install pre-commit-update - pre-commit-update --
-dry-run except: - main when: manual allow_failure: true ``` **NOTE:** This is
-just an example, feel free to do your own configuration ### 2) pre-commit hook
-usage example You can also use `pre-commit-update` as a hook in your `pre-
-commit` hooks: ```yaml - repo: https://gitlab.com/vojko.pribudic.foss/pre-
-commit-update rev: v0.3.1 # Insert the latest tag here hooks: - id: pre-commit-
-update args: [--dry-run, --exclude, black, --keep, isort] ``` ### 3)
-pyproject.toml usage example You can configure `pre-commit-update` in your
-`pyproject.toml` as below (feel free to do your own configuration): ```toml
-[tool.pre-commit-update] dry_run = true all_versions = false verbose = true
-exclude = ["isort"] keep = ["black"] ``` **NOTE:** If some of the options are
-missing (for example `exclude` option), `pre-commit-update` will use default
-value for that option (default for `exclude` option would be an empty list).
-***IMPORTANT*** If you invoke `pre-commit-update` with any arguments (e.g.
-`pre-commit-update -d`), `pyproject.toml` configuration will be **overridden**.
-This means that all the arguments passed while calling `pre-commit-update` will
-have priority over configuration defined inside `pyproject.toml`. If you want
-to override boolean flags, you can do so by passing the negative flag value.
-For example, given the configuration above, to override `verbose` flag from
-`pyproject.toml`, you would invoke `pre-commit-update` with either `--no-
-verbose` or `-nv`.
+example) 5. [ Configuration ](#5-configuration) ## 1. Reasoning `pre-commit` is
+a nice little tool that helps you polish your code before releasing it into the
+wild. It is fairly easy to use. A single `pre-commit-config.yaml` file can hold
+multiple hooks (checks) that will go through your code or repository and do
+certain checks. The problem is that the file is static and once you pin your
+hook versions after a while they get outdated. `pre-commit-update` was created
+because there is no easy way to update your hooks by using `pre-commit
+autoupdate` as it is not versatile enough. ## 2. Features | Feature | pre-
+commit-update | pre-commit autoupdate | |:-------------------------------------
+-------------:|:-----------------:|:------------------------------------------
+-:| | Dry run (checks for updates, does not update) | Yes | No | | Stable
+versions only | Yes | No | | Exclude repo(s) from update check | Yes |
+Workaround (updates only specified repo(s)) | | Keep repo(s) (checks for
+updates, does not update) | Yes | No | | Update by hash instead of tag | Yes |
+Yes | | Can be used as a pre-commit hook | Yes | No | | Can be configured in
+`pyproject.toml` | Yes | No | ## 3. Installation `pre-commit-update` is
+available on PyPI: ```console $ python -m pip install pre-commit-update ```
+**NOTE:** Please make sure that `git` is installed. ## 4. Usage `pre-commit-
+update` CLI can be used as below: ```console Usage: pre-commit-update [OPTIONS]
+Options: -d, --dry-run / -nd, --no-dry-run Dry run only checks for the new
+versions without updating [default: nd] -a, --all-versions / -na, --no-all-
+versions Include the alpha/beta versions when updating [default: na] -v, --
+verbose / -nv, --no-verbose Display the complete output [default: nv] -p, --
+preview / -np, --no-preview Previews the cli configuration values by
+overwriting order (disables the actual cli work if enabled!) [default: np] -e,
+--exclude REPO_URL_TRIM Exclude specific repo(s) by the `repo` url trim -k, --
+keep REPO_URL_TRIM Keep the version of specific repo(s) by the `repo` url trim
+(still checks for the new versions) -h, --help Show this message and exit. ```
+If you want to just check for updates (without updating `pre-commit-
+config.yaml`), for example, you would use: ```console $ pre-commit-update -
+d ``` or ```console $ pre-commit-update --dry-run ``` **NOTE:** If you are to
+use the `exclude` or `keep` options, please pass the repo url trim as a
+parameter. Keep in mind that if you have multiple hooks (id's) configured for a
+single repo and you `exclude` that repo, **NONE** of the hooks will be updated,
+whole repo will be excluded. Example of repo url trim: https://github.com/ambv/
+black -> `black` (you will only pass `black` as a parameter to `exclude` or
+`keep`) ### 1) Pipeline usage example #### a) GitLab job: ```yaml pre-commit-
+hooks-update: stage: update script: # install git if not present in the image -
+pip install pre-commit-update - pre-commit-update --dry-run except: - main
+when: manual allow_failure: true ``` **NOTE:** This is just an example, feel
+free to do your own configuration ### 2) pre-commit hook usage example You can
+also use `pre-commit-update` as a hook in your `pre-commit` hooks: ```yaml -
+repo: https://gitlab.com/vojko.pribudic.foss/pre-commit-update rev: v0.3.2 #
+Insert the latest tag here hooks: - id: pre-commit-update args: [--dry-run, --
+exclude, black, --keep, isort] ``` ## 5. Configuration You can configure `pre-
+commit-update` in your `pyproject.toml` as below (feel free to do your own
+configuration): ```toml [tool.pre-commit-update] dry_run = true all_versions =
+false verbose = true preview = false exclude = ["isort"] keep = ["black"] ```
+**NOTE:** If some of the options are missing (for example `exclude` option),
+`pre-commit-update` will use default value for that option (default for
+`exclude` option would be an empty list). ***IMPORTANT*** If you invoke `pre-
+commit-update` with any arguments (e.g. `pre-commit-update -d`),
+`pyproject.toml` configuration will be **overridden**. This means that all the
+arguments passed while calling `pre-commit-update` will have priority over the
+configuration defined inside `pyproject.toml`. If you want to override boolean
+flags, you can do so by passing the negative flag value. For example, given the
+configuration above, to override `verbose` flag from `pyproject.toml`, you
+would invoke `pre-commit-update` with either `--no-verbose` or `-nv`. You can
+always check the configuration overrides (priorities) by running `pre-commit-
+update -p` / `pre-commit-update --preview`
```

