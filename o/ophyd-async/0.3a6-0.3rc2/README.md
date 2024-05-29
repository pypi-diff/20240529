# Comparing `tmp/ophyd_async-0.3a6.tar.gz` & `tmp/ophyd_async-0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_async-0.3a6.tar", last modified: Tue May 28 15:21:27 2024, max compression
+gzip compressed data, was "ophyd_async-0.3rc2.tar", last modified: Tue May 28 15:52:55 2024, max compression
```

## Comparing `ophyd_async-0.3a6.tar` & `ophyd_async-0.3rc2.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.627468 ophyd_async-0.3a6/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.595468 ophyd_async-0.3a6/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.595468 ophyd_async-0.3a6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.591468 ophyd_async-0.3a6/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.595468 ophyd_async-0.3a6/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.595468 ophyd_async-0.3a6/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-28 15:21:27.627468 ophyd_async-0.3a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/_templates/README
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/examples/epics_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/examples/foo_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0003-ophyd-async-migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0004-repository-structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0005-respect-black-line-length.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0006-procedural-device-definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/design-goals.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/event-loop-choice.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/flyscanning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/choose-interfaces-for-devices.md
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/compound-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/make-a-simple-device.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/make-a-standard-detector.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/write-tests-for-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/images/bluesky_ophyd_epics_devices_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/images/bluesky_ophyd_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/images/ophyd_favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/tutorials/using-existing-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:21:27.627468 ophyd_async-0.3a6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.591468 ophyd_async-0.3a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/src/ophyd_async/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.607468 ophyd_async-0.3a6/src/ophyd_async/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/mock_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/mock_signal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16456 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/soft_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.607468 ophyd_async-0.3a6/src/ophyd_async/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.607468 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/_aioca.py
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/_p4p.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.607468 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/aravis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/ad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/kinetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/vimba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/_hdffile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/demo/mover.db
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/demo/sensor.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/motion/motor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/pvi/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/pvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/pvi/pvi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/signal/_epics_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/signal/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/panda/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_common_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/panda/writers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/writers/_hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/writers/_panda_hdf_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/plan_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/plan_stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/plan_stubs/ensure_connected.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/plan_stubs/fly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/demo/sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_detector_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_detector_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/src/ophyd_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_device_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_mock_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_soft_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_watchable_async_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/_backend/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_aravis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_kinetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_vimba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/demo/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/demo/test_demo_ad_sim_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/motion/test_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/test_pvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/test_records.db
--rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/test_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/panda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/panda/db/
--rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/db/panda.db
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_panda_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_panda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/plan_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/plan_stubs/test_fly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/protocols/test_protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/sim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/demo/test_sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/test_pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/test_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/test_sim_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/test_streaming_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.876015 ophyd_async-0.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.840015 ophyd_async-0.3rc2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.840015 ophyd_async-0.3rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.832015 ophyd_async-0.3rc2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.840015 ophyd_async-0.3rc2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.840015 ophyd_async-0.3rc2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.840015 ophyd_async-0.3rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-28 15:52:55.876015 ophyd_async-0.3rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.844015 ophyd_async-0.3rc2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.844015 ophyd_async-0.3rc2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/_templates/README
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.844015 ophyd_async-0.3rc2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/examples/epics_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/examples/foo_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.844015 ophyd_async-0.3rc2/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.844015 ophyd_async-0.3rc2/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/decisions/0003-ophyd-async-migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/decisions/0004-repository-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/decisions/0005-respect-black-line-length.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/decisions/0006-procedural-device-definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/design-goals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/event-loop-choice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations/flyscanning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.844015 ophyd_async-0.3rc2/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/how-to/choose-interfaces-for-devices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/how-to/compound-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/how-to/make-a-simple-device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/how-to/make-a-standard-detector.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/how-to/write-tests-for-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.848015 ophyd_async-0.3rc2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/images/bluesky_ophyd_epics_devices_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/images/bluesky_ophyd_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/images/ophyd_favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.848015 ophyd_async-0.3rc2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.848015 ophyd_async-0.3rc2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/tutorials/using-existing-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:52:55.876015 ophyd_async-0.3rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.832015 ophyd_async-0.3rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.848015 ophyd_async-0.3rc2/src/ophyd_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 15:52:55.000000 ophyd_async-0.3rc2/src/ophyd_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.852015 ophyd_async-0.3rc2/src/ophyd_async/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/mock_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/mock_signal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16456 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/soft_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.852015 ophyd_async-0.3rc2/src/ophyd_async/epics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.852015 ophyd_async-0.3rc2/src/ophyd_async/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/_backend/_aioca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/_backend/_p4p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/_backend/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.852015 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/aravis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.856015 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.856015 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/ad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/vimba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.856015 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/_hdffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.856015 ophyd_async-0.3rc2/src/ophyd_async/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/demo/mover.db
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/demo/sensor.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.856015 ophyd_async-0.3rc2/src/ophyd_async/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/motion/motor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.856015 ophyd_async-0.3rc2/src/ophyd_async/epics/pvi/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/pvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/pvi/pvi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.860015 ophyd_async-0.3rc2/src/ophyd_async/epics/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/signal/_epics_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/epics/signal/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.860015 ophyd_async-0.3rc2/src/ophyd_async/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/_common_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.860015 ophyd_async-0.3rc2/src/ophyd_async/panda/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/writers/_hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/panda/writers/_panda_hdf_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.860015 ophyd_async-0.3rc2/src/ophyd_async/plan_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/plan_stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/plan_stubs/ensure_connected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/plan_stubs/fly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.860015 ophyd_async-0.3rc2/src/ophyd_async/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.860015 ophyd_async-0.3rc2/src/ophyd_async/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/sim/demo/sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/sim/pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/sim/sim_pattern_detector_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/sim/sim_pattern_detector_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/src/ophyd_async/sim/sim_pattern_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.872015 ophyd_async-0.3rc2/src/ophyd_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-28 15:52:55.000000 ophyd_async-0.3rc2/src/ophyd_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-05-28 15:52:55.000000 ophyd_async-0.3rc2/src/ophyd_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:52:55.000000 ophyd_async-0.3rc2/src/ophyd_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 15:52:55.000000 ophyd_async-0.3rc2/src/ophyd_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 15:52:55.000000 ophyd_async-0.3rc2/src/ophyd_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 15:52:55.000000 ophyd_async-0.3rc2/src/ophyd_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.860015 ophyd_async-0.3rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.864015 ophyd_async-0.3rc2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_device_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12530 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_mock_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_soft_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/core/test_watchable_async_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.864015 ophyd_async-0.3rc2/tests/epics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.864015 ophyd_async-0.3rc2/tests/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/_backend/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.868015 ophyd_async-0.3rc2/tests/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_aravis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_vimba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/areadetector/test_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.868015 ophyd_async-0.3rc2/tests/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/demo/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/demo/test_demo_ad_sim_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.868015 ophyd_async-0.3rc2/tests/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/motion/test_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/test_pvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/test_records.db
+-rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/epics/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.868015 ophyd_async-0.3rc2/tests/panda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.868015 ophyd_async-0.3rc2/tests/panda/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/panda/db/panda.db
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/panda/test_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/panda/test_panda_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/panda/test_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/panda/test_panda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/panda/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/panda/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/panda/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.868015 ophyd_async-0.3rc2/tests/plan_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/plan_stubs/test_fly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.868015 ophyd_async-0.3rc2/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/protocols/test_protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.872015 ophyd_async-0.3rc2/tests/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/sim/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:55.872015 ophyd_async-0.3rc2/tests/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/sim/demo/test_sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/sim/test_pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/sim/test_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/sim/test_sim_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/sim/test_streaming_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-28 15:52:50.000000 ophyd_async-0.3rc2/tests/test_log.py
```

### Comparing `ophyd_async-0.3a6/.devcontainer/devcontainer.json` & `ophyd_async-0.3rc2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/CONTRIBUTING.md` & `ophyd_async-0.3rc2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/actions/install_requirements/action.yml` & `ophyd_async-0.3rc2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/dependabot.yml` & `ophyd_async-0.3rc2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/pages/make_switcher.py` & `ophyd_async-0.3rc2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/workflows/_check.yml` & `ophyd_async-0.3rc2/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/workflows/_dist.yml` & `ophyd_async-0.3rc2/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/workflows/_docs.yml` & `ophyd_async-0.3rc2/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/workflows/_release.yml` & `ophyd_async-0.3rc2/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/workflows/_test.yml` & `ophyd_async-0.3rc2/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.github/workflows/ci.yml` & `ophyd_async-0.3rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.gitignore` & `ophyd_async-0.3rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.mailmap` & `ophyd_async-0.3rc2/.mailmap`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/.pre-commit-config.yaml` & `ophyd_async-0.3rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/Dockerfile` & `ophyd_async-0.3rc2/Dockerfile`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/LICENSE` & `ophyd_async-0.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/PKG-INFO` & `ophyd_async-0.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a6
+Version: 0.3rc2
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ophyd_async-0.3a6/README.md` & `ophyd_async-0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/_templates/custom-class-template.rst` & `ophyd_async-0.3rc2/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/_templates/custom-module-template.rst` & `ophyd_async-0.3rc2/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/conf.py` & `ophyd_async-0.3rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/examples/epics_demo.py` & `ophyd_async-0.3rc2/docs/examples/epics_demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/examples/foo_detector.py` & `ophyd_async-0.3rc2/docs/examples/foo_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `ophyd_async-0.3rc2/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/explanations/decisions/0003-ophyd-async-migration.rst` & `ophyd_async-0.3rc2/docs/explanations/decisions/0003-ophyd-async-migration.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/explanations/decisions/0004-repository-structure.rst` & `ophyd_async-0.3rc2/docs/explanations/decisions/0004-repository-structure.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/explanations/decisions/0005-respect-black-line-length.rst` & `ophyd_async-0.3rc2/docs/explanations/decisions/0005-respect-black-line-length.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/explanations/decisions/0006-procedural-device-definitions.rst` & `ophyd_async-0.3rc2/docs/explanations/decisions/0006-procedural-device-definitions.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/explanations/design-goals.rst` & `ophyd_async-0.3rc2/docs/explanations/design-goals.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/explanations/event-loop-choice.rst` & `ophyd_async-0.3rc2/docs/explanations/event-loop-choice.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/explanations/flyscanning.rst` & `ophyd_async-0.3rc2/docs/explanations/flyscanning.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/how-to/choose-interfaces-for-devices.md` & `ophyd_async-0.3rc2/docs/how-to/choose-interfaces-for-devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/how-to/compound-devices.rst` & `ophyd_async-0.3rc2/docs/how-to/compound-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/how-to/make-a-simple-device.rst` & `ophyd_async-0.3rc2/docs/how-to/make-a-simple-device.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/how-to/make-a-standard-detector.rst` & `ophyd_async-0.3rc2/docs/how-to/make-a-standard-detector.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/how-to/write-tests-for-devices.rst` & `ophyd_async-0.3rc2/docs/how-to/write-tests-for-devices.rst`

 * *Files 13% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 
 In addition this example also utilizes helper functions like ``assert_reading`` and ``assert_value`` to ensure the validity of device readings and values. For more information see: :doc:`API.core<../generated/ophyd_async.core>`
 
 .. literalinclude:: ../../tests/epics/demo/test_demo.py
    :pyobject: test_sensor_reading_shows_value
 
 
