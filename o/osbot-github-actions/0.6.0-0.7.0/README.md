# Comparing `tmp/osbot_github_actions-0.6.0.tar.gz` & `tmp/osbot_github_actions-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osbot_github_actions-0.6.0.tar", max compression
+gzip compressed data, was "osbot_github_actions-0.7.0.tar", max compression
```

## Comparing `osbot_github_actions-0.6.0.tar` & `osbot_github_actions-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-05-28 19:49:05.718845 osbot_github_actions-0.6.0/LICENSE
--rw-r--r--   0        0        0      110 2024-05-28 19:49:05.718845 osbot_github_actions-0.6.0/README.md
--rw-r--r--   0        0        0       16 2024-05-28 19:49:05.718845 osbot_github_actions-0.6.0/osbot_github_actions/__init__.py
--rw-r--r--   0        0        0      471 2024-05-28 19:49:05.718845 osbot_github_actions-0.6.0/osbot_github_actions/utils/Version.py
--rw-r--r--   0        0        0        0 2024-05-28 19:49:05.718845 osbot_github_actions-0.6.0/osbot_github_actions/utils/__init__.py
--rw-r--r--   0        0        0        7 2024-05-28 19:49:05.718845 osbot_github_actions-0.6.0/osbot_github_actions/version
--rw-r--r--   0        0        0      618 2024-05-28 19:49:05.718845 osbot_github_actions-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 osbot_github_actions-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 23:37:14.275988 osbot_github_actions-0.7.0/LICENSE
+-rw-r--r--   0        0        0      110 2024-05-28 23:37:14.275988 osbot_github_actions-0.7.0/README.md
+-rw-r--r--   0        0        0       16 2024-05-28 23:37:14.275988 osbot_github_actions-0.7.0/osbot_github_actions/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-28 23:37:14.275988 osbot_github_actions-0.7.0/osbot_github_actions/utils/Version.py
+-rw-r--r--   0        0        0        0 2024-05-28 23:37:14.275988 osbot_github_actions-0.7.0/osbot_github_actions/utils/__init__.py
+-rw-r--r--   0        0        0        7 2024-05-28 23:37:14.275988 osbot_github_actions-0.7.0/osbot_github_actions/version
+-rw-r--r--   0        0        0      618 2024-05-28 23:37:14.275988 osbot_github_actions-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 osbot_github_actions-0.7.0/PKG-INFO
```

### Comparing `osbot_github_actions-0.6.0/LICENSE` & `osbot_github_actions-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osbot_github_actions-0.6.0/pyproject.toml` & `osbot_github_actions-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name        = "osbot_github_actions"
-version     = "v0.6.0"
+version     = "v0.7.0"
 description = "OWASP Security Bot - GitHub Actions"
 authors     = ["Dinis Cruz <dinis.cruz@owasp.org>"]
 license     = "MIT"
 readme      = "README.md"
 repository  = "https://github.com/owasp-sbot/OSBot-GitHub-Actions"
 homepage    = "https://github.com/owasp-sbot/OSBot-GitHub-Actions"
```

### Comparing `osbot_github_actions-0.6.0/PKG-INFO` & `osbot_github_actions-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osbot_github_actions
-Version: 0.6.0
+Version: 0.7.0
 Summary: OWASP Security Bot - GitHub Actions
 Home-page: https://github.com/owasp-sbot/OSBot-GitHub-Actions
 License: MIT
 Author: Dinis Cruz
 Author-email: dinis.cruz@owasp.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,9 +16,9 @@
 Project-URL: Repository, https://github.com/owasp-sbot/OSBot-GitHub-Actions
 Description-Content-Type: text/markdown
 
 # OSBot__Repo_Template
 
 ## Repo details
 
-![Current Release](https://img.shields.io/badge/release-v0.6.0-blue)
+![Current Release](https://img.shields.io/badge/release-v0.7.0-blue)
```

