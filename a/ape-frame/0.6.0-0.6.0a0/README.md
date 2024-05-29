# Comparing `tmp/ape-frame-0.6.0.tar.gz` & `tmp/ape-frame-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-frame-0.6.0.tar", last modified: Wed May 29 20:16:22 2024, max compression
+gzip compressed data, was "ape-frame-0.6.0a0.tar", last modified: Tue Jun 27 13:59:53 2023, max compression
```

## Comparing `ape-frame-0.6.0.tar` & `ape-frame-0.6.0a0.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:16:22.251627 ape-frame-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:16:22.251627 ape-frame-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:16:22.251627 ape-frame-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:16:22.251627 ape-frame-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-29 20:15:30.000000 ape-frame-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-29 20:15:30.000000 ape-frame-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-29 20:15:30.000000 ape-frame-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 20:16:22.251627 ape-frame-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 20:15:30.000000 ape-frame-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:16:22.251627 ape-frame-0.6.0/ape_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-29 20:15:30.000000 ape-frame-0.6.0/ape_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-29 20:15:30.000000 ape-frame-0.6.0/ape_frame/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-29 20:15:30.000000 ape-frame-0.6.0/ape_frame/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-29 20:15:30.000000 ape-frame-0.6.0/ape_frame/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:15:30.000000 ape-frame-0.6.0/ape_frame/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 20:16:22.000000 ape-frame-0.6.0/ape_frame/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:16:22.251627 ape-frame-0.6.0/ape_frame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 20:16:22.000000 ape-frame-0.6.0/ape_frame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-29 20:16:22.000000 ape-frame-0.6.0/ape_frame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:16:22.000000 ape-frame-0.6.0/ape_frame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:16:22.000000 ape-frame-0.6.0/ape_frame.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-29 20:16:22.000000 ape-frame-0.6.0/ape_frame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 20:16:22.000000 ape-frame-0.6.0/ape_frame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 20:15:30.000000 ape-frame-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 20:16:22.251627 ape-frame-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-29 20:15:30.000000 ape-frame-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:16:22.251627 ape-frame-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:15:30.000000 ape-frame-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 20:15:30.000000 ape-frame-0.6.0/tests/test_accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/ape_frame/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-27 13:59:52.000000 ape-frame-0.6.0a0/ape_frame/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/ape_frame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 13:59:53.336301 ape-frame-0.6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/tests/__init__.py
```

### Comparing `ape-frame-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ---
 name: Feature request
 about: Request a new feature, or an improvement to existing functionality.
-labels: enhancement
+labels: 'enhancement'
 ---
 
 ### Overview
 
 Provide a simple overview of what you wish to see added. Please include:
 
-- What you are trying to do
-- Why Ape's current functionality is inadequate to address your goal
+* What you are trying to do
+* Why Ape's current functionality is inadequate to address your goal
 
 ### Specification
 
 Describe the syntax and semantics of how you would like to see this feature implemented. The more detailed the better!
 
 Remember, your feature is much more likely to be included if it does not involve any breaking changes.
```

### Comparing `ape-frame-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 ---
 name: Work item
 about: New work item for Ape team
-labels: backlog
+labels: 'backlog'
+
 ---
 
 ### Elevator pitch:
-
 <!-- 1-2 line summary of the scope of this work item -->
 
 ### Value:
-
 <!--
   Who is this for?
   Persona or group of people whom will derive value from the scenario.
   What benefits will be achieved or business metrics improved?
 -->
 
 ### Dependencies:
-
 <!-- Call out key people, teams, tech dependencies, or assumptions. -->
 
 ### Design approach:
-
 <!--
   Free text / diagram / whiteboard picture / etc. that clearly shows your approach and considerations to build the task list.
   Existing code patterns in production code base that you will base your work off of.
 -->
 
 ### Task list:
-
 <!-- Bulleted list describing the exit criteria, desired end state and any documentation, monitors, work for DRI, etc. that will need to be added to make sure someone else can support once it's live. -->
-
-- [ ] Tasks go here
+* [ ] Tasks go here
 
 ### Estimated completion date:
 
-### Design review:
 
+### Design review:
 <!-- 1-2 people needed for signoff -->
-
 Do not signoff unless:
-
-- 1. agreed the tasks and design approach will achieve acceptance, and
-- 2. the work can be completed by one person within the SLA.
-     Design reviewers should consider simpler approaches to achieve goals.
+- 1) agreed the tasks and design approach will achieve acceptance, and
+- 2) the work can be completed by one person within the SLA.
+Design reviewers should consider simpler approaches to achieve goals.
 
 (Please leave a comment to sign off)