+Given that the mock signal holds a ``unittest.mock.Mock`` object you can retrieve this object and assert that the device has been set correctly using ``get_mock_put``. You are also free to use any other behaviour that ``unittest.mock.Mock`` provides, such as in this example which sets the parent of the mock to allow ordering across signals to be asserted:
+
+.. literalinclude:: ../../tests/epics/demo/test_demo.py
+   :pyobject: test_retrieve_mock_and_assert
+
 There are several other test utility functions:
 
 Use ``callback_on_mock_put``, for hooking in logic when a mock value changes (e.g. because someone puts to it). This can be called directly, or used as a context, with the callbacks ending after exit.
 
 .. literalinclude:: ../../tests/epics/demo/test_demo.py
    :pyobject: test_mover_stopped
```

### Comparing `ophyd_async-0.3a6/docs/images/bluesky_ophyd_epics_devices_logo.svg` & `ophyd_async-0.3rc2/docs/images/bluesky_ophyd_epics_devices_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/images/bluesky_ophyd_logo.svg` & `ophyd_async-0.3rc2/docs/images/bluesky_ophyd_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/images/ophyd_favicon.svg` & `ophyd_async-0.3rc2/docs/images/ophyd_favicon.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/index.md` & `ophyd_async-0.3rc2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/reference/api.rst` & `ophyd_async-0.3rc2/docs/reference/api.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/tutorials/installation.md` & `ophyd_async-0.3rc2/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/docs/tutorials/using-existing-devices.rst` & `ophyd_async-0.3rc2/docs/tutorials/using-existing-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/pyproject.toml` & `ophyd_async-0.3rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/__init__.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,18 @@
     load_from_yaml,
     save_device,
     save_to_yaml,
     set_signal_values,
     walk_rw_signals,
 )
 from .flyer import HardwareTriggeredFlyable, TriggerLogic
