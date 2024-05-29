# Comparing `tmp/edge_containers_cli-3.5.2.tar.gz` & `tmp/edge_containers_cli-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_containers_cli-3.5.2.tar", last modified: Thu May 23 07:27:41 2024, max compression
+gzip compressed data, was "edge_containers_cli-3.5.3.tar", last modified: Wed May 29 07:56:02 2024, max compression
```

## Comparing `edge_containers_cli-3.5.2.tar` & `edge_containers_cli-3.5.3.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.013455 edge_containers_cli-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.993455 edge_containers_cli-3.5.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.993455 edge_containers_cli-3.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.989455 edge_containers_cli-3.5.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.993455 edge_containers_cli-3.5.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.997455 edge_containers_cli-3.5.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2753 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.997455 edge_containers_cli-3.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/workflows/_sys_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.997455 edge_containers_cli-3.5.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-23 07:27:41.013455 edge_containers_cli-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.997455 edge_containers_cli-3.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.997455 edge_containers_cli-3.5.2/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.997455 edge_containers_cli-3.5.2/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.997455 edge_containers_cli-3.5.2/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    99678 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.001455 edge_containers_cli-3.5.2/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:27:41.013455 edge_containers_cli-3.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.993455 edge_containers_cli-3.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.005455 edge_containers_cli-3.5.2/src/edge_containers_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 07:27:40.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.005455 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/k8s_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/local_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15426 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/monitor.tcss
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/src/edge_containers_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.013455 edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-23 07:27:40.000000 edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-23 07:27:40.000000 edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:27:40.000000 edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 07:27:40.000000 edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 07:27:40.000000 edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 07:27:40.000000 edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/autocomplete.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/bl01t/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/bl01t/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/bl01t/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1253 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/.github/workflows/ci_verify.sh
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/.github/workflows/verify.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1874 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/environment.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.993455 edge_containers_cli-3.5.2/tests/data/bl01t/helm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/bl01t/helm/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/helm/shared/Chart.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/helm/shared/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/helm/shared/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.993455 edge_containers_cli-3.5.2/tests/data/bl01t/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/bl01t/include/iocs/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/include/iocs/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/bl01t/include/iocs/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/include/iocs/templates/configmap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:40.993455 edge_containers_cli-3.5.2/tests/data/bl01t/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:41.009455 edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/config/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/pretend_helm.tgz
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/values.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/bl01t/update-helm
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/data/local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/test_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-23 07:27:35.000000 edge_containers_cli-3.5.2/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.305050 edge_containers_cli-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.285050 edge_containers_cli-3.5.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.289050 edge_containers_cli-3.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.281051 edge_containers_cli-3.5.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.289050 edge_containers_cli-3.5.3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.289050 edge_containers_cli-3.5.3/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2753 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.289050 edge_containers_cli-3.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/workflows/_sys_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.289050 edge_containers_cli-3.5.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15398 2024-05-29 07:56:02.305050 edge_containers_cli-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.289050 edge_containers_cli-3.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.289050 edge_containers_cli-3.5.3/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.289050 edge_containers_cli-3.5.3/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    99678 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.293051 edge_containers_cli-3.5.3/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:56:02.305050 edge_containers_cli-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.285050 edge_containers_cli-3.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.297051 edge_containers_cli-3.5.3/src/edge_containers_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 07:56:02.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.297051 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/k8s_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/local_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16118 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/monitor.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/src/edge_containers_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.305050 edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15398 2024-05-29 07:56:02.000000 edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-29 07:56:02.000000 edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:56:02.000000 edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 07:56:02.000000 edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 07:56:02.000000 edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 07:56:02.000000 edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/autocomplete.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/data/bl01t/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/data/bl01t/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/data/bl01t/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1253 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/.github/workflows/ci_verify.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/.github/workflows/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1874 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/environment.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.285050 edge_containers_cli-3.5.3/tests/data/bl01t/helm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/data/bl01t/helm/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/helm/shared/Chart.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/helm/shared/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/helm/shared/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.285050 edge_containers_cli-3.5.3/tests/data/bl01t/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/data/bl01t/include/iocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/include/iocs/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/data/bl01t/include/iocs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/include/iocs/templates/configmap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.285050 edge_containers_cli-3.5.3/tests/data/bl01t/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.301051 edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:02.305050 edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/pretend_helm.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/values.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/bl01t/update-helm
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/data/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/test_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-29 07:55:58.000000 edge_containers_cli-3.5.3/tests/test_system.py
```

### Comparing `edge_containers_cli-3.5.2/.devcontainer/devcontainer.json` & `edge_containers_cli-3.5.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/CONTRIBUTING.md` & `edge_containers_cli-3.5.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/actions/install_requirements/action.yml` & `edge_containers_cli-3.5.3/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/dependabot.yml` & `edge_containers_cli-3.5.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/pages/make_switcher.py` & `edge_containers_cli-3.5.3/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/workflows/_check.yml` & `edge_containers_cli-3.5.3/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/workflows/_dist.yml` & `edge_containers_cli-3.5.3/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/workflows/_release.yml` & `edge_containers_cli-3.5.3/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/workflows/_sys_test.yml` & `edge_containers_cli-3.5.3/.github/workflows/_sys_test.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/workflows/_test.yml` & `edge_containers_cli-3.5.3/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.github/workflows/ci.yml` & `edge_containers_cli-3.5.3/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
   test:
     needs: check
     if: needs.check.outputs.branch-pr == ''
     strategy:
       matrix:
         runs-on: ["ubuntu-latest"] # can add windows-latest, macos-latest
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.10", "3.11", "3.12"]
         include:
           # Include one that runs in the dev environment
           - runs-on: "ubuntu-latest"
             python-version: "dev"
       fail-fast: false
     uses: ./.github/workflows/_test.yml
     with:
@@ -36,15 +36,15 @@
 
   system:
     needs: check
     if: needs.check.outputs.branch-pr == ''
     strategy:
       matrix:
         runs-on: ["ubuntu-latest"]
-        python-version: ["3.11"]
+        python-version: ["3.12"]
       fail-fast: false
     uses: ./.github/workflows/_sys_test.yml
     with:
       runs-on: ${{ matrix.runs-on }}
       python-version: ${{ matrix.python-version }}
 
   dist:
```

### Comparing `edge_containers_cli-3.5.2/.gitignore` & `edge_containers_cli-3.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.pre-commit-config.yaml` & `edge_containers_cli-3.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/.vscode/launch.json` & `edge_containers_cli-3.5.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/LICENSE` & `edge_containers_cli-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/PKG-INFO` & `edge_containers_cli-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-containers-cli
-Version: 3.5.2
+Version: 3.5.3
 Summary: CLI for deploying and managing epics containers IOCs and services
 Author-email: Giles Knap <giles.knap@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,18 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/epics-containers/edge-containers-cli
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: natsort
 Requires-Dist: typer[all]
 Requires-Dist: requests
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
```

### Comparing `edge_containers_cli-3.5.2/README.md` & `edge_containers_cli-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/conf.py` & `edge_containers_cli-3.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `edge_containers_cli-3.5.3/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/explanations/decisions.rst` & `edge_containers_cli-3.5.3/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/how-to/build-docs.rst` & `edge_containers_cli-3.5.3/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/how-to/lint.rst` & `edge_containers_cli-3.5.3/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/how-to/make-release.rst` & `edge_containers_cli-3.5.3/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/how-to/pin-requirements.rst` & `edge_containers_cli-3.5.3/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/how-to/test-container.rst` & `edge_containers_cli-3.5.3/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/how-to/update-tools.rst` & `edge_containers_cli-3.5.3/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/index.rst` & `edge_containers_cli-3.5.3/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/reference/standards.rst` & `edge_containers_cli-3.5.3/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/developer/tutorials/dev-install.rst` & `edge_containers_cli-3.5.3/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/images/dls-favicon.ico` & `edge_containers_cli-3.5.3/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/images/dls-logo.svg` & `edge_containers_cli-3.5.3/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/index.rst` & `edge_containers_cli-3.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/user/explanations/docs-structure.rst` & `edge_containers_cli-3.5.3/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/user/index.rst` & `edge_containers_cli-3.5.3/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/docs/user/tutorials/installation.rst` & `edge_containers_cli-3.5.3/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/pyproject.toml` & `edge_containers_cli-3.5.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edge-containers-cli"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 description = "CLI for deploying and managing epics containers IOCs and services"
 
 dependencies = [
     "natsort",
     "typer[all]",
     "requests",
@@ -22,15 +22,15 @@
     "polars",
     "textual",
 ]
 
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
     "copier",
     "pipdeptree",
     "pre-commit",
     "pyright",
@@ -105,17 +105,18 @@
     tests: pytest --cov=edge_containers_cli --cov-report term --cov-report xml:cov.xml {posargs}
 """
 
 [tool.ruff]
 src = ["src", "tests"]
 line-length = 88
 lint.ignore = [
-    "C408", # Unnecessary collection call - e.g. list(...) instead of [...]
-    "E501", # Line too long, should be fixed by black.
-    "B008", # Do not perform function calls in argument defaults.
+    "C408",  # Unnecessary collection call - e.g. list(...) instead of [...]
+    "E501",  # Line too long, should be fixed by black.
+    "B008",  # Do not perform function calls in argument defaults.
+    "UP007", # Do not complain about Optional[] (TODO: remove once typer is patched)
 ]
 lint.select = [
     "B",  # flake8-bugbear - https://docs.astral.sh/ruff/rules/#flake8-bugbear-b
     "C4", # flake8-comprehensions - https://docs.astral.sh/ruff/rules/#flake8-comprehensions-c4
     "E",  # pycodestyle errors - https://docs.astral.sh/ruff/rules/#error-e
     "F",  # pyflakes rules - https://docs.astral.sh/ruff/rules/#pyflakes-f
     "W",  # pycodestyle warnings - https://docs.astral.sh/ruff/rules/#warning-w
```

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/__main__.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/autocomplete.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/cli.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/cli.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/commands.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/commands.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/helm.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/helm.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/k8s_commands.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/k8s_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Relies on the Helm class for deployment aspects.
 """
 
 from datetime import datetime
 from io import StringIO
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional
 
 import polars
 import typer
 
 import edge_containers_cli.globals as globals
 import edge_containers_cli.shell as shell
 from edge_containers_cli.cmds.commands import Commands
@@ -35,15 +35,15 @@
         raise typer.Exit(1)
 
     # return statefulset/name or deployment/name
     log.debug(f"fullname = {result}")
     return str(result).strip()
 
 
-def check_namespace(namespace: Optional[str]):
+def check_namespace(namespace: str | None):
     """
     Verify we have a good namespace that exists in the cluster
     """
     if not namespace:
         log.error("Please set EC_K8S_NAMESPACE or pass --namespace")
         raise typer.Exit(1)
 
@@ -121,15 +121,15 @@
 
     def exec(self, service_name):
         fullname = check_service(service_name, self.namespace)
         shell.run_command(f"kubectl -it -n {self.namespace} exec {fullname} -- bash")
 
     def logs(
         self, service_name: str, prev: bool, follow: bool, stdout: bool = False
-    ) -> Optional[Union[str, bool]]:
+    ) -> Optional[str | bool]:
         fullname = check_service(service_name, self.namespace)
         previous = "-p" if prev else ""
         fol = "-f" if follow else ""
 
         if stdout:
             a = shell.run_command(
                 f"kubectl -n {self.namespace} logs {fullname} {previous} {fol}",
```

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/local_commands.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/local_commands.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/monitor.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """TUI monitor for containerised IOCs."""
 
+from collections.abc import Callable
 from functools import total_ordering
 from threading import Thread
 from time import sleep
-from typing import Any, Callable, Union, cast
+from typing import Any, cast
 
 import polars
 from rich.style import Style
 from rich.syntax import Syntax
 from rich.text import Text
 
 # from textual import on
@@ -181,25 +182,49 @@
             Style(color=color.rich_color),
             justify=justify,
         )
 
     def __lt__(self, other: Any) -> bool:
         if type(other) != SortableText:
             return NotImplemented
-        return cast(bool, self.value < other.value)
+
+        # Handle None as values
+        match self.value, other.value:
+            case (None, None) | (None, _):
+                return False
+            case (_, None):
+                return True
+            case _:
+                return cast(bool, self.value < other.value)
 
     def __gt__(self, other: Any) -> bool:
         if type(other) != SortableText:
             return NotImplemented
-        return cast(bool, self.value > other.value)
+
+        # Handle None as values
+        match self.value, other.value:
+            case (None, None) | (_, None):
+                return False
+            case (None, _):
+                return True
+            case _:
+                return cast(bool, self.value > other.value)
 
     def __eq__(self, other: Any) -> bool:
         if type(other) != SortableText:
             return NotImplemented
-        return cast(bool, self.value == other.value)
+
+        # Handle None as values
+        match self.value, other.value:
+            case (None, _) | (_, None):
+                return False
+            case (None, None):
+                return True
+            case _:
+                return cast(bool, self.value == other.value)
 
 
 class IocTable(Widget):
     """Widget to display the IOC table."""
 
     default_sort_column_id = "name"
     # init=False otherwise triggers table query before yielded in compose
@@ -236,15 +261,15 @@
         exclude = ["deployed", "image"]
 
         for i, ioc in enumerate(self.iocs):
             ioc = {key: value for key, value in ioc.items() if key not in exclude}
             self.iocs[i] = ioc
         self.columns = [key for key in self.iocs[0].keys() if key not in exclude]
 
-    def _convert_df_to_list(self, iocs_df: Union[polars.DataFrame, list]) -> list[dict]:
+    def _convert_df_to_list(self, iocs_df: polars.DataFrame | list) -> list[dict]:
         if isinstance(iocs_df, polars.DataFrame):
             iocs = iocs_df.to_dicts()
         else:
             iocs = iocs_df
 
         return iocs
 
@@ -349,38 +374,38 @@
             table.remove_row(old_row_key)
 
         # Sort by column
         table.sort(self.sort_column_id, reverse=False)
 
 
 class MonitorApp(App):
-    def __init__(
-        self,
-        beamline: str,
-        commands: Commands,
-        running_only: bool,
-    ) -> None:
-        super().__init__()
-
-        self.commands = commands
-        self.running_only = running_only
-        self.beamline = beamline
-
     CSS_PATH = "monitor.tcss"
 
     BINDINGS = [
         Binding("escape", "close_application", "Exit"),
         Binding("s", "start_ioc", "Start IOC"),
         Binding("t", "stop_ioc", "Stop IOC"),
         Binding("r", "restart_ioc", "Restart IOC"),
         Binding("l", "ioc_logs", "IOC Logs"),
         Binding("o", "sort", "Sort"),
         # Binding("d", "toggle_dark", "Toggle dark mode"),
     ]
 
+    def __init__(
+        self,
+        beamline: str,
+        commands: Commands,
+        running_only: bool,
+    ) -> None:
+        super().__init__()
+
+        self.commands = commands
+        self.running_only = running_only
+        self.beamline = beamline
+
     def compose(self) -> ComposeResult:
         """Create child widgets for the app."""
         yield Header(show_clock=True)
         self.table = IocTable(self.commands, self.running_only)
         yield self.table
         yield Footer()
 
@@ -405,15 +430,15 @@
         assert isinstance(table, DataTable)
         # Fetches hightlighted row ID (integer)
         row = table.cursor_row
         ioc_row = table.ordered_rows[row]
         col_keys = [ord_col.key.value for ord_col in table.ordered_columns]
         col_i = col_keys.index(col_key)
         ioc_col = table.ordered_columns[col_i]
-        cell: Union[str, SortableText] = table.get_cell(ioc_row.key, ioc_col.key)
+        cell: str | SortableText = table.get_cell(ioc_row.key, ioc_col.key)
         # SortableText inherits __str__() from Text
         return str(cell)
 
     def _get_service_name(self) -> str:
         service_name = self._get_highlighted_cell("name")
         return service_name
```

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/cmds/monitor.tcss` & `edge_containers_cli-3.5.3/src/edge_containers_cli/cmds/monitor.tcss`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/docker.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Utility functions for working interacting with docker / podman CLI
 """
 
 import re
 from pathlib import Path
 from time import sleep
