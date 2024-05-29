# Comparing `tmp/pyproject_creator-0.1.2.tar.gz` & `tmp/pyproject_creator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_creator-0.1.2.tar", max compression
+gzip compressed data, was "pyproject_creator-0.2.0.tar", max compression
```

## Comparing `pyproject_creator-0.1.2.tar` & `pyproject_creator-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1065 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/LICENSE
--rw-r--r--   0        0        0     2275 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/README.md
--rw-r--r--   0        0        0     2238 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/__init__.py
--rw-r--r--   0        0        0     5591 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/cli.py
--rw-r--r--   0        0        0     8420 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/template/.cz.toml
--rw-r--r--   0        0        0     3077 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/template/.gitignore
--rw-r--r--   0        0        0     2181 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/template/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1127 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/template/github_action/workflows/test.yml
--rw-r--r--   0        0        0        0 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/template/logs/__init__.py
--rw-r--r--   0        0        0     3252 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/template/logs/_default.py
--rw-r--r--   0        0        0     2345 2024-05-28 07:03:30.374385 pyproject_creator-0.1.2/pyproject_creator/template/pyproject.template
--rw-r--r--   0        0        0        0 2024-05-28 07:03:30.378385 pyproject_creator-0.1.2/pyproject_creator/template/scripts/__init__.py
--rw-r--r--   0        0        0      303 2024-05-28 07:03:30.378385 pyproject_creator-0.1.2/pyproject_creator/template/scripts/commit_with_pre_commit.py
--rw-r--r--   0        0        0        0 2024-05-28 07:03:30.378385 pyproject_creator-0.1.2/pyproject_creator/template/tests/__init__.py
--rw-r--r--   0        0        0       43 2024-05-28 07:03:30.378385 pyproject_creator-0.1.2/pyproject_creator/template/tests/test_sample.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 pyproject_creator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-29 08:29:46.570895 pyproject_creator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2365 2024-05-29 08:29:46.570895 pyproject_creator-0.2.0/README.md
+-rw-r--r--   0        0        0     2691 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/__init__.py
+-rw-r--r--   0        0        0     5628 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/cli.py
+-rw-r--r--   0        0        0     8420 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/.cz.toml
+-rw-r--r--   0        0        0     3077 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/.gitignore
+-rw-r--r--   0        0        0     2181 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1127 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/github_action/workflows/test.yml
+-rw-r--r--   0        0        0        0 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/logs/__init__.py
+-rw-r--r--   0        0        0     3289 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/logs/_default.py
+-rw-r--r--   0        0        0     2345 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/pyproject.template
+-rw-r--r--   0        0        0        0 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/scripts/__init__.py
+-rw-r--r--   0        0        0      339 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/scripts/commit_with_pre_commit.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/tests/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/tests/test_sample.py
+-rw-r--r--   0        0        0     2890 1970-01-01 00:00:00.000000 pyproject_creator-0.2.0/PKG-INFO
```

### Comparing `pyproject_creator-0.1.2/LICENSE` & `pyproject_creator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.1.2/README.md` & `pyproject_creator-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Pyproject Creator
-
+![test](https://github.com/atiasn/docs/actions/workflows/test.yml/badge.svg?branch=master)
 Pyproject Creator 是一个旨在简化创建 Python 项目过程的工具。它可以生成一些基础项目结构组件。
 
 基础组件：
 - Poetry 用于包管理
 - pre-commit 用于代码格式化和 linting
 - Commitizen 用于规范 git commit
```

### Comparing `pyproject_creator-0.1.2/pyproject.toml` & `pyproject_creator-0.2.0/pyproject_creator/template/pyproject.template`

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,95 @@
 [tool.poetry]
-name = "pyproject-creator"
-version = "0.1.2"
-description = "A tool to create Python project templates"
-authors = ["NextKele <ritboylei@gmail.com>"]
-license = "MIT"
+name = "{{ project_name }}"
+version = "0.1.0"
+description = "{{ project_description }}"
+authors = ["{{ author }}"]
+{% if project_license %}license = "{{ project_license }}"
+{% endif -%}
 readme = "README.md"
 
-[tool.poetry.dependencies]
-python = "^3.11"
-jinja2 = "^3.1.4"
-click = "^8.1.7"
-
 [[tool.poetry.source]]
 name = "tuna"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple"
 priority = "primary"
 
+[tool.poetry.dependencies]
+{% if need_logs == "y" %}loguru = "^0.7.2"
+{% endif -%}
+python = "^{{ python_version }}"
+
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.2.1"
-mypy = "^1.10.0"
+{% if need_tests == "y" %}pytest = "^8.2.1"
+{% endif -%}
 isort = "^5.13.2"
 black = "^24.4.2"
 pre-commit-hooks = "^4.6.0"
 pre-commit = "^3.7.1"
 commitizen = "^3.27.0"
-pytest-mock = "^3.14.0"
-loguru = "^0.7.2"
-
-[tool.poetry.scripts]
-pypct = "pyproject_creator.cli:create_project"
 
 [tool.black]
 line-length = 99
 target-version = ["py311", "py312"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
 
 [tool.mypy]
 strict = true
-files = ["pyproject_creator", "scripts", "tests"]
+files = ["pyproject_creator"{% if need_tests == "y" %}, "tests"{% endif -%}]
 pretty = true
 
 [tool.isort]
 profile = "black"
 line_length = 99
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
-src_paths = ["pyproject_creator", "scripts", "tests"]
+src_paths = ["{{ project_src_name }}"{% if need_tests == "y" %}, "tests"{% endif -%}]
 extra_standard_library = ["typing_extensions"]
 
 [tool.ruff]
 line-length = 99
 target-version = "py311"
-src = ["pyproject_creator", "scripts", "tests"]
+src = ["{{ project_src_name }}"{% if need_tests == "y" %}, "tests"{% endif -%}]
 
 [tool.ruff.lint]
 select = [
     "F",  # Pyflakes
     "W",  # pycodestyle warnings
     "E",  # pycodestyle errors
     "UP",  # pyupgrade
     "ASYNC",  # flake8-async
     "C4",  # flake8-comprehensions
     "T10",  # flake8-debugger
     "T20",  # flake8-print
     "PYI",  # flake8-pyi
-    "PT",  # flake8-pytest-style
+    {% if need_tests == "y" %}"PT",  # flake8-pytest-style
+    {% endif -%}
     "Q",  # flake8-quotes
     "RUF"  # Ruff-specific rules
 ]
 ignore = [
     "E402",  # module-import-not-at-top-of-file
     "UP037",  # quoted-annotation
     "RUF001",  # ambiguous-unicode-character-string
     "RUF002",  # ambiguous-unicode-character-docstring
     "RUF003",  # ambiguous-unicode-character-comment
     "T201",  # print found
-    "PT004"  # not return anything
 ]
 
 [tool.ruff.lint.flake8-quotes]
 inline-quotes = "double"
 multiline-quotes = "double"
 docstring-quotes = "double"
 
-[tool.ruff.lint.flake8-pytest-style]
+{% if need_tests == "y" %}[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
+{% endif -%}
 [tool.ruff.format]
 quote-style = "double"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyproject_creator-0.1.2/pyproject_creator/cli.py` & `pyproject_creator-0.2.0/pyproject_creator/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import os
 import re
 import shutil
 import subprocess
 from pathlib import Path
 
 import click
 import jinja2
 
+
 BASE_PATH: Path = Path(__file__).parent.resolve()
 
 
 def validate_project_name(value: str) -> str:
     """Validate the project name to ensure it meets the required criteria."""
     if not re.match(r"^[a-zA-Z0-9][a-zA-Z0-9_-]*$", value):
         raise click.BadParameter(
```

### Comparing `pyproject_creator-0.1.2/pyproject_creator/template/.cz.toml` & `pyproject_creator-0.2.0/pyproject_creator/template/.cz.toml`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.commitizen]
+bump_message = "🔖 release: $current_version → $new_version"
+major_version_zero = true
 name = "cz_customize"
 tag_format = "$version"
-version_scheme = "pep440"
-version_provider = "poetry"
 update_changelog_on_bump = true
-major_version_zero = true
 version_files = ["pyproject.toml:^version"]
-bump_message = "🔖 release: $current_version → $new_version"
+version_provider = "poetry"
+version_scheme = "pep440"
 
 [tool.commitizen.customize]
-message_template = "{{change_type}}: {{message}}"
-example = "✨ feat: this feature enables customization through config file"
-schema = "<change_type>: <message>"
-schema_pattern = "^(?P<emoji>[^\\s]+)\\s(?P<change_type>feat|fix|docs|style|refactor|test|deploy|ui|release|types|lint|add_dep|rm_dep|downgrade|upgrade|pin|ci_fix|ci_update|analytics|config|scripts|i18n|typos|init|wip|revert|merge|compiled|api|move|breaking|accessibility|comments|drunk|logs|rm_logs|ux|architecture|gitignore|flags|catch_errors|deprecate|rm_dead_code|dev_exp|performance|rm_code|assets):\\s(?P<message>.+)"
-bump_pattern = "^(breaking|feat|fix|hotfix)"
 bump_map = {"breaking" = "MAJOR", "feat" = "MINOR", "fix" = "PATCH", "hotfix" = "PATCH"}
+bump_pattern = "^(breaking|feat|fix|hotfix)"
+change_type_map = {"feat" = "Feat", "fix" = "Fix"}
 change_type_order = ["BREAKING CHANGE", "feat", "fix", "perf", "refactor", "docs", "style", "test", "build", "ci", "chore", "revert", "release", "wip"]
+changelog_pattern = "^(feat|fix|docs|style|refactor|test|deploy|ui|release|types|lint|add_dep|rm_dep|downgrade|upgrade|pin|ci_fix|ci_update|analytics|config|scripts|i18n|typos|init|wip|revert|merge|compiled|api|move|breaking|accessibility|comments|drunk|logs|rm_logs|ux|architecture|gitignore|flags|catch_errors|deprecate|rm_dead_code|dev_exp|performance|rm_code|assets)?(!)?"
+commit_parser = "^(?P<emoji>[^\\s]+)\\s(?P<change_type>feat|fix|docs|style|refactor|test|deploy|ui|release|types|lint|add_dep|rm_dep|downgrade|upgrade|pin|ci_fix|ci_update|analytics|config|scripts|i18n|typos|init|wip|revert|merge|compiled|api|move|breaking|accessibility|comments|drunk|logs|rm_logs|ux|architecture|gitignore|flags|catch_errors|deprecate|rm_dead_code|dev_exp|performance|rm_code|assets):\\s(?P<message>.+)$"
+example = "✨ feat: this feature enables customization through config file"
 info = """
 This is a customized Commitizen configuration for our project.
 
 Commit Types:
 - ✨ feat: Introduce new features.
 - 🐛 fix: Fix a bug.
 - 📝 docs: Add or update documentation.
@@ -70,21 +70,19 @@
 
 Each commit message should follow this format:
 <change_type>: <message>
 
 Example:
 ✨ feat: Add new authentication module
 """
-commit_parser = "^(?P<emoji>[^\\s]+)\\s(?P<change_type>feat|fix|docs|style|refactor|test|deploy|ui|release|types|lint|add_dep|rm_dep|downgrade|upgrade|pin|ci_fix|ci_update|analytics|config|scripts|i18n|typos|init|wip|revert|merge|compiled|api|move|breaking|accessibility|comments|drunk|logs|rm_logs|ux|architecture|gitignore|flags|catch_errors|deprecate|rm_dead_code|dev_exp|performance|rm_code|assets):\\s(?P<message>.+)$"
-changelog_pattern = "^(feat|fix|docs|style|refactor|test|deploy|ui|release|types|lint|add_dep|rm_dep|downgrade|upgrade|pin|ci_fix|ci_update|analytics|config|scripts|i18n|typos|init|wip|revert|merge|compiled|api|move|breaking|accessibility|comments|drunk|logs|rm_logs|ux|architecture|gitignore|flags|catch_errors|deprecate|rm_dead_code|dev_exp|performance|rm_code|assets)?(!)?"
-change_type_map = {"feat" = "Feat", "fix" = "Fix"}
+message_template = "{{change_type}}: {{message}}"
+schema = "<change_type>: <message>"
+schema_pattern = "^(?P<emoji>[^\\s]+)\\s(?P<change_type>feat|fix|docs|style|refactor|test|deploy|ui|release|types|lint|add_dep|rm_dep|downgrade|upgrade|pin|ci_fix|ci_update|analytics|config|scripts|i18n|typos|init|wip|revert|merge|compiled|api|move|breaking|accessibility|comments|drunk|logs|rm_logs|ux|architecture|gitignore|flags|catch_errors|deprecate|rm_dead_code|dev_exp|performance|rm_code|assets):\\s(?P<message>.+)"
 
 [[tool.commitizen.customize.questions]]
-type = "list"
-name = "change_type"
 choices = [
     {value = "✨ feat", name = "✨ feat: Introduce new features."},
     {value = "🐛 fix", name = "🐛 fix: Fix a bug."},
     {value = "📝 docs", name = "📝 docs: Add or update documentation."},
     {value = "📄 license", name = "📄 license: Add or update license."},
     {value = "🎨 style", name = "🎨 style: Improve structure / format of the code."},
     {value = "♻️ refactor", name = "♻️ refactor: Refactor code."},
@@ -128,12 +126,14 @@
     {value = "⚰️ rm_dead_code", name = "⚰️ rm_dead_code: Remove dead code."},
     {value = "🧑‍💻 dev_exp", name = "🧑‍💻 dev_exp: Improve developer experience."},
     {value = "⚡️ performance", name = "⚡️ performance: Improve performance."},
     {value = "🔥 rm_code", name = "🔥 rm_code: Remove code or files."},
     {value = "🍱 assets", name = "🍱 assets: Add or update assets."}
 ]
 message = "Select the type of change you are committing"
+name = "change_type"
+type = "list"
 
 [[tool.commitizen.customize.questions]]
-type = "input"
-name = "message"
 message = "Please input commit message body:\n"
+name = "message"
+type = "input"
```

### Comparing `pyproject_creator-0.1.2/pyproject_creator/template/.gitignore` & `pyproject_creator-0.2.0/pyproject_creator/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.1.2/pyproject_creator/template/.pre-commit-config.yaml` & `pyproject_creator-0.2.0/pyproject_creator/template/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.1.2/pyproject_creator/template/github_action/workflows/test.yml` & `pyproject_creator-0.2.0/pyproject_creator/template/github_action/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.1.2/pyproject_creator/template/logs/_default.py` & `pyproject_creator-0.2.0/pyproject_creator/template/logs/_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 默认信息:
 
 - 格式: `[%(asctime)s %(name)s] %(levelname)s: %(message)s`
 - 等级: `INFO` ，根据 `settings.log_level` 配置改变
 - 输出: 输出至 stdout
 """
 
+from __future__ import annotations
+
 import re
 import sys
 import inspect
 import logging
 from re import Match
 from typing import TYPE_CHECKING
 
 import loguru
 
+
 if TYPE_CHECKING:
     from loguru import Logger, Record
 
 logger: "Logger" = loguru.logger
 
 
 # default_handler = logging.StreamHandler(sys.stdout)
```

### Comparing `pyproject_creator-0.1.2/PKG-INFO` & `pyproject_creator-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyproject-creator
-Version: 0.1.2
+Version: 0.2.0
 Summary: A tool to create Python project templates
 License: MIT
 Author: NextKele
 Author-email: ritboylei@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Pyproject Creator
-
+![test](https://github.com/atiasn/docs/actions/workflows/test.yml/badge.svg?branch=master)
 Pyproject Creator 是一个旨在简化创建 Python 项目过程的工具。它可以生成一些基础项目结构组件。
 
 基础组件：
 - Poetry 用于包管理
 - pre-commit 用于代码格式化和 linting
 - Commitizen 用于规范 git commit
```