-from .mock_signal_backend import (
-    MockSignalBackend,
-)
+from .mock_signal_backend import MockSignalBackend
 from .mock_signal_utils import (
-    assert_mock_put_called_with,
     callback_on_mock_put,
+    get_mock_put,
     mock_puts_blocked,
     reset_mock_put_calls,
     set_mock_put_proceeds,
     set_mock_value,
     set_mock_values,
 )
 from .signal import (
@@ -66,15 +64,15 @@
     get_dtype,
     get_unique,
     merge_gathered_dicts,
     wait_for_connection,
 )
 
 __all__ = [
-    "assert_mock_put_called_with",
+    "get_mock_put",
     "callback_on_mock_put",
     "mock_puts_blocked",
     "set_mock_values",
     "reset_mock_put_calls",
     "SignalBackend",
     "SoftSignalBackend",
     "DetectorControl",
```

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/_providers.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/_providers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/async_status.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/async_status.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/detector.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/device.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/device.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/device_save_loader.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/flyer.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/flyer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/mock_signal_backend.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/mock_signal_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import asyncio
 from functools import cached_property
-from typing import Optional, Type
+from typing import Callable, Optional, Type
 from unittest.mock import Mock
 
 from bluesky.protocols import Descriptor, Reading
 
 from ophyd_async.core.signal_backend import SignalBackend
 from ophyd_async.core.soft_signal_backend import SoftSignalBackend
 from ophyd_async.core.utils import DEFAULT_TIMEOUT, ReadingValueCallback, T
 
 
-class MockSignalBackend(SignalBackend):
+class MockSignalBackend(SignalBackend[T]):
     def __init__(
         self,
         datatype: Optional[Type[T]] = None,
         initial_backend: Optional[SignalBackend[T]] = None,
     ) -> None:
         if isinstance(initial_backend, MockSignalBackend):
             raise ValueError("Cannot make a MockSignalBackend for a MockSignalBackends")
@@ -27,31 +27,31 @@
             ), "Must supply either initial_backend or datatype"
             datatype = self.initial_backend.datatype
 
         self.datatype = datatype
 
         if not isinstance(self.initial_backend, SoftSignalBackend):
             # If the backend is a hard signal backend, or not provided,
-            # then we create a soft signal to mimick it
+            # then we create a soft signal to mimic it
 
             self.soft_backend = SoftSignalBackend(datatype=datatype)
         else:
-            self.soft_backend = initial_backend
+            self.soft_backend = self.initial_backend
 
     def source(self, name: str) -> str:
         if self.initial_backend:
             return f"mock+{self.initial_backend.source(name)}"
         return f"mock+{name}"
 
     async def connect(self, timeout: float = DEFAULT_TIMEOUT) -> None:
         pass
 
     @cached_property
     def put_mock(self) -> Mock:
-        return Mock(name="put")
+        return Mock(name="put", spec=Callable)
 
     @cached_property
     def put_proceeds(self) -> asyncio.Event:
         put_proceeds = asyncio.Event()
         put_proceeds.set()
         return put_proceeds
 
@@ -61,17 +61,14 @@
 
         if wait:
             await asyncio.wait_for(self.put_proceeds.wait(), timeout=timeout)
 
     def set_value(self, value: T):
         self.soft_backend.set_value(value)
 
-    async def get_descriptor(self, source: str) -> Descriptor:
-        return await self.soft_backend.get_descriptor(source)
-
     async def get_reading(self) -> Reading:
         return await self.soft_backend.get_reading()
 
     async def get_value(self) -> T:
         return await self.soft_backend.get_value()
 
     async def get_setpoint(self) -> T:
```

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/mock_signal_utils.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/mock_signal_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextlib import asynccontextmanager, contextmanager
-from typing import Any, Callable, Iterable, Iterator, List
-from unittest.mock import ANY, Mock
+from typing import Any, Callable, Iterable
+from unittest.mock import Mock
 
 from ophyd_async.core.signal import Signal
 from ophyd_async.core.utils import T
 
 from .mock_signal_backend import MockSignalBackend
 
 
@@ -18,36 +18,36 @@
 
 def set_mock_value(signal: Signal[T], value: T):
     """Set the value of a signal that is in mock mode."""
     backend = _get_mock_signal_backend(signal)
     backend.set_value(value)
 
 
-def set_mock_put_proceeds(signal: Signal[T], proceeds: bool):
+def set_mock_put_proceeds(signal: Signal, proceeds: bool):
     """Allow or block a put with wait=True from proceeding"""
     backend = _get_mock_signal_backend(signal)
 
     if proceeds:
         backend.put_proceeds.set()
     else:
         backend.put_proceeds.clear()
 
 
 @asynccontextmanager
-async def mock_puts_blocked(*signals: List[Signal]):
+async def mock_puts_blocked(*signals: Signal):
     for signal in signals:
         set_mock_put_proceeds(signal, False)
     yield
     for signal in signals:
         set_mock_put_proceeds(signal, True)
 
 
-def assert_mock_put_called_with(signal: Signal, value: Any, wait=ANY, timeout=ANY):
-    backend = _get_mock_signal_backend(signal)
-    backend.put_mock.assert_called_with(value, wait=wait, timeout=timeout)
+def get_mock_put(signal: Signal) -> Mock:
+    """Get the mock associated with the put call on the signal."""
+    return _get_mock_signal_backend(signal).put_mock
 
 
 def reset_mock_put_calls(signal: Signal):
     backend = _get_mock_signal_backend(signal)
     backend.put_mock.reset_mock()
 
 
@@ -75,23 +75,23 @@
     def __next__(self):
         # Will propogate StopIteration
         self.index, next_value = next(self.iterator)
         set_mock_value(self.signal, next_value)
         return next_value
 
     def __del__(self):
-        if self.require_all_consumed and self.index != len(self.values):
+        if self.require_all_consumed and self.index != len(list(self.values)):
             raise AssertionError("Not all values have been consumed.")
 
 
 def set_mock_values(
     signal: Signal,
     values: Iterable[Any],
     require_all_consumed: bool = False,
-) -> Iterator[Any]:
+) -> _SetValuesIterator:
     """Iterator to set a signal to a sequence of values, optionally repeating the
     sequence.
 
     Parameters
     ----------
     signal:
         A signal with a `MockSignalBackend` backend.
@@ -123,15 +123,15 @@
 
 @contextmanager
 def _unset_side_effect_cm(put_mock: Mock):
     yield
     put_mock.side_effect = None
 
 
-def callback_on_mock_put(signal: Signal, callback: Callable[[T], None]):
+def callback_on_mock_put(signal: Signal[T], callback: Callable[[T], None]):
     """For setting a callback when a backend is put to.
 
     Can either be used in a context, with the callback being
     unset on exit, or as an ordinary function.
 
     Parameters
     ----------