-from typing import Optional, Union
+from typing import Optional
 
 import typer
 
 import edge_containers_cli.globals as globals
 import edge_containers_cli.shell as shell
 from edge_containers_cli.logging import log
 
@@ -107,15 +107,15 @@
 
     def logs(
         self,
         container: str,
         previous: bool = False,
         follow: bool = False,
         stdout: bool = False,
-    ) -> Optional[Union[str, bool]]:
+    ) -> Optional[str | bool]:
         """
         show logs from a container
         """
         self.is_running(container, error=True)
         prev = " -p" if previous else ""
         fol = " -f" if follow else ""
```

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/git.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/git.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/globals.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/globals.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/logging.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/logging.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/shell.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/shell.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 functions for executing commands and querying environment in the linux shell
 """
 
 import subprocess
-from typing import Union
 
 import typer
 from rich.console import Console
 from rich.style import Style
 
 import edge_containers_cli.globals as globals
 
@@ -35,15 +34,15 @@
     print an output to the console
     """
     console.print(output, style=Style(color="deep_sky_blue3", bold=True))
 
 
 def run_command(
     command: str, interactive=True, error_OK=False, show=False
-) -> Union[str, bool]:
+) -> str | bool:
     """
     Run a command and return the output
 
     if interactive is true then allow stdin and stdout, return the return code,
     otherwise return True for success and False for failure
 
     args:
@@ -61,15 +60,15 @@
     if interactive:
         output = error_out = ""
     else:
         output = p_result.stdout.decode()
         error_out = p_result.stderr.decode()
 
     if interactive:
-        result: Union[str, bool] = p_result.returncode == 0
+        result: str | bool = p_result.returncode == 0
     else:
         result = output + error_out
 
     if p_result.returncode != 0 and not error_OK:
         echo_error("\nCommand Failed:")
         if not globals.EC_VERBOSE:
             echo_command(command)
```

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli/utils.py` & `edge_containers_cli-3.5.3/src/edge_containers_cli/utils.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/PKG-INFO` & `edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-containers-cli
-Version: 3.5.2
+Version: 3.5.3
 Summary: CLI for deploying and managing epics containers IOCs and services
 Author-email: Giles Knap <giles.knap@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,18 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/epics-containers/edge-containers-cli
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: natsort
 Requires-Dist: typer[all]
 Requires-Dist: requests
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
```

### Comparing `edge_containers_cli-3.5.2/src/edge_containers_cli.egg-info/SOURCES.txt` & `edge_containers_cli-3.5.3/src/edge_containers_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/conftest.py` & `edge_containers_cli-3.5.3/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import shutil
+from collections.abc import Callable
 from pathlib import Path
 from types import SimpleNamespace
