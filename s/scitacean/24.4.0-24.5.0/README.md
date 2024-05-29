# Comparing `tmp/scitacean-24.4.0.tar.gz` & `tmp/scitacean-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scitacean-24.4.0.tar", last modified: Fri Apr 19 13:49:21 2024, max compression
+gzip compressed data, was "scitacean-24.5.0.tar", last modified: Wed May 29 08:10:48 2024, max compression
```

## Comparing `scitacean-24.4.0.tar` & `scitacean-24.5.0.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.529352 scitacean-24.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 13:49:16.000000 scitacean-24.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-19 13:49:16.000000 scitacean-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-19 13:49:16.000000 scitacean-24.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-19 13:49:16.000000 scitacean-24.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-19 13:49:16.000000 scitacean-24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 13:49:16.000000 scitacean-24.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-19 13:49:21.529352 scitacean-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-19 13:49:16.000000 scitacean-24.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-19 13:49:16.000000 scitacean-24.4.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/anaconda-icon.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_templates/scitacean-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_templates/scitacean-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/coding-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/dependency-management.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.509351 scitacean-24.4.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/classes-and-concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/downloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/testing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/uploading.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-19 13:49:16.000000 scitacean-24.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.509351 scitacean-24.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:49:21.529352 scitacean-24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.497351 scitacean-24.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.513351 scitacean-24.4.0/src/scitacean/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    45884 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_dataset_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.513351 scitacean-24.4.0/src/scitacean/_html_repr/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/_attachment_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/_common_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/_dataset_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.513351 scitacean-24.4.0/src/scitacean/_html_repr/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/images/lock.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.513351 scitacean-24.4.0/src/scitacean/_html_repr/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/styles/attachment.css
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/styles/common.css
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/styles/dataset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.517351 scitacean-24.4.0/src/scitacean/_html_repr/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/attachment_field_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/attachment_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/dataset_field_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/dataset_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/files_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/metadata_repr.html.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.517351 scitacean-24.4.0/src/scitacean/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/dataclass_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/file_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/orcid.py
--rw-r--r--   0 runner    (1001) docker     (127)    40371 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/datablock.py
--rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    28055 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.517351 scitacean-24.4.0/src/scitacean/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/_pytest_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.517351 scitacean-24.4.0/src/scitacean/testing/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/_pytest_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/docker-compose-backend-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/src/scitacean/testing/sftp/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/Dockerfile-sftp-server
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/_pytest_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/_sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/docker-compose-sftp-server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/src/scitacean/testing/sftp/sftp_server_seed/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/sftp_server_seed/table.csv
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/sftp_server_seed/text.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/src/scitacean/transfer/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/transfer/link.py
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/transfer/sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/transfer/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/src/scitacean/util/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/util/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/util/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/src/scitacean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/attachment_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/datablock_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/dataset_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/sample_client_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/common/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/dataset_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29310 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/download_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/filesystem_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/html_repr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/html_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/html_repr/html_repr_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/testing/strategies_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/thumbnail_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/transfer/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/transfer/link_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14556 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/transfer/sftp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/upload_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/util/formatter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.501351 scitacean-24.4.0/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tools/model-generation/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/generate_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tools/model-generation/spec/
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/dataset-fields.yml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/field-name-overrides.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/field-type-overrides.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/field-validations.yml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/masked-fields.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tools/model-generation/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/templates/dataset_fields.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/templates/model.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-19 13:49:16.000000 scitacean-24.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.924448 scitacean-24.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.896448 scitacean-24.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-29 08:10:42.000000 scitacean-24.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.896448 scitacean-24.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-29 08:10:42.000000 scitacean-24.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 08:10:42.000000 scitacean-24.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-29 08:10:42.000000 scitacean-24.5.0/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-29 08:10:42.000000 scitacean-24.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-29 08:10:42.000000 scitacean-24.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-29 08:10:42.000000 scitacean-24.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-29 08:10:42.000000 scitacean-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-29 08:10:42.000000 scitacean-24.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-29 08:10:42.000000 scitacean-24.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 08:10:42.000000 scitacean-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 08:10:42.000000 scitacean-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-29 08:10:48.920448 scitacean-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 08:10:42.000000 scitacean-24.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 08:10:42.000000 scitacean-24.5.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.896448 scitacean-24.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.896448 scitacean-24.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/_static/anaconda-icon.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.896448 scitacean-24.5.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.900448 scitacean-24.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/_templates/scitacean-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/_templates/scitacean-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.900448 scitacean-24.5.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/developer/coding-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/developer/dependency-management.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/developer/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/developer/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.900448 scitacean-24.5.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.900448 scitacean-24.5.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/user-guide/classes-and-concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/user-guide/downloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/user-guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/user-guide/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/user-guide/testing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-05-29 08:10:42.000000 scitacean-24.5.0/docs/user-guide/uploading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-29 08:10:42.000000 scitacean-24.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.904448 scitacean-24.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-29 08:10:42.000000 scitacean-24.5.0/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:10:48.924448 scitacean-24.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.892448 scitacean-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.904448 scitacean-24.5.0/src/scitacean/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44870 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_dataset_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.908448 scitacean-24.5.0/src/scitacean/_html_repr/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/_attachment_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/_common_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/_dataset_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.908448 scitacean-24.5.0/src/scitacean/_html_repr/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/images/lock.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.908448 scitacean-24.5.0/src/scitacean/_html_repr/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/styles/attachment.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/styles/common.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/styles/dataset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.908448 scitacean-24.5.0/src/scitacean/_html_repr/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/templates/attachment_field_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/templates/attachment_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/templates/dataset_field_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/templates/dataset_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/templates/files_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_html_repr/templates/metadata_repr.html.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.908448 scitacean-24.5.0/src/scitacean/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_internal/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_internal/file_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_internal/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/_internal/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44339 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/datablock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20085 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27618 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.912448 scitacean-24.5.0/src/scitacean/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/_pytest_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.912448 scitacean-24.5.0/src/scitacean/testing/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/backend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/backend/_pytest_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/backend/docker-compose-backend-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/backend/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/backend/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.912448 scitacean-24.5.0/src/scitacean/testing/sftp/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/sftp/Dockerfile-sftp-server
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/sftp/_pytest_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/sftp/_sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/sftp/docker-compose-sftp-server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/sftp/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.912448 scitacean-24.5.0/src/scitacean/testing/sftp/sftp_server_seed/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/sftp/sftp_server_seed/table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/sftp/sftp_server_seed/text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/testing/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.916448 scitacean-24.5.0/src/scitacean/transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/transfer/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/transfer/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/transfer/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.916448 scitacean-24.5.0/src/scitacean/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/util/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/util/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-29 08:10:42.000000 scitacean-24.5.0/src/scitacean/warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.920448 scitacean-24.5.0/src/scitacean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-29 08:10:48.000000 scitacean-24.5.0/src/scitacean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-29 08:10:48.000000 scitacean-24.5.0/src/scitacean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:10:48.000000 scitacean-24.5.0/src/scitacean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-29 08:10:48.000000 scitacean-24.5.0/src/scitacean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 08:10:48.000000 scitacean-24.5.0/src/scitacean.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.916448 scitacean-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.916448 scitacean-24.5.0/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/client/attachment_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/client/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/client/datablock_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/client/dataset_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/client/query_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/client/sample_client_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.916448 scitacean-24.5.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/dataset_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29256 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/download_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/filesystem_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.916448 scitacean-24.5.0/tests/html_repr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/html_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/html_repr/html_repr_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.920448 scitacean-24.5.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/testing/strategies_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/thumbnail_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.920448 scitacean-24.5.0/tests/transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/transfer/link_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14578 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/transfer/sftp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/upload_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.920448 scitacean-24.5.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-29 08:10:42.000000 scitacean-24.5.0/tests/util/formatter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.892448 scitacean-24.5.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.920448 scitacean-24.5.0/tools/model-generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/generate_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.920448 scitacean-24.5.0/tools/model-generation/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/spec/dataset-fields.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/spec/field-name-overrides.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/spec/field-type-overrides.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/spec/field-validations.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/spec/masked-fields.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/spec/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:10:48.920448 scitacean-24.5.0/tools/model-generation/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/templates/dataset_fields.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-29 08:10:42.000000 scitacean-24.5.0/tools/model-generation/templates/model.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-29 08:10:42.000000 scitacean-24.5.0/tox.ini
```

### Comparing `scitacean-24.4.0/.github/workflows/ci.yml` & `scitacean-24.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/.github/workflows/codeql-analysis.yml` & `scitacean-24.5.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/.github/workflows/dependency-review.yml` & `scitacean-24.5.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/.github/workflows/docs.yml` & `scitacean-24.5.0/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e docs
       - run: touch html/.nojekyll
       - uses: actions/upload-artifact@v4
         with:
           name: documentation
           path: html/
-      - uses: JamesIves/github-pages-deploy-action@v4.5.0
+      - uses: JamesIves/github-pages-deploy-action@v4.6.1
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           single-commit: true
           ssh-key: ${{ secrets.GH_PAGES_DEPLOY_KEY }}
```

### Comparing `scitacean-24.4.0/.github/workflows/release.yml` & `scitacean-24.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/.pre-commit-config.yaml` & `scitacean-24.5.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   rev: 0.7.1
   hooks:
     - id: nbstripout
       types: ["jupyter"]
       args: ["--drop-empty-cells",
              "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'"]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.0
+  rev: v0.4.2
   hooks:
     - id: ruff-format
       types_or: [ python, pyi ]
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
       types_or: [ python, pyi, jupyter ]
 - repo: https://github.com/codespell-project/codespell
```

### Comparing `scitacean-24.4.0/CODE_OF_CONDUCT.md` & `scitacean-24.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/CONTRIBUTING.md` & `scitacean-24.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/LICENSE` & `scitacean-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/PKG-INFO` & `scitacean-24.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitacean
-Version: 24.4.0
+Version: 24.5.0
 Summary: High-level interface for SciCat
 Author: Scitacean contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, SciCat Project
         All rights reserved.
         
@@ -48,24 +48,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: email-validator
+Requires-Dist: email-validator>=2
+Requires-Dist: httpx>=0.24
 Requires-Dist: pydantic>=2
-Requires-Dist: python-dateutil
-Requires-Dist: requests>=2.31
+Requires-Dist: python-dateutil>=2.8
 Provides-Extra: sftp
-Requires-Dist: paramiko; extra == "sftp"
+Requires-Dist: paramiko>=3; extra == "sftp"
 Provides-Extra: test