```

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/signal.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/signal.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/signal_backend.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/signal_backend.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """A read/write/monitor backend for a Signals"""
 
     #: Datatype of the signal value
     datatype: Optional[Type[T]] = None
 
     #: Like ca://PV_PREFIX:SIGNAL
     @abstractmethod
-    def source(name: str) -> str:
+    def source(self, name: str) -> str:
         """Return source of signal. Signals may pass a name to the backend, which can be
         used or discarded."""
 
     @abstractmethod
     async def connect(self, timeout: float = DEFAULT_TIMEOUT):
         """Connect to underlying hardware"""
```

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/soft_signal_backend.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/soft_signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/standard_readable.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/standard_readable.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/core/utils.py` & `ophyd_async-0.3rc2/src/ophyd_async/core/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/_backend/_aioca.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/_backend/_aioca.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/_backend/_p4p.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/_backend/_p4p.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/_backend/common.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/_backend/common.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/aravis.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/aravis.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/ad_base.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/ad_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/kinetix.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/kinetix.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/pilatus.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/pilatus.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/single_trigger_det.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/utils.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/vimba.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/vimba.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/_hdffile.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/_hdffile.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/hdf_writer.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/hdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/nd_plugin.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/areadetector/writers/nd_plugin.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/demo/__init__.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/demo/demo_ad_sim_detector.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/demo/demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/demo/mover.db` & `ophyd_async-0.3rc2/src/ophyd_async/epics/demo/mover.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/demo/sensor.db` & `ophyd_async-0.3rc2/src/ophyd_async/epics/demo/sensor.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/motion/motor.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/motion/motor.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/pvi/pvi.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/pvi/pvi.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/signal/_epics_transport.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/signal/_epics_transport.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/epics/signal/signal.py` & `ophyd_async-0.3rc2/src/ophyd_async/epics/signal/signal.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/log.py` & `ophyd_async-0.3rc2/src/ophyd_async/log.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/panda/__init__.py` & `ophyd_async-0.3rc2/src/ophyd_async/panda/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/panda/_common_blocks.py` & `ophyd_async-0.3rc2/src/ophyd_async/panda/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/panda/_hdf_panda.py` & `ophyd_async-0.3rc2/src/ophyd_async/panda/_hdf_panda.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/panda/_panda_controller.py` & `ophyd_async-0.3rc2/src/ophyd_async/panda/_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/panda/_table.py` & `ophyd_async-0.3rc2/src/ophyd_async/panda/_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/panda/_trigger.py` & `ophyd_async-0.3rc2/src/ophyd_async/panda/_trigger.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/panda/writers/_hdf_writer.py` & `ophyd_async-0.3rc2/src/ophyd_async/panda/writers/_hdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/panda/writers/_panda_hdf_file.py` & `ophyd_async-0.3rc2/src/ophyd_async/panda/writers/_panda_hdf_file.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/plan_stubs/ensure_connected.py` & `ophyd_async-0.3rc2/src/ophyd_async/plan_stubs/ensure_connected.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/plan_stubs/fly.py` & `ophyd_async-0.3rc2/src/ophyd_async/plan_stubs/fly.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/protocols.py` & `ophyd_async-0.3rc2/src/ophyd_async/protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/sim/demo/sim_motor.py` & `ophyd_async-0.3rc2/src/ophyd_async/sim/demo/sim_motor.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/sim/pattern_generator.py` & `ophyd_async-0.3rc2/src/ophyd_async/sim/pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_detector_control.py` & `ophyd_async-0.3rc2/src/ophyd_async/sim/sim_pattern_detector_control.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_detector_writer.py` & `ophyd_async-0.3rc2/src/ophyd_async/sim/sim_pattern_detector_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_generator.py` & `ophyd_async-0.3rc2/src/ophyd_async/sim/sim_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async.egg-info/PKG-INFO` & `ophyd_async-0.3rc2/src/ophyd_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a6
+Version: 0.3rc2
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ophyd_async-0.3a6/src/ophyd_async.egg-info/SOURCES.txt` & `ophyd_async-0.3rc2/src/ophyd_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/src/ophyd_async.egg-info/requires.txt` & `ophyd_async-0.3rc2/src/ophyd_async.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/conftest.py` & `ophyd_async-0.3rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_async_status.py` & `ophyd_async-0.3rc2/tests/core/test_async_status.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_device.py` & `ophyd_async-0.3rc2/tests/core/test_device.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_device_collector.py` & `ophyd_async-0.3rc2/tests/core/test_device_collector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_device_save_loader.py` & `ophyd_async-0.3rc2/tests/core/test_device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_flyer.py` & `ophyd_async-0.3rc2/tests/core/test_flyer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_mock_signal_backend.py` & `ophyd_async-0.3rc2/tests/core/test_mock_signal_backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 import asyncio
 import re
 from itertools import repeat
