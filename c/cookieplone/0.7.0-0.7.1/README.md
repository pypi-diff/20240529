# Comparing `tmp/cookieplone-0.7.0.tar.gz` & `tmp/cookieplone-0.7.1.tar.gz`

## Comparing `cookieplone-0.7.0.tar` & `cookieplone-0.7.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 cookieplone-0.7.0/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.7.0/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.7.0/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.7.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/__main__.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/generator.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/logger.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/repository.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/templates/__init__.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/templates/fixtures.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/templates/types.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/files.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/formatters.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/git.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/internal.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/plone.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.7.0/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/test_cli.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/test_filters.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/plone/dependencies.zcml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/plone/metadata.xml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/templates/project/cookiecutter.json
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/templates/project/{{ cookiecutter.__folder_name }}/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/templates/sub/bar/cookiecutter.json
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/templates/sub/bar/{{ cookiecutter.__folder_name }}/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/templates/conftest.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/templates/test_fixtures.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_git.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_internal.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_plone.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.7.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.7.0/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.7.0/README.md
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 cookieplone-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 cookieplone-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 cookieplone-0.7.1/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.7.1/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.7.1/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.7.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/__main__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/generator.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/logger.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/repository.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/templates/__init__.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/templates/fixtures.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/templates/types.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/files.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/formatters.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/plone.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.7.1/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.7.1/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/test_filters.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/_resources/plone/dependencies.zcml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/_resources/plone/metadata.xml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/_resources/templates/project/cookiecutter.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/_resources/templates/project/{{ cookiecutter.__folder_name }}/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/_resources/templates/sub/bar/cookiecutter.json
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/_resources/templates/sub/bar/{{ cookiecutter.__folder_name }}/README.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/templates/conftest.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/templates/test_fixtures.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_internal.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_plone.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.7.1/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.7.1/README.md
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 cookieplone-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 cookieplone-0.7.1/PKG-INFO
```

### Comparing `cookieplone-0.7.0/.pre-commit-config.yaml` & `cookieplone-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/CHANGES.md` & `cookieplone-0.7.1/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.7.1 (2024-05-29)
+
+
+### Bug fixes:
+
+- Fix issue with Welcome Screen display [@ericof] 
+
 ## 0.7.0 (2024-05-27)
 
 
 ### New features:
 
 - Add --info option to display current settings [@ericof] [#27](https://github.com/plone/cookieplone/issues/27)
 - Add pytest fixtures to be used in template development [@ericof] [#29](https://github.com/plone/cookieplone/issues/29)
```

### Comparing `cookieplone-0.7.0/Makefile` & `cookieplone-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/.github/workflows/changelog.yml` & `cookieplone-0.7.1/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/.github/workflows/main.yml` & `cookieplone-0.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/cli.py` & `cookieplone-0.7.1/cookieplone/cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/data.py` & `cookieplone-0.7.1/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/exceptions.py` & `cookieplone-0.7.1/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/generator.py` & `cookieplone-0.7.1/cookieplone/generator.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/logger.py` & `cookieplone-0.7.1/cookieplone/logger.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/repository.py` & `cookieplone-0.7.1/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/settings.py` & `cookieplone-0.7.1/cookieplone/settings.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/filters/__init__.py` & `cookieplone-0.7.1/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/templates/fixtures.py` & `cookieplone-0.7.1/cookieplone/templates/fixtures.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/console.py` & `cookieplone-0.7.1/cookieplone/utils/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,17 @@
 
 
 def welcome_screen(templates: list[list[str]] | None = None):
     items = [
         Align.center(f"[bold blue]{BANNER}[/bold blue]"),
     ]
     if templates:
-        items.append(Panel(table_available_templates(templates, title="Templates")))
+        items.append(
+            Panel(table_available_templates(title="Templates", rows=templates))
+        )
     panel = Panel(
         Group(*items),
         title="cookieplone",
     )
     base_print(panel)
```

### Comparing `cookieplone-0.7.0/cookieplone/utils/files.py` & `cookieplone-0.7.1/cookieplone/utils/files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/formatters.py` & `cookieplone-0.7.1/cookieplone/utils/formatters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/git.py` & `cookieplone-0.7.1/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/internal.py` & `cookieplone-0.7.1/cookieplone/utils/internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/plone.py` & `cookieplone-0.7.1/cookieplone/utils/plone.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/sanity.py` & `cookieplone-0.7.1/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/validators.py` & `cookieplone-0.7.1/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/versions.py` & `cookieplone-0.7.1/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/cookieplone/utils/commands/__init__.py` & `cookieplone-0.7.1/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/conftest.py` & `cookieplone-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/test_cli.py` & `cookieplone-0.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/test_filters.py` & `cookieplone-0.7.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/_resources/templates/project/cookiecutter.json` & `cookieplone-0.7.1/tests/_resources/templates/project/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/_resources/templates/sub/bar/cookiecutter.json` & `cookieplone-0.7.1/tests/_resources/templates/sub/bar/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/templates/conftest.py` & `cookieplone-0.7.1/tests/templates/conftest.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/templates/test_fixtures.py` & `cookieplone-0.7.1/tests/templates/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_commands.py` & `cookieplone-0.7.1/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_console.py` & `cookieplone-0.7.1/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_files.py` & `cookieplone-0.7.1/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_git.py` & `cookieplone-0.7.1/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_internal.py` & `cookieplone-0.7.1/tests/utils/test_internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_plone.py` & `cookieplone-0.7.1/tests/utils/test_plone.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_sanity.py` & `cookieplone-0.7.1/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_validators.py` & `cookieplone-0.7.1/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/tests/utils/test_versions.py` & `cookieplone-0.7.1/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/.gitignore` & `cookieplone-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/LICENSE` & `cookieplone-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/README.md` & `cookieplone-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/pyproject.toml` & `cookieplone-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.7.0/PKG-INFO` & `cookieplone-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.7.0
+Version: 0.7.1
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
```