-Requires-Dist: filelock; extra == "test"
-Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: pyyaml; extra == "test"
+Requires-Dist: filelock>=3; extra == "test"
+Requires-Dist: hypothesis>=6.48; extra == "test"
+Requires-Dist: pyyaml>=5; extra == "test"
 
 [![PyPI badge](https://img.shields.io/pypi/v/scitacean.svg?style=flat-square&color=green)](https://pypi.python.org/pypi/scitacean)
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/scitacean?style=flat-square&color=green)](https://anaconda.org/conda-forge/scitacean)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7520487.svg)](https://doi.org/10.5281/zenodo.7520487)
 [![License: BSD 3-Clause](https://img.shields.io/github/license/SciCatProject/scitacean?style=flat-square&color=yellowgreen)](LICENSE)
 
 <picture>
```

### Comparing `scitacean-24.4.0/README.md` & `scitacean-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/SECURITY.md` & `scitacean-24.5.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/_static/anaconda-icon.js` & `scitacean-24.5.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/_static/css/custom.css` & `scitacean-24.5.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/_static/favicon.ico` & `scitacean-24.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/_static/logo-dark.svg` & `scitacean-24.5.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/_static/logo.svg` & `scitacean-24.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/_templates/scitacean-class-template.rst` & `scitacean-24.5.0/docs/_templates/scitacean-class-template.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/_templates/scitacean-module-template.rst` & `scitacean-24.5.0/docs/_templates/scitacean-module-template.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/conf.py` & `scitacean-24.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/developer/coding-conventions.rst` & `scitacean-24.5.0/docs/developer/coding-conventions.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/developer/dependency-management.rst` & `scitacean-24.5.0/docs/developer/dependency-management.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/developer/getting-started.rst` & `scitacean-24.5.0/docs/developer/getting-started.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/developer/testing.rst` & `scitacean-24.5.0/docs/developer/testing.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/index.rst` & `scitacean-24.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/reference/index.rst` & `scitacean-24.5.0/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/release-notes.rst` & `scitacean-24.5.0/docs/release-notes.rst`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,42 @@
 
    Deprecations
    ~~~~~~~~~~~~
 
    Stability, Maintainability, and Testing
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+vversion
+--------
+
+Security
+~~~~~~~~
+
+Features
+~~~~~~~~
+
+* Added experimental :meth:`client.ScicatClient.query_datasets` for querying datasets by field.
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+Bugfixes
+~~~~~~~~
+
+Documentation
+~~~~~~~~~~~~~
+
+Deprecations
+~~~~~~~~~~~~
+
+Stability, Maintainability, and Testing
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Replaced networking dependency ``requests`` with ``httpx``.
+
 v24.04.0
 --------
 
 Features
 ~~~~~~~~
 
 * Added functions for downloading and uploading samples: :meth:`Client.get_sample`, :meth:`Client.upload_new_sample_now`.
```

### Comparing `scitacean-24.4.0/docs/user-guide/classes-and-concepts.rst` & `scitacean-24.5.0/docs/user-guide/classes-and-concepts.rst`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/user-guide/downloading.ipynb` & `scitacean-24.5.0/docs/user-guide/downloading.ipynb`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/user-guide/logo.png` & `scitacean-24.5.0/docs/user-guide/logo.png`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/docs/user-guide/testing.ipynb` & `scitacean-24.5.0/docs/user-guide/testing.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999392614188533%*

 * *Differences: {"'cells'": "{35: {'source': {insert: [(4, '\\n')], delete: [4]}}}"}*

```diff
@@ -478,15 +478,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def test_something_with_real_client(real_client):\n",
                 "    if real_client is None:\n",
                 "        pytest.skip(\"Backend tests disabled\")\n",
                 "        # or do something else\n",
-                "    \n",
+                "\n",
                 "    # do the actual tests"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "36",
             "metadata": {},
```

### Comparing `scitacean-24.4.0/docs/user-guide/uploading.ipynb` & `scitacean-24.5.0/docs/user-guide/uploading.ipynb`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/pyproject.toml` & `scitacean-24.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,29 +24,33 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Typing :: Typed",
 ]
 requires-python = ">=3.10"
 dependencies = [
-    "email-validator",
+    "email-validator >= 2",
+    "httpx >= 0.24",
     "pydantic >= 2",
-    "python-dateutil",
-    "requests >= 2.31",
+    "python-dateutil >= 2.8",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Documentation" = "https://scicatproject.github.io/scitacean"
 "Bug Tracker" = "https://github.com/SciCatProject/scitacean/issues"
 "Source" = "https://github.com/SciCatProject/scitacean"
 
 [project.optional-dependencies]
-sftp = ["paramiko"]
-test = ["filelock", "hypothesis", "pyyaml"]
+sftp = ["paramiko >= 3"]
+test = [
+    "filelock >= 3",
+    "hypothesis >= 6.48",
+    "pyyaml >= 5"
+]
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 testpaths = "tests"
 addopts = """
@@ -90,31 +94,32 @@
 
 [tool.ruff]
 line-length = 88
 extend-include = ["*.ipynb"]
 extend-exclude = [".*", "__pycache__", "build", "dist", "venv"]
 
 [tool.ruff.lint]
-select = ["B", "D", "E", "F", "G", "I", "S", "T20", "UP", "PGH", "FBT003", "RUF"]
+select = ["B", "C4", "D", "DTZ", "E", "F", "G", "I", "FBT003", "PERF", "PGH", "PT", "PYI", "RUF", "S", "T20", "UP", "W"]
 ignore = [
-    "B905", # `zip()` without an explicit `strict=` parameter
-    "S324", # insecure hsh function; we don't use hashing for security
-    "E741", "E742", "E743", # do not use names ‘l’, ‘O’, or ‘I’; they are not a problem with a proper font
-    "UP038",  # does not seem to work and leads to slower code
-    "E111", "E114", "E117", "D206", "D300",  # conflict with ruff format
-    "D105",
+    "D105",  # most magic methods don't need docstrings as their purpose is always the same
+    "E741", "E742", "E743",  # do not use names ‘l’, ‘O’, or ‘I’; they are not a problem with a proper font
+    "UP038",  # leads to slower code
+    # Conflict with ruff format, see
+    # https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
+    "COM812", "COM819", "D206", "D300", "E111", "E114", "E117", "ISC001", "ISC002", "Q000", "Q001", "Q002", "Q003", "W191",
 ]
 fixable = ["I001"]
 isort.known-first-party = ["scitacean"]
 pydocstyle.convention = "numpy"
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = [
     "S101",  # asserts are fine in tests
     "D10",  # no docstrings required in tests
+    "S324",  # insecure hsh function; we don't use hashing for security
 ]
 "docs/*" = [
     "D", "E402", "F811", "F841", "RUF015", "S101", "T201",
 ]
 "*.ipynb" = ["I"]
 "docs/conf.py" = ["D10"]
 "tools/*" = ["D10"]
```

### Comparing `scitacean-24.4.0/requirements/base.txt` & `scitacean-24.5.0/requirements/base.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,60 @@
-# SHA1:6b8a253be2c23e3bf131e90c6b06c34bf612344f
+# SHA1:3e3a0c875b5da89f27065e036b85c7bcbf0d1700
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 annotated-types==0.6.0
     # via pydantic
-bcrypt==4.1.2
+anyio==4.3.0
+    # via httpx
+bcrypt==4.1.3
     # via paramiko
 certifi==2024.2.2
-    # via requests
+    # via
+    #   httpcore
+    #   httpx
 cffi==1.16.0
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.3.2
-    # via requests
-cryptography==42.0.5
+cryptography==42.0.7
     # via paramiko
-decorator==5.1.1
-    # via fabric
-deprecated==1.2.14
-    # via fabric
 dnspython==2.6.1
     # via email-validator
 email-validator==2.1.1
     # via -r base.in
-fabric==3.2.2
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
     # via -r base.in
 idna==3.7
     # via
+    #   anyio
     #   email-validator
-    #   requests
-invoke==2.2.0
-    # via fabric
+    #   httpx
 paramiko==3.4.0
-    # via
-    #   -r base.in
-    #   fabric
+    # via -r base.in
 pycparser==2.22
     # via cffi
-pydantic==2.7.0
+pydantic==2.7.1
     # via -r base.in
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pynacl==1.5.0
     # via paramiko
 python-dateutil==2.9.0.post0
     # via -r base.in
-requests==2.31.0
-    # via -r base.in
 six==1.16.0
     # via python-dateutil
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
 typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
-urllib3==2.2.1
-    # via requests
-wrapt==1.16.0
-    # via deprecated
```

### Comparing `scitacean-24.4.0/requirements/ci.txt` & `scitacean-24.5.0/requirements/ci.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,31 +9,27 @@
     # via tox
 chardet==5.2.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.4
+filelock==3.14.0
     # via
     #   tox
     #   virtualenv
 packaging==24.0
     # via
     #   pyproject-api
     #   tox
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   tox
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via tox
 pyproject-api==1.6.1
     # via tox
-tomli==2.0.1
-    # via
-    #   pyproject-api
-    #   tox
-tox==4.14.2
+tox==4.15.0
     # via -r ci.in
-virtualenv==20.25.3
+virtualenv==20.26.2
     # via tox
```

### Comparing `scitacean-24.4.0/requirements/dev.txt` & `scitacean-24.5.0/requirements/dev.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,42 @@
-# SHA1:769a2bd5b2bd098ca3a15ab6c50d67b6f30f0af4
+# SHA1:f8f8b250cced1edd7282d46fd442979050ea8c1a
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
 -r ci.txt
 -r docs.txt
 -r mypy.txt
 -r static.txt
 -r test.txt
 -r wheels.txt
-anyio==4.3.0
-    # via
-    #   httpx
-    #   jupyter-server
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 async-lru==2.0.4
     # via jupyterlab
 click==8.1.7
     # via
     #   pip-compile-multi
     #   pip-tools
 fqdn==1.5.1
     # via jsonschema
-h11==0.14.0
-    # via httpcore
-httpcore==1.0.5
-    # via httpx
-httpx==0.27.0
-    # via jupyterlab
 isoduration==20.11.0
     # via jsonschema
 json5==0.9.25
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.21.1
+jsonschema[format-nongpl]==4.22.0
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
 jupyter-events==0.10.0
     # via jupyter-server
 jupyter-lsp==2.2.5
@@ -55,17 +45,17 @@
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
 jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.1.6
+jupyterlab==4.2.0
     # via -r dev.in
-jupyterlab-server==2.26.0
+jupyterlab-server==2.27.1
     # via jupyterlab
 notebook-shim==0.2.4
     # via jupyterlab
 overrides==7.7.0
     # via jupyter-server
 pip-compile-multi==2.6.3
     # via -r dev.in
@@ -79,33 +69,29 @@
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-ruff==0.4.1
+ruff==0.4.4
     # via -r dev.in
 send2trash==1.8.3
     # via jupyter-server
-sniffio==1.3.1
-    # via
-    #   anyio
-    #   httpx
 terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 toposort==1.10
     # via pip-compile-multi
 uri-template==1.3.0
     # via jsonschema
 webcolors==1.13
     # via jsonschema
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via jupyter-server
 wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `scitacean-24.4.0/requirements/docs.txt` & `scitacean-24.5.0/requirements/docs.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,65 +3,69 @@
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
 -r test.txt
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
 alabaster==0.7.16
     # via sphinx
 asttokens==2.4.1
     # via stack-data
-autodoc-pydantic==2.1.0
+autodoc-pydantic==2.2.0
     # via -r docs.in
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.1.0
     # via nbconvert
+charset-normalizer==3.3.2
+    # via requests
 comm==0.2.2
     # via ipykernel
 debugpy==1.8.1
     # via ipykernel
+decorator==5.1.1
+    # via ipython
 defusedxml==0.7.1
     # via nbconvert
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
 imagesize==1.4.1
     # via sphinx
 ipykernel==6.29.4
     # via -r docs.in
-ipython==8.23.0
+ipython==8.24.0
     # via
     #   -r docs.in
     #   ipykernel
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
@@ -82,73 +86,75 @@
     # via
     #   jinja2
     #   nbconvert
 matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.2
     # via nbconvert
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via -r docs.in
 nbclient==0.10.0
     # via nbconvert
-nbconvert==7.16.3
+nbconvert==7.16.4
     # via nbsphinx
 nbformat==5.10.4
     # via
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.3
+nbsphinx==0.9.4
     # via -r docs.in
 nest-asyncio==1.6.0
     # via ipykernel
 pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via jupyter-core
 prompt-toolkit==3.0.43
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pydantic-settings==2.2.1
     # via autodoc-pydantic
 pydata-sphinx-theme==0.15.2
     # via -r docs.in
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   nbconvert
     #   pydata-sphinx-theme
     #   sphinx
 python-dotenv==1.0.1
     # via pydantic-settings
-pyzmq==26.0.1
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
-referencing==0.34.0
+referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-rpds-py==0.18.0
+requests==2.31.0
+    # via sphinx
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
@@ -178,15 +184,15 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 stack-data==0.6.3
     # via ipython
-tinycss2==1.2.1
+tinycss2==1.3.0
     # via nbconvert
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
 traitlets==5.14.3
     # via
@@ -196,13 +202,15 @@
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
+urllib3==2.2.1
+    # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
```

### Comparing `scitacean-24.4.0/requirements/static.txt` & `scitacean-24.5.0/requirements/static.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 #
 #    pip-compile-multi
 #
 cfgv==3.4.0
     # via pre-commit
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.4
+filelock==3.14.0
     # via virtualenv
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
 nodeenv==1.8.0
     # via pre-commit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via virtualenv
-pre-commit==3.7.0
+pre-commit==3.7.1
     # via -r static.in
 pyyaml==6.0.1
     # via pre-commit
-virtualenv==20.25.3
+virtualenv==20.26.2
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `scitacean-24.4.0/requirements/test.txt` & `scitacean-24.5.0/requirements/test.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-# SHA1:75deeef1826d3fede48f6f2de96ad90ac30e27a5
+# SHA1:6249614025d02c5c95194d10c86593010e5fbf04
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
 attrs==23.2.0
     # via hypothesis
-exceptiongroup==1.2.1
-    # via
-    #   hypothesis
-    #   pytest
 execnet==2.1.1
     # via pytest-xdist
-filelock[typing]==3.13.4
+filelock[typing]==3.14.0
     # via -r test.in
-hypothesis==6.100.1
+hypothesis==6.102.4
     # via -r test.in
 iniconfig==2.0.0
     # via pytest
 packaging==24.0
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pyfakefs==5.4.1
+pyfakefs==5.5.0
     # via -r test.in
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   -r test.in
     #   pytest-randomly
     #   pytest-socket
     #   pytest-xdist
 pytest-randomly==3.15.0
     # via -r test.in
 pytest-socket==0.7.0
     # via -r test.in
-pytest-xdist==3.5.0
+pytest-xdist==3.6.1
     # via -r test.in
 pyyaml==6.0.1
     # via -r test.in
 sortedcontainers==2.4.0
     # via hypothesis
-tomli==2.0.1
-    # via pytest
```

### Comparing `scitacean-24.4.0/src/scitacean/__init__.py` & `scitacean-24.5.0/src/scitacean/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_base_model.py` & `scitacean-24.5.0/src/scitacean/_base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,19 +232,14 @@
     dateutil's.
     """
     if not isinstance(value, str):
         return value
     return parse_datetime(value)
 
 
-def validate_drop(_: Any) -> None:
-    """Return ``None``."""
-    return None
-
-
 def validate_emails(value: str | None) -> str | None:
     if value is None:
         return value
     return ";".join(pydantic.validate_email(item)[1] for item in value.split(";"))
 
 
 def validate_orcids(value: str | None) -> str | None:
```

### Comparing `scitacean-24.4.0/src/scitacean/_dataset_fields.py` & `scitacean-24.5.0/src/scitacean/_dataset_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 # Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # flake8: noqa
 
 """Base class for Dataset."""
 
 from __future__ import annotations
 
+from dataclasses import dataclass
 from datetime import datetime, timezone
-from typing import Any, Dict, List, Literal, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Literal, TypeVar
 
 import dateutil.parser
 
 from ._base_model import DatasetType
-from ._internal.dataclass_wrapper import dataclass_optional_args
 from .datablock import OrigDatablock
 from .filesystem import RemotePath
 from .model import (
     construct,
     Attachment,
     BaseModel,
     BaseUserModel,
@@ -33,46 +33,46 @@
 )
 from .pid import PID
 
 
 M = TypeVar("M", bound=BaseModel)
 
 
-def _parse_datetime(x: Optional[Union[datetime, str]]) -> Optional[datetime]:
+def _parse_datetime(x: datetime | str | None) -> datetime | None:
     if isinstance(x, datetime) or x is None:
         return x
     if x == "now":
         return datetime.now(tz=timezone.utc)
     return dateutil.parser.parse(x)
 
 
-def _parse_pid(pid: Optional[Union[str, PID]]) -> Optional[PID]:
+def _parse_pid(pid: str | PID | None) -> PID | None:
     if pid is None:
         return pid
     return PID.parse(pid)
 
 
-def _parse_remote_path(path: Optional[Union[str, RemotePath]]) -> Optional[RemotePath]:
+def _parse_remote_path(path: str | RemotePath | None) -> RemotePath | None:
     if path is None:
         return path
     return RemotePath(path)
 
 
-def _validate_checksum_algorithm(algorithm: Optional[str]) -> Optional[str]:
+def _validate_checksum_algorithm(algorithm: str | None) -> str | None:
     if algorithm is None:
         return algorithm
     import hashlib
 
     if algorithm not in hashlib.algorithms_available:
         raise ValueError(f"Checksum algorithm not recognized: {algorithm}")
     return algorithm
 
 
 class DatasetBase:
-    @dataclass_optional_args(frozen=True, kw_only=True, slots=True)
+    @dataclass(frozen=True, kw_only=True, slots=True)
     class Field:
         name: str
         description: str
         read_only: bool
         required: bool
         scicat_name: str
         type: type
@@ -99,15 +99,15 @@
         ),
         Field(
             name="access_groups",
             description="Optional additional groups which have read access to the data. Users which are members in one of the groups listed here are allowed to access this data. The special group 'public' makes data available to all users.",
             read_only=False,
             required=False,
             scicat_name="accessGroups",
-            type=List[str],
+            type=list[str],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="api_version",
             description="Version of the API used in creation of the dataset.",
             read_only=True,
@@ -224,30 +224,20 @@
             required=False,
             scicat_name="endTime",
             type=datetime,
             used_by_derived=False,
             used_by_raw=True,
         ),
         Field(
-            name="history",
-            description="List of objects containing old and new values.",
-            read_only=True,
-            required=False,
-            scicat_name="history",
-            type=type(None),
-            used_by_derived=True,
-            used_by_raw=True,
-        ),
-        Field(
             name="input_datasets",
             description="Array of input dataset identifiers used in producing the derived dataset. Ideally these are the global identifier to existing datasets inside this or federated data catalogs. This field is required if the dataset is a Derived dataset.",
             read_only=False,
             required=True,
             scicat_name="inputDatasets",
-            type=List[PID],
+            type=list[PID],
             used_by_derived=True,
             used_by_raw=False,
         ),
         Field(
             name="instrument_group",
             description="Optional additional groups which have read and write access to the data. Users which are members in one of the groups listed here are allowed to access this data.",
             read_only=False,
@@ -299,25 +289,25 @@
         ),
         Field(
             name="job_parameters",
             description="The creation process of the derived data will usually depend on input job parameters. The full structure of these input parameters are stored here.",
             read_only=False,
             required=False,
             scicat_name="jobParameters",
-            type=Dict[str, Any],
+            type=dict[str, Any],
             used_by_derived=True,
             used_by_raw=False,
         ),
         Field(
             name="keywords",
             description="Array of tags associated with the meaning or contents of this dataset. Values should ideally come from defined vocabularies, taxonomies, ontologies or knowledge graphs.",
             read_only=False,
             required=False,
             scicat_name="keywords",
-            type=List[str],
+            type=list[str],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="license",
             description="Name of the license under which the data can be used.",
             read_only=False,
@@ -419,15 +409,15 @@
         ),
         Field(
             name="relationships",
             description="Stores the relationships with other datasets.",
             read_only=False,
             required=False,
             scicat_name="relationships",
-            type=List[Relationship],
+            type=list[Relationship],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="sample_id",
             description="ID of the sample used when collecting the data.",
             read_only=False,
@@ -439,15 +429,15 @@
         ),
         Field(
             name="shared_with",
             description="List of users that the dataset has been shared with.",
             read_only=False,
             required=False,
             scicat_name="sharedWith",
-            type=List[str],
+            type=list[str],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="source_folder",
             description="Absolute file path on file server containing the files of this dataset, e.g. /some/path/to/sourcefolder. In case of a single file dataset, e.g. HDF5 data, it contains the path up to, but excluding the filename. Trailing slashes are removed.",
             read_only=False,
@@ -469,15 +459,15 @@
         ),
         Field(
             name="techniques",
             description="Stores the metadata information for techniques.",
             read_only=False,
             required=False,
             scicat_name="techniques",
-            type=List[Technique],
+            type=list[Technique],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="updated_at",
             description="Date and time when this record was updated last. This property is added and maintained by mongoose.",
             read_only=True,
@@ -499,15 +489,15 @@
         ),
         Field(
             name="used_software",
             description="A list of links to software repositories which uniquely identifies the pieces of software, including versions, used for yielding the derived data. This field is required if the dataset is a Derived dataset.",
             read_only=False,
             required=True,
             scicat_name="usedSoftware",
-            type=List[str],
+            type=list[str],
             used_by_derived=True,
             used_by_raw=False,
         ),
         Field(
             name="validation_status",
             description="Defines a level of trust, e.g. a measure of how much data was verified or used by other persons.",
             read_only=False,
@@ -529,15 +519,14 @@
         "_created_by",
         "_creation_location",
         "_creation_time",
         "_data_format",
         "_data_quality_metrics",
         "_description",
         "_end_time",
-        "_history",
         "_input_datasets",
         "_instrument_group",
         "_instrument_id",
         "_investigator",
         "_is_published",
         "_job_log_data",
         "_job_parameters",
@@ -567,51 +556,51 @@
         "_default_checksum_algorithm",
         "_orig_datablocks",
         "_attachments",
     )
 
     def __init__(
         self,
-        type: Union[DatasetType, Literal["raw", "derived"]],
-        access_groups: Optional[List[str]] = None,
-        classification: Optional[str] = None,
-        comment: Optional[str] = None,
-        contact_email: Optional[str] = None,
-        creation_location: Optional[str] = None,
-        creation_time: Optional[Union[str, datetime]] = "now",
-        data_format: Optional[str] = None,
-        data_quality_metrics: Optional[int] = None,
-        description: Optional[str] = None,
-        end_time: Optional[datetime] = None,
-        input_datasets: Optional[List[PID]] = None,
-        instrument_group: Optional[str] = None,
-        instrument_id: Optional[str] = None,
-        investigator: Optional[str] = None,
-        is_published: Optional[bool] = None,
-        job_log_data: Optional[str] = None,
-        job_parameters: Optional[Dict[str, Any]] = None,
-        keywords: Optional[List[str]] = None,
-        license: Optional[str] = None,
-        name: Optional[str] = None,
-        orcid_of_owner: Optional[str] = None,
-        owner: Optional[str] = None,
-        owner_email: Optional[str] = None,
-        owner_group: Optional[str] = None,
-        principal_investigator: Optional[str] = None,
-        proposal_id: Optional[str] = None,
-        relationships: Optional[List[Relationship]] = None,
-        sample_id: Optional[str] = None,
-        shared_with: Optional[List[str]] = None,
-        source_folder: Optional[Union[RemotePath, str]] = None,
-        source_folder_host: Optional[str] = None,
-        techniques: Optional[List[Technique]] = None,
-        used_software: Optional[List[str]] = None,
-        validation_status: Optional[str] = None,
-        meta: Optional[Dict[str, Any]] = None,
-        checksum_algorithm: Optional[str] = "blake2b",
+        type: DatasetType | Literal["raw", "derived"],
+        access_groups: list[str] | None = None,
+        classification: str | None = None,
+        comment: str | None = None,
+        contact_email: str | None = None,
+        creation_location: str | None = None,
+        creation_time: str | datetime | None = "now",
+        data_format: str | None = None,
+        data_quality_metrics: int | None = None,
+        description: str | None = None,
+        end_time: datetime | None = None,
+        input_datasets: list[PID] | None = None,
+        instrument_group: str | None = None,
+        instrument_id: str | None = None,
+        investigator: str | None = None,
+        is_published: bool | None = None,
+        job_log_data: str | None = None,
+        job_parameters: dict[str, Any] | None = None,
+        keywords: list[str] | None = None,
+        license: str | None = None,
+        name: str | None = None,
+        orcid_of_owner: str | None = None,
+        owner: str | None = None,
+        owner_email: str | None = None,
+        owner_group: str | None = None,
+        principal_investigator: str | None = None,
+        proposal_id: str | None = None,
+        relationships: list[Relationship] | None = None,
+        sample_id: str | None = None,
+        shared_with: list[str] | None = None,
+        source_folder: RemotePath | str | None = None,
+        source_folder_host: str | None = None,
+        techniques: list[Technique] | None = None,
+        used_software: list[str] | None = None,
+        validation_status: str | None = None,
+        meta: dict[str, Any] | None = None,
+        checksum_algorithm: str | None = "blake2b",
     ) -> None:
         self._type = DatasetType(type)
         self._access_groups = access_groups
         self._classification = classification
         self._comment = comment
         self._contact_email = contact_email
         self._creation_location = creation_location
@@ -643,466 +632,460 @@
         self._source_folder_host = source_folder_host
         self._techniques = techniques
         self._used_software = used_software
         self._validation_status = validation_status
         self._api_version = None
         self._created_at = None
         self._created_by = None
-        self._history = None
         self._lifecycle = None
         self._pid = None
         self._updated_at = None
         self._updated_by = None
         self._meta = meta or {}
         self._default_checksum_algorithm = _validate_checksum_algorithm(
             checksum_algorithm
         )
-        self._orig_datablocks: List[OrigDatablock] = []
-        self._attachments: Optional[List[Attachment]] = []
+        self._orig_datablocks: list[OrigDatablock] = []
+        self._attachments: list[Attachment] | None = []
 
     @property
-    def access_groups(self) -> Optional[List[str]]:
+    def access_groups(self) -> list[str] | None:
         """Optional additional groups which have read access to the data. Users which are members in one of the groups listed here are allowed to access this data. The special group 'public' makes data available to all users."""
         return self._access_groups
 
     @access_groups.setter
-    def access_groups(self, access_groups: Optional[List[str]]) -> None:
+    def access_groups(self, access_groups: list[str] | None) -> None:
         """Optional additional groups which have read access to the data. Users which are members in one of the groups listed here are allowed to access this data. The special group 'public' makes data available to all users."""
         self._access_groups = access_groups
 
     @property
-    def api_version(self) -> Optional[str]:
+    def api_version(self) -> str | None:
         """Version of the API used in creation of the dataset."""
         return self._api_version
 
     @property
-    def classification(self) -> Optional[str]:
+    def classification(self) -> str | None:
         """ACIA information about AUthenticity,COnfidentiality,INtegrity and AVailability requirements of dataset. E.g. AV(ailabilty)=medium could trigger the creation of a two tape copies. Format 'AV=medium,CO=low'"""
         return self._classification
 
     @classification.setter
-    def classification(self, classification: Optional[str]) -> None:
+    def classification(self, classification: str | None) -> None:
         """ACIA information about AUthenticity,COnfidentiality,INtegrity and AVailability requirements of dataset. E.g. AV(ailabilty)=medium could trigger the creation of a two tape copies. Format 'AV=medium,CO=low'"""
         self._classification = classification
 
     @property
-    def comment(self) -> Optional[str]:
+    def comment(self) -> str | None:
         """Comment the user has about a given dataset."""
         return self._comment
 
     @comment.setter
-    def comment(self, comment: Optional[str]) -> None:
+    def comment(self, comment: str | None) -> None:
         """Comment the user has about a given dataset."""
         self._comment = comment
 
     @property
-    def contact_email(self) -> Optional[str]:
+    def contact_email(self) -> str | None:
         """Email of the contact person for this dataset. The string may contain a list of emails, which should then be separated by semicolons."""
         return self._contact_email
 
     @contact_email.setter
-    def contact_email(self, contact_email: Optional[str]) -> None:
+    def contact_email(self, contact_email: str | None) -> None:
         """Email of the contact person for this dataset. The string may contain a list of emails, which should then be separated by semicolons."""
         self._contact_email = contact_email
 
     @property
-    def created_at(self) -> Optional[datetime]:
+    def created_at(self) -> datetime | None:
         """Date and time when this record was created. This property is added and maintained by mongoose."""
         return self._created_at
 
     @property
-    def created_by(self) -> Optional[str]:
+    def created_by(self) -> str | None:
         """Indicate the user who created this record. This property is added and maintained by the system."""
         return self._created_by
 
     @property
-    def creation_location(self) -> Optional[str]:
+    def creation_location(self) -> str | None:
         """Unique location identifier where data was taken, usually in the form /Site-name/facility-name/instrumentOrBeamline-name. This field is required if the dataset is a Raw dataset."""
         return self._creation_location
 
     @creation_location.setter
-    def creation_location(self, creation_location: Optional[str]) -> None:
+    def creation_location(self, creation_location: str | None) -> None:
         """Unique location identifier where data was taken, usually in the form /Site-name/facility-name/instrumentOrBeamline-name. This field is required if the dataset is a Raw dataset."""
         self._creation_location = creation_location
 
     @property
-    def creation_time(self) -> Optional[datetime]:
+    def creation_time(self) -> datetime | None:
         """Time when dataset became fully available on disk, i.e. all containing files have been written. Format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server."""
         return self._creation_time
 
     @creation_time.setter
-    def creation_time(self, creation_time: Optional[Union[str, datetime]]) -> None:
+    def creation_time(self, creation_time: str | datetime | None) -> None:
         """Time when dataset became fully available on disk, i.e. all containing files have been written. Format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server."""
         self._creation_time = _parse_datetime(creation_time)
 
     @property
-    def data_format(self) -> Optional[str]:
+    def data_format(self) -> str | None:
         """Defines the format of the data files in this dataset, e.g Nexus Version x.y."""
         return self._data_format
 
     @data_format.setter
-    def data_format(self, data_format: Optional[str]) -> None:
+    def data_format(self, data_format: str | None) -> None:
         """Defines the format of the data files in this dataset, e.g Nexus Version x.y."""
         self._data_format = data_format
 
     @property
-    def data_quality_metrics(self) -> Optional[int]:
+    def data_quality_metrics(self) -> int | None:
         """Data Quality Metrics given by the user to rate the dataset."""
         return self._data_quality_metrics
 
     @data_quality_metrics.setter
-    def data_quality_metrics(self, data_quality_metrics: Optional[int]) -> None:
+    def data_quality_metrics(self, data_quality_metrics: int | None) -> None:
         """Data Quality Metrics given by the user to rate the dataset."""
         self._data_quality_metrics = data_quality_metrics
 
     @property
-    def description(self) -> Optional[str]:
+    def description(self) -> str | None:
         """Free text explanation of contents of dataset."""
         return self._description
 
     @description.setter
-    def description(self, description: Optional[str]) -> None:
+    def description(self, description: str | None) -> None:
         """Free text explanation of contents of dataset."""
         self._description = description
 
     @property
-    def end_time(self) -> Optional[datetime]:
+    def end_time(self) -> datetime | None:
         """End time of data acquisition for this dataset, format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server."""
         return self._end_time
 
     @end_time.setter
-    def end_time(self, end_time: Optional[datetime]) -> None:
+    def end_time(self, end_time: datetime | None) -> None:
         """End time of data acquisition for this dataset, format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server."""
         self._end_time = end_time
 
     @property
-    def history(self) -> Optional[None]:
-        """List of objects containing old and new values."""
-        return self._history
-
-    @property
-    def input_datasets(self) -> Optional[List[PID]]:
+    def input_datasets(self) -> list[PID] | None:
         """Array of input dataset identifiers used in producing the derived dataset. Ideally these are the global identifier to existing datasets inside this or federated data catalogs. This field is required if the dataset is a Derived dataset."""
         return self._input_datasets
 
     @input_datasets.setter
-    def input_datasets(self, input_datasets: Optional[List[PID]]) -> None:
+    def input_datasets(self, input_datasets: list[PID] | None) -> None:
         """Array of input dataset identifiers used in producing the derived dataset. Ideally these are the global identifier to existing datasets inside this or federated data catalogs. This field is required if the dataset is a Derived dataset."""
         self._input_datasets = input_datasets
 
     @property
-    def instrument_group(self) -> Optional[str]:
+    def instrument_group(self) -> str | None:
         """Optional additional groups which have read and write access to the data. Users which are members in one of the groups listed here are allowed to access this data."""
         return self._instrument_group
 
     @instrument_group.setter
-    def instrument_group(self, instrument_group: Optional[str]) -> None:
+    def instrument_group(self, instrument_group: str | None) -> None:
         """Optional additional groups which have read and write access to the data. Users which are members in one of the groups listed here are allowed to access this data."""
         self._instrument_group = instrument_group
 
     @property
-    def instrument_id(self) -> Optional[str]:
+    def instrument_id(self) -> str | None:
         """ID of the instrument where the data was created."""
         return self._instrument_id
 
     @instrument_id.setter
-    def instrument_id(self, instrument_id: Optional[str]) -> None:
+    def instrument_id(self, instrument_id: str | None) -> None:
         """ID of the instrument where the data was created."""
         self._instrument_id = instrument_id
 
     @property
-    def investigator(self) -> Optional[str]:
+    def investigator(self) -> str | None:
         """First name and last name of the person or people pursuing the data analysis. The string may contain a list of names, which should then be separated by semicolons."""
         return self._investigator
 
     @investigator.setter
-    def investigator(self, investigator: Optional[str]) -> None:
+    def investigator(self, investigator: str | None) -> None:
         """First name and last name of the person or people pursuing the data analysis. The string may contain a list of names, which should then be separated by semicolons."""
         self._investigator = investigator
 
     @property
-    def is_published(self) -> Optional[bool]:
+    def is_published(self) -> bool | None:
         """Flag is true when data are made publicly available."""
         return self._is_published
 
     @is_published.setter
-    def is_published(self, is_published: Optional[bool]) -> None:
+    def is_published(self, is_published: bool | None) -> None:
         """Flag is true when data are made publicly available."""
         self._is_published = is_published
 
     @property
-    def job_log_data(self) -> Optional[str]:
+    def job_log_data(self) -> str | None:
         """The output job logfile. Keep the size of this log data well below 15 MB."""
         return self._job_log_data
 
     @job_log_data.setter
-    def job_log_data(self, job_log_data: Optional[str]) -> None:
+    def job_log_data(self, job_log_data: str | None) -> None:
         """The output job logfile. Keep the size of this log data well below 15 MB."""
         self._job_log_data = job_log_data
 
     @property
-    def job_parameters(self) -> Optional[Dict[str, Any]]:
+    def job_parameters(self) -> dict[str, Any] | None:
         """The creation process of the derived data will usually depend on input job parameters. The full structure of these input parameters are stored here."""
         return self._job_parameters
 
     @job_parameters.setter
-    def job_parameters(self, job_parameters: Optional[Dict[str, Any]]) -> None:
+    def job_parameters(self, job_parameters: dict[str, Any] | None) -> None:
         """The creation process of the derived data will usually depend on input job parameters. The full structure of these input parameters are stored here."""
         self._job_parameters = job_parameters
 
     @property
-    def keywords(self) -> Optional[List[str]]:
+    def keywords(self) -> list[str] | None:
         """Array of tags associated with the meaning or contents of this dataset. Values should ideally come from defined vocabularies, taxonomies, ontologies or knowledge graphs."""
         return self._keywords
 
     @keywords.setter
-    def keywords(self, keywords: Optional[List[str]]) -> None:
+    def keywords(self, keywords: list[str] | None) -> None:
         """Array of tags associated with the meaning or contents of this dataset. Values should ideally come from defined vocabularies, taxonomies, ontologies or knowledge graphs."""
         self._keywords = keywords
 
     @property
-    def license(self) -> Optional[str]:
+    def license(self) -> str | None:
         """Name of the license under which the data can be used."""
         return self._license
 
     @license.setter
-    def license(self, license: Optional[str]) -> None:
+    def license(self, license: str | None) -> None:
         """Name of the license under which the data can be used."""
         self._license = license
 
     @property
-    def lifecycle(self) -> Optional[Lifecycle]:
+    def lifecycle(self) -> Lifecycle | None:
         """Describes the current status of the dataset during its lifetime with respect to the storage handling systems."""
         return self._lifecycle
 
     @property
-    def name(self) -> Optional[str]:
+    def name(self) -> str | None:
         """A name for the dataset, given by the creator to carry some semantic meaning. Useful for display purposes e.g. instead of displaying the pid. Will be autofilled if missing using info from sourceFolder."""
         return self._name
 
     @name.setter
-    def name(self, name: Optional[str]) -> None:
+    def name(self, name: str | None) -> None:
         """A name for the dataset, given by the creator to carry some semantic meaning. Useful for display purposes e.g. instead of displaying the pid. Will be autofilled if missing using info from sourceFolder."""
         self._name = name
 
     @property
-    def orcid_of_owner(self) -> Optional[str]:
+    def orcid_of_owner(self) -> str | None:
         """ORCID of the owner or custodian. The string may contain a list of ORCIDs, which should then be separated by semicolons."""
         return self._orcid_of_owner
 
     @orcid_of_owner.setter
-    def orcid_of_owner(self, orcid_of_owner: Optional[str]) -> None:
+    def orcid_of_owner(self, orcid_of_owner: str | None) -> None:
         """ORCID of the owner or custodian. The string may contain a list of ORCIDs, which should then be separated by semicolons."""
         self._orcid_of_owner = orcid_of_owner
 
     @property
-    def owner(self) -> Optional[str]:
+    def owner(self) -> str | None:
         """Owner or custodian of the dataset, usually first name + last name. The string may contain a list of persons, which should then be separated by semicolons."""
         return self._owner
 
     @owner.setter
-    def owner(self, owner: Optional[str]) -> None:
+    def owner(self, owner: str | None) -> None:
         """Owner or custodian of the dataset, usually first name + last name. The string may contain a list of persons, which should then be separated by semicolons."""
         self._owner = owner
 
     @property
-    def owner_email(self) -> Optional[str]:
+    def owner_email(self) -> str | None:
         """Email of the owner or custodian of the dataset. The string may contain a list of emails, which should then be separated by semicolons."""
         return self._owner_email
 
     @owner_email.setter
-    def owner_email(self, owner_email: Optional[str]) -> None:
+    def owner_email(self, owner_email: str | None) -> None:
         """Email of the owner or custodian of the dataset. The string may contain a list of emails, which should then be separated by semicolons."""
         self._owner_email = owner_email
 
     @property
-    def owner_group(self) -> Optional[str]:
+    def owner_group(self) -> str | None:
         """Defines the group which owns the data, and therefore has unrestricted access to this data. Usually a pgroup like p12151"""
         return self._owner_group
 
     @owner_group.setter
-    def owner_group(self, owner_group: Optional[str]) -> None:
+    def owner_group(self, owner_group: str | None) -> None:
         """Defines the group which owns the data, and therefore has unrestricted access to this data. Usually a pgroup like p12151"""
         self._owner_group = owner_group
 
     @property
-    def pid(self) -> Optional[PID]:
+    def pid(self) -> PID | None:
         """Persistent Identifier for datasets derived from UUIDv4 and prepended automatically by site specific PID prefix like 20.500.12345/"""
         return self._pid
 
     @property
-    def principal_investigator(self) -> Optional[str]:
+    def principal_investigator(self) -> str | None:
         """First name and last name of principal investigator(s). If multiple PIs are present, use a semicolon separated list. This field is required if the dataset is a Raw dataset."""
         return self._principal_investigator
 
     @principal_investigator.setter
-    def principal_investigator(self, principal_investigator: Optional[str]) -> None:
+    def principal_investigator(self, principal_investigator: str | None) -> None:
         """First name and last name of principal investigator(s). If multiple PIs are present, use a semicolon separated list. This field is required if the dataset is a Raw dataset."""
         self._principal_investigator = principal_investigator
 
     @property
-    def proposal_id(self) -> Optional[str]:
+    def proposal_id(self) -> str | None:
         """The ID of the proposal to which the dataset belongs."""
         return self._proposal_id
 
     @proposal_id.setter
-    def proposal_id(self, proposal_id: Optional[str]) -> None:
+    def proposal_id(self, proposal_id: str | None) -> None:
         """The ID of the proposal to which the dataset belongs."""
         self._proposal_id = proposal_id
 
     @property
-    def relationships(self) -> Optional[List[Relationship]]:
+    def relationships(self) -> list[Relationship] | None:
         """Stores the relationships with other datasets."""
         return self._relationships
 
     @relationships.setter
-    def relationships(self, relationships: Optional[List[Relationship]]) -> None:
+    def relationships(self, relationships: list[Relationship] | None) -> None:
         """Stores the relationships with other datasets."""
         self._relationships = relationships
 
     @property
-    def sample_id(self) -> Optional[str]:
+    def sample_id(self) -> str | None:
         """ID of the sample used when collecting the data."""
         return self._sample_id
 
     @sample_id.setter
-    def sample_id(self, sample_id: Optional[str]) -> None:
+    def sample_id(self, sample_id: str | None) -> None:
         """ID of the sample used when collecting the data."""
         self._sample_id = sample_id
 
     @property
-    def shared_with(self) -> Optional[List[str]]:
+    def shared_with(self) -> list[str] | None:
         """List of users that the dataset has been shared with."""
         return self._shared_with
 
     @shared_with.setter
-    def shared_with(self, shared_with: Optional[List[str]]) -> None:
+    def shared_with(self, shared_with: list[str] | None) -> None:
         """List of users that the dataset has been shared with."""
         self._shared_with = shared_with
 
     @property
-    def source_folder(self) -> Optional[RemotePath]:
+    def source_folder(self) -> RemotePath | None:
         """Absolute file path on file server containing the files of this dataset, e.g. /some/path/to/sourcefolder. In case of a single file dataset, e.g. HDF5 data, it contains the path up to, but excluding the filename. Trailing slashes are removed."""
         return self._source_folder
 
     @source_folder.setter
-    def source_folder(self, source_folder: Optional[Union[RemotePath, str]]) -> None:
+    def source_folder(self, source_folder: RemotePath | str | None) -> None:
         """Absolute file path on file server containing the files of this dataset, e.g. /some/path/to/sourcefolder. In case of a single file dataset, e.g. HDF5 data, it contains the path up to, but excluding the filename. Trailing slashes are removed."""
         self._source_folder = _parse_remote_path(source_folder)
 
     @property
-    def source_folder_host(self) -> Optional[str]:
+    def source_folder_host(self) -> str | None:
         """DNS host name of file server hosting sourceFolder, optionally including a protocol e.g. [protocol://]fileserver1.example.com"""
         return self._source_folder_host
 
     @source_folder_host.setter
-    def source_folder_host(self, source_folder_host: Optional[str]) -> None:
+    def source_folder_host(self, source_folder_host: str | None) -> None:
         """DNS host name of file server hosting sourceFolder, optionally including a protocol e.g. [protocol://]fileserver1.example.com"""
         self._source_folder_host = source_folder_host
 
     @property
-    def techniques(self) -> Optional[List[Technique]]:
+    def techniques(self) -> list[Technique] | None:
         """Stores the metadata information for techniques."""
         return self._techniques
 
     @techniques.setter
-    def techniques(self, techniques: Optional[List[Technique]]) -> None:
+    def techniques(self, techniques: list[Technique] | None) -> None:
         """Stores the metadata information for techniques."""
         self._techniques = techniques
 
     @property
-    def updated_at(self) -> Optional[datetime]:
+    def updated_at(self) -> datetime | None:
         """Date and time when this record was updated last. This property is added and maintained by mongoose."""
         return self._updated_at
 
     @property
-    def updated_by(self) -> Optional[str]:
+    def updated_by(self) -> str | None:
         """Indicate the user who updated this record last. This property is added and maintained by the system."""
         return self._updated_by
 
     @property
-    def used_software(self) -> Optional[List[str]]:
+    def used_software(self) -> list[str] | None:
         """A list of links to software repositories which uniquely identifies the pieces of software, including versions, used for yielding the derived data. This field is required if the dataset is a Derived dataset."""
         return self._used_software
 
     @used_software.setter
-    def used_software(self, used_software: Optional[List[str]]) -> None:
+    def used_software(self, used_software: list[str] | None) -> None:
         """A list of links to software repositories which uniquely identifies the pieces of software, including versions, used for yielding the derived data. This field is required if the dataset is a Derived dataset."""
         self._used_software = used_software
 
     @property
-    def validation_status(self) -> Optional[str]:
+    def validation_status(self) -> str | None:
         """Defines a level of trust, e.g. a measure of how much data was verified or used by other persons."""
         return self._validation_status
 
     @validation_status.setter
-    def validation_status(self, validation_status: Optional[str]) -> None:
+    def validation_status(self, validation_status: str | None) -> None:
         """Defines a level of trust, e.g. a measure of how much data was verified or used by other persons."""
         self._validation_status = validation_status
 
     @property
-    def meta(self) -> Dict[str, Any]:
+    def meta(self) -> dict[str, Any]:
         """Dict of scientific metadata."""
         return self._meta
 
     @meta.setter
-    def meta(self, meta: Dict[str, Any]) -> None:
+    def meta(self, meta: dict[str, Any]) -> None:
         """Dict of scientific metadata."""
         self._meta = meta
 
     @property
     def type(self) -> DatasetType:
         """Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models."""
         return self._type
 
     @staticmethod
     def _prepare_fields_from_download(
         download_model: DownloadDataset,
-    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+    ) -> tuple[dict[str, Any], dict[str, Any]]:
         init_args = {}
         read_only = {}
         for field in DatasetBase._FIELD_SPEC:
             if field.read_only:
                 read_only["_" + field.name] = getattr(download_model, field.scicat_name)
             else:
                 init_args[field.name] = getattr(download_model, field.scicat_name)
 
         init_args["meta"] = download_model.scientificMetadata
         _convert_download_fields_in_place(init_args, read_only)
 
         return init_args, read_only
 
     @staticmethod
-    def _convert_readonly_fields_in_place(read_only: Dict[str, Any]) -> None:
+    def _convert_readonly_fields_in_place(read_only: dict[str, Any]) -> None:
         if (pid := read_only.get("_pid")) is not None:
             read_only["_pid"] = _parse_pid(pid)
 
 
 def _convert_download_fields_in_place(
-    init_args: Dict[str, Any], read_only: Dict[str, Any]
+    init_args: dict[str, Any], read_only: dict[str, Any]
 ) -> None:
     for mod, key in ((Technique, "techniques"), (Relationship, "relationships")):
         init_args[key] = _list_field_from_download(mod, init_args.get(key))
 
     DatasetBase._convert_readonly_fields_in_place(read_only)
     if (lifecycle := read_only.get("_lifecycle")) is not None:
         read_only["_lifecycle"] = Lifecycle.from_download_model(
             _as_model(DownloadLifecycle, lifecycle)
         )
 
 
 def _list_field_from_download(
-    mod: Type[BaseUserModel], value: Optional[List[Any]]
-) -> Optional[List[BaseUserModel]]:
+    mod: type[BaseUserModel], value: list[Any] | None
+) -> list[BaseUserModel] | None:
     if value is None:
         return None
     return [
         mod.from_download_model(_as_model(mod.download_model_type(), item))
         for item in value
     ]
 
 
 # If validation fails, sub models are not converted automatically by Pydantic.
-def _as_model(mod: Type[M], value: Union[M, Dict[str, Any]]) -> M:
+def _as_model(mod: type[M], value: M | dict[str, Any]) -> M:
     if isinstance(value, dict):
         return construct(mod, **value, _strict_validation=False)
     return value
```

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/__init__.py` & `scitacean-24.5.0/src/scitacean/_html_repr/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/_attachment_html.py` & `scitacean-24.5.0/src/scitacean/_html_repr/_attachment_html.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/_common_html.py` & `scitacean-24.5.0/src/scitacean/_html_repr/_common_html.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Common functions for HTML reprs."""
 
 import html
+from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 
-from .._internal.dataclass_wrapper import dataclass_optional_args
 from ..filesystem import RemotePath
 from ..model import History, Lifecycle, Relationship, Technique
 from ..pid import PID
 from . import _resources
 
 
-@dataclass_optional_args(kw_only=True, frozen=True, slots=True)
+@dataclass(kw_only=True, frozen=True, slots=True)
 class Field:
     name: str
     value: Any
     type: type
     description: str
     read_only: bool
     required: bool
```

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/_dataset_html.py` & `scitacean-24.5.0/src/scitacean/_html_repr/_dataset_html.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/_resources.py` & `scitacean-24.5.0/src/scitacean/_html_repr/_resources.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/images/lock.svg` & `scitacean-24.5.0/src/scitacean/_html_repr/images/lock.svg`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/styles/attachment.css` & `scitacean-24.5.0/src/scitacean/_html_repr/styles/attachment.css`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/styles/common.css` & `scitacean-24.5.0/src/scitacean/_html_repr/styles/common.css`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/styles/dataset.css` & `scitacean-24.5.0/src/scitacean/_html_repr/styles/dataset.css`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/templates/attachment_repr.html.template` & `scitacean-24.5.0/src/scitacean/_html_repr/templates/attachment_repr.html.template`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_html_repr/templates/dataset_repr.html.template` & `scitacean-24.5.0/src/scitacean/_html_repr/templates/dataset_repr.html.template`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_internal/docker.py` & `scitacean-24.5.0/src/scitacean/_internal/docker.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_internal/file_counter.py` & `scitacean-24.5.0/src/scitacean/_internal/file_counter.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_internal/jwt.py` & `scitacean-24.5.0/src/scitacean/_internal/jwt.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/_internal/orcid.py` & `scitacean-24.5.0/src/scitacean/_internal/orcid.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/client.py` & `scitacean-24.5.0/src/scitacean/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 # Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Client to handle communication with SciCat servers."""
 
 from __future__ import annotations
 
 import dataclasses
 import datetime
+import json
 import re
 import warnings
 from collections.abc import Callable, Iterable, Iterator
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Any
 from urllib.parse import quote_plus
 
-import requests
+import httpx
+import pydantic
 
 from . import model
 from ._base_model import convert_download_to_user_model
 from .dataset import Dataset
 from .error import ScicatCommError, ScicatLoginError
 from .file import File
 from .filesystem import RemotePath
@@ -287,15 +289,16 @@
                 )
             except ScicatCommError:
                 con.revert_upload(*uploaded_files)
                 raise
 
         with_new_pid = dataset.replace(_read_only={"pid": finalized_model.pid})
         finalized_orig_datablocks = self._upload_orig_datablocks(
-            with_new_pid.make_datablock_upload_models().orig_datablocks
+            with_new_pid.make_datablock_upload_models().orig_datablocks,
+            with_new_pid.pid,  # type: ignore[arg-type]
         )
         finalized_attachments = self._upload_attachments_for_dataset(
             with_new_pid.make_attachment_upload_models(),
             dataset_id=with_new_pid.pid,  # type: ignore[arg-type]
         )
 
         return Dataset.from_download_models(
@@ -329,28 +332,30 @@
             If the upload to SciCat fails.
         """
         sample = dataclasses.replace(sample, sample_id=None)
         finalized_model = self.scicat.create_sample_model(sample.make_upload_model())
         return model.Sample.from_download_model(finalized_model)
 
     def _upload_orig_datablocks(
-        self, orig_datablocks: list[model.UploadOrigDatablock] | None
+        self,
+        orig_datablocks: list[model.UploadOrigDatablock] | None,
+        dataset_id: PID,
     ) -> list[model.DownloadOrigDatablock]:
         if not orig_datablocks:
             return []
 
         try:
             return [
-                self.scicat.create_orig_datablock(orig_datablock)
+                self.scicat.create_orig_datablock(orig_datablock, dataset_id=dataset_id)
                 for orig_datablock in orig_datablocks
             ]
         except ScicatCommError as exc:
             raise RuntimeError(
                 "Failed to upload original datablocks for SciCat dataset "
-                f"{orig_datablocks[0].datasetId}:"
+                f"{dataset_id}:"
                 f"\n{exc.args}\nThe dataset and data files were successfully uploaded "
                 "but are not linked with each other. Please fix the dataset manually!"
             ) from exc
 
     def _upload_attachments_for_dataset(
         self, attachments: list[model.UploadAttachment], *, dataset_id: PID
     ) -> list[model.DownloadAttachment]:
@@ -701,14 +706,120 @@
             )
         return model.construct(
             model.DownloadDataset,
             _strict_validation=strict_validation,
             **dset_json,
         )
 
+    def query_datasets(
+        self,
+        fields: dict[str, Any],
+        *,
+        limit: int | None = None,
+        order: str | None = None,
+        strict_validation: bool = False,
+    ) -> list[model.DownloadDataset]:
+        """Query for datasets in SciCat.
+
+        Attention
+        ---------
+        This function is experimental and may change or be removed in the future.
+        It is currently unclear how best to implement querying because SciCat
+        provides multiple, very different APIs and there are plans for supporting
+        queries via Mongo query language directly.
+
+        See `issue #177 <https://github.com/SciCatProject/scitacean/issues/177>`_
+        for a discussion.
+
+        Parameters
+        ----------
+        fields:
+            Fields to query for.
+            Returned datasets must match all fields exactly.
+            See examples below.
+        limit:
+            Maximum number of results to return.
+            Requires ``order`` to be specified.
+            If not given, all matching datasets are returned.
+        order:
+            Specify order of results.
+            For example, ``"creationTime:asc"`` and ``"creationTime:desc"`` return
+            results in ascending or descending order in creation time, respectively.
+        strict_validation:
+            If ``True``, the datasets must pass validation.
+            If ``False``, datasets are still returned if validation fails.
+            Note that some dataset fields may have a bad value or type.
+            A warning will be logged if validation fails.
+
+        Returns
+        -------
+        :
+            A list of dataset models that match the query.
+
+        Examples
+        --------
+        Get all datasets belonging to proposal ``abc.123``:
+
+        .. code-block:: python
+
+            scicat_client.query_datasets({'proposalId': 'abc.123'})
+
+        Get all datasets that belong to proposal ``abc.123``
+        **and** have name ``"ds name"``: (The name and proposal must match exactly.)
+
+        .. code-block:: python
+
+            scicat_client.query_datasets({
+                'proposalId': 'abc.123',
+                'datasetName': 'ds name'
+            })
+
+        Return only the newest 5 datasets for proposal ``bc.123``:
+
+        .. code-block:: python
+
+            scicat_client.query_datasets(
+                {'proposalId': 'bc.123'},
+                limit=5,
+                order="creationTime:desc",
+            )
+        """
+        # Use a pydantic model to support serializing custom types to JSON.
+        params_model = pydantic.create_model(  # type: ignore[call-overload]
+            "QueryParams", **{key: (type(field), ...) for key, field in fields.items()}
+        )
+        params = {"fields": params_model(**fields).model_dump_json()}
+
+        limits: dict[str, str | int] = {}
+        if order is not None:
+            limits["order"] = order
+        if limit is not None:
+            if order is None:
+                raise ValueError("`order` is required when `limit` is specified.")
+            limits["limit"] = limit
+        if limits:
+            params["limits"] = json.dumps(limits)
+
+        dsets_json = self._call_endpoint(
+            cmd="get",
+            url="datasets/fullquery",
+            params=params,
+            operation="query_datasets",
+        )
+        if not dsets_json:
+            return []
+        return [
+            model.construct(
+                model.DownloadDataset,
+                _strict_validation=strict_validation,
+                **dset_json,
+            )
+            for dset_json in dsets_json
+        ]
+
     def get_orig_datablocks(
         self, pid: PID, strict_validation: bool = False
     ) -> list[model.DownloadOrigDatablock]:
         """Fetch all orig datablocks from SciCat for a given dataset.
 
         Parameters
         ----------
@@ -858,15 +969,18 @@
             cmd="post", url="datasets", data=dset, operation="create_dataset_model"
         )
         return model.construct(
             model.DownloadDataset, _strict_validation=False, **uploaded
         )
 
     def create_orig_datablock(
-        self, dblock: model.UploadOrigDatablock
+        self,
+        dblock: model.UploadOrigDatablock,
+        *,
+        dataset_id: PID,
     ) -> model.DownloadOrigDatablock:
         """Create a new orig datablock in SciCat.
 
         The datablock PID must be either
 
         - ``None``, in which case SciCat assigns an ID.
         - An unused id, in which case SciCat uses it for the new datablock.
@@ -874,24 +988,26 @@
         If the ID already exists, creation will fail without
         modification to the database.
 
         Parameters
         ----------
         dblock:
             Model of the orig datablock to create.
+        dataset_id:
+            PID of the dataset that this datablock belongs to.
 
         Raises
         ------
         scitacean.ScicatCommError
             If SciCat refuses the datablock or communication
             fails for some other reason.
         """
         uploaded = self._call_endpoint(
             cmd="post",
-            url="origdatablocks",
+            url=f"datasets/{quote_plus(str(dataset_id))}/origdatablocks",
             data=dblock,
             operation="create_orig_datablock",
         )
         return model.construct(
             model.DownloadOrigDatablock, _strict_validation=False, **uploaded
         )
 