-from unittest.mock import MagicMock, call
+from unittest.mock import ANY, MagicMock, call
 
 import pytest
 
 from ophyd_async.core import MockSignalBackend, SignalRW
 from ophyd_async.core.device import Device, DeviceCollector
 from ophyd_async.core.mock_signal_utils import (
-    assert_mock_put_called_with,
     callback_on_mock_put,
+    get_mock_put,
     mock_puts_blocked,
     reset_mock_put_calls,
     set_mock_put_proceeds,
     set_mock_value,
     set_mock_values,
 )
-from ophyd_async.core.signal import (
-    SignalW,
-    soft_signal_r_and_setter,
-    soft_signal_rw,
-)
+from ophyd_async.core.signal import SignalW, soft_signal_r_and_setter, soft_signal_rw
 from ophyd_async.core.soft_signal_backend import SoftSignalBackend
 from ophyd_async.epics.signal.signal import epics_signal_r, epics_signal_rw
 
 
 @pytest.mark.parametrize("connect_mock_mode", [True, False])
 async def test_mock_signal_backend(connect_mock_mode):
     mock_signal = SignalRW(MockSignalBackend(datatype=str))
     # If mock is false it will be handled like a normal signal, otherwise it will
     # initalize a new backend from the one in the line above
     await mock_signal.connect(mock=connect_mock_mode)