```

### Comparing `ape-frame-0.6.0/.github/release-drafter.yml` & `ape-frame-0.6.0a0/.github/release-drafter.yml`

 * *Files 22% similar despite different names*

```diff
@@ -27,11 +27,11 @@
   patch:
     labels:
       - 'patch'
   default: patch
 
 template: |
   ## Changes
-
+  
   $CHANGES
-
+  
   Special thanks to: $CONTRIBUTORS
```

### Comparing `ape-frame-0.6.0/.github/workflows/commitlint.yaml` & `ape-frame-0.6.0a0/.github/workflows/commitlint.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v4
+        - uses: actions/checkout@v2
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v5
+          uses: actions/setup-python@v2
           with:
-              python-version: "3.10"
+              python-version: 3.8
 
         - name: Install Dependencies
-          run: pip install commitizen
+          run: pip install .[dev]
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-frame-0.6.0/.github/workflows/prtitle.yaml` & `ape-frame-0.6.0a0/.github/workflows/title.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v4
+        - uses: actions/checkout@v2
 
         - name: Setup Python
-          uses: actions/setup-python@v5
+          uses: actions/setup-python@v2
           with:
-              python-version: "3.10"
+              python-version: 3.8
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-frame-0.6.0/.github/workflows/publish.yaml` & `ape-frame-0.6.0a0/.github/workflows/publish.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v4
+    - uses: actions/checkout@v2
 
     - name: Set up Python
-      uses: actions/setup-python@v5
+      uses: actions/setup-python@v2
       with:
-        python-version: "3.10"
+        python-version: 3.8
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
-
+        
     - name: Build
       run: python setup.py sdist bdist_wheel
 
     - name: Publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `ape-frame-0.6.0/.github/workflows/test.yaml` & `ape-frame-0.6.0a0/.github/workflows/test.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,69 @@
 on: ["push", "pull_request"]
 
 name: Test
 
-concurrency:
-  # Cancel older, in-progress jobs from the same PR, same workflow.
-  # use run_id if the job is triggered by a push to ensure
-  # push-triggered jobs to not get canceled.
-  group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
-  cancel-in-progress: true
-
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v4
+        - uses: actions/checkout@v2
 
         - name: Setup Python
-          uses: actions/setup-python@v5
+          uses: actions/setup-python@v2
           with:
-              python-version: "3.10"
+              python-version: 3.8
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
           run: black --check .
 
-        - name: Run isort
-          run: isort --check-only .
-
         - name: Run flake8
           run: flake8 .
 
-        - name: Run mdformat
-          run: mdformat . --check
+        - name: Run isort
+          run: isort --check-only .
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v4
+        - uses: actions/checkout@v2
 
         - name: Setup Python
-          uses: actions/setup-python@v5
+          uses: actions/setup-python@v2
           with:
-              python-version: "3.10"
+              python-version: 3.8
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                # TODO: Replace with macos-latest when works again.
-                #   https://github.com/actions/setup-python/issues/808
-                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
+                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
+                python-version: [3.8, 3.9, "3.10"]
 
         steps:
-        - uses: actions/checkout@v4
+        - uses: actions/checkout@v2
 
         - name: Setup Python
-          uses: actions/setup-python@v5
+          uses: actions/setup-python@v2
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
@@ -87,19 +75,19 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v4
+#        - uses: actions/checkout@v2
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v5
+#          uses: actions/setup-python@v2
 #          with:
-#              python-version: "3.10"
+#              python-version: 3.8
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-frame-0.6.0/.gitignore` & `ape-frame-0.6.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-frame-0.6.0/CONTRIBUTING.md` & `ape-frame-0.6.0a0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
-Join the ApeWorX [Discord](https://discord.gg/apeworx) if you have any questions.
+Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
```