@@ -998,37 +1114,41 @@
             data=dset,
             operation="validate_dataset_model",
         )
         if not response["valid"]:
             raise ValueError(f"Dataset {dset} did not pass validation in SciCat.")
 
     def _send_to_scicat(
-        self, *, cmd: str, url: str, data: model.BaseModel | None = None
-    ) -> requests.Response:
+        self,
+        *,
+        cmd: str,
+        url: str,
+        data: model.BaseModel | None = None,
+        params: dict[str, str] | None = None,
+    ) -> httpx.Response:
         if self._token is not None:
             token = self._token.get_str()
             headers = {"Authorization": f"Bearer {token}"}
         else:
             token = ""
             headers = {}
 
         if data is not None:
             headers["Content-Type"] = "application/json"
 
         try:
-            return requests.request(
+            return httpx.request(
                 method=cmd,
                 url=url,
-                data=data.model_dump_json(exclude_none=True)
+                content=data.model_dump_json(exclude_none=True)
                 if data is not None
                 else None,
+                params=params,
                 headers=headers,
                 timeout=self._timeout.seconds,
-                stream=False,
-                verify=True,
             )
         except Exception as exc:
             # Remove concrete request function call from backtrace to hide the token.
             # Also modify the error message to strip out the token.
             # It shows up, e.g. in urllib3.exceptions.NewConnectionError.
             # This turns the exception args into strings.
             # But we have little use of more structured errors, so that should be fine.
@@ -1037,33 +1157,34 @@
             ) from None
 
     def _call_endpoint(
         self,
         *,
         cmd: str,
         url: str,
-        data: model.BaseModel | None = None,
         operation: str,
+        data: model.BaseModel | None = None,
+        params: dict[str, str] | None = None,
     ) -> Any:
         full_url = _url_concat(self._base_url, url)
         logger = get_logger()
         logger.info("Calling SciCat API at %s for operation '%s'", full_url, operation)
 