+    assert isinstance(mock_signal._backend, MockSignalBackend)
 
     assert await mock_signal._backend.get_value() == ""
     await mock_signal._backend.put("test")
     assert await mock_signal._backend.get_value() == "test"
     assert mock_signal._backend.put_mock.call_args_list == [
         call("test", wait=True, timeout=None),
     ]
@@ -70,14 +67,16 @@
     assert await mock_signal._backend.get_value() == 10
 
 
 async def test_set_mock_put_proceeds():
     mock_signal = SignalW(SoftSignalBackend(str))
     await mock_signal.connect(mock=True)
 
+    assert isinstance(mock_signal._backend, MockSignalBackend)
+
     assert mock_signal._backend.put_proceeds.is_set() is True
 
     set_mock_put_proceeds(mock_signal, False)
     assert mock_signal._backend.put_proceeds.is_set() is False
     set_mock_put_proceeds(mock_signal, True)
     assert mock_signal._backend.put_proceeds.is_set() is True
 
@@ -91,14 +90,15 @@
     with pytest.raises(asyncio.exceptions.TimeoutError):
         await mock_signal.set("test", wait=True, timeout=1)
 
 
 async def test_put_proceeds_timeout():
     mock_signal = SignalW(SoftSignalBackend(str))
     await mock_signal.connect(mock=True)
+    assert isinstance(mock_signal._backend, MockSignalBackend)
 
     assert mock_signal._backend.put_proceeds.is_set() is True
 
     set_mock_put_proceeds(mock_signal, False)
     assert mock_signal._backend.put_proceeds.is_set() is False
     set_mock_put_proceeds(mock_signal, True)
     assert mock_signal._backend.put_proceeds.is_set() is True
@@ -108,22 +108,22 @@
     signal = SignalRW(SoftSignalBackend(int))
 
     exc_msgs = []
     with pytest.raises(AssertionError) as exc:
         set_mock_value(signal, 10)
     exc_msgs.append(str(exc.value))
     with pytest.raises(AssertionError) as exc:
-        assert_mock_put_called_with(signal, 10)
+        get_mock_put(signal).assert_called_once_with(10)
     exc_msgs.append(str(exc.value))
     with pytest.raises(AssertionError) as exc:
-        async with mock_puts_blocked(signal, 10):
+        async with mock_puts_blocked(signal):
             ...
     exc_msgs.append(str(exc.value))
     with pytest.raises(AssertionError) as exc:
-        with callback_on_mock_put(signal, 10):
+        with callback_on_mock_put(signal, lambda x: _):
             ...
     exc_msgs.append(str(exc.value))
     with pytest.raises(AssertionError) as exc:
         set_mock_put_proceeds(signal, False)
     exc_msgs.append(str(exc.value))
     with pytest.raises(AssertionError) as exc:
         for _ in set_mock_values(signal, [10]):
@@ -133,24 +133,21 @@
     for msg in exc_msgs:
         assert msg == (
             "Expected to receive a `MockSignalBackend`, instead "
             f" received {SoftSignalBackend}. "
         )
 
 
-async def test_assert_mock_put_called_with():
+async def test_get_mock_put():
     mock_signal = epics_signal_rw(str, "READ_PV", "WRITE_PV", name="mock_name")
     await mock_signal.connect(mock=True)
     await mock_signal.set("test_value", wait=True, timeout=100)
 