### Comparing `ape-frame-0.6.0/LICENSE` & `ape-frame-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-frame-0.6.0/PKG-INFO` & `ape-frame-0.6.0a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: ape-frame
-Version: 0.6.0
+Version: 0.6.0a0
 Summary: ape-frame: Frame (https://frame.sh) account plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-frame
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
+Description: # Quick Start
+        
+        TODO: Description
+        
+        ## Dependencies
+        
+        * [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+        
+        ## Installation
+        
+        ### via `pip`
+        
+        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+        
+        ```bash
+        pip install ape-frame
+        ```
+        
+        ### via `setuptools`
+        
+        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+        
+        ```bash
+        git clone https://github.com/ApeWorX/ape-frame.git
+        cd ape-frame
+        python3 setup.py install
+        ```
+        
+        ## Quick Usage
+        
+        TODO: Describe library overview in code
+        
+        ## Development
+        
+        This project is in development and should be considered a beta.
+        Things might not be in their final state and breaking changes may occur.
+        Comments, questions, criticisms and pull requests are welcomed.
+        
 Keywords: ethereum
-Classifier: Development Status :: 4 - Beta
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
-License-File: LICENSE
-
-# Quick Start
-
-TODO: Description
-
-## Dependencies
-
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
-
-## Installation
-
-### via `pip`
-
-You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-
-```bash
-pip install ape-frame
-```
-
-### via `setuptools`
-
-You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-
-```bash
-git clone https://github.com/ApeWorX/ape-frame.git
-cd ape-frame
-python3 setup.py install
-```
-
-## Quick Usage
-
-TODO: Describe library overview in code
-
-## Development
-
-This project is in development and should be considered a beta.
-Things might not be in their final state and breaking changes may occur.
-Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-frame-0.6.0/README.md` & `ape-frame-0.6.0a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 TODO: Description
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+* [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-frame-0.6.0/ape_frame/__init__.py` & `ape-frame-0.6.0a0/ape_frame/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 
 from .accounts import AccountContainer, FrameAccount
 from .providers import FrameProvider
 
 NETWORKS = {
     "ethereum": [
         "mainnet",
+        "goerli",
         "sepolia",
     ],
     "arbitrum": [
         "mainnet",
-        "sepolia",
     ],
     "optimism": [
         "mainnet",
-        "sepolia",
     ],
     "polygon": [
         "mainnet",
-        "amoy",
     ],
 }
 
 
 @plugins.register(plugins.AccountPlugin)
 def account_types():
     return AccountContainer, FrameAccount
```

### Comparing `ape-frame-0.6.0/ape_frame/providers.py` & `ape-frame-0.6.0a0/ape_frame/providers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 from typing import Any
 
-from ape.api import UpstreamProvider
+from ape.api import UpstreamProvider, Web3Provider
 from ape.exceptions import ProviderError
-from ape_ethereum.provider import Web3Provider
 from eth_utils import to_hex
-from requests import HTTPError
+from requests import HTTPError  # type: ignore[import]
 from web3 import HTTPProvider, Web3
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
 from web3.middleware import geth_poa_middleware
 
-from ape_frame.exceptions import FrameNotConnectedError, FrameProviderError
+from .exceptions import FrameNotConnectedError, FrameProviderError
 
 
 class FrameProvider(Web3Provider, UpstreamProvider):
     _original_chain_id: int = -1
 
     @property
     def uri(self) -> str:
         # TODO: Add config for this
-        return "http://127.0.0.1:1248"
+        return "http://127.0.01:1248"
 
     @property
     def connection_str(self) -> str:
         return self.uri
 
     def connect(self):
-        headers = {
-            "Origin": "Ape/ape-frame/provider",
-            "User-Agent": "ape-frame/0.1.0",
-            "Content-Type": "application/json",
-        }
-        self._web3 = Web3(HTTPProvider(self.uri, request_kwargs={"headers": headers}))
+        self._web3 = Web3(HTTPProvider(self.uri))
 
         if "Frame" not in self._web3.client_version:
             raise FrameNotConnectedError()
 
         self._original_chain_id = self._web3.eth.chain_id
 
         # NOTE: Make sure Frame is on the right network
         if self.network.chain_id != self._original_chain_id:
             self._make_request(
                 "wallet_switchEthereumChain",
                 [{"chainId": to_hex(self.network.chain_id)}],
             )
 
         # Any chain that *began* as PoA needs the middleware for pre-merge blocks
-        ethereum_sepolia = 11155111
-        optimism = (10, 11155420)
-        polygon = (137, 80002)
+        ethereum_goerli = 5
+        optimism = (10, 420)
+        polygon = (137, 80001)
         try:
-            if self._web3.eth.chain_id in (ethereum_sepolia, *optimism, *polygon):
+
+            if self._web3.eth.chain_id in (ethereum_goerli, *optimism, *polygon):
                 self._web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
             self._web3.eth.set_gas_price_strategy(rpc_gas_price_strategy)
         except Exception as err:
             raise ProviderError(f"Failed to connect to Frame.\n{repr(err)}") from err
 
     def disconnect(self):
@@ -61,19 +56,19 @@
         self._make_request(
             "wallet_switchEthereumChain",
             [{"chainId": to_hex(self._original_chain_id)}],
         )
 
         self._web3 = None
 
-    def _make_request(self, endpoint: str, parameters: list) -> Any:  # type: ignore[override]
+    def _make_request(self, endpoint: str, parameters: list) -> Any:
         try:
             return super()._make_request(endpoint, parameters)
         except HTTPError as err:
-            response_data = err.response.json() if err.response else {}
+            response_data = err.response.json()
             if "error" not in response_data:
                 raise FrameProviderError(str(err)) from err
 
             error_data = response_data["error"]
             message = (
                 error_data.get("message", str(error_data))
                 if isinstance(error_data, dict)
```

### Comparing `ape-frame-0.6.0/ape_frame.egg-info/PKG-INFO` & `ape-frame-0.6.0a0/ape_frame.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: ape-frame
-Version: 0.6.0
+Version: 0.6.0a0
 Summary: ape-frame: Frame (https://frame.sh) account plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-frame
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
+Description: # Quick Start
+        
+        TODO: Description
+        
+        ## Dependencies
+        
+        * [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+        
+        ## Installation
+        
+        ### via `pip`
+        
+        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+        
+        ```bash
+        pip install ape-frame
+        ```
+        
+        ### via `setuptools`
+        
+        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+        
+        ```bash
+        git clone https://github.com/ApeWorX/ape-frame.git
+        cd ape-frame
+        python3 setup.py install
+        ```
+        
+        ## Quick Usage
+        
+        TODO: Describe library overview in code
+        
+        ## Development
+        
+        This project is in development and should be considered a beta.
+        Things might not be in their final state and breaking changes may occur.
+        Comments, questions, criticisms and pull requests are welcomed.
+        
 Keywords: ethereum
-Classifier: Development Status :: 4 - Beta
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
-License-File: LICENSE
-
-# Quick Start
-
-TODO: Description
-
-## Dependencies
-
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
-
-## Installation
-
-### via `pip`
-
-You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-
-```bash
-pip install ape-frame
-```
-
-### via `setuptools`
-
-You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-
-```bash
-git clone https://github.com/ApeWorX/ape-frame.git
-cd ape-frame
-python3 setup.py install
-```
-
-## Quick Usage
-
-TODO: Describe library overview in code
-
-## Development
-
-This project is in development and should be considered a beta.
-Things might not be in their final state and breaking changes may occur.
-Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-frame-0.6.0/ape_frame.egg-info/SOURCES.txt` & `ape-frame-0.6.0a0/ape_frame.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,27 +7,25 @@
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
 .github/ISSUE_TEMPLATE/work-item.md
-.github/workflows/codeql.yaml
 .github/workflows/commitlint.yaml
 .github/workflows/draft.yaml
-.github/workflows/prtitle.yaml
 .github/workflows/publish.yaml
 .github/workflows/test.yaml
+.github/workflows/title.yaml
 ape_frame/__init__.py
 ape_frame/accounts.py
 ape_frame/exceptions.py
 ape_frame/providers.py
 ape_frame/py.typed
 ape_frame/version.py
 ape_frame.egg-info/PKG-INFO
 ape_frame.egg-info/SOURCES.txt
 ape_frame.egg-info/dependency_links.txt
 ape_frame.egg-info/not-zip-safe
 ape_frame.egg-info/requires.txt
 ape_frame.egg-info/top_level.txt
-tests/__init__.py
-tests/test_accounts.py
+tests/__init__.py
```

### Comparing `ape-frame-0.6.0/pyproject.toml` & `ape-frame-0.6.0a0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
+target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
+    -n auto
     -p no:ape_test
     --cov-branch
     --cov-report term
     --cov-report html
     --cov-report xml
     --cov=ape_frame
 """
@@ -32,10 +33,7 @@
 
 [tool.isort]
 line_length = 100
 force_grid_wrap = 0
 include_trailing_comma = true
 multi_line_output = 3
 use_parentheses = true
-
-[tool.mdformat]
-number = true
```

### Comparing `ape-frame-0.6.0/setup.py` & `ape-frame-0.6.0a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
-        "pytest-xdist",  # Multi-process runner
+        "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=24.4.2,<25",  # Auto-formatter and linter
-        "mypy>=1.10.0,<2",  # Static type analyzer
-        "types-requests",  # Needed due to mypy typeshed
-        "types-setuptools",  # Needed due to mypy typeshed
-        "types-PyYAML",  # Needed due to mypy typeshed
-        "flake8>=7.0.0,<8",  # Style linter
-        "isort>=5.13.2,<6",  # Import sorting linter
-        "mdformat>=0.7.17",  # Auto-formatter for markdown
-        "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
-        "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
-        "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
+        "black>=22.10.0",  # auto-formatter and linter
+        "mypy>=0.982",  # Static type analyzer
+        "types-setuptools",  # Needed for mypy type shed
+        "flake8>=5.0.4",  # Style linter
+        "isort>=5.10.1",  # Import sorting linter
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
         "wheel",  # Packaging tool
         "twine",  # Package upload tool
     ],
     "dev": [
@@ -56,32 +50,30 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-frame",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.10,<0.8",
+        "eth-ape>=0.6.0,<0.7.0",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_frame"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_frame": ["py.typed"]},
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
     ],
 )
```