-        response = self._send_to_scicat(cmd=cmd, url=full_url, data=data)
-        if not response.ok:
+        response = self._send_to_scicat(cmd=cmd, url=full_url, data=data, params=params)
+        if not response.is_success:
             logger.error(
                 "SciCat API call to %s failed: %s %s: %s",
                 full_url,
                 response.status_code,
-                response.reason,
+                response.reason_phrase,
                 response.text,
             )
             raise ScicatCommError(
                 f"Error in operation '{operation}': {response.status_code} "
-                f"{response.reason}: {response.text}"
+                f"{response.reason_phrase}: {response.text}"
             )
         logger.info("API call successful for operation '%s'", operation)
 
         return None if not response.text else response.json()
 
 
 def _url_concat(a: str, b: str) -> str:
@@ -1096,46 +1217,42 @@
         _strict_validation=strict_validation,
         **{**fields, "dataFileList": files},
     )
 
 
 def _log_in_via_users_login(
     url: str, username: StrStorage, password: StrStorage, timeout: datetime.timedelta
-) -> requests.Response:
+) -> httpx.Response:
     # Currently only used for functional accounts.
-    response = requests.post(
+    response = httpx.post(
         _url_concat(url, "Users/login"),
         json={"username": username.get_str(), "password": password.get_str()},
-        stream=False,
-        verify=True,
         timeout=timeout.seconds,
     )
-    if not response.ok:
+    if not response.is_success:
         get_logger().info(
             "Failed to log in via endpoint Users/login: %s", response.text
         )
     return response
 
 
 def _log_in_via_auth_msad(
     url: str, username: StrStorage, password: StrStorage, timeout: datetime.timedelta
-) -> requests.Response:
+) -> httpx.Response:
     # Used for user accounts.
     import re
 
     # Strip the api/vn suffix
     base_url = re.sub(r"/api/v\d+/?", "", url)