-    # can leave out kwargs
-    assert_mock_put_called_with(mock_signal, "test_value")
-    assert_mock_put_called_with(mock_signal, "test_value", wait=True)
-    assert_mock_put_called_with(mock_signal, "test_value", timeout=100)
-    assert_mock_put_called_with(mock_signal, "test_value", wait=True, timeout=100)
+    mock = get_mock_put(mock_signal)
+    mock.assert_called_once_with("test_value", wait=True, timeout=100)
 
     def err_text(text, wait, timeout):
         return (
             f"Expected: put('{re.escape(str(text))}', wait={re.escape(str(wait))},"
             f" timeout={re.escape(str(timeout))})",
             "Actual: put('test_value', wait=True, timeout=100)",
         )
@@ -158,15 +155,15 @@
     for text, wait, timeout in [
         ("wrong_name", True, 100),  # name wrong
         ("test_value", False, 100),  # wait wrong
         ("test_value", True, 0),  # timeout wrong
         ("test_value", False, 0),  # wait and timeout wrong
     ]:
         with pytest.raises(AssertionError) as exc:
-            assert_mock_put_called_with(mock_signal, text, wait=wait, timeout=timeout)
+            mock.assert_called_once_with(text, wait=wait, timeout=timeout)
         for err_substr in err_text(text, wait, timeout):
             assert err_substr in str(exc.value)
 
 
 @pytest.fixture
 async def mock_signals():
     async with DeviceCollector(mock=True):
@@ -212,18 +209,16 @@
     signal2_callbacks.assert_called_once_with("second_value", wait=True, timeout=1)
 
 
 async def test_callback_on_mock_put_no_ctx():
     mock_signal = SignalRW(SoftSignalBackend(float))
     await mock_signal.connect(mock=True)
     calls = []
-    (
-        callback_on_mock_put(
-            mock_signal, lambda *args, **kwargs: calls.append({**kwargs, "_args": args})
-        ),
+    callback_on_mock_put(
+        mock_signal, lambda *args, **kwargs: calls.append({**kwargs, "_args": args})
     )
     await mock_signal.set(10.0)
     assert calls == [
         {
             "_args": (10.0,),
             "timeout": 10.0,
             "wait": True,
@@ -245,24 +240,24 @@
         "some_function_without_kwargs() got an unexpected keyword argument 'wait'"
     )
 
 
 async def test_set_mock_values(mock_signals):
     signal1, signal2 = mock_signals
 
-    await signal2.get_value() == "first_value"
+    assert await signal2.get_value() == "first_value"
     for value_set in set_mock_values(signal1, ["second_value", "third_value"]):
         assert await signal1.get_value() == value_set
 
     iterator = set_mock_values(signal2, ["second_value", "third_value"])
-    await signal2.get_value() == "first_value"
+    assert await signal2.get_value() == "first_value"
     next(iterator)
-    await signal2.get_value() == "second_value"
+    assert await signal2.get_value() == "second_value"
     next(iterator)
-    await signal2.get_value() == "third_value"
+    assert await signal2.get_value() == "third_value"
 
 
 async def test_set_mock_values_exhausted_passes(mock_signals):
     signal1, signal2 = mock_signals
     for value_set in set_mock_values(
         signal1, ["second_value", "third_value"], require_all_consumed=True
     ):
@@ -296,18 +291,18 @@
     # Set so it doesn't raise the same error on teardown
     iterator.require_all_consumed = False
 
 
 async def test_reset_mock_put_calls(mock_signals):
     signal1, signal2 = mock_signals
     await signal1.set("test_value", wait=True, timeout=1)
-    assert_mock_put_called_with(signal1, "test_value")
+    get_mock_put(signal1).assert_called_with("test_value", wait=ANY, timeout=ANY)
     reset_mock_put_calls(signal1)
     with pytest.raises(AssertionError) as exc:
-        assert_mock_put_called_with(signal1, "test_value")
+        get_mock_put(signal1).assert_called_with("test_value", wait=ANY, timeout=ANY)
     # Replacing spaces because they change between runners
     # (e.g the github actions runner has more)
     assert str(exc.value).replace(" ", "").replace("\n", "") == (
         "expectedcallnotfound."
         "Expected:put('test_value',wait=<ANY>,timeout=<ANY>)"
         "Actual:notcalled."
     )
@@ -346,7 +341,17 @@
     assert await device.signal.get_value() == 1
 
     signal, backend_put = soft_signal_r_and_setter(int)
     await signal.connect(mock=False)
     assert await signal.get_value() == 0
     backend_put(100)
     assert await signal.get_value() == 100
+
+
+async def test_when_put_mock_called_with_typo_then_fails_but_calling_directly_passes():
+    mock_signal = SignalRW(SoftSignalBackend(int))
+    await mock_signal.connect(mock=True)
+    assert isinstance(mock_signal._backend, MockSignalBackend)
+    mock = mock_signal._backend.put_mock
+    with pytest.raises(AttributeError):
+        mock.asssert_called_once()  # Note typo here is deliberate!
+    mock()
```

### Comparing `ophyd_async-0.3a6/tests/core/test_signal.py` & `ophyd_async-0.3rc2/tests/core/test_signal.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_soft_signal_backend.py` & `ophyd_async-0.3rc2/tests/core/test_soft_signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_standard_readable.py` & `ophyd_async-0.3rc2/tests/core/test_standard_readable.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_utils.py` & `ophyd_async-0.3rc2/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/core/test_watchable_async_status.py` & `ophyd_async-0.3rc2/tests/core/test_watchable_async_status.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/_backend/test_common.py` & `ophyd_async-0.3rc2/tests/epics/_backend/test_common.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_aravis.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_aravis.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_controllers.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_controllers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_drivers.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_drivers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_kinetix.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_kinetix.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_pilatus.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_pilatus.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_scans.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_single_trigger_det.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_utils.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_vimba.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_vimba.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/areadetector/test_writers.py` & `ophyd_async-0.3rc2/tests/epics/areadetector/test_writers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/demo/test_demo.py` & `ophyd_async-0.3rc2/tests/epics/demo/test_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ophyd_async.core import (
     DeviceCollector,
     NotConnected,
     assert_emitted,
     assert_reading,
     assert_value,
     callback_on_mock_put,
+    get_mock_put,
     set_mock_value,
 )
 from ophyd_async.epics import demo
 
 # Long enough for multiple asyncio event loop cycles to run so
 # all the tasks have a chance to run
 A_WHILE = 0.001
@@ -172,14 +173,37 @@
                 "timestamp": ANY,
                 "alarm_severity": 0,
             }
         },
     )
 
 