-from typing import Callable, Union
 
 from pytest import fixture
 from ruamel.yaml import YAML
 from typer import Context
 from typer.testing import CliRunner
 
 from edge_containers_cli.__main__ import cli
@@ -69,15 +69,15 @@
         if interactive:
             assert isinstance(rsp, bool), "interactive commands must return bool"
         else:
             assert isinstance(rsp, str), "non-interactive commands must return str"
 
         return rsp
 
-    def set_seq(self, cmd_rsp: list[dict[str, Union[str, bool]]]):
+    def set_seq(self, cmd_rsp: list[dict[str, str | bool]]):
         """
         Set up the expected sequence of commands that we expect to see come
         through the mock of run_command. Also supplies the response to
         return for each command. The structure of the list is as per the
         YAML files used in the tests e.g. tests/data/ioc.yaml
         """
         shutil.rmtree(TMPDIR, ignore_errors=True)
```

### Comparing `edge_containers_cli-3.5.2/tests/data/autocomplete.yaml` & `edge_containers_cli-3.5.3/tests/data/autocomplete.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/.github/workflows/ci_verify.sh` & `edge_containers_cli-3.5.3/tests/data/bl01t/.github/workflows/ci_verify.sh`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/LICENSE` & `edge_containers_cli-3.5.3/tests/data/bl01t/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/README.md` & `edge_containers_cli-3.5.3/tests/data/bl01t/README.md`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/environment.sh` & `edge_containers_cli-3.5.3/tests/data/bl01t/environment.sh`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/helm/shared/README.md` & `edge_containers_cli-3.5.3/tests/data/bl01t/helm/shared/README.md`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/helm/shared/values.yaml` & `edge_containers_cli-3.5.3/tests/data/bl01t/helm/shared/values.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/include/iocs/Chart.yaml` & `edge_containers_cli-3.5.3/tests/data/bl01t/include/iocs/Chart.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml` & `edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db` & `edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml` & `edge_containers_cli-3.5.3/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/ioc.yaml` & `edge_containers_cli-3.5.3/tests/data/ioc.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/data/local.yaml` & `edge_containers_cli-3.5.3/tests/data/local.yaml`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/test_autocomplete.py` & `edge_containers_cli-3.5.3/tests/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/test_ioc.py` & `edge_containers_cli-3.5.3/tests/test_ioc.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/test_local.py` & `edge_containers_cli-3.5.3/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `edge_containers_cli-3.5.2/tests/test_system.py` & `edge_containers_cli-3.5.3/tests/test_system.py`

 * *Files identical despite different names*