-    response = requests.post(
+    response = httpx.post(
         _url_concat(base_url, "auth/msad"),
         json={"username": username.get_str(), "password": password.get_str()},
-        stream=False,
-        verify=True,
         timeout=timeout.seconds,
     )
-    if not response.ok:
+    if not response.is_success:
         get_logger().error("Failed to log in via auth/msad: %s", response.text)
     return response
 
 
 def _get_token(
     url: str, username: StrStorage, password: StrStorage, timeout: datetime.timedelta
 ) -> str:
@@ -1147,21 +1264,21 @@
     # Try both and see what works. This is not nice but seems to be the only
     # feasible solution right now.
     get_logger().info("Logging in to %s", url)
 
     response = _log_in_via_users_login(
         url=url, username=username, password=password, timeout=timeout
     )
-    if response.ok:
+    if response.is_success:
         return str(response.json()["id"])  # not sure if semantically correct
 
     response = _log_in_via_auth_msad(
         url=url, username=username, password=password, timeout=timeout
     )
-    if response.ok:
+    if response.is_success:
         return str(response.json()["access_token"])
 
     get_logger().error("Failed log in:  %s", response.text)
     raise ScicatLoginError(response.content)
 
 
 FileSelector = (
```

### Comparing `scitacean-24.4.0/src/scitacean/datablock.py` & `scitacean-24.5.0/src/scitacean/datablock.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,17 @@
 """Wrappers for (Orig)Datablocks."""
 
 from __future__ import annotations
 
 import dataclasses
 from collections.abc import Iterable, Iterator
 from datetime import datetime
-from typing import TYPE_CHECKING
 
 from .file import File
 from .model import DownloadOrigDatablock, UploadOrigDatablock
-from .pid import PID
-
-if TYPE_CHECKING:
-    from .dataset import Dataset
 
 # TODO Datablock
 
 
 @dataclasses.dataclass
 class OrigDatablock:
     """Dataclass for an orig datablock.
@@ -28,21 +23,18 @@
     :class:`scitacean.model.OrigDatablock`.
     They are used for building datasets and get converted to/from pydantic
     models for communication with a server.
     """
 
     _files: list[File] = dataclasses.field(init=False)
     checksum_algorithm: str | None = None
-    instrument_group: str | None = None
-    owner_group: str | None = None
     init_files: dataclasses.InitVar[Iterable[File] | None] = None
     _access_groups: list[str] | None = None
     _created_at: datetime | None = None
     _created_by: str | None = None
-    _dataset_id: PID | None = None
     _id: str | None = None
     _is_published: bool | None = None
     _updated_at: datetime | None = None
     _updated_by: str | None = None
 
     def __post_init__(self, init_files: Iterable[File] | None) -> None:
         self._files = list(init_files) if init_files is not None else []
@@ -63,20 +55,17 @@
         -------
         :
             A new instance.
         """
         dblock = orig_datablock_model
         return OrigDatablock(
             checksum_algorithm=dblock.chkAlg,
-            owner_group=dblock.ownerGroup,
-            instrument_group=dblock.instrumentGroup,
             _access_groups=dblock.accessGroups,
             _created_at=dblock.createdAt,
             _created_by=dblock.createdBy,
-            _dataset_id=orig_datablock_model.datasetId,
             _id=orig_datablock_model.id,
             _is_published=orig_datablock_model.isPublished,
             _updated_at=dblock.updatedAt,
             _updated_by=dblock.updatedBy,
             init_files=[
                 File.from_download_model(file, checksum_algorithm=dblock.chkAlg)
                 for file in dblock.dataFileList or ()
@@ -115,19 +104,14 @@
 
     @property
     def updated_by(self) -> str | None:
         """User who last updated this datablock."""
         return self._updated_by
 
     @property
-    def dataset_id(self) -> PID | None:
-        """PID of the dataset this datablock belongs to."""
-        return self._dataset_id
-
-    @property
     def datablock_id(self) -> str | None:
         """ID of this datablock."""
         return self._id
 
     @property
     def is_published(self) -> bool | None:
         """Return whether the datablock is public on SciCat."""
@@ -142,30 +126,20 @@
             File objects to add.
         """
         self._files.extend(
             dataclasses.replace(f, checksum_algorithm=self.checksum_algorithm)
             for f in files
         )
 
-    def make_upload_model(self, dataset: Dataset) -> UploadOrigDatablock:
+    def make_upload_model(self) -> UploadOrigDatablock:
         """Build a new pydantic model to upload this datablock.
 
-        Parameters
-        ----------
-        dataset:
-            The dataset that this orig datablock belongs to.
-
         Returns
         -------
         :
             A new model for this orig datablock.
         """
-        owner_group = self.owner_group or dataset.owner_group
         return UploadOrigDatablock(
             chkAlg=self.checksum_algorithm,
             size=self.size,
             dataFileList=[file.make_model(for_archive=False) for file in self.files],
-            datasetId=dataset.pid,  # type: ignore[arg-type]
-            ownerGroup=owner_group,
-            accessGroups=self.access_groups or dataset.access_groups,
-            instrumentGroup=self.instrument_group or dataset.instrument_group,
         )
```

### Comparing `scitacean-24.4.0/src/scitacean/dataset.py` & `scitacean-24.5.0/src/scitacean/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
 
         Returns
         -------
         :
             The newly added datablock.
         """
         dblock = OrigDatablock(
-            checksum_algorithm=checksum_algorithm, _dataset_id=self.pid
+            checksum_algorithm=checksum_algorithm,
         )
         self._orig_datablocks.append(dblock)
         return dblock
 
     def _lookup_orig_datablock(self, id_: str) -> OrigDatablock:
         try:
             return next(db for db in self._orig_datablocks if db.datablock_id == id_)
@@ -428,15 +428,15 @@
             return self.add_orig_datablock(
                 checksum_algorithm=self._default_checksum_algorithm
             )
         return self._orig_datablocks[key]
 
     def make_upload_model(self) -> UploadDerivedDataset | UploadRawDataset:
         """Construct a SciCat upload model from self."""
-        model: type[UploadRawDataset] | type[UploadDerivedDataset] = (
+        model: type[UploadRawDataset | UploadDerivedDataset] = (
             UploadRawDataset if self.type == DatasetType.RAW else UploadDerivedDataset
         )
         # Datablocks are not included here because they are handled separately
         # by make_datablock_upload_models and their own endpoints.
         special = ("relationships", "techniques")
         return model(
             numberOfFiles=self.number_of_files,
@@ -466,15 +466,15 @@
         :
             Structure with datablock and orig datablock models.
         """
         if self.number_of_files == 0:
             return DatablockUploadModels(orig_datablocks=None)
         return DatablockUploadModels(
             orig_datablocks=[
-                dblock.make_upload_model(self) for dblock in self._orig_datablocks
+                dblock.make_upload_model() for dblock in self._orig_datablocks
             ]
         )
 
     def make_attachment_upload_models(self) -> list[UploadAttachment]:
         """Build models for all registered attachments.
 
         Raises
@@ -513,16 +513,16 @@
             and other fields that are not ``None``.
 
 
         .. versionadded:: 23.10.0
         """
         from itertools import chain
 
-        all_fields = set(field.name for field in self.fields())
-        my_fields = set(field.name for field in self.fields(dataset_type=self.type))
+        all_fields = {field.name for field in self.fields()}
+        my_fields = {field.name for field in self.fields(dataset_type=self.type)}
         other_fields = all_fields - my_fields
         invalid_fields = (
             f_name for f_name in other_fields if getattr(self, f_name) is not None
         )
 
         return chain(my_fields, invalid_fields)
```

### Comparing `scitacean-24.4.0/src/scitacean/file.py` & `scitacean-24.5.0/src/scitacean/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,21 +375,21 @@
         Returns
         -------
         :
             A new file object.
         """
         if remote_creation_time is None:
             remote_creation_time = datetime.now().astimezone(timezone.utc)
-        args = dict(
-            remote_path=RemotePath(remote_path) if remote_path is not None else None,
-            remote_gid=remote_gid,
-            remote_uid=remote_uid,
-            remote_perm=remote_perm,
-            _remote_creation_time=remote_creation_time,
-        )
+        args = {
+            "remote_path": RemotePath(remote_path) if remote_path is not None else None,
+            "remote_gid": remote_gid,
+            "remote_uid": remote_uid,
+            "remote_perm": remote_perm,
+            "_remote_creation_time": remote_creation_time,
+        }
         return dataclasses.replace(
             self,
             _remote_size=remote_size if remote_size is not None else self.size,
             _remote_checksum=self.checksum(),
             **{key: val for key, val in args.items() if val is not None},  # type: ignore[arg-type]
         )
```

### Comparing `scitacean-24.4.0/src/scitacean/filesystem.py` & `scitacean-24.5.0/src/scitacean/filesystem.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/logging.py` & `scitacean-24.5.0/src/scitacean/logging.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/model.py` & `scitacean-24.5.0/src/scitacean/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,38 +76,37 @@
    :toctree: ../functions
 
    construct
 """
 
 from __future__ import annotations
 
+from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 
 import pydantic
 from pydantic import NonNegativeInt
 
 from ._base_model import (
     BaseModel,
     BaseUserModel,
     DatasetType,
     construct,
     validate_datetime,
-    validate_drop,
     validate_emails,
     validate_orcids,
 )
-from ._internal.dataclass_wrapper import dataclass_optional_args
 from .filesystem import RemotePath
 from .pid import PID
 from .thumbnail import Thumbnail
 
 
 class DownloadDataset(
-    BaseModel, masked=("attachments", "datablocks", "origdatablocks")
+    BaseModel, masked=("attachments", "datablocks", "history", "origdatablocks")
 ):
     contactEmail: str | None = None
     creationLocation: str | None = None
     creationTime: datetime | None = None
     inputDatasets: list[PID] | None = None
     investigator: str | None = None
     numberOfFilesArchived: NonNegativeInt | None = None
@@ -123,15 +122,14 @@
     comment: str | None = None
     createdAt: datetime | None = None
     createdBy: str | None = None
     dataFormat: str | None = None
     dataQualityMetrics: int | None = None
     description: str | None = None
     endTime: datetime | None = None
-    history: None = None
     instrumentGroup: str | None = None
     instrumentId: str | None = None
     isPublished: bool | None = None
     jobLogData: str | None = None
     jobParameters: dict[str, Any] | None = None
     keywords: list[str] | None = None
     license: str | None = None
@@ -156,18 +154,14 @@
 
     @pydantic.field_validator(
         "creationTime", "createdAt", "endTime", "updatedAt", mode="before"
     )
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
-    @pydantic.field_validator("history", mode="before")
-    def _validate_drop(cls, value: Any) -> Any:
-        return validate_drop(value)
-
     @pydantic.field_validator("contactEmail", "ownerEmail", mode="before")
     def _validate_emails(cls, value: Any) -> Any:
         return validate_emails(value)
 
     @pydantic.field_validator("orcidOfOwner", mode="before")
     def _validate_orcids(cls, value: Any) -> Any:
         return validate_orcids(value)
@@ -342,20 +336,16 @@
     @classmethod
     def upload_model_type(cls) -> type[UploadOrigDatablock]:
         return UploadOrigDatablock
 
 
 class UploadOrigDatablock(BaseModel):
     dataFileList: list[UploadDataFile]
-    datasetId: PID
     size: NonNegativeInt
-    accessGroups: list[str] | None = None
     chkAlg: str | None = None
-    instrumentGroup: str | None = None
-    ownerGroup: str | None = None
 
     @classmethod
     def download_model_type(cls) -> type[DownloadOrigDatablock]:
         return DownloadOrigDatablock
 
 
 class DownloadDatablock(BaseModel):
@@ -584,15 +574,15 @@
         return Sample
 
     @classmethod
     def download_model_type(cls) -> type[DownloadSample]:
         return DownloadSample
 
 
-@dataclass_optional_args(kw_only=True, slots=True)
+@dataclass(kw_only=True, slots=True)
 class Attachment(BaseUserModel):
     caption: str
     owner_group: str
     access_groups: list[str] | None = None
     dataset_id: PID | None = None
     id: str | None = None
     instrument_group: str | None = None
@@ -639,15 +629,15 @@
         return UploadAttachment
 
     @classmethod
     def download_model_type(cls) -> type[DownloadAttachment]:
         return DownloadAttachment
 
 
-@dataclass_optional_args(kw_only=True, slots=True)
+@dataclass(kw_only=True, slots=True)
 class Lifecycle(BaseUserModel):
     _archivable: bool | None = None
     _archive_retention_time: datetime | None = None
     _archive_return_message: dict[str, Any] | None = None
     _archive_status_message: str | None = None
     _date_of_disk_purging: datetime | None = None
     _date_of_publishing: datetime | None = None
@@ -722,15 +712,15 @@
         return cls(**cls._download_model_dict(download_model))
 
     @classmethod
     def download_model_type(cls) -> type[DownloadLifecycle]:
         return DownloadLifecycle
 
 
-@dataclass_optional_args(kw_only=True, slots=True)
+@dataclass(kw_only=True, slots=True)
 class Technique(BaseUserModel):
     name: str
     pid: str
 
     @classmethod
     def from_download_model(cls, download_model: DownloadTechnique) -> Technique:
         """Construct an instance from an associated SciCat download model."""
@@ -745,15 +735,15 @@
         return UploadTechnique
 
     @classmethod
     def download_model_type(cls) -> type[DownloadTechnique]:
         return DownloadTechnique
 
 
-@dataclass_optional_args(kw_only=True, slots=True)
+@dataclass(kw_only=True, slots=True)
 class Relationship(BaseUserModel):
     pid: PID
     relationship: str
 
     @classmethod
     def from_download_model(cls, download_model: DownloadRelationship) -> Relationship:
         """Construct an instance from an associated SciCat download model."""
@@ -768,15 +758,15 @@
         return UploadRelationship
 
     @classmethod
     def download_model_type(cls) -> type[DownloadRelationship]:
         return DownloadRelationship
 
 
-@dataclass_optional_args(kw_only=True, slots=True)
+@dataclass(kw_only=True, slots=True)
 class History(BaseUserModel):
     __id: str | None = None
     _updated_at: datetime | None = None
     _updated_by: datetime | None = None
 
     @property
     def _id(self) -> str | None:
@@ -796,15 +786,15 @@
         return cls(**cls._download_model_dict(download_model))
 
     @classmethod
     def download_model_type(cls) -> type[DownloadHistory]:
         return DownloadHistory
 
 
-@dataclass_optional_args(kw_only=True, slots=True)
+@dataclass(kw_only=True, slots=True)
 class Instrument(BaseUserModel):
     _custom_metadata: dict[str, Any] | None = None
     _name: str | None = None
     _pid: str | None = None
     _unique_name: str | None = None
 
     @property
@@ -829,15 +819,15 @@
         return cls(**cls._download_model_dict(download_model))
 
     @classmethod
     def download_model_type(cls) -> type[DownloadInstrument]:
         return DownloadInstrument
 
 
-@dataclass_optional_args(kw_only=True, slots=True)
+@dataclass(kw_only=True, slots=True)
 class Sample(BaseUserModel):
     owner_group: str
     access_groups: list[str] | None = None
     description: str | None = None
     instrument_group: str | None = None
     is_published: bool | None = None
     owner: str | None = None
```

### Comparing `scitacean-24.4.0/src/scitacean/pid.py` & `scitacean-24.5.0/src/scitacean/pid.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/_pytest_helpers.py` & `scitacean-24.5.0/src/scitacean/testing/_pytest_helpers.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/backend/__init__.py` & `scitacean-24.5.0/src/scitacean/testing/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/backend/_backend.py` & `scitacean-24.5.0/src/scitacean/testing/backend/_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import time
 from copy import deepcopy
 from pathlib import Path
 from typing import Any
 from urllib.parse import urljoin
 
-import requests
+import httpx
 import yaml
 
 from ..._internal.docker import docker_compose_down, docker_compose_up
 from . import config
 
 _PathLike = str | os.PathLike[str]
 
@@ -85,22 +85,22 @@
     -------
     :
         The first element indicates whether the connection was successful.
         The second element is an error message.
     """
     scicat_access = config.local_access("user1")
     try:
-        response = requests.post(
+        response = httpx.post(
             urljoin(scicat_access.url, "Users/login"),
             json=scicat_access.user.credentials,
             timeout=0.5,
         )
-    except requests.ConnectionError as err:
+    except (httpx.NetworkError, httpx.TransportError) as err:
         return False, str(err)
-    if response.ok:
+    if response.is_success:
         return True, ""
     return False, str(f"{response}: {response.text}")
 
 
 def wait_until_backend_is_live(max_time: float, n_tries: int) -> None:
     """Sleep until a connection to the backend can be made.
```

### Comparing `scitacean-24.4.0/src/scitacean/testing/backend/_pytest_helpers.py` & `scitacean-24.5.0/src/scitacean/testing/backend/_pytest_helpers.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/backend/config.py` & `scitacean-24.5.0/src/scitacean/testing/backend/config.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/backend/docker-compose-backend-template.yaml` & `scitacean-24.5.0/src/scitacean/testing/backend/docker-compose-backend-template.yaml`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/backend/fixtures.py` & `scitacean-24.5.0/src/scitacean/testing/backend/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     if request.param == "fake":
         return request.getfixturevalue("fake_client")  # type: ignore[no-any-return]
     skip_if_not_backend(request)
     return request.getfixturevalue("real_client")  # type: ignore[no-any-return]
 
 
 @pytest.fixture()
-def require_scicat_backend(request, scicat_backend) -> None:
+def require_scicat_backend(request, scicat_backend) -> None:  # noqa: PT004
     """Fixture to declare that a test needs a local scicat backend.
 
     Like :func:`scitacean.testing.backend.scicat_backend`
     but this skips the test if backend tests are disabled.
     """
     skip_if_not_backend(request)
```

### Comparing `scitacean-24.4.0/src/scitacean/testing/backend/seed.py` & `scitacean-24.5.0/src/scitacean/testing/backend/seed.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,19 +39,17 @@
         accessGroups=["uu", "faculty"],
         classification="IN=medium,AV=low,CO=low",
         contactEmail="ponder.stibbons@uu.am",
         creationTime=parse_datetime("2004-06-13T01:45:28.100Z"),
         datasetName="My darkest magic yet",
         description="Doing some dark shit",
         isPublished=False,
-        numberOfFiles=2,
         numberOfFilesArchived=0,
         owner="PLACEHOLDER",
         ownerEmail="PLACE@HOLD.ER",
-        size=619,
         sourceFolder=RemotePath("/hex/data/123"),
         type=DatasetType.RAW,
         principalInvestigator="Ponder Stibbons",
         creationLocation=SITE,
         techniques=[UploadTechnique(pid="DM666", name="dark_magic")],
         scientificMetadata={
             "data_type": "event data",
@@ -64,19 +62,17 @@
         accessGroups=["uu", "faculty"],
         classification="IN=medium,AV=low,CO=low",
         contactEmail="ponder.stibbons@uu.am",
         creationTime=parse_datetime("2005-11-04T13:37:44.002Z"),
         datasetName="Reprocessed dark magic",
         description="Making it even darker",
         isPublished=True,
-        numberOfFiles=1,
         numberOfFilesArchived=0,
         owner="PLACEHOLDER",
         ownerEmail="PLACE@HOLD.ER",
-        size=464,
         sourceFolder=RemotePath("/hex/data/dd"),
         type=DatasetType.DERIVED,
         investigator="Ponder Stibbons",
         inputDatasets=[],
         usedSoftware=["scitacean"],
         scientificMetadata={
             "data_type": "reduced",
@@ -88,19 +84,17 @@
         accessGroups=["uu"],
         classification="IN=medium,AV=low,CO=low",
         contactEmail="mustrum.ridcully69@uu.am",
         creationTime=parse_datetime("1998-11-05T23:00:42.000Z"),
         datasetName="Shoe counter",
         description="Got all these shoes!",
         isPublished=True,
-        numberOfFiles=1,
         numberOfFilesArchived=0,
         owner="PLACEHOLDER",
         ownerEmail="PLACE@HOLD.ER",
-        size=64,
         sourceFolder=RemotePath("/hex/secret/stuff"),
         type=DatasetType.RAW,
         principalInvestigator="Mustrum Ridcully",
         creationLocation=SITE,
         techniques=[UploadTechnique(pid="S", name="shoes")],
     ),
     "partially-broken": model.construct(
@@ -129,18 +123,15 @@
     ),
 }
 
 # Orig datablocks to upload to the database.
 _ORIG_DATABLOCKS: dict[str, list[UploadOrigDatablock]] = {
     "raw": [
         UploadOrigDatablock(
-            datasetId=PID(pid="PLACEHOLDER"),
-            ownerGroup="PLACEHOLDER",
             size=619,
-            accessGroups=["uu", "faculty"],
             chkAlg="md5",
             dataFileList=[
                 UploadDataFile(
                     path="file1.txt",
                     size=300,
                     time=parse_datetime("2005-11-04T13:22:09.000Z"),
                     chk="97157d347fe9af920f5e61e96cf401cb",
@@ -158,18 +149,15 @@
                     perm="777",
                 ),
             ],
         )
     ],
     "derived": [
         UploadOrigDatablock(
-            datasetId=PID(pid="PLACEHOLDER"),
-            ownerGroup="PLACEHOLDER",
             size=464,
-            accessGroups=["uu", "faculty"],
             chkAlg="sha256",
             dataFileList=[
                 UploadDataFile(
                     path="table.csv",
                     size=464,
                     time=parse_datetime("2005-10-31T00:00:01.000Z"),
                     chk="dddd8355da9105acabb9928196f022ca0581ffb73d8b89c891eb6f71477cb4cb",
@@ -178,18 +166,15 @@
                     perm="656",
                 ),
             ],
         )
     ],
     "public": [
         UploadOrigDatablock(
-            datasetId=PID(pid="PLACEHOLDER"),
-            ownerGroup="PLACEHOLDER",
             size=64,
-            accessGroups=["uu"],
             chkAlg="md5",
             dataFileList=[
                 UploadDataFile(
                     path="shoes",
                     size=64,
                     time=parse_datetime("1998-11-05T22:56:13.000Z"),
                     chk="95fe96bf90f6a53c1e20d6578e0d9e6e",
@@ -235,23 +220,14 @@
     dset = deepcopy(dset)
     dset.owner = user.username
     dset.ownerGroup = user.group
     dset.ownerEmail = user.email
     return dset
 
 
-def _apply_config_orig_datablock(
-    dblock: UploadOrigDatablock, dset: DownloadDataset, user: SciCatUser
-) -> UploadOrigDatablock:
-    dblock = deepcopy(dblock)
-    dblock.ownerGroup = user.group
-    dblock.datasetId = dset.pid  # type: ignore[assignment]
-    return dblock
-
-
 def _apply_config_attachment(
     attachment: UploadAttachment, user: SciCatUser
 ) -> UploadAttachment:
     attachment = deepcopy(attachment)
     attachment.ownerGroup = user.group
     return attachment
 
@@ -278,28 +254,32 @@
     }
     download_datasets = {
         key: _create_dataset_model(client, dset)
         for key, dset in upload_datasets.items()
     }
     INITIAL_DATASETS.update(download_datasets)
 
-    upload_orig_datablocks = {
+    download_orig_datablocks = {
         key: [
-            _apply_config_orig_datablock(
-                dblock, download_datasets[key], scicat_access.user
+            client.scicat.create_orig_datablock(
+                dblock,
+                dataset_id=download_datasets[key].pid,  # type: ignore[arg-type]
             )
             for dblock in dblocks
         ]
         for key, dblocks in _ORIG_DATABLOCKS.items()
     }
-    download_orig_datablocks = {
-        key: [client.scicat.create_orig_datablock(dblock) for dblock in dblocks]
-        for key, dblocks in upload_orig_datablocks.items()
-    }
     INITIAL_ORIG_DATABLOCKS.update(download_orig_datablocks)
+    for key, dblocks in INITIAL_ORIG_DATABLOCKS.items():
+        # Need to set these after uploading the datablocks to
+        # make sure that the database has the correct values.
+        INITIAL_DATASETS[key].numberOfFiles = sum(
+            len(dblock.dataFileList or ()) for dblock in dblocks
+        )
+        INITIAL_DATASETS[key].size = sum(dblock.size or 0 for dblock in dblocks)
 
     upload_attachments = {
         key: [
             _apply_config_attachment(attachment, scicat_access.user)
             for attachment in attachments
         ]
         for key, attachments in _ATTACHMENTS.items()
```

### Comparing `scitacean-24.4.0/src/scitacean/testing/client.py` & `scitacean-24.5.0/src/scitacean/testing/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,18 +232,17 @@
                 "because there already is a dataset with this pid."
             )
         self.main.datasets[pid] = ingested
         return ingested
 
     @_conditionally_disabled
     def create_orig_datablock(
-        self, dblock: model.UploadOrigDatablock
+        self, dblock: model.UploadOrigDatablock, *, dataset_id: PID
     ) -> model.DownloadOrigDatablock:
         """Create a new orig datablock in SciCat."""
-        dataset_id = dblock.datasetId
         if (dset := self.main.datasets.get(dataset_id)) is None:
             raise ScicatCommError(f"No dataset with id {dataset_id}")
         ingested = _process_orig_datablock(dblock, dset)
         self.main.orig_datablocks.setdefault(dataset_id, []).append(ingested)
         return ingested
 
     @_conditionally_disabled
@@ -353,14 +352,15 @@
     processed = model.construct(
         model.DownloadOrigDatablock,
         _strict_validation=False,
         createdBy="fake",
         createdAt=created_at,
         updatedBy="fake",
         updatedAt=created_at,
+        datasetId=dset.pid,
         **fields,
     )
     return processed
 
 
 def _process_attachment(
     attachment: model.UploadAttachment, dataset_id: PID | None = None
```

### Comparing `scitacean-24.4.0/src/scitacean/testing/docs.py` & `scitacean-24.5.0/src/scitacean/testing/docs.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/sftp/__init__.py` & `scitacean-24.5.0/src/scitacean/testing/sftp/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/sftp/_pytest_helpers.py` & `scitacean-24.5.0/src/scitacean/testing/sftp/_pytest_helpers.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/sftp/_sftp.py` & `scitacean-24.5.0/src/scitacean/testing/sftp/_sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         .iterdir()
     )
 
 
 def local_access() -> SFTPAccess:
     config = _docker_compose_file()
     service = config["services"]["scitacean-test-sftp-server"]
-    env = {k: v for k, v in map(lambda s: s.split("="), service["environment"])}
+    env = dict(map(lambda s: s.split("="), service["environment"]))
     return SFTPAccess(
         host="localhost",
         port=service["ports"][0].split(":")[0],
         user=SFTPUser(
             username=env["USER_NAME"],
             password=env["USER_PASSWORD"],
         ),
```

### Comparing `scitacean-24.4.0/src/scitacean/testing/sftp/docker-compose-sftp-server.yaml` & `scitacean-24.5.0/src/scitacean/testing/sftp/docker-compose-sftp-server.yaml`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/sftp/fixtures.py` & `scitacean-24.5.0/src/scitacean/testing/sftp/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     """
     if sftp_base_dir is None:
         return None
     return sftp_base_dir / "data"
 
 
 @pytest.fixture()
-def require_sftp_fileserver(request, sftp_fileserver) -> None:
+def require_sftp_fileserver(request, sftp_fileserver) -> None:  # noqa: PT004
     """Fixture to declare that a test needs a local SFTP server.
 
     Like :func:`scitacean.testing.sftp.sftp_fileserver`
     but this skips the test if SFTP tests are disabled.
     """
     skip_if_not_sftp(request)
```

### Comparing `scitacean-24.4.0/src/scitacean/testing/strategies.py` & `scitacean-24.5.0/src/scitacean/testing/strategies.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/testing/transfer.py` & `scitacean-24.5.0/src/scitacean/testing/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             self.fs.create_file(local, contents=self.files[remote])
         else:
             with open(local, "wb") as f:
                 f.write(self.files[remote])
 
     def download_files(self, *, remote: list[RemotePath], local: list[Path]) -> None:
         """Download multiple files."""
-        for r, l in zip(remote, local):
+        for r, l in zip(remote, local, strict=True):
             self.download_file(remote=r, local=l)
 
 
 class FakeUploadConnection:
     """'Upload' files to a fake file transfer."""
 
     def __init__(
```

### Comparing `scitacean-24.4.0/src/scitacean/thumbnail.py` & `scitacean-24.5.0/src/scitacean/thumbnail.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 from __future__ import annotations
 
 import base64
 import mimetypes
 import os
 import re
 from collections.abc import Callable
+from dataclasses import dataclass
 from typing import Any
 
 from pydantic import GetCoreSchemaHandler
 from pydantic_core import core_schema
 
-from ._internal.dataclass_wrapper import dataclass_optional_args
 
-
-@dataclass_optional_args(init=False, kw_only=True, slots=True)
+@dataclass(init=False, kw_only=True, slots=True)
 class Thumbnail:
     """Encodes an image to be used as a thumbnail in SciCat.
 
     Thumbnails are *small* images used, e.g., in attachments.
     In SciCat, they are base64-encoded strings and have a size limit.
 
     This class handles the encoding but does not enforce a size limit
```

### Comparing `scitacean-24.4.0/src/scitacean/transfer/link.py` & `scitacean-24.5.0/src/scitacean/transfer/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     Should be created using
     :meth:`scitacean.transfer.link.LinkFileTransfer.connect_for_download`.
     """
 
     def download_files(self, *, remote: list[RemotePath], local: list[Path]) -> None:
         """Download files from the given remote path."""
-        for r, l in zip(remote, local):
+        for r, l in zip(remote, local, strict=True):
             self.download_file(remote=r, local=l)
 
     def download_file(self, *, remote: RemotePath, local: Path) -> None:
         """Download a file from the given remote path."""
         get_logger().info(
             "Linking file %s to %s",
             remote,
```

### Comparing `scitacean-24.4.0/src/scitacean/transfer/sftp.py` & `scitacean-24.5.0/src/scitacean/transfer/sftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def __init__(self, *, sftp_client: SFTPClient, host: str) -> None:
         self._sftp_client = sftp_client
         self._host = host
 
     def download_files(self, *, remote: list[RemotePath], local: list[Path]) -> None:
         """Download files from the given remote path."""
-        for r, l in zip(remote, local):
+        for r, l in zip(remote, local, strict=True):
             self.download_file(remote=r, local=l)
 
     def download_file(self, *, remote: RemotePath, local: Path) -> None:
         """Download a file from the given remote path."""
         get_logger().info(
             "Downloading file %s from host %s to %s",
             remote,
```

### Comparing `scitacean-24.4.0/src/scitacean/transfer/util.py` & `scitacean-24.5.0/src/scitacean/transfer/util.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/typing.py` & `scitacean-24.5.0/src/scitacean/typing.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/util/credentials.py` & `scitacean-24.5.0/src/scitacean/util/credentials.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean/util/formatter.py` & `scitacean-24.5.0/src/scitacean/util/formatter.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/src/scitacean.egg-info/PKG-INFO` & `scitacean-24.5.0/src/scitacean.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitacean
-Version: 24.4.0
+Version: 24.5.0
 Summary: High-level interface for SciCat
 Author: Scitacean contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, SciCat Project
         All rights reserved.
         
@@ -48,24 +48,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: email-validator
+Requires-Dist: email-validator>=2
+Requires-Dist: httpx>=0.24
 Requires-Dist: pydantic>=2
-Requires-Dist: python-dateutil
-Requires-Dist: requests>=2.31
+Requires-Dist: python-dateutil>=2.8
 Provides-Extra: sftp
-Requires-Dist: paramiko; extra == "sftp"
+Requires-Dist: paramiko>=3; extra == "sftp"
 Provides-Extra: test
-Requires-Dist: filelock; extra == "test"
-Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: pyyaml; extra == "test"
+Requires-Dist: filelock>=3; extra == "test"
+Requires-Dist: hypothesis>=6.48; extra == "test"
+Requires-Dist: pyyaml>=5; extra == "test"
 
 [![PyPI badge](https://img.shields.io/pypi/v/scitacean.svg?style=flat-square&color=green)](https://pypi.python.org/pypi/scitacean)
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/scitacean?style=flat-square&color=green)](https://anaconda.org/conda-forge/scitacean)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7520487.svg)](https://doi.org/10.5281/zenodo.7520487)
 [![License: BSD 3-Clause](https://img.shields.io/github/license/SciCatProject/scitacean?style=flat-square&color=yellowgreen)](LICENSE)
 
 <picture>
```

### Comparing `scitacean-24.4.0/src/scitacean.egg-info/SOURCES.txt` & `scitacean-24.5.0/src/scitacean.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 src/scitacean/_html_repr/templates/attachment_field_repr.html.template
 src/scitacean/_html_repr/templates/attachment_repr.html.template
 src/scitacean/_html_repr/templates/dataset_field_repr.html.template
 src/scitacean/_html_repr/templates/dataset_repr.html.template
 src/scitacean/_html_repr/templates/files_repr.html.template
 src/scitacean/_html_repr/templates/metadata_repr.html.template
 src/scitacean/_internal/__init__.py
-src/scitacean/_internal/dataclass_wrapper.py
 src/scitacean/_internal/docker.py
 src/scitacean/_internal/file_counter.py
 src/scitacean/_internal/jwt.py
 src/scitacean/_internal/orcid.py
 src/scitacean/testing/__init__.py
 src/scitacean/testing/_pytest_helpers.py
 src/scitacean/testing/client.py
@@ -139,14 +138,15 @@
 tests/thumbnail_test.py
 tests/upload_test.py
 tests/client/__init__.py
 tests/client/attachment_client_test.py
 tests/client/client_test.py
 tests/client/datablock_client_test.py
 tests/client/dataset_client_test.py
+tests/client/query_client_test.py
 tests/client/sample_client_test.py
 tests/common/__init__.py
 tests/common/files.py
 tests/html_repr/__init__.py
 tests/html_repr/html_repr_test.py
 tests/testing/__init__.py
 tests/testing/strategies_test.py
```

### Comparing `scitacean-24.4.0/tests/client/attachment_client_test.py` & `scitacean-24.5.0/tests/client/attachment_client_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,34 +132,34 @@
 def test_get_attachments_for_dataset_no_attachments(scicat_client):
     assert INITIAL_ATTACHMENTS.get("raw") is None
     dset = INITIAL_DATASETS["raw"]
     attachments = scicat_client.get_attachments_for_dataset(dset.pid)
     assert attachments == []
 
 
-@pytest.mark.parametrize("key", ("raw", "derived"))
+@pytest.mark.parametrize("key", ["raw", "derived"])
 def test_get_dataset_does_not_initialise_attachments(client, key):
     dset = INITIAL_DATASETS["derived"]
     downloaded = client.get_dataset(dset.pid)
     assert downloaded.attachments is None
 
 
-@pytest.mark.parametrize("key", ("raw", "derived"))
+@pytest.mark.parametrize("key", ["raw", "derived"])
 def test_download_attachments_for_dataset(client, key):
     dset = INITIAL_DATASETS[key]
     downloaded = client.get_dataset(dset.pid)
     with_attachments = client.download_attachments_for(downloaded)
     expected = [
         Attachment.from_download_model(attachment)
         for attachment in INITIAL_ATTACHMENTS.get(key, ())
     ]
     assert with_attachments.attachments == expected
 
 
-@pytest.mark.parametrize("key", ("raw", "derived"))
+@pytest.mark.parametrize("key", ["raw", "derived"])
 def test_get_dataset_with_attachments(client, key):
     dset = INITIAL_DATASETS[key]
     downloaded = client.get_dataset(dset.pid, attachments=True)
     expected = [
         Attachment.from_download_model(attachment)
         for attachment in INITIAL_ATTACHMENTS.get(key, ())
     ]
```

### Comparing `scitacean-24.4.0/tests/client/client_test.py` & `scitacean-24.5.0/tests/client/client_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 def test_connection_error_does_not_contain_token():
     client = Client.from_token(
         url="https://not-actually-a_server",
         token="the token/which_must-be.kept secret",  # noqa: S106
     )
     try:
         client.get_dataset("does not exist")
-        assert False, "There must be an exception"  # noqa: B011
+        pytest.fail("There must be an exception")
     except Exception as exc:
-        assert "the token/which_must-be.kept secret" not in str(exc)
+        assert "the token/which_must-be.kept secret" not in str(exc)  # noqa: PT017
         for arg in exc.args:
             assert "the token/which_must-be.kept secret" not in str(arg)
 
 
 def test_fake_can_disable_functions():
     client = FakeClient(
         disable={
```

### Comparing `scitacean-24.4.0/tests/client/datablock_client_test.py` & `scitacean-24.5.0/tests/client/datablock_client_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,30 +46,27 @@
     return UploadOrigDatablock(
         size=9235,
         dataFileList=[
             UploadDataFile(
                 path="data.nxs", size=9235, time=parse_date("2023-08-18T13:52:33.000Z")
             )
         ],
-        datasetId="PLACEHOLDER",
-        ownerGroup=scicat_access.user.group,
     )
 
 
-@pytest.mark.parametrize("key", ("raw", "derived"))
+@pytest.mark.parametrize("key", ["raw", "derived"])
 def test_get_orig_datablock(scicat_client, key):
     dblock = INITIAL_ORIG_DATABLOCKS[key][0]
     downloaded = scicat_client.get_orig_datablocks(dblock.datasetId)
     assert downloaded == [dblock]
 
 
 def test_create_first_orig_datablock(scicat_client, derived_dataset, orig_datablock):
     uploaded = scicat_client.create_dataset_model(derived_dataset)
-    orig_datablock.datasetId = uploaded.pid
-    scicat_client.create_orig_datablock(orig_datablock)
+    scicat_client.create_orig_datablock(orig_datablock, dataset_id=uploaded.pid)
     downloaded = scicat_client.get_orig_datablocks(uploaded.pid)
     assert len(downloaded) == 1
     downloaded = downloaded[0]
     for key, expected in orig_datablock:
         # The database populates a number of fields that are orig_datablock in dset.
         # But we don't want to test those here as we don't want to test the database.
         if expected is not None and key != "dataFileList":
```

### Comparing `scitacean-24.4.0/tests/client/dataset_client_test.py` & `scitacean-24.5.0/tests/client/dataset_client_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="arg-type, index"
 
 import pydantic
 import pytest
 from dateutil.parser import parse as parse_date
 
-from scitacean import PID, Client, RemotePath, ScicatCommError
+from scitacean import PID, Client, Dataset, RemotePath, ScicatCommError
 from scitacean.client import ScicatClient
 from scitacean.model import (
     DatasetType,
     UploadDerivedDataset,
 )
 from scitacean.testing.backend.seed import (
     INITIAL_DATASETS,
@@ -36,15 +36,15 @@
         usedSoftware=[],
         ownerGroup=scicat_access.user.group,
         accessGroups=["koelle"],
         numberOfFilesArchived=0,
     )
 
 
-@pytest.mark.parametrize("key", ("raw", "derived"))
+@pytest.mark.parametrize("key", ["raw", "derived"])
 def test_get_dataset_model(scicat_client, key):
     dset = INITIAL_DATASETS[key]
     downloaded = scicat_client.get_dataset_model(dset.pid)
     # The backend may update the dataset after upload.
     # We cannot easily predict when that happens.
     downloaded.updatedAt = dset.updatedAt
     assert downloaded == dset
@@ -64,30 +64,32 @@
         if expected is not None:
             assert expected == dict(downloaded)[key], f"key = {key}"
 
 
 def test_validate_dataset_model(real_client, require_scicat_backend, derived_dataset):
     real_client.scicat.validate_dataset_model(derived_dataset)
     derived_dataset.contactEmail = "NotAnEmail"
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="validation in SciCat"):
         real_client.scicat.validate_dataset_model(derived_dataset)
 
 
 def test_get_dataset(client):
     dset = INITIAL_DATASETS["raw"]
     dblock = INITIAL_ORIG_DATABLOCKS["raw"][0]
     downloaded = client.get_dataset(dset.pid)
 
     assert downloaded.source_folder == dset.sourceFolder
     assert downloaded.creation_time == dset.creationTime
     assert downloaded.access_groups == dset.accessGroups
     assert downloaded.meta["temperature"] == dset.scientificMetadata["temperature"]
     assert downloaded.meta["data_type"] == dset.scientificMetadata["data_type"]
 
-    for dset_file, expected_file in zip(downloaded.files, dblock.dataFileList):
+    for dset_file, expected_file in zip(
+        downloaded.files, dblock.dataFileList, strict=True
+    ):
         assert dset_file.local_path is None
         assert dset_file.size == expected_file.size
         assert dset_file.creation_time == expected_file.time
 
 
 def test_can_get_public_dataset_without_login(require_scicat_backend, scicat_access):
     client = Client.without_login(url=scicat_access.url)
@@ -96,15 +98,17 @@
     dblock = INITIAL_ORIG_DATABLOCKS["public"][0]
     downloaded = client.get_dataset(dset.pid)
 
     assert downloaded.source_folder == dset.sourceFolder
     assert downloaded.creation_time == dset.creationTime
     assert downloaded.access_groups == dset.accessGroups
 
-    for dset_file, expected_file in zip(downloaded.files, dblock.dataFileList):
+    for dset_file, expected_file in zip(
+        downloaded.files, dblock.dataFileList, strict=True
+    ):
         assert dset_file.local_path is None
         assert dset_file.size == expected_file.size
         assert dset_file.creation_time == expected_file.time
 
 
 def test_cannot_upload_without_login(
     require_scicat_backend, derived_dataset, scicat_access
@@ -133,7 +137,26 @@
     assert downloaded.size == 0
 
 
 def test_get_broken_dataset_strict_validation(real_client, require_scicat_backend):
     dset = INITIAL_DATASETS["partially-broken"]
     with pytest.raises(pydantic.ValidationError):
         real_client.get_dataset(dset.pid, strict_validation=True)
+
+
+def test_dataset_with_orig_datablock_roundtrip(client):
+    ds = Dataset.from_download_models(
+        INITIAL_DATASETS["raw"], INITIAL_ORIG_DATABLOCKS["raw"], []
+    ).as_new()
+    # Unset fields that a raw dataset should not have but where initialized
+    # in the download model.
+    ds.input_datasets = None
+    ds.used_software = None
+
+    # We don't need a file transfer because all files are on remote.
+    finalized = client.upload_new_dataset_now(ds)
+    downloaded = client.get_dataset(finalized.pid)
+
+    assert downloaded.name == ds.name
+    assert downloaded.owner == ds.owner
+    assert downloaded.size == ds.size
+    assert downloaded.number_of_files == ds.number_of_files
```

### Comparing `scitacean-24.4.0/tests/client/sample_client_test.py` & `scitacean-24.5.0/tests/client/sample_client_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tests/common/files.py` & `scitacean-24.5.0/tests/common/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     checksum_digest = checksum.hexdigest()
 
     fs.create_file(path, contents=contents)
     # Not exact but should at least be precise to the second
     # and avoids potential difficulties of querying the file system.
     creation_time = datetime.now().astimezone(timezone.utc)
 
-    return dict(
-        path=path,
-        creation_time=creation_time,
-        checksum=checksum_digest,
-        size=len(contents),
-    )
+    return {
+        "path": path,
+        "creation_time": creation_time,
+        "checksum": checksum_digest,
+        "size": len(contents),
+    }
```

### Comparing `scitacean-24.4.0/tests/conftest.py` & `scitacean-24.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tests/dataset_fields_test.py` & `scitacean-24.5.0/tests/dataset_fields_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,23 +32,23 @@
 
 def test_init_dataset_with_only_type():
     dset = Dataset(type="raw")
     assert dset.type == DatasetType.RAW
 
 
 @pytest.mark.parametrize(
-    "typ", ("raw", "derived", DatasetType.RAW, DatasetType.DERIVED)
+    "typ", ["raw", "derived", DatasetType.RAW, DatasetType.DERIVED]
 )
 def test_init_dataset_accepted_types(typ):
     dset = Dataset(type=typ)
     assert dset.type == typ
 
 
 def test_init_dataset_raises_for_bad_type():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="DatasetType"):
         Dataset(type="bad-type")  # type: ignore[arg-type]
 
 
 def test_init_dataset_needs_type():
     with pytest.raises(TypeError):
         Dataset()  # type: ignore[call-arg]
 
@@ -416,16 +416,15 @@
         owner="Mustrum Ridcully",
         owner_group="faculty",
         principal_investigator="p.stibbons@uu.am",
         source_folder=RemotePath("/hex/source62"),
     )
     val = data.draw(st.from_type(field.type))
     assume(val is not None)
-    setattr(dset, field.name, val)
-    with pytest.raises(ValueError):
+    with pytest.raises(pydantic.ValidationError):
         dset.make_upload_model()
 
 
 @pytest.mark.parametrize(
     "field",
     (
         f
@@ -447,19 +446,19 @@
         source_folder=RemotePath("/hex/source62"),
         input_datasets=[PID(pid="623-122")],
         used_software=["scitacean", "magick"],
     )
     val = data.draw(st.from_type(field.type))
     assume(val is not None)
     setattr(dset, field.name, val)
-    with pytest.raises(ValueError):
+    with pytest.raises(pydantic.ValidationError):
         dset.make_upload_model()
 
 
-@pytest.mark.parametrize("field", ("contact_email", "owner_email"))
+@pytest.mark.parametrize("field", ["contact_email", "owner_email"])
 def test_email_validation(field):
     dset = Dataset(
         type="raw",
         contact_email="p.stibbons@uu.am",
         creation_time="2142-04-02T16:44:56",
         owner="Mustrum Ridcully",
         owner_group="faculty",
@@ -469,19 +468,19 @@
     setattr(dset, field, "not-an-email")
     with pytest.raises(pydantic.ValidationError):
         dset.make_upload_model()
 
 
 @pytest.mark.parametrize(
     "good_orcid",
-    (
+    [
         "https://orcid.org/0000-0002-3761-3201",
         "https://orcid.org/0000-0001-2345-6789",
         "https://orcid.org/0000-0003-2818-0368",
-    ),
+    ],
 )
 def test_orcid_validation_valid(good_orcid):
     dset = Dataset(
         type="raw",
         contact_email="jan-lukas.wynen@ess.eu",
         creation_location="scitacean/tests",
         creation_time="2142-04-02T16:44:56",
@@ -492,20 +491,20 @@
         orcid_of_owner=good_orcid,
     )
     assert dset.make_upload_model().orcidOfOwner == good_orcid
 
 
 @pytest.mark.parametrize(
     "bad_orcid",
-    (
+    [
         "0000-0002-3761-3201",
         "https://not-orcid.eu/0000-0002-3761-3201",
         "https://orcid.org/0010-0002-3765-3201",
         "https://orcid.org/0000-0002-3761-320X",
-    ),
+    ],
 )
 def test_orcid_validation_missing_url(bad_orcid):
     dset = Dataset(
         type="raw",
         contact_email="jan-lukas.wynen@ess.eu",
         creation_time="2142-04-02T16:44:56",
         owner="Jan-Lukas Wynen",
```

### Comparing `scitacean-24.4.0/tests/dataset_test.py` & `scitacean-24.5.0/tests/dataset_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         comment="Where did this come from?",
         createdAt=parse_datetime("1995-08-06T14:14:14Z"),
         createdBy="pstibbons",
         dataFormat=".thaum",
         dataQualityMetrics=24,
         description="Some shady data",
         endTime=parse_datetime("1995-08-03T00:00:00Z"),
-        history=None,
         instrumentGroup="professors",
         instrumentId="0000-aa",
         isPublished=True,
         jobLogData=None,
         jobParameters=None,
         keywords=["thaum", "shady"],
         license="NoThouchy",
@@ -108,15 +107,14 @@
         comment="Why did we actually make this data?",
         createdAt=parse_datetime("1995-08-06T14:14:14Z"),
         createdBy="pstibbons",
         dataFormat=None,
         dataQualityMetrics=24,
         description="Dubiously analyzed data",
         endTime=None,
-        history=None,
         instrumentGroup="professors",
         instrumentId=None,
         isPublished=True,
         jobLogData="process interrupted",
         jobParameters={"nodes": 4},
         keywords=["thaum", "dubious"],
         license="NoThouchy",
@@ -182,25 +180,25 @@
 def test_from_download_models_does_not_initialize_wrong_fields(dataset_download_model):
     dset = Dataset.from_download_models(dataset_download_model, [])
     for field in dset.fields():
         if not field.used_by(dataset_download_model.type):
             assert getattr(dset, field.name) is None
 
 
-@pytest.mark.parametrize("typ", (DatasetType.RAW, DatasetType.DERIVED))
+@pytest.mark.parametrize("typ", [DatasetType.RAW, DatasetType.DERIVED])
 def test_new_dataset_has_no_files(typ):
     dset = Dataset(type=typ)
     assert len(list(dset.files)) == 0
     assert dset.number_of_files == 0
     assert dset.number_of_files_archived == 0
     assert dset.packed_size == 0
     assert dset.size == 0
 
 
-@pytest.mark.parametrize("typ", (DatasetType.RAW, DatasetType.DERIVED))
+@pytest.mark.parametrize("typ", [DatasetType.RAW, DatasetType.DERIVED])
 def test_add_local_file_to_new_dataset(typ, fs):
     file_data = make_file(fs, "local/folder/data.dat")
 
     dset = Dataset(type=typ)
     dset.add_local_files("local/folder/data.dat")
 
     assert len(list(dset.files)) == 1
@@ -217,15 +215,15 @@
     assert f.size == file_data["size"]
     assert f.checksum_algorithm == "blake2b"
 
     assert abs(file_data["creation_time"] - f.creation_time) < timedelta(seconds=1)
     assert abs(file_data["creation_time"] - f.make_model().time) < timedelta(seconds=1)
 
 
-@pytest.mark.parametrize("typ", (DatasetType.RAW, DatasetType.DERIVED))
+@pytest.mark.parametrize("typ", [DatasetType.RAW, DatasetType.DERIVED])
 def test_add_multiple_local_files_to_new_dataset(typ, fs):
     file_data0 = make_file(fs, "common/location1/data.dat")
     file_data1 = make_file(fs, "common/song.mp3")
 
     dset = Dataset(type=typ)
     dset.add_local_files("common/location1/data.dat", "common/song.mp3")
 
@@ -250,15 +248,15 @@
     assert f1.is_on_local
     assert f1.remote_access_path(dset.source_folder) is None
     assert f1.local_path == Path("common/song.mp3")
     assert f1.size == file_data1["size"]
     assert f1.checksum_algorithm == "blake2b"
 
 
-@pytest.mark.parametrize("typ", (DatasetType.RAW, DatasetType.DERIVED))
+@pytest.mark.parametrize("typ", [DatasetType.RAW, DatasetType.DERIVED])
 def test_add_multiple_local_files_to_new_dataset_with_base_path(typ, fs):
     file_data0 = make_file(fs, "common/location1/data.dat")
     file_data1 = make_file(fs, "common/song.mp3")
 
     dset = Dataset(type=typ)
     dset.add_local_files(
         "common/location1/data.dat", "common/song.mp3", base_path="common"
@@ -285,16 +283,16 @@
     assert f1.is_on_local
     assert f1.remote_access_path(dset.source_folder) is None
     assert f1.local_path == Path("common/song.mp3")
     assert f1.size == file_data1["size"]
     assert f1.checksum_algorithm == "blake2b"
 
 
-@pytest.mark.parametrize("typ", (DatasetType.RAW, DatasetType.DERIVED))
-@pytest.mark.parametrize("algorithm", ("sha256", None))
+@pytest.mark.parametrize("typ", [DatasetType.RAW, DatasetType.DERIVED])
+@pytest.mark.parametrize("algorithm", ["sha256", None])
 def test_can_set_default_checksum_algorithm(typ, algorithm, fs):
     make_file(fs, "local/data.dat")
 
     dset = Dataset(type=typ, checksum_algorithm=algorithm)
     dset.add_local_files("local/data.dat")
 
     [f] = dset.files
@@ -329,24 +327,27 @@
     assert dataset.make_datablock_upload_models().orig_datablocks is None
 
 
 @given(sst.datasets(pid=st.builds(PID)))
 @settings(max_examples=10)
 def test_make_scicat_models_datablock_with_one_file(dataset):
     file_model = model.DownloadDataFile(
-        path="path", size=6163, chk="8450ac0", gid="group", time=datetime.now()
+        path="path",
+        size=6163,
+        chk="8450ac0",
+        gid="group",
+        time=datetime.now(tz=timezone.utc),
     )
     dataset.add_files(File.from_download_model(local_path=None, model=file_model))
 
     blocks = dataset.make_datablock_upload_models().orig_datablocks
     assert len(blocks) == 1
 
     block = blocks[0]
     assert block.size == 6163
-    assert block.datasetId == dataset.pid
     assert block.dataFileList == [model.UploadDataFile(**file_model.model_dump())]
 
 
 def test_attachments_are_empty_by_default():
     dataset = Dataset(
         type="raw",
         owner="ridcully",
@@ -434,15 +435,17 @@
 
 @given(sst.datasets())
 @settings(max_examples=10)
 def test_eq_self(dset):
     dset.add_files(
         File.from_download_model(
             local_path=None,
-            model=model.DownloadDataFile(path="path", size=94571, time=datetime.now()),
+            model=model.DownloadDataFile(
+                path="path", size=94571, time=datetime.now(tz=timezone.utc)
+            ),
         )
     )
     dset.attachments.append(
         model.Attachment(caption="The attachment", owner_group="owner")
     )
     assert dset == dset
 
@@ -477,37 +480,39 @@
 @settings(max_examples=10)
 def test_neq_single_mismatched_file(initial):
     modified = initial.replace()
     modified.add_files(
         File.from_download_model(
             local_path=None,
             model=model.DownloadDataFile(
-                path="path", size=51553312, time=datetime.now()
+                path="path", size=51553312, time=datetime.now(tz=timezone.utc)
             ),
         )
     )
     initial.add_files(
         File.from_download_model(
             local_path=None,
-            model=model.DownloadDataFile(path="path", size=94571, time=datetime.now()),
+            model=model.DownloadDataFile(
+                path="path", size=94571, time=datetime.now(tz=timezone.utc)
+            ),
         )
     )
     assert modified != initial
     assert initial != modified
 
 
 @given(sst.datasets())
 @settings(max_examples=10)
 def test_neq_extra_file(initial):
     modified = initial.replace()
     modified.add_files(
         File.from_download_model(
             local_path="/local",
             model=model.DownloadDataFile(
-                path="path", size=51553312, time=datetime.now()
+                path="path", size=51553312, time=datetime.now(tz=timezone.utc)
             ),
         )
     )
     assert modified != initial
     assert initial != modified
 
 
@@ -567,15 +572,14 @@
 @pytest.mark.parametrize(
     "field",
     (
         field
         for field in Dataset.fields(read_only=True)
         if field.name
         not in (
-            "history",
             "lifecycle",
             "number_of_files",
             "number_of_files_archived",
             "size",
             "packed_size",
         )
     ),
@@ -610,15 +614,14 @@
         techniques=[model.Technique(pid="tech/abcd.01", name="magick")],
         type="raw",
         _read_only={"api_version": 666},
     )
     assert replaced.owner == initial.owner
     assert replaced.size == initial.size
     assert replaced.updated_at == initial.updated_at
-    assert replaced.history == initial.history
 
 
 @given(sst.datasets())
 @settings(max_examples=1)
 def test_replace_rejects_bad_arguments(initial):
     with pytest.raises(TypeError):
         initial.replace(this_is_not_a_valid="argument", owner="the-owner-of-it-all")
@@ -634,15 +637,17 @@
 
 
 @given(sst.datasets())
 @settings(max_examples=1)
 def test_replace_does_not_change_files_with_input_files(initial):
     file = File.from_download_model(
         local_path=None,
-        model=model.DownloadDataFile(path="path", size=6163, time=datetime.now()),
+        model=model.DownloadDataFile(
+            path="path", size=6163, time=datetime.now(tz=timezone.utc)
+        ),
     )
     initial.add_files(file)
     replaced = initial.replace(owner="a-new-owner")
     assert replaced.number_of_files == 1
     assert replaced.size == 6163
     assert list(replaced.files) == list(initial.files)
 
@@ -674,31 +679,31 @@
     initial.meta["old-key"] = "old-val"
     replaced = initial.replace(owner="a-new-owner", meta=None)
     assert replaced.meta == {}
 
 
 @pytest.mark.parametrize(
     "attachments",
-    (None, [], [model.Attachment(caption="Attachment 1", owner_group="owner")]),
+    [None, [], [model.Attachment(caption="Attachment 1", owner_group="owner")]],
 )
 @given(initial=sst.datasets())
 @settings(max_examples=1)
 def test_replace_preserves_attachments(initial, attachments):
     initial.attachments = attachments
     replaced = initial.replace(owner="a-new-owner")
     assert replaced.attachments == attachments
 
 
 @pytest.mark.parametrize(
     "attachments",
-    (None, [], [model.Attachment(caption="Attachment 1", owner_group="owner")]),
+    [None, [], [model.Attachment(caption="Attachment 1", owner_group="owner")]],
 )
 @pytest.mark.parametrize(
     "target_attachments",
-    (None, [], [model.Attachment(caption="Attachment 2", owner_group="owner")]),
+    [None, [], [model.Attachment(caption="Attachment 2", owner_group="owner")]],
 )
 @given(initial=sst.datasets())
 @settings(max_examples=1)
 def test_replace_attachments(initial, attachments, target_attachments):
     replaced = initial.replace(attachments=target_attachments)
     assert replaced.attachments == target_attachments
 
@@ -707,15 +712,14 @@
 @settings(max_examples=5)
 def test_as_new(initial):
     new = initial.as_new()
     assert new.created_at is None
     assert new.created_by is None
     assert new.updated_at is None
     assert new.updated_by is None
-    assert new.history is None
     assert new.lifecycle is None
     assert abs(new.creation_time - datetime.now(tz=timezone.utc)) < timedelta(seconds=1)
 
     assert new.number_of_files == initial.number_of_files
     assert new.size == initial.size
     assert new.name == initial.name
     assert new.input_datasets == initial.input_datasets
@@ -725,15 +729,14 @@
 @given(sst.datasets(pid=PID(pid="some-id")))
 @settings(max_examples=5)
 def test_derive_default(initial):
     derived = initial.derive()
     assert derived.type == "derived"
     assert derived.input_datasets == [initial.pid]
     assert derived.lifecycle is None
-    assert derived.history is None
 
     assert derived.investigator == initial.investigator
     assert derived.owner == initial.owner
     assert derived.orcid_of_owner == initial.orcid_of_owner
     assert derived.owner_email == initial.owner_email
     assert derived.contact_email == initial.contact_email
     assert derived.techniques == initial.techniques
@@ -747,15 +750,14 @@
 @given(sst.datasets(pid=PID(pid="some-id")))
 @settings(max_examples=5)
 def test_derive_set_keep(initial):
     derived = initial.derive(keep=("name", "used_software"))
     assert derived.type == "derived"
     assert derived.input_datasets == [initial.pid]
     assert derived.lifecycle is None
-    assert derived.history is None
 
     assert derived.name == initial.name
     assert derived.used_software == initial.used_software
 
     assert derived.number_of_files == 0
     assert derived.number_of_files_archived == 0
 
@@ -763,34 +765,33 @@
 @given(sst.datasets(pid=PID(pid="some-id")))
 @settings(max_examples=5)
 def test_derive_keep_nothing(initial):
     derived = initial.derive(keep=())
     assert derived.type == "derived"
     assert derived.input_datasets == [initial.pid]
     assert derived.lifecycle is None
-    assert derived.history is None
 
     assert derived.investigator is None
     assert derived.owner is None
     assert derived.name is None
     assert derived.used_software is None
     assert derived.number_of_files == 0
     assert derived.number_of_files_archived == 0
 
 
 @given(sst.datasets(pid=None))
 @settings(max_examples=5)
 def test_derive_requires_pid(initial):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="pid"):
         initial.derive()
 
 
 @pytest.mark.parametrize(
     "attachments",
-    (None, [], [model.Attachment(caption="Attachment 1", owner_group="owner")]),
+    [None, [], [model.Attachment(caption="Attachment 1", owner_group="owner")]],
 )
 @given(initial=sst.datasets(pid=PID(pid="some-id")))
 @settings(max_examples=1)
 def test_derive_removes_attachments(initial, attachments):
     initial.attachments = attachments
     derived = initial.derive()
     assert derived.attachments == []
@@ -804,48 +805,48 @@
     else:
         raise ValueError(my_type, " is not valid DatasetType.")
 
 
 @given(initial=sst.datasets(for_upload=True))
 @settings(max_examples=10)
 def test_dataset_dict_like_keys_per_type(initial: Dataset) -> None:
-    my_names = set(
+    my_names = {
         field.name for field in Dataset._FIELD_SPEC if field.used_by(initial.type)
-    )
+    }
     assert set(initial.keys()) == my_names
 
 
 @given(initial=sst.datasets(for_upload=True))
 @settings(max_examples=10)
 def test_dataset_dict_like_keys_including_invalid_field(initial):
     invalid_name, invalid_value = invalid_field_example(initial.type)
 
-    my_names = set(
+    my_names = {
         field.name for field in Dataset._FIELD_SPEC if field.used_by(initial.type)
-    )
+    }
     assert invalid_name not in my_names
     my_names.add(invalid_name)
 
     setattr(initial, invalid_name, invalid_value)
 
     assert set(initial.keys()) == my_names
 
 
 @given(initial=sst.datasets(for_upload=True))
 @settings(max_examples=10)
 def test_dataset_dict_like_values(initial: Dataset) -> None:
-    for key, value in zip(initial.keys(), initial.values()):
+    for key, value in zip(initial.keys(), initial.values(), strict=True):
         assert value == getattr(initial, key)
 
 
 @given(initial=sst.datasets(for_upload=True))
 @settings(max_examples=10)
 def test_dataset_dict_like_values_with_invalid_field(initial: Dataset) -> None:
     setattr(initial, *invalid_field_example(initial.type))
-    for key, value in zip(initial.keys(), initial.values()):
+    for key, value in zip(initial.keys(), initial.values(), strict=True):
         assert value == getattr(initial, key)
 
 
 @given(initial=sst.datasets(for_upload=True))
 @settings(max_examples=10)
 def test_dataset_dict_like_items_with_invalid_field(initial: Dataset) -> None:
     setattr(initial, *invalid_field_example(initial.type))
@@ -856,15 +857,15 @@
 @given(initial=sst.datasets(for_upload=True))
 @settings(max_examples=10)
 def test_dataset_dict_like_getitem(initial):
     assert initial["type"] == initial.type
 
 
 @pytest.mark.parametrize(
-    ("is_attr", "wrong_field"), ((True, "size"), (False, "OBVIOUSLYWRONGNAME"))
+    ("is_attr", "wrong_field"), [(True, "size"), (False, "OBVIOUSLYWRONGNAME")]
 )
 @given(initial=sst.datasets(for_upload=True))
 @settings(max_examples=10)
 def test_dataset_dict_like_getitem_wrong_field_raises(initial, is_attr, wrong_field):
     # 'size' should be included in the field later.
     # It is now excluded because it is ``manual`` field. See issue#151.
     assert hasattr(initial, wrong_field) == is_attr
@@ -891,15 +892,15 @@
     assert initial[invalid_field] is None
     initial[invalid_field] = invalid_value
     assert initial[invalid_field] == invalid_value
 
 
 @pytest.mark.parametrize(
     ("is_attr", "wrong_field", "wrong_value"),
-    ((True, "size", 10), (False, "OBVIOUSLYWRONGNAME", "OBVIOUSLYWRONGVALUE")),
+    [(True, "size", 10), (False, "OBVIOUSLYWRONGNAME", "OBVIOUSLYWRONGVALUE")],
 )
 @given(initial=sst.datasets(for_upload=True))
 @settings(max_examples=10)
 def test_dataset_dict_like_setitem_wrong_field_raises(
     initial, is_attr, wrong_field, wrong_value
 ):
     # ``manual`` fields such as ``size`` should raise with ``__setitem__``.
```

### Comparing `scitacean-24.4.0/tests/download_test.py` & `scitacean-24.5.0/tests/download_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def _checksum(data: bytes) -> str:
     checksum = hashlib.new("md5")
     checksum.update(data)
     return checksum.hexdigest()
 
 
-@pytest.fixture
+@pytest.fixture()
 def data_files():
     contents = {
         "file1.dat": b"contents-of-file1",
         "log/what-happened.log": b"ERROR Flux is off the scale",
         "thaum.dat": b"0 4 2 59 330 2314552",
     }
     files = [
@@ -37,15 +37,15 @@
             time=parse_date("1995-08-06T14:14:14"),
         )
         for name, content in contents.items()
     ]
     return files, contents
 
 
-@pytest.fixture
+@pytest.fixture()
 def dataset_and_files(data_files):
     model = DownloadDataset(
         contactEmail="p.stibbons@uu.am",
         creationTime=parse_date("1995-08-06T14:14:14"),
         numberOfFiles=len(data_files[0]),
         numberOfFilesArchived=0,
         owner="pstibbons",
```

### Comparing `scitacean-24.4.0/tests/file_test.py` & `scitacean-24.5.0/tests/file_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from scitacean.filesystem import checksum_of_file
 from scitacean.logging import logger_name
 from scitacean.model import DownloadDataFile
 
 from .common.files import make_file
 
 
-@pytest.fixture
+@pytest.fixture()
 def fake_file(fs):
     return make_file(fs, path=Path("local", "dir", "events.nxs"))
 
 
 def test_file_from_local(fake_file):
     file = replace(File.from_local(fake_file["path"]), checksum_algorithm="md5")
     assert file.remote_access_path("/remote") is None
@@ -84,15 +84,15 @@
     assert file.size == fake_file["size"]
     assert file.remote_uid == "user-usy"
     assert file.remote_gid == "groupy-group"
     assert file.remote_perm == "wrx"
     assert abs(fake_file["creation_time"] - file.creation_time) < timedelta(seconds=1)
 
 
-@pytest.mark.parametrize("alg", ("md5", "sha256", "blake2s"))
+@pytest.mark.parametrize("alg", ["md5", "sha256", "blake2s"])
 def test_file_from_local_select_checksum_algorithm(fake_file, alg):
     file = replace(File.from_local(fake_file["path"]), checksum_algorithm=alg)
     expected = checksum_of_file(fake_file["path"], algorithm=alg)
     assert file.checksum() == expected
 
 
 def test_file_from_local_remote_path_uses_forward_slash(fs):
@@ -373,15 +373,15 @@
     )
     downloaded = file.downloaded(local_path=fake_file["path"])
     with caplog.at_level("INFO", logger=logger_name()):
         downloaded.validate_after_download()
     assert "does not match size reported in dataset" in caplog.text
 
 
-@pytest.mark.parametrize("chk", ("sha256", None))
+@pytest.mark.parametrize("chk", ["sha256", None])
 def test_local_is_not_up_to_date_for_remote_file(chk):
     file = File.from_download_model(
         DownloadDataFile(
             path="data.csv",
             size=65178,
             chk=chk,
             time=parse_date("2022-06-22T15:42:53.123Z"),
```

### Comparing `scitacean-24.4.0/tests/filesystem_test.py` & `scitacean-24.5.0/tests/filesystem_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,28 +35,28 @@
 def test_remote_path_init_requires_path_like():
     with pytest.raises(TypeError):
         RemotePath(6133)  # type: ignore[arg-type]
     with pytest.raises(TypeError):
         RemotePath(["folder", "file.dat"])  # type: ignore[arg-type]
 
 
-@pytest.mark.parametrize("local_type", (PurePath, Path))
+@pytest.mark.parametrize("local_type", [PurePath, Path])
 def test_remote_path_rejects_os_path(local_type):
     with pytest.raises(TypeError):
         RemotePath(local_type("dir", "file.csv"))
 
 
-@pytest.mark.parametrize("local_type", (PurePath, PurePosixPath, PureWindowsPath))
+@pytest.mark.parametrize("local_type", [PurePath, PurePosixPath, PureWindowsPath])
 def test_remote_path_from_local(local_type):
     local_path = local_type("dir", "folder", "file.csv")
     remote_path = RemotePath.from_local(local_path)
     assert remote_path == RemotePath("dir/folder/file.csv")
 
 
-@pytest.mark.parametrize("local_type", (PurePath, PurePosixPath, PureWindowsPath))
+@pytest.mark.parametrize("local_type", [PurePath, PurePosixPath, PureWindowsPath])
 def test_remote_path_posix_uses_forward_slashes(local_type):
     local_path = local_type("dir", "folder", "file.csv")
     remote_path = RemotePath.from_local(local_path)
     assert remote_path.posix == "dir/folder/file.csv"
 
 
 def test_remote_path_str():
@@ -71,42 +71,42 @@
     assert RemotePath("folder/file.dat").to_local() == PurePath("folder", "file.dat")
     assert RemotePath("/folder/file.dat").to_local() == PurePath("/folder", "file.dat")
     assert RemotePath("folder//file.dat").to_local() == PurePath("folder", "file.dat")
     assert RemotePath("folder/file.dat/").to_local() == PurePath("folder", "file.dat")
 
 
 @pytest.mark.parametrize(
-    "types", ((RemotePath, RemotePath), (RemotePath, str), (str, RemotePath))
+    "types", [(RemotePath, RemotePath), (RemotePath, str), (str, RemotePath)]
 )
 def test_remote_path_eq(types):
     ta, tb = types
     assert ta("/source/data.csv") == tb("/source/data.csv")
 
 
 @pytest.mark.parametrize(
-    "types", ((RemotePath, RemotePath), (RemotePath, str), (str, RemotePath))
+    "types", [(RemotePath, RemotePath), (RemotePath, str), (str, RemotePath)]
 )
 def test_remote_path_neq(types):
     ta, tb = types
     assert ta("/source/data.csv") != tb("/host/dir/song.mp3")
 
 
 @pytest.mark.parametrize(
-    "types", ((RemotePath, RemotePath), (RemotePath, str), (str, RemotePath))
+    "types", [(RemotePath, RemotePath), (RemotePath, str), (str, RemotePath)]
 )
 def test_remote_path_join(types):
     ta, tb = types
     assert ta("/source/123") / tb("file.data") == RemotePath("/source/123/file.data")
     assert ta("/source/123/") / tb("file.data") == RemotePath("/source/123/file.data")
     assert ta("/source/123") / tb("/file.data") == RemotePath("/source/123/file.data")
     assert ta("/source/123/") / tb("/file.data") == RemotePath("/source/123/file.data")
 
 
 @pytest.mark.parametrize(
-    "types", ((RemotePath, RemotePath), (RemotePath, str), (str, RemotePath))
+    "types", [(RemotePath, RemotePath), (RemotePath, str), (str, RemotePath)]
 )
 def test_remote_path_join_url(types):
     ta, tb = types
     assert ta("https://server.eu") / tb("1234-abcd/data.txt") == RemotePath(
         "https://server.eu/1234-abcd/data.txt"
     )
     assert ta("https://server.eu/") / tb("1234-abcd/data.txt") == RemotePath(
@@ -158,15 +158,15 @@
 def test_remote_path_truncated():
     assert RemotePath("something-long.txt").truncated(10) == "someth.txt"
     assert RemotePath("longlonglong/short").truncated(5) == "longl/short"
     assert RemotePath("a-long.data.dir/filename.csv").truncated(7) == "a-l.dir/fil.csv"
     assert RemotePath("file.longextension").truncated(9) == "f.longext"
 
 
-@pytest.mark.parametrize("size", (0, 1, 57121))
+@pytest.mark.parametrize("size", [0, 1, 57121])
 def test_file_size(fs, size):
     fs.create_file("image.tiff", st_size=size)
     assert file_size(Path("image.tiff")) == size
 
 
 def test_file_modification_time(fs):
     fs.create_file("data.dat")
@@ -174,15 +174,15 @@
     assert abs(file_modification_time(Path("data.dat")) - expected) < timedelta(
         seconds=5
     )
 
 
 @pytest.mark.parametrize(
     "contents",
-    (b"small file contents", b"large contents " * 100000),
+    [b"small file contents", b"large contents " * 100000],
     ids=("small", "large"),
 )
 def test_checksum_of_file(fs, contents):
     fs.create_file("file.txt", contents=contents)
 
     assert (
         checksum_of_file("file.txt", algorithm="md5")
@@ -190,15 +190,15 @@
     )
     assert (
         checksum_of_file("file.txt", algorithm="sha256")
         == hashlib.sha256(contents).hexdigest()
     )
 
 
-@pytest.mark.parametrize("path_type", (str, Path, RemotePath))
+@pytest.mark.parametrize("path_type", [str, Path, RemotePath])
 def test_escape_path_returns_same_type_as_input(path_type):
     assert isinstance(escape_path(path_type("x")), path_type)
 
 
 @given(st.text())
 def test_escape_path_returns_ascii(path):
     # does not raise
```

### Comparing `scitacean-24.4.0/tests/html_repr/html_repr_test.py` & `scitacean-24.5.0/tests/html_repr/html_repr_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tests/model_test.py` & `scitacean-24.5.0/tests/model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     return st.builds(cls, **private_fields)
 
 
 @settings(max_examples=10)
 @given(data=st.data())
 @pytest.mark.parametrize(
     "model_types",
-    (
+    [
         (model.Attachment, model.UploadAttachment),
         (model.Technique, model.UploadTechnique),
         (model.Relationship, model.UploadRelationship),
-    ),
+    ],
 )
 # Cannot test (model.Sample, model.UploadSample) because hypothesis
 # cannot handle fields with type Any.
 def test_can_make_upload_model(model_types, data):
     user_model_type, upload_model_type = model_types
     user_model = data.draw(build_user_model_for_upload(user_model_type))
     upload_model = user_model.make_upload_model()
@@ -57,30 +57,30 @@
     assert upload_attachment.thumbnail == attachment.thumbnail
 
 
 @settings(max_examples=10)
 @given(st.builds(model.Attachment))
 def test_upload_model_rejects_non_upload_fields(attachment):
     attachment._created_by = "the-creator"
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="field.*upload"):
         attachment.make_upload_model()
 
 
 @settings(max_examples=10)
 @given(data=st.data())
 @pytest.mark.parametrize(
     "model_types",
-    (
+    [
         (model.Attachment, model.DownloadAttachment),
         (model.Lifecycle, model.DownloadLifecycle),
         (model.Technique, model.DownloadTechnique),
         (model.History, model.DownloadHistory),
         (model.Instrument, model.DownloadInstrument),
         (model.Relationship, model.DownloadRelationship),
-    ),
+    ],
 )
 def test_can_make_from_download_model(model_types, data):
     user_model_type, download_model_type = model_types
     download_model = data.draw(st.builds(download_model_type))
     # doesn't raise
     user_model_type.from_download_model(download_model)
 
@@ -125,15 +125,14 @@
     assert finalized.usedSoftware == ["software1"]
 
     # Default values
     assert finalized.createdAt  # some non-empty str
     assert finalized.createdBy  # some non-empty str
     assert finalized.classification  # some non-empty str
     assert finalized.datasetName  # some non-empty str
-    assert finalized.history is None
     assert finalized.isPublished is False
     assert finalized.keywords == []
     assert finalized.numberOfFiles == 0
     assert finalized.numberOfFilesArchived == 0
     assert finalized.packedSize == 0
     assert finalized.pid  # some non-empty str
     assert finalized.scientificMetadata == {}
@@ -181,15 +180,14 @@
     assert finalized.sourceFolder == "/source/folder"
 
     # Default values
     assert finalized.createdAt  # some non-empty str
     assert finalized.createdBy  # some non-empty str
     assert finalized.classification  # some non-empty str
     assert finalized.datasetName  # some non-empty str
-    assert finalized.history is None
     assert finalized.isPublished is False
     assert finalized.keywords == []
     assert finalized.numberOfFiles == 0
     assert finalized.numberOfFilesArchived == 0
     assert finalized.packedSize == 0
     assert finalized.pid  # some non-empty str
     assert finalized.scientificMetadata == {}
```

### Comparing `scitacean-24.4.0/tests/testing/strategies_test.py` & `scitacean-24.5.0/tests/testing/strategies_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tests/thumbnail_test.py` & `scitacean-24.5.0/tests/thumbnail_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tests/transfer/link_test.py` & `scitacean-24.5.0/tests/transfer/link_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scitacean contributors (https://github.com/SciCatProject/scitacean)
 
 import hashlib
 import sys
-from datetime import datetime
+from datetime import datetime, timezone
 
 import pytest
 
 from scitacean import PID, Dataset, DatasetType, RemotePath
 from scitacean.model import DownloadDataFile, DownloadDataset, DownloadOrigDatablock
 from scitacean.testing.client import FakeClient
 from scitacean.transfer.link import LinkFileTransfer
@@ -71,15 +71,15 @@
     remote_dir.mkdir()
     remote_dir.joinpath("file1.txt").write_text(content)
 
     ds = DownloadDataset(
         accessGroups=["group1"],
         contactEmail="p.stibbons@uu.am",
         creationLocation="UU",
-        creationTime=datetime(2023, 6, 23, 10, 0, 0),
+        creationTime=datetime(2023, 6, 23, 10, 0, 0, tzinfo=timezone.utc),
         numberOfFiles=1,
         numberOfFilesArchived=0,
         owner="PonderStibbons",
         ownerGroup="uu",
         pid=PID(prefix="UU.0123", pid="1234567890"),
         principalInvestigator="MustrumRidcully",
         size=len(content),
@@ -88,15 +88,15 @@
     )
     db = DownloadOrigDatablock(
         dataFileList=[
             DownloadDataFile(
                 path="file1.txt",
                 size=len(content),
                 chk=checksum,
-                time=datetime(2023, 6, 23, 10, 0, 0),
+                time=datetime(2023, 6, 23, 10, 0, 0, tzinfo=timezone.utc),
             )
         ],
         datasetId=ds.pid,
         size=len(content),
         chkAlg="md5",
     )
 
@@ -130,15 +130,15 @@
     local_dir.mkdir()
     local_dir.joinpath("file1.txt").write_text(content)
 
     ds = DownloadDataset(
         accessGroups=["group1"],
         contactEmail="p.stibbons@uu.am",
         creationLocation="UU",
-        creationTime=datetime(2023, 6, 23, 10, 0, 0),
+        creationTime=datetime(2023, 6, 23, 10, 0, 0, tzinfo=timezone.utc),
         numberOfFiles=1,
         numberOfFilesArchived=0,
         owner="PonderStibbons",
         ownerGroup="uu",
         pid=PID(prefix="UU.0123", pid="1234567890"),
         principalInvestigator="MustrumRidcully",
         size=len(content),
@@ -147,15 +147,15 @@
     )
     db = DownloadOrigDatablock(
         dataFileList=[
             DownloadDataFile(
                 path="file1.txt",
                 size=len(content),
                 chk=checksum,
-                time=datetime(2023, 6, 23, 10, 0, 0),
+                time=datetime(2023, 6, 23, 10, 0, 0, tzinfo=timezone.utc),
             )
         ],
         datasetId=ds.pid,
         size=len(content),
         chkAlg="md5",
     )
 
@@ -191,15 +191,15 @@
     local_dir.mkdir()
     local_dir.joinpath("file1.txt").write_text(content + content)
 
     ds = DownloadDataset(
         accessGroups=["group1"],
         contactEmail="p.stibbons@uu.am",
         creationLocation="UU",
-        creationTime=datetime(2023, 6, 23, 10, 0, 0),
+        creationTime=datetime(2023, 6, 23, 10, 0, 0, tzinfo=timezone.utc),
         numberOfFiles=1,
         numberOfFilesArchived=0,
         owner="PonderStibbons",
         ownerGroup="uu",
         pid=PID(prefix="UU.0123", pid="1234567890"),
         principalInvestigator="MustrumRidcully",
         size=len(content),
@@ -208,15 +208,15 @@
     )
     db = DownloadOrigDatablock(
         dataFileList=[
             DownloadDataFile(
                 path="file1.txt",
                 size=len(content),
                 chk=checksum,
-                time=datetime(2023, 6, 23, 10, 0, 0),
+                time=datetime(2023, 6, 23, 10, 0, 0, tzinfo=timezone.utc),
             )
         ],
         datasetId=ds.pid,
         size=len(content),
         chkAlg="md5",
     )
```

### Comparing `scitacean-24.4.0/tests/transfer/sftp_test.py` & `scitacean-24.5.0/tests/transfer/sftp_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     SFTPDownloadConnection,
     SFTPFileTransfer,
     SFTPUploadConnection,
 )
 
 
 @pytest.fixture(scope="session", autouse=True)
-def server(request, sftp_fileserver):
+def _server(request, sftp_fileserver):
     skip_if_not_sftp(request)
 
 
 def test_download_one_file(sftp_access, sftp_connect_with_username_password, tmp_path):
     sftp = SFTPFileTransfer(
         host=sftp_access.host,
         port=sftp_access.port,
@@ -397,15 +397,15 @@
             port=sftp_access.port,
         ),
     )
     ds = Dataset(
         access_groups=["group1"],
         contact_email="p.stibbons@uu.am",
         creation_location="UU",
-        creation_time=datetime(2023, 6, 23, 10, 0, 0),
+        creation_time=datetime(2023, 6, 23, 10, 0, 0, tzinfo=timezone.utc),
         owner="PonderStibbons",
         owner_group="uu",
         principal_investigator="MustrumRidcully",
         source_folder="/data",
         type="raw",
     )
     ds.add_local_files(tmp_path / "file1.txt", base_path=tmp_path)
```

### Comparing `scitacean-24.4.0/tests/upload_test.py` & `scitacean-24.5.0/tests/upload_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # TODO source_folder changed / populated in file after upload
 
 
 def get_file_transfer(client: Client) -> FakeFileTransfer:
     return client.file_transfer  # type: ignore[return-value]
 
 
-@pytest.fixture
+@pytest.fixture()
 def dataset():
     return Dataset(
         access_groups=["group1", "2nd_group"],
         investigator="ridcully@uu.am",
         contact_email="p.stibbons@uu.am",
         source_folder="/hex/source123",
         creation_time=parse_date("2011-08-24T12:34:56Z"),
@@ -47,23 +47,23 @@
             "temperature": {"value": "123", "unit": "K"},
             "weight": {"value": "42", "unit": "mg"},
         },
         type=DatasetType.DERIVED,
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def dataset_with_files(dataset, fs):
     make_file(fs, path="file.nxs", contents=b"contents of file.nxs")
     make_file(fs, path="the_log_file.log", contents=b"this is a log file")
     dataset.add_local_files("file.nxs", "the_log_file.log")
     return dataset
 
 
-@pytest.fixture
+@pytest.fixture()
 def attachments():
     return [
         Attachment(
             caption="Attachment no 1",
             owner_group="uu",
             thumbnail=Thumbnail(mime="png/jpeg", data=b"840109725761"),
         ),
@@ -71,15 +71,15 @@
             caption="Second attachment",
             owner_group="uu",
             thumbnail=Thumbnail(mime=None, data=b"5189762957"),
         ),
     ]
 
 
-@pytest.fixture
+@pytest.fixture()
 def client(fs, scicat_access):
     return FakeClient.from_credentials(
         url="",
         **scicat_access.user.credentials,
         file_transfer=FakeFileTransfer(fs=fs, files={}, reverted={}),
     )
 
@@ -167,18 +167,18 @@
             "updated_by": finalized.updated_by,
         }
     )
     assert finalized == expected
 
 
 def test_upload_with_both_remote_and_local_files(client, dataset_with_files):
-    original_file_names = set(
+    original_file_names = {
         dataset_with_files.source_folder / file.remote_path
         for file in dataset_with_files.files
-    )
+    }
     dataset_with_files.add_files(
         File.from_remote(
             remote_path="file1.h5", size=6123, creation_time="2019-09-09T19:29:39Z"
         )
     )
 
     finalized = client.upload_new_dataset_now(dataset_with_files)
@@ -280,15 +280,15 @@
 
 
 def test_upload_does_not_create_dataset_if_validation_fails(dataset_with_files, fs):
     client = FakeClient(
         disable={"validate_dataset_model": ValueError("Validation failed")},
         file_transfer=FakeFileTransfer(fs=fs),
     )
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Validation"):
         client.upload_new_dataset_now(dataset_with_files)
 
     assert not client.datasets
     assert not client.orig_datablocks
     assert not client.attachments
     assert not get_file_transfer(client).files
```

### Comparing `scitacean-24.4.0/tests/util/formatter_test.py` & `scitacean-24.5.0/tests/util/formatter_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,9 +55,9 @@
     dset = Dataset(type="raw", owner="Nanny Ogg")
     formatted = DatasetPathFormatter().format("{type}/{owner}.data", dset=dset)
     assert formatted == "raw/Nanny Ogg.data"
 
 
 def test_dataset_formatter_does_not_allow_none():
     dset = Dataset(type="raw", owner=None)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="format path"):
         DatasetPathFormatter().format("{owner}", dset=dset)
```

### Comparing `scitacean-24.4.0/tools/model-generation/README.md` & `scitacean-24.5.0/tools/model-generation/README.md`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tools/model-generation/generate_models.py` & `scitacean-24.5.0/tools/model-generation/generate_models.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tools/model-generation/spec/__init__.py` & `scitacean-24.5.0/tools/model-generation/spec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     download: bool = False
     validation: str | None = None
 
     def full_type_for(self, kind: Literal["download", "upload", "user"]) -> str:
         return (
             self.type_for(kind)
             if self.required and kind != "download"
-            else f"Optional[{self.type_for(kind)}]"
+            else f"{self.type_for(kind)} | None"
         )
 
     def type_for(self, kind: Literal["download", "upload", "user"]) -> str:
         """Translate SciCat schema/DTO names into Scitacean model names."""
         if kind == "upload":
             prefix = "Upload"
         elif kind == "download":
@@ -139,15 +139,15 @@
         if manual is None:
             return list(self.fields.values())
         return [field for field in self.fields.values() if field.manual == manual]
 
 
 _SCHEMA_GROUPS = {
     "Attachment": ("CreateAttachmentDto", "Attachment"),
-    "OrigDatablock": ("CreateOrigDatablockDto", "OrigDatablock"),
+    "OrigDatablock": ("CreateDatasetOrigDatablockDto", "OrigDatablock"),
     "Datablock": ("CreateDatasetDatablockDto", "Datablock"),
     "Lifecycle": (None, "LifecycleClass"),
     "Technique": ("TechniqueClass", "TechniqueClass"),
     "Relationship": ("RelationshipClass", "RelationshipClass"),
     "History": (None, "HistoryClass"),
     "DataFile": ("DataFile", "DataFile"),
     "Instrument": (None, "Instrument"),
```

### Comparing `scitacean-24.4.0/tools/model-generation/spec/dataset-fields.yml` & `scitacean-24.5.0/tools/model-generation/spec/dataset-fields.yml`

 * *Files 14% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 # They are used both for values set by the user of Scitacean and for values downloaded from SCiCat.
 #   func: Function to call on input values.
 #         The return type must be the type of the field (see also field-type-overrides.yml).
 #   arg_type: Type hint for input values.
 conversions:
   creationTime:
     func: _parse_datetime
-    arg_type: Union[str, datetime]
+    arg_type: str | datetime
   pid:
     func: _parse_pid
-    arg_type: Union[PID, str]
+    arg_type: PID | str
   sourceFolder:
     func: _parse_remote_path
-    arg_type: Union[RemotePath, str]
+    arg_type: RemotePath | str
 
 # Mark those fields as read-only in addition to those identified as read only from the schema.
 # Read-only fields must be None in uploads.
 extra_read_only:
   - version
   - pid
```

### Comparing `scitacean-24.4.0/tools/model-generation/spec/field-validations.yml` & `scitacean-24.5.0/tools/model-generation/spec/field-validations.yml`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tools/model-generation/spec/schema.py` & `scitacean-24.5.0/tools/model-generation/spec/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Load schemas from a SciCat API."""
 
 import dataclasses
 from typing import Any
 
-import requests
+import httpx
 
 
 @dataclasses.dataclass
 class SchemaField:
     name: str
     description: str
     type: str
@@ -39,17 +39,17 @@
     if spec["type"] == "string":
         if spec.get("format", "") == "date-time":
             return "datetime"
         return "str"
     if spec["type"] == "boolean":
         return "bool"
     if spec["type"] == "array":
-        return "List[{}]".format(parse_field_type(spec["items"]))
+        return "list[{}]".format(parse_field_type(spec["items"]))
     if spec["type"] == "object":
-        return "Dict[str, Any]"
+        return "dict[str, Any]"
     raise ValueError(f"Unknown field type: {spec['type']}")
 
 
 def parse_schema_fields(spec: dict[str, Any]) -> dict[str, SchemaField]:
     return {
         name: SchemaField(
             name=name,
@@ -72,18 +72,18 @@
 
 def fetch_specs(url: str) -> dict[str, Any]:
     """Download the raw schema JSON from the API.
 
     ``url`` needs to point to a 'json-explorer' of a SciCat backend with version >= 4.
     E.g. ``http://localhost:3000/explorer-json`` for a locally running instance.
     """
-    response = requests.get(url, timeout=10)
-    if not response.ok:
+    response = httpx.get(url, timeout=10)
+    if not response.is_success:
         raise RuntimeError(
-            f"Failed to fetch specs: {response.status_code} {response.reason}"
+            f"Failed to fetch specs: {response.status_code} {response.reason_phrase}"
         )
     return response.json()
 
 
 def load_schemas(url: str) -> dict[str, Schema]:
     spec_json = fetch_specs(url)
     return parse_schemas(spec_json["components"]["schemas"])
```

### Comparing `scitacean-24.4.0/tools/model-generation/templates/__init__.py` & `scitacean-24.5.0/tools/model-generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-24.4.0/tools/model-generation/templates/dataset_fields.py.jinja` & `scitacean-24.5.0/tools/model-generation/templates/dataset_fields.py.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% macro init_arg_type(field) %}
 {%- if field.conversion is none -%}
-    Optional[{{ field.type_for("user")|replace("NonNegativeInt", "int") }}]
+    {{ field.type_for("user")|replace("NonNegativeInt", "int") }} | None
 {%- else -%}
-    Optional[{{ field.conversion.arg_type }}]
+    {{ field.conversion.arg_type }} | None
 {%- endif -%}
 {% endmacro %}
 
 {% macro field_assignment(field) %}
 {%- if field.conversion is none -%}
     self._{{ field.name }} = {{ field.name }}
 {%- else -%}
@@ -28,21 +28,21 @@
 # Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # flake8: noqa
 
 """Base class for Dataset."""
 
 from __future__ import annotations
 
+from dataclasses import dataclass
 from datetime import datetime, timezone
-from typing import Any, Dict, List, Literal, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Literal, TypeVar
 
 import dateutil.parser
 
 from ._base_model import DatasetType
-from ._internal.dataclass_wrapper import dataclass_optional_args
 from .datablock import OrigDatablock
 from .filesystem import RemotePath
 from .model import (
     construct,
     Attachment,
     BaseModel,
     BaseUserModel,
@@ -54,46 +54,46 @@
 )
 from .pid import PID
 
 
 M = TypeVar("M", bound=BaseModel)
 
 
-def _parse_datetime(x: Optional[Union[datetime, str]]) -> Optional[datetime]:
+def _parse_datetime(x: datetime | str | None) -> datetime | None:
     if isinstance(x, datetime) or x is None:
         return x
     if x == "now":
         return datetime.now(tz=timezone.utc)
     return dateutil.parser.parse(x)
 
 
-def _parse_pid(pid: Optional[Union[str, PID]]) -> Optional[PID]:
+def _parse_pid(pid: str | PID | None) -> PID | None:
     if pid is None:
         return pid
     return PID.parse(pid)
 
 
-def _parse_remote_path(path: Optional[Union[str, RemotePath]]) -> Optional[RemotePath]:
+def _parse_remote_path(path: str | RemotePath | None) -> RemotePath | None:
     if path is None:
         return path
     return RemotePath(path)
 
 
-def _validate_checksum_algorithm(algorithm: Optional[str]) -> Optional[str]:
+def _validate_checksum_algorithm(algorithm: str | None) -> str | None:
     if algorithm is None:
         return algorithm
     import hashlib
 
     if algorithm not in hashlib.algorithms_available:
         raise ValueError(f"Checksum algorithm not recognized: {algorithm}")
     return algorithm
 
 
 class DatasetBase:
-    @dataclass_optional_args(frozen=True, kw_only=True, slots=True)
+    @dataclass(frozen=True, kw_only=True, slots=True)
     class Field:
         name: str
         description: str
         read_only: bool
         required: bool
         scicat_name: str
         type: type
@@ -140,114 +140,114 @@
         "_type",
         "_default_checksum_algorithm",
         "_orig_datablocks",
         "_attachments",
     )
 
     def __init__(self,
-        type: Union[DatasetType, Literal["raw", "derived"]],
+        type: DatasetType | Literal["raw", "derived"],
 {%- for field in spec.user_dset_fields(manual=False)|sort(attribute="name")|selectattr("upload") %}
         {{ field.name }}: {{ init_arg_type(field) }} = {{ field.default }},
 {%- endfor %}
-        meta: Optional[Dict[str, Any]] = None,
-        checksum_algorithm: Optional[str] = "blake2b",
+        meta: dict[str, Any] | None = None,
+        checksum_algorithm: str | None = "blake2b",
     ) -> None:
         self._type = DatasetType(type)
 {%- for field in spec.user_dset_fields(manual=False)|sort(attribute="name")|selectattr("upload") %}
         {{ field_assignment(field) }}
 {%- endfor %}
 {%- for field in spec.user_dset_fields(manual=False)|sort(attribute="name")|rejectattr("upload") %}
         self._{{ field.name }} = None
 {%- endfor %}
         self._meta = meta or {}
         self._default_checksum_algorithm = _validate_checksum_algorithm(
             checksum_algorithm
         )
-        self._orig_datablocks: List[OrigDatablock] = []
-        self._attachments: Optional[List[Attachment]] = []
+        self._orig_datablocks: list[OrigDatablock] = []
+        self._attachments: list[Attachment] | None = []
 
 {%- for field in spec.user_dset_fields(manual=False)|sort(attribute="name") %}
     @property
-    def {{ field.name }}(self) -> Optional[{{ field.type_for("user") }}]:
+    def {{ field.name }}(self) -> {{ field.type_for("user") }} | None:
         """{{ field.description }}"""
         return self._{{ field.name }}
 {% if field.upload %}
     @{{ field.name }}.setter
     def {{ field.name }}(self, {{ field.name }}: {{ init_arg_type(field) }}) -> None:
         """{{ field.description }}"""
         {{ field_assignment(field) }}
 {% endif %}
 {%- endfor %}
 
     @property
-    def meta(self) -> Dict[str, Any]:
+    def meta(self) -> dict[str, Any]:
         """Dict of scientific metadata."""
         return self._meta
 
     @meta.setter
-    def meta(self, meta: Dict[str, Any]) -> None:
+    def meta(self, meta: dict[str, Any]) -> None:
         """Dict of scientific metadata."""
         self._meta = meta
 
     @property
     def type(self) -> DatasetType:
         """Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models."""
         return self._type
 
     @staticmethod
     def _prepare_fields_from_download(
         download_model: DownloadDataset
-    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+    ) -> tuple[dict[str, Any], dict[str, Any]]:
         init_args = {}
         read_only = {}
         for field in DatasetBase._FIELD_SPEC:
             if field.read_only:
                 read_only["_"+field.name] = getattr(download_model, field.scicat_name)
             else:
                 init_args[field.name] = getattr(download_model, field.scicat_name)
 
         init_args["meta"] = download_model.scientificMetadata
         _convert_download_fields_in_place(init_args, read_only)
 
         return init_args, read_only
 
     @staticmethod
-    def _convert_readonly_fields_in_place(read_only: Dict[str, Any]) -> None:
+    def _convert_readonly_fields_in_place(read_only: dict[str, Any]) -> None:
     {% for field in spec.user_dset_fields(manual=False)|sort(attribute="name")|selectattr("conversion") %}
         {%- if not field.upload %}
         if ({{ field.name }} := read_only.get("_{{ field.name }}")) is not None:
             read_only["_{{ field.name }}"] = {{ field.conversion.func }}({{ field.name }})
         {%- endif -%}
     {%- endfor %}
 
 
 def _convert_download_fields_in_place(
-    init_args: Dict[str, Any], read_only: Dict[str, Any]
+    init_args: dict[str, Any], read_only: dict[str, Any]
 ) -> None:
     for mod, key in ((Technique, "techniques"), (Relationship, "relationships")):
         init_args[key] = _list_field_from_download(mod, init_args.get(key))
 
     DatasetBase._convert_readonly_fields_in_place(read_only)
     if (lifecycle := read_only.get("_lifecycle")) is not None:
         read_only["_lifecycle"] = Lifecycle.from_download_model(
             _as_model(DownloadLifecycle, lifecycle)
         )
 
 
 def _list_field_from_download(
-    mod: Type[BaseUserModel], value: Optional[List[Any]]
-) -> Optional[List[BaseUserModel]]:
+    mod: type[BaseUserModel], value: list[Any] | None
+) -> list[BaseUserModel] | None:
     if value is None:
         return None
     return [
         mod.from_download_model(_as_model(mod.download_model_type(), item))
         for item in value
     ]
 
 
 # If validation fails, sub models are not converted automatically by Pydantic.
 def _as_model(
-    mod: Type[M], value: Union[M, Dict[str, Any]]
+    mod: type[M], value: M | dict[str, Any]
 ) -> M:
     if isinstance(value, dict):
         return construct(mod, **value, _strict_validation=False)
     return value
```

### Comparing `scitacean-24.4.0/tools/model-generation/templates/model.py.jinja` & `scitacean-24.5.0/tools/model-generation/templates/model.py.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {%- macro validations(fields) %}
-{%- for validation in ("datetime", "drop", "emails", "orcids") %}
+{%- for validation in ("datetime", "emails", "orcids") %}
 {%- set fields = fields|selectattr("validation", "eq", validation)|list -%}
 {% if fields %}
 
     @pydantic.field_validator({{ fields|map("attr", "scicat_name")|map("quote")|join(", ") }}, mode="before")
     def _validate_{{ validation }}(cls, value: Any) -> Any:
         return validate_{{ validation }}(value)
 {%- endif %}
@@ -88,31 +88,30 @@
    :toctree: ../functions
 
    construct
 """
 
 from __future__ import annotations
 
+from dataclasses import dataclass
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Type
+from typing import Any
 
 import pydantic
 from pydantic import NonNegativeInt
 
 from ._base_model import (
     BaseModel,
     BaseUserModel,
     DatasetType,
     construct,
     validate_datetime,
-    validate_drop,
     validate_emails,
     validate_orcids,
 )
-from ._internal.dataclass_wrapper import dataclass_optional_args
 from .filesystem import RemotePath
 from .pid import PID
 from .thumbnail import Thumbnail
 
 {% set fields = dset_spec.fields_for("download") -%}
 class DownloadDataset(BaseModel{{ mask_keyword(dset_spec, "download") }}):
 {%- for field in fields -%}
@@ -138,36 +137,36 @@
 {% for field in fields -%}
 {{ model_field(field, kind) }}
 {%- endfor %}
 {{- validations(fields) }}
 
 {%- if spec.name not in ["DataFile", "Datablock", "OrigDatablock"] %}
     @classmethod
-    def user_model_type(cls) -> Type[{{ spec.name }}]:
+    def user_model_type(cls) -> type[{{ spec.name }}]:
         return {{ spec.name }}
 {%- endif %}
 
 {%- if kind == "download" and spec.upload_name %}
     @classmethod
-    def upload_model_type(cls) -> Type[{{ spec.upload_name }}]:
+    def upload_model_type(cls) -> type[{{ spec.upload_name }}]:
         return {{ spec.upload_name }}
 {%- endif %}
 
 {%- if kind == "upload" %}
     @classmethod
-    def download_model_type(cls) -> Type[{{ spec.download_name }}]:
+    def download_model_type(cls) -> type[{{ spec.download_name }}]:
         return {{ spec.download_name }}
 {%- endif %}
 
 {% endif -%}
 {% endfor -%}
 {% endfor -%}
 
 {% for spec in specs.values()|rejectattr("name", "in", ["DataFile", "Datablock", "OrigDatablock"]) -%}
-@dataclass_optional_args(kw_only=True, slots=True)
+@dataclass(kw_only=True, slots=True)
 class {{ spec.name }}(BaseUserModel):
 {% set fields = spec.fields_for("user")|sort(attribute="upload", reverse=True) -%}
 {% for field in fields %}
     {% if field.upload %}{{ field.name }}{% else %}_{{ field.name }}{% endif %}: {{ field.full_type_for("user") }}{{ field_default(field) }}
 {%- endfor %}
 {% for field in fields|rejectattr("upload") %}
     @property
@@ -182,20 +181,20 @@
     def make_upload_model(self) -> {{ spec.upload_name }}:
         """Construct a SciCat upload model from self."""
         return {{ spec.upload_name }}(**self._upload_model_dict())
 {% endif %}
 
 {%- if spec.upload_name %}
     @classmethod
-    def upload_model_type(cls) -> Type[{{ spec.upload_name }}]:
+    def upload_model_type(cls) -> type[{{ spec.upload_name }}]:
         return {{ spec.upload_name }}
 {%- endif %}
 
     @classmethod
-    def download_model_type(cls) -> Type[{{ spec.download_name }}]:
+    def download_model_type(cls) -> type[{{ spec.download_name }}]:
         return {{ spec.download_name }}
 
 {% endfor -%}
 
 # Some models contain fields that are other models which are defined
 # further down in the file.
 # Instead of ordering models according to their dependencies, resolve
```

### Comparing `scitacean-24.4.0/tox.ini` & `scitacean-24.5.0/tox.ini`

 * *Files identical despite different names*