+async def test_retrieve_mock_and_assert(mock_mover: demo.Mover):
+    mover_setpoint_mock = get_mock_put(mock_mover.setpoint)
+    await mock_mover.setpoint.set(10)
+    mover_setpoint_mock.assert_called_once_with(10, wait=ANY, timeout=ANY)
+
+    # Assert that velocity is set before move
+    mover_velocity_mock = get_mock_put(mock_mover.velocity)
+
+    parent_mock = Mock()
+    parent_mock.attach_mock(mover_setpoint_mock, "setpoint")
+    parent_mock.attach_mock(mover_velocity_mock, "velocity")
+
+    await mock_mover.velocity.set(100)
+    await mock_mover.setpoint.set(67)
+
+    parent_mock.assert_has_calls(
+        [
+            call.velocity(100, wait=True, timeout=ANY),
+            call.setpoint(67, wait=True, timeout=ANY),
+        ]
+    )
+
+
 async def test_read_mover(mock_mover: demo.Mover):
     await mock_mover.stage()
     assert (await mock_mover.read())["mock_mover"]["value"] == 0.0
     assert (await mock_mover.read_configuration())["mock_mover-velocity"]["value"] == 1
     assert (await mock_mover.describe_configuration())["mock_mover-units"][
         "shape"
     ] == []
```

### Comparing `ophyd_async-0.3a6/tests/epics/demo/test_demo_ad_sim_detector.py` & `ophyd_async-0.3rc2/tests/epics/demo/test_demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/motion/test_motor.py` & `ophyd_async-0.3rc2/tests/epics/motion/test_motor.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/test_pvi.py` & `ophyd_async-0.3rc2/tests/epics/test_pvi.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/test_records.db` & `ophyd_async-0.3rc2/tests/epics/test_records.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/epics/test_signals.py` & `ophyd_async-0.3rc2/tests/epics/test_signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/panda/db/panda.db` & `ophyd_async-0.3rc2/tests/panda/db/panda.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/panda/test_hdf_panda.py` & `ophyd_async-0.3rc2/tests/panda/test_hdf_panda.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/panda/test_panda_connect.py` & `ophyd_async-0.3rc2/tests/panda/test_panda_connect.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/panda/test_panda_controller.py` & `ophyd_async-0.3rc2/tests/panda/test_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/panda/test_panda_utils.py` & `ophyd_async-0.3rc2/tests/panda/test_panda_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/panda/test_table.py` & `ophyd_async-0.3rc2/tests/panda/test_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/panda/test_trigger.py` & `ophyd_async-0.3rc2/tests/panda/test_trigger.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/panda/test_writer.py` & `ophyd_async-0.3rc2/tests/panda/test_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/plan_stubs/test_fly.py` & `ophyd_async-0.3rc2/tests/plan_stubs/test_fly.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/protocols/test_protocols.py` & `ophyd_async-0.3rc2/tests/protocols/test_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/sim/demo/test_sim_motor.py` & `ophyd_async-0.3rc2/tests/sim/demo/test_sim_motor.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/sim/test_pattern_generator.py` & `ophyd_async-0.3rc2/tests/sim/test_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/sim/test_sim_detector.py` & `ophyd_async-0.3rc2/tests/sim/test_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/sim/test_sim_writer.py` & `ophyd_async-0.3rc2/tests/sim/test_sim_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/sim/test_streaming_plan.py` & `ophyd_async-0.3rc2/tests/sim/test_streaming_plan.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a6/tests/test_log.py` & `ophyd_async-0.3rc2/tests/test_log.py`

 * *Files identical despite different names*

