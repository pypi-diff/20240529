# Comparing `tmp/eradiate-0.27.0rc0.tar.gz` & `tmp/eradiate-0.27.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eradiate-0.27.0rc0.tar", last modified: Wed Apr 24 16:13:37 2024, max compression
+gzip compressed data, was "eradiate-0.27.0rc1.tar", last modified: Mon Apr 29 15:08:02 2024, max compression
```

## Comparing `eradiate-0.27.0rc0.tar` & `eradiate-0.27.0rc1.tar`

### file list

```diff
@@ -1,642 +1,689 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.032335 eradiate-0.27.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.932334 eradiate-0.27.0rc0/.devcontainer/
--rwxr-xr-x   0 runner    (1001) docker     (127)      135 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.devcontainer/create-command.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.932334 eradiate-0.27.0rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.932334 eradiate-0.27.0rc0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.932334 eradiate-0.27.0rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-04-24 16:13:37.032335 eradiate-0.27.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.936334 eradiate-0.27.0rc0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.936334 eradiate-0.27.0rc0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_ext/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_ext/pluginparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.936334 eradiate-0.27.0rc0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (127)    17013 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    32795 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-black.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25531 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-darkgrey.png
--rw-r--r--   0 runner    (1001) docker     (127)    34059 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-darkgrey.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    34061 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.920334 eradiate-0.27.0rc0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.940334 eradiate-0.27.0rc0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.940334 eradiate-0.27.0rc0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/_templates/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/convert_figures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.948335 eradiate-0.27.0rc0/docs/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    20540 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/atmosphere_attributes.png
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/atmosphere_attributes.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28149 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-east_left.png
--rw-r--r--   0 runner    (1001) docker     (127)    32937 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-east_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28852 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-east_right.png
--rw-r--r--   0 runner    (1001) docker     (127)    35278 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-east_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-north_left.png
--rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-north_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28115 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-north_right.png
--rw-r--r--   0 runner    (1001) docker     (127)    32455 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-north_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28153 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-south_left.png
--rw-r--r--   0 runner    (1001) docker     (127)    32939 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-south_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28118 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-south_right.png
--rw-r--r--   0 runner    (1001) docker     (127)    32455 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-south_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28178 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-west_left.png
--rw-r--r--   0 runner    (1001) docker     (127)    32935 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-west_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-west_right.png
--rw-r--r--   0 runner    (1001) docker     (127)    32437 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/azimuth-west_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/cartesian-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/cartesian-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25301 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/cuboid_leaf_cloud_params.png
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/cuboid_leaf_cloud_params.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.948335 eradiate-0.27.0rc0/docs/fig/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/diagrams/class_diagram_biosphere.drawio
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
--rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/diagrams/package.drawio
--rw-r--r--   0 runner    (1001) docker     (127)    40438 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/eradiate-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/icon_eradiate.png
--rw-r--r--   0 runner    (1001) docker     (127)    38873 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/package.png
--rw-r--r--   0 runner    (1001) docker     (127)    57417 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/package.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32384 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/radiancemeter_hsphere.png
--rw-r--r--   0 runner    (1001) docker     (127)    43351 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/radiancemeter_hsphere.svg
--rw-r--r--   0 runner    (1001) docker     (127)    36773 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/radiancemeter_plane.png
--rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/radiancemeter_plane.svg
--rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/requirement_layers.png
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/requirement_layers.svg
--rw-r--r--   0 runner    (1001) docker     (127)    21451 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/solid_2017.png
--rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_ckd_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (127)    16459 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_ckd_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_ckd_noatm_interval.png
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_ckd_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (127)    27127 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_noatm_interval1.png
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_noatm_interval2.png
--rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spherical-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/spherical-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/fig/thuillier_2003.png
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/generate_md_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/generate_rst_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/generate_rst_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/index_latex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    17968 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.948335 eradiate-0.27.0rc0/docs/rst/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22779 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/dependencies.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.952335 eradiate-0.27.0rc0/docs/rst/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/developer_guide/design_atmosphere.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/developer_guide/dev_install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/developer_guide/factory_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/developer_guide/lazy_loading.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/developer_guide/radiometric_kernel_interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/developer_guide/scene_generator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/developer_guide/update.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/maintainer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.956334 eradiate-0.27.0rc0/docs/rst/reference_api/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/attrs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/constants.rst
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/converters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/eradiate_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/factory.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/frame.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/kernel.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/mode.rst
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/notebook.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/plot.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/quad.rst
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/radprops.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/rng.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/scenes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/spectral.rst
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/srf_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/test_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/units.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/validators.rst
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/warp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_api/xarray.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.956334 eradiate-0.27.0rc0/docs/rst/reference_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/reference_plugins/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.956334 eradiate-0.27.0rc0/docs/rst/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.960335 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/absorption.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.960335 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
--rw-r--r--   0 runner    (1001) docker     (127)    26889 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/fig/good_resolution.png
--rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/fig/line.png
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/heterogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/homogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/molecular.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/particle_layer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/basic_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/conventions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.960335 eradiate-0.27.0rc0/docs/rst/user_guide/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/absorption.rst
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/atmosphere_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/atmosphere_thermoprops.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.960335 eradiate-0.27.0rc0/docs/rst/user_guide/data/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    30117 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
--rw-r--r--   0 runner    (1001) docker     (127)    59107 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/fig/pt_points.png
--rw-r--r--   0 runner    (1001) docker     (127)    28580 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/particle_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/solar_irradiance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/data/srf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/onedim_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/package_structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/scene_loader.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/spectral_discretization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/rst/user_guide/unit_guide_user.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.960335 eradiate-0.27.0rc0/docs/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/src/reference_cli.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.964335 eradiate-0.27.0rc0/docs/src/release_notes/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/src/release_notes/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/src/release_notes/v0.23.x_and_older.md
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/src/release_notes/v0.24.x.md
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/src/release_notes/v0.25.x.md
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/src/release_notes/v0.26.x.md
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/docs/src/release_notes/v0.27.x.md
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.964335 eradiate-0.27.0rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/check_conda_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.968335 eradiate-0.27.0rc0/requirements/conda/
--rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-dependencies-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-dependencies-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    17336 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-dependencies-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (127)    45955 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-dev-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    38847 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-dev-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    41374 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-dev-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)    31183 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-docs-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    21356 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-docs-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    24791 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-docs-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-main-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-main-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    17336 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-main-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)    45955 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-optional-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    38847 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-optional-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    41374 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-optional-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-optional.yml
--rw-r--r--   0 runner    (1001) docker     (127)    26801 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-recommended-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    25297 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-recommended-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    25976 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-recommended-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-recommended.yml
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-tests-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-tests-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-tests-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/conda/environment-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/copy_envvars.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/environment.in
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/layered.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/make_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/make_pip_in_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/make_pip_txt_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.972335 eradiate-0.27.0rc0/requirements/pip/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/dependencies.in
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/dependencies.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-24 16:13:32.000000 eradiate-0.27.0rc0/requirements/pip/dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/dev.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/docs.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/main.in
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/main.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/optional.in
--rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/optional.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/recommended.in
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/recommended.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-24 16:13:32.000000 eradiate-0.27.0rc0/requirements/pip/recommended.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/tests.in
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/requirements/pip/tests.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/setpath.bat
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/setpath.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/setpath.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:13:37.032335 eradiate-0.27.0rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.924334 eradiate-0.27.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.976335 eradiate-0.27.0rc0/src/eradiate/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11586 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/cfconventions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.976335 eradiate-0.27.0rc0/src/eradiate/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/cli/srf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.976335 eradiate-0.27.0rc0/src/eradiate/config/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/config/_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/config/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/config/default.toml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.980335 eradiate-0.27.0rc0/src/eradiate/data/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_safe_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)   211295 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/downloads_all.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16905 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/data/downloads_minimal.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.980335 eradiate-0.27.0rc0/src/eradiate/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/experiments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/experiments/_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/experiments/_canopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14479 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/experiments/_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/experiments/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/experiments/_dem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/experiments/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.984335 eradiate-0.27.0rc0/src/eradiate/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/_bitmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/_bsdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/kernel/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.984335 eradiate-0.27.0rc0/src/eradiate/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/notebook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/notebook/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.984335 eradiate-0.27.0rc0/src/eradiate/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/pipelines/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/pipelines/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24859 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/pipelines/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/quad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.984335 eradiate-0.27.0rc0/src/eradiate/radprops/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/radprops/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    32254 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/radprops/_absorption.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/radprops/_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/radprops/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/radprops/rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/rng.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.984335 eradiate-0.27.0rc0/src/eradiate/scenes/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.988335 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29357 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_molecular.py
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.988335 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_canopies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_canopy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)    39011 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_rami_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)    17140 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.992335 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_black.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_hapke.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_opacity_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_rpv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_rtls.py
--rw-r--r--   0 runner    (1001) docker     (127)    17684 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.992335 eradiate-0.27.0rc0/src/eradiate/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/illumination/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_astro_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.992335 eradiate-0.27.0rc0/src/eradiate/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/integrators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/integrators/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/integrators/_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.996335 eradiate-0.27.0rc0/src/eradiate/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)    22469 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/_perspective.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/measure/_radiancemeter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.996335 eradiate-0.27.0rc0/src/eradiate/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/phase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/phase/_blend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/phase/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/phase/_hg.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/phase/_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/phase/_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/phase/_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:36.996335 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.000335 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_multi_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.000335 eradiate-0.27.0rc0/src/eradiate/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/surface/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/surface/_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/surface/_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/surface/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/scenes/surface/_dem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.000335 eradiate-0.27.0rc0/src/eradiate/spectral/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/spectral/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17725 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/spectral/ckd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/spectral/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/spectral/mono.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/spectral/spectral_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    29383 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.000335 eradiate-0.27.0rc0/src/eradiate/test_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/test_tools/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/test_tools/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/test_tools/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/test_tools/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/test_tools/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/test_tools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/units.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.004335 eradiate-0.27.0rc0/src/eradiate/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11933 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13952 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/util/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/util/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.004335 eradiate-0.27.0rc0/src/eradiate/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/xarray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/xarray/_accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/xarray/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/src/eradiate/xarray/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.028335 eradiate-0.27.0rc0/src/eradiate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-04-24 16:13:36.000000 eradiate-0.27.0rc0/src/eradiate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-04-24 16:13:36.000000 eradiate-0.27.0rc0/src/eradiate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:13:36.000000 eradiate-0.27.0rc0/src/eradiate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 16:13:36.000000 eradiate-0.27.0rc0/src/eradiate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-24 16:13:36.000000 eradiate-0.27.0rc0/src/eradiate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 16:13:36.000000 eradiate-0.27.0rc0/src/eradiate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.004335 eradiate-0.27.0rc0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.004335 eradiate-0.27.0rc0/tests/01_unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.008335 eradiate-0.27.0rc0/tests/01_unit/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/test_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/test_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/test_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/test_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/data/test_safe_online.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.008335 eradiate-0.27.0rc0/tests/01_unit/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/experiments/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/experiments/test_canopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/experiments/test_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/experiments/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/experiments/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/experiments/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.008335 eradiate-0.27.0rc0/tests/01_unit/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/kernel/test_gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/kernel/test_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/kernel/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/kernel/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/kernel/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.008335 eradiate-0.27.0rc0/tests/01_unit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/pipelines/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/pipelines/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/pipelines/test_logic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.012335 eradiate-0.27.0rc0/tests/01_unit/radprops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/radprops/test_absorption.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/radprops/test_rayleigh_scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/radprops/test_zgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.012335 eradiate-0.27.0rc0/tests/01_unit/scenes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.012335 eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13483 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.012335 eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_tree_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_tree_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.016335 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_black.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_hapke.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_rpv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_rtls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.016335 eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/test_astro_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/test_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/test_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.016335 eradiate-0.27.0rc0/tests/01_unit/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/integrators/test_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.016335 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_perspective.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.016335 eradiate-0.27.0rc0/tests/01_unit/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/phase/test_blend.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/phase/test_hg.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/phase/test_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/phase/test_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/phase/test_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.020335 eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.020335 eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_multi_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.020335 eradiate-0.27.0rc0/tests/01_unit/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/surface/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/surface/test_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/surface/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    29485 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/scenes/test_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.020335 eradiate-0.27.0rc0/tests/01_unit/spectral/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/spectral/test_ckd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/spectral/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/spectral/test_mono.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.020335 eradiate-0.27.0rc0/tests/01_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_tools/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/test_warp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.024335 eradiate-0.27.0rc0/tests/01_unit/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/util/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/util/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.024335 eradiate-0.27.0rc0/tests/01_unit/xarray_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/xarray_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/01_unit/xarray_/test_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.024335 eradiate-0.27.0rc0/tests/02_system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_albedo.py
--rw-r--r--   0 runner    (1001) docker     (127)    25390 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_atmosphere_rpv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_ckd_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_compare_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_heterogeneous_atmosphere_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_heterogeneous_atmosphere_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_irradiance_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_kernel_render_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_maximum_scene_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_mdistant_insitu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_onedim_lambertian_brf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_onedim_phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_onedim_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/02_system/test_spectral_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.028335 eradiate-0.27.0rc0/tests/03_regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.028335 eradiate-0.27.0rc0/tests/03_regression/atmospheres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/atmospheres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/atmospheres/test_rpv_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/atmospheres/test_rpv_afgl1986_continental.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.028335 eradiate-0.27.0rc0/tests/03_regression/rami4atm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/rami4atm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:37.028335 eradiate-0.27.0rc0/tests/03_regression/romc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/romc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/romc/test_het01.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/romc/test_het04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/03_regression/romc/test_het06.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-24 16:13:27.000000 eradiate-0.27.0rc0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.729938 eradiate-0.27.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.629939 eradiate-0.27.0rc1/.devcontainer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      135 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.devcontainer/create-command.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.629939 eradiate-0.27.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.629939 eradiate-0.27.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.629939 eradiate-0.27.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-29 15:08:02.729938 eradiate-0.27.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.633939 eradiate-0.27.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.633939 eradiate-0.27.0rc1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_ext/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_ext/pluginparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.633939 eradiate-0.27.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)    17013 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32795 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25531 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-darkgrey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34059 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-darkgrey.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34061 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.617939 eradiate-0.27.0rc1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.633939 eradiate-0.27.0rc1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.633939 eradiate-0.27.0rc1/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/_templates/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/convert_figures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.641939 eradiate-0.27.0rc1/docs/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    20540 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/atmosphere_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/atmosphere_attributes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28149 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-east_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32937 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-east_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28852 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-east_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35278 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-east_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-north_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-north_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28115 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-north_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32455 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-north_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28153 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-south_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32939 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-south_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28118 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-south_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32455 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-south_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28178 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-west_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32935 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-west_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-west_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32437 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/azimuth-west_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/cartesian-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/cartesian-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25301 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/cuboid_leaf_cloud_params.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/cuboid_leaf_cloud_params.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.645938 eradiate-0.27.0rc1/docs/fig/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/diagrams/class_diagram_biosphere.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    72629 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/diagrams/package.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    40438 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/eradiate-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/icon_eradiate.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35418 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/package.png
+-rw-r--r--   0 runner    (1001) docker     (127)   232270 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/package.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32384 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/radiancemeter_hsphere.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43351 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/radiancemeter_hsphere.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    36773 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/radiancemeter_plane.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/radiancemeter_plane.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.653938 eradiate-0.27.0rc1/docs/fig/rami_scenes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32289 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ADJACENT_CANOPIES_MEDIUM_ERECTOPHILE_SPARSE_PLANOPHILE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32437 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ADJACENT_CANOPIES_SPARSE_ERECTOPHILE_DENSE_PLANOPHILE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35160 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/AGRICULTURAL_CROPS_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56720 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_ERECTOPHILE_B_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48599 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_ERECTOPHILE_C_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39795 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_DENSE_BRF_MODEL_A_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42011 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_DENSE_BRF_MODEL_B_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32764 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_DENSE_BRF_MODEL_C_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40917 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_SPARSE_BRF_MODEL_A_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41211 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_SPARSE_BRF_MODEL_B_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32630 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_SPARSE_BRF_MODEL_C_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54396 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_PLANOPHILE_A_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56275 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_PLANOPHILE_B_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49288 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_PLANOPHILE_C_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31442 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/CONSTANT_SLOPE_DISTRIBUTION_DENSE_INCLINATION_15_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31267 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/CONSTANT_SLOPE_DISTRIBUTION_DENSE_INCLINATION_30_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34698 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/CONSTANT_SLOPE_DISTRIBUTION_SPARSE_INCLINATION_15_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34281 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/CONSTANT_SLOPE_DISTRIBUTION_SPARSE_INCLINATION_30_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    50592 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/JARVSELJA_BIRCH_STAND_SUMMER_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57116 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/JARVSELJA_BIRCH_STAND_WINTER_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42280 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/JARVSELJA_PINE_STAND_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47308 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/OFENPASS_PINE_STAND_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34887 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/SAVANNA_PRE_FIRE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    52914 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_ERECTOPHILE_SPARSE_PLANOPHILE_DENSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53834 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_ERECTOPHILE_SPARSE_PLANOPHILE_MEDIUM_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54830 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_ERECTOPHILE_SPARSE_PLANOPHILE_SPARSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39330 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_DENSE_UNDERSTORIES_DENSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39731 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_DENSE_UNDERSTORIES_SPARSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39471 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_MEDIUM_UNDERSTORIES_DENSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40133 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_MEDIUM_UNDERSTORIES_SPARSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38926 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_SPARSE_UNDERSTORIES_DENSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39919 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_SPARSE_UNDERSTORIES_SPARSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53627 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_PLANOPHILE_SPARSE_ERECTOPHILE_DENSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54384 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_PLANOPHILE_SPARSE_ERECTOPHILE_MEDIUM_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55431 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/TWO_LAYER_CANOPY_PLANOPHILE_SPARSE_ERECTOPHILE_SPARSE_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42795 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/WELLINGTON_CITRUS_ORCHARD_30_90.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    50049 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/rami_scenes/WYTHAM_WOOD_30_90.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/requirement_layers.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/requirement_layers.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    21451 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/solid_2017.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_ckd_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16459 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27127 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spherical-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/spherical-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/fig/thuillier_2003.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/generate_md_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/generate_rst_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/generate_rst_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/generate_rst_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/index_latex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.617939 eradiate-0.27.0rc1/docs/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.653938 eradiate-0.27.0rc1/docs/resources/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/resources/config/default.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.653938 eradiate-0.27.0rc1/docs/rst/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22779 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.653938 eradiate-0.27.0rc1/docs/rst/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/atmosphere_molecular_absorption.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/atmosphere_thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/data_format_details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.653938 eradiate-0.27.0rc1/docs/rst/data/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)   208042 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/fig/govaerts_2021-continental-extrapolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)   195787 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/fig/govaerts_2021-desert-extrapolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30117 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/fig/p_interp_rerr_histo_65349.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59107 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/fig/pt_points.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28580 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/fig/w_interp_rerr_histo_101325.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.653938 eradiate-0.27.0rc1/docs/rst/data/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/generated/aerosols_particles.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/generated/rami_scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/solar_irradiance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/data/srf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/dependencies.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.657938 eradiate-0.27.0rc1/docs/rst/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/developer_guide/design_atmosphere.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/developer_guide/dev_install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/developer_guide/factory_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/developer_guide/lazy_loading.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/developer_guide/scene_generator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/developer_guide/update.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/maintainer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.661938 eradiate-0.27.0rc1/docs/rst/reference_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/converters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/eradiate_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/experiments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/frame.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/kernel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/mode.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/quad.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/rng.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/spectral.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/srf_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/test_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/warp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_api/xarray.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.661938 eradiate-0.27.0rc1/docs/rst/reference_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/reference_plugins/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.661938 eradiate-0.27.0rc1/docs/rst/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.665938 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/absorption.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.665938 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26889 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/fig/line.png
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/homogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/molecular.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/particle_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/basic_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/canopy_scene_loader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/dem_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/package_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/spectral_discretization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/rst/user_guide/unit_guide_user.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.665938 eradiate-0.27.0rc1/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/src/reference_cli.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.665938 eradiate-0.27.0rc1/docs/src/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/src/release_notes/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/src/release_notes/v0.23.x_and_older.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/src/release_notes/v0.24.x.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/src/release_notes/v0.25.x.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/src/release_notes/v0.26.x.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/docs/src/release_notes/v0.27.x.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.665938 eradiate-0.27.0rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/check_conda_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.673938 eradiate-0.27.0rc1/requirements/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-dependencies-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-dependencies-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-dependencies-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46656 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-dev-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    39542 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-dev-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    42072 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-dev-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    32564 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-docs-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    22729 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-docs-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-docs-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-main-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-main-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-main-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46656 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-optional-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    39542 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-optional-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    42072 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-optional-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-optional.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    26083 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-recommended-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    25293 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-recommended-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    25975 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-recommended-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-recommended.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-tests-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-tests-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-tests-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/conda/environment-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/copy_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/environment.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/layered.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/make_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/make_pip_in_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/make_pip_txt_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.673938 eradiate-0.27.0rc1/requirements/pip/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/dependencies.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-29 15:07:58.000000 eradiate-0.27.0rc1/requirements/pip/dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/dev.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/docs.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/main.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/main.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/optional.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/optional.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/recommended.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/recommended.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-29 15:07:58.000000 eradiate-0.27.0rc1/requirements/pip/recommended.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/tests.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/requirements/pip/tests.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/setpath.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/setpath.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/setpath.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:08:02.729938 eradiate-0.27.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.621939 eradiate-0.27.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.677938 eradiate-0.27.0rc1/src/eradiate/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11586 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/cfconventions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.681938 eradiate-0.27.0rc1/src/eradiate/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/cli/srf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.681938 eradiate-0.27.0rc1/src/eradiate/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/config/_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/config/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/config/default.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.681938 eradiate-0.27.0rc1/src/eradiate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_safe_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211295 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/downloads_all.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16905 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/data/downloads_minimal.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.685938 eradiate-0.27.0rc1/src/eradiate/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/experiments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/experiments/_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/experiments/_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14479 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/experiments/_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/experiments/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/experiments/_dem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/experiments/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.685938 eradiate-0.27.0rc1/src/eradiate/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/_bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/_bsdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/kernel/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.685938 eradiate-0.27.0rc1/src/eradiate/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/notebook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/notebook/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.685938 eradiate-0.27.0rc1/src/eradiate/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/pipelines/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/pipelines/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24859 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/pipelines/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/quad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.689938 eradiate-0.27.0rc1/src/eradiate/radprops/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/radprops/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    32254 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/radprops/_absorption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/radprops/_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/radprops/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/radprops/rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/rng.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.689938 eradiate-0.27.0rc1/src/eradiate/scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.689938 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29357 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_molecular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.689938 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_canopies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_canopy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39011 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_rami_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17140 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.693938 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_black.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_hapke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_opacity_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_rtls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17684 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.693938 eradiate-0.27.0rc1/src/eradiate/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/illumination/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_astro_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.693938 eradiate-0.27.0rc1/src/eradiate/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/integrators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/integrators/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/integrators/_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.697938 eradiate-0.27.0rc1/src/eradiate/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22469 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/measure/_radiancemeter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.697938 eradiate-0.27.0rc1/src/eradiate/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/phase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/phase/_blend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/phase/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/phase/_hg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/phase/_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/phase/_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/phase/_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.697938 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.701938 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_multi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.701938 eradiate-0.27.0rc1/src/eradiate/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/surface/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/surface/_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/surface/_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/surface/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18254 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/scenes/surface/_dem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.701938 eradiate-0.27.0rc1/src/eradiate/spectral/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/spectral/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17725 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/spectral/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/spectral/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/spectral/mono.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/spectral/spectral_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29383 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.701938 eradiate-0.27.0rc1/src/eradiate/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/test_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/test_tools/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/test_tools/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/test_tools/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/test_tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/test_tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/units.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.705938 eradiate-0.27.0rc1/src/eradiate/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11933 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13952 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/util/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/util/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.705938 eradiate-0.27.0rc1/src/eradiate/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/xarray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/xarray/_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/xarray/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/src/eradiate/xarray/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.725938 eradiate-0.27.0rc1/src/eradiate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-29 15:08:02.000000 eradiate-0.27.0rc1/src/eradiate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23935 2024-04-29 15:08:02.000000 eradiate-0.27.0rc1/src/eradiate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:08:02.000000 eradiate-0.27.0rc1/src/eradiate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 15:08:02.000000 eradiate-0.27.0rc1/src/eradiate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-29 15:08:02.000000 eradiate-0.27.0rc1/src/eradiate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 15:08:02.000000 eradiate-0.27.0rc1/src/eradiate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.705938 eradiate-0.27.0rc1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.705938 eradiate-0.27.0rc1/tests/01_unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.709938 eradiate-0.27.0rc1/tests/01_unit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/test_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/test_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/test_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/data/test_safe_online.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.709938 eradiate-0.27.0rc1/tests/01_unit/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/experiments/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/experiments/test_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/experiments/test_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/experiments/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/experiments/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/experiments/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.709938 eradiate-0.27.0rc1/tests/01_unit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/kernel/test_gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/kernel/test_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/kernel/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/kernel/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/kernel/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.709938 eradiate-0.27.0rc1/tests/01_unit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/pipelines/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/pipelines/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/pipelines/test_logic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.709938 eradiate-0.27.0rc1/tests/01_unit/radprops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/radprops/test_absorption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/radprops/test_rayleigh_scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/radprops/test_zgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.713938 eradiate-0.27.0rc1/tests/01_unit/scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.713938 eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13483 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.713938 eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_tree_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_tree_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.713938 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_black.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_hapke.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_rtls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.713938 eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/test_astro_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/test_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/test_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.717938 eradiate-0.27.0rc1/tests/01_unit/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/integrators/test_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.717938 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.717938 eradiate-0.27.0rc1/tests/01_unit/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/phase/test_blend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/phase/test_hg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/phase/test_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/phase/test_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/phase/test_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.717938 eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.721938 eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_multi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.721938 eradiate-0.27.0rc1/tests/01_unit/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/surface/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/surface/test_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/surface/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29485 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/scenes/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.721938 eradiate-0.27.0rc1/tests/01_unit/spectral/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/spectral/test_ckd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/spectral/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/spectral/test_mono.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.721938 eradiate-0.27.0rc1/tests/01_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_tools/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/test_warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.721938 eradiate-0.27.0rc1/tests/01_unit/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/util/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/util/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.721938 eradiate-0.27.0rc1/tests/01_unit/xarray_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/xarray_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/01_unit/xarray_/test_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.725938 eradiate-0.27.0rc1/tests/02_system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_albedo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25390 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_atmosphere_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_ckd_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_compare_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_heterogeneous_atmosphere_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_heterogeneous_atmosphere_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_irradiance_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_kernel_render_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_maximum_scene_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_mdistant_insitu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_onedim_lambertian_brf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_onedim_phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_onedim_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/02_system/test_spectral_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.725938 eradiate-0.27.0rc1/tests/03_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.725938 eradiate-0.27.0rc1/tests/03_regression/atmospheres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/atmospheres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/atmospheres/test_rpv_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/atmospheres/test_rpv_afgl1986_continental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.725938 eradiate-0.27.0rc1/tests/03_regression/rami4atm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/rami4atm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:08:02.725938 eradiate-0.27.0rc1/tests/03_regression/romc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/romc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/romc/test_het01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/romc/test_het04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/03_regression/romc/test_het06.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-29 15:07:55.000000 eradiate-0.27.0rc1/tests/conftest.py
```

### Comparing `eradiate-0.27.0rc0/.clang-format` & `eradiate-0.27.0rc1/.clang-format`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/.devcontainer/devcontainer.json` & `eradiate-0.27.0rc1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/.github/ISSUE_TEMPLATE/bug_report.md` & `eradiate-0.27.0rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/.github/ISSUE_TEMPLATE/feature_request.md` & `eradiate-0.27.0rc1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/.github/pull_request_template.md` & `eradiate-0.27.0rc1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/.github/workflows/cd.yml` & `eradiate-0.27.0rc1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/.github/workflows/ci.yml` & `eradiate-0.27.0rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/.pre-commit-config.yaml` & `eradiate-0.27.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/.readthedocs.yml` & `eradiate-0.27.0rc1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/CITATION.cff` & `eradiate-0.27.0rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/CONTRIBUTING.md` & `eradiate-0.27.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/LICENSE` & `eradiate-0.27.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/Makefile` & `eradiate-0.27.0rc1/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 	make -C docs serve
 
 docs-linkcheck:
 	make -C docs linkcheck
 
 docs-rst:
 	make -C docs rst-api
+	make -C docs rst-data
 	make -C docs rst-plugins
 	make -C docs md-cli
 
 docs-render-tutorials:
 	$(PYTHON) tutorials/run.py run
 
 docs-clean:
```

### Comparing `eradiate-0.27.0rc0/PKG-INFO` & `eradiate-0.27.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.27.0rc0
+Version: 0.27.0rc1
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
@@ -14,15 +14,14 @@
 Requires-Dist: eradiate-mitsuba==0.2.1
 Requires-Dist: aenum
 Requires-Dist: attrs>=22.2
 Requires-Dist: cachetools>=5.3
 Requires-Dist: click
 Requires-Dist: dessinemoi>=23.1.0
 Requires-Dist: dynaconf>=3.2
-Requires-Dist: importlib_resources
 Requires-Dist: joseki>=2.6.0
 Requires-Dist: lazy_loader>=0.1
 Requires-Dist: matplotlib>=3.3
 Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: pint
 Requires-Dist: pinttrs>=23.2.0
@@ -47,15 +46,14 @@
 Requires-Dist: seaborn; extra == "recommended"
 Requires-Dist: aenum; extra == "recommended"
 Requires-Dist: attrs>=22.2; extra == "recommended"
 Requires-Dist: cachetools>=5.3; extra == "recommended"
 Requires-Dist: click; extra == "recommended"
 Requires-Dist: dessinemoi>=23.1.0; extra == "recommended"
 Requires-Dist: dynaconf>=3.2; extra == "recommended"
-Requires-Dist: importlib_resources; extra == "recommended"
 Requires-Dist: joseki>=2.6.0; extra == "recommended"
 Requires-Dist: lazy_loader>=0.1; extra == "recommended"
 Requires-Dist: matplotlib>=3.3; extra == "recommended"
 Requires-Dist: netcdf4; extra == "recommended"
 Requires-Dist: numpy; extra == "recommended"
 Requires-Dist: pint; extra == "recommended"
 Requires-Dist: pinttrs>=23.2.0; extra == "recommended"
```

### Comparing `eradiate-0.27.0rc0/README.md` & `eradiate-0.27.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/Makefile` & `eradiate-0.27.0rc1/docs/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -8,37 +8,41 @@
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
-.PHONY: help serve html-plot rst-api rst-plugins clean clean_generated Makefile
+.PHONY: help serve html-plot rst-api rst-data rst-plugins clean clean_generated Makefile
 
 serve:
 	sphinx-autobuild "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 html-plot:
 	$(SPHINXBUILD) -D plot_gallery=1 -b html "$(SOURCEDIR)" "$(BUILDDIR)/html" $(SPHINXOPTS) $(O)
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
 
 rst-api:
 	python generate_rst_api.py
 
+rst-data:
+	python generate_rst_data.py
+
 rst-plugins:
 	python generate_rst_plugins.py
 
 md-cli:
 	python generate_md_cli.py
 
 clean: clean_generated
 	rm -rf _build/*
 
 clean_generated:
+	rm -rf rst/data/generated/*
 	rm -rf rst/reference_api/generated/*
 	rm -rf rst/reference_plugins/generated/*
 	rm -rf examples/generated/*
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
```

### Comparing `eradiate-0.27.0rc0/docs/_ext/exec.py` & `eradiate-0.27.0rc1/docs/_ext/exec.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_ext/pluginparameters.py` & `eradiate-0.27.0rc1/docs/_ext/pluginparameters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-black.png` & `eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-black.svg` & `eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-black.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-darkgrey.png` & `eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-darkgrey.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-darkgrey.svg` & `eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-darkgrey.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-white.png` & `eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-white.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_static/eradiate-logo-typo-white.svg` & `eradiate-0.27.0rc1/docs/_static/eradiate-logo-typo-white.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_templates/autosummary/module.rst` & `eradiate-0.27.0rc1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/_templates/sections/footer-content.html` & `eradiate-0.27.0rc1/docs/_templates/sections/footer-content.html`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/conf.py` & `eradiate-0.27.0rc1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,16 +287,19 @@
 # -------------------------- Custom generation steps ---------------------------
 
 
 def custom_step(app):
     sys.path.append(os.path.dirname(os.path.abspath(__file__)))
     import generate_md_cli
     import generate_rst_api
+    import generate_rst_data
     import generate_rst_plugins
 
     generate_md_cli.generate()  # CLI reference
     generate_rst_plugins.generate()  # Plugins
     generate_rst_api.generate_factory_docs()  # Factories
+    generate_rst_data.generate_particle_radprops_summary()  # Summary
+    generate_rst_data.generate_rami_scene_summary()  # Summary
 
 
 def setup(app):
     app.connect("builder-inited", custom_step)
```

### Comparing `eradiate-0.27.0rc0/docs/fig/atmosphere_attributes.png` & `eradiate-0.27.0rc1/docs/fig/atmosphere_attributes.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/atmosphere_attributes.svg` & `eradiate-0.27.0rc1/docs/fig/atmosphere_attributes.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-east_left.png` & `eradiate-0.27.0rc1/docs/fig/azimuth-east_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-east_left.svg` & `eradiate-0.27.0rc1/docs/fig/azimuth-east_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-east_right.png` & `eradiate-0.27.0rc1/docs/fig/azimuth-east_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-east_right.svg` & `eradiate-0.27.0rc1/docs/fig/azimuth-east_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-north_left.png` & `eradiate-0.27.0rc1/docs/fig/azimuth-north_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-north_left.svg` & `eradiate-0.27.0rc1/docs/fig/azimuth-north_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-north_right.png` & `eradiate-0.27.0rc1/docs/fig/azimuth-north_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-north_right.svg` & `eradiate-0.27.0rc1/docs/fig/azimuth-north_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-south_left.png` & `eradiate-0.27.0rc1/docs/fig/azimuth-south_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-south_left.svg` & `eradiate-0.27.0rc1/docs/fig/azimuth-south_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-south_right.png` & `eradiate-0.27.0rc1/docs/fig/azimuth-south_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-south_right.svg` & `eradiate-0.27.0rc1/docs/fig/azimuth-south_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-west_left.png` & `eradiate-0.27.0rc1/docs/fig/azimuth-west_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-west_left.svg` & `eradiate-0.27.0rc1/docs/fig/azimuth-west_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-west_right.png` & `eradiate-0.27.0rc1/docs/fig/azimuth-west_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/azimuth-west_right.svg` & `eradiate-0.27.0rc1/docs/fig/azimuth-west_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/cartesian-coordinate-system.png` & `eradiate-0.27.0rc1/docs/fig/cartesian-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/cartesian-coordinate-system.svg` & `eradiate-0.27.0rc1/docs/fig/cartesian-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/cuboid_leaf_cloud_params.png` & `eradiate-0.27.0rc1/docs/fig/cuboid_leaf_cloud_params.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/cuboid_leaf_cloud_params.svg` & `eradiate-0.27.0rc1/docs/fig/cuboid_leaf_cloud_params.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/diagrams/class_diagram_biosphere.drawio` & `eradiate-0.27.0rc1/docs/fig/diagrams/class_diagram_biosphere.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio` & `eradiate-0.27.0rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/eradiate-logo-typo-black.png` & `eradiate-0.27.0rc1/docs/fig/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/eradiate-logo.svg` & `eradiate-0.27.0rc1/docs/fig/eradiate-logo.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/icon_eradiate.png` & `eradiate-0.27.0rc1/docs/fig/icon_eradiate.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/radiancemeter_hsphere.png` & `eradiate-0.27.0rc1/docs/fig/radiancemeter_hsphere.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/radiancemeter_hsphere.svg` & `eradiate-0.27.0rc1/docs/fig/radiancemeter_hsphere.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/radiancemeter_plane.png` & `eradiate-0.27.0rc1/docs/fig/radiancemeter_plane.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/radiancemeter_plane.svg` & `eradiate-0.27.0rc1/docs/fig/radiancemeter_plane.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/requirement_layers.png` & `eradiate-0.27.0rc1/docs/fig/requirement_layers.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/requirement_layers.svg` & `eradiate-0.27.0rc1/docs/fig/requirement_layers.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/solid_2017.png` & `eradiate-0.27.0rc1/docs/fig/solid_2017.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_ckd_atm_interval.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_ckd_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_ckd_atm_isolated.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_ckd_noatm_interval.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_ckd_noatm_isolated.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_atm_interval.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_atm_isolated.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_noatm_interval1.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_noatm_interval2.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spectral_discretization_mono_noatm_isolated.png` & `eradiate-0.27.0rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spherical-coordinate-system.png` & `eradiate-0.27.0rc1/docs/fig/spherical-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/spherical-coordinate-system.svg` & `eradiate-0.27.0rc1/docs/fig/spherical-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/fig/thuillier_2003.png` & `eradiate-0.27.0rc1/docs/fig/thuillier_2003.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/generate_md_cli.py` & `eradiate-0.27.0rc1/docs/generate_md_cli.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/generate_rst_api.py` & `eradiate-0.27.0rc1/docs/generate_rst_api.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/generate_rst_plugins.py` & `eradiate-0.27.0rc1/docs/generate_rst_plugins.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/index.rst` & `eradiate-0.27.0rc1/docs/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 
    .. grid-item-card:: :fas:`graduation-cap` Tutorials
       :link: sec-tutorials
       :link-type: ref
 
       A practical introduction to Eradiate.
 
+   .. grid-item-card:: :fas:`database` Data guide
+      :link: sec-data-intro
+      :link-type: ref
+
+      Information about data formats and shipped datasets.
+
    .. grid-item-card:: :fas:`file-code` Reference
       :link: sec-reference_api
       :link-type: ref
 
       The complete reference.
 
 .. toctree::
@@ -62,14 +68,27 @@
    src/release_notes/index.md
    rst/bibliography
 
 .. toctree::
    :maxdepth: 3
    :hidden:
    :titlesonly:
-   :caption: Developers/contributors
+   :caption: Data
 
+   rst/data/intro
+   Aerosols / particles <rst/data/generated/aerosols_particles.rst>
+   rst/data/atmosphere_thermoprops
+   rst/data/atmosphere_molecular_absorption
+   Solar irradiance <rst/data/solar_irradiance.rst>
+   rst/data/srf
+   rst/data/generated/rami_scenes
+
+.. toctree::
+   :maxdepth: 3
+   :hidden:
+   :titlesonly:
+   :caption: Developers/contributors
 
-   rst/dependencies
    rst/contributing
+   rst/dependencies
    rst/maintainer_guide
    rst/developer_guide/index
```

### Comparing `eradiate-0.27.0rc0/docs/make.bat` & `eradiate-0.27.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/references.bib` & `eradiate-0.27.0rc1/docs/references.bib`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 % Formatted and sorted with bibtex-tidy
 % https://github.com/FlamingTempura/bibtex-tidy
+
 @techreport{Anderson1986AtmosphericConstituentProfiles,
   title        = {AFGL Atmospheric Constituent Profiles (0-120) km},
   author       = {G.P. Anderson and J.H Chetwynd and S.A. Clough and E.P. Shettle and F.X. Kneizys},
   year         = 1986,
   number       = {AFGL-TR-86-0110},
   url          = {https://ui.adsabs.harvard.edu/abs/1986afgl.rept.....A/abstract},
   institution  = {Air Force Geophysics Laboratory}
@@ -15,59 +16,58 @@
   journal      = {Planetary and Space Science},
   volume       = 32,
   number       = 6,
   pages        = {785--790},
   doi          = {10.1016/0032-0633(84)90102-8},
   issn         = {0032-0633},
   url          = {http://www.sciencedirect.com/science/article/pii/0032063384901028},
-  shortjournal = {Planetary and Space Science},
+  shortjournal = {Planetary and Space Science}
 }
 @article{Burggraaff2020BiasesIncorrectReflectance,
   title        = {Biases from incorrect reflectance convolution},
   author       = {Burggraaff, Olivier},
   year         = 2020,
   month        = apr,
   journal      = {Optics Express},
   volume       = 28,
   number       = 9,
   pages        = {13801--13816},
   doi          = {10.1364/OE.391470},
   issn         = {1094-4087},
   url          = {https://opg.optica.org/oe/abstract.cfm?uri=oe-28-9-13801},
-  urldate      = {2023-07-20},
+  urldate      = {2023-07-20}
 }
 @article{Coddington2021TSIS1HSRS,
-	title = {The {TSIS}-1 {Hybrid} {Solar} {Reference} {Spectrum}},
-	volume = {48},
-	issn = {1944-8007},
-	doi = {10.1029/2020GL091709},
-	number = {12},
-	journal = {Geophysical Research Letters},
-	author = {Coddington, O. M. and Richard, E. C. and Harber, D. and Pilewskie, P. and Woods, T. N. and Chance, K. and Liu, X. and Sun, K.},
-	year = {2021},
-
+  title        = {The {TSIS}-1 {Hybrid} {Solar} {Reference} {Spectrum}},
+  author       = {Coddington, O. M. and Richard, E. C. and Harber, D. and Pilewskie, P. and Woods, T. N. and Chance, K. and Liu, X. and Sun, K.},
+  year         = 2021,
+  journal      = {Geophysical Research Letters},
+  volume       = 48,
+  number       = 12,
+  doi          = {10.1029/2020GL091709},
+  issn         = {1944-8007}
 }
 @article{Coddington2022TSIS1HSRSVersion2,
-  author          = {Coddington, O. and Richard, E. and Harber, D. and Pilewskie, P. and Woods, T. N. and Snow, M. and Chance, K. and Liu, X. and and Sun, K.},
-  journal         = {Earth and Space Science Journal},
-  title           = {Version 2 of the TSIS-1 Hybrid Solar Reference Spectrum and Extension to the Full Spectrum},
-  year            = {2022 (accepted)}
+  title        = {Version 2 of the TSIS-1 Hybrid Solar Reference Spectrum and Extension to the Full Spectrum},
+  author       = {Coddington, O. and Richard, E. and Harber, D. and Pilewskie, P. and Woods, T. N. and Snow, M. and Chance, K. and Liu, X. and and Sun, K.},
+  year         = {2022 (accepted)},
+  journal      = {Earth and Space Science Journal}
 }
 @article{Eberhard2010CorrectEquationsCommon,
   title        = {Correct equations and common approximations for calculating {Rayleigh} scatter in pure gases and mixtures and evaluation of differences},
   author       = {Eberhard, Wynn L.},
   year         = 2010,
   month        = mar,
   journal      = {Applied Optics},
   volume       = 49,
   number       = 7,
   pages        = {1116--1130},
   doi          = {10.1364/AO.49.001116},
   issn         = {2155-3165},
-  url          = {https://www.osapublishing.org/ao/abstract.cfm?uri=ao-49-7-1116},
+  url          = {https://www.osapublishing.org/ao/abstract.cfm?uri=ao-49-7-1116}
 }
 @techreport{EradiateScientificHandbook2020,
   title        = {Eradiate Scientific Handbook},
   author       = {Eradiate Team},
   year         = 2020,
   url          = {https://www.eradiate.eu/site/docs/},
   institution  = {Eradiate}
@@ -98,15 +98,15 @@
   year         = 1992,
   journal      = {Journal of the Atmospheric Sciences},
   volume       = 49,
   number       = 22,
   pages        = {2139--2156},
   doi          = {10.1175/1520-0469(1992)049<2139:OTCDMF>2.0.CO;2},
   issn         = {0022-4928},
-  url          = {https://journals.ametsoc.org/doi/abs/10.1175/1520-0469%281992%29049%3C2139%3AOTCDMF%3E2.0.CO%3B2},
+  url          = {https://journals.ametsoc.org/doi/abs/10.1175/1520-0469%281992%29049%3C2139%3AOTCDMF%3E2.0.CO%3B2}
 }
 @article{Gordon2016HITRAN2016MolecularSpectroscopic,
   title        = {The {HITRAN2016} Molecular Spectroscopic Database},
   author       = {I.E. Gordon and L.S. Rothman and C. Hill and R.V. Kochanov and Y. Tan and P.F. Bernath and M. Birk and V. Boudon and A. Campargue and K.V. Chance and B.J. Drouin and J.-M. Flaud and R.R. Gamache and J.T. Hodges and D. Jacquemart and V.I. Perevalov and A. Perrin and K.P. Shine and M.-A.H. Smith and J. Tennyson and G.C. Toon and H. Tran and V.G. Tyuterev and A. Barbe and A.G. Császár and V.M. Devi and T. Furtenbacher and J.J. Harrison and J.-M. Hartmann and A. Jolly and T.J. Johnson and T. Karman and I. Kleiner and A.A. Kyuberis and J. Loos and O.M. Lyulin and S.T. Massie and S.N. Mikhailenko and N. Moazzen-Ahmadi and H.S.P. Müller and O.V. Naumenko and A.V. Nikitin and O.L. Polyansky and M. Rey and M. Rotger and S.W. Sharpe and K. Sung and E. Starikova and S.A. Tashkun and J. Vander Auwera and G. Wagner and J. Wilzewski and P. Wcisło and S. Yu and E.J. Zak},
   year         = 2017,
   journal      = {Journal of Quantative Spectroscopy and Radiative Transfer},
   volume       = 203,
@@ -128,57 +128,57 @@
 @article{Hansen1974LightScatteringPlanetary,
   title        = {Light scattering in planetary atmospheres},
   author       = {Hansen, James E., and Larry D. Travis},
   year         = 1974,
   journal      = {Space Science Reviews},
   doi          = {10.1007/BF00168069}
 }
-@article{HAPKE198441,
-  title = {Bidirectional reflectance spectroscopy: 3. Correction for macroscopic roughness},
-  journal = {Icarus},
-  volume = {59},
-  number = {1},
-  pages = {41-59},
-  year = {1984},
-  issn = {0019-1035},
-  doi = {https://doi.org/10.1016/0019-1035(84)90054-X},
-  url = {https://www.sciencedirect.com/science/article/pii/001910358490054X},
-  author = {Hapke, Bruce},
+@article{Hapke1984BidirectionalReflectanceSpectroscopy,
+  title        = {Bidirectional reflectance spectroscopy: 3. Correction for macroscopic roughness},
+  author       = {Hapke, Bruce},
+  year         = 1984,
+  journal      = {Icarus},
+  volume       = 59,
+  number       = 1,
+  pages        = {41--59},
+  doi          = {https://doi.org/10.1016/0019-1035(84)90054-X},
+  issn         = {0019-1035},
+  url          = {https://www.sciencedirect.com/science/article/pii/001910358490054X}
 }
 @article{Henyey1941Diffuse,
   title        = {Diffuse radiation in the galaxy},
   author       = {Henyey, L.G. and Greenstein, J.L.},
   year         = 1941,
   journal      = {The Astrophysical Journal},
   volume       = 93,
   pages        = {70--83}
 }
 @misc{ISO201980000QuantitiesUnits,
   title        = {80000-2:2019 — {{Quantities}} and Units — {{Part}} 2: {{Mathematics}}},
   author       = {ISO},
-  url          = {https://www.iso.org/standard/64973.html},
-  year         = 2019
+  year         = 2019,
+  url          = {https://www.iso.org/standard/64973.html}
 }
 @article{Jakob2022DrJit,
   title        = {Dr.{{Jit}}: {{A Just-In-Time Compiler}} for {{Differentiable Rendering}}},
   author       = {Jakob, Wenzel and Speierer, Sébastien and Roussel, Nicolas and Vicini, Delio},
+  year         = 2022,
   journal      = {ACM Transactions on Graphics},
   volume       = 41,
   number       = 4,
   pages        = {1--19},
   doi          = {10.1145/3528223.3530099},
   issn         = {0730-0301, 1557-7368},
-  url          = {http://arxiv.org/abs/2202.01284},
-  year         = 2022
+  url          = {http://arxiv.org/abs/2202.01284}
 }
 @misc{Jakob2022Mitsuba3,
   title        = {Mitsuba 3 renderer},
   author       = {Wenzel Jakob and Sébastien Speierer and Nicolas Roussel and Merlin Nimier-David and Delio Vicini and Tizian Zeltner and Baptiste Nicolet and Miguel Crespo and Vincent Leroy and Ziyi Zhang},
   year         = 2022,
-  note         = {https://mitsuba-renderer.org},
+  note         = {https://mitsuba-renderer.org}
 }
 @book{Liou2002IntroductionAtmosphericRadiation,
   title        = {An Introduction to Atmospheric Radiation},
   author       = {Liou, Kuo-Nan},
   year         = 2002,
   publisher    = {Elsevier},
   volume       = 84,
@@ -197,15 +197,15 @@
   year         = 2019,
   journal      = {ACM Trans. Graph.},
   volume       = 38,
   number       = 4,
   pages        = {44:1--44:13},
   doi          = {10.1145/3306346.3323025},
   issn         = {0730-0301},
-  url          = {http://doi.acm.org/10.1145/3306346.3323025},
+  url          = {http://doi.acm.org/10.1145/3306346.3323025}
 }
 @misc{MODIS2004,
   author       = {MODIS Characterization Support Team},
   year         = 2004,
   url          = {https://mcst.gsfc.nasa.gov/sites/default/files/file_attachments/MODIS_PFM_IB_OOB_RSR_merged.xls},
   institution  = {National Aeronautics and Space Administration},
   howpublished = {https://mcst.gsfc.nasa.gov/calibration/parameters}
@@ -238,15 +238,15 @@
   journal      = {ACM Transactions on Graphics},
   volume       = 38,
   number       = 6,
   pages        = {203:1--203:17},
   doi          = {10.1145/3355089.3356498},
   issn         = {0730-0301},
   url          = {http://rgl.epfl.ch/publications/NimierDavidVicini2019Mitsuba2},
-  shortjournal = {ACM Trans. Graph.},
+  shortjournal = {ACM Trans. Graph.}
 }
 @article{Peck1972DispersionAir,
   title        = {Dispersion of air},
   author       = {E.R. Peck and K. Reeder},
   year         = 1972,
   journal      = {Journal of the optical society of America},
   doi          = {10.1364/JOSA.62.000958}
@@ -335,15 +335,15 @@
   volume       = 214,
   number       = 1,
   pages        = {1--22},
   doi          = {10.1023/A:1024048429145},
   issn         = {1573-093X},
   url          = {https://doi.org/10.1023/A:1024048429145},
   shortjournal = {Solar Physics},
-  date         = {2003-05-01},
+  date         = {2003-05-01}
 }
 @inproceedings{Widlowski2006Rayspread,
   title        = {Rayspread: {{A Virtual Laboratory}} for {{Rapid BRF Simulations Over}} 3-{{D Plant Canopies}}},
   shorttitle   = {Rayspread},
   author       = {Widlowski, Jean-Luc and Lavergne, Thomas and Pinty, Bernard and Verstraete, Michel and Gobron, Nadine},
   year         = 2006,
   booktitle    = {Computational {{Methods}} in {{Transport}}},
@@ -370,9 +370,10 @@
   publisher    = {{Optical Society of America}},
   volume       = 19,
   number       = 20,
   pages        = {3427--3428},
   doi          = {10.1364/AO.19.003427},
   issn         = {2155-3165},
   url          = {https://www.osapublishing.org/ao/abstract.cfm?uri=ao-19-20-3427},
-  shortjournal = {Appl. Opt., AO},
+  shortjournal = {Appl. Opt., AO}
 }
+
```

### Comparing `eradiate-0.27.0rc0/docs/rst/contributing.rst` & `eradiate-0.27.0rc1/docs/rst/contributing.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/dependencies.rst` & `eradiate-0.27.0rc1/docs/rst/dependencies.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/developer_guide/design_atmosphere.rst` & `eradiate-0.27.0rc1/docs/rst/developer_guide/design_atmosphere.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/developer_guide/dev_install.rst` & `eradiate-0.27.0rc1/docs/rst/developer_guide/dev_install.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/developer_guide/factory_guide.rst` & `eradiate-0.27.0rc1/docs/rst/developer_guide/factory_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/developer_guide/lazy_loading.rst` & `eradiate-0.27.0rc1/docs/rst/developer_guide/lazy_loading.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/developer_guide/radiometric_kernel_interface.rst` & `eradiate-0.27.0rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/developer_guide/scene_generator.rst` & `eradiate-0.27.0rc1/docs/rst/developer_guide/scene_generator.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/developer_guide/update.rst` & `eradiate-0.27.0rc1/docs/rst/developer_guide/update.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/maintainer_guide.rst` & `eradiate-0.27.0rc1/docs/rst/maintainer_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/config.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/config.rst`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 ------------
 
 .. py:currentmodule:: eradiate.config
 
 .. data:: ENV
    :annotation: = str
 
-   Path to the Eradiate source code directory, if relevant. Takes the value of
-   the ``ERADIATE_SOURCE_DIR`` environment variable if it is set; otherwise
-   defaults to ``None``.
-
-.. data:: SOURCE_DIR
-   :annotation: = pathlib.Path or None
-
    Identifier of the environment in which Eradiate is used. Takes the value of
    the ``ERADIATE_ENV`` environment variable if it is set; otherwise defaults to
    ``"default"``.
 
+.. data:: SOURCE_DIR
+   :annotation: = pathlib.Path or None
+
+   Path to the Eradiate source code directory, if relevant. Takes the value of
+   the ``ERADIATE_SOURCE_DIR`` environment variable if it is set; otherwise
+   defaults to ``None``.
 
 .. py:currentmodule:: eradiate.config
 
 .. data:: settings
    :annotation: = dynaconf.Dynaconf
 
    Main settings data structure. It supports array and attribute indexing, both
@@ -37,16 +36,15 @@
 
       settings["some.key"]
       settings["SOME.KEY"]
       settings.some.key
       settings.SOME.KEY
 
    All settings have a default value specified by the
-   `default configuration file\
-   <https://github.com/eradiate/eradiate/blob/abs_db/src/eradiate/config/default.toml>`_
+   :ref:`default configuration file <sec-user_guide-config-default>`
    and can be overridden by the user from an ``eradiate.toml`` file, placed in
    the current working directory or higher. Each setting can also be overridden
    using `environment variables <https://www.dynaconf.com/envvars/>`_ with the
    ``ERADIATE_`` prefix.
 
    .. admonition:: Example
       :class: tip
```

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/data.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/data.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/eradiate_core.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/eradiate_core.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/experiments.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/experiments.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/factory.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/factory.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/index.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/kernel.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/kernel.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/pipelines.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/pipelines.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/scenes.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/scenes.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/spectral.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/spectral.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/srf_tools.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/srf_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/test_tools.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/test_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/reference_api/xarray.rst` & `eradiate-0.27.0rc1/docs/rst/reference_api/xarray.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/absorption.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/fig/bad_resolution.png` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/fig/good_resolution.png` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/fig/line.png` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/fig/line.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/heterogeneous.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/intro.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/molecular.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/molecular.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/basic_concepts.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/basic_concepts.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/conventions.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/conventions.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/data/absorption.rst` & `eradiate-0.27.0rc1/docs/rst/data/atmosphere_molecular_absorption.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,17 @@
-.. _sec-user_guide-data-absorption:
+.. _sec-data-molecular_absorption:
 
-Absorption data
-===============
+Atmosphere: Molecular absorption
+================================
 
-Absorption datasets tabulate the volume absorption coefficient of a gas mixture
-against spectral index, mixture's components' volume fraction, air pressure
-and air temperature.
-
-For monochromatic absorption datasets, the spectral index consists
-of a radiation wavelength or radiation wavenumber coordinate.
-
-For CKD absorption datasets, the spectral index consists of two coordinates:
-
-* the center of the spectral band (in wavelength or wavenumber space)
-* the absorption coefficient cumulative probability, or :math:`g`-point.
-
-Data access
------------
-
-Distributed absorption datasets are available from the
-`Eradiate store <http://eradiate.eu/data/store/>`_.
-
-.. note::
-
-   You can also plug in your own datasets, provided they comply with the
-   below specifications.
+Molecular absorption datasets tabulate the volume absorption coefficient of a
+gas mixture against the spectral coordinates, the volume fraction of the mixture
+components, air pressure and air temperature.
+Eradiate's built-in molecular absorption datasets are managed by the data store
+(see :ref:`sec-data-intro` for details).
 
 Specifications
 --------------
 
 Monochromatic
 ~~~~~~~~~~~~~
 
@@ -54,17 +37,17 @@
 
 one optional data variable:
 
 * ``error [w, ng]`` : relative error on atmosphere band-averaged transmittance,
 
 at least five :term:`dimension coordinates <dimension coordinate>`:
 
-* ``w`` : radiation wavelength or radiation wavenumber of the band center,
-* ``wbv`` : band wavelength bounds,
-* ``g`` : quadrature :math:`g`-point,
+* ``w`` : radiation wavelength or radiation wavenumber of the band center
+* ``wbv`` : band wavelength bounds
+* ``g`` : quadrature :math:`g`-point / absorption coefficient cumulative probability
 * ``x_M`` (where ``M`` is the molecule formula, e.g. ``x_H2O``, ``x_CO2``): gas
   mixture mole fractions (1 to :math:`N_M` coordinates where :math:`N_M` is the
   number of molecules in the mixture),
 * ``p`` : air pressure,
 * ``t`` : and air temperature,
 
 and, if the data variable ``error`` is present:
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/data/atmosphere_thermoprops.rst` & `eradiate-0.27.0rc1/docs/rst/data/atmosphere_thermoprops.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. _sec-user_guide-data-thermoprops:
+.. _sec-data-thermoprops:
 
-Atmosphere: thermophysical properties
+Atmosphere: Thermophysical properties
 =====================================
 
 An atmospheric thermophysical property data set provides the spatial variation
 of air pressure, air temperature, air number density and air constituents'
 mole fractions.
 
 Standard atmospheric profiles, including manipulation methods, are provided
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png` & `eradiate-0.27.0rc1/docs/rst/data/fig/p_interp_rerr_histo_65349.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/data/fig/pt_points.png` & `eradiate-0.27.0rc1/docs/rst/data/fig/pt_points.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png` & `eradiate-0.27.0rc1/docs/rst/data/fig/w_interp_rerr_histo_101325.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/data/solar_irradiance.rst` & `eradiate-0.27.0rc1/docs/rst/data/solar_irradiance.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-.. _sec-user_guide-data-solar_irradiance:
+.. _sec-data-solar_irradiance:
 
 Solar irradiance spectra
 ========================
 
-A solar irradiance spectrum dataset provides the Sun's irradiance
-spectrum at a Sun-Earth distance of 1 astronomical unit.
-Solar spectral irradiance data may come from observations—*e.g.* using a
-spectrometer onboard a satellite—or theoretical models such as the blackbody
-model, or from a combination of observation data and theoretical models.
-
-Data access
------------
-
-All solar irradiance spectrum datasets required by Eradiate are
-managed the data store (see :ref:`sec-user_guide-data-intro` for details).
+Solar irradiance spectrum datasets provides the solar irradiance spectrum at a
+Sun-Earth distance of 1 astronomical unit. Solar spectral irradiance data may
+come from observations—*e.g.* using a spectrometer onboard a satellite—or
+theoretical models such as the blackbody model, or from a combination of
+observation data and theoretical models. Solar irradiance data is managed by the
+data store (see :ref:`sec-data-intro` for details).
 
 Identifier format
 ^^^^^^^^^^^^^^^^^
 
 Identifiers for solar irradiance spectrum datasets (except ``blackbody_sun``)
 are constructed based on the format ``{author}_{year}[-{extra}]`` where:
 
@@ -307,19 +302,19 @@
 A version of the ``thuillier_2003`` spectrum extrapolated to 2500 nm so that it
 covers the wavelength range from 200 to 2500 nm.
 The figure below illustrates the original and extrapolated versions and
 highlights the extrapolation region.
 
 .. only:: latex
 
-   .. image:: ../../../fig/data/data/srf/thuillier_2003_extrapolated.png
+   .. image:: /fig/data/data/srf/thuillier_2003_extrapolated.png
 
 .. only:: not latex
 
-   .. image:: ../../../fig/data/data/srf/thuillier_2003_extrapolated.svg
+   .. image:: /fig/data/data/srf/thuillier_2003_extrapolated.svg
 
 .. note::
 
    For the reference, we provide below the values of the integrated original
    and extrapolated solar irradiance spectra, evaluated by integrating the
    irradiance spectrum along wavelength using the trapezoidal rule.
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/data/srf.rst` & `eradiate-0.27.0rc1/docs/rst/data/srf.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 A spectral response function data set provide the spectral response of a
 given instrument on a specific platform and in a specific spectral band.
 
 Data access
 -----------
 
 All spectral response function data sets required by Eradiate are
-managed the data store (see :ref:`sec-user_guide-data-intro` for details).
+managed the data store (see :ref:`sec-data-intro` for details).
 
 .. _sec-user_guide-data-srf-naming_convention:
 
 Identifier format
 ^^^^^^^^^^^^^^^^^
 
 Identifiers for spectral response function are built according to the format
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/index.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 .. _sec-user_guide:
 
-User guides
-===========
+User guide
+==========
 
-.. toctree::
-   :maxdepth: 1
-
-   install
-   basic_concepts
-   conventions
-   package_structure
-   onedim_experiment
-   spectral_discretization
-   unit_guide_user
-   scene_loader
-   data/index
+The user guide introduces a range of topics explaining parts of Eradiate from a
+user's perspective. Reading this material is not necessary to learn how to run
+simulations with Eradiate—for this, it is advised to refer to the
+:ref:`sec-tutorials`.
 
 What is Eradiate?
 -----------------
 
 Eradiate is a modern radiative transfer model for Earth observation
 applications. It primarily targets calibration/validation applications and
 focuses on delivering highly accurate results.
@@ -28,30 +20,46 @@
 runs and collect results.
 
 Features: What can I do with Eradiate?
 --------------------------------------
 
 Perform monochromatic and band simulations.
     Eradiate can simulate radiative transfer for a single wavelength or a
-    spectral band (using the correlated *k*-distribution method) between 280
-    and 2400 nm.
+    spectral band (using the correlated *k*-distribution method) between in the
+    solar reflective domain.
 
 Perform simulations on one-dimensional scenes.
-    Eradiate can simulate top-of-atmosphere radiance and reflectance on 1D
-    scenes with plane parallel geometry.
-    These scenes consist of a smooth surface underneath an atmosphere including
-    gases and an arbitrary number of aerosol layers. Under the hood, Eradiate
+    Eradiate can simulate top-of-atmosphere and in-situ radiance and reflectance
+    on 1D scenes consisting of a smooth surface underneath an atmosphere
+    including gases and an arbitrary number of aerosol layers, and discretized
+    into uniform, horizontally invariant layers. Under the hood, Eradiate
     performs these simulations using 3D scenes carefully designed to produce
     results similar to what one would get with 1D geometries.
 
-    Eradiate has experimental support for spherical shell geometries (validation
-    is in progress).
+    Eradiate supports plane-parallel and spherical-shell geometries.
 
 Perform simulations on three-dimensional scenes.
-    Eradiate can simulate top-of-canopy/atmosphere radiance on 3D scenes
-    consisting of a vegetated ground patch with or without atmosphere above it
-    (plane parallel geometry only).
+    Eradiate can simulate top-of-canopy/atmosphere radiance and in-situ radiance
+    and reflectance on 3D scenes consisting of a vegetated ground patch, with or
+    without atmosphere above it.
 
 .. seealso::
 
    For a full list of features, head to
    `our website <https://www.eradiate.eu/>`_.
+
+Guides
+------
+
+.. toctree::
+   :maxdepth: 1
+
+   install
+   basic_concepts
+   config
+   package_structure
+   atmosphere_experiment
+   dem_experiment
+   canopy_scene_loader
+   spectral_discretization
+   conventions
+   unit_guide_user
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/install.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 This will install the latest stable version of Eradiate, along with all the
 dependencies necessary to run it. If you want to install the latest development
 version, please refer to the :ref:`sec-developer_guide-dev_install`.
 
 .. warning::
 
    Eradiate uses a modified version of the Mitsuba 3 renderer, distributed on
-   PyPI as the ``eradiate-mitsuba``. That package conflicts with the ``mitsuba``
+   PyPI as ``eradiate-mitsuba``. That package conflicts with the ``mitsuba``
    package distributed by the Mitsuba team and both cannot be installed
    together.
 
    The ``eradiate`` PyPI package lists ``eradiate-mitsuba`` as a dependency. A
    normal usage pattern should result in the correct flavour of Mitsuba being
    installed automatically. However, if you are installing Eradiate to an
    environment already containing a Mitsuba installation, be sure to remove it
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/onedim_experiment.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/atmosphere_experiment.rst`

 * *Files 13% similar despite different names*

```diff
@@ -48,33 +48,34 @@
 Plane parallel [:class:`.PlaneParallelGeometry`, ``plane_parallel``]
     By default, the surface and atmosphere are assumed translationally invariant
     in the X and Y directions. This approximation provides satisfactory accuracy
     in many situations.
 
 Spherical shell [:class:`.SphericalShellGeometry`, ``spherical_shell``]
     When this geometry configuration is used, the scene is built with a
-    rotationally invariant symmetry. This configuration accounts for the
-    roundedness of the planet. **This feature is experimental and is being
-    validated.**
+    rotationally invariant symmetry. This configuration accounts for planetary
+    curvature.
 
 Illumination [``illumination``]
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The one-dimensional experiment currently supports only one illumination type.
-
 Directional illumination [:class:`.DirectionalIllumination`, ``directional``]
     An infinitely distant emitter which emits light in a single direction
     (angular Dirac delta distribution of incoming radiance). This type of
-    illumination is used to simulate incoming Solar radiation. By default, a
-    Solar spectrum is automatically selected.
+    illumination is used to simulate incoming solar radiation.
+
+Astronomical object [:class:`.AstroObjectIllumination`, ``astro_object``]
+    An infinitely distant emitter that emits light in a conical section of the
+    angular space. It aims at providing a more realistic representation of
+    natural illuminants than the directional emitter.
 
 In addition, this angular distribution can be associated a spectrum.
 A variety of pre-defined Solar irradiance spectra are defined (see
-:ref:`sec-user_guide-data-solar_irradiance` for a complete list of shipped
-irradiance spectrum datasets).
+:ref:`sec-data-solar_irradiance` for a complete list of shipped irradiance
+spectra).
 
 Measures [``measures``]
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 This experiment currently supports the computation of radiative quantities at
 the top of the atmosphere. This parameter can be specified as a single measure,
 or as a list of measures.
@@ -102,15 +103,15 @@
     TOA bidirectional reflectance factor (TOA BRF) [``brf``]
         The TOA BRDF normalised by the BRDF of a non-absorbing diffuse
         (Lambertian) surface.
 
 Distant fluxmeter [:class:`.DistantFluxMeasure`, ``distant_flux``]
     This measure records the flux leaving the scene (in W/m²/nm) over the entire
     hemisphere. It is mostly used to compute the scene albedo. The following
-    quantities are available from the results dataset:
+    quantities are available from the result dataset:
 
     Radiosity [``radiosity``]
         The flux leaving the scene in W/m²/nm.
 
     Albedo [``albedo``]
         The total scene albedo.
 
@@ -146,54 +147,27 @@
     BRDF, parametrised by a reflectance parameter.
 
 Rahman-Pinty-Verstraete (RPV) surface [:class:`.RPVBSDF`, ``rpv``]
     This reflection model features an anisotropic behaviour and is commonly
     used for land surface reflection modelling. Eradiate implements several
     variants of it with 3 or 4 parameters.
 
+Ross thick-Li sparse (RTLS) surface [:class:`.RTLSBSDF`, ``rtls``]
+    This reflection model is commonly used in remote sensing applications.
+
+Hapke surface [:class:`.HapkeBSDF`]
+    A reflection model specialized for bare soil.
+
 Black surface [:class:`.BlackBSDF`, ``black``]
     The black surface absorbs all incoming radiation, irrespective of
     incident angle or wavelength.
 
-Digital elevation model [``dem``]
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-Eradiate extends the standard functionalities of one-dimensional simulations with
-digital elevation models (DEM). A three-dimensional surface can be defined with the ``dem``
-parameter. The DEM can be defined in several ways and it can be used with any BSDF type
-mentioned in the surface section above. Since a DEM surface model always has a finite
-horizontal extent, Eradiate adds horizontal elements to the edge of the DEM surface
-to prevent rays from escaping under it. The remaining surface area outside of the DEM is
-covered with the surface specified in the ``surface`` section.
-
-Note that Eradiate does not adjust the horizontal level of the flat surface automatically.
-If the DEM contains elevation values below the flat surface level (0m per default), the 3D
-surface will intersect the flat surface and the areas below the flat surface's level will
-be obscured by it.
-
-There are three ways to define a DEM geometry:
-
-An xarray DataArray [:meth:`.DEMSurface.from_dataarray`]
-    A DataArray defining a digital elevation model needs to have two coordinates named
-    `lat` for the latitude and `lon` for the longitude, specified in degrees and the
-    elevation data specified in kernel units of length.
-
-Triangulated meshes [:class:`.FileMesh`, ``file_mesh``]
-    To define the DEM using a triangulated mesh users can supply either a .obj file
-    or a .ply file. The mesh file will be interpreted as kernel units of length.
-    In this case no constructor method is used. Instead the `shape` member of the
-    `dem` class is directly defined with this mesh shape.
-
-Analytical functions [:meth:`.DEMSurface.from_analytical`]
-    Digital elevation models can be defined using functions, which take an x and
-    y position and return the corresponding elevation value.
-
 Result output
 -------------
 
-The :meth:`.AtmosphereExperiment.run` method stores the computed results in the
-``results`` attribute as a dictionary mapping measure identifiers to a
-:class:`~xarray.Dataset` object. Each data set has one variable for each
-computed physical quantity (*e.g.* spectral irradiance, leaving radiance, BRDF
-and BRF for the ``distant`` measure). Results can then be easily exported to
-files (*e.g.* NetCDF) and visualised using xarray's integrated plotting
-features or external plotting components.
+When running an experiment with the :func:`eradiate.run` function, the computed
+results are stored in the ``results`` attribute as a dictionary mapping measure
+identifiers to a :class:`~xarray.Dataset` object. Each data set has one variable
+for each computed physical quantity (*e.g.* spectral irradiance, leaving
+radiance, BRDF and BRF for the ``distant`` measure). Results can then be easily
+exported to files (*e.g.* NetCDF) and visualised using xarray's integrated
+plotting features or external plotting components.
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/package_structure.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/package_structure.rst`

 * *Files 7% similar despite different names*

```diff
@@ -27,74 +27,73 @@
     illumination and measures in the scene on which you'll run your radiative
     transfer simulation.
 
 Experiments [:mod:`eradiate.experiments`]
     In this package, you will find interfaces to trigger simulation runs,
     including pre- and post-processing operations.
 
+Command-line interface [:mod:`eradiate.cli`]
+    This package contains the implementation of the Eradiate command-line
+    interface.
+
 Radiometric kernel
 ------------------
 
 Kernel [:mod:`eradiate.kernel`]
     This module provides functionality related with Eradiate's radiometric
     kernel Mitsuba.
 
-Data handling and visualisation
+Data handling and visualization
 -------------------------------
 
 Data handling [:mod:`eradiate.data`]
     This package serves data shipped with Eradiate.
 
 Post-processing pipeline definitions [:mod:`eradiate.pipelines`]
     This package provides a post-processing pipeline framework used to convert
     raw sensor results yielded by kernel sensors to quantities of interest for
     Earth observation applications (*e.g.* reflectance). The data is stored as
     xarray labelled arrays (:term:`Dataset`).
 
-xarray utility functions [:mod:`eradiate.xarray`]
-    Various support components taking advantage of the xarray library.
-
 Plotting [:mod:`eradiate.plot`]
     This module defines optional utility functions to create
     `Matplotlib <https://matplotlib.org>`_-based visualisations of Eradiate's
     input and output data.
 
 Physical properties
 -------------------
 
 Radiative properties [:mod:`eradiate.radprops`]
     This package provides abstractions used to define radiative properties used
     to create scenes.
 
-Thermosphysical properties [:mod:`eradiate.thermoprops`]
-    This package provides abstractions used to define thermophysical properties
-    of scene objects. The output of its components are generally used as input
-    of components responsible for radiative property computation.
+Other support components
+------------------------
 
 Numerical constants [:mod:`eradiate.constants`]
     Various numerical constants used throughout the code base.
 
-Other support components
-------------------------
+Class writing facilities [``eradiate.{`` :mod:`~eradiate.attrs`, :mod:`~eradiate.converters`, :mod:`~eradiate.validators`, :mod:`~eradiate._factory` ``}``]
+    These components are part of Eradiate's core class writing system. It relies
+    on the `attrs <https://www.attrs.org>`_ library, extended for `Pint <https://pint.readthedocs.io>`_
+    compatibility by the `Pinttrs <https://pinttrs.readthedocs.io>`_ library.
 
-Unit support [:mod:`eradiate.units`]
-    Various utility functions and data variables used to safely handle unit
-    conversions in Eradiate.
+Exceptions [:mod:`eradiate.exceptions`]
+    Exception and warning definitions.
 
 Math support [``eradiate.{`` :mod:`~eradiate.frame`, :mod:`~eradiate.quad`, :mod:`~eradiate.warp` ``}``]
     For the cases where Eradiate's math dependencies and kernel are not
     enough, additional mathematical tools are provided.
 
 Random number generation [:mod:`eradiate.rng`]
     Support components for fine control of random number generation.
 
-Exceptions [:mod:`eradiate.exceptions`]
-    Exception and warning definitions.
+Unit support [:mod:`eradiate.units`]
+    Various utility functions and data variables used to safely handle unit
+    conversions in Eradiate.
 
-Class writing facilities [``eradiate.{`` :mod:`~eradiate.attrs`, :mod:`~eradiate.converters`, :mod:`~eradiate.validators`, :mod:`~eradiate._factory` ``}``]
-    These components are part of Eradiate's core class writing system. It relies
-    on the `attrs <https://www.attrs.org>`_ library, extended for `Pint <https://pint.readthedocs.io>`_
-    compatibility by the `Pinttrs <https://pinttrs.readthedocs.io>`_ library.
+xarray utility functions [:mod:`eradiate.xarray`]
+    Various support components taking advantage of the xarray library.
 
 Miscellaneous [:mod:`eradiate.util`]
     Other support components which don't fit in any of the aforementioned
     classification entries.
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/scene_loader.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/canopy_scene_loader.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-.. _sec-user_guide-scene_loader:
+.. _sec-user_guide-canopy_scene_loader:
 
-Scene loader
-============
+Canopy scene loader
+===================
 
 This page presents the canopy scene loader. A scene is composed by a
 ``scenario.json`` file and a set of mesh files. The ``scenario.json`` file
 contains the description of the scene, including the properties of the surface
 and canopies within the scene. The mesh files contain the geometry of the canopy
 elements.
 
@@ -228,42 +228,42 @@
                        "type": "interpolated",
                    }
                ),
            },
        },
    }
 
+.. _sec-user_guide-canopy_scene_loader-rami_scenes:
 
 RAMI benchmark scenarios
 ------------------------
 
 We provide a specific loader for scenes derived from the
 `RAMI-V scene list <https://rami-benchmark.jrc.ec.europa.eu/_www/phase_descr.php?strPhase=RAMI5>`_.
-These pre-configured are available for use and downloaded upon request via the
-datastore.\ [#sn2]_ These are downloaded when a specific scenario is requested via the
-datastore. Due to their size and the number of files they contain, the scenarios
-are downloaded in a compressed format and, by default, extracted to the current
-working directory. The extracted files are then used to load the scenario. To
-change the default location for the extracted files, set the appropriate
-parameter in the :func:`.load_rami_scenario` function.
-
-.. [#sn2] We thank the `DART <https://dart.omp.eu/>`_ team for allowing us to
-   use their 3D model files to derive our scene models.
+The list of pre-configured scenes is available in the
+:doc:`data guide </rst/data/generated/rami_scenes>`. Shipped data are downloaded
+automatically when a specific scenario is requested via the datastore. Due to
+their size and the number of files they contain, the scenarios are downloaded in
+a compressed format and, by default, extracted to the current working directory.
+The extracted files are then used to load the scenario. To change the default
+location for the extracted files, set the appropriate parameter in the
+:func:`.load_rami_scenario` function.
 
 .. code-block:: python
 
     from pathlib import Path
 
     import eradiate
     from eradiate.experiments import CanopyExperiment
     from eradiate.scenes.biosphere import load_rami_scenario
     from eradiate.units import unit_registry as ureg
 
     eradiate.set_mode("mono")
 
+    # Use the RAMI ID to reference the scenario
     scenario_data = load_rami_scenario("HOM30_DIS_ED0")
 
     scenario = CanopyExperiment(
         **scenario_data,
         measures={
             "type": "perspective",
             "film_resolution": (50, 50),
```

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/spectral_discretization.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/spectral_discretization.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/rst/user_guide/unit_guide_user.rst` & `eradiate-0.27.0rc1/docs/rst/user_guide/unit_guide_user.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/src/reference_cli.md` & `eradiate-0.27.0rc1/docs/src/reference_cli.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ```console
 $ eradiate [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
-* `--log-level [CRITICAL|ERROR|WARNING|INFO|DEBUG|NOTSET]`: Set log level.  [default: LogLevel.WARNING]
+* `--log-level [CRITICAL|ERROR|WARNING|INFO|DEBUG|NOTSET]`: Set log level.  [default: WARNING]
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `data`: Manage data.
@@ -56,19 +56,20 @@
 
 ```console
 $ eradiate data fetch [OPTIONS] [FILE_LIST]...
 ```
 
 **Arguments**:
 
-* `[FILE_LIST]...`: An arbitrary number of relative paths to files to be retrieved from the data store or file group specifications. If unset, the list of files is read from a YAML file which can be specified by using the ``--from-file`` option and defaults to ``$ERADIATE_SOURCE_DIR/data/downloads_all.yml`` a production environment and ``$ERADIATE_SOURCE_DIR/data/downloads_minimal.yml`` in a development environment.
+* `[FILE_LIST]...`: An arbitrary number of relative paths to files to be retrieved from the data store or file list specifications. If unset, the list of files is read from a YAML file which can be specified by using the ``--from-file`` option, if it is specified. Otherwise, it defaults to ``all`` in a production environment and ``minimal`` in a development environment.
 
 **Options**:
 
 * `-f, --from-file TEXT`: Optional path to a file list (YAML format). If this option is set, the FILES argument(s) will be ignored.
+* `-l, --list`: List built-in file lists and exit.
 * `--help`: Show this message and exit.
 
 #### `eradiate data info`
 
 Display information about data store configuration.
 
 **Usage**:
```

### Comparing `eradiate-0.27.0rc0/docs/src/release_notes/index.md` & `eradiate-0.27.0rc1/docs/src/release_notes/index.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/src/release_notes/v0.23.x_and_older.md` & `eradiate-0.27.0rc1/docs/src/release_notes/v0.23.x_and_older.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/src/release_notes/v0.24.x.md` & `eradiate-0.27.0rc1/docs/src/release_notes/v0.24.x.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/docs/src/release_notes/v0.25.x.md` & `eradiate-0.27.0rc1/docs/src/release_notes/v0.25.x.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   yourself. Of course, the built-in profiles are still available.
   Thermophysical property handling is now externalized to a new library
   [Joseki](https://github.com/rayference/joseki). Joseki's output format is
   [documented here](https://rayference.github.io/joseki/2.5/explanation/#dataset-schema).
 * We added an interface to customize atmospheric absorption data. If you need to
   fit the data for a specific use case (*e.g.* to work with an atmosphere from
   another planet than Earth), it is now possible. The data format is described
-  in our {ref}`data guide <sec-user_guide-data-absorption>`.
+  in our {ref}`data guide <sec-data-molecular_absorption>`.
 * The quadrature rule used for spectral discretization in CKD mode can now be
   specified in a flexible way. The number of quadrature points is no longer set
   to a built-in value, and the atmospheric absorption datasets ship metadata
   that can be leveraged to dynamically select a quadrature that minimizes the
   error on atmospheric transmittance.
 
 ```{important}
```

### Comparing `eradiate-0.27.0rc0/docs/src/release_notes/v0.26.x.md` & `eradiate-0.27.0rc1/docs/src/release_notes/v0.26.x.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   post-processing, improves its flexibility and maintainability. While this
   should not have a noticeable impact from a user's perspective, it will allow
   the implementation of several features prevented by the old pipeline system.
   A {doc}`tutorial </tutorials/advanced/postprocessing_pipelines>` showcases a
   few features of this new system.
 * We introduced a new scene loader based on JSON files designed to facilitate
   the loading of mesh-based canopy scenes. The scene loader is described in a
-  {ref}`user guide page <sec-user_guide-scene_loader>`, and a simplified
+  {ref}`user guide page <sec-user_guide-canopy_scene_loader>`, and a simplified
   interface automating the loading of the RAMI-V scenarios is provided.
 
 ### Removed
 
 * ⚠️ Drop support of Python 3.8 ({ghpr}`382`): Eradiate now requires Python 3.9+.
 
 ### Added
```

### Comparing `eradiate-0.27.0rc0/docs/src/release_notes/v0.27.x.md` & `eradiate-0.27.0rc1/docs/src/release_notes/v0.27.x.md`

 * *Files 11% similar despite different names*

```diff
@@ -18,25 +18,37 @@
 * Introduced a new {class}`.AbsorptionDatabase` abstraction in charge of
   managing atmospheric molecular absorption data ({ghpr}`397`).
 * Eradiate can now be configured using TOML files ({ghpr}`397`).
 * The `eradiate data fetch` command-line interface now accepts keywords to
   facilitate absorption database downloads ({ghpr}`397`).
 * Gaussian SRF datasets can now be dynamically generated using the
   :func:`.srf_tools.make_gaussian` function ({ghpr}`401`).
-* All `.Shape` classes now support a `to_world` member, which defines an arbitrary
-  transformation of the object.
+* All `.Shape` classes now support a `to_world` member, which defines an
+  arbitrary transformation of the object ({ghpr}`381`).
+* The eradiate data fetch command is extended with the possibility to fetch
+  groups of files (*e.g.* `eradiate data fetch monotropa`) ({ghpr}`405`).
 
 ### Changed
 
 * ⚠️ Most settings are now accessed through the :attr:`.settings` mapping
   ({ghpr}`397`).
+* 📖 The Data documentation content is extracted from the user guide and moved
+  to its own section ({ghpr}`405`).
 
 ### Fixed
 
 * Large absorption databases are now handled with little to no performance
   penalty ({ghpr}`397`).
+* DEM Surfaces would not behave correctly when used with a
+  {class}`.SphericalShellGeometry` ({ghpr}`402`).
+* CKD bin selection no longer crashes if theoretically identical min and max
+  bounds of two adjacent bins have an actual mismatch due to floating point
+  precision issues ({ghpr}`406`).
+* The SRF weighting operation is removed from monochromatic post-processing
+  pipelines ({ghpr}`406`).
 
 ### Internal changes
 
 * 🖥️ Settings are now powered by the Dynaconf library ({ghpr}`397`).
 * 🖥️ Renamed and refactored atmosphere fixtures for performance and clarity
   ({ghpr}`397`).
+* 🖥️ Reorganized test code and fixtures for clarity ({ghpr}`399`).
```

### Comparing `eradiate-0.27.0rc0/pyproject.toml` & `eradiate-0.27.0rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -32,23 +32,21 @@
   "ignore:numpy.ndarray size changed, may indicate binary incompatibility:RuntimeWarning",
   # Remove the following when Jupyter stops issuing those
   "ignore:Jupyter is migrating its paths to use standard platformdirs"
 ]
 testpaths = "tests"
 
 [tool.ruff]
-ignore = ["E501", "F821"]
-select = ["I", "F", "E"]
 src = ["src", "tests"]
 
-[tool.ruff.isort]
-relative-imports-order = "closest-to-furthest"
-
-[tool.ruff.lint.per-file-ignores]
-"*.ipynb" = ["E402"]
+[tool.ruff.lint]
+ignore = ["E501", "F821"]
+isort = {relative-imports-order = "closest-to-furthest"}
+per-file-ignores = {"*.ipynb" = ["E402"]}
+select = ["I", "F", "E"]
 
 [tool.setuptools]
 include-package-data = true  # Required because of package data
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements/pip/dependencies.txt"]}
```

### Comparing `eradiate-0.27.0rc0/requirements/_utils.py` & `eradiate-0.27.0rc1/requirements/_utils.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-dependencies-linux-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-dependencies-linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 75a4f851fadaade2f108f24f50388a2b911e9a6bf3b74d5e299028f50c27c755
+# input_hash: 7b572c9cec772c110dbacafccb8d9cfe2c58d334785cc68f78608da0a8b164be
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda#2f4327a1cbe7f022401b236e915a5fef
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda#f6f6600d18a4047b54f803cf708b868a
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda#10569984e7db886e4f1abc2b47ad79a1
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda#3cfab3e709f77e9f1b3d380eb622494a
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-4_cp39.conda#bfe4b3259a8ac6cdf0037752904da6a7
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda#aae89d3736661c36a5591788aebd0817
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda#df88796bd09a0d2ed292e59101478ad8
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.11-hd590300_1.conda#0bb492cca54017ea314b809b1ee3a176
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
@@ -31,22 +31,22 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-h43f5ff8_6.conda#e54a5ddc67e673f9105cf2a2e9c070b0
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.4.0-hd590300_0.conda#b26e8aa824079e1be0294e7152ca4559
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.32.6-h59595ed_0.conda#9160cdeb523a1b20cf8d2a0bf821f45d
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda#97da8860a0da5413c7c98a3b3838a645
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda#9d731343cff6ee2e5a25c4a091bf8e2a
@@ -67,36 +67,36 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.69-h0f662aa_0.conda#25cb5999faa414e5ccb2c1388f62d3d5
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_6.conda#3666a850342f8f3be88f9a93d948d027
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda#b3316cbe90249da4f8e84cd66e1cc55b
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_2.conda#9a3a42df8a95f65334dfc7b80da1195d
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
 https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.3.0-hf1915f5_4.conda#784a4df6676c581ca624fbe460703a6d
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_6.conda#9342e7c44c38bea649490f72d92c382d
 https://conda.anaconda.org/conda-forge/linux-64/libllvm15-15.0.7-hb3ce162_4.conda#8a35df3cbc0c8b12cc8af9473ae75eef
 https://conda.anaconda.org/conda-forge/linux-64/libllvm18-18.1.3-h2448989_0.conda#927b6d6e80b2c0d4405a58b61ca248a3
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
 https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.3.0-hca2cd23_4.conda#1b50eebe2a738a3146c154d2eceaa8b6
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.98-h1d7d5a4_0.conda#54b56c2fdf973656b748e0378900ec13
 https://conda.anaconda.org/conda-forge/linux-64/python-3.9.19-h0755675_0_cpython.conda#d9ee3647fbd9e8595b8df759b2bbefb8
@@ -114,40 +114,40 @@
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_4.conda#c9deba4959ea5b5f72f1e3e4a71ae014
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_6.conda#a9d23c02485c5cf055f9ac90eb9c9c63
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py39h7633fee_1.conda#c9f74d717e5a2847a9f8b779c54130f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang-cpp15-15.0.7-default_h127d8a8_5.conda#d0a9633b53cdc319b8a1a532ae7822b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-18.1.3-default_h5d6823c_0.conda#5fff487759736b275dc3e4a263cac666
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h4637d8d_4.conda#d4529f4dff3057982a7617c7ac58fde3
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
-https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.48-h71f35ed_0.conda#4d18d86916705d352d5f4adfb7f0edd3
+https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.49-h4f305b6_0.conda#dfcfd72c7a430d3616763ecfbefe4ca9
 https://conda.anaconda.org/conda-forge/linux-64/libpq-16.2-h33b98f1_1.conda#9e49ec2a61d02623b379dc332eb6889d
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py39hd1e30aa_0.conda#b1961e70cfe8e1eac243faf933d1813f
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py39hd1e30aa_0.conda#1e865e9188204cdfb1fd2531780add88
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.1.0-py39hd1e30aa_0.conda#1da984bbb6e765743e13388ba7b7b2c8
@@ -155,15 +155,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.41-hd590300_0.conda#81f740407b45e3f9047b3174fa94eb9e
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py39hd1e30aa_0.conda#79f5dd8778873faa54e8f7b2729fe8a6
-https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_4.conda#5521382ee30b96b35eb0037fc3c4f2b4
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_6.conda#a1e026a82a562b443845db5614ca568a
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.3-hd590300_0.conda#32d16ad533c59bb0a3c5ffaf16110829
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.2-hc60ed4a_1.conda#ef1910918dd895516a769ed36b5b3a4e
@@ -175,35 +175,35 @@
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py39hd1e30aa_0.conda#2289054e90cf07e35280bbe798811dc8
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.12-py39h3d6467e_0.conda#e667a3ab0df62c54e60e1843d2e6defb
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.24.1-h98fc4e7_1.conda#b04b5cdf3ba01430db27979250bc5a1d
-https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.4.0-h3d44ed6_0.conda#27f46291a6aaa3c2a4f798ebd35a7ddb
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-255-h3516f8a_1.conda#3366af27f0b593544a6cd453c7932ac5
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py39h474f0d3_0.conda#aa265f5697237aa13cc10f53fa8acc4f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.12.2-py39h3d6467e_5.conda#93aff412f3e49fdb43361c0215cbd72d
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py39h44dd56e_0.conda#baea2f5dfb3ab7b1c836385d2e1daca7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py39h7633fee_0.conda#bdc188e59857d6efab332714e0d01d93
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.24.1-hfa15dee_1.conda#a6dd2bbc684913e2bef0a54ce56fcbfb
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.1-py39hddac248_0.conda#85293a042c24a08e71b7608ee66b6134
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.2-py39hddac248_0.conda#259c4e76e6bda8888aefc098ae1ba749
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-17.0-hb77b528_0.conda#07f45f1be1c25345faddb8db0de8039b
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py39h474f0d3_0.conda#46ae0ecba9726ab4fa44c78fefa522cf
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py39he9076e7_0.conda#1919384a8420e7bb25f6c3a582e0857c
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py39h4282601_100.conda#d2809fbf0d8ae7b8ca92c456cb44a7d4
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-hc9dc06e_21.conda#b325046180590c868ce0dbf267b82eb8
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.9-py39h52134e7_5.conda#e1f148e57d071b09187719df86f513c1
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.8.4-py39hf3d152e_0.conda#c66d2da2669fddc657b679bccab95775
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-dependencies-osx-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-dependencies-osx-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: eb11a2d8eb89786097a27487924072f85f65d5922f61721c5dd27c31fd301a83
+# input_hash: 9a27640db306d64567b7c93c59d01122bcbcac0a9f767a7403acc09f23ec469e
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda#6097a6ca9ada32699b5fc4312dd6ef18
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.28.1-h10d778d_0.conda#d5eb7992227254c0e9a0ce71151f0079
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda#f2eacee8c33c43692f1ccfd33d0f50b1
 https://conda.anaconda.org/conda-forge/osx-64/icu-73.2-hf5e326d_0.conda#5cc301d759ec03f28328428e28f65591
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.1.0-h0dc2134_1.conda#9e6c31441c9aa24e41ace40d6151aab6
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.20-h49d49c5_0.conda#d46104f6a896a0bc6a1d37b88b2edf5c
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-h10d778d_2.conda#899db79329439820b7e8f8de41bca902
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hd75f5a5_2.conda#6c3628d047e151efba7cf08c5e54d1ca
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-3.0.0-h0dc2134_1.conda#72507f8e3961bc968af17435060b6dd6
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.2-h10d778d_1.conda#1ff09ca6e85ee516442a6a94cdfc7065
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.4.0-h10d778d_0.conda#b2c0047ea73819d992484faacbbe1c24
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-18.1.3-hb6ac08f_0.conda#506f270f4f00980d27cc1fc127e0ed37
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda#50f28c512e9ad78589e3eab34833f762
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.9-4_cp39.conda#2d9f6c00555127a9058cfa955adf1090
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
@@ -27,17 +27,17 @@
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.1.3-h73e2aa4_0.conda#66d3c1f6dd4636216b4fca7a748d50eb
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.1.0-h0dc2134_1.conda#9ee0bab91b2ca579e10353738be36063
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.1.0-h0dc2134_1.conda#8a421fe09c6187f0eb5e2338a8a8be6d
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-13.2.0-h2873a65_3.conda#e4fb4d23ec2870ff3c40d10afe305aec
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda#65dcddb15965c9de2c0365cb14910532
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda#086f56e13a96a6cfb1bf640505ae6b70
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda#68e462226209f35182ef66eda0f794ff
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda#bd85e0ca9e1ffaadc3b56079fd956035
+https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda#50b997370584f2c83ca0c38e9028eab9
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda#570a6f04802df580be529f3a72d2bbf7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.2.0-h6dc393e_1.conda#9c322ec36340610fcf213b72999b049e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda#bf830ba5afc507c6232d4ef0fb1a882d
 https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda#80abc41d0c48b82fe0f04e7f42f5cb7e
@@ -58,32 +58,32 @@
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.5-py39h8ee36c8_1.conda#6072db04642b21329b0502a177ec18bf
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.16-ha2f27b4_0.conda#1442db8f03517834843666c422238c9b
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.7.1-h726d00d_0.conda#fa58e5eaa12006bc3289a71357bef167
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.27-openmp_hfef2a42_0.conda#00237c9c7f2cb6725fe2960680a6e225
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.2-h7310d3a_0.conda#05a14cc9d725dd74995927968d6547e3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.8-py39ha09f3b3_0.conda#835c656934865805c0b02dbff74fe5b7
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py39ha09f3b3_0.conda#4541517b5a605bf45d4a5fb074bb4cf5
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.1.0-py39hdc70f33_0.conda#ede122e9ef2775a8879063d9d3ee819f
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
@@ -110,17 +110,17 @@
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.26.4-py39h28c39a1_0.conda#1b07000dc6aed4a69e91107dac4464d3
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.3-py39h5b4affa_0.conda#20fd617b1f9fcefe5ec1577d38ae7bdb
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.2.1-py39h0ca7971_0.conda#a4c478d3b64c81d1742dc8073e4996b6
-https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.1-py39haf03413_0.conda#d29dc35b665029951dae988810f84508
+https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.2-py39haf03413_0.conda#11225cf1f769af217ffc01f0a21d40fa
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.13.0-py39h0ed1e0f_0.conda#3a4d0af4fe2006bedc33ca61e9a0b4d6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.8.4-py39h7070ae8_0.conda#cb9e1f8aff1f759b9685e908f9dc0a5b
 https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.5-nompi_py39h824b2b2_100.conda#07525171115894fe9c4aba755460c51a
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.8.4-py39h6e9494a_0.conda#371fe0f738d9f3baa20cf06656b78b0a
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-dependencies-win-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-dependencies-win-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: ae79d6c8f77a4025f83607ea33add72fb0e7594c0e2541cb8ba67c0c9de75466
+# input_hash: f21962fd543545651a0c09a2f835c6abf6accf18b527b98395fa2fc50f5c5acd
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda#63da060240ab8087b60d1357051ea7d6
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda#30ebb9fd99666d8b8675fcee541a09f3
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda#c66eb2fd33b999ccc258aef85689758e
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-0.22.5-h5728263_2.conda#75a6982b9ff0a8db0f53303527b07af8
 https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2#b0309b72560df66f71a9d5e34a5efdfa
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.9-4_cp39.conda#948b0d93d4ab1372d8fd45e1560afd47
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-devel-0.22.5-h5728263_2.conda#8377da2cc31200d7181d2e48d60e4c7b
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2#53a1c73e1e3d185516d7e3af177596d9
@@ -22,16 +22,16 @@
 https://conda.anaconda.org/conda-forge/win-64/libaec-1.1.3-h63175ca_0.conda#8723000f6ffdbdaef16025f0a01b64c5
 https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.1.0-hcfcfb64_1.conda#f77f319fb82980166569e1280d5b2864
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.20-hcfcfb64_0.conda#b12b5bde5eb201a1df75e49320cc938a
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda#e1eb10b1cca179f2baa3601e4efc8712
 https://conda.anaconda.org/conda-forge/win-64/libjpeg-turbo-3.0.0-hcfcfb64_1.conda#3f1b948619c45b1ca714d60c7389092c
 https://conda.anaconda.org/conda-forge/win-64/libogg-1.3.4-h8ffe710_1.tar.bz2#04286d905a0dcb7f7d4a12bdfe02516d
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda#f95359f8dc5abf7da7776ece9ef10bc5
-https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.2-hcfcfb64_1.conda#fdf80cb33c32d4d002bb89c37cfff5b7
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda#73f5dc8e2d55d9a1e14b11f49c3b4a28
+https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.4.0-hcfcfb64_0.conda#abd61d0ab127ec5cd68f62c2969e6f34
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda#958e0418e93e50c575bff70fbcaa12d8
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
 https://conda.anaconda.org/conda-forge/win-64/snappy-1.2.0-hfb803bf_1.conda#a419bf04a7c76a46639e315ac1b8bf72
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda#fc048363eb8f03cd1737600a5d08aafe
@@ -40,15 +40,15 @@
 https://conda.anaconda.org/conda-forge/win-64/krb5-1.21.2-heb0366b_0.conda#6e8b0f22b4eef3b3cb3849bb4c3d47f9
 https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.1.0-hcfcfb64_1.conda#19ce3e1dacc7912b3d6ff40690ba9ae0
 https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.1.0-hcfcfb64_1.conda#71e890a0b361fd58743a13f77e1506b7
 https://conda.anaconda.org/conda-forge/win-64/libintl-0.22.5-h5728263_2.conda#aa622c938af057adc119f8b8eecada01
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.43-h19919ed_0.conda#77e398acc32617a0384553aea29e866b
 https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
 https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2#e1a22282de0169c93e4ffe6ce6acc212
-https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_1.conda#eb9f59dd51f50f5aa369813fa63ba569
+https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_2.conda#ac7af7a949db01dae61ddc48f4a93d79
 https://conda.anaconda.org/conda-forge/win-64/libzip-1.10.1-h1d365fa_3.conda#5c629cd12d89e2856c17b1dc5fcf44a4
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.43-h17e33f8_0.conda#d0485b8aa2cedb141a7bd27b4efa4c9c
 https://conda.anaconda.org/conda-forge/win-64/python-3.9.19-h4de0772_0_cpython.conda#b6999bc275e0e6beae7b1c8ea0be1e85
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda#792bb5da68bf0a6cac6a6072ecb8dbeb
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
@@ -60,70 +60,70 @@
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-hdaf720e_2.conda#3761b23693f768dc75a8fd0a73ca053f
 https://conda.anaconda.org/conda-forge/win-64/gettext-tools-0.22.5-h7d00a51_2.conda#ef1c3bb48c013099c4872640a5f2096c
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.5-py39h1f6ef14_1.conda#4fc5bd0a7b535252028c647cc27d6c87
 https://conda.anaconda.org/conda-forge/win-64/libclang13-18.1.3-default_hf64faad_0.conda#9217c37b478ec601af909aafc954a6fc
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.7.1-hd5e4a3a_0.conda#3396aff340d0903e8814c2852d631e4e
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-0.22.5-h5728263_2.conda#f4c826b19bf1ccee2a63a2c685039728
-https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_4.conda#9baf04fc7002450a932cf97cb9625ebb
-https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda#87da045f6d26ce9fe20ad76a18f6a18a
+https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_6.conda#cd5c6efbe213c089f78575c98ab9a0ed
+https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda#ee944f0d41d9e2048f9d7492c1623ca3
 https://conda.anaconda.org/conda-forge/win-64/libintl-devel-0.22.5-h5728263_2.conda#a2ad82fae23975e4ccbfab2847d31d48
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.6.0-hddb2be6_3.conda#6d1828c9039929e2f185c5fa9d133018
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.8-py39ha55989b_0.conda#07aae1fdd812b411cec84c0d47339d22
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py39ha55989b_0.conda#d8f52e8e1d02f9a5901f9224e2ddf98f
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.1.0-py39ha55989b_0.conda#20ec896e8d97f2ff8be1124e624dc8f2
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/win-64/brotli-1.1.0-hcfcfb64_1.conda#f47f6db2528e38321fb00ae31674c133
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda#3549ecbceb6cd77b91a105511b7d0786
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
-https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_4.conda#44cd44c004db728bf5788c1d46ce7334
+https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_6.conda#40d452e4012c00f644b1dd6319fcdbcf
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.14.3-nompi_h73e8ff5_100.conda#1e91ce0f3a914b0dab762539c0df4ff1
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.16-h67d730c_0.conda#d3592435917b62a8becff3a60db674f6
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-devel-0.22.5-h5728263_2.conda#6f42ec61abc6d52a4079800a640319c5
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.15-hcd874cb_0.conda#090d91b69396f14afef450c285f9758c
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda#7e7099ad94ac3b599808950cec30ad4e
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.18.6-py39ha55989b_0.conda#7839645d467f5d3bc52709a3d484fa62
 https://conda.anaconda.org/conda-forge/win-64/sip-6.7.12-py39h99910a6_0.conda#0cc5774390ada632ed7975203057c91c
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda#21069f3ed16812f9f4f2700667b6ec86
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda#21745fdd12f01b41178596143cbecffd
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/win-64/fonttools-4.51.0-py39ha55989b_0.conda#5d19302bab29e347116b743e793aa7d6
 https://conda.anaconda.org/conda-forge/win-64/gettext-0.22.5-h5728263_2.conda#da84216f88a8c89eb943c683ceb34d7d
-https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_4.conda#d0a05e8a76abb68b2beb7b16c6d49213
+https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_6.conda#a4036d0bc6f499ebe9fef7b887f3ca0f
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.9.2-nompi_h07c049d_113.conda#2aa431a5a05e3679eea4faad0f47b119
 https://conda.anaconda.org/conda-forge/win-64/mkl-2024.1.0-h66d3029_692.conda#b43ec7ed045323edeff31e348eea8652
 https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py39h9ee4981_0.conda#6d69d57c41867acc162ef0205a8efaef
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.12.2-py39h99910a6_5.conda#dffbcea794c524c471772a5f697c2aea
@@ -139,17 +139,17 @@
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-22_win64_mkl.conda#c752cc2af9f3d8d7b2fdebb915a33ef7
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.26.4-py39hddb5d58_0.conda#6e30ff8f2d3f59f45347dfba8bc22a04
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-hcef0176_21.conda#76544d3dfeff8fd52250df168cb0005b
 https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.3-py39hd88c2e4_0.conda#12e356a0e7e5a8e67538aa66fbd21c47
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.2.1-py39h1f6ef14_0.conda#03e25c6bae87f4f9595337255b44b0fb
-https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.1-py39h32e6231_0.conda#7ca03abc7f2f9c91a9fdc02780bfa572
+https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.2-py39h32e6231_0.conda#0df69e098aa54373d4edb3eaaa2338ba
 https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.9-py39hb77abff_5.conda#5ed899124a51958336371ff01482b8fd
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.13.0-py39hddb5d58_0.conda#cfe749056fb9ed9dbc096b5751becf34
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.8.4-py39hf19769e_0.conda#7836c3dc5814f6d55a7392657c576e88
 https://conda.anaconda.org/conda-forge/win-64/netcdf4-1.6.5-nompi_py39h9a3bb69_100.conda#e271773571fa2908d8fd598878890db2
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.8.4-py39hcbf5309_0.conda#cc66c372d5eb745665da06ce56b7d72b
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-dev-linux-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-dev-linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 5b0485937e0a03182e2f3b1a21f55c7ce045f3f148d46011fd73e55f316ee82e
+# input_hash: b5796a88d528d140fb4eaf550a1fec4d817f597ed69bbae3efbf21291ae56fc6
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda#2f4327a1cbe7f022401b236e915a5fef
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda#f6f6600d18a4047b54f803cf708b868a
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda#10569984e7db886e4f1abc2b47ad79a1
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda#3cfab3e709f77e9f1b3d380eb622494a
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.13-ha770c72_0.conda#9105ee57dc4869bc5d1876b531202676
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-4_cp39.conda#bfe4b3259a8ac6cdf0037752904da6a7
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda#aae89d3736661c36a5591788aebd0817
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda#df88796bd09a0d2ed292e59101478ad8
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.11-hd590300_1.conda#0bb492cca54017ea314b809b1ee3a176
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
 https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
 https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.2-hd590300_0.conda#3bf7b9fd5a7136126e0234db4b87c8b6
@@ -34,15 +34,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-h43f5ff8_6.conda#e54a5ddc67e673f9105cf2a2e9c070b0
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
@@ -72,37 +72,37 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.69-h0f662aa_0.conda#25cb5999faa414e5ccb2c1388f62d3d5
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_6.conda#3666a850342f8f3be88f9a93d948d027
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda#b3316cbe90249da4f8e84cd66e1cc55b
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_2.conda#9a3a42df8a95f65334dfc7b80da1195d
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
 https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.3.0-hf1915f5_4.conda#784a4df6676c581ca624fbe460703a6d
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h59595ed_1.conda#7fc9d3288d2420bb3637647621018000
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_6.conda#9342e7c44c38bea649490f72d92c382d
 https://conda.anaconda.org/conda-forge/linux-64/libllvm15-15.0.7-hb3ce162_4.conda#8a35df3cbc0c8b12cc8af9473ae75eef
 https://conda.anaconda.org/conda-forge/linux-64/libllvm18-18.1.3-h2448989_0.conda#927b6d6e80b2c0d4405a58b61ca248a3
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
 https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.3.0-hca2cd23_4.conda#1b50eebe2a738a3146c154d2eceaa8b6
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.98-h1d7d5a4_0.conda#54b56c2fdf973656b748e0378900ec13
 https://conda.anaconda.org/conda-forge/linux-64/python-3.9.19-h0755675_0_cpython.conda#d9ee3647fbd9e8595b8df759b2bbefb8
@@ -111,17 +111,18 @@
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.9-h8ee46fc_0.conda#077b6e8ad6a3ddb741fce2496dd01bec
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
-https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
+https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-h04ea711_2.conda#f730d54ba9cd543666d7220c9f7ed563
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.1.0-hd590300_1.conda#f27a24d46e3ea7b70a1f98e50c62508f
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py39h3d6467e_1.conda#c48418c8b35f1d59ae9ae1174812b40a
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
@@ -131,43 +132,42 @@
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py39h3d6467e_0.conda#d48142fba253b2a1074f8ddee84749cb
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py39hf3d152e_4.conda#0d71b15b6e77f2ae2ef81a478a384ead
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py39hf3d152e_5.conda#d74cf0b3351ffc48f1388424df827755
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_5.conda#8fdb82e5d9694dd8e9ed9ac8fdf48a26
-https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_4.conda#c9deba4959ea5b5f72f1e3e4a71ae014
+https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.11-hb9ae30d_0.conda#9bd27b5e21da16e40cf799bc2acf47d1
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_6.conda#a9d23c02485c5cf055f9ac90eb9c9c63
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
-https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda#53511e966e3ced065fbb1d3d5470d16d
 https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2#9800ad1699b42612478755a2d26c722d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/linux-64/jsonpointer-2.4-py39hf3d152e_3.conda#23255e64bc45e9bc0b7d87c108357ce6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py39h7633fee_1.conda#c9f74d717e5a2847a9f8b779c54130f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang-cpp15-15.0.7-default_h127d8a8_5.conda#d0a9633b53cdc319b8a1a532ae7822b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-18.1.3-default_h5d6823c_0.conda#5fff487759736b275dc3e4a263cac666
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h4637d8d_4.conda#d4529f4dff3057982a7617c7ac58fde3
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
-https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.48-h71f35ed_0.conda#4d18d86916705d352d5f4adfb7f0edd3
+https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.49-h4f305b6_0.conda#dfcfd72c7a430d3616763ecfbefe4ca9
 https://conda.anaconda.org/conda-forge/linux-64/libpq-16.2-h33b98f1_1.conda#9e49ec2a61d02623b379dc332eb6889d
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.3.2-h658648e_1.conda#0ebb65e8d86843865796c7c95a941f34
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py39hd1e30aa_0.conda#9a9a22eb1f83c44953319ee3b027769f
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.2-pyhd8ed1ab_0.conda#5cbee699846772cc939bef23a0d524ed
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda#d5c98e9706fdc5328d49a9bf2ce5fb42
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.7-py39h7633fee_0.conda#f668e146a2ed03a4e62ffbb98b3115fb
@@ -179,16 +179,16 @@
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.10.0-pyhd8ed1ab_0.conda#8c6a4a704308f5d91f3a974a72db1096
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py39hd1e30aa_0.conda#ec86403fde8793ac1c36f8afa3d15902
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
@@ -196,200 +196,206 @@
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py39hd1e30aa_1.conda#37218233bcdc310e4fde6453bc1b40d8
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py39h8c080ef_0.conda#852eb7bf636d4108530a27100c23f1c1
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.2-py39ha1047a2_0.conda#916ab2d35fbe7a2ad3ba03f96c78922d
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.18.0-py39h9fdd4d6_0.conda#ca1e1ff2be5c41142e412c83b88960e4
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py39hd1e30aa_0.conda#b1961e70cfe8e1eac243faf933d1813f
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh0d859eb_0.conda#778594b20097b5a948c59e50ae42482a
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2#62f26a3d1387acee31322208f0cfa3e0
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda#37c47ea93ef00dd80d880fc4ba21256a
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py39hd1e30aa_0.conda#1e865e9188204cdfb1fd2531780add88
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.1.0-py39hd1e30aa_0.conda#1da984bbb6e765743e13388ba7b7b2c8
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
+https://conda.anaconda.org/conda-forge/linux-64/websockets-12.0-py39hd1e30aa_0.conda#34476c3670224efb4000f20c8c42eb5b
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.41-hd590300_0.conda#81f740407b45e3f9047b3174fa94eb9e
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda#5f25798dcefd8252ce5f9dc494d5f571
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.4-pyhd8ed1ab_0.conda#3d081de3a6ea9f894bbb585e8e3a4dcb
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
+https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda#c747b1d79f136013c3b7ebcba876afa6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py39h7a31438_0.conda#ac992767d7f8ed2cb27e71e78f0fb2d7
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.4-pyhd8ed1ab_0.conda#7c2b6931f9b3548ed78478332095c3e9
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda#948d84721b578d426294e17a02e24cbb
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py39hd1e30aa_0.conda#79f5dd8778873faa54e8f7b2729fe8a6
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.11-pyhd8ed1ab_0.conda#623b19f616f2ca0c261441067e18ae40
-https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_4.conda#5521382ee30b96b35eb0037fc3c4f2b4
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_6.conda#a1e026a82a562b443845db5614ca568a
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2#b748fbf7060927a6e82df7cb5ee8f097
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda#5271aed7436e2145d405a53ba05610aa
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_1.conda#7b756504d362cbad9b73a50a5455cafd
 https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda#547670a612fd335eaa5ffbf0fa75cb64
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py39hf3d152e_0.conda#612f7a003a8a407955572c0d53952ceb
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.3-hd590300_0.conda#32d16ad533c59bb0a3c5ffaf16110829
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h119a65a_9.conda#cfebc557e54905dadc355c0e9f003004
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.2-hc60ed4a_1.conda#ef1910918dd895516a769ed36b5b3a4e
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.7.0-h662e7e4_0.conda#b32c0da42b1f24a98577bb3d7fc0b995
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda#629f3203c99b32e0988910c93e77f3b6
 https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py39h90c7501_0.conda#1e3b6af9592be71ce19f0a6aae05d97b
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py39hd1e30aa_0.conda#2289054e90cf07e35280bbe798811dc8
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.12-py39h3d6467e_0.conda#e667a3ab0df62c54e60e1843d2e6defb
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh0d859eb_0.conda#efba281bbdae5f6b0a1d53c6d4a97c93
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.18-pyhd8ed1ab_0.conda#bf61cfd2a7f212efba378167a07d4a6a
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.0-pyhd8ed1ab_0.conda#7d2bc38bd1777c86cc345e510735d9ff
 https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda#997c29372bdbe2afee073dff71f35923
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py39hd1e30aa_4.conda#6a04738e75f877b68552fc19cb045233
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/linux-64/cryptography-42.0.5-py39hd4f0224_0.conda#74adeac31d6368a9dcf1a867a052cffa
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.43-pyhd8ed1ab_0.conda#0b2154c1818111e17381b1df5b4b0176
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.24.1-h98fc4e7_1.conda#b04b5cdf3ba01430db27979250bc5a1d
-https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.4.0-h3d44ed6_0.conda#27f46291a6aaa3c2a4f798ebd35a7ddb
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
+https://conda.anaconda.org/conda-forge/noarch/jaraco.context-5.3.0-pyhd8ed1ab_1.conda#72d7ad2dcd0f37eccb2ee35a1c8f6aaa
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-255-h3516f8a_1.conda#3366af27f0b593544a6cd453c7932ac5
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py39h474f0d3_0.conda#aa265f5697237aa13cc10f53fa8acc4f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.16.3-py39h9fdd4d6_0.conda#35fef239167838ec05bc714a70fbd6d9
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.18.2-py39ha68c5e3_0.conda#25e4460e21b75d8371cc388860a11be9
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.12.2-py39h3d6467e_5.conda#93aff412f3e49fdb43361c0215cbd72d
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.1.1-pyhd8ed1ab_0.conda#52b91ecba854d55b28ad916a8b10da24
 https://conda.anaconda.org/conda-forge/noarch/python-build-1.2.1-pyhd8ed1ab_0.conda#d657cde3b3943fcedf6038138eea84de
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
+https://conda.anaconda.org/conda-forge/linux-64/uvicorn-0.29.0-py39hf3d152e_0.conda#0d7cbecfb218788337acd7737c8d7fd4
+https://conda.anaconda.org/conda-forge/linux-64/watchfiles-0.21.0-py39h9fdd4d6_0.conda#176ddbfc26cc9da781910e18d600bf86
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-23.1.0-pyhd8ed1ab_0.conda#3afef1f55a1366b4d3b6a0d92e2235e4
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.14.0-pyhd8ed1ab_0.conda#a661c39e223bf3038b38126b0bbf43d9
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py39h44dd56e_0.conda#baea2f5dfb3ab7b1c836385d2e1daca7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py39h7633fee_0.conda#bdc188e59857d6efab332714e0d01d93
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.4-pyhd8ed1ab_0.conda#e54a91c3a65491b13c68f7696425bac8
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.24.1-hfa15dee_1.conda#a6dd2bbc684913e2bef0a54ce56fcbfb
 https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda#9f359af5a886fd6ca6b2b6ea02e58332
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.18.1-pyh707e725_3.conda#15c6f45a45f7ac27f6d60b0b084f6761
 https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.1-py39hddac248_0.conda#85293a042c24a08e71b7608ee66b6134
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.2-py39hddac248_0.conda#259c4e76e6bda8888aefc098ae1ba749
 https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.2-ha41ecd1_0.conda#a658eeabf188c3040da36b0763de2bfd
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
 https://conda.anaconda.org/conda-forge/noarch/pip-tools-7.4.1-pyhd8ed1ab_0.conda#73203bd783da9c37c2cdabb1f3b9d44d
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-17.0-hb77b528_0.conda#07f45f1be1c25345faddb8db0de8039b
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.3-py39hf3d152e_1.conda#90a592a19a0de2536d9e63886a569715
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.6.4-pyhd8ed1ab_0.conda#2e8e9f16431085f4b5a218b31fe557a3
-https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.1.2-py39h44dd56e_0.conda#fbff274dc712b7d59f32f9b89bbc0151
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda#f5dac044e2aaccf73b85053f6db360b5
+https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.1.4-py39h44dd56e_0.conda#904ee2e5d137acfe238e6f0bcb46817d
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py39h474f0d3_0.conda#46ae0ecba9726ab4fa44c78fefa522cf
 https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py39hf3d152e_2.conda#0e6f3ef2dd562ed33d2a18d9c6f78d88
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/linux-64/astropy-6.0.1-py39h44dd56e_0.conda#8e41cc53247a1d21d53339c80b75f673
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.14.0-pyhd8ed1ab_0.conda#4c08fa6e7d1d3f124ad815e21b2210e9
 https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h280cfa0_4.conda#410f86e58e880dcc7b0e910a8e89c05c
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda#e0deff12c601ce5cb7476f93718f3168
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.2-pyhd8ed1ab_0.conda#67f86478c78637f68c1f3858973021f2
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.21.1-pyhd8ed1ab_0.conda#26bce4b5405738c09304d4f4796b2c2a
-https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda#db81e05a29ff5d52ca21b18bbf880520
-https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hce6bd6c_0.conda#0891de8980ee29828542dbf9578838b9
+https://conda.anaconda.org/conda-forge/noarch/keyring-25.2.0-pyha804496_0.conda#7a14341f0ed09e83e28b28140f058ae0
+https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hadf69e7_1.conda#0e2b5bd9533043b41f9482ae9e2c16b5
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py39he9076e7_0.conda#1919384a8420e7bb25f6c3a582e0857c
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda#0b57b5368ab7fc7cdc9e3511fa867214
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py39h4282601_100.conda#d2809fbf0d8ae7b8ca92c456cb44a7d4
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-hc9dc06e_21.conda#b325046180590c868ce0dbf267b82eb8
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/linux-64/statsmodels-0.14.1-py39h44dd56e_0.conda#dc565186b972bd87e49b9c35390ddd8c
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.6-pyhd8ed1ab_0.conda#16195242f8b17c9ca49f1ea34f1c027f
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.7-pyhd8ed1ab_0.conda#154d0c643be6a9ce6fbe655d007d8e4e
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-9.0.0-h78e8752_1.conda#a3f4cd4a512ec5db35ffbf25ba11f537
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.9-py39h52134e7_5.conda#e1f148e57d071b09187719df86f513c1
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.8.4-py39hf3d152e_0.conda#c66d2da2669fddc657b679bccab95775
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-dev-osx-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-dev-osx-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: b999a6c9f39c420db057dec65fd5d2e01109be13652ecd8ecbdc76d5c1efcf0f
+# input_hash: 2b84465b84cfa81790393537b9fe0a4ab921e6816915257b66c9da28c5c5b3f1
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda#6097a6ca9ada32699b5fc4312dd6ef18
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.28.1-h10d778d_0.conda#d5eb7992227254c0e9a0ce71151f0079
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda#f2eacee8c33c43692f1ccfd33d0f50b1
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
@@ -43,17 +43,17 @@
 https://conda.anaconda.org/conda-forge/osx-64/libasprintf-devel-0.22.5-h5ff76d1_2.conda#c7182eda3bc727384e2f98f4d680fa7d
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.1.0-h0dc2134_1.conda#9ee0bab91b2ca579e10353738be36063
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.1.0-h0dc2134_1.conda#8a421fe09c6187f0eb5e2338a8a8be6d
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-13.2.0-h2873a65_3.conda#e4fb4d23ec2870ff3c40d10afe305aec
 https://conda.anaconda.org/conda-forge/osx-64/libintl-0.22.5-h5ff76d1_2.conda#3fb6774cb8cdbb93a6013b67bcf9716d
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda#65dcddb15965c9de2c0365cb14910532
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda#086f56e13a96a6cfb1bf640505ae6b70
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda#68e462226209f35182ef66eda0f794ff
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda#bd85e0ca9e1ffaadc3b56079fd956035
+https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda#50b997370584f2c83ca0c38e9028eab9
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda#570a6f04802df580be529f3a72d2bbf7
 https://conda.anaconda.org/conda-forge/osx-64/pcre2-10.43-h0ad2156_0.conda#9c8651803886ce9d5983e107a0df4ea8
 https://conda.anaconda.org/conda-forge/osx-64/pixman-0.43.4-h73e2aa4_0.conda#cb134c1e03fd32f4e6bea3f6de2614fd
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.2.0-h6dc393e_1.conda#9c322ec36340610fcf213b72999b049e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda#bf830ba5afc507c6232d4ef0fb1a882d
@@ -64,29 +64,30 @@
 https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.1.0-h0dc2134_1.conda#ece565c215adcc47fc1db4e651ee094b
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h60636b9_2.conda#25152fce119320c980e5470e64834b50
 https://conda.anaconda.org/conda-forge/osx-64/gettext-tools-0.22.5-h5ff76d1_2.conda#37e1cb0efeff4d4623a6357e37e0105d
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.21.2-hb884880_0.conda#80505a68783f01dc8d7308c075261b2f
 https://conda.anaconda.org/conda-forge/osx-64/libgettextpo-0.22.5-h5ff76d1_2.conda#54cc9d12c29c2f0516f2ef4987de53ae
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-13_2_0_h97931a8_3.conda#0b6e23a012ee7a9a5f6b244f5a92c1d5
-https://conda.anaconda.org/conda-forge/osx-64/libglib-2.80.0-h81c1438_4.conda#eb94cd8fdcb676d17a5119189f87c4ae
+https://conda.anaconda.org/conda-forge/osx-64/libglib-2.80.0-h81c1438_6.conda#54dd1ed37dd65c5d13600bcc5ebbd0a1
 https://conda.anaconda.org/conda-forge/osx-64/libintl-devel-0.22.5-h5ff76d1_2.conda#ea0a07e556d6b238db685cae6e3585d0
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.58.0-h64cf6d3_1.conda#faecc55c2a8155d9ff1c0ff9a0fef64f
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.6.0-h129831d_3.conda#568593071d2e6cea7b5fc1f75bfa10ca
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.10.1-hc158999_3.conda#6112b3173f3aa2f12a8f40d07a77cc35
 https://conda.anaconda.org/conda-forge/osx-64/python-3.9.19-h7a9c478_0_cpython.conda#7d53d366acd9dbfb498c69326ccb520a
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda#cc4834a9ee7cc49ce8d25177c47b10d8
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
-https://conda.anaconda.org/conda-forge/osx-64/atk-1.0-2.38.0-h1d18e73_1.tar.bz2#5a538295f97a484ee332aacc131718b5
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
+https://conda.anaconda.org/conda-forge/osx-64/atk-1.0-2.38.0-h4bec284_2.conda#d9684247c943d492d9aac8687bc5db77
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/osx-64/brotli-1.1.0-h0dc2134_1.conda#9272dd3b19c4e8212f8542cefd5c3d67
 https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.1.0-py39h840bb9f_1.conda#bf1edb07835e15685718843f7e71bab1
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
@@ -95,30 +96,29 @@
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py39hd253f6c_0.conda#328dc0de8a70c8f8de65d37a6b289220
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py39h6e9494a_4.conda#2075bada3661d0a7fb762b4f84f7c06a
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py39h6e9494a_5.conda#7738300100023129d58567edc49ee90b
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/osx-64/fontconfig-2.14.2-h5bb23bf_0.conda#86cc5867dfbee4178118392bae4a3c89
-https://conda.anaconda.org/conda-forge/osx-64/gdk-pixbuf-2.42.10-hd9e0ca3_5.conda#308cefd960b6ba51bdbdc5ba9e9b2377
+https://conda.anaconda.org/conda-forge/osx-64/gdk-pixbuf-2.42.11-ha9f1606_0.conda#ab407c96c658772c9bcd7161931fd933
 https://conda.anaconda.org/conda-forge/osx-64/gts-0.7.6-h53e17e3_4.conda#848cc963fcfbd063c7a023024aa3bec0
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
-https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda#53511e966e3ced065fbb1d3d5470d16d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/osx-64/jsonpointer-2.4-py39h6e9494a_3.conda#7712a5f0d4f3f7d9ec69fb24dcf9bf0a
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.5-py39h8ee36c8_1.conda#6072db04642b21329b0502a177ec18bf
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.16-ha2f27b4_0.conda#1442db8f03517834843666c422238c9b
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.7.1-h726d00d_0.conda#fa58e5eaa12006bc3289a71357bef167
 https://conda.anaconda.org/conda-forge/osx-64/libgettextpo-devel-0.22.5-h5ff76d1_2.conda#1e0384c52cd8b54812912e7234e66056
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.27-openmp_hfef2a42_0.conda#00237c9c7f2cb6725fe2960680a6e225
@@ -136,64 +136,66 @@
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.10.0-pyhd8ed1ab_0.conda#8c6a4a704308f5d91f3a974a72db1096
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py39ha09f3b3_0.conda#e8737c3c0c404559b0e2c8a9eb91e977
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py39hdc70f33_1.conda#542378f49240a94056b50ab1385b3bfb
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py39hcb7a90d_0.conda#39754a321b3dece3df9a0eb213d43dc8
+https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.2-py39hffc4518_0.conda#13c761db6b475447b63702e5f7ee3015
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.18.0-py39hcf47035_0.conda#0e8641e9f0d42d844cf17f5520225e6e
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.8-py39ha09f3b3_0.conda#835c656934865805c0b02dbff74fe5b7
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2#62f26a3d1387acee31322208f0cfa3e0
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda#37c47ea93ef00dd80d880fc4ba21256a
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py39ha09f3b3_0.conda#4541517b5a605bf45d4a5fb074bb4cf5
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.1.0-py39hdc70f33_0.conda#ede122e9ef2775a8879063d9d3ee819f
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
+https://conda.anaconda.org/conda-forge/osx-64/websockets-12.0-py39ha09f3b3_0.conda#14a37a956881ee2df098931d2c8b40c9
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda#5f25798dcefd8252ce5f9dc494d5f571
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.4-pyhd8ed1ab_0.conda#3d081de3a6ea9f894bbb585e8e3a4dcb
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
+https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda#c747b1d79f136013c3b7ebcba876afa6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/osx-64/cairo-1.18.0-h99e66fa_0.conda#13f830b1bf46018f7062d1b798d53eca
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py39h18ef598_0.conda#c31ac48f93f773fd27e99f113cfffb98
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.4-pyhd8ed1ab_0.conda#7c2b6931f9b3548ed78478332095c3e9
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
@@ -204,133 +206,137 @@
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.11-pyhd8ed1ab_0.conda#623b19f616f2ca0c261441067e18ae40
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2#b748fbf7060927a6e82df7cb5ee8f097
 https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.3-nompi_h691f4bf_100.conda#8e2ac4ae815a8c9743fe37d70f48f075
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda#5271aed7436e2145d405a53ba05610aa
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_1.conda#7b756504d362cbad9b73a50a5455cafd
 https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda#547670a612fd335eaa5ffbf0fa75cb64
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.1-py39h6e9494a_0.conda#9611b1806866adc1693cfb5a323f16e4
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-22_osx64_openblas.conda#b80966a8c8dd0b531f8e65f709d732e8
 https://conda.anaconda.org/conda-forge/osx-64/libgd-2.3.3-h0dceb68_9.conda#1feb43971521d430bf826f8398598c5b
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda#629f3203c99b32e0988910c93e77f3b6
 https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py39h9dabb2a_0.conda#e385068c9511542eff20422f7e799064
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-10.2-py39h8602b6b_0.conda#37b6b21536780b9665b9c84908318d7a
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.18.6-py39ha09f3b3_0.conda#6eb863d10b7aeef1f58ba1ebf92f59bd
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh31c8845_0.conda#00b54981b923f5aefcd5e8547de056d5
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.18-pyhd8ed1ab_0.conda#bf61cfd2a7f212efba378167a07d4a6a
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.0-pyhd8ed1ab_0.conda#7d2bc38bd1777c86cc345e510735d9ff
 https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda#997c29372bdbe2afee073dff71f35923
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py39hdc70f33_4.conda#3a0f682e6fdf53ff630c22cdd90ac0c1
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.43-pyhd8ed1ab_0.conda#0b2154c1818111e17381b1df5b4b0176
-https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-8.3.0-hf45c392_0.conda#41d890485f909e4ecdc608741718c75e
+https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-8.4.0-h72fa137_0.conda#7d065a2266ae5eb2a5d91a6dca4fca69
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
+https://conda.anaconda.org/conda-forge/noarch/jaraco.context-5.3.0-pyhd8ed1ab_1.conda#72d7ad2dcd0f37eccb2ee35a1c8f6aaa
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-22_osx64_openblas.conda#b9fef82772330f61b2b0201c72d2c29b
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-22_osx64_openblas.conda#f21b282ff7ba14df6134a0fe6ab42b1b
 https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_h7760872_113.conda#bce76ace6497221c2a2a02840aaceac5
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.16.3-py39hcf47035_0.conda#ca2dc68c950341730cd6140a0d141cf1
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.18.2-py39h3013830_0.conda#1509b51dadc688c5a71771483d195d52
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-10.2-py39h8602b6b_0.conda#271f368ad661bf3bba2d5740ac8ee24c
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.1.1-pyhd8ed1ab_0.conda#52b91ecba854d55b28ad916a8b10da24
 https://conda.anaconda.org/conda-forge/noarch/python-build-1.2.1-pyhd8ed1ab_0.conda#d657cde3b3943fcedf6038138eea84de
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
+https://conda.anaconda.org/conda-forge/osx-64/uvicorn-0.29.0-py39h6e9494a_0.conda#79786774d034370e5e7bf2707b7613d5
+https://conda.anaconda.org/conda-forge/osx-64/watchfiles-0.21.0-py39h3f9c672_0.conda#9c6ce8f29c4c66782417b26bb4a7d5dd
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-23.1.0-pyhd8ed1ab_0.conda#3afef1f55a1366b4d3b6a0d92e2235e4
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.14.0-pyhd8ed1ab_0.conda#a661c39e223bf3038b38126b0bbf43d9
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.4-pyhd8ed1ab_0.conda#e54a91c3a65491b13c68f7696425bac8
 https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda#9f359af5a886fd6ca6b2b6ea02e58332
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.18.1-pyh707e725_3.conda#15c6f45a45f7ac27f6d60b0b084f6761
 https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
-https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh534df25_0.conda#537a5385c6cee5fa2275a457e0b51b21
+https://conda.anaconda.org/conda-forge/noarch/keyring-25.2.0-pyh534df25_0.conda#acaf59f096327bc5757c91303cae99ca
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.26.4-py39h28c39a1_0.conda#1b07000dc6aed4a69e91107dac4464d3
 https://conda.anaconda.org/conda-forge/osx-64/pango-1.52.2-h7f2093b_0.conda#ea9611aee7e61e4ff18c4dc56ec100ab
 https://conda.anaconda.org/conda-forge/noarch/pip-tools-7.4.1-pyhd8ed1ab_0.conda#73203bd783da9c37c2cdabb1f3b9d44d
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.3-py39h6e9494a_1.conda#450b8f37439740c0e79acbeba7d1d678
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.6.4-pyhd8ed1ab_0.conda#2e8e9f16431085f4b5a218b31fe557a3
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda#f5dac044e2aaccf73b85053f6db360b5
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh31c8845_0.conda#c3cb67fc72fb38020fe7923dbbcf69b0
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.14.0-pyhd8ed1ab_0.conda#4c08fa6e7d1d3f124ad815e21b2210e9
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.3-py39h5b4affa_0.conda#20fd617b1f9fcefe5ec1577d38ae7bdb
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.2.1-py39h0ca7971_0.conda#a4c478d3b64c81d1742dc8073e4996b6
 https://conda.anaconda.org/conda-forge/osx-64/gtk2-2.24.33-h8ca4665_4.conda#ff451625250bf843393ca3d660accab3
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda#28e74fca8d8abf09c1ed0d190a17e307
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.2-pyhd8ed1ab_0.conda#67f86478c78637f68c1f3858973021f2
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.21.1-pyhd8ed1ab_0.conda#26bce4b5405738c09304d4f4796b2c2a
-https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.58.0-h7b06fc5_0.conda#3ad98f9e1ad2b0c9b202b9d5212752d2
+https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.58.0-h7b06fc5_1.conda#e4a5f1bb5962ec6f2f2d2f0467ed0826
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda#0b57b5368ab7fc7cdc9e3511fa867214
-https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.1-py39haf03413_0.conda#d29dc35b665029951dae988810f84508
+https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.2-py39haf03413_0.conda#11225cf1f769af217ffc01f0a21d40fa
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
-https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.1.2-py39h5b4affa_0.conda#d1167fcafcd783b8b3835ec7cf6931c7
+https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.1.4-py39h5b4affa_0.conda#6743589ba4d7d219c4e2790d4c1d4b13
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.13.0-py39h0ed1e0f_0.conda#3a4d0af4fe2006bedc33ca61e9a0b4d6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/osx-64/astropy-6.0.1-py39h5b4affa_0.conda#f883a58c4337d0a6f0996a533aae15f0
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.6-pyhd8ed1ab_0.conda#16195242f8b17c9ca49f1ea34f1c027f
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.7-pyhd8ed1ab_0.conda#154d0c643be6a9ce6fbe655d007d8e4e
 https://conda.anaconda.org/conda-forge/osx-64/graphviz-9.0.0-hee74176_1.conda#7cd479251093c332aa9fe93cfb8f698b
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.8.4-py39h7070ae8_0.conda#cb9e1f8aff1f759b9685e908f9dc0a5b
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.5-nompi_py39h824b2b2_100.conda#07525171115894fe9c4aba755460c51a
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/osx-64/statsmodels-0.14.1-py39h5b4affa_0.conda#4cc025969fa47342955213653d1352c8
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.8.4-py39h6e9494a_0.conda#371fe0f738d9f3baa20cf06656b78b0a
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-dev-win-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-dev-win-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: 9ad718ef7b5a9fbf088fa23ac9c09be94a00a86afe4fb2986ea855c6b8b67d03
+# input_hash: 2c6414ffedc11afaa29ea902e4debab1ee1854a776195e8394589b994c279ef5
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda#63da060240ab8087b60d1357051ea7d6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda#30ebb9fd99666d8b8675fcee541a09f3
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda#c66eb2fd33b999ccc258aef85689758e
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-0.22.5-h5728263_2.conda#75a6982b9ff0a8db0f53303527b07af8
 https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda#bc592d03f62779511d392c175dcece64
 https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2#b0309b72560df66f71a9d5e34a5efdfa
 https://conda.anaconda.org/conda-forge/win-64/pandoc-3.1.13-h57928b3_0.conda#4caaf4c37a0efc8a06492dba2d871bbb
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.9-4_cp39.conda#948b0d93d4ab1372d8fd45e1560afd47
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
@@ -36,15 +36,15 @@
 https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.1.0-hcfcfb64_1.conda#f77f319fb82980166569e1280d5b2864
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.20-hcfcfb64_0.conda#b12b5bde5eb201a1df75e49320cc938a
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda#e1eb10b1cca179f2baa3601e4efc8712
 https://conda.anaconda.org/conda-forge/win-64/libjpeg-turbo-3.0.0-hcfcfb64_1.conda#3f1b948619c45b1ca714d60c7389092c
 https://conda.anaconda.org/conda-forge/win-64/libogg-1.3.4-h8ffe710_1.tar.bz2#04286d905a0dcb7f7d4a12bdfe02516d
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda#f95359f8dc5abf7da7776ece9ef10bc5
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda#73f5dc8e2d55d9a1e14b11f49c3b4a28
 https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.2-hcfcfb64_1.conda#fdf80cb33c32d4d002bb89c37cfff5b7
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda#958e0418e93e50c575bff70fbcaa12d8
 https://conda.anaconda.org/conda-forge/win-64/pixman-0.43.4-h63175ca_0.conda#b98135614135d5f458b75ab9ebb9558c
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
@@ -57,28 +57,29 @@
 https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.1.0-hcfcfb64_1.conda#19ce3e1dacc7912b3d6ff40690ba9ae0
 https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.1.0-hcfcfb64_1.conda#71e890a0b361fd58743a13f77e1506b7
 https://conda.anaconda.org/conda-forge/win-64/libintl-0.22.5-h5728263_2.conda#aa622c938af057adc119f8b8eecada01
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.43-h19919ed_0.conda#77e398acc32617a0384553aea29e866b
 https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
 https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2#e1a22282de0169c93e4ffe6ce6acc212
 https://conda.anaconda.org/conda-forge/win-64/libwebp-1.3.2-hcfcfb64_1.conda#6202a1ba6be2713084cf0452d4e8c10c
-https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_1.conda#eb9f59dd51f50f5aa369813fa63ba569
+https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_2.conda#ac7af7a949db01dae61ddc48f4a93d79
 https://conda.anaconda.org/conda-forge/win-64/libzip-1.10.1-h1d365fa_3.conda#5c629cd12d89e2856c17b1dc5fcf44a4
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.43-h17e33f8_0.conda#d0485b8aa2cedb141a7bd27b4efa4c9c
 https://conda.anaconda.org/conda-forge/win-64/python-3.9.19-h4de0772_0_cpython.conda#b6999bc275e0e6beae7b1c8ea0be1e85
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-h63175ca_1.conda#e8867cc4d023f41f54bd64a33436b0a1
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda#792bb5da68bf0a6cac6a6072ecb8dbeb
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/win-64/blosc-1.21.5-hbd69f2e_1.conda#06c7d9a1cdecef43921be8b577a61ee7
 https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.1.0-hcfcfb64_1.conda#0105229d7c5fabaa840043a86c10ec64
 https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.1.0-py39h99910a6_1.conda#f24ba3942ece1e5d3dcde934f0532998
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
@@ -87,37 +88,36 @@
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py39h99910a6_0.conda#412a0fe4d63fab41a73776839a5856db
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py39hcbf5309_4.conda#adae8d63d214069960445c1aba41eea5
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py39hcbf5309_5.conda#461b44faa5dd942c6be4405a8df37587
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-hdaf720e_2.conda#3761b23693f768dc75a8fd0a73ca053f
 https://conda.anaconda.org/conda-forge/win-64/gettext-tools-0.22.5-h7d00a51_2.conda#ef1c3bb48c013099c4872640a5f2096c
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
-https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda#53511e966e3ced065fbb1d3d5470d16d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/win-64/jsonpointer-2.4-py39hcbf5309_3.conda#e066b7eb0c8669f0549aaf6aef50f880
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.5-py39h1f6ef14_1.conda#4fc5bd0a7b535252028c647cc27d6c87
 https://conda.anaconda.org/conda-forge/win-64/libclang13-18.1.3-default_hf64faad_0.conda#9217c37b478ec601af909aafc954a6fc
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.7.1-hd5e4a3a_0.conda#3396aff340d0903e8814c2852d631e4e
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-0.22.5-h5728263_2.conda#f4c826b19bf1ccee2a63a2c685039728
-https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_4.conda#9baf04fc7002450a932cf97cb9625ebb
-https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda#87da045f6d26ce9fe20ad76a18f6a18a
+https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_6.conda#cd5c6efbe213c089f78575c98ab9a0ed
+https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda#ee944f0d41d9e2048f9d7492c1623ca3
 https://conda.anaconda.org/conda-forge/win-64/libintl-devel-0.22.5-h5728263_2.conda#a2ad82fae23975e4ccbfab2847d31d48
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.6.0-hddb2be6_3.conda#6d1828c9039929e2f185c5fa9d133018
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py39ha55989b_0.conda#f8b7e33c8bf98901925817b7f4436c7e
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.2-pyhd8ed1ab_0.conda#5cbee699846772cc939bef23a0d524ed
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda#d5c98e9706fdc5328d49a9bf2ce5fb42
 https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.7-py39h1f6ef14_0.conda#74e894b9e9ef693559594bdb472da770
@@ -128,16 +128,16 @@
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.10.0-pyhd8ed1ab_0.conda#8c6a4a704308f5d91f3a974a72db1096
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py39ha55989b_0.conda#59cff26058f788059a310208dde2e01d
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
@@ -147,152 +147,158 @@
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py39h99910a6_2.conda#eab91442160b49994dd2e224e6082770
 https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py39hcbf5309_1.conda#b81928cd8f6e5faf318ad6ddf8b0c7a5
 https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.13-py39h99910a6_0.conda#6dc677d08286a639b3c064a7a4376e06
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py39ha55989b_1.conda#5c3a9da77fc79c21c5c1fd7ea06306a2
-https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py39h7eaf5a6_0.conda#113b93bd971d355b1d52df09c1161628
+https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.2-py39h03e5c00_0.conda#5e1e67cb1d03a2cce828bac7aa6642a5
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.18.0-py39hf21820d_0.conda#32fa6863c2216dbe787adaf874433713
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.8-py39ha55989b_0.conda#07aae1fdd812b411cec84c0d47339d22
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2#62f26a3d1387acee31322208f0cfa3e0
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda#37c47ea93ef00dd80d880fc4ba21256a
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py39ha55989b_0.conda#d8f52e8e1d02f9a5901f9224e2ddf98f
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.1.0-py39ha55989b_0.conda#20ec896e8d97f2ff8be1124e624dc8f2
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
+https://conda.anaconda.org/conda-forge/win-64/websockets-12.0-py39ha55989b_0.conda#24b1cf33f77a58400a2098e0cdc04e8f
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/xorg-kbproto-1.0.7-hcd874cb_1002.tar.bz2#8d11c1dac4756ca57e78c1bfe173bba4
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
 https://conda.anaconda.org/conda-forge/win-64/xorg-xextproto-7.3.0-hcd874cb_1003.conda#6e6c2639620e436bddb7c040cd4f3adb
 https://conda.anaconda.org/conda-forge/win-64/xorg-xproto-7.0.31-hcd874cb_1007.tar.bz2#88f3c65d2ad13826a9e0b162063be023
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda#5f25798dcefd8252ce5f9dc494d5f571
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.4-pyhd8ed1ab_0.conda#3d081de3a6ea9f894bbb585e8e3a4dcb
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
+https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda#c747b1d79f136013c3b7ebcba876afa6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/conda-forge/win-64/brotli-1.1.0-hcfcfb64_1.conda#f47f6db2528e38321fb00ae31674c133
 https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py39ha55989b_0.conda#3641cc4492220301e0b0c65cf2985a80
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda#3549ecbceb6cd77b91a105511b7d0786
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda#948d84721b578d426294e17a02e24cbb
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/win-64/fontconfig-2.14.2-hbde0cde_0.conda#08767992f1a4f1336a257af1241034bd
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.11-pyhd8ed1ab_0.conda#623b19f616f2ca0c261441067e18ae40
-https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_4.conda#44cd44c004db728bf5788c1d46ce7334
+https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_6.conda#40d452e4012c00f644b1dd6319fcdbcf
 https://conda.anaconda.org/conda-forge/win-64/gts-0.7.6-h6b5321d_4.conda#a41f14768d5e377426ad60c613f2923b
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2#b748fbf7060927a6e82df7cb5ee8f097
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.14.3-nompi_h73e8ff5_100.conda#1e91ce0f3a914b0dab762539c0df4ff1
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda#5271aed7436e2145d405a53ba05610aa
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_1.conda#7b756504d362cbad9b73a50a5455cafd
 https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda#547670a612fd335eaa5ffbf0fa75cb64
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py39hcbf5309_0.conda#78ec20214b67efe5caebb4f08bdee094
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.16-h67d730c_0.conda#d3592435917b62a8becff3a60db674f6
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-devel-0.22.5-h5728263_2.conda#6f42ec61abc6d52a4079800a640319c5
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.15-hcd874cb_0.conda#090d91b69396f14afef450c285f9758c
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda#7e7099ad94ac3b599808950cec30ad4e
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.18.6-py39ha55989b_0.conda#7839645d467f5d3bc52709a3d484fa62
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh5737063_0.conda#5a86a21050ca3831ec7f77fb302f1132
 https://conda.anaconda.org/conda-forge/win-64/sip-6.7.12-py39h99910a6_0.conda#0cc5774390ada632ed7975203057c91c
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda#21069f3ed16812f9f4f2700667b6ec86
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda#21745fdd12f01b41178596143cbecffd
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh5737063_0.conda#4abd500577430a942a995fd0d09b76a2
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.0-pyhd8ed1ab_0.conda#7d2bc38bd1777c86cc345e510735d9ff
 https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda#997c29372bdbe2afee073dff71f35923
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py39ha55989b_4.conda#40f25bc759e1ea863a6e468380cd2363
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/win-64/cairo-1.18.0-h1fef639_0.conda#b3fe2c6381ec74afe8128e16a11eee02
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.4-pyhd8ed1ab_0.conda#7c2b6931f9b3548ed78478332095c3e9
 https://conda.anaconda.org/conda-forge/win-64/fonttools-4.51.0-py39ha55989b_0.conda#5d19302bab29e347116b743e793aa7d6
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/win-64/gettext-0.22.5-h5728263_2.conda#da84216f88a8c89eb943c683ceb34d7d
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.43-pyhd8ed1ab_0.conda#0b2154c1818111e17381b1df5b4b0176
-https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_4.conda#d0a05e8a76abb68b2beb7b16c6d49213
+https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_6.conda#a4036d0bc6f499ebe9fef7b887f3ca0f
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
+https://conda.anaconda.org/conda-forge/noarch/jaraco.context-5.3.0-pyhd8ed1ab_1.conda#72d7ad2dcd0f37eccb2ee35a1c8f6aaa
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.9.2-nompi_h07c049d_113.conda#2aa431a5a05e3679eea4faad0f47b119
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/win-64/mkl-2024.1.0-h66d3029_692.conda#b43ec7ed045323edeff31e348eea8652
 https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py39h9ee4981_0.conda#6d69d57c41867acc162ef0205a8efaef
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.16.3-py39hf21820d_0.conda#2c10071c595fa4c2f021f51f0852c37b
+https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.18.2-py39h92a245a_0.conda#5d16ca48eb70a12b953439c03c7e4513
 https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.12.2-py39h99910a6_5.conda#dffbcea794c524c471772a5f697c2aea
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.1.1-pyhd8ed1ab_0.conda#52b91ecba854d55b28ad916a8b10da24
 https://conda.anaconda.org/conda-forge/noarch/python-build-1.2.1-pyhd8ed1ab_0.conda#d657cde3b3943fcedf6038138eea84de
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.18-pyhd8ed1ab_0.conda#bf61cfd2a7f212efba378167a07d4a6a
+https://conda.anaconda.org/conda-forge/win-64/uvicorn-0.29.0-py39hcbf5309_0.conda#75e90ff63b09f4443258dd7829bb6032
+https://conda.anaconda.org/conda-forge/win-64/watchfiles-0.21.0-py39hf21820d_0.conda#5409cf692b0dec68648e6e8a6721e5ee
 https://conda.anaconda.org/conda-forge/win-64/xorg-libx11-1.8.9-hefa74cf_0.conda#3672e991346895f332af1ebc60b8bca9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-23.1.0-pyhd8ed1ab_0.conda#3afef1f55a1366b4d3b6a0d92e2235e4
 https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.24.1-hb4038d2_1.conda#8a6dfe53ad02a3b151e6383a950043ee
-https://conda.anaconda.org/conda-forge/win-64/harfbuzz-8.3.0-h7ab893a_0.conda#b8ef0beb91df83c5e6038c9509b9f730
+https://conda.anaconda.org/conda-forge/win-64/harfbuzz-8.4.0-h7ab893a_0.conda#bf9b853f9702724a5ec4e68dc637cc29
 https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda#9f359af5a886fd6ca6b2b6ea02e58332
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.18.1-pyh7428d3b_3.conda#656a798e52fbe1ca72f7d97b3c36aeff
 https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
-https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh7428d3b_0.conda#993d4eaf46a94e1ba4d1a15fbed07953
+https://conda.anaconda.org/conda-forge/noarch/keyring-25.2.0-pyh7428d3b_0.conda#33f009280144917e907939141af7cf7c
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-22_win64_mkl.conda#65c56ecdeceffd6c32d3d54db7e02c6e
 https://conda.anaconda.org/conda-forge/noarch/pip-tools-7.4.1-pyhd8ed1ab_0.conda#73203bd783da9c37c2cdabb1f3b9d44d
 https://conda.anaconda.org/conda-forge/win-64/pybtex-docutils-1.0.3-py39hcbf5309_1.conda#0131fba9b943b68a01e2ac623004c48f
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.6.4-pyhd8ed1ab_0.conda#2e8e9f16431085f4b5a218b31fe557a3
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda#f5dac044e2aaccf73b85053f6db360b5
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libice-1.1.1-hcd874cb_0.conda#5271e3af4791170e2c55d02818366916
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxext-1.3.4-hcd874cb_2.conda#2aa695ac3c56193fd8d526e3b511e021
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.14.0-pyhd8ed1ab_0.conda#a661c39e223bf3038b38126b0bbf43d9
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.4-pyhd8ed1ab_0.conda#e54a91c3a65491b13c68f7696425bac8
@@ -310,49 +316,49 @@
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.14.0-pyhd8ed1ab_0.conda#4c08fa6e7d1d3f124ad815e21b2210e9
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.26.4-py39hddb5d58_0.conda#6e30ff8f2d3f59f45347dfba8bc22a04
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-hcef0176_21.conda#76544d3dfeff8fd52250df168cb0005b
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxt-1.3.0-hcd874cb_1.conda#511a29edd2ff3d973f63e54f19dcc06e
 https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.3-py39hd88c2e4_0.conda#12e356a0e7e5a8e67538aa66fbd21c47
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.6-pyhd8ed1ab_0.conda#16195242f8b17c9ca49f1ea34f1c027f
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.7-pyhd8ed1ab_0.conda#154d0c643be6a9ce6fbe655d007d8e4e
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.2.1-py39h1f6ef14_0.conda#03e25c6bae87f4f9595337255b44b0fb
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
-https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.1-py39h32e6231_0.conda#7ca03abc7f2f9c91a9fdc02780bfa572
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
+https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.2-py39h32e6231_0.conda#0df69e098aa54373d4edb3eaaa2338ba
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
-https://conda.anaconda.org/conda-forge/win-64/pyerfa-2.0.1.2-py39hd88c2e4_0.conda#b252cec19b9dfb27ce61ea3ebf90717a
+https://conda.anaconda.org/conda-forge/win-64/pyerfa-2.0.1.4-py39hd88c2e4_0.conda#173997708f936f15e527756c01e2b744
 https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.9-py39hb77abff_5.conda#5ed899124a51958336371ff01482b8fd
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.13.0-py39hddb5d58_0.conda#cfe749056fb9ed9dbc096b5751becf34
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxpm-3.5.17-hcd874cb_0.conda#029be9b667bf3896fa28bc32adb1bfc3
 https://conda.anaconda.org/conda-forge/win-64/astropy-6.0.1-py39hd88c2e4_0.conda#efb93481436d459f13e041b2572d584c
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
 https://conda.anaconda.org/conda-forge/win-64/libgd-2.3.3-h312136b_9.conda#69c987e1f9268d9ade86497c4ab8cc45
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.8.4-py39hf19769e_0.conda#7836c3dc5814f6d55a7392657c576e88
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
 https://conda.anaconda.org/conda-forge/win-64/netcdf4-1.6.5-nompi_py39h9a3bb69_100.conda#e271773571fa2908d8fd598878890db2
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/win-64/statsmodels-0.14.1-py39hd88c2e4_0.conda#b51565db0ed851e9031da82171d0e02f
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/win-64/graphviz-9.0.0-h51cb2cd_1.conda#9e73e70557ae3c1c9d4bdf70f47dd141
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.8.4-py39hcbf5309_0.conda#cc66c372d5eb745665da06ce56b7d72b
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-dev.yml` & `eradiate-0.27.0rc1/requirements/conda/environment-optional.yml`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,28 @@
   - pip-tools>=6.5
   - pip>=22
   - setuptools>=61
   # docs
   - autodocsumm
   - myst-parser
   - nbsphinx>=0.9.0
+  - seaborn
   - sphinx
   - sphinx-autobuild
   - sphinx-book-theme>=1.0
   - sphinx-copybutton
   - sphinx-design
   - sphinxcontrib-bibtex>=2.0
   # main
   - aenum
   - attrs>=22.2
   - cachetools>=5.3
   - click
   - dessinemoi>=23.1.0
   - dynaconf>=3.2
-  - importlib_resources
   - joseki>=2.6.0
   - lazy_loader>=0.1
   - matplotlib>=3.3
   - netcdf4
   - numpy
   - pint
   - pinttrs>=23.2.0
@@ -41,19 +41,19 @@
   - ruamel.yaml
   - scipy
   - sf-hamilton>=1.40
   - shellingham!=1.5.1
   - tqdm
   - typer>=0.9.0
   - xarray>=0.19,!=0.20.*
+  # optional
   # recommended
   - aabbtree
   - astropy
   - ipython
   - ipywidgets
   - jupyterlab
   - python-dateutil
   - python-graphviz
-  - seaborn
   # tests
   - pytest
   - pytest-json-report
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-docs-linux-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-docs-linux-64.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 60ddbda9593aef782cabb255ec786ee0bfcb86d57116ead3ab460ee29f6f829b
+# input_hash: ec73d7b1b91349285e67c061312a5e1f339f025fb4010d62a796c29ff79bb313
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda#2f4327a1cbe7f022401b236e915a5fef
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda#f6f6600d18a4047b54f803cf708b868a
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda#10569984e7db886e4f1abc2b47ad79a1
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda#3cfab3e709f77e9f1b3d380eb622494a
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.13-ha770c72_0.conda#9105ee57dc4869bc5d1876b531202676
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-4_cp39.conda#bfe4b3259a8ac6cdf0037752904da6a7
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda#aae89d3736661c36a5591788aebd0817
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda#df88796bd09a0d2ed292e59101478ad8
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.11-hd590300_1.conda#0bb492cca54017ea314b809b1ee3a176
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
@@ -32,23 +32,23 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-h43f5ff8_6.conda#e54a5ddc67e673f9105cf2a2e9c070b0
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.4.0-hd590300_0.conda#b26e8aa824079e1be0294e7152ca4559
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.32.6-h59595ed_0.conda#9160cdeb523a1b20cf8d2a0bf821f45d
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda#97da8860a0da5413c7c98a3b3838a645
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda#9d731343cff6ee2e5a25c4a091bf8e2a
@@ -70,37 +70,37 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.69-h0f662aa_0.conda#25cb5999faa414e5ccb2c1388f62d3d5
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_6.conda#3666a850342f8f3be88f9a93d948d027
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda#b3316cbe90249da4f8e84cd66e1cc55b
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_2.conda#9a3a42df8a95f65334dfc7b80da1195d
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
 https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.3.0-hf1915f5_4.conda#784a4df6676c581ca624fbe460703a6d
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h59595ed_1.conda#7fc9d3288d2420bb3637647621018000
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_6.conda#9342e7c44c38bea649490f72d92c382d
 https://conda.anaconda.org/conda-forge/linux-64/libllvm15-15.0.7-hb3ce162_4.conda#8a35df3cbc0c8b12cc8af9473ae75eef
 https://conda.anaconda.org/conda-forge/linux-64/libllvm18-18.1.3-h2448989_0.conda#927b6d6e80b2c0d4405a58b61ca248a3
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
 https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.3.0-hca2cd23_4.conda#1b50eebe2a738a3146c154d2eceaa8b6
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.98-h1d7d5a4_0.conda#54b56c2fdf973656b748e0378900ec13
 https://conda.anaconda.org/conda-forge/linux-64/python-3.9.19-h0755675_0_cpython.conda#d9ee3647fbd9e8595b8df759b2bbefb8
@@ -119,78 +119,83 @@
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py39hf3d152e_4.conda#0d71b15b6e77f2ae2ef81a478a384ead
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py39hf3d152e_5.conda#d74cf0b3351ffc48f1388424df827755
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_4.conda#c9deba4959ea5b5f72f1e3e4a71ae014
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_6.conda#a9d23c02485c5cf055f9ac90eb9c9c63
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py39h7633fee_1.conda#c9f74d717e5a2847a9f8b779c54130f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang-cpp15-15.0.7-default_h127d8a8_5.conda#d0a9633b53cdc319b8a1a532ae7822b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-18.1.3-default_h5d6823c_0.conda#5fff487759736b275dc3e4a263cac666
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h4637d8d_4.conda#d4529f4dff3057982a7617c7ac58fde3
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
-https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.48-h71f35ed_0.conda#4d18d86916705d352d5f4adfb7f0edd3
+https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.49-h4f305b6_0.conda#dfcfd72c7a430d3616763ecfbefe4ca9
 https://conda.anaconda.org/conda-forge/linux-64/libpq-16.2-h33b98f1_1.conda#9e49ec2a61d02623b379dc332eb6889d
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py39hd1e30aa_0.conda#9a9a22eb1f83c44953319ee3b027769f
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.2-pyhd8ed1ab_0.conda#5cbee699846772cc939bef23a0d524ed
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py39hd1e30aa_1.conda#37218233bcdc310e4fde6453bc1b40d8
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py39h8c080ef_0.conda#852eb7bf636d4108530a27100c23f1c1
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.2-py39ha1047a2_0.conda#916ab2d35fbe7a2ad3ba03f96c78922d
 https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.18.0-py39h9fdd4d6_0.conda#ca1e1ff2be5c41142e412c83b88960e4
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py39hd1e30aa_0.conda#b1961e70cfe8e1eac243faf933d1813f
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py39hd1e30aa_0.conda#1e865e9188204cdfb1fd2531780add88
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.1.0-py39hd1e30aa_0.conda#1da984bbb6e765743e13388ba7b7b2c8
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
+https://conda.anaconda.org/conda-forge/linux-64/websockets-12.0-py39hd1e30aa_0.conda#34476c3670224efb4000f20c8c42eb5b
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.41-hd590300_0.conda#81f740407b45e3f9047b3174fa94eb9e
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
+https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py39hd1e30aa_0.conda#79f5dd8778873faa54e8f7b2729fe8a6
-https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_4.conda#5521382ee30b96b35eb0037fc3c4f2b4
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_6.conda#a1e026a82a562b443845db5614ca568a
+https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py39hf3d152e_0.conda#612f7a003a8a407955572c0d53952ceb
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
@@ -200,69 +205,76 @@
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.2-hc60ed4a_1.conda#ef1910918dd895516a769ed36b5b3a4e
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.7.0-h662e7e4_0.conda#b32c0da42b1f24a98577bb3d7fc0b995
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py39h90c7501_0.conda#1e3b6af9592be71ce19f0a6aae05d97b
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py39hd1e30aa_0.conda#2289054e90cf07e35280bbe798811dc8
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.12-py39h3d6467e_0.conda#e667a3ab0df62c54e60e1843d2e6defb
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.24.1-h98fc4e7_1.conda#b04b5cdf3ba01430db27979250bc5a1d
-https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.4.0-h3d44ed6_0.conda#27f46291a6aaa3c2a4f798ebd35a7ddb
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-255-h3516f8a_1.conda#3366af27f0b593544a6cd453c7932ac5
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py39h474f0d3_0.conda#aa265f5697237aa13cc10f53fa8acc4f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.12.2-py39h3d6467e_5.conda#93aff412f3e49fdb43361c0215cbd72d
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
+https://conda.anaconda.org/conda-forge/linux-64/uvicorn-0.29.0-py39hf3d152e_0.conda#0d7cbecfb218788337acd7737c8d7fd4
+https://conda.anaconda.org/conda-forge/linux-64/watchfiles-0.21.0-py39h9fdd4d6_0.conda#176ddbfc26cc9da781910e18d600bf86
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py39h44dd56e_0.conda#baea2f5dfb3ab7b1c836385d2e1daca7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py39h7633fee_0.conda#bdc188e59857d6efab332714e0d01d93
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.24.1-hfa15dee_1.conda#a6dd2bbc684913e2bef0a54ce56fcbfb
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.1-py39hddac248_0.conda#85293a042c24a08e71b7608ee66b6134
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.2-py39hddac248_0.conda#259c4e76e6bda8888aefc098ae1ba749
+https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-17.0-hb77b528_0.conda#07f45f1be1c25345faddb8db0de8039b
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.3-py39hf3d152e_1.conda#90a592a19a0de2536d9e63886a569715
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py39h474f0d3_0.conda#46ae0ecba9726ab4fa44c78fefa522cf
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py39he9076e7_0.conda#1919384a8420e7bb25f6c3a582e0857c
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda#0b57b5368ab7fc7cdc9e3511fa867214
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py39h4282601_100.conda#d2809fbf0d8ae7b8ca92c456cb44a7d4
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-hc9dc06e_21.conda#b325046180590c868ce0dbf267b82eb8
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
+https://conda.anaconda.org/conda-forge/linux-64/statsmodels-0.14.1-py39h44dd56e_0.conda#dc565186b972bd87e49b9c35390ddd8c
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.9-py39h52134e7_5.conda#e1f148e57d071b09187719df86f513c1
+https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.8.4-py39hf3d152e_0.conda#c66d2da2669fddc657b679bccab95775
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
+https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-docs-osx-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-docs-osx-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 1fc0409bba384f1aaa011827456f35dcda6bb09614b3f7bcfff7f34662d79e41
+# input_hash: 2bfe58b1db5172ba204ce507d8d309d0509ccbbabe56aebea7422cfbc77d8c18
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda#6097a6ca9ada32699b5fc4312dd6ef18
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.28.1-h10d778d_0.conda#d5eb7992227254c0e9a0ce71151f0079
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda#f2eacee8c33c43692f1ccfd33d0f50b1
 https://conda.anaconda.org/conda-forge/osx-64/icu-73.2-hf5e326d_0.conda#5cc301d759ec03f28328428e28f65591
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.1.0-h0dc2134_1.conda#9e6c31441c9aa24e41ace40d6151aab6
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.20-h49d49c5_0.conda#d46104f6a896a0bc6a1d37b88b2edf5c
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-h10d778d_2.conda#899db79329439820b7e8f8de41bca902
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hd75f5a5_2.conda#6c3628d047e151efba7cf08c5e54d1ca
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-3.0.0-h0dc2134_1.conda#72507f8e3961bc968af17435060b6dd6
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.2-h10d778d_1.conda#1ff09ca6e85ee516442a6a94cdfc7065
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.4.0-h10d778d_0.conda#b2c0047ea73819d992484faacbbe1c24
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-18.1.3-hb6ac08f_0.conda#506f270f4f00980d27cc1fc127e0ed37
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda#50f28c512e9ad78589e3eab34833f762
 https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.13-h694c41f_0.conda#569f0ad9ff2d8654e5630d5a3232e6f1
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.9-4_cp39.conda#2d9f6c00555127a9058cfa955adf1090
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
@@ -30,17 +30,17 @@
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.1.3-h73e2aa4_0.conda#66d3c1f6dd4636216b4fca7a748d50eb
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.1.0-h0dc2134_1.conda#9ee0bab91b2ca579e10353738be36063
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.1.0-h0dc2134_1.conda#8a421fe09c6187f0eb5e2338a8a8be6d
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-13.2.0-h2873a65_3.conda#e4fb4d23ec2870ff3c40d10afe305aec
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda#65dcddb15965c9de2c0365cb14910532
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda#086f56e13a96a6cfb1bf640505ae6b70
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda#68e462226209f35182ef66eda0f794ff
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda#bd85e0ca9e1ffaadc3b56079fd956035
+https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda#50b997370584f2c83ca0c38e9028eab9
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda#570a6f04802df580be529f3a72d2bbf7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.2.0-h6dc393e_1.conda#9c322ec36340610fcf213b72999b049e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda#bf830ba5afc507c6232d4ef0fb1a882d
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-h93d8f39_0.conda#4c055e46b394be36681fe476c1e2ee6e
 https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
@@ -64,77 +64,82 @@
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py39h6e9494a_4.conda#2075bada3661d0a7fb762b4f84f7c06a
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py39h6e9494a_5.conda#7738300100023129d58567edc49ee90b
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.5-py39h8ee36c8_1.conda#6072db04642b21329b0502a177ec18bf
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.16-ha2f27b4_0.conda#1442db8f03517834843666c422238c9b
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.7.1-h726d00d_0.conda#fa58e5eaa12006bc3289a71357bef167
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.27-openmp_hfef2a42_0.conda#00237c9c7f2cb6725fe2960680a6e225
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.5-py39ha09f3b3_0.conda#db347b50af50d030b73be1d1e457cac2
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.2-pyhd8ed1ab_0.conda#5cbee699846772cc939bef23a0d524ed
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.2-h7310d3a_0.conda#05a14cc9d725dd74995927968d6547e3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py39hdc70f33_1.conda#542378f49240a94056b50ab1385b3bfb
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py39hcb7a90d_0.conda#39754a321b3dece3df9a0eb213d43dc8
+https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.2-py39hffc4518_0.conda#13c761db6b475447b63702e5f7ee3015
 https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.18.0-py39hcf47035_0.conda#0e8641e9f0d42d844cf17f5520225e6e
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.8-py39ha09f3b3_0.conda#835c656934865805c0b02dbff74fe5b7
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py39ha09f3b3_0.conda#4541517b5a605bf45d4a5fb074bb4cf5
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.1.0-py39hdc70f33_0.conda#ede122e9ef2775a8879063d9d3ee819f
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
+https://conda.anaconda.org/conda-forge/osx-64/websockets-12.0-py39ha09f3b3_0.conda#14a37a956881ee2df098931d2c8b40c9
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
+https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.51.0-py39ha09f3b3_0.conda#713f4aa3625e861796da39bbeb112675
+https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.3-nompi_h691f4bf_100.conda#8e2ac4ae815a8c9743fe37d70f48f075
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.1-py39h6e9494a_0.conda#9611b1806866adc1693cfb5a323f16e4
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-22_osx64_openblas.conda#b80966a8c8dd0b531f8e65f709d732e8
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py39h9dabb2a_0.conda#e385068c9511542eff20422f7e799064
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.18.6-py39ha09f3b3_0.conda#6eb863d10b7aeef1f58ba1ebf92f59bd
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
@@ -144,42 +149,49 @@
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-22_osx64_openblas.conda#f21b282ff7ba14df6134a0fe6ab42b1b
 https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_h7760872_113.conda#bce76ace6497221c2a2a02840aaceac5
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
+https://conda.anaconda.org/conda-forge/osx-64/uvicorn-0.29.0-py39h6e9494a_0.conda#79786774d034370e5e7bf2707b7613d5
+https://conda.anaconda.org/conda-forge/osx-64/watchfiles-0.21.0-py39h3f9c672_0.conda#9c6ce8f29c4c66782417b26bb4a7d5dd
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.26.4-py39h28c39a1_0.conda#1b07000dc6aed4a69e91107dac4464d3
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.3-py39h6e9494a_1.conda#450b8f37439740c0e79acbeba7d1d678
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.3-py39h5b4affa_0.conda#20fd617b1f9fcefe5ec1577d38ae7bdb
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.2.1-py39h0ca7971_0.conda#a4c478d3b64c81d1742dc8073e4996b6
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda#0b57b5368ab7fc7cdc9e3511fa867214
-https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.1-py39haf03413_0.conda#d29dc35b665029951dae988810f84508
+https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.2-py39haf03413_0.conda#11225cf1f769af217ffc01f0a21d40fa
+https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.13.0-py39h0ed1e0f_0.conda#3a4d0af4fe2006bedc33ca61e9a0b4d6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.8.4-py39h7070ae8_0.conda#cb9e1f8aff1f759b9685e908f9dc0a5b
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.5-nompi_py39h824b2b2_100.conda#07525171115894fe9c4aba755460c51a
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
+https://conda.anaconda.org/conda-forge/osx-64/statsmodels-0.14.1-py39h5b4affa_0.conda#4cc025969fa47342955213653d1352c8
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.8.4-py39h6e9494a_0.conda#371fe0f738d9f3baa20cf06656b78b0a
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
+https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
+https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-docs-win-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-docs-win-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: fdc29eea9fb50c1f619e26b589c039d8ffbe7e4756e93db1f1068f6447e5be85
+# input_hash: b0c0d0c31011c2889b3afdb275ef0154448a22a6302dd310c7f8859c75bb24bd
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda#63da060240ab8087b60d1357051ea7d6
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda#30ebb9fd99666d8b8675fcee541a09f3
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda#c66eb2fd33b999ccc258aef85689758e
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-0.22.5-h5728263_2.conda#75a6982b9ff0a8db0f53303527b07af8
 https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2#b0309b72560df66f71a9d5e34a5efdfa
 https://conda.anaconda.org/conda-forge/win-64/pandoc-3.1.13-h57928b3_0.conda#4caaf4c37a0efc8a06492dba2d871bbb
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.9-4_cp39.conda#948b0d93d4ab1372d8fd45e1560afd47
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-devel-0.22.5-h5728263_2.conda#8377da2cc31200d7181d2e48d60e4c7b
@@ -24,16 +24,16 @@
 https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.1.0-hcfcfb64_1.conda#f77f319fb82980166569e1280d5b2864
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.20-hcfcfb64_0.conda#b12b5bde5eb201a1df75e49320cc938a
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda#e1eb10b1cca179f2baa3601e4efc8712
 https://conda.anaconda.org/conda-forge/win-64/libjpeg-turbo-3.0.0-hcfcfb64_1.conda#3f1b948619c45b1ca714d60c7389092c
 https://conda.anaconda.org/conda-forge/win-64/libogg-1.3.4-h8ffe710_1.tar.bz2#04286d905a0dcb7f7d4a12bdfe02516d
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda#f95359f8dc5abf7da7776ece9ef10bc5
-https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.2-hcfcfb64_1.conda#fdf80cb33c32d4d002bb89c37cfff5b7
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda#73f5dc8e2d55d9a1e14b11f49c3b4a28
+https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.4.0-hcfcfb64_0.conda#abd61d0ab127ec5cd68f62c2969e6f34
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda#958e0418e93e50c575bff70fbcaa12d8
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
 https://conda.anaconda.org/conda-forge/win-64/snappy-1.2.0-hfb803bf_1.conda#a419bf04a7c76a46639e315ac1b8bf72
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda#fc048363eb8f03cd1737600a5d08aafe
@@ -43,15 +43,15 @@
 https://conda.anaconda.org/conda-forge/win-64/krb5-1.21.2-heb0366b_0.conda#6e8b0f22b4eef3b3cb3849bb4c3d47f9
 https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.1.0-hcfcfb64_1.conda#19ce3e1dacc7912b3d6ff40690ba9ae0
 https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.1.0-hcfcfb64_1.conda#71e890a0b361fd58743a13f77e1506b7
 https://conda.anaconda.org/conda-forge/win-64/libintl-0.22.5-h5728263_2.conda#aa622c938af057adc119f8b8eecada01
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.43-h19919ed_0.conda#77e398acc32617a0384553aea29e866b
 https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
 https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2#e1a22282de0169c93e4ffe6ce6acc212
-https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_1.conda#eb9f59dd51f50f5aa369813fa63ba569
+https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_2.conda#ac7af7a949db01dae61ddc48f4a93d79
 https://conda.anaconda.org/conda-forge/win-64/libzip-1.10.1-h1d365fa_3.conda#5c629cd12d89e2856c17b1dc5fcf44a4
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.43-h17e33f8_0.conda#d0485b8aa2cedb141a7bd27b4efa4c9c
 https://conda.anaconda.org/conda-forge/win-64/python-3.9.19-h4de0772_0_cpython.conda#b6999bc275e0e6beae7b1c8ea0be1e85
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-h63175ca_1.conda#e8867cc4d023f41f54bd64a33436b0a1
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda#792bb5da68bf0a6cac6a6072ecb8dbeb
@@ -64,75 +64,80 @@
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py39hcbf5309_4.conda#adae8d63d214069960445c1aba41eea5
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py39hcbf5309_5.conda#461b44faa5dd942c6be4405a8df37587
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-hdaf720e_2.conda#3761b23693f768dc75a8fd0a73ca053f
 https://conda.anaconda.org/conda-forge/win-64/gettext-tools-0.22.5-h7d00a51_2.conda#ef1c3bb48c013099c4872640a5f2096c
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.5-py39h1f6ef14_1.conda#4fc5bd0a7b535252028c647cc27d6c87
 https://conda.anaconda.org/conda-forge/win-64/libclang13-18.1.3-default_hf64faad_0.conda#9217c37b478ec601af909aafc954a6fc
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.7.1-hd5e4a3a_0.conda#3396aff340d0903e8814c2852d631e4e
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-0.22.5-h5728263_2.conda#f4c826b19bf1ccee2a63a2c685039728
-https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_4.conda#9baf04fc7002450a932cf97cb9625ebb
-https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda#87da045f6d26ce9fe20ad76a18f6a18a
+https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_6.conda#cd5c6efbe213c089f78575c98ab9a0ed
+https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda#ee944f0d41d9e2048f9d7492c1623ca3
 https://conda.anaconda.org/conda-forge/win-64/libintl-devel-0.22.5-h5728263_2.conda#a2ad82fae23975e4ccbfab2847d31d48
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.6.0-hddb2be6_3.conda#6d1828c9039929e2f185c5fa9d133018
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py39ha55989b_0.conda#f8b7e33c8bf98901925817b7f4436c7e
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.2-pyhd8ed1ab_0.conda#5cbee699846772cc939bef23a0d524ed
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py39h99910a6_2.conda#eab91442160b49994dd2e224e6082770
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py39ha55989b_1.conda#5c3a9da77fc79c21c5c1fd7ea06306a2
-https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py39h7eaf5a6_0.conda#113b93bd971d355b1d52df09c1161628
+https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.2-py39h03e5c00_0.conda#5e1e67cb1d03a2cce828bac7aa6642a5
 https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.18.0-py39hf21820d_0.conda#32fa6863c2216dbe787adaf874433713
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.8-py39ha55989b_0.conda#07aae1fdd812b411cec84c0d47339d22
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py39ha55989b_0.conda#d8f52e8e1d02f9a5901f9224e2ddf98f
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.1.0-py39ha55989b_0.conda#20ec896e8d97f2ff8be1124e624dc8f2
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
+https://conda.anaconda.org/conda-forge/win-64/websockets-12.0-py39ha55989b_0.conda#24b1cf33f77a58400a2098e0cdc04e8f
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
+https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/conda-forge/win-64/brotli-1.1.0-hcfcfb64_1.conda#f47f6db2528e38321fb00ae31674c133
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda#3549ecbceb6cd77b91a105511b7d0786
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
-https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_4.conda#44cd44c004db728bf5788c1d46ce7334
+https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_6.conda#40d452e4012c00f644b1dd6319fcdbcf
+https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.14.3-nompi_h73e8ff5_100.conda#1e91ce0f3a914b0dab762539c0df4ff1
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py39hcbf5309_0.conda#78ec20214b67efe5caebb4f08bdee094
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
@@ -141,39 +146,42 @@
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.15-hcd874cb_0.conda#090d91b69396f14afef450c285f9758c
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda#7e7099ad94ac3b599808950cec30ad4e
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.18.6-py39ha55989b_0.conda#7839645d467f5d3bc52709a3d484fa62
 https://conda.anaconda.org/conda-forge/win-64/sip-6.7.12-py39h99910a6_0.conda#0cc5774390ada632ed7975203057c91c
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda#21069f3ed16812f9f4f2700667b6ec86
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda#21745fdd12f01b41178596143cbecffd
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/win-64/fonttools-4.51.0-py39ha55989b_0.conda#5d19302bab29e347116b743e793aa7d6
 https://conda.anaconda.org/conda-forge/win-64/gettext-0.22.5-h5728263_2.conda#da84216f88a8c89eb943c683ceb34d7d
-https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_4.conda#d0a05e8a76abb68b2beb7b16c6d49213
+https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_6.conda#a4036d0bc6f499ebe9fef7b887f3ca0f
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.9.2-nompi_h07c049d_113.conda#2aa431a5a05e3679eea4faad0f47b119
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/win-64/mkl-2024.1.0-h66d3029_692.conda#b43ec7ed045323edeff31e348eea8652
 https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py39h9ee4981_0.conda#6d69d57c41867acc162ef0205a8efaef
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.12.2-py39h99910a6_5.conda#dffbcea794c524c471772a5f697c2aea
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
+https://conda.anaconda.org/conda-forge/win-64/uvicorn-0.29.0-py39hcbf5309_0.conda#75e90ff63b09f4443258dd7829bb6032
+https://conda.anaconda.org/conda-forge/win-64/watchfiles-0.21.0-py39hf21820d_0.conda#5409cf692b0dec68648e6e8a6721e5ee
 https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.24.1-hb4038d2_1.conda#8a6dfe53ad02a3b151e6383a950043ee
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-22_win64_mkl.conda#65c56ecdeceffd6c32d3d54db7e02c6e
 https://conda.anaconda.org/conda-forge/win-64/pybtex-docutils-1.0.3-py39hcbf5309_1.conda#0131fba9b943b68a01e2ac623004c48f
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
@@ -184,32 +192,36 @@
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.26.4-py39hddb5d58_0.conda#6e30ff8f2d3f59f45347dfba8bc22a04
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-hcef0176_21.conda#76544d3dfeff8fd52250df168cb0005b
 https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.3-py39hd88c2e4_0.conda#12e356a0e7e5a8e67538aa66fbd21c47
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.2.1-py39h1f6ef14_0.conda#03e25c6bae87f4f9595337255b44b0fb
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
-https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.1-py39h32e6231_0.conda#7ca03abc7f2f9c91a9fdc02780bfa572
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
+https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.2-py39h32e6231_0.conda#0df69e098aa54373d4edb3eaaa2338ba
+https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
 https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.9-py39hb77abff_5.conda#5ed899124a51958336371ff01482b8fd
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.13.0-py39hddb5d58_0.conda#cfe749056fb9ed9dbc096b5751becf34
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.8.4-py39hf19769e_0.conda#7836c3dc5814f6d55a7392657c576e88
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
 https://conda.anaconda.org/conda-forge/win-64/netcdf4-1.6.5-nompi_py39h9a3bb69_100.conda#e271773571fa2908d8fd598878890db2
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
+https://conda.anaconda.org/conda-forge/win-64/statsmodels-0.14.1-py39hd88c2e4_0.conda#b51565db0ed851e9031da82171d0e02f
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.8.4-py39hcbf5309_0.conda#cc66c372d5eb745665da06ce56b7d72b
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
+https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
+https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-docs.yml` & `eradiate-0.27.0rc1/requirements/conda/environment-docs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 dependencies:
   # default
   - python=3.9
   # docs
   - autodocsumm
   - myst-parser
   - nbsphinx>=0.9.0
+  - seaborn
   - sphinx
   - sphinx-autobuild
   - sphinx-book-theme>=1.0
   - sphinx-copybutton
   - sphinx-design
   - sphinxcontrib-bibtex>=2.0
   # main
   - aenum
   - attrs>=22.2
   - cachetools>=5.3
   - click
   - dessinemoi>=23.1.0
   - dynaconf>=3.2
-  - importlib_resources
   - joseki>=2.6.0
   - lazy_loader>=0.1
   - matplotlib>=3.3
   - netcdf4
   - numpy
   - pint
   - pinttrs>=23.2.0
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-main-linux-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-main-linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 75a4f851fadaade2f108f24f50388a2b911e9a6bf3b74d5e299028f50c27c755
+# input_hash: 7b572c9cec772c110dbacafccb8d9cfe2c58d334785cc68f78608da0a8b164be
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda#2f4327a1cbe7f022401b236e915a5fef
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda#f6f6600d18a4047b54f803cf708b868a
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda#10569984e7db886e4f1abc2b47ad79a1
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda#3cfab3e709f77e9f1b3d380eb622494a
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-4_cp39.conda#bfe4b3259a8ac6cdf0037752904da6a7
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda#aae89d3736661c36a5591788aebd0817
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda#df88796bd09a0d2ed292e59101478ad8
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.11-hd590300_1.conda#0bb492cca54017ea314b809b1ee3a176
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
@@ -31,22 +31,22 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-h43f5ff8_6.conda#e54a5ddc67e673f9105cf2a2e9c070b0
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.4.0-hd590300_0.conda#b26e8aa824079e1be0294e7152ca4559
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.32.6-h59595ed_0.conda#9160cdeb523a1b20cf8d2a0bf821f45d
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda#97da8860a0da5413c7c98a3b3838a645
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda#9d731343cff6ee2e5a25c4a091bf8e2a
@@ -67,36 +67,36 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.69-h0f662aa_0.conda#25cb5999faa414e5ccb2c1388f62d3d5
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_6.conda#3666a850342f8f3be88f9a93d948d027
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda#b3316cbe90249da4f8e84cd66e1cc55b
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_2.conda#9a3a42df8a95f65334dfc7b80da1195d
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
 https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.3.0-hf1915f5_4.conda#784a4df6676c581ca624fbe460703a6d
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_6.conda#9342e7c44c38bea649490f72d92c382d
 https://conda.anaconda.org/conda-forge/linux-64/libllvm15-15.0.7-hb3ce162_4.conda#8a35df3cbc0c8b12cc8af9473ae75eef
 https://conda.anaconda.org/conda-forge/linux-64/libllvm18-18.1.3-h2448989_0.conda#927b6d6e80b2c0d4405a58b61ca248a3
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
 https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.3.0-hca2cd23_4.conda#1b50eebe2a738a3146c154d2eceaa8b6
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.98-h1d7d5a4_0.conda#54b56c2fdf973656b748e0378900ec13
 https://conda.anaconda.org/conda-forge/linux-64/python-3.9.19-h0755675_0_cpython.conda#d9ee3647fbd9e8595b8df759b2bbefb8
@@ -114,40 +114,40 @@
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_4.conda#c9deba4959ea5b5f72f1e3e4a71ae014
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_6.conda#a9d23c02485c5cf055f9ac90eb9c9c63
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py39h7633fee_1.conda#c9f74d717e5a2847a9f8b779c54130f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang-cpp15-15.0.7-default_h127d8a8_5.conda#d0a9633b53cdc319b8a1a532ae7822b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-18.1.3-default_h5d6823c_0.conda#5fff487759736b275dc3e4a263cac666
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h4637d8d_4.conda#d4529f4dff3057982a7617c7ac58fde3
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
-https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.48-h71f35ed_0.conda#4d18d86916705d352d5f4adfb7f0edd3
+https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.49-h4f305b6_0.conda#dfcfd72c7a430d3616763ecfbefe4ca9
 https://conda.anaconda.org/conda-forge/linux-64/libpq-16.2-h33b98f1_1.conda#9e49ec2a61d02623b379dc332eb6889d
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py39hd1e30aa_0.conda#b1961e70cfe8e1eac243faf933d1813f
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py39hd1e30aa_0.conda#1e865e9188204cdfb1fd2531780add88
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.1.0-py39hd1e30aa_0.conda#1da984bbb6e765743e13388ba7b7b2c8
@@ -155,15 +155,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.41-hd590300_0.conda#81f740407b45e3f9047b3174fa94eb9e
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py39hd1e30aa_0.conda#79f5dd8778873faa54e8f7b2729fe8a6
-https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_4.conda#5521382ee30b96b35eb0037fc3c4f2b4
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_6.conda#a1e026a82a562b443845db5614ca568a
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.3-hd590300_0.conda#32d16ad533c59bb0a3c5ffaf16110829
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.2-hc60ed4a_1.conda#ef1910918dd895516a769ed36b5b3a4e
@@ -175,35 +175,35 @@
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py39hd1e30aa_0.conda#2289054e90cf07e35280bbe798811dc8
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.12-py39h3d6467e_0.conda#e667a3ab0df62c54e60e1843d2e6defb
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.24.1-h98fc4e7_1.conda#b04b5cdf3ba01430db27979250bc5a1d
-https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.4.0-h3d44ed6_0.conda#27f46291a6aaa3c2a4f798ebd35a7ddb
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-255-h3516f8a_1.conda#3366af27f0b593544a6cd453c7932ac5
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py39h474f0d3_0.conda#aa265f5697237aa13cc10f53fa8acc4f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.12.2-py39h3d6467e_5.conda#93aff412f3e49fdb43361c0215cbd72d
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py39h44dd56e_0.conda#baea2f5dfb3ab7b1c836385d2e1daca7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py39h7633fee_0.conda#bdc188e59857d6efab332714e0d01d93
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.24.1-hfa15dee_1.conda#a6dd2bbc684913e2bef0a54ce56fcbfb
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.1-py39hddac248_0.conda#85293a042c24a08e71b7608ee66b6134
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.2-py39hddac248_0.conda#259c4e76e6bda8888aefc098ae1ba749
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-17.0-hb77b528_0.conda#07f45f1be1c25345faddb8db0de8039b
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py39h474f0d3_0.conda#46ae0ecba9726ab4fa44c78fefa522cf
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py39he9076e7_0.conda#1919384a8420e7bb25f6c3a582e0857c
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py39h4282601_100.conda#d2809fbf0d8ae7b8ca92c456cb44a7d4
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-hc9dc06e_21.conda#b325046180590c868ce0dbf267b82eb8
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.9-py39h52134e7_5.conda#e1f148e57d071b09187719df86f513c1
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.8.4-py39hf3d152e_0.conda#c66d2da2669fddc657b679bccab95775
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-main-osx-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-main-osx-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: eb11a2d8eb89786097a27487924072f85f65d5922f61721c5dd27c31fd301a83
+# input_hash: 9a27640db306d64567b7c93c59d01122bcbcac0a9f767a7403acc09f23ec469e
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda#6097a6ca9ada32699b5fc4312dd6ef18
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.28.1-h10d778d_0.conda#d5eb7992227254c0e9a0ce71151f0079
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda#f2eacee8c33c43692f1ccfd33d0f50b1
 https://conda.anaconda.org/conda-forge/osx-64/icu-73.2-hf5e326d_0.conda#5cc301d759ec03f28328428e28f65591
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.1.0-h0dc2134_1.conda#9e6c31441c9aa24e41ace40d6151aab6
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.20-h49d49c5_0.conda#d46104f6a896a0bc6a1d37b88b2edf5c
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-h10d778d_2.conda#899db79329439820b7e8f8de41bca902
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hd75f5a5_2.conda#6c3628d047e151efba7cf08c5e54d1ca
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-3.0.0-h0dc2134_1.conda#72507f8e3961bc968af17435060b6dd6
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.2-h10d778d_1.conda#1ff09ca6e85ee516442a6a94cdfc7065
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.4.0-h10d778d_0.conda#b2c0047ea73819d992484faacbbe1c24
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-18.1.3-hb6ac08f_0.conda#506f270f4f00980d27cc1fc127e0ed37
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda#50f28c512e9ad78589e3eab34833f762
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.9-4_cp39.conda#2d9f6c00555127a9058cfa955adf1090
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
@@ -27,17 +27,17 @@
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.1.3-h73e2aa4_0.conda#66d3c1f6dd4636216b4fca7a748d50eb
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.1.0-h0dc2134_1.conda#9ee0bab91b2ca579e10353738be36063
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.1.0-h0dc2134_1.conda#8a421fe09c6187f0eb5e2338a8a8be6d
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-13.2.0-h2873a65_3.conda#e4fb4d23ec2870ff3c40d10afe305aec
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda#65dcddb15965c9de2c0365cb14910532
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda#086f56e13a96a6cfb1bf640505ae6b70
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda#68e462226209f35182ef66eda0f794ff
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda#bd85e0ca9e1ffaadc3b56079fd956035
+https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda#50b997370584f2c83ca0c38e9028eab9
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda#570a6f04802df580be529f3a72d2bbf7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.2.0-h6dc393e_1.conda#9c322ec36340610fcf213b72999b049e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda#bf830ba5afc507c6232d4ef0fb1a882d
 https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda#80abc41d0c48b82fe0f04e7f42f5cb7e
@@ -58,32 +58,32 @@
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.5-py39h8ee36c8_1.conda#6072db04642b21329b0502a177ec18bf
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.16-ha2f27b4_0.conda#1442db8f03517834843666c422238c9b
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.7.1-h726d00d_0.conda#fa58e5eaa12006bc3289a71357bef167
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.27-openmp_hfef2a42_0.conda#00237c9c7f2cb6725fe2960680a6e225
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.2-h7310d3a_0.conda#05a14cc9d725dd74995927968d6547e3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.8-py39ha09f3b3_0.conda#835c656934865805c0b02dbff74fe5b7
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py39ha09f3b3_0.conda#4541517b5a605bf45d4a5fb074bb4cf5
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.1.0-py39hdc70f33_0.conda#ede122e9ef2775a8879063d9d3ee819f
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
@@ -110,17 +110,17 @@
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.26.4-py39h28c39a1_0.conda#1b07000dc6aed4a69e91107dac4464d3
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.3-py39h5b4affa_0.conda#20fd617b1f9fcefe5ec1577d38ae7bdb
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.2.1-py39h0ca7971_0.conda#a4c478d3b64c81d1742dc8073e4996b6
-https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.1-py39haf03413_0.conda#d29dc35b665029951dae988810f84508
+https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.2-py39haf03413_0.conda#11225cf1f769af217ffc01f0a21d40fa
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.13.0-py39h0ed1e0f_0.conda#3a4d0af4fe2006bedc33ca61e9a0b4d6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.8.4-py39h7070ae8_0.conda#cb9e1f8aff1f759b9685e908f9dc0a5b
 https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.5-nompi_py39h824b2b2_100.conda#07525171115894fe9c4aba755460c51a
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.8.4-py39h6e9494a_0.conda#371fe0f738d9f3baa20cf06656b78b0a
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-main-win-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-main-win-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: ae79d6c8f77a4025f83607ea33add72fb0e7594c0e2541cb8ba67c0c9de75466
+# input_hash: f21962fd543545651a0c09a2f835c6abf6accf18b527b98395fa2fc50f5c5acd
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda#63da060240ab8087b60d1357051ea7d6
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda#30ebb9fd99666d8b8675fcee541a09f3
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda#c66eb2fd33b999ccc258aef85689758e
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-0.22.5-h5728263_2.conda#75a6982b9ff0a8db0f53303527b07af8
 https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2#b0309b72560df66f71a9d5e34a5efdfa
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.9-4_cp39.conda#948b0d93d4ab1372d8fd45e1560afd47
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-devel-0.22.5-h5728263_2.conda#8377da2cc31200d7181d2e48d60e4c7b
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2#53a1c73e1e3d185516d7e3af177596d9
@@ -22,16 +22,16 @@
 https://conda.anaconda.org/conda-forge/win-64/libaec-1.1.3-h63175ca_0.conda#8723000f6ffdbdaef16025f0a01b64c5
 https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.1.0-hcfcfb64_1.conda#f77f319fb82980166569e1280d5b2864
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.20-hcfcfb64_0.conda#b12b5bde5eb201a1df75e49320cc938a
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda#e1eb10b1cca179f2baa3601e4efc8712
 https://conda.anaconda.org/conda-forge/win-64/libjpeg-turbo-3.0.0-hcfcfb64_1.conda#3f1b948619c45b1ca714d60c7389092c
 https://conda.anaconda.org/conda-forge/win-64/libogg-1.3.4-h8ffe710_1.tar.bz2#04286d905a0dcb7f7d4a12bdfe02516d
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda#f95359f8dc5abf7da7776ece9ef10bc5
-https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.2-hcfcfb64_1.conda#fdf80cb33c32d4d002bb89c37cfff5b7
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda#73f5dc8e2d55d9a1e14b11f49c3b4a28
+https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.4.0-hcfcfb64_0.conda#abd61d0ab127ec5cd68f62c2969e6f34
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda#958e0418e93e50c575bff70fbcaa12d8
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
 https://conda.anaconda.org/conda-forge/win-64/snappy-1.2.0-hfb803bf_1.conda#a419bf04a7c76a46639e315ac1b8bf72
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda#fc048363eb8f03cd1737600a5d08aafe
@@ -40,15 +40,15 @@
 https://conda.anaconda.org/conda-forge/win-64/krb5-1.21.2-heb0366b_0.conda#6e8b0f22b4eef3b3cb3849bb4c3d47f9
 https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.1.0-hcfcfb64_1.conda#19ce3e1dacc7912b3d6ff40690ba9ae0
 https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.1.0-hcfcfb64_1.conda#71e890a0b361fd58743a13f77e1506b7
 https://conda.anaconda.org/conda-forge/win-64/libintl-0.22.5-h5728263_2.conda#aa622c938af057adc119f8b8eecada01
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.43-h19919ed_0.conda#77e398acc32617a0384553aea29e866b
 https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
 https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2#e1a22282de0169c93e4ffe6ce6acc212
-https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_1.conda#eb9f59dd51f50f5aa369813fa63ba569
+https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_2.conda#ac7af7a949db01dae61ddc48f4a93d79
 https://conda.anaconda.org/conda-forge/win-64/libzip-1.10.1-h1d365fa_3.conda#5c629cd12d89e2856c17b1dc5fcf44a4
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.43-h17e33f8_0.conda#d0485b8aa2cedb141a7bd27b4efa4c9c
 https://conda.anaconda.org/conda-forge/win-64/python-3.9.19-h4de0772_0_cpython.conda#b6999bc275e0e6beae7b1c8ea0be1e85
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda#792bb5da68bf0a6cac6a6072ecb8dbeb
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
@@ -60,70 +60,70 @@
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-hdaf720e_2.conda#3761b23693f768dc75a8fd0a73ca053f
 https://conda.anaconda.org/conda-forge/win-64/gettext-tools-0.22.5-h7d00a51_2.conda#ef1c3bb48c013099c4872640a5f2096c
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.5-py39h1f6ef14_1.conda#4fc5bd0a7b535252028c647cc27d6c87
 https://conda.anaconda.org/conda-forge/win-64/libclang13-18.1.3-default_hf64faad_0.conda#9217c37b478ec601af909aafc954a6fc
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.7.1-hd5e4a3a_0.conda#3396aff340d0903e8814c2852d631e4e
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-0.22.5-h5728263_2.conda#f4c826b19bf1ccee2a63a2c685039728
-https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_4.conda#9baf04fc7002450a932cf97cb9625ebb
-https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda#87da045f6d26ce9fe20ad76a18f6a18a
+https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_6.conda#cd5c6efbe213c089f78575c98ab9a0ed
+https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda#ee944f0d41d9e2048f9d7492c1623ca3
 https://conda.anaconda.org/conda-forge/win-64/libintl-devel-0.22.5-h5728263_2.conda#a2ad82fae23975e4ccbfab2847d31d48
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.6.0-hddb2be6_3.conda#6d1828c9039929e2f185c5fa9d133018
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.8-py39ha55989b_0.conda#07aae1fdd812b411cec84c0d47339d22
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py39ha55989b_0.conda#d8f52e8e1d02f9a5901f9224e2ddf98f
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.1.0-py39ha55989b_0.conda#20ec896e8d97f2ff8be1124e624dc8f2
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/win-64/brotli-1.1.0-hcfcfb64_1.conda#f47f6db2528e38321fb00ae31674c133
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda#3549ecbceb6cd77b91a105511b7d0786
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
-https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_4.conda#44cd44c004db728bf5788c1d46ce7334
+https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_6.conda#40d452e4012c00f644b1dd6319fcdbcf
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.14.3-nompi_h73e8ff5_100.conda#1e91ce0f3a914b0dab762539c0df4ff1
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.16-h67d730c_0.conda#d3592435917b62a8becff3a60db674f6
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-devel-0.22.5-h5728263_2.conda#6f42ec61abc6d52a4079800a640319c5
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.15-hcd874cb_0.conda#090d91b69396f14afef450c285f9758c
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda#7e7099ad94ac3b599808950cec30ad4e
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.18.6-py39ha55989b_0.conda#7839645d467f5d3bc52709a3d484fa62
 https://conda.anaconda.org/conda-forge/win-64/sip-6.7.12-py39h99910a6_0.conda#0cc5774390ada632ed7975203057c91c
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda#21069f3ed16812f9f4f2700667b6ec86
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda#21745fdd12f01b41178596143cbecffd
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/win-64/fonttools-4.51.0-py39ha55989b_0.conda#5d19302bab29e347116b743e793aa7d6
 https://conda.anaconda.org/conda-forge/win-64/gettext-0.22.5-h5728263_2.conda#da84216f88a8c89eb943c683ceb34d7d
-https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_4.conda#d0a05e8a76abb68b2beb7b16c6d49213
+https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_6.conda#a4036d0bc6f499ebe9fef7b887f3ca0f
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.9.2-nompi_h07c049d_113.conda#2aa431a5a05e3679eea4faad0f47b119
 https://conda.anaconda.org/conda-forge/win-64/mkl-2024.1.0-h66d3029_692.conda#b43ec7ed045323edeff31e348eea8652
 https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py39h9ee4981_0.conda#6d69d57c41867acc162ef0205a8efaef
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.12.2-py39h99910a6_5.conda#dffbcea794c524c471772a5f697c2aea
@@ -139,17 +139,17 @@
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-22_win64_mkl.conda#c752cc2af9f3d8d7b2fdebb915a33ef7
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.26.4-py39hddb5d58_0.conda#6e30ff8f2d3f59f45347dfba8bc22a04
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-hcef0176_21.conda#76544d3dfeff8fd52250df168cb0005b
 https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.3-py39hd88c2e4_0.conda#12e356a0e7e5a8e67538aa66fbd21c47
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.2.1-py39h1f6ef14_0.conda#03e25c6bae87f4f9595337255b44b0fb
-https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.1-py39h32e6231_0.conda#7ca03abc7f2f9c91a9fdc02780bfa572
+https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.2-py39h32e6231_0.conda#0df69e098aa54373d4edb3eaaa2338ba
 https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.9-py39hb77abff_5.conda#5ed899124a51958336371ff01482b8fd
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.13.0-py39hddb5d58_0.conda#cfe749056fb9ed9dbc096b5751becf34
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.8.4-py39hf19769e_0.conda#7836c3dc5814f6d55a7392657c576e88
 https://conda.anaconda.org/conda-forge/win-64/netcdf4-1.6.5-nompi_py39h9a3bb69_100.conda#e271773571fa2908d8fd598878890db2
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.8.4-py39hcbf5309_0.conda#cc66c372d5eb745665da06ce56b7d72b
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-optional-linux-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-optional-linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 5b0485937e0a03182e2f3b1a21f55c7ce045f3f148d46011fd73e55f316ee82e
+# input_hash: b5796a88d528d140fb4eaf550a1fec4d817f597ed69bbae3efbf21291ae56fc6
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda#2f4327a1cbe7f022401b236e915a5fef
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda#f6f6600d18a4047b54f803cf708b868a
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda#10569984e7db886e4f1abc2b47ad79a1
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda#3cfab3e709f77e9f1b3d380eb622494a
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.13-ha770c72_0.conda#9105ee57dc4869bc5d1876b531202676
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-4_cp39.conda#bfe4b3259a8ac6cdf0037752904da6a7
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda#aae89d3736661c36a5591788aebd0817
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda#df88796bd09a0d2ed292e59101478ad8
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.11-hd590300_1.conda#0bb492cca54017ea314b809b1ee3a176
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
 https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
 https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.2-hd590300_0.conda#3bf7b9fd5a7136126e0234db4b87c8b6
@@ -34,15 +34,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-h43f5ff8_6.conda#e54a5ddc67e673f9105cf2a2e9c070b0
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
@@ -72,37 +72,37 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.69-h0f662aa_0.conda#25cb5999faa414e5ccb2c1388f62d3d5
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_6.conda#3666a850342f8f3be88f9a93d948d027
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda#b3316cbe90249da4f8e84cd66e1cc55b
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_2.conda#9a3a42df8a95f65334dfc7b80da1195d
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
 https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.3.0-hf1915f5_4.conda#784a4df6676c581ca624fbe460703a6d
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h59595ed_1.conda#7fc9d3288d2420bb3637647621018000
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_6.conda#9342e7c44c38bea649490f72d92c382d
 https://conda.anaconda.org/conda-forge/linux-64/libllvm15-15.0.7-hb3ce162_4.conda#8a35df3cbc0c8b12cc8af9473ae75eef
 https://conda.anaconda.org/conda-forge/linux-64/libllvm18-18.1.3-h2448989_0.conda#927b6d6e80b2c0d4405a58b61ca248a3
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
 https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.3.0-hca2cd23_4.conda#1b50eebe2a738a3146c154d2eceaa8b6
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.98-h1d7d5a4_0.conda#54b56c2fdf973656b748e0378900ec13
 https://conda.anaconda.org/conda-forge/linux-64/python-3.9.19-h0755675_0_cpython.conda#d9ee3647fbd9e8595b8df759b2bbefb8
@@ -111,17 +111,18 @@
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.9-h8ee46fc_0.conda#077b6e8ad6a3ddb741fce2496dd01bec
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
-https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
+https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-h04ea711_2.conda#f730d54ba9cd543666d7220c9f7ed563
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.1.0-hd590300_1.conda#f27a24d46e3ea7b70a1f98e50c62508f
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py39h3d6467e_1.conda#c48418c8b35f1d59ae9ae1174812b40a
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
@@ -131,43 +132,42 @@
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py39h3d6467e_0.conda#d48142fba253b2a1074f8ddee84749cb
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py39hf3d152e_4.conda#0d71b15b6e77f2ae2ef81a478a384ead
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py39hf3d152e_5.conda#d74cf0b3351ffc48f1388424df827755
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_5.conda#8fdb82e5d9694dd8e9ed9ac8fdf48a26
-https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_4.conda#c9deba4959ea5b5f72f1e3e4a71ae014
+https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.11-hb9ae30d_0.conda#9bd27b5e21da16e40cf799bc2acf47d1
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_6.conda#a9d23c02485c5cf055f9ac90eb9c9c63
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
-https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda#53511e966e3ced065fbb1d3d5470d16d
 https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2#9800ad1699b42612478755a2d26c722d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/linux-64/jsonpointer-2.4-py39hf3d152e_3.conda#23255e64bc45e9bc0b7d87c108357ce6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py39h7633fee_1.conda#c9f74d717e5a2847a9f8b779c54130f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang-cpp15-15.0.7-default_h127d8a8_5.conda#d0a9633b53cdc319b8a1a532ae7822b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-18.1.3-default_h5d6823c_0.conda#5fff487759736b275dc3e4a263cac666
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h4637d8d_4.conda#d4529f4dff3057982a7617c7ac58fde3
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
-https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.48-h71f35ed_0.conda#4d18d86916705d352d5f4adfb7f0edd3
+https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.49-h4f305b6_0.conda#dfcfd72c7a430d3616763ecfbefe4ca9
 https://conda.anaconda.org/conda-forge/linux-64/libpq-16.2-h33b98f1_1.conda#9e49ec2a61d02623b379dc332eb6889d
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.3.2-h658648e_1.conda#0ebb65e8d86843865796c7c95a941f34
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py39hd1e30aa_0.conda#9a9a22eb1f83c44953319ee3b027769f
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.2-pyhd8ed1ab_0.conda#5cbee699846772cc939bef23a0d524ed
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda#d5c98e9706fdc5328d49a9bf2ce5fb42
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.7-py39h7633fee_0.conda#f668e146a2ed03a4e62ffbb98b3115fb
@@ -179,16 +179,16 @@
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.10.0-pyhd8ed1ab_0.conda#8c6a4a704308f5d91f3a974a72db1096
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py39hd1e30aa_0.conda#ec86403fde8793ac1c36f8afa3d15902
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
@@ -196,200 +196,206 @@
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py39hd1e30aa_1.conda#37218233bcdc310e4fde6453bc1b40d8
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py39h8c080ef_0.conda#852eb7bf636d4108530a27100c23f1c1
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.2-py39ha1047a2_0.conda#916ab2d35fbe7a2ad3ba03f96c78922d
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.18.0-py39h9fdd4d6_0.conda#ca1e1ff2be5c41142e412c83b88960e4
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py39hd1e30aa_0.conda#b1961e70cfe8e1eac243faf933d1813f
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh0d859eb_0.conda#778594b20097b5a948c59e50ae42482a
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2#62f26a3d1387acee31322208f0cfa3e0
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda#37c47ea93ef00dd80d880fc4ba21256a
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py39hd1e30aa_0.conda#1e865e9188204cdfb1fd2531780add88
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.1.0-py39hd1e30aa_0.conda#1da984bbb6e765743e13388ba7b7b2c8
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
+https://conda.anaconda.org/conda-forge/linux-64/websockets-12.0-py39hd1e30aa_0.conda#34476c3670224efb4000f20c8c42eb5b
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.41-hd590300_0.conda#81f740407b45e3f9047b3174fa94eb9e
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda#5f25798dcefd8252ce5f9dc494d5f571
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.4-pyhd8ed1ab_0.conda#3d081de3a6ea9f894bbb585e8e3a4dcb
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
+https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda#c747b1d79f136013c3b7ebcba876afa6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py39h7a31438_0.conda#ac992767d7f8ed2cb27e71e78f0fb2d7
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.4-pyhd8ed1ab_0.conda#7c2b6931f9b3548ed78478332095c3e9
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda#948d84721b578d426294e17a02e24cbb
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py39hd1e30aa_0.conda#79f5dd8778873faa54e8f7b2729fe8a6
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.11-pyhd8ed1ab_0.conda#623b19f616f2ca0c261441067e18ae40
-https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_4.conda#5521382ee30b96b35eb0037fc3c4f2b4
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_6.conda#a1e026a82a562b443845db5614ca568a
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2#b748fbf7060927a6e82df7cb5ee8f097
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda#5271aed7436e2145d405a53ba05610aa
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_1.conda#7b756504d362cbad9b73a50a5455cafd
 https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda#547670a612fd335eaa5ffbf0fa75cb64
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py39hf3d152e_0.conda#612f7a003a8a407955572c0d53952ceb
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.3-hd590300_0.conda#32d16ad533c59bb0a3c5ffaf16110829
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h119a65a_9.conda#cfebc557e54905dadc355c0e9f003004
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.2-hc60ed4a_1.conda#ef1910918dd895516a769ed36b5b3a4e
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.7.0-h662e7e4_0.conda#b32c0da42b1f24a98577bb3d7fc0b995
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda#629f3203c99b32e0988910c93e77f3b6
 https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py39h90c7501_0.conda#1e3b6af9592be71ce19f0a6aae05d97b
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py39hd1e30aa_0.conda#2289054e90cf07e35280bbe798811dc8
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.12-py39h3d6467e_0.conda#e667a3ab0df62c54e60e1843d2e6defb
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh0d859eb_0.conda#efba281bbdae5f6b0a1d53c6d4a97c93
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.18-pyhd8ed1ab_0.conda#bf61cfd2a7f212efba378167a07d4a6a
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.0-pyhd8ed1ab_0.conda#7d2bc38bd1777c86cc345e510735d9ff
 https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda#997c29372bdbe2afee073dff71f35923
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py39hd1e30aa_4.conda#6a04738e75f877b68552fc19cb045233
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/linux-64/cryptography-42.0.5-py39hd4f0224_0.conda#74adeac31d6368a9dcf1a867a052cffa
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.43-pyhd8ed1ab_0.conda#0b2154c1818111e17381b1df5b4b0176
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.24.1-h98fc4e7_1.conda#b04b5cdf3ba01430db27979250bc5a1d
-https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.4.0-h3d44ed6_0.conda#27f46291a6aaa3c2a4f798ebd35a7ddb
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
+https://conda.anaconda.org/conda-forge/noarch/jaraco.context-5.3.0-pyhd8ed1ab_1.conda#72d7ad2dcd0f37eccb2ee35a1c8f6aaa
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-255-h3516f8a_1.conda#3366af27f0b593544a6cd453c7932ac5
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py39h474f0d3_0.conda#aa265f5697237aa13cc10f53fa8acc4f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.16.3-py39h9fdd4d6_0.conda#35fef239167838ec05bc714a70fbd6d9
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.18.2-py39ha68c5e3_0.conda#25e4460e21b75d8371cc388860a11be9
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.12.2-py39h3d6467e_5.conda#93aff412f3e49fdb43361c0215cbd72d
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.1.1-pyhd8ed1ab_0.conda#52b91ecba854d55b28ad916a8b10da24
 https://conda.anaconda.org/conda-forge/noarch/python-build-1.2.1-pyhd8ed1ab_0.conda#d657cde3b3943fcedf6038138eea84de
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
+https://conda.anaconda.org/conda-forge/linux-64/uvicorn-0.29.0-py39hf3d152e_0.conda#0d7cbecfb218788337acd7737c8d7fd4
+https://conda.anaconda.org/conda-forge/linux-64/watchfiles-0.21.0-py39h9fdd4d6_0.conda#176ddbfc26cc9da781910e18d600bf86
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-23.1.0-pyhd8ed1ab_0.conda#3afef1f55a1366b4d3b6a0d92e2235e4
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.14.0-pyhd8ed1ab_0.conda#a661c39e223bf3038b38126b0bbf43d9
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py39h44dd56e_0.conda#baea2f5dfb3ab7b1c836385d2e1daca7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py39h7633fee_0.conda#bdc188e59857d6efab332714e0d01d93
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.4-pyhd8ed1ab_0.conda#e54a91c3a65491b13c68f7696425bac8
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.24.1-hfa15dee_1.conda#a6dd2bbc684913e2bef0a54ce56fcbfb
 https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda#9f359af5a886fd6ca6b2b6ea02e58332
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.18.1-pyh707e725_3.conda#15c6f45a45f7ac27f6d60b0b084f6761
 https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.1-py39hddac248_0.conda#85293a042c24a08e71b7608ee66b6134
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.2-py39hddac248_0.conda#259c4e76e6bda8888aefc098ae1ba749
 https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.2-ha41ecd1_0.conda#a658eeabf188c3040da36b0763de2bfd
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
 https://conda.anaconda.org/conda-forge/noarch/pip-tools-7.4.1-pyhd8ed1ab_0.conda#73203bd783da9c37c2cdabb1f3b9d44d
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-17.0-hb77b528_0.conda#07f45f1be1c25345faddb8db0de8039b
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.3-py39hf3d152e_1.conda#90a592a19a0de2536d9e63886a569715
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.6.4-pyhd8ed1ab_0.conda#2e8e9f16431085f4b5a218b31fe557a3
-https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.1.2-py39h44dd56e_0.conda#fbff274dc712b7d59f32f9b89bbc0151
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda#f5dac044e2aaccf73b85053f6db360b5
+https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.1.4-py39h44dd56e_0.conda#904ee2e5d137acfe238e6f0bcb46817d
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py39h474f0d3_0.conda#46ae0ecba9726ab4fa44c78fefa522cf
 https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py39hf3d152e_2.conda#0e6f3ef2dd562ed33d2a18d9c6f78d88
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/linux-64/astropy-6.0.1-py39h44dd56e_0.conda#8e41cc53247a1d21d53339c80b75f673
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.14.0-pyhd8ed1ab_0.conda#4c08fa6e7d1d3f124ad815e21b2210e9
 https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h280cfa0_4.conda#410f86e58e880dcc7b0e910a8e89c05c
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda#e0deff12c601ce5cb7476f93718f3168
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.2-pyhd8ed1ab_0.conda#67f86478c78637f68c1f3858973021f2
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.21.1-pyhd8ed1ab_0.conda#26bce4b5405738c09304d4f4796b2c2a
-https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda#db81e05a29ff5d52ca21b18bbf880520
-https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hce6bd6c_0.conda#0891de8980ee29828542dbf9578838b9
+https://conda.anaconda.org/conda-forge/noarch/keyring-25.2.0-pyha804496_0.conda#7a14341f0ed09e83e28b28140f058ae0
+https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hadf69e7_1.conda#0e2b5bd9533043b41f9482ae9e2c16b5
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py39he9076e7_0.conda#1919384a8420e7bb25f6c3a582e0857c
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda#0b57b5368ab7fc7cdc9e3511fa867214
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py39h4282601_100.conda#d2809fbf0d8ae7b8ca92c456cb44a7d4
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-hc9dc06e_21.conda#b325046180590c868ce0dbf267b82eb8
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/linux-64/statsmodels-0.14.1-py39h44dd56e_0.conda#dc565186b972bd87e49b9c35390ddd8c
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.6-pyhd8ed1ab_0.conda#16195242f8b17c9ca49f1ea34f1c027f
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.7-pyhd8ed1ab_0.conda#154d0c643be6a9ce6fbe655d007d8e4e
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-9.0.0-h78e8752_1.conda#a3f4cd4a512ec5db35ffbf25ba11f537
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.9-py39h52134e7_5.conda#e1f148e57d071b09187719df86f513c1
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.8.4-py39hf3d152e_0.conda#c66d2da2669fddc657b679bccab95775
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-optional-osx-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-optional-osx-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: b999a6c9f39c420db057dec65fd5d2e01109be13652ecd8ecbdc76d5c1efcf0f
+# input_hash: 2b84465b84cfa81790393537b9fe0a4ab921e6816915257b66c9da28c5c5b3f1
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda#6097a6ca9ada32699b5fc4312dd6ef18
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.28.1-h10d778d_0.conda#d5eb7992227254c0e9a0ce71151f0079
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda#f2eacee8c33c43692f1ccfd33d0f50b1
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
@@ -43,17 +43,17 @@
 https://conda.anaconda.org/conda-forge/osx-64/libasprintf-devel-0.22.5-h5ff76d1_2.conda#c7182eda3bc727384e2f98f4d680fa7d
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.1.0-h0dc2134_1.conda#9ee0bab91b2ca579e10353738be36063
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.1.0-h0dc2134_1.conda#8a421fe09c6187f0eb5e2338a8a8be6d
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-13.2.0-h2873a65_3.conda#e4fb4d23ec2870ff3c40d10afe305aec
 https://conda.anaconda.org/conda-forge/osx-64/libintl-0.22.5-h5ff76d1_2.conda#3fb6774cb8cdbb93a6013b67bcf9716d
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda#65dcddb15965c9de2c0365cb14910532
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda#086f56e13a96a6cfb1bf640505ae6b70
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda#68e462226209f35182ef66eda0f794ff
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda#bd85e0ca9e1ffaadc3b56079fd956035
+https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda#50b997370584f2c83ca0c38e9028eab9
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda#570a6f04802df580be529f3a72d2bbf7
 https://conda.anaconda.org/conda-forge/osx-64/pcre2-10.43-h0ad2156_0.conda#9c8651803886ce9d5983e107a0df4ea8
 https://conda.anaconda.org/conda-forge/osx-64/pixman-0.43.4-h73e2aa4_0.conda#cb134c1e03fd32f4e6bea3f6de2614fd
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.2.0-h6dc393e_1.conda#9c322ec36340610fcf213b72999b049e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda#bf830ba5afc507c6232d4ef0fb1a882d
@@ -64,29 +64,30 @@
 https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.1.0-h0dc2134_1.conda#ece565c215adcc47fc1db4e651ee094b
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h60636b9_2.conda#25152fce119320c980e5470e64834b50
 https://conda.anaconda.org/conda-forge/osx-64/gettext-tools-0.22.5-h5ff76d1_2.conda#37e1cb0efeff4d4623a6357e37e0105d
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.21.2-hb884880_0.conda#80505a68783f01dc8d7308c075261b2f
 https://conda.anaconda.org/conda-forge/osx-64/libgettextpo-0.22.5-h5ff76d1_2.conda#54cc9d12c29c2f0516f2ef4987de53ae
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-13_2_0_h97931a8_3.conda#0b6e23a012ee7a9a5f6b244f5a92c1d5
-https://conda.anaconda.org/conda-forge/osx-64/libglib-2.80.0-h81c1438_4.conda#eb94cd8fdcb676d17a5119189f87c4ae
+https://conda.anaconda.org/conda-forge/osx-64/libglib-2.80.0-h81c1438_6.conda#54dd1ed37dd65c5d13600bcc5ebbd0a1
 https://conda.anaconda.org/conda-forge/osx-64/libintl-devel-0.22.5-h5ff76d1_2.conda#ea0a07e556d6b238db685cae6e3585d0
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.58.0-h64cf6d3_1.conda#faecc55c2a8155d9ff1c0ff9a0fef64f
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.6.0-h129831d_3.conda#568593071d2e6cea7b5fc1f75bfa10ca
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.10.1-hc158999_3.conda#6112b3173f3aa2f12a8f40d07a77cc35
 https://conda.anaconda.org/conda-forge/osx-64/python-3.9.19-h7a9c478_0_cpython.conda#7d53d366acd9dbfb498c69326ccb520a
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda#cc4834a9ee7cc49ce8d25177c47b10d8
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
-https://conda.anaconda.org/conda-forge/osx-64/atk-1.0-2.38.0-h1d18e73_1.tar.bz2#5a538295f97a484ee332aacc131718b5
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
+https://conda.anaconda.org/conda-forge/osx-64/atk-1.0-2.38.0-h4bec284_2.conda#d9684247c943d492d9aac8687bc5db77
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/osx-64/brotli-1.1.0-h0dc2134_1.conda#9272dd3b19c4e8212f8542cefd5c3d67
 https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.1.0-py39h840bb9f_1.conda#bf1edb07835e15685718843f7e71bab1
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
@@ -95,30 +96,29 @@
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py39hd253f6c_0.conda#328dc0de8a70c8f8de65d37a6b289220
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py39h6e9494a_4.conda#2075bada3661d0a7fb762b4f84f7c06a
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py39h6e9494a_5.conda#7738300100023129d58567edc49ee90b
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/osx-64/fontconfig-2.14.2-h5bb23bf_0.conda#86cc5867dfbee4178118392bae4a3c89
-https://conda.anaconda.org/conda-forge/osx-64/gdk-pixbuf-2.42.10-hd9e0ca3_5.conda#308cefd960b6ba51bdbdc5ba9e9b2377
+https://conda.anaconda.org/conda-forge/osx-64/gdk-pixbuf-2.42.11-ha9f1606_0.conda#ab407c96c658772c9bcd7161931fd933
 https://conda.anaconda.org/conda-forge/osx-64/gts-0.7.6-h53e17e3_4.conda#848cc963fcfbd063c7a023024aa3bec0
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
-https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda#53511e966e3ced065fbb1d3d5470d16d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/osx-64/jsonpointer-2.4-py39h6e9494a_3.conda#7712a5f0d4f3f7d9ec69fb24dcf9bf0a
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.5-py39h8ee36c8_1.conda#6072db04642b21329b0502a177ec18bf
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.16-ha2f27b4_0.conda#1442db8f03517834843666c422238c9b
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.7.1-h726d00d_0.conda#fa58e5eaa12006bc3289a71357bef167
 https://conda.anaconda.org/conda-forge/osx-64/libgettextpo-devel-0.22.5-h5ff76d1_2.conda#1e0384c52cd8b54812912e7234e66056
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.27-openmp_hfef2a42_0.conda#00237c9c7f2cb6725fe2960680a6e225
@@ -136,64 +136,66 @@
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.10.0-pyhd8ed1ab_0.conda#8c6a4a704308f5d91f3a974a72db1096
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py39ha09f3b3_0.conda#e8737c3c0c404559b0e2c8a9eb91e977
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py39hdc70f33_1.conda#542378f49240a94056b50ab1385b3bfb
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py39hcb7a90d_0.conda#39754a321b3dece3df9a0eb213d43dc8
+https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.2-py39hffc4518_0.conda#13c761db6b475447b63702e5f7ee3015
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.18.0-py39hcf47035_0.conda#0e8641e9f0d42d844cf17f5520225e6e
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.8-py39ha09f3b3_0.conda#835c656934865805c0b02dbff74fe5b7
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2#62f26a3d1387acee31322208f0cfa3e0
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda#37c47ea93ef00dd80d880fc4ba21256a
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py39ha09f3b3_0.conda#4541517b5a605bf45d4a5fb074bb4cf5
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.1.0-py39hdc70f33_0.conda#ede122e9ef2775a8879063d9d3ee819f
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
+https://conda.anaconda.org/conda-forge/osx-64/websockets-12.0-py39ha09f3b3_0.conda#14a37a956881ee2df098931d2c8b40c9
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda#5f25798dcefd8252ce5f9dc494d5f571
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.4-pyhd8ed1ab_0.conda#3d081de3a6ea9f894bbb585e8e3a4dcb
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
+https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda#c747b1d79f136013c3b7ebcba876afa6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/osx-64/cairo-1.18.0-h99e66fa_0.conda#13f830b1bf46018f7062d1b798d53eca
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py39h18ef598_0.conda#c31ac48f93f773fd27e99f113cfffb98
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.4-pyhd8ed1ab_0.conda#7c2b6931f9b3548ed78478332095c3e9
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
@@ -204,133 +206,137 @@
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.11-pyhd8ed1ab_0.conda#623b19f616f2ca0c261441067e18ae40
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2#b748fbf7060927a6e82df7cb5ee8f097
 https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.3-nompi_h691f4bf_100.conda#8e2ac4ae815a8c9743fe37d70f48f075
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda#5271aed7436e2145d405a53ba05610aa
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_1.conda#7b756504d362cbad9b73a50a5455cafd
 https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda#547670a612fd335eaa5ffbf0fa75cb64
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.1-py39h6e9494a_0.conda#9611b1806866adc1693cfb5a323f16e4
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-22_osx64_openblas.conda#b80966a8c8dd0b531f8e65f709d732e8
 https://conda.anaconda.org/conda-forge/osx-64/libgd-2.3.3-h0dceb68_9.conda#1feb43971521d430bf826f8398598c5b
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda#629f3203c99b32e0988910c93e77f3b6
 https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py39h9dabb2a_0.conda#e385068c9511542eff20422f7e799064
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-10.2-py39h8602b6b_0.conda#37b6b21536780b9665b9c84908318d7a
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.18.6-py39ha09f3b3_0.conda#6eb863d10b7aeef1f58ba1ebf92f59bd
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh31c8845_0.conda#00b54981b923f5aefcd5e8547de056d5
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.18-pyhd8ed1ab_0.conda#bf61cfd2a7f212efba378167a07d4a6a
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.0-pyhd8ed1ab_0.conda#7d2bc38bd1777c86cc345e510735d9ff
 https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda#997c29372bdbe2afee073dff71f35923
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py39hdc70f33_4.conda#3a0f682e6fdf53ff630c22cdd90ac0c1
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.43-pyhd8ed1ab_0.conda#0b2154c1818111e17381b1df5b4b0176
-https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-8.3.0-hf45c392_0.conda#41d890485f909e4ecdc608741718c75e
+https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-8.4.0-h72fa137_0.conda#7d065a2266ae5eb2a5d91a6dca4fca69
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
+https://conda.anaconda.org/conda-forge/noarch/jaraco.context-5.3.0-pyhd8ed1ab_1.conda#72d7ad2dcd0f37eccb2ee35a1c8f6aaa
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-22_osx64_openblas.conda#b9fef82772330f61b2b0201c72d2c29b
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-22_osx64_openblas.conda#f21b282ff7ba14df6134a0fe6ab42b1b
 https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_h7760872_113.conda#bce76ace6497221c2a2a02840aaceac5
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.16.3-py39hcf47035_0.conda#ca2dc68c950341730cd6140a0d141cf1
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.18.2-py39h3013830_0.conda#1509b51dadc688c5a71771483d195d52
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-10.2-py39h8602b6b_0.conda#271f368ad661bf3bba2d5740ac8ee24c
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.1.1-pyhd8ed1ab_0.conda#52b91ecba854d55b28ad916a8b10da24
 https://conda.anaconda.org/conda-forge/noarch/python-build-1.2.1-pyhd8ed1ab_0.conda#d657cde3b3943fcedf6038138eea84de
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
+https://conda.anaconda.org/conda-forge/osx-64/uvicorn-0.29.0-py39h6e9494a_0.conda#79786774d034370e5e7bf2707b7613d5
+https://conda.anaconda.org/conda-forge/osx-64/watchfiles-0.21.0-py39h3f9c672_0.conda#9c6ce8f29c4c66782417b26bb4a7d5dd
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-23.1.0-pyhd8ed1ab_0.conda#3afef1f55a1366b4d3b6a0d92e2235e4
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.14.0-pyhd8ed1ab_0.conda#a661c39e223bf3038b38126b0bbf43d9
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.4-pyhd8ed1ab_0.conda#e54a91c3a65491b13c68f7696425bac8
 https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda#9f359af5a886fd6ca6b2b6ea02e58332
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.18.1-pyh707e725_3.conda#15c6f45a45f7ac27f6d60b0b084f6761
 https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
-https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh534df25_0.conda#537a5385c6cee5fa2275a457e0b51b21
+https://conda.anaconda.org/conda-forge/noarch/keyring-25.2.0-pyh534df25_0.conda#acaf59f096327bc5757c91303cae99ca
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.26.4-py39h28c39a1_0.conda#1b07000dc6aed4a69e91107dac4464d3
 https://conda.anaconda.org/conda-forge/osx-64/pango-1.52.2-h7f2093b_0.conda#ea9611aee7e61e4ff18c4dc56ec100ab
 https://conda.anaconda.org/conda-forge/noarch/pip-tools-7.4.1-pyhd8ed1ab_0.conda#73203bd783da9c37c2cdabb1f3b9d44d
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.3-py39h6e9494a_1.conda#450b8f37439740c0e79acbeba7d1d678
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.6.4-pyhd8ed1ab_0.conda#2e8e9f16431085f4b5a218b31fe557a3
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda#f5dac044e2aaccf73b85053f6db360b5
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh31c8845_0.conda#c3cb67fc72fb38020fe7923dbbcf69b0
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.14.0-pyhd8ed1ab_0.conda#4c08fa6e7d1d3f124ad815e21b2210e9
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.3-py39h5b4affa_0.conda#20fd617b1f9fcefe5ec1577d38ae7bdb
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.2.1-py39h0ca7971_0.conda#a4c478d3b64c81d1742dc8073e4996b6
 https://conda.anaconda.org/conda-forge/osx-64/gtk2-2.24.33-h8ca4665_4.conda#ff451625250bf843393ca3d660accab3
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda#28e74fca8d8abf09c1ed0d190a17e307
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.2-pyhd8ed1ab_0.conda#67f86478c78637f68c1f3858973021f2
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.21.1-pyhd8ed1ab_0.conda#26bce4b5405738c09304d4f4796b2c2a
-https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.58.0-h7b06fc5_0.conda#3ad98f9e1ad2b0c9b202b9d5212752d2
+https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.58.0-h7b06fc5_1.conda#e4a5f1bb5962ec6f2f2d2f0467ed0826
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda#0b57b5368ab7fc7cdc9e3511fa867214
-https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.1-py39haf03413_0.conda#d29dc35b665029951dae988810f84508
+https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.2-py39haf03413_0.conda#11225cf1f769af217ffc01f0a21d40fa
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
-https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.1.2-py39h5b4affa_0.conda#d1167fcafcd783b8b3835ec7cf6931c7
+https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.1.4-py39h5b4affa_0.conda#6743589ba4d7d219c4e2790d4c1d4b13
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.13.0-py39h0ed1e0f_0.conda#3a4d0af4fe2006bedc33ca61e9a0b4d6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/osx-64/astropy-6.0.1-py39h5b4affa_0.conda#f883a58c4337d0a6f0996a533aae15f0
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.6-pyhd8ed1ab_0.conda#16195242f8b17c9ca49f1ea34f1c027f
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.7-pyhd8ed1ab_0.conda#154d0c643be6a9ce6fbe655d007d8e4e
 https://conda.anaconda.org/conda-forge/osx-64/graphviz-9.0.0-hee74176_1.conda#7cd479251093c332aa9fe93cfb8f698b
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.8.4-py39h7070ae8_0.conda#cb9e1f8aff1f759b9685e908f9dc0a5b
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.5-nompi_py39h824b2b2_100.conda#07525171115894fe9c4aba755460c51a
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/osx-64/statsmodels-0.14.1-py39h5b4affa_0.conda#4cc025969fa47342955213653d1352c8
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.8.4-py39h6e9494a_0.conda#371fe0f738d9f3baa20cf06656b78b0a
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-optional-win-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-optional-win-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: 9ad718ef7b5a9fbf088fa23ac9c09be94a00a86afe4fb2986ea855c6b8b67d03
+# input_hash: 2c6414ffedc11afaa29ea902e4debab1ee1854a776195e8394589b994c279ef5
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda#63da060240ab8087b60d1357051ea7d6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda#30ebb9fd99666d8b8675fcee541a09f3
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda#c66eb2fd33b999ccc258aef85689758e
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-0.22.5-h5728263_2.conda#75a6982b9ff0a8db0f53303527b07af8
 https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda#bc592d03f62779511d392c175dcece64
 https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2#b0309b72560df66f71a9d5e34a5efdfa
 https://conda.anaconda.org/conda-forge/win-64/pandoc-3.1.13-h57928b3_0.conda#4caaf4c37a0efc8a06492dba2d871bbb
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.9-4_cp39.conda#948b0d93d4ab1372d8fd45e1560afd47
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
@@ -36,15 +36,15 @@
 https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.1.0-hcfcfb64_1.conda#f77f319fb82980166569e1280d5b2864
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.20-hcfcfb64_0.conda#b12b5bde5eb201a1df75e49320cc938a
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda#e1eb10b1cca179f2baa3601e4efc8712
 https://conda.anaconda.org/conda-forge/win-64/libjpeg-turbo-3.0.0-hcfcfb64_1.conda#3f1b948619c45b1ca714d60c7389092c
 https://conda.anaconda.org/conda-forge/win-64/libogg-1.3.4-h8ffe710_1.tar.bz2#04286d905a0dcb7f7d4a12bdfe02516d
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda#f95359f8dc5abf7da7776ece9ef10bc5
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda#73f5dc8e2d55d9a1e14b11f49c3b4a28
 https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.2-hcfcfb64_1.conda#fdf80cb33c32d4d002bb89c37cfff5b7
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda#958e0418e93e50c575bff70fbcaa12d8
 https://conda.anaconda.org/conda-forge/win-64/pixman-0.43.4-h63175ca_0.conda#b98135614135d5f458b75ab9ebb9558c
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
@@ -57,28 +57,29 @@
 https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.1.0-hcfcfb64_1.conda#19ce3e1dacc7912b3d6ff40690ba9ae0
 https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.1.0-hcfcfb64_1.conda#71e890a0b361fd58743a13f77e1506b7
 https://conda.anaconda.org/conda-forge/win-64/libintl-0.22.5-h5728263_2.conda#aa622c938af057adc119f8b8eecada01
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.43-h19919ed_0.conda#77e398acc32617a0384553aea29e866b
 https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
 https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2#e1a22282de0169c93e4ffe6ce6acc212
 https://conda.anaconda.org/conda-forge/win-64/libwebp-1.3.2-hcfcfb64_1.conda#6202a1ba6be2713084cf0452d4e8c10c
-https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_1.conda#eb9f59dd51f50f5aa369813fa63ba569
+https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_2.conda#ac7af7a949db01dae61ddc48f4a93d79
 https://conda.anaconda.org/conda-forge/win-64/libzip-1.10.1-h1d365fa_3.conda#5c629cd12d89e2856c17b1dc5fcf44a4
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.43-h17e33f8_0.conda#d0485b8aa2cedb141a7bd27b4efa4c9c
 https://conda.anaconda.org/conda-forge/win-64/python-3.9.19-h4de0772_0_cpython.conda#b6999bc275e0e6beae7b1c8ea0be1e85
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-h63175ca_1.conda#e8867cc4d023f41f54bd64a33436b0a1
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda#792bb5da68bf0a6cac6a6072ecb8dbeb
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.16-pyhd8ed1ab_0.conda#def531a3ac77b7fb8c21d17bb5d0badb
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/win-64/blosc-1.21.5-hbd69f2e_1.conda#06c7d9a1cdecef43921be8b577a61ee7
 https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.1.0-hcfcfb64_1.conda#0105229d7c5fabaa840043a86c10ec64
 https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.1.0-py39h99910a6_1.conda#f24ba3942ece1e5d3dcde934f0532998
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.3-pyhd8ed1ab_0.conda#cd4c26c702a9bcdc70ff05b609ddacbe
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
@@ -87,37 +88,36 @@
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py39h99910a6_0.conda#412a0fe4d63fab41a73776839a5856db
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda#db16c66b759a64dc5183d69cc3745a52
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py39hcbf5309_4.conda#adae8d63d214069960445c1aba41eea5
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py39hcbf5309_5.conda#461b44faa5dd942c6be4405a8df37587
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda#6baa2e7fc09bd2c7c82cb6662d5f1d36
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-hdaf720e_2.conda#3761b23693f768dc75a8fd0a73ca053f
 https://conda.anaconda.org/conda-forge/win-64/gettext-tools-0.22.5-h7d00a51_2.conda#ef1c3bb48c013099c4872640a5f2096c
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
-https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda#53511e966e3ced065fbb1d3d5470d16d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/win-64/jsonpointer-2.4-py39hcbf5309_3.conda#e066b7eb0c8669f0549aaf6aef50f880
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.5-py39h1f6ef14_1.conda#4fc5bd0a7b535252028c647cc27d6c87
 https://conda.anaconda.org/conda-forge/win-64/libclang13-18.1.3-default_hf64faad_0.conda#9217c37b478ec601af909aafc954a6fc
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.7.1-hd5e4a3a_0.conda#3396aff340d0903e8814c2852d631e4e
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-0.22.5-h5728263_2.conda#f4c826b19bf1ccee2a63a2c685039728
-https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_4.conda#9baf04fc7002450a932cf97cb9625ebb
-https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda#87da045f6d26ce9fe20ad76a18f6a18a
+https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_6.conda#cd5c6efbe213c089f78575c98ab9a0ed
+https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda#ee944f0d41d9e2048f9d7492c1623ca3
 https://conda.anaconda.org/conda-forge/win-64/libintl-devel-0.22.5-h5728263_2.conda#a2ad82fae23975e4ccbfab2847d31d48
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.6.0-hddb2be6_3.conda#6d1828c9039929e2f185c5fa9d133018
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py39ha55989b_0.conda#f8b7e33c8bf98901925817b7f4436c7e
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.2-pyhd8ed1ab_0.conda#5cbee699846772cc939bef23a0d524ed
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda#d5c98e9706fdc5328d49a9bf2ce5fb42
 https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.7-py39h1f6ef14_0.conda#74e894b9e9ef693559594bdb472da770
@@ -128,16 +128,16 @@
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.10.0-pyhd8ed1ab_0.conda#8c6a4a704308f5d91f3a974a72db1096
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py39ha55989b_0.conda#59cff26058f788059a310208dde2e01d
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
@@ -147,152 +147,158 @@
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py39h99910a6_2.conda#eab91442160b49994dd2e224e6082770
 https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py39hcbf5309_1.conda#b81928cd8f6e5faf318ad6ddf8b0c7a5
 https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.13-py39h99910a6_0.conda#6dc677d08286a639b3c064a7a4376e06
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py39ha55989b_1.conda#5c3a9da77fc79c21c5c1fd7ea06306a2
-https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py39h7eaf5a6_0.conda#113b93bd971d355b1d52df09c1161628
+https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.2-py39h03e5c00_0.conda#5e1e67cb1d03a2cce828bac7aa6642a5
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.18.0-py39hf21820d_0.conda#32fa6863c2216dbe787adaf874433713
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.8-py39ha55989b_0.conda#07aae1fdd812b411cec84c0d47339d22
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2#62f26a3d1387acee31322208f0cfa3e0
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0.conda#da1d979339e2714c30a8e806a33ec087
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda#37c47ea93ef00dd80d880fc4ba21256a
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda#2fcb582444635e2c402e8569bb94e039
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py39ha55989b_0.conda#d8f52e8e1d02f9a5901f9224e2ddf98f
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.1.0-py39ha55989b_0.conda#20ec896e8d97f2ff8be1124e624dc8f2
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
+https://conda.anaconda.org/conda-forge/win-64/websockets-12.0-py39ha55989b_0.conda#24b1cf33f77a58400a2098e0cdc04e8f
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda#0b5293a157c2b5cd513dd1b03d8d3aae
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/xorg-kbproto-1.0.7-hcd874cb_1002.tar.bz2#8d11c1dac4756ca57e78c1bfe173bba4
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
 https://conda.anaconda.org/conda-forge/win-64/xorg-xextproto-7.3.0-hcd874cb_1003.conda#6e6c2639620e436bddb7c040cd4f3adb
 https://conda.anaconda.org/conda-forge/win-64/xorg-xproto-7.0.31-hcd874cb_1007.tar.bz2#88f3c65d2ad13826a9e0b162063be023
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda#5f25798dcefd8252ce5f9dc494d5f571
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.4-pyhd8ed1ab_0.conda#3d081de3a6ea9f894bbb585e8e3a4dcb
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
+https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda#c747b1d79f136013c3b7ebcba876afa6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.1.0-pyhd8ed1ab_0.conda#0ed9d7c0e9afa7c025807a9a8136ea3e
 https://conda.anaconda.org/conda-forge/win-64/brotli-1.1.0-hcfcfb64_1.conda#f47f6db2528e38321fb00ae31674c133
 https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py39ha55989b_0.conda#3641cc4492220301e0b0c65cf2985a80
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda#3549ecbceb6cd77b91a105511b7d0786
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda#948d84721b578d426294e17a02e24cbb
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/win-64/fontconfig-2.14.2-hbde0cde_0.conda#08767992f1a4f1336a257af1241034bd
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.11-pyhd8ed1ab_0.conda#623b19f616f2ca0c261441067e18ae40
-https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_4.conda#44cd44c004db728bf5788c1d46ce7334
+https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_6.conda#40d452e4012c00f644b1dd6319fcdbcf
 https://conda.anaconda.org/conda-forge/win-64/gts-0.7.6-h6b5321d_4.conda#a41f14768d5e377426ad60c613f2923b
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2#b748fbf7060927a6e82df7cb5ee8f097
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.14.3-nompi_h73e8ff5_100.conda#1e91ce0f3a914b0dab762539c0df4ff1
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda#5271aed7436e2145d405a53ba05610aa
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_1.conda#7b756504d362cbad9b73a50a5455cafd
 https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda#547670a612fd335eaa5ffbf0fa75cb64
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py39hcbf5309_0.conda#78ec20214b67efe5caebb4f08bdee094
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.16-h67d730c_0.conda#d3592435917b62a8becff3a60db674f6
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-devel-0.22.5-h5728263_2.conda#6f42ec61abc6d52a4079800a640319c5
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.15-hcd874cb_0.conda#090d91b69396f14afef450c285f9758c
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda#7e7099ad94ac3b599808950cec30ad4e
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda#f586ac1e56c8638b64f9c8122a7b8a67
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.18.6-py39ha55989b_0.conda#7839645d467f5d3bc52709a3d484fa62
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh5737063_0.conda#5a86a21050ca3831ec7f77fb302f1132
 https://conda.anaconda.org/conda-forge/win-64/sip-6.7.12-py39h99910a6_0.conda#0cc5774390ada632ed7975203057c91c
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda#21069f3ed16812f9f4f2700667b6ec86
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda#21745fdd12f01b41178596143cbecffd
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh5737063_0.conda#4abd500577430a942a995fd0d09b76a2
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda#8797a4e26be36880a603aba29c785352
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.0-pyhd8ed1ab_0.conda#7d2bc38bd1777c86cc345e510735d9ff
 https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda#997c29372bdbe2afee073dff71f35923
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py39ha55989b_4.conda#40f25bc759e1ea863a6e468380cd2363
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/win-64/cairo-1.18.0-h1fef639_0.conda#b3fe2c6381ec74afe8128e16a11eee02
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.4-pyhd8ed1ab_0.conda#7c2b6931f9b3548ed78478332095c3e9
 https://conda.anaconda.org/conda-forge/win-64/fonttools-4.51.0-py39ha55989b_0.conda#5d19302bab29e347116b743e793aa7d6
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/win-64/gettext-0.22.5-h5728263_2.conda#da84216f88a8c89eb943c683ceb34d7d
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.43-pyhd8ed1ab_0.conda#0b2154c1818111e17381b1df5b4b0176
-https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_4.conda#d0a05e8a76abb68b2beb7b16c6d49213
+https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_6.conda#a4036d0bc6f499ebe9fef7b887f3ca0f
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
+https://conda.anaconda.org/conda-forge/noarch/jaraco.context-5.3.0-pyhd8ed1ab_1.conda#72d7ad2dcd0f37eccb2ee35a1c8f6aaa
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.9.2-nompi_h07c049d_113.conda#2aa431a5a05e3679eea4faad0f47b119
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/win-64/mkl-2024.1.0-h66d3029_692.conda#b43ec7ed045323edeff31e348eea8652
 https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py39h9ee4981_0.conda#6d69d57c41867acc162ef0205a8efaef
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.16.3-py39hf21820d_0.conda#2c10071c595fa4c2f021f51f0852c37b
+https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.18.2-py39h92a245a_0.conda#5d16ca48eb70a12b953439c03c7e4513
 https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.12.2-py39h99910a6_5.conda#dffbcea794c524c471772a5f697c2aea
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.1.1-pyhd8ed1ab_0.conda#52b91ecba854d55b28ad916a8b10da24
 https://conda.anaconda.org/conda-forge/noarch/python-build-1.2.1-pyhd8ed1ab_0.conda#d657cde3b3943fcedf6038138eea84de
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/starlette-0.37.2-pyhd8ed1ab_0.conda#7e5550dfa3ed2c2019988cbb9f8302ea
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.18-pyhd8ed1ab_0.conda#bf61cfd2a7f212efba378167a07d4a6a
+https://conda.anaconda.org/conda-forge/win-64/uvicorn-0.29.0-py39hcbf5309_0.conda#75e90ff63b09f4443258dd7829bb6032
+https://conda.anaconda.org/conda-forge/win-64/watchfiles-0.21.0-py39hf21820d_0.conda#5409cf692b0dec68648e6e8a6721e5ee
 https://conda.anaconda.org/conda-forge/win-64/xorg-libx11-1.8.9-hefa74cf_0.conda#3672e991346895f332af1ebc60b8bca9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-23.1.0-pyhd8ed1ab_0.conda#3afef1f55a1366b4d3b6a0d92e2235e4
 https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.24.1-hb4038d2_1.conda#8a6dfe53ad02a3b151e6383a950043ee
-https://conda.anaconda.org/conda-forge/win-64/harfbuzz-8.3.0-h7ab893a_0.conda#b8ef0beb91df83c5e6038c9509b9f730
+https://conda.anaconda.org/conda-forge/win-64/harfbuzz-8.4.0-h7ab893a_0.conda#bf9b853f9702724a5ec4e68dc637cc29
 https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda#9f359af5a886fd6ca6b2b6ea02e58332
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.18.1-pyh7428d3b_3.conda#656a798e52fbe1ca72f7d97b3c36aeff
 https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
-https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh7428d3b_0.conda#993d4eaf46a94e1ba4d1a15fbed07953
+https://conda.anaconda.org/conda-forge/noarch/keyring-25.2.0-pyh7428d3b_0.conda#33f009280144917e907939141af7cf7c
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-22_win64_mkl.conda#65c56ecdeceffd6c32d3d54db7e02c6e
 https://conda.anaconda.org/conda-forge/noarch/pip-tools-7.4.1-pyhd8ed1ab_0.conda#73203bd783da9c37c2cdabb1f3b9d44d
 https://conda.anaconda.org/conda-forge/win-64/pybtex-docutils-1.0.3-py39hcbf5309_1.conda#0131fba9b943b68a01e2ac623004c48f
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.6.4-pyhd8ed1ab_0.conda#2e8e9f16431085f4b5a218b31fe557a3
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda#f5dac044e2aaccf73b85053f6db360b5
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libice-1.1.1-hcd874cb_0.conda#5271e3af4791170e2c55d02818366916
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxext-1.3.4-hcd874cb_2.conda#2aa695ac3c56193fd8d526e3b511e021
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.14.0-pyhd8ed1ab_0.conda#a661c39e223bf3038b38126b0bbf43d9
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.4-pyhd8ed1ab_0.conda#e54a91c3a65491b13c68f7696425bac8
@@ -310,49 +316,49 @@
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.14.0-pyhd8ed1ab_0.conda#4c08fa6e7d1d3f124ad815e21b2210e9
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.26.4-py39hddb5d58_0.conda#6e30ff8f2d3f59f45347dfba8bc22a04
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-hcef0176_21.conda#76544d3dfeff8fd52250df168cb0005b
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxt-1.3.0-hcd874cb_1.conda#511a29edd2ff3d973f63e54f19dcc06e
 https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.3-py39hd88c2e4_0.conda#12e356a0e7e5a8e67538aa66fbd21c47
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.6-pyhd8ed1ab_0.conda#16195242f8b17c9ca49f1ea34f1c027f
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.5.7-pyhd8ed1ab_0.conda#154d0c643be6a9ce6fbe655d007d8e4e
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.2.1-py39h1f6ef14_0.conda#03e25c6bae87f4f9595337255b44b0fb
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
-https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.1-py39h32e6231_0.conda#7ca03abc7f2f9c91a9fdc02780bfa572
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
+https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.2-py39h32e6231_0.conda#0df69e098aa54373d4edb3eaaa2338ba
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
-https://conda.anaconda.org/conda-forge/win-64/pyerfa-2.0.1.2-py39hd88c2e4_0.conda#b252cec19b9dfb27ce61ea3ebf90717a
+https://conda.anaconda.org/conda-forge/win-64/pyerfa-2.0.1.4-py39hd88c2e4_0.conda#173997708f936f15e527756c01e2b744
 https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.9-py39hb77abff_5.conda#5ed899124a51958336371ff01482b8fd
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.13.0-py39hddb5d58_0.conda#cfe749056fb9ed9dbc096b5751becf34
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxpm-3.5.17-hcd874cb_0.conda#029be9b667bf3896fa28bc32adb1bfc3
 https://conda.anaconda.org/conda-forge/win-64/astropy-6.0.1-py39hd88c2e4_0.conda#efb93481436d459f13e041b2572d584c
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
 https://conda.anaconda.org/conda-forge/win-64/libgd-2.3.3-h312136b_9.conda#69c987e1f9268d9ade86497c4ab8cc45
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.8.4-py39hf19769e_0.conda#7836c3dc5814f6d55a7392657c576e88
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_0.conda#1344bbd74e8bcd1acdd8ec0824e9840c
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.16.3-hd8ed1ab_1.conda#105151637d2223d6274c5c79d839cc64
 https://conda.anaconda.org/conda-forge/win-64/netcdf4-1.6.5-nompi_py39h9a3bb69_100.conda#e271773571fa2908d8fd598878890db2
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/win-64/statsmodels-0.14.1-py39hd88c2e4_0.conda#b51565db0ed851e9031da82171d0e02f
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/win-64/graphviz-9.0.0-h51cb2cd_1.conda#9e73e70557ae3c1c9d4bdf70f47dd141
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.8.4-py39hcbf5309_0.conda#cc66c372d5eb745665da06ce56b7d72b
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_0.conda#b0c9bbbe54a11a6db3bec51eb0ef0281
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.16.3-hd8ed1ab_1.conda#c80cd9bcb93679ceb9ea0938cf5f7db0
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.12-pyhd8ed1ab_0.conda#b0e58323e15cb50328a1bb3e8158a49c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
 https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.3-pyhd8ed1ab_0.conda#0dbaa7d08d3d79b2a1a4dd6a02cc4581
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.15.2-pyhd8ed1ab_0.conda#ce99859070b0e17ccc63234ca58f3ed8
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.2.4-pyhd8ed1ab_0.conda#13996799cc0b00919a3c1b9b02e02217
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2024.4.16-pyhd8ed1ab_0.conda#108af3d0ad050d1efd1c48be5852c42b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.1.2-pyhd8ed1ab_0.conda#fa675936fa91d74cc2a45fbc8df1598b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.5.0-pyhd8ed1ab_0.conda#264b3c697fa9cdade87eb0abe4440d54
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0.conda#611a35a27914fac3aa37611a6fe40bb5
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.6.2-pyhd8ed1ab_0.conda#ac0947374ec8b703181808828bf5dfec
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0.conda#d7e4954df0d3aea2eacc7835ad12671d
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0.conda#7e1e7437273682ada2ed5e9e9714b140
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-optional.yml` & `eradiate-0.27.0rc1/requirements/conda/environment-dev.yml`

 * *Files 13% similar despite different names*

```diff
@@ -11,28 +11,28 @@
   - pip-tools>=6.5
   - pip>=22
   - setuptools>=61
   # docs
   - autodocsumm
   - myst-parser
   - nbsphinx>=0.9.0
+  - seaborn
   - sphinx
   - sphinx-autobuild
   - sphinx-book-theme>=1.0
   - sphinx-copybutton
   - sphinx-design
   - sphinxcontrib-bibtex>=2.0
   # main
   - aenum
   - attrs>=22.2
   - cachetools>=5.3
   - click
   - dessinemoi>=23.1.0
   - dynaconf>=3.2
-  - importlib_resources
   - joseki>=2.6.0
   - lazy_loader>=0.1
   - matplotlib>=3.3
   - netcdf4
   - numpy
   - pint
   - pinttrs>=23.2.0
@@ -41,20 +41,18 @@
   - ruamel.yaml
   - scipy
   - sf-hamilton>=1.40
   - shellingham!=1.5.1
   - tqdm
   - typer>=0.9.0
   - xarray>=0.19,!=0.20.*
-  # optional
   # recommended
   - aabbtree
   - astropy
   - ipython
   - ipywidgets
   - jupyterlab
   - python-dateutil
   - python-graphviz
-  - seaborn
   # tests
   - pytest
   - pytest-json-report
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-recommended-linux-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-recommended-linux-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,34 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda#2f4327a1cbe7f022401b236e915a5fef
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda#f6f6600d18a4047b54f803cf708b868a
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda#10569984e7db886e4f1abc2b47ad79a1
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda#3cfab3e709f77e9f1b3d380eb622494a
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda#dccc2d142812964fcc6abdc97b672dff
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda#aae89d3736661c36a5591788aebd0817
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda#df88796bd09a0d2ed292e59101478ad8
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
-https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
 https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.2-hd590300_0.conda#3bf7b9fd5a7136126e0234db4b87c8b6
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
-https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
-https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-h43f5ff8_6.conda#e54a5ddc67e673f9105cf2a2e9c070b0
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
@@ -49,61 +46,58 @@
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2#be93aabceefa2fac576e971aef407908
 https://conda.anaconda.org/conda-forge/linux-64/xorg-renderproto-0.11.1-h7f98852_1002.tar.bz2#06feff3d2634e3097ce2fe681474b534
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.6.2-h59595ed_0.conda#53fb86322bdb89496d7579fe3f02fd61
-https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
-https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_6.conda#3666a850342f8f3be88f9a93d948d027
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda#b3316cbe90249da4f8e84cd66e1cc55b
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_2.conda#9a3a42df8a95f65334dfc7b80da1195d
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h59595ed_1.conda#7fc9d3288d2420bb3637647621018000
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
-https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_6.conda#9342e7c44c38bea649490f72d92c382d
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
-https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda#ad7b68400f3a6ebe72b00be093c7f301
+https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda#2540b74d304f71d3e89c81209db4db84
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.9-h8ee46fc_0.conda#077b6e8ad6a3ddb741fce2496dd01bec
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
-https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
+https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-h04ea711_2.conda#f730d54ba9cd543666d7220c9f7ed563
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.1.0-hd590300_1.conda#f27a24d46e3ea7b70a1f98e50c62508f
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py312h30efb56_1.conda#45801a89533d3336a365284d93298e36
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py312h30efb56_0.conda#bdd639417094ace2fb1ce10b20d68d5d
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.10-h829c605_5.conda#8fdb82e5d9694dd8e9ed9ac8fdf48a26
+https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.11-hb9ae30d_0.conda#9bd27b5e21da16e40cf799bc2acf47d1
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/linux-64/jsonpointer-2.4-py312h7900ff3_3.conda#50f62bdb9b60b13c2f6ae69957342e4d
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py312h8572e83_1.conda#c1e71f2bc05d8e8e033aefac2c490d05
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.3.2-h658648e_1.conda#0ebb65e8d86843865796c7c95a941f34
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py312h98912ed_0.conda#6ff0b9582da2d4a74a1f9ae1f9ce2af6
@@ -112,47 +106,47 @@
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda#6598c056f64dc8800d40add25e4e2c34
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda#3facaca6cc0f7988df3250efccd32da3
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py312h98912ed_1.conda#e3fd78d8d490af1d84763b9fe3f2e552
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py312h886d080_0.conda#cc2cdf8f1792d29d21e17024745813d8
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.2-py312h8fd38d8_0.conda#361b4d1d4dd409d1c7584aba8db5021a
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.18.0-py312h4b3b743_0.conda#cc8165b34bdb002ade83b068f44e5774
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh0d859eb_0.conda#778594b20097b5a948c59e50ae42482a
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda#e8332e534dca8c5c12c8352e0a23501c
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda#5f25798dcefd8252ce5f9dc494d5f571
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.4-pyhd8ed1ab_0.conda#3d081de3a6ea9f894bbb585e8e3a4dcb
@@ -171,63 +165,63 @@
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py312h7900ff3_0.conda#eee5a2e3465220ed87196bbb5665f420
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h119a65a_9.conda#cfebc557e54905dadc355c0e9f003004
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda#629f3203c99b32e0988910c93e77f3b6
 https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py312hdcec9eb_0.conda#425bb325f970e57a047ac57c4586489d
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh0d859eb_0.conda#efba281bbdae5f6b0a1d53c6d4a97c93
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py312h98912ed_4.conda#00536e0a1734dcde9815fe227f32fc5a
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
-https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.4.0-h3d44ed6_0.conda#27f46291a6aaa3c2a4f798ebd35a7ddb
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py312heda63a1_0.conda#d8285bea2a350f63fab23bf460221f3f
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-23.1.0-pyhd8ed1ab_0.conda#3afef1f55a1366b4d3b6a0d92e2235e4
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py312h8572e83_0.conda#12c6a831ef734f0b2dd4caff514cbb7f
 https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda#9f359af5a886fd6ca6b2b6ea02e58332
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda#f0abe827c8a7c6d91bccdf90cb1fbee3
 https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.1-py312hfb8ada1_0.conda#e8fcd9179004edd4fb1bcd888d0aeb47
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.2-py312hfb8ada1_0.conda#3ccf705c4375feff4879ed4dd8c4cd90
 https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.2-ha41ecd1_0.conda#a658eeabf188c3040da36b0763de2bfd
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
-https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.1.2-py312hc7c0aa3_0.conda#e139cc775af7f13bffa3e4fd2d472a58
+https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.1.4-py312hc7c0aa3_0.conda#5573fa93bdbf5d1b4a81797d1c19e046
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py312heda63a1_0.conda#c53b9f319cafc679476f5613599857e8
 https://conda.anaconda.org/conda-forge/linux-64/astropy-6.0.1-py312hc7c0aa3_0.conda#7783f5436a1cdf53767ce6710cdd1649
 https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h280cfa0_4.conda#410f86e58e880dcc7b0e910a8e89c05c
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda#e0deff12c601ce5cb7476f93718f3168
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.2-pyhd8ed1ab_0.conda#67f86478c78637f68c1f3858973021f2
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.21.1-pyhd8ed1ab_0.conda#26bce4b5405738c09304d4f4796b2c2a
-https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hce6bd6c_0.conda#0891de8980ee29828542dbf9578838b9
+https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.58.0-hadf69e7_1.conda#0e2b5bd9533043b41f9482ae9e2c16b5
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py312he5832f3_0.conda#5377a9a29f607eebe4ad63eb82bcb575
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda#0b57b5368ab7fc7cdc9e3511fa867214
 https://conda.anaconda.org/conda-forge/linux-64/statsmodels-0.14.1-py312hc7c0aa3_0.conda#877a274575366e98a5f59e9b3e024b32
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-9.0.0-h78e8752_1.conda#a3f4cd4a512ec5db35ffbf25ba11f537
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-recommended-osx-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-recommended-osx-64.lock`

 * *Files 0% similar despite different names*

```diff
@@ -37,59 +37,59 @@
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libasprintf-devel-0.22.5-h5ff76d1_2.conda#c7182eda3bc727384e2f98f4d680fa7d
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.1.0-h0dc2134_1.conda#9ee0bab91b2ca579e10353738be36063
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.1.0-h0dc2134_1.conda#8a421fe09c6187f0eb5e2338a8a8be6d
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-13.2.0-h2873a65_3.conda#e4fb4d23ec2870ff3c40d10afe305aec
 https://conda.anaconda.org/conda-forge/osx-64/libintl-0.22.5-h5ff76d1_2.conda#3fb6774cb8cdbb93a6013b67bcf9716d
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda#65dcddb15965c9de2c0365cb14910532
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda#086f56e13a96a6cfb1bf640505ae6b70
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda#68e462226209f35182ef66eda0f794ff
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda#bd85e0ca9e1ffaadc3b56079fd956035
+https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda#50b997370584f2c83ca0c38e9028eab9
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda#570a6f04802df580be529f3a72d2bbf7
 https://conda.anaconda.org/conda-forge/osx-64/pcre2-10.43-h0ad2156_0.conda#9c8651803886ce9d5983e107a0df4ea8
 https://conda.anaconda.org/conda-forge/osx-64/pixman-0.43.4-h73e2aa4_0.conda#cb134c1e03fd32f4e6bea3f6de2614fd
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda#bf830ba5afc507c6232d4ef0fb1a882d
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-h93d8f39_0.conda#4c055e46b394be36681fe476c1e2ee6e
 https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda#80abc41d0c48b82fe0f04e7f42f5cb7e
 https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.1.0-h0dc2134_1.conda#ece565c215adcc47fc1db4e651ee094b
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h60636b9_2.conda#25152fce119320c980e5470e64834b50
 https://conda.anaconda.org/conda-forge/osx-64/gettext-tools-0.22.5-h5ff76d1_2.conda#37e1cb0efeff4d4623a6357e37e0105d
 https://conda.anaconda.org/conda-forge/osx-64/libgettextpo-0.22.5-h5ff76d1_2.conda#54cc9d12c29c2f0516f2ef4987de53ae
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-13_2_0_h97931a8_3.conda#0b6e23a012ee7a9a5f6b244f5a92c1d5
-https://conda.anaconda.org/conda-forge/osx-64/libglib-2.80.0-h81c1438_4.conda#eb94cd8fdcb676d17a5119189f87c4ae
+https://conda.anaconda.org/conda-forge/osx-64/libglib-2.80.0-h81c1438_6.conda#54dd1ed37dd65c5d13600bcc5ebbd0a1
 https://conda.anaconda.org/conda-forge/osx-64/libintl-devel-0.22.5-h5ff76d1_2.conda#ea0a07e556d6b238db685cae6e3585d0
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.6.0-h129831d_3.conda#568593071d2e6cea7b5fc1f75bfa10ca
-https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda#0179b8007ba008cf5bec11f3b3853902
+https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda#df1448ec6cbf8eceb03d29003cf72ae6
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda#cc4834a9ee7cc49ce8d25177c47b10d8
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
-https://conda.anaconda.org/conda-forge/osx-64/atk-1.0-2.38.0-h1d18e73_1.tar.bz2#5a538295f97a484ee332aacc131718b5
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
+https://conda.anaconda.org/conda-forge/osx-64/atk-1.0-2.38.0-h4bec284_2.conda#d9684247c943d492d9aac8687bc5db77
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
 https://conda.anaconda.org/conda-forge/osx-64/brotli-1.1.0-h0dc2134_1.conda#9272dd3b19c4e8212f8542cefd5c3d67
 https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.1.0-py312heafc425_1.conda#a288b88f06b8bfe0dedaf5c4b6ac6b7a
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py312hede676d_0.conda#e0de4e018d6013b6c2e2ae42640fb65c
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/osx-64/fontconfig-2.14.2-h5bb23bf_0.conda#86cc5867dfbee4178118392bae4a3c89
-https://conda.anaconda.org/conda-forge/osx-64/gdk-pixbuf-2.42.10-hd9e0ca3_5.conda#308cefd960b6ba51bdbdc5ba9e9b2377
+https://conda.anaconda.org/conda-forge/osx-64/gdk-pixbuf-2.42.11-ha9f1606_0.conda#ab407c96c658772c9bcd7161931fd933
 https://conda.anaconda.org/conda-forge/osx-64/gts-0.7.6-h53e17e3_4.conda#848cc963fcfbd063c7a023024aa3bec0
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/osx-64/jsonpointer-2.4-py312hb401068_3.conda#637aa8f6c1c61f659f1496e9b2dc7552
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.5-py312h49ebfd2_1.conda#21f174a5cfb5964069c374171a979157
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.16-ha2f27b4_0.conda#1442db8f03517834843666c422238c9b
 https://conda.anaconda.org/conda-forge/osx-64/libgettextpo-devel-0.22.5-h5ff76d1_2.conda#1e0384c52cd8b54812912e7234e66056
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.27-openmp_hfef2a42_0.conda#00237c9c7f2cb6725fe2960680a6e225
 https://conda.anaconda.org/conda-forge/osx-64/libwebp-1.3.2-h44782d1_1.conda#46d48ff2cd600a82db18d7b83471aa86
@@ -99,46 +99,46 @@
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda#6598c056f64dc8800d40add25e4e2c34
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.2-h7310d3a_0.conda#05a14cc9d725dd74995927968d6547e3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda#03926e7089a5e61b77043b470ae7b553
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py312h104f124_1.conda#260ed90aaf06061edabd7209638cf03b
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py312hc789acb_0.conda#af49da330d412bc3203bc84f8153d685
+https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.2-py312h18237bf_0.conda#ef0464a4c36e227cc941c549adbd5f87
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.18.0-py312h1b0e595_0.conda#75d882a5a5ff8e970eff0e30591d6ca6
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda#2d2d1fde5800d45cb56218583156d23d
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda#ac95aa8ed65adfdde51132595c79aade
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda#5f25798dcefd8252ce5f9dc494d5f571
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.4-pyhd8ed1ab_0.conda#3d081de3a6ea9f894bbb585e8e3a4dcb
 https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda#9669586875baeced8fc30c0826c3270e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.3-pyha770c72_0.conda#332493000404d8411859539a5a630865
@@ -155,31 +155,31 @@
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py312hb401068_0.conda#a205e28ce7ab71773dcaaf94f6418612
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-22_osx64_openblas.conda#b80966a8c8dd0b531f8e65f709d732e8
 https://conda.anaconda.org/conda-forge/osx-64/libgd-2.3.3-h0dceb68_9.conda#1feb43971521d430bf826f8398598c5b
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda#629f3203c99b32e0988910c93e77f3b6
 https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py312h0c923fa_0.conda#6f0591ae972e9b815739da3392fbb3c3
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-10.2-py312h74abf1d_0.conda#fc53fe067431dee92471aac39ed58128
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh31c8845_0.conda#00b54981b923f5aefcd5e8547de056d5
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py312h104f124_4.conda#dddfb6125aed1fb84eb13319007c08fd
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
-https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-8.3.0-hf45c392_0.conda#41d890485f909e4ecdc608741718c75e
+https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-8.4.0-h72fa137_0.conda#7d065a2266ae5eb2a5d91a6dca4fca69
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda#6ef2b72d291b39e479d7694efa2b2b98
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda#a0e4efb5f35786a05af4809a2fb1f855
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-22_osx64_openblas.conda#b9fef82772330f61b2b0201c72d2c29b
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-22_osx64_openblas.conda#f21b282ff7ba14df6134a0fe6ab42b1b
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-10.2-py312h74abf1d_0.conda#b5fca135abb5b6d34afceb96c91e60fd
@@ -195,28 +195,28 @@
 https://conda.anaconda.org/conda-forge/osx-64/pango-1.52.2-h7f2093b_0.conda#ea9611aee7e61e4ff18c4dc56ec100ab
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh31c8845_0.conda#c3cb67fc72fb38020fe7923dbbcf69b0
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.2.1-py312h9230928_0.conda#079df34ce7c71259cfdd394645370891
 https://conda.anaconda.org/conda-forge/osx-64/gtk2-2.24.33-h8ca4665_4.conda#ff451625250bf843393ca3d660accab3
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda#28e74fca8d8abf09c1ed0d190a17e307
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.2-pyhd8ed1ab_0.conda#67f86478c78637f68c1f3858973021f2
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.21.1-pyhd8ed1ab_0.conda#26bce4b5405738c09304d4f4796b2c2a
-https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.58.0-h7b06fc5_0.conda#3ad98f9e1ad2b0c9b202b9d5212752d2
+https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.58.0-h7b06fc5_1.conda#e4a5f1bb5962ec6f2f2d2f0467ed0826
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda#0b57b5368ab7fc7cdc9e3511fa867214
-https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.1-py312h83c8a23_0.conda#c562e07382cdc3194c21b8eca06460ff
+https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.2-py312h83c8a23_0.conda#b422a5d39ff0cd72923aef807f280145
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
-https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.1.2-py312h3f2338b_0.conda#0342bfab6b7340de1840a3fb7c73ce2b
+https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.1.4-py312h3f2338b_0.conda#d8132701147c2e7d13b93879f63a62b8
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.13.0-py312h8adb940_0.conda#818232a7807c76970172af9c7698ba4a
 https://conda.anaconda.org/conda-forge/osx-64/astropy-6.0.1-py312h3f2338b_0.conda#057f5d530d337b37ba2cf4c4b43af622
 https://conda.anaconda.org/conda-forge/osx-64/graphviz-9.0.0-hee74176_1.conda#7cd479251093c332aa9fe93cfb8f698b
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.8.4-py312h1fe5000_0.conda#3e3097734a5042cb6d2675e69bf1fc5a
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/osx-64/statsmodels-0.14.1-py312h3f2338b_0.conda#65131405e95790c86f9ad45e3004724d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-recommended-win-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-recommended-win-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # input_hash: 140ed1c3c92d540517db0891331ccf11d834d0f8186d785832c17814e00fb771
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda#63da060240ab8087b60d1357051ea7d6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda#30ebb9fd99666d8b8675fcee541a09f3
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda#c66eb2fd33b999ccc258aef85689758e
 https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda#bc592d03f62779511d392c175dcece64
 https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2#b0309b72560df66f71a9d5e34a5efdfa
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda#17f4ccf6be9ded08bd0a376f489ac1a6
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
 https://conda.anaconda.org/conda-forge/win-64/expat-2.6.2-h63175ca_0.conda#52f9dec6758ceb8ce0ea8af9fa13eb1a
@@ -31,38 +31,38 @@
 https://conda.anaconda.org/conda-forge/win-64/lerc-4.0.0-h63175ca_0.tar.bz2#1900cb3cab5055833cfddb0ba233b074
 https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.1.0-hcfcfb64_1.conda#f77f319fb82980166569e1280d5b2864
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.20-hcfcfb64_0.conda#b12b5bde5eb201a1df75e49320cc938a
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda#e1eb10b1cca179f2baa3601e4efc8712
 https://conda.anaconda.org/conda-forge/win-64/libjpeg-turbo-3.0.0-hcfcfb64_1.conda#3f1b948619c45b1ca714d60c7389092c
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda#f95359f8dc5abf7da7776ece9ef10bc5
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda#73f5dc8e2d55d9a1e14b11f49c3b4a28
 https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.2-hcfcfb64_1.conda#fdf80cb33c32d4d002bb89c37cfff5b7
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda#958e0418e93e50c575bff70fbcaa12d8
 https://conda.anaconda.org/conda-forge/win-64/pixman-0.43.4-h63175ca_0.conda#b98135614135d5f458b75ab9ebb9558c
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda#fc048363eb8f03cd1737600a5d08aafe
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.1.0-hcfcfb64_1.conda#19ce3e1dacc7912b3d6ff40690ba9ae0
 https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.1.0-hcfcfb64_1.conda#71e890a0b361fd58743a13f77e1506b7
 https://conda.anaconda.org/conda-forge/win-64/libintl-0.22.5-h5728263_2.conda#aa622c938af057adc119f8b8eecada01
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.43-h19919ed_0.conda#77e398acc32617a0384553aea29e866b
 https://conda.anaconda.org/conda-forge/win-64/libwebp-1.3.2-hcfcfb64_1.conda#6202a1ba6be2713084cf0452d4e8c10c
-https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_1.conda#eb9f59dd51f50f5aa369813fa63ba569
+https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_2.conda#ac7af7a949db01dae61ddc48f4a93d79
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.43-h17e33f8_0.conda#d0485b8aa2cedb141a7bd27b4efa4c9c
-https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda#be8803e9f75a477df61d4aabea3c1246
+https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda#f07c8c5dd98767f9a652de5d039b284e
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-h63175ca_1.conda#e8867cc4d023f41f54bd64a33436b0a1
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda#792bb5da68bf0a6cac6a6072ecb8dbeb
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
-https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.8.0.32.4-pyhd8ed1ab_0.conda#5e17cd1c08dd19e99ac0476404f550e6
+https://conda.anaconda.org/conda-forge/noarch/astropy-iers-data-0.2024.4.29.0.28.48-pyhd8ed1ab_0.conda#3ece30e82dd783d789fbc3f5a9c72911
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda#5e4c0743c70186509d1412e03c2d8dfa
 https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.1.0-hcfcfb64_1.conda#0105229d7c5fabaa840043a86c10ec64
 https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.1.0-py312h53d5487_1.conda#d01a6667b99f0e8ad4097af66c938e62
 https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
@@ -72,64 +72,64 @@
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda#e16be50e378d8a4533b989035b196ab8
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-hdaf720e_2.conda#3761b23693f768dc75a8fd0a73ca053f
 https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2#914d6646c4dbb1fd3ff539830a12fd71
 https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2#9f765cbfab6870c8435b9eefecd7a1f4
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.24-pyhd8ed1ab_0.conda#fc9780a517b51ea3798fc011c17ffd51
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.25-pyhd8ed1ab_0.conda#5d8c241a9261e720a34a07a3e1ac4109
 https://conda.anaconda.org/conda-forge/win-64/jsonpointer-2.4-py312h2e8e312_3.conda#9d9572e257bf4559f20629efb0d3511d
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.10-pyhd8ed1ab_0.conda#16b73b2c4ff7dda8bbecf88aadfe2027
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.5-py312h0d7def4_1.conda#77c9d46fc8680bb08f4e1ebb6669e44e
-https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_4.conda#9baf04fc7002450a932cf97cb9625ebb
-https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda#87da045f6d26ce9fe20ad76a18f6a18a
+https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_6.conda#cd5c6efbe213c089f78575c98ab9a0ed
+https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda#ee944f0d41d9e2048f9d7492c1623ca3
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.6.0-hddb2be6_3.conda#6d1828c9039929e2f185c5fa9d133018
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py312he70551f_0.conda#4950a739b19edaac1ed29ca9474e49ac
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.2-pyhd8ed1ab_0.conda#5cbee699846772cc939bef23a0d524ed
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda#6598c056f64dc8800d40add25e4e2c34
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda#81534b420deb77da8833f2289b8d47ac
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda#405678b942f2481cecdb3e010f4925d9
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.20.0-pyhd8ed1ab_0.conda#9a19b94034dd3abb2b348c8b93388035
 https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda#5f2998851564bea33a159bd00e6249e8
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda#844d9eb3b43095b031874477f7d70088
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda#4d3ceee3af4b0f9a1f48f57176bf8625
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda#f44c8f35c3f99eca30d6f5b68ddb0f42
 https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.13-py312h53d5487_0.conda#84bc43e330340c01ce93231c096d4ab1
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py312he70551f_1.conda#f91e0baa89ba21166916624ba7bfb422
-https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py312h1ac6f91_0.conda#74194f888cc7b11d8c18edf416b61a1b
+https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.2-py312hd7027bb_0.conda#edf821f4104e0f1cfc572711804014ad
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.18.0-py312hfccd98a_0.conda#4f201390adc379696fb0bd3f2b5cdcc7
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda#490730480d76cf9c8f8f2849719c6e2b
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.5-pyhd8ed1ab_1.conda#3f144b2c34f8cb5a9abd9ed23a39c561
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda#98907504f8c3eb0452bb10362227ce16
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda#af5fa2d2186003472e766a23c46cae04
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda#3df84416a021220d8b5700c613af2dc5
 https://conda.anaconda.org/conda-forge/noarch/types-python-dateutil-2.9.0.20240316-pyhd8ed1ab_0.conda#7831efa91d57475373ee52fb92e8d137
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda#68f0738df502a14213624b288c60c9ad
 https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda#daf5160ff9cde3a468556965329085b9
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.7.0-pyhd8ed1ab_0.conda#50ad31e07d706aae88b14a4ac9c73f23
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.8.0-pyhd8ed1ab_0.conda#f372c576b8774922da83cda2b12f9d29
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.10-pyhd8ed1ab_0.conda#521f489e3babeddeec638c2add7e9e64
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/xorg-kbproto-1.0.7-hcd874cb_1002.tar.bz2#8d11c1dac4756ca57e78c1bfe173bba4
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
 https://conda.anaconda.org/conda-forge/win-64/xorg-xextproto-7.3.0-hcd874cb_1003.conda#6e6c2639620e436bddb7c040cd4f3adb
 https://conda.anaconda.org/conda-forge/win-64/xorg-xproto-7.0.31-hcd874cb_1007.tar.bz2#88f3c65d2ad13826a9e0b162063be023
@@ -152,26 +152,26 @@
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda#81a3be0b2023e1ea8555781f0ad904a2
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda#e7d8df6509ba635247ff9aea31134262
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py312h2e8e312_0.conda#3ed5c1981d05f125696f392407d36ce2
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.3.0-pyhd8ed1ab_1.conda#afcd1b53bcac8844540358e33f33d28f
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.16-h67d730c_0.conda#d3592435917b62a8becff3a60db674f6
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.15-hcd874cb_0.conda#090d91b69396f14afef450c285f9758c
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda#779345c95648be40d22aaa89de7d4254
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda#7e7099ad94ac3b599808950cec30ad4e
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.7.0-pyhd8ed1ab_0.conda#24fba5a9d161ad8103d4e84c0e1a3ed4
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda#0bf64bf10eee21f46ac83c161917fa86
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda#e4492c22e314be5c75db3469e3bbf3d9
+https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda#52ddb316ef9136ba610f7fac57da9062
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.3-pyh5737063_0.conda#5a86a21050ca3831ec7f77fb302f1132
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda#21069f3ed16812f9f4f2700667b6ec86
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda#21745fdd12f01b41178596143cbecffd
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.18.1-pyh5737063_0.conda#4abd500577430a942a995fd0d09b76a2
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda#8662629d9a05f9cff364e31ca106c1ac
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda#471e3988f8ca5e9eb3ce6be7eac3bcee
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py312he70551f_4.conda#69b7a1d899d46b91f8eecab9abf9728c
 https://conda.anaconda.org/conda-forge/noarch/arrow-1.3.0-pyhd8ed1ab_0.conda#b77d8c2313158e6e461ca0efb1c2c508
 https://conda.anaconda.org/conda-forge/win-64/cairo-1.18.0-h1fef639_0.conda#b3fe2c6381ec74afe8128e16a11eee02
 https://conda.anaconda.org/conda-forge/win-64/fonttools-4.51.0-py312he70551f_0.conda#6820105f0928bb46b99358d45d4f3994
 https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda#a6b9a0158301e697e4d0a36a3d60e133
@@ -180,15 +180,15 @@
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.5.3-pyhd8ed1ab_0.conda#219b3833aa8ed91d47d1be6ca03f30be
 https://conda.anaconda.org/conda-forge/win-64/mkl-2024.1.0-h66d3029_692.conda#b43ec7ed045323edeff31e348eea8652
 https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py312h6f6a607_0.conda#8d5f5f1fa36200f1ef987299a47de403
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/win-64/xorg-libx11-1.8.9-hefa74cf_0.conda#3672e991346895f332af1ebc60b8bca9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-23.1.0-pyhd8ed1ab_0.conda#3afef1f55a1366b4d3b6a0d92e2235e4
-https://conda.anaconda.org/conda-forge/win-64/harfbuzz-8.3.0-h7ab893a_0.conda#b8ef0beb91df83c5e6038c9509b9f730
+https://conda.anaconda.org/conda-forge/win-64/harfbuzz-8.4.0-h7ab893a_0.conda#bf9b853f9702724a5ec4e68dc637cc29
 https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda#9f359af5a886fd6ca6b2b6ea02e58332
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh7428d3b_0.conda#f803d121b60dff8f4d8f9264b7c6e8bf
 https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda#8a3a3d01629da20befa340919e3dd2c4
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda#c03972cfce69ad913d520c652e5ed908
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-22_win64_mkl.conda#65c56ecdeceffd6c32d3d54db7e02c6e
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
@@ -203,26 +203,26 @@
 https://conda.anaconda.org/conda-forge/win-64/pango-1.52.2-h07c897b_0.conda#d4b8ab1b86d06d9d6c65eaed989a018d
 https://conda.anaconda.org/conda-forge/win-64/xorg-libsm-1.2.4-hcd874cb_0.conda#25926681339df15918243d9a7cec25a1
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.10.0-pyhd8ed1ab_0.conda#ed45423c41b3da15ea1df39b1f80c2ca
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.10.0-pyhd8ed1ab_0.conda#15b51397e0fe8ea7d7da60d83eb76ebc
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.26.4-py312h8753938_0.conda#f9ac74c3b07c396014434aca1e58d362
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxt-1.3.0-hcd874cb_1.conda#511a29edd2ff3d973f63e54f19dcc06e
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.2.1-py312h0d7def4_0.conda#bc0160f16ae02e18de578eaddadd4f61
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_0.conda#0cab42b4917e71df9dc2224b9940ef19
-https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.1-py312h2ab9e98_0.conda#864da9103c0201f4ee512910eee91ab0
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.16.3-pyhd8ed1ab_1.conda#2f34a65aee1d1f354e701d166413783a
+https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.2-py312h2ab9e98_0.conda#32723785b7b4fca8784cc7cadb097009
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.6-pyhd8ed1ab_0.conda#a5b55d1cb110cdcedc748b5c3e16e687
-https://conda.anaconda.org/conda-forge/win-64/pyerfa-2.0.1.2-py312ha90f08f_0.conda#555842d2cc3ec0dd91c85bf9e9c491aa
+https://conda.anaconda.org/conda-forge/win-64/pyerfa-2.0.1.4-py312ha90f08f_0.conda#82f951dc7db82be47159e4da69b1c701
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.13.0-py312h8753938_0.conda#0acd540ee94e0f2148e8d351ed7c49e8
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxpm-3.5.17-hcd874cb_0.conda#029be9b667bf3896fa28bc32adb1bfc3
 https://conda.anaconda.org/conda-forge/win-64/astropy-6.0.1-py312ha90f08f_0.conda#25d024a2c21f50a4f734e8d91e99f2bc
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.13.0-pyhd8ed1ab_0.conda#e242df505f194c4932fbb840a99207e2
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.14.0-pyhd8ed1ab_0.conda#b82b9798563dea0cd8e4e3074227f04c
 https://conda.anaconda.org/conda-forge/win-64/libgd-2.3.3-h312136b_9.conda#69c987e1f9268d9ade86497c4ab8cc45
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.8.4-py312h26ecaf7_0.conda#e83910bd39860772aaefee3e0eb1c29f
 https://conda.anaconda.org/conda-forge/win-64/statsmodels-0.14.1-py312ha90f08f_0.conda#16f577f829d422d205396be1b774a5ee
 https://conda.anaconda.org/conda-forge/win-64/graphviz-9.0.0-h51cb2cd_1.conda#9e73e70557ae3c1c9d4bdf70f47dd141
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.5-pyhd8ed1ab_0.conda#885867f6adab3d7ecdf8ab6ca0785f51
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.26.0-pyhd8ed1ab_0.conda#bd9f28ac8833e63eeadb69aa1341f269
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.27.1-pyhd8ed1ab_0.conda#d97923b777ce837cf67e7858ac600834
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.4-pyhd8ed1ab_0.conda#3d85618e2c97ab896b5b5e298d32b5b3
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.13.2-pyhd8ed1ab_0.conda#0918a9201e824211cdf444dbf8d55752
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.6-pyhd8ed1ab_0.conda#8b0a6b8edbaef9796d2b925c63441b8e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.1.8-pyhd8ed1ab_0.conda#1116781efc9fd1654a9da329d5d3ba26
 https://conda.anaconda.org/conda-forge/noarch/python-graphviz-0.20.3-pyh717bed2_0.conda#031c005eb6d4513013d99ed163dd5f59
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.13.2-hd8ed1ab_0.conda#fd31ebf5867914de597f9961c478e482
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-tests-linux-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-tests-linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 11740d44caa859db385fa6134265951c773515b84ebeecc70651711c4f054d1d
+# input_hash: 51da749d6c37de837c59b9102ae5587942eb5d0c42ef647eb2b6460ee62fe1ca
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda#2f4327a1cbe7f022401b236e915a5fef
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda#6185f640c43843e5ad6fd1c5372c3f80
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda#f6f6600d18a4047b54f803cf708b868a
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda#10569984e7db886e4f1abc2b47ad79a1
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda#3cfab3e709f77e9f1b3d380eb622494a
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-4_cp39.conda#bfe4b3259a8ac6cdf0037752904da6a7
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda#d211c42b9ce49aee3734fdc828731689
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda#aae89d3736661c36a5591788aebd0817
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda#d4ff227c46917d3b4565302a2bbb276b
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda#df88796bd09a0d2ed292e59101478ad8
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.11-hd590300_1.conda#0bb492cca54017ea314b809b1ee3a176
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda#69b8b6202a07720f448be700e300ccf4
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.28.1-hd590300_0.conda#dcde58ff9a1f30b0037a2315d1846d1f
 https://conda.anaconda.org/conda-forge/linux-64/gettext-tools-0.22.5-h59595ed_2.conda#985f2f453fb72408d6b6f1be0f324033
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h59595ed_1003.conda#f87c7b7c2cb45f323ffbce941c78ab7c
 https://conda.anaconda.org/conda-forge/linux-64/icu-73.2-h59595ed_0.conda#cc47e1facc155f91abd89b11e48e72ff
@@ -31,22 +31,22 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-0.22.5-h661eb56_2.conda#dd197c968bf9760bba0031888d431ede
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.1.0-hd590300_1.conda#aec6c91c7371c26392a06708a73c70e5
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.20-hd590300_0.conda#8e88f9389f1165d7c0936fe40d9a9a79
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-hd590300_2.conda#172bf1cd1ff8629f2b1179945ed45055
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda#e7ba12deb7020dd080c6c70e7b6f6a3d
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-0.22.5-h59595ed_2.conda#172bcc51059416e7ce99e7b528cede83
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda#7a6bd7a12a4bd359e2afe6c0fa1acace
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-h43f5ff8_6.conda#e54a5ddc67e673f9105cf2a2e9c070b0
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda#d66573916ffcf376178462f1b61c941e
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-3.0.0-hd590300_1.conda#ea25936bb4080d843790b586850f82b8
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda#30fd6e37fe21f86f4bd26d6ee73eeec7
 https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda#049b7df8bae5e184d1de42cdf64855f8
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.4.0-hd590300_0.conda#b26e8aa824079e1be0294e7152ca4559
 https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda#5aa797f8787fe7a17d1b0821485b5adc
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.32.6-h59595ed_0.conda#9160cdeb523a1b20cf8d2a0bf821f45d
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda#97da8860a0da5413c7c98a3b3838a645
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda#9d731343cff6ee2e5a25c4a091bf8e2a
@@ -67,36 +67,36 @@
 https://conda.anaconda.org/conda-forge/linux-64/libasprintf-devel-0.22.5-h661eb56_2.conda#02e41ab5834dcdcc8590cf29d9526f50
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.1.0-hd590300_1.conda#f07002e225d7a60a694d42a7bf5ff53f
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.1.0-hd590300_1.conda#5fc11c6020d421960607d821310fcd4d
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.69-h0f662aa_0.conda#25cb5999faa414e5ccb2c1388f62d3d5
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
 https://conda.anaconda.org/conda-forge/linux-64/libgettextpo-devel-0.22.5-h59595ed_2.conda#b63d9b6da3653179a278077f0de20014
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda#e73e9cfd1191783392131e6238bdb3e9
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_6.conda#3666a850342f8f3be88f9a93d948d027
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.58.0-h47da74e_1.conda#700ac6ea6d53d5510591c4344d5c989a
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.43-h2797004_0.conda#009981dd9cfcaa4dbfa25ffaed86bcae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda#866983a220e27a80cb75e85cb30466a1
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda#b3316cbe90249da4f8e84cd66e1cc55b
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda#6853448e9ca1cfd5f15382afd2a6d123
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_2.conda#9a3a42df8a95f65334dfc7b80da1195d
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.10.1-h2629f0a_3.conda#ac79812548e7e8cf61f7b0abdef01d3b
 https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.3.0-hf1915f5_4.conda#784a4df6676c581ca624fbe460703a6d
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda#8292dea9e022d9610a11fce5e0896ed8
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda#d453b98d9c83e71da0741bb0ff4d76bc
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda#04b88013080254850d6c01ed54810589
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.5-hc2324a3_1.conda#11d76bee958b1989bd1ac6ee7372ea6d
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.1.0-hd590300_1.conda#39f910d205726805a958da408ca194ba
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-h267a509_2.conda#9ae35c3d96db2c94ce0cef86efdfa2cb
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.22.5-h59595ed_2.conda#219ba82e95d7614cf7140d2a4afc0926
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda#cd95826dbd331ed1be26bdf401432844
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda#0269d2b7fa89f4a37cdee5ad6161f6cc
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_6.conda#9342e7c44c38bea649490f72d92c382d
 https://conda.anaconda.org/conda-forge/linux-64/libllvm15-15.0.7-hb3ce162_4.conda#8a35df3cbc0c8b12cc8af9473ae75eef
 https://conda.anaconda.org/conda-forge/linux-64/libllvm18-18.1.3-h2448989_0.conda#927b6d6e80b2c0d4405a58b61ca248a3
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.27-pthreads_h413a1c8_0.conda#a356024784da6dfd4683dc5ecf45b155
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda#66f03896ffbe1a110ffda05c7a856504
 https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.3.0-hca2cd23_4.conda#1b50eebe2a738a3146c154d2eceaa8b6
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.98-h1d7d5a4_0.conda#54b56c2fdf973656b748e0378900ec13
 https://conda.anaconda.org/conda-forge/linux-64/python-3.9.19-h0755675_0_cpython.conda#d9ee3647fbd9e8595b8df759b2bbefb8
@@ -115,42 +115,42 @@
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_4.conda#c9deba4959ea5b5f72f1e3e4a71ae014
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_6.conda#a9d23c02485c5cf055f9ac90eb9c9c63
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.5-py39h7633fee_1.conda#c9f74d717e5a2847a9f8b779c54130f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.16-hb7c19ff_0.conda#51bb7010fc86f70eee639b4bb7a894f5
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-22_linux64_openblas.conda#1a2a0cd3153464fee6646f3dd6dad9b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang-cpp15-15.0.7-default_h127d8a8_5.conda#d0a9633b53cdc319b8a1a532ae7822b8
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-18.1.3-default_h5d6823c_0.conda#5fff487759736b275dc3e4a263cac666
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h4637d8d_4.conda#d4529f4dff3057982a7617c7ac58fde3
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.7.1-hca28451_0.conda#755c7f876815003337d2c61ff5d047e5
 https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
-https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.48-h71f35ed_0.conda#4d18d86916705d352d5f4adfb7f0edd3
+https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.49-h4f305b6_0.conda#dfcfd72c7a430d3616763ecfbefe4ca9
 https://conda.anaconda.org/conda-forge/linux-64/libpq-16.2-h33b98f1_1.conda#9e49ec2a61d02623b379dc332eb6889d
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda#7f2e286780f072ed750df46dc2631138
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.8-py39hd1e30aa_0.conda#b1961e70cfe8e1eac243faf933d1813f
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py39hd1e30aa_0.conda#1e865e9188204cdfb1fd2531780add88
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.1.0-py39hd1e30aa_0.conda#1da984bbb6e765743e13388ba7b7b2c8
@@ -158,58 +158,58 @@
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.41-hd590300_0.conda#81f740407b45e3f9047b3174fa94eb9e
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda#f907bb958910dc404647326ca80c263e
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.51.0-py39hd1e30aa_0.conda#79f5dd8778873faa54e8f7b2729fe8a6
-https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_4.conda#5521382ee30b96b35eb0037fc3c4f2b4
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_6.conda#a1e026a82a562b443845db5614ca568a
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.3-nompi_h4f84152_100.conda#d471a5c3abc984b662d9bae3bb7fd8a5
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-22_linux64_openblas.conda#4b31699e0ec5de64d5896e580389c9a1
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.3-hd590300_0.conda#32d16ad533c59bb0a3c5ffaf16110829
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-22_linux64_openblas.conda#b083767b6c877e24ee597d93b87ab838
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.2-hc60ed4a_1.conda#ef1910918dd895516a769ed36b5b3a4e
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.7.0-h662e7e4_0.conda#b32c0da42b1f24a98577bb3d7fc0b995
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py39h90c7501_0.conda#1e3b6af9592be71ce19f0a6aae05d97b
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.18.6-py39hd1e30aa_0.conda#2289054e90cf07e35280bbe798811dc8
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.12-py39h3d6467e_0.conda#e667a3ab0df62c54e60e1843d2e6defb
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.24.1-h98fc4e7_1.conda#b04b5cdf3ba01430db27979250bc5a1d
-https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda#5a6f6c00ef982a9bc83558d9ac8f64a0
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.4.0-h3d44ed6_0.conda#27f46291a6aaa3c2a4f798ebd35a7ddb
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h9612171_113.conda#b2414908e43c442ddc68e6148774a304
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-255-h3516f8a_1.conda#3366af27f0b593544a6cd453c7932ac5
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.26.4-py39h474f0d3_0.conda#aa265f5697237aa13cc10f53fa8acc4f
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.12.2-py39h3d6467e_5.conda#93aff412f3e49fdb43361c0215cbd72d
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.1.1-pyhd8ed1ab_0.conda#52b91ecba854d55b28ad916a8b10da24
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.3-py39h44dd56e_0.conda#baea2f5dfb3ab7b1c836385d2e1daca7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.2.1-py39h7633fee_0.conda#bdc188e59857d6efab332714e0d01d93
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.24.1-hfa15dee_1.conda#a6dd2bbc684913e2bef0a54ce56fcbfb
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.1-py39hddac248_0.conda#85293a042c24a08e71b7608ee66b6134
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.2.2-py39hddac248_0.conda#259c4e76e6bda8888aefc098ae1ba749
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-17.0-hb77b528_0.conda#07f45f1be1c25345faddb8db0de8039b
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.13.0-py39h474f0d3_0.conda#46ae0ecba9726ab4fa44c78fefa522cf
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.8.4-py39he9076e7_0.conda#1919384a8420e7bb25f6c3a582e0857c
 https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.5-nompi_py39h4282601_100.conda#d2809fbf0d8ae7b8ca92c456cb44a7d4
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-hc9dc06e_21.conda#b325046180590c868ce0dbf267b82eb8
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.9-py39h52134e7_5.conda#e1f148e57d071b09187719df86f513c1
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.8.4-py39hf3d152e_0.conda#c66d2da2669fddc657b679bccab95775
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-tests-osx-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-tests-osx-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 8c7dd1ef0af5cbd9ca11a96fddcc559053b94f49ec59c92b997ea7b41087414a
+# input_hash: 3261d5e13b4179aa5bd9145672a489591ce01cd7db2f66fb37170013013e5268
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda#6097a6ca9ada32699b5fc4312dd6ef18
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.28.1-h10d778d_0.conda#d5eb7992227254c0e9a0ce71151f0079
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda#f2eacee8c33c43692f1ccfd33d0f50b1
 https://conda.anaconda.org/conda-forge/osx-64/icu-73.2-hf5e326d_0.conda#5cc301d759ec03f28328428e28f65591
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.1.0-h0dc2134_1.conda#9e6c31441c9aa24e41ace40d6151aab6
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.20-h49d49c5_0.conda#d46104f6a896a0bc6a1d37b88b2edf5c
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-h10d778d_2.conda#899db79329439820b7e8f8de41bca902
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hd75f5a5_2.conda#6c3628d047e151efba7cf08c5e54d1ca
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-3.0.0-h0dc2134_1.conda#72507f8e3961bc968af17435060b6dd6
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.2-h10d778d_1.conda#1ff09ca6e85ee516442a6a94cdfc7065
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.4.0-h10d778d_0.conda#b2c0047ea73819d992484faacbbe1c24
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-18.1.3-hb6ac08f_0.conda#506f270f4f00980d27cc1fc127e0ed37
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda#50f28c512e9ad78589e3eab34833f762
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.9-4_cp39.conda#2d9f6c00555127a9058cfa955adf1090
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
@@ -27,17 +27,17 @@
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.1.3-h73e2aa4_0.conda#66d3c1f6dd4636216b4fca7a748d50eb
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.1.0-h0dc2134_1.conda#9ee0bab91b2ca579e10353738be36063
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.1.0-h0dc2134_1.conda#8a421fe09c6187f0eb5e2338a8a8be6d
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-13.2.0-h2873a65_3.conda#e4fb4d23ec2870ff3c40d10afe305aec
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda#65dcddb15965c9de2c0365cb14910532
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda#086f56e13a96a6cfb1bf640505ae6b70
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda#68e462226209f35182ef66eda0f794ff
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda#bd85e0ca9e1ffaadc3b56079fd956035
+https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda#50b997370584f2c83ca0c38e9028eab9
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda#570a6f04802df580be529f3a72d2bbf7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.2.0-h6dc393e_1.conda#9c322ec36340610fcf213b72999b049e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda#bf830ba5afc507c6232d4ef0fb1a882d
 https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda#80abc41d0c48b82fe0f04e7f42f5cb7e
@@ -59,34 +59,34 @@
 https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda#0876280e409658fc6f9e75d035960333
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda#f3ad426304898027fc619827ff428eca
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.5-py39h8ee36c8_1.conda#6072db04642b21329b0502a177ec18bf
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.16-ha2f27b4_0.conda#1442db8f03517834843666c422238c9b
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.7.1-h726d00d_0.conda#fa58e5eaa12006bc3289a71357bef167
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.27-openmp_hfef2a42_0.conda#00237c9c7f2cb6725fe2960680a6e225
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.2-h7310d3a_0.conda#05a14cc9d725dd74995927968d6547e3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.8-py39ha09f3b3_0.conda#835c656934865805c0b02dbff74fe5b7
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py39ha09f3b3_0.conda#4541517b5a605bf45d4a5fb074bb4cf5
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.1.0-py39hdc70f33_0.conda#ede122e9ef2775a8879063d9d3ee819f
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
@@ -95,15 +95,15 @@
 https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.3-nompi_h691f4bf_100.conda#8e2ac4ae815a8c9743fe37d70f48f075
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-22_osx64_openblas.conda#b80966a8c8dd0b531f8e65f709d732e8
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py39h9dabb2a_0.conda#e385068c9511542eff20422f7e799064
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.18.6-py39ha09f3b3_0.conda#6eb863d10b7aeef1f58ba1ebf92f59bd
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-0.12.3-pyhd8ed1ab_0.conda#cf2c3a89f89644c53cadbfeb124914e9
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda#08807a87fa7af10754d46f63b368e016
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
@@ -117,17 +117,17 @@
 https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda#ba445bf767ae6f0d959ff2b40c20912b
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.26.4-py39h28c39a1_0.conda#1b07000dc6aed4a69e91107dac4464d3
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/typer-slim-standard-0.12.3-hd8ed1ab_0.conda#8e56b98837d17e6ace4dc455d905709a
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.3-py39h5b4affa_0.conda#20fd617b1f9fcefe5ec1577d38ae7bdb
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.2.1-py39h0ca7971_0.conda#a4c478d3b64c81d1742dc8073e4996b6
-https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.1-py39haf03413_0.conda#d29dc35b665029951dae988810f84508
+https://conda.anaconda.org/conda-forge/osx-64/pandas-2.2.2-py39haf03413_0.conda#11225cf1f769af217ffc01f0a21d40fa
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.13.0-py39h0ed1e0f_0.conda#3a4d0af4fe2006bedc33ca61e9a0b4d6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.8.4-py39h7070ae8_0.conda#cb9e1f8aff1f759b9685e908f9dc0a5b
 https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.5-nompi_py39h824b2b2_100.conda#07525171115894fe9c4aba755460c51a
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.8.4-py39h6e9494a_0.conda#371fe0f738d9f3baa20cf06656b78b0a
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
```

### Comparing `eradiate-0.27.0rc0/requirements/conda/environment-tests-win-64.lock` & `eradiate-0.27.0rc1/requirements/conda/environment-tests-win-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: 1cfc82e59fcdda1546c52710854826406018e832b12de9ff3d9e51d5d62d28e8
+# input_hash: 40a0ea0203d23a0d7fb4cf7c57579a39336674e7df32304246cd7771e4210818
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda#63da060240ab8087b60d1357051ea7d6
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda#30ebb9fd99666d8b8675fcee541a09f3
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda#c66eb2fd33b999ccc258aef85689758e
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-0.22.5-h5728263_2.conda#75a6982b9ff0a8db0f53303527b07af8
 https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2#b0309b72560df66f71a9d5e34a5efdfa
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.9-4_cp39.conda#948b0d93d4ab1372d8fd45e1560afd47
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda#161081fc7cec0bfda0d86d7cb595f8d8
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/libasprintf-devel-0.22.5-h5728263_2.conda#8377da2cc31200d7181d2e48d60e4c7b
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2#53a1c73e1e3d185516d7e3af177596d9
@@ -22,16 +22,16 @@
 https://conda.anaconda.org/conda-forge/win-64/libaec-1.1.3-h63175ca_0.conda#8723000f6ffdbdaef16025f0a01b64c5
 https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.1.0-hcfcfb64_1.conda#f77f319fb82980166569e1280d5b2864
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.20-hcfcfb64_0.conda#b12b5bde5eb201a1df75e49320cc938a
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda#e1eb10b1cca179f2baa3601e4efc8712
 https://conda.anaconda.org/conda-forge/win-64/libjpeg-turbo-3.0.0-hcfcfb64_1.conda#3f1b948619c45b1ca714d60c7389092c
 https://conda.anaconda.org/conda-forge/win-64/libogg-1.3.4-h8ffe710_1.tar.bz2#04286d905a0dcb7f7d4a12bdfe02516d
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda#f95359f8dc5abf7da7776ece9ef10bc5
-https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.2-hcfcfb64_1.conda#fdf80cb33c32d4d002bb89c37cfff5b7
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda#73f5dc8e2d55d9a1e14b11f49c3b4a28
+https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.4.0-hcfcfb64_0.conda#abd61d0ab127ec5cd68f62c2969e6f34
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda#958e0418e93e50c575bff70fbcaa12d8
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
 https://conda.anaconda.org/conda-forge/win-64/snappy-1.2.0-hfb803bf_1.conda#a419bf04a7c76a46639e315ac1b8bf72
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda#fc048363eb8f03cd1737600a5d08aafe
@@ -40,15 +40,15 @@
 https://conda.anaconda.org/conda-forge/win-64/krb5-1.21.2-heb0366b_0.conda#6e8b0f22b4eef3b3cb3849bb4c3d47f9
 https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.1.0-hcfcfb64_1.conda#19ce3e1dacc7912b3d6ff40690ba9ae0
 https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.1.0-hcfcfb64_1.conda#71e890a0b361fd58743a13f77e1506b7
 https://conda.anaconda.org/conda-forge/win-64/libintl-0.22.5-h5728263_2.conda#aa622c938af057adc119f8b8eecada01
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.43-h19919ed_0.conda#77e398acc32617a0384553aea29e866b
 https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
 https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2#e1a22282de0169c93e4ffe6ce6acc212
-https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_1.conda#eb9f59dd51f50f5aa369813fa63ba569
+https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_2.conda#ac7af7a949db01dae61ddc48f4a93d79
 https://conda.anaconda.org/conda-forge/win-64/libzip-1.10.1-h1d365fa_3.conda#5c629cd12d89e2856c17b1dc5fcf44a4
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.43-h17e33f8_0.conda#d0485b8aa2cedb141a7bd27b4efa4c9c
 https://conda.anaconda.org/conda-forge/win-64/python-3.9.19-h4de0772_0_cpython.conda#b6999bc275e0e6beae7b1c8ea0be1e85
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda#792bb5da68bf0a6cac6a6072ecb8dbeb
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
@@ -61,73 +61,73 @@
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda#7f4a9e3fcff3f6356ae99244a014da6a
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda#5cd86562580f274031ede6aa6aa24441
 https://conda.anaconda.org/conda-forge/noarch/dynaconf-3.2.5-pyhd8ed1ab_0.conda#d0ea2f2c4cb3ccff052ee0c5fc807d6e
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda#8d652ea2ee8eaee02ed8dc820bc794aa
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-hdaf720e_2.conda#3761b23693f768dc75a8fd0a73ca053f
 https://conda.anaconda.org/conda-forge/win-64/gettext-tools-0.22.5-h7d00a51_2.conda#ef1c3bb48c013099c4872640a5f2096c
-https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda#1a76f09108576397c41c0b0c5bd84134
+https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda#c0cc1420498b17414d8617d0b9f506ca
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.5-py39h1f6ef14_1.conda#4fc5bd0a7b535252028c647cc27d6c87
 https://conda.anaconda.org/conda-forge/win-64/libclang13-18.1.3-default_hf64faad_0.conda#9217c37b478ec601af909aafc954a6fc
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.7.1-hd5e4a3a_0.conda#3396aff340d0903e8814c2852d631e4e
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-0.22.5-h5728263_2.conda#f4c826b19bf1ccee2a63a2c685039728
-https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_4.conda#9baf04fc7002450a932cf97cb9625ebb
-https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda#87da045f6d26ce9fe20ad76a18f6a18a
+https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_6.conda#cd5c6efbe213c089f78575c98ab9a0ed
+https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda#ee944f0d41d9e2048f9d7492c1623ca3
 https://conda.anaconda.org/conda-forge/win-64/libintl-devel-0.22.5-h5728263_2.conda#a2ad82fae23975e4ccbfab2847d31d48
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.6.0-hddb2be6_3.conda#6d1828c9039929e2f185c5fa9d133018
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda#776a8dd9e824f77abac30e6ef43a8f7a
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda#248f521b64ce055e7feae3105e7abeb8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda#a0bc3eec34b0fab84be6b2da94e98e20
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda#139e9feb65187e916162917bb2484976
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda#d478a8a3044cdff1aa6e62f9269cefe0
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda#d3483c8fc2dc2cc3f5cf43e26d60cabf
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda#18c6deb6f9602e32446398203c8f0e91
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda#140a7f159396547e9799aa98f9f0742e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda#b9a4dacf97241704529131a0dfc0494f
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda#98206ea9954216ee7540f0c773f2104d
 https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda#3eeeeb9e4827ace8c0c1419c85d590ad
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.8-py39ha55989b_0.conda#07aae1fdd812b411cec84c0d47339d22
-https://conda.anaconda.org/conda-forge/noarch/setuptools-69.2.0-pyhd8ed1ab_0.conda#da214ecd521a720a9d521c68047682dc
+https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda#7462280d81f639363e6e63c81276bd9e
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda#d08db09a552699ee9e7eec56b4eb3899
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py39ha55989b_0.conda#d8f52e8e1d02f9a5901f9224e2ddf98f
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda#6ef2fc37559256cf682d8b3375e89b80
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.1.0-py39ha55989b_0.conda#20ec896e8d97f2ff8be1124e624dc8f2
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda#2e4d6bc0b14e10f895fc6791a7d9b26a
 https://conda.anaconda.org/conda-forge/win-64/brotli-1.1.0-hcfcfb64_1.conda#f47f6db2528e38321fb00ae31674c133
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda#3549ecbceb6cd77b91a105511b7d0786
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-24.1.0-py_0.tar.bz2#7c034fc39ac52936640aecab2d7fa0d7
-https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_4.conda#44cd44c004db728bf5788c1d46ce7334
+https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_6.conda#40d452e4012c00f644b1dd6319fcdbcf
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.14.3-nompi_h73e8ff5_100.conda#1e91ce0f3a914b0dab762539c0df4ff1
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda#0896606848b2dc5cebdf111b6543aa04
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda#c5d3907ad8bd7bf557521a1833cf7e6d
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.16-h67d730c_0.conda#d3592435917b62a8becff3a60db674f6
 https://conda.anaconda.org/conda-forge/win-64/libgettextpo-devel-0.22.5-h5728263_2.conda#6f42ec61abc6d52a4079800a640319c5
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.15-hcd874cb_0.conda#090d91b69396f14afef450c285f9758c
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda#7e7099ad94ac3b599808950cec30ad4e
 https://conda.anaconda.org/conda-forge/noarch/pint-0.23-pyhd8ed1ab_0.conda#d47f9170e3933e53368e0d447c16856f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
-https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda#94ff09cdedcb7b17e9cd5097ee2cfcff
+https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda#088ff7e08f4f10a06190468048c2a353
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda#2cf4264fffb9e6eff6031c5b6884d61c
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.18.6-py39ha55989b_0.conda#7839645d467f5d3bc52709a3d484fa62
 https://conda.anaconda.org/conda-forge/win-64/sip-6.7.12-py39h99910a6_0.conda#0cc5774390ada632ed7975203057c91c
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda#21069f3ed16812f9f4f2700667b6ec86
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda#21745fdd12f01b41178596143cbecffd
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.66.2-pyhd8ed1ab_0.conda#2b8dfb969f984497f3f98409a9545776
 https://conda.anaconda.org/conda-forge/noarch/typing_inspect-0.9.0-pyhd8ed1ab_0.conda#9e924b76b91908a17e28a19a0ab88687
 https://conda.anaconda.org/conda-forge/win-64/fonttools-4.51.0-py39ha55989b_0.conda#5d19302bab29e347116b743e793aa7d6
 https://conda.anaconda.org/conda-forge/win-64/gettext-0.22.5-h5728263_2.conda#da84216f88a8c89eb943c683ceb34d7d
-https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_4.conda#d0a05e8a76abb68b2beb7b16c6d49213
+https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_6.conda#a4036d0bc6f499ebe9fef7b887f3ca0f
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-6.4.0-pyhd8ed1ab_0.conda#dcbadab7a68738a028e195ab68ab2d2e
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda#a284ff318fbdb0dd83928275b4b6087c
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.9.2-nompi_h07c049d_113.conda#2aa431a5a05e3679eea4faad0f47b119
 https://conda.anaconda.org/conda-forge/win-64/mkl-2024.1.0-h66d3029_692.conda#b43ec7ed045323edeff31e348eea8652
 https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py39h9ee4981_0.conda#6d69d57c41867acc162ef0205a8efaef
 https://conda.anaconda.org/eradiate/noarch/pinttrs-24.1.0-py_0.tar.bz2#c51f4806cf84fbf9578b7ce8e8462b20
 https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.12.2-py39h99910a6_5.conda#dffbcea794c524c471772a5f697c2aea
@@ -145,17 +145,17 @@
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-22_win64_mkl.conda#c752cc2af9f3d8d7b2fdebb915a33ef7
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.8.1-pyhd8ed1ab_0.conda#d15917f33140f8d2ac9ca44db7ec8a25
 https://conda.anaconda.org/conda-forge/noarch/typer-0.12.3-pyhd8ed1ab_0.conda#10efd02b22c39c0a46312ef7cb16d237
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.26.4-py39hddb5d58_0.conda#6e30ff8f2d3f59f45347dfba8bc22a04
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-hcef0176_21.conda#76544d3dfeff8fd52250df168cb0005b
 https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.3-py39hd88c2e4_0.conda#12e356a0e7e5a8e67538aa66fbd21c47
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.2.1-py39h1f6ef14_0.conda#03e25c6bae87f4f9595337255b44b0fb
-https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.1-py39h32e6231_0.conda#7ca03abc7f2f9c91a9fdc02780bfa572
+https://conda.anaconda.org/conda-forge/win-64/pandas-2.2.2-py39h32e6231_0.conda#0df69e098aa54373d4edb3eaaa2338ba
 https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.9-py39hb77abff_5.conda#5ed899124a51958336371ff01482b8fd
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.13.0-py39hddb5d58_0.conda#cfe749056fb9ed9dbc096b5751becf34
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.8.4-py39hf19769e_0.conda#7836c3dc5814f6d55a7392657c576e88
 https://conda.anaconda.org/conda-forge/win-64/netcdf4-1.6.5-nompi_py39h9a3bb69_100.conda#e271773571fa2908d8fd598878890db2
-https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.56.0-pyhd8ed1ab_0.conda#6609c4a3b9196b61cea661796cdb86d9
+https://conda.anaconda.org/conda-forge/noarch/sf-hamilton-1.59.1-pyhd8ed1ab_0.conda#d41dba17d7ef879c349f4656d049d2e4
 https://conda.anaconda.org/conda-forge/noarch/xarray-2024.3.0-pyhd8ed1ab_0.conda#772d7ee42b65d0840130eabd5bd3fc17
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.8.4-py39hcbf5309_0.conda#cc66c372d5eb745665da06ce56b7d72b
 https://conda.anaconda.org/conda-forge/noarch/ussa1976-0.3.4-pyhd8ed1ab_0.conda#c29c9ce2a92397b9c579c29b01c25248
 https://conda.anaconda.org/conda-forge/noarch/joseki-2.6.1-pyhd8ed1ab_0.conda#9254772a1cbda17955d0b4890a73984f
```

### Comparing `eradiate-0.27.0rc0/requirements/copy_envvars.py` & `eradiate-0.27.0rc1/requirements/copy_envvars.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/requirements/layered.yml` & `eradiate-0.27.0rc1/requirements/layered.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
   packages:
     - "aenum"
     - "attrs>=22.2"
     - "cachetools>=5.3"
     - "click"
     - "dessinemoi>=23.1.0"
     - "dynaconf>=3.2"
-    - "importlib_resources"
     - "joseki>=2.6.0"
     - "lazy_loader>=0.1"
     - "matplotlib>=3.3"
     - "netcdf4"
     - "numpy"
     - "pint"
     - "pinttrs>=23.2.0"
@@ -50,14 +49,15 @@
 docs:
   includes:
     - main
   packages:
     - "autodocsumm"
     - "myst-parser"
     - "nbsphinx>=0.9.0"
+    - "seaborn"
     - "sphinx-book-theme>=1.0"
     - "sphinx"
     - "sphinxcontrib-bibtex>=2.0"
     - "sphinx-autobuild"
     - "sphinx-copybutton"
     - "sphinx-design"
```

### Comparing `eradiate-0.27.0rc0/requirements/make_conda_env.py` & `eradiate-0.27.0rc1/requirements/make_conda_env.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/requirements/make_pip_in_files.py` & `eradiate-0.27.0rc1/requirements/make_pip_in_files.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/requirements/make_pip_txt_files.py` & `eradiate-0.27.0rc1/requirements/make_pip_txt_files.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/requirements/pip/dependencies.lock.txt` & `eradiate-0.27.0rc1/requirements/pip/dependencies.lock.txt`

 * *Files 4% similar despite different names*

```diff
@@ -55,30 +55,29 @@
     # via
     #   -c requirements/pip/optional.lock.txt
     #   eradiate-mitsuba
 dynaconf==3.2.5
     # via
     #   -c requirements/pip/optional.lock.txt
     #   -r requirements/pip/main.in
-eradiate-mitsuba==0.2.0
+eradiate-mitsuba==0.2.1
     # via
     #   -c requirements/pip/optional.lock.txt
     #   -r requirements/pip/dependencies.in
 fonttools==4.51.0
     # via
     #   -c requirements/pip/optional.lock.txt
     #   matplotlib
-idna==3.6
+idna==3.7
     # via
     #   -c requirements/pip/optional.lock.txt
     #   requests
 importlib-resources==6.4.0
     # via
     #   -c requirements/pip/optional.lock.txt
-    #   -r requirements/pip/main.in
     #   joseki
     #   matplotlib
 joseki==2.6.1
     # via
     #   -c requirements/pip/optional.lock.txt
     #   -r requirements/pip/main.in
 kiwisolver==1.4.5
@@ -128,15 +127,15 @@
 packaging==24.0
     # via
     #   -c requirements/pip/optional.lock.txt
     #   lazy-loader
     #   matplotlib
     #   pooch
     #   xarray
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   -c requirements/pip/optional.lock.txt
     #   joseki
     #   sf-hamilton
     #   xarray
 pillow==10.3.0
     # via
@@ -148,15 +147,15 @@
     #   -r requirements/pip/main.in
     #   joseki
     #   pinttrs
 pinttrs==24.1.0
     # via
     #   -c requirements/pip/optional.lock.txt
     #   -r requirements/pip/main.in
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   -c requirements/pip/optional.lock.txt
     #   pooch
 pooch==1.8.1
     # via
     #   -c requirements/pip/optional.lock.txt
     #   -r requirements/pip/main.in
@@ -196,15 +195,15 @@
     #   ruamel-yaml
 scipy==1.13.0
     # via
     #   -c requirements/pip/optional.lock.txt
     #   -r requirements/pip/main.in
     #   joseki
     #   ussa1976
-sf-hamilton==1.57.0
+sf-hamilton==1.59.1
     # via
     #   -c requirements/pip/optional.lock.txt
     #   -r requirements/pip/main.in
 shellingham==1.5.4
     # via
     #   -c requirements/pip/optional.lock.txt
     #   -r requirements/pip/main.in
```

### Comparing `eradiate-0.27.0rc0/requirements/pip/dev.lock.txt` & `eradiate-0.27.0rc1/requirements/pip/dev.lock.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,27 @@
     # via sphinx
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   jupyter-server
+    #   starlette
+    #   watchfiles
 appdirs==1.4.4
     # via ensureconda
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 astropy==6.0.1
     # via -r requirements/pip/recommended.in
-astropy-iers-data==0.2024.4.8.0.32.4
+astropy-iers-data==0.2024.4.29.0.28.48
     # via astropy
 asttokens==2.4.1
     # via stack-data
 async-lru==2.0.4
     # via jupyterlab
 attrs==23.2.0
     # via
@@ -48,15 +50,15 @@
 autodocsumm==0.2.12
     # via -r requirements/pip/docs.in
 babel==2.14.0
     # via
     #   jupyterlab-server
     #   pydata-sphinx-theme
     #   sphinx
-backports-tarfile==1.0.0
+backports-tarfile==1.1.1
     # via jaraco-context
 beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.1.0
     # via nbconvert
@@ -96,14 +98,15 @@
     #   click-default-group
     #   conda-lock
     #   ensureconda
     #   joseki
     #   pip-tools
     #   typer
     #   ussa1976
+    #   uvicorn
 click-default-group==1.2.4
     # via conda-lock
 clikit==0.6.2
     # via conda-lock
 colorama==0.4.6
     # via sphinx-autobuild
 comm==0.2.2
@@ -134,29 +137,29 @@
     # via nbconvert
 dessinemoi==24.1.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 distlib==0.3.8
     # via virtualenv
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinxcontrib-bibtex
 dynaconf==3.2.5
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 ensureconda==1.4.4
     # via conda-lock
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   anyio
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
@@ -172,22 +175,24 @@
     #   -c requirements/pip/main.lock.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
 graphviz==0.20.3
     # via -r requirements/pip/recommended.in
 h11==0.14.0
-    # via httpcore
+    # via
+    #   httpcore
+    #   uvicorn
 html5lib==1.1
     # via conda-lock
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
     # via jupyterlab
-idna==3.6
+idna==3.7
     # via
     #   -c requirements/pip/main.lock.txt
     #   anyio
     #   httpx
     #   jsonschema
     #   requests
 imagesize==1.4.1
@@ -202,15 +207,14 @@
     #   keyring
     #   nbconvert
     #   sphinx
     #   sphinxcontrib-bibtex
 importlib-resources==6.4.0
     # via
     #   -c requirements/pip/main.lock.txt
-    #   -r requirements/pip/main.in
     #   joseki
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
 ipykernel==6.29.4
     # via jupyterlab
 ipython==8.18.1
@@ -222,15 +226,15 @@
     # via -r requirements/pip/recommended.in
 isoduration==20.11.0
     # via jsonschema
 jaraco-classes==3.4.0
     # via keyring
 jaraco-context==5.3.0
     # via keyring
-jaraco-functools==4.0.0
+jaraco-functools==4.0.1
     # via keyring
 jedi==0.19.1
     # via ipython
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
@@ -244,15 +248,15 @@
     #   nbconvert
     #   nbsphinx
     #   sphinx
 joseki==2.6.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
-json5==0.9.24
+json5==0.9.25
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.21.1
     # via
     #   jupyter-events
     #   jupyterlab-server
@@ -273,44 +277,42 @@
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyter-events==0.10.0
     # via jupyter-server
 jupyter-lsp==2.2.5
     # via jupyterlab
-jupyter-server==2.13.0
+jupyter-server==2.14.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
 jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.1.6
+jupyterlab==4.1.8
     # via -r requirements/pip/recommended.in
 jupyterlab-pygments==0.3.0
     # via nbconvert
-jupyterlab-server==2.26.0
+jupyterlab-server==2.27.1
     # via jupyterlab
 jupyterlab-widgets==3.0.10
     # via ipywidgets
-keyring==25.1.0
+keyring==25.2.0
     # via conda-lock
 kiwisolver==1.4.5
     # via
     #   -c requirements/pip/main.lock.txt
     #   matplotlib
 latexcodec==3.0.0
     # via pybtex
 lazy-loader==0.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
-livereload==2.6.3
-    # via sphinx-autobuild
 markdown-it-py==3.0.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   mdit-py-plugins
     #   myst-parser
     #   rich
 markupsafe==2.1.5
@@ -318,15 +320,15 @@
     #   jinja2
     #   nbconvert
 matplotlib==3.8.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
     #   seaborn
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via
@@ -340,15 +342,15 @@
     #   jaraco-functools
 msgpack==1.0.8
     # via cachecontrol
 mypy-extensions==1.0.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   typing-inspect
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via -r requirements/pip/docs.in
 nbclient==0.10.0
     # via nbconvert
 nbconvert==7.16.3
     # via
     #   jupyter-server
     #   nbsphinx
@@ -406,15 +408,15 @@
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
     #   xarray
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   joseki
     #   seaborn
     #   sf-hamilton
     #   xarray
 pandocfilters==1.5.1
@@ -439,21 +441,21 @@
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 pip-tools==7.4.1
     # via -r requirements/pip/dev.in
 pkginfo==1.10.0
     # via conda-lock
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   jupyter-core
     #   pooch
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pooch==1.8.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 prometheus-client==0.20.0
     # via jupyter-server
@@ -471,21 +473,21 @@
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
 pybtex-docutils==1.0.3
     # via sphinxcontrib-bibtex
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.1
     # via conda-lock
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
-pyerfa==2.0.1.3
+pyerfa==2.0.1.4
     # via astropy
 pygments==2.17.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   accessible-pygments
     #   ipython
     #   nbconvert
@@ -494,19 +496,19 @@
     #   sphinx
 pylev==1.4.0
     # via clikit
 pyparsing==3.1.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   matplotlib
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
     # via -r requirements/pip/tests.in
 pytest-metadata==3.1.1
@@ -528,20 +530,20 @@
 pyyaml==6.0.1
     # via
     #   astropy
     #   conda-lock
     #   jupyter-events
     #   myst-parser
     #   pybtex
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   jupyter-events
 requests==2.31.0
     # via
     #   -c requirements/pip/main.lock.txt
@@ -580,59 +582,60 @@
 scipy==1.13.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
     #   joseki
     #   ussa1976
 seaborn==0.13.2
-    # via -r requirements/pip/recommended.in
+    # via
+    #   -r requirements/pip/docs.in
+    #   -r requirements/pip/recommended.in
 secretstorage==3.3.3
     # via keyring
 send2trash==1.8.3
     # via jupyter-server
-sf-hamilton==1.57.0
+sf-hamilton==1.59.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 shellingham==1.5.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
     #   typer
 six==1.16.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   asttokens
     #   bleach
     #   html5lib
-    #   livereload
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r requirements/pip/docs.in
     #   autodocsumm
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-book-theme
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinxcontrib-bibtex
-sphinx-autobuild==2024.2.4
+sphinx-autobuild==2024.4.16
     # via -r requirements/pip/docs.in
 sphinx-book-theme==1.1.2
     # via -r requirements/pip/docs.in
 sphinx-copybutton==0.5.2
     # via -r requirements/pip/docs.in
 sphinx-design==0.5.0
     # via -r requirements/pip/docs.in
@@ -648,45 +651,46 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 stack-data==0.6.3
     # via ipython
+starlette==0.37.2
+    # via sphinx-autobuild
 terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
-tinycss2==1.2.1
+tinycss2==1.3.0
     # via nbconvert
 tomli==2.0.1
     # via
     #   build
     #   conda-lock
     #   jupyterlab
     #   pip-tools
-    #   pyproject-hooks
     #   pytest
+    #   sphinx
 tomlkit==0.12.4
     # via conda-lock
 toolz==0.12.1
     # via conda-lock
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
-    #   livereload
     #   terminado
 tqdm==4.66.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
-traitlets==5.14.2
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
@@ -712,16 +716,18 @@
     #   conda-lock
     #   ipython
     #   pint
     #   pydantic
     #   pydantic-core
     #   pydata-sphinx-theme
     #   sf-hamilton
+    #   starlette
     #   typer
     #   typing-inspect
+    #   uvicorn
 typing-inspect==0.9.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   sf-hamilton
 tzdata==2024.1
     # via
     #   -c requirements/pip/main.lock.txt
@@ -732,27 +738,33 @@
     # via
     #   -c requirements/pip/main.lock.txt
     #   requests
 ussa1976==0.3.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   joseki
-virtualenv==20.25.1
+uvicorn==0.29.0
+    # via sphinx-autobuild
+virtualenv==20.26.0
     # via conda-lock
+watchfiles==0.21.0
+    # via sphinx-autobuild
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   html5lib
     #   tinycss2
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via jupyter-server
+websockets==12.0
+    # via sphinx-autobuild
 wheel==0.43.0
     # via pip-tools
 widgetsnbextension==4.0.10
     # via ipywidgets
 xarray==2024.3.0
     # via
     #   -c requirements/pip/main.lock.txt
@@ -766,11 +778,11 @@
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via
     #   -r requirements/pip/dev.in
     #   pip-tools
-setuptools==69.2.0
+setuptools==69.5.1
     # via
     #   -r requirements/pip/dev.in
     #   pip-tools
```

### Comparing `eradiate-0.27.0rc0/requirements/pip/docs.lock.txt` & `eradiate-0.27.0rc1/requirements/pip/docs.lock.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
 aenum==3.1.15
     # via -r requirements/pip/main.in
 alabaster==0.7.16
     # via sphinx
+anyio==4.3.0
+    # via
+    #   starlette
+    #   watchfiles
 attrs==23.2.0
     # via
     #   -r requirements/pip/main.in
     #   dessinemoi
     #   joseki
     #   jsonschema
     #   pinttrs
@@ -42,51 +46,57 @@
     # via requests
 click==8.1.7
     # via
     #   -r requirements/pip/main.in
     #   joseki
     #   typer
     #   ussa1976
+    #   uvicorn
 colorama==0.4.6
     # via sphinx-autobuild
 contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 defusedxml==0.7.1
     # via nbconvert
 dessinemoi==24.1.0
     # via -r requirements/pip/main.in
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinxcontrib-bibtex
 dynaconf==3.2.5
     # via -r requirements/pip/main.in
+exceptiongroup==1.2.1
+    # via anyio
 fastjsonschema==2.19.1
     # via nbformat
 fonttools==4.51.0
     # via matplotlib
-idna==3.6
-    # via requests
+h11==0.14.0
+    # via uvicorn
+idna==3.7
+    # via
+    #   anyio
+    #   requests
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==7.1.0
     # via
     #   jupyter-client
     #   nbconvert
     #   sphinx
     #   sphinxcontrib-bibtex
 importlib-resources==6.4.0
     # via
-    #   -r requirements/pip/main.in
     #   joseki
     #   matplotlib
 jinja2==3.1.3
     # via
     #   myst-parser
     #   nbconvert
     #   nbsphinx
@@ -109,36 +119,36 @@
     # via nbconvert
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 lazy-loader==0.4
     # via -r requirements/pip/main.in
-livereload==2.6.3
-    # via sphinx-autobuild
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
     #   rich
 markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
 matplotlib==3.8.4
-    # via -r requirements/pip/main.in
+    # via
+    #   -r requirements/pip/main.in
+    #   seaborn
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.2
     # via nbconvert
 mypy-extensions==1.0.0
     # via typing-inspect
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via -r requirements/pip/docs.in
 nbclient==0.10.0
     # via nbconvert
 nbconvert==7.16.3
     # via nbsphinx
 nbformat==5.10.4
     # via
@@ -158,43 +168,45 @@
     #   cftime
     #   contourpy
     #   joseki
     #   matplotlib
     #   netcdf4
     #   pandas
     #   scipy
+    #   seaborn
     #   sf-hamilton
     #   ussa1976
     #   xarray
 packaging==24.0
     # via
     #   lazy-loader
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   sphinx
     #   xarray
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   joseki
+    #   seaborn
     #   sf-hamilton
     #   xarray
 pandocfilters==1.5.1
     # via nbconvert
 pillow==10.3.0
     # via matplotlib
 pint==0.23
     # via
     #   -r requirements/pip/main.in
     #   joseki
     #   pinttrs
 pinttrs==24.1.0
     # via -r requirements/pip/main.in
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   jupyter-core
     #   pooch
 pooch==1.8.1
     # via -r requirements/pip/main.in
 pybtex==0.24.0
     # via
@@ -220,17 +232,17 @@
     #   pandas
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   myst-parser
     #   pybtex
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via jupyter-client
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   pooch
     #   sphinx
@@ -247,43 +259,46 @@
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 scipy==1.13.0
     # via
     #   -r requirements/pip/main.in
     #   joseki
     #   ussa1976
-sf-hamilton==1.57.0
+seaborn==0.13.2
+    # via -r requirements/pip/docs.in
+sf-hamilton==1.59.1
     # via -r requirements/pip/main.in
 shellingham==1.5.4
     # via
     #   -r requirements/pip/main.in
     #   typer
 six==1.16.0
     # via
     #   bleach
-    #   livereload
     #   pybtex
     #   python-dateutil
+sniffio==1.3.1
+    # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r requirements/pip/docs.in
     #   autodocsumm
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-book-theme
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinxcontrib-bibtex
-sphinx-autobuild==2024.2.4
+sphinx-autobuild==2024.4.16
     # via -r requirements/pip/docs.in
 sphinx-book-theme==1.1.2
     # via -r requirements/pip/docs.in
 sphinx-copybutton==0.5.2
     # via -r requirements/pip/docs.in
 sphinx-design==0.5.0
     # via -r requirements/pip/docs.in
@@ -297,51 +312,62 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-tinycss2==1.2.1
+starlette==0.37.2
+    # via sphinx-autobuild
+tinycss2==1.3.0
     # via nbconvert
+tomli==2.0.1
+    # via sphinx
 tornado==6.4
-    # via
-    #   jupyter-client
-    #   livereload
+    # via jupyter-client
 tqdm==4.66.2
     # via -r requirements/pip/main.in
-traitlets==5.14.2
+traitlets==5.14.3
     # via
     #   jupyter-client
     #   jupyter-core
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
 typer==0.12.3
     # via -r requirements/pip/main.in
 typing-extensions==4.11.0
     # via
+    #   anyio
     #   pint
     #   pydata-sphinx-theme
     #   sf-hamilton
+    #   starlette
     #   typer
     #   typing-inspect
+    #   uvicorn
 typing-inspect==0.9.0
     # via sf-hamilton
 tzdata==2024.1
     # via pandas
 urllib3==2.2.1
     # via requests
 ussa1976==0.3.4
     # via joseki
+uvicorn==0.29.0
+    # via sphinx-autobuild
+watchfiles==0.21.0
+    # via sphinx-autobuild
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
+websockets==12.0
+    # via sphinx-autobuild
 xarray==2024.3.0
     # via
     #   -r requirements/pip/main.in
     #   joseki
     #   ussa1976
 zipp==3.18.1
     # via
```

### Comparing `eradiate-0.27.0rc0/requirements/pip/main.lock.txt` & `eradiate-0.27.0rc1/requirements/pip/main.lock.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,19 +34,18 @@
     # via matplotlib
 dessinemoi==24.1.0
     # via -r requirements/pip/main.in
 dynaconf==3.2.5
     # via -r requirements/pip/main.in
 fonttools==4.51.0
     # via matplotlib
-idna==3.6
+idna==3.7
     # via requests
 importlib-resources==6.4.0
     # via
-    #   -r requirements/pip/main.in
     #   joseki
     #   matplotlib
 joseki==2.6.1
     # via -r requirements/pip/main.in
 kiwisolver==1.4.5
     # via matplotlib
 lazy-loader==0.4
@@ -79,29 +78,29 @@
     #   xarray
 packaging==24.0
     # via
     #   lazy-loader
     #   matplotlib
     #   pooch
     #   xarray
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   joseki
     #   sf-hamilton
     #   xarray
 pillow==10.3.0
     # via matplotlib
 pint==0.23
     # via
     #   -r requirements/pip/main.in
     #   joseki
     #   pinttrs
 pinttrs==24.1.0
     # via -r requirements/pip/main.in
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via pooch
 pooch==1.8.1
     # via -r requirements/pip/main.in
 pygments==2.17.2
     # via rich
 pyparsing==3.1.2
     # via matplotlib
@@ -122,15 +121,15 @@
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 scipy==1.13.0
     # via
     #   -r requirements/pip/main.in
     #   joseki
     #   ussa1976
-sf-hamilton==1.57.0
+sf-hamilton==1.59.1
     # via -r requirements/pip/main.in
 shellingham==1.5.4
     # via
     #   -r requirements/pip/main.in
     #   typer
 six==1.16.0
     # via python-dateutil
```

### Comparing `eradiate-0.27.0rc0/requirements/pip/optional.lock.txt` & `eradiate-0.27.0rc1/requirements/pip/optional.lock.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,27 @@
     # via sphinx
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   jupyter-server
+    #   starlette
+    #   watchfiles
 appdirs==1.4.4
     # via ensureconda
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 astropy==6.0.1
     # via -r requirements/pip/recommended.in
-astropy-iers-data==0.2024.4.8.0.32.4
+astropy-iers-data==0.2024.4.29.0.28.48
     # via astropy
 asttokens==2.4.1
     # via stack-data
 async-lru==2.0.4
     # via jupyterlab
 attrs==23.2.0
     # via
@@ -48,15 +50,15 @@
 autodocsumm==0.2.12
     # via -r requirements/pip/docs.in
 babel==2.14.0
     # via
     #   jupyterlab-server
     #   pydata-sphinx-theme
     #   sphinx
-backports-tarfile==1.0.0
+backports-tarfile==1.1.1
     # via jaraco-context
 beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.1.0
     # via nbconvert
@@ -96,14 +98,15 @@
     #   click-default-group
     #   conda-lock
     #   ensureconda
     #   joseki
     #   pip-tools
     #   typer
     #   ussa1976
+    #   uvicorn
 click-default-group==1.2.4
     # via conda-lock
 clikit==0.6.2
     # via conda-lock
 colorama==0.4.6
     # via sphinx-autobuild
 comm==0.2.2
@@ -134,15 +137,15 @@
     # via nbconvert
 dessinemoi==24.1.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 distlib==0.3.8
     # via virtualenv
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinxcontrib-bibtex
@@ -150,17 +153,17 @@
     # via eradiate-mitsuba
 dynaconf==3.2.5
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 ensureconda==1.4.4
     # via conda-lock
-eradiate-mitsuba==0.2.0
+eradiate-mitsuba==0.2.1
     # via -r requirements/pip/optional.in
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   anyio
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
@@ -176,22 +179,24 @@
     #   -c requirements/pip/main.lock.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
 graphviz==0.20.3
     # via -r requirements/pip/recommended.in
 h11==0.14.0
-    # via httpcore
+    # via
+    #   httpcore
+    #   uvicorn
 html5lib==1.1
     # via conda-lock
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
     # via jupyterlab
-idna==3.6
+idna==3.7
     # via
     #   -c requirements/pip/main.lock.txt
     #   anyio
     #   httpx
     #   jsonschema
     #   requests
 imagesize==1.4.1
@@ -206,15 +211,14 @@
     #   keyring
     #   nbconvert
     #   sphinx
     #   sphinxcontrib-bibtex
 importlib-resources==6.4.0
     # via
     #   -c requirements/pip/main.lock.txt
-    #   -r requirements/pip/main.in
     #   joseki
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
 ipykernel==6.29.4
     # via jupyterlab
 ipython==8.18.1
@@ -226,15 +230,15 @@
     # via -r requirements/pip/recommended.in
 isoduration==20.11.0
     # via jsonschema
 jaraco-classes==3.4.0
     # via keyring
 jaraco-context==5.3.0
     # via keyring
-jaraco-functools==4.0.0
+jaraco-functools==4.0.1
     # via keyring
 jedi==0.19.1
     # via ipython
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
@@ -248,15 +252,15 @@
     #   nbconvert
     #   nbsphinx
     #   sphinx
 joseki==2.6.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
-json5==0.9.24
+json5==0.9.25
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.21.1
     # via
     #   jupyter-events
     #   jupyterlab-server
@@ -277,44 +281,42 @@
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyter-events==0.10.0
     # via jupyter-server
 jupyter-lsp==2.2.5
     # via jupyterlab
-jupyter-server==2.13.0
+jupyter-server==2.14.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
 jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.1.6
+jupyterlab==4.1.8
     # via -r requirements/pip/recommended.in
 jupyterlab-pygments==0.3.0
     # via nbconvert
-jupyterlab-server==2.26.0
+jupyterlab-server==2.27.1
     # via jupyterlab
 jupyterlab-widgets==3.0.10
     # via ipywidgets
-keyring==25.1.0
+keyring==25.2.0
     # via conda-lock
 kiwisolver==1.4.5
     # via
     #   -c requirements/pip/main.lock.txt
     #   matplotlib
 latexcodec==3.0.0
     # via pybtex
 lazy-loader==0.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
-livereload==2.6.3
-    # via sphinx-autobuild
 markdown-it-py==3.0.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   mdit-py-plugins
     #   myst-parser
     #   rich
 markupsafe==2.1.5
@@ -322,15 +324,15 @@
     #   jinja2
     #   nbconvert
 matplotlib==3.8.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
     #   seaborn
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via
@@ -344,15 +346,15 @@
     #   jaraco-functools
 msgpack==1.0.8
     # via cachecontrol
 mypy-extensions==1.0.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   typing-inspect
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via -r requirements/pip/docs.in
 nbclient==0.10.0
     # via nbconvert
 nbconvert==7.16.3
     # via
     #   jupyter-server
     #   nbsphinx
@@ -410,15 +412,15 @@
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
     #   xarray
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   joseki
     #   seaborn
     #   sf-hamilton
     #   xarray
 pandocfilters==1.5.1
@@ -443,21 +445,21 @@
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 pip-tools==7.4.1
     # via -r requirements/pip/dev.in
 pkginfo==1.10.0
     # via conda-lock
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   jupyter-core
     #   pooch
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pooch==1.8.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 prometheus-client==0.20.0
     # via jupyter-server
@@ -475,21 +477,21 @@
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
 pybtex-docutils==1.0.3
     # via sphinxcontrib-bibtex
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.1
     # via conda-lock
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
-pyerfa==2.0.1.3
+pyerfa==2.0.1.4
     # via astropy
 pygments==2.17.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   accessible-pygments
     #   ipython
     #   nbconvert
@@ -498,19 +500,19 @@
     #   sphinx
 pylev==1.4.0
     # via clikit
 pyparsing==3.1.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   matplotlib
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
     # via -r requirements/pip/tests.in
 pytest-metadata==3.1.1
@@ -532,20 +534,20 @@
 pyyaml==6.0.1
     # via
     #   astropy
     #   conda-lock
     #   jupyter-events
     #   myst-parser
     #   pybtex
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   jupyter-events
 requests==2.31.0
     # via
     #   -c requirements/pip/main.lock.txt
@@ -584,59 +586,60 @@
 scipy==1.13.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
     #   joseki
     #   ussa1976
 seaborn==0.13.2
-    # via -r requirements/pip/recommended.in
+    # via
+    #   -r requirements/pip/docs.in
+    #   -r requirements/pip/recommended.in
 secretstorage==3.3.3
     # via keyring
 send2trash==1.8.3
     # via jupyter-server
-sf-hamilton==1.57.0
+sf-hamilton==1.59.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
 shellingham==1.5.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
     #   typer
 six==1.16.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   asttokens
     #   bleach
     #   html5lib
-    #   livereload
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r requirements/pip/docs.in
     #   autodocsumm
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-book-theme
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinxcontrib-bibtex
-sphinx-autobuild==2024.2.4
+sphinx-autobuild==2024.4.16
     # via -r requirements/pip/docs.in
 sphinx-book-theme==1.1.2
     # via -r requirements/pip/docs.in
 sphinx-copybutton==0.5.2
     # via -r requirements/pip/docs.in
 sphinx-design==0.5.0
     # via -r requirements/pip/docs.in
@@ -652,45 +655,46 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 stack-data==0.6.3
     # via ipython
+starlette==0.37.2
+    # via sphinx-autobuild
 terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
-tinycss2==1.2.1
+tinycss2==1.3.0
     # via nbconvert
 tomli==2.0.1
     # via
     #   build
     #   conda-lock
     #   jupyterlab
     #   pip-tools
-    #   pyproject-hooks
     #   pytest
+    #   sphinx
 tomlkit==0.12.4
     # via conda-lock
 toolz==0.12.1
     # via conda-lock
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
-    #   livereload
     #   terminado
 tqdm==4.66.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   -r requirements/pip/main.in
-traitlets==5.14.2
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
@@ -716,16 +720,18 @@
     #   conda-lock
     #   ipython
     #   pint
     #   pydantic
     #   pydantic-core
     #   pydata-sphinx-theme
     #   sf-hamilton
+    #   starlette
     #   typer
     #   typing-inspect
+    #   uvicorn
 typing-inspect==0.9.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   sf-hamilton
 tzdata==2024.1
     # via
     #   -c requirements/pip/main.lock.txt
@@ -736,27 +742,33 @@
     # via
     #   -c requirements/pip/main.lock.txt
     #   requests
 ussa1976==0.3.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   joseki
-virtualenv==20.25.1
+uvicorn==0.29.0
+    # via sphinx-autobuild
+virtualenv==20.26.0
     # via conda-lock
+watchfiles==0.21.0
+    # via sphinx-autobuild
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   html5lib
     #   tinycss2
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via jupyter-server
+websockets==12.0
+    # via sphinx-autobuild
 wheel==0.43.0
     # via pip-tools
 widgetsnbextension==4.0.10
     # via ipywidgets
 xarray==2024.3.0
     # via
     #   -c requirements/pip/main.lock.txt
@@ -770,11 +782,11 @@
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via
     #   -r requirements/pip/dev.in
     #   pip-tools
-setuptools==69.2.0
+setuptools==69.5.1
     # via
     #   -r requirements/pip/dev.in
     #   pip-tools
```

### Comparing `eradiate-0.27.0rc0/requirements/pip/recommended.lock.txt` & `eradiate-0.27.0rc1/requirements/pip/recommended.lock.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 astropy==6.0.1
     # via -r requirements/pip/recommended.in
-astropy-iers-data==0.2024.4.8.0.32.4
+astropy-iers-data==0.2024.4.29.0.28.48
     # via astropy
 asttokens==2.4.1
     # via stack-data
 async-lru==2.0.4
     # via jupyterlab
 attrs==23.2.0
     # via
@@ -61,15 +61,15 @@
     #   matplotlib
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   anyio
     #   ipython
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
@@ -83,15 +83,15 @@
     # via -r requirements/pip/recommended.in
 h11==0.14.0
     # via httpcore
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
     # via jupyterlab
-idna==3.6
+idna==3.7
     # via
     #   -c requirements/pip/main.lock.txt
     #   anyio
     #   httpx
     #   jsonschema
     #   requests
 importlib-metadata==7.1.0
@@ -120,15 +120,15 @@
     # via ipython
 jinja2==3.1.3
     # via
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   nbconvert
-json5==0.9.24
+json5==0.9.25
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.21.1
     # via
     #   jupyter-events
     #   jupyterlab-server
@@ -149,27 +149,27 @@
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyter-events==0.10.0
     # via jupyter-server
 jupyter-lsp==2.2.5
     # via jupyterlab
-jupyter-server==2.13.0
+jupyter-server==2.14.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
 jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.1.6
+jupyterlab==4.1.8
     # via -r requirements/pip/recommended.in
 jupyterlab-pygments==0.3.0
     # via nbconvert
-jupyterlab-server==2.26.0
+jupyterlab-server==2.27.1
     # via jupyterlab
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 kiwisolver==1.4.5
     # via
     #   -c requirements/pip/main.lock.txt
     #   matplotlib
@@ -177,15 +177,15 @@
     # via
     #   jinja2
     #   nbconvert
 matplotlib==3.8.4
     # via
     #   -c requirements/pip/main.lock.txt
     #   seaborn
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mistune==3.0.2
     # via nbconvert
 nbclient==0.10.0
     # via nbconvert
@@ -217,29 +217,29 @@
     #   astropy
     #   ipykernel
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   matplotlib
     #   nbconvert
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   seaborn
 pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pillow==10.3.0
     # via
     #   -c requirements/pip/main.lock.txt
     #   matplotlib
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   jupyter-core
 prometheus-client==0.20.0
     # via jupyter-server
 prompt-toolkit==3.0.43
     # via ipython
@@ -249,15 +249,15 @@
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
 pycparser==2.22
     # via cffi
-pyerfa==2.0.1.3
+pyerfa==2.0.1.4
     # via astropy
 pygments==2.17.2
     # via
     #   -c requirements/pip/main.lock.txt
     #   ipython
     #   nbconvert
 pyparsing==3.1.2
@@ -278,20 +278,20 @@
     # via
     #   -c requirements/pip/main.lock.txt
     #   pandas
 pyyaml==6.0.1
     # via
     #   astropy
     #   jupyter-events
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   jupyter-events
 requests==2.31.0
     # via
     #   -c requirements/pip/main.lock.txt
@@ -327,26 +327,26 @@
     # via beautifulsoup4
 stack-data==0.6.3
     # via ipython
 terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
-tinycss2==1.2.1
+tinycss2==1.3.0
     # via nbconvert
 tomli==2.0.1
     # via jupyterlab
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   terminado
-traitlets==5.14.2
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
@@ -379,15 +379,15 @@
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via jupyter-server
 widgetsnbextension==4.0.10
     # via ipywidgets
 zipp==3.18.1
     # via
     #   -c requirements/pip/main.lock.txt
     #   importlib-metadata
```

### Comparing `eradiate-0.27.0rc0/requirements/pip/tests.lock.txt` & `eradiate-0.27.0rc1/requirements/pip/tests.lock.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,23 +32,22 @@
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 dessinemoi==24.1.0
     # via -r requirements/pip/main.in
 dynaconf==3.2.5
     # via -r requirements/pip/main.in
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 fonttools==4.51.0
     # via matplotlib
-idna==3.6
+idna==3.7
     # via requests
 importlib-resources==6.4.0
     # via
-    #   -r requirements/pip/main.in
     #   joseki
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
 joseki==2.6.1
     # via -r requirements/pip/main.in
 kiwisolver==1.4.5
@@ -84,39 +83,39 @@
 packaging==24.0
     # via
     #   lazy-loader
     #   matplotlib
     #   pooch
     #   pytest
     #   xarray
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   joseki
     #   sf-hamilton
     #   xarray
 pillow==10.3.0
     # via matplotlib
 pint==0.23
     # via
     #   -r requirements/pip/main.in
     #   joseki
     #   pinttrs
 pinttrs==24.1.0
     # via -r requirements/pip/main.in
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via pooch
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pooch==1.8.1
     # via -r requirements/pip/main.in
 pygments==2.17.2
     # via rich
 pyparsing==3.1.2
     # via matplotlib
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
     # via -r requirements/pip/tests.in
 pytest-metadata==3.1.1
@@ -138,15 +137,15 @@
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 scipy==1.13.0
     # via
     #   -r requirements/pip/main.in
     #   joseki
     #   ussa1976
-sf-hamilton==1.57.0
+sf-hamilton==1.59.1
     # via -r requirements/pip/main.in
 shellingham==1.5.4
     # via
     #   -r requirements/pip/main.in
     #   typer
 six==1.16.0
     # via python-dateutil
```

### Comparing `eradiate-0.27.0rc0/setpath.sh` & `eradiate-0.27.0rc1/setpath.sh`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/__init__.pyi` & `eradiate-0.27.0rc1/src/eradiate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/_factory.py` & `eradiate-0.27.0rc1/src/eradiate/_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/_mode.py` & `eradiate-0.27.0rc1/src/eradiate/_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/attrs.py` & `eradiate-0.27.0rc1/src/eradiate/attrs.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/cfconventions.py` & `eradiate-0.27.0rc1/src/eradiate/cfconventions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/cli/__init__.py` & `eradiate-0.27.0rc1/src/eradiate/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/cli/data.py` & `eradiate-0.27.0rc1/src/eradiate/cli/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os.path
 import textwrap
 from pathlib import Path
 from typing import List, Optional
 
 import typer
-from importlib_resources import files
 from rich.console import Console
 from ruamel.yaml import YAML
 from typing_extensions import Annotated
 
 import eradiate
 
-from ..data._util import get_file_list
+from ..data._util import get_file_list, known_file_lists
 from ..exceptions import DataError
 
 app = typer.Typer()
 console = Console(color_system=None)
 
 
 @app.callback()
@@ -114,58 +113,68 @@
 
 @app.command()
 def fetch(
     file_list: Annotated[
         Optional[List[str]],
         typer.Argument(
             help="An arbitrary number of relative paths to files to be "
-            "retrieved from the data store or file group specifications. "
+            "retrieved from the data store or file list specifications. "
             "If unset, the list of files is read from a YAML file which can be "
-            "specified by using the ``--from-file`` option and defaults to "
-            "``$ERADIATE_SOURCE_DIR/data/downloads_all.yml`` a production "
-            "environment and "
-            "``$ERADIATE_SOURCE_DIR/data/downloads_minimal.yml`` in a "
-            "development environment."
+            "specified by using the ``--from-file`` option, if it is specified. "
+            "Otherwise, it defaults to ``all`` in a production environment and "
+            "``minimal`` in a development environment."
         ),
     ] = None,
     from_file: Annotated[
         Optional[str],
         typer.Option(
             "--from-file",
             "-f",
             help="Optional path to a file list (YAML format). If this option "
             "is set, the FILES argument(s) will be ignored.",
         ),
     ] = None,
+    list: Annotated[
+        bool,
+        typer.Option(
+            "--list",
+            "-l",
+            help="List built-in file lists and exit.",
+        ),
+    ] = False,
 ):
     """
     Fetch files from the Eradiate data store.
     """
+    if list:
+        print("Known file lists:")
+        for file_list in known_file_lists():
+            print(f"  {file_list}")
+        exit(0)
+
+    if not file_list:
+        if from_file is None:
+            if eradiate.config.SOURCE_DIR is None:
+                file_list = ["all"]
+            else:
+                file_list = ["minimal"]
+        else:
+            console.print(f"Reading file list from '{from_file}'")
+            yaml = YAML()
+            file_list = yaml.load(Path(from_file))
+
     converted = []
     for spec in file_list:
         try:
             converted.extend(get_file_list(spec))
         except ValueError:
             converted.append(spec)
 
     file_list = converted
 
-    if not file_list:
-        if from_file is None:
-            if eradiate.config.SOURCE_DIR is None:
-                from_file = files("eradiate") / "data/downloads_all.yml"
-            else:
-                from_file = (
-                    eradiate.config.SOURCE_DIR
-                    / "src/eradiate/data/downloads_minimal.yml"
-                )
-        console.print(f"Reading file list from '{from_file}'")
-        yaml = YAML()
-        file_list = yaml.load(Path(from_file))
-
     for filename in file_list:
         try:
             console.print(f"[blue]Fetching '{filename}'[/]")
             path = eradiate.data.data_store.fetch(filename)
         except DataError:
             console.print("[red]✗[/] not found")
         else:
```

### Comparing `eradiate-0.27.0rc0/src/eradiate/cli/show.py` & `eradiate-0.27.0rc1/src/eradiate/cli/show.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/cli/srf.py` & `eradiate-0.27.0rc1/src/eradiate/cli/srf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/config/_env.py` & `eradiate-0.27.0rc1/src/eradiate/config/_env.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/config/_settings.py` & `eradiate-0.27.0rc1/src/eradiate/config/_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import enum
+import importlib.resources
 from pathlib import Path
 
-import importlib_resources
 from dynaconf import Dynaconf, Validator
 
 from ._env import ENV, SOURCE_DIR
 from ..frame import AzimuthConvention
 
 
 class ProgressLevel(enum.IntEnum):
@@ -27,21 +27,21 @@
     return (
         Path("./eradiate_downloads").absolute().resolve()
         if SOURCE_DIR is None
         else SOURCE_DIR / ".eradiate_downloads"
     )
 
 
-DEFAULTS = importlib_resources.files("eradiate.config").joinpath(f"{ENV}.toml")
+DEFAULTS = importlib.resources.files("eradiate.config").joinpath(f"{ENV}.toml")
 
 #: Main settings data structure. See the `Dynaconf documentation <https://www.dynaconf.com/>`_
 #: for details.
 settings = Dynaconf(
     settings_files=[DEFAULTS, "eradiate.toml"],
-    env_prefix="ERADIATE",
+    envvar_prefix="ERADIATE",
     merge_enabled=True,
     validate_on_update=True,
     validators=[
         Validator(
             "AZIMUTH_CONVENTION",
             cast=lambda x: (AzimuthConvention[x.upper()] if isinstance(x, str) else x),
         ),
```

### Comparing `eradiate-0.27.0rc0/src/eradiate/config/default.toml` & `eradiate-0.27.0rc1/docs/resources/config/default.toml`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/contexts.py` & `eradiate-0.27.0rc1/src/eradiate/contexts.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/converters.py` & `eradiate-0.27.0rc1/src/eradiate/converters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/__init__.pyi` & `eradiate-0.27.0rc1/src/eradiate/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/_access.py` & `eradiate-0.27.0rc1/src/eradiate/data/_access.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/_blind_directory.py` & `eradiate-0.27.0rc1/src/eradiate/data/_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/_blind_online.py` & `eradiate-0.27.0rc1/src/eradiate/data/_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/_core.py` & `eradiate-0.27.0rc1/src/eradiate/data/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/_multi.py` & `eradiate-0.27.0rc1/src/eradiate/data/_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/_safe_directory.py` & `eradiate-0.27.0rc1/src/eradiate/data/_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/_safe_online.py` & `eradiate-0.27.0rc1/src/eradiate/data/_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/_store.py` & `eradiate-0.27.0rc1/src/eradiate/data/_store.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/downloads_all.yml` & `eradiate-0.27.0rc1/src/eradiate/data/downloads_all.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/data/downloads_minimal.yml` & `eradiate-0.27.0rc1/src/eradiate/data/downloads_minimal.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/exceptions.py` & `eradiate-0.27.0rc1/src/eradiate/exceptions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/experiments/_atmosphere.py` & `eradiate-0.27.0rc1/src/eradiate/experiments/_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/experiments/_canopy.py` & `eradiate-0.27.0rc1/src/eradiate/experiments/_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/experiments/_canopy_atmosphere.py` & `eradiate-0.27.0rc1/src/eradiate/experiments/_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/experiments/_core.py` & `eradiate-0.27.0rc1/src/eradiate/experiments/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/experiments/_dem.py` & `eradiate-0.27.0rc1/src/eradiate/experiments/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/experiments/_helpers.py` & `eradiate-0.27.0rc1/src/eradiate/experiments/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/frame.py` & `eradiate-0.27.0rc1/src/eradiate/frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/__init__.pyi` & `eradiate-0.27.0rc1/src/eradiate/kernel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/_bitmap.py` & `eradiate-0.27.0rc1/src/eradiate/kernel/_bitmap.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/_bsdf.py` & `eradiate-0.27.0rc1/src/eradiate/kernel/_bsdf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/_kernel_dict.py` & `eradiate-0.27.0rc1/src/eradiate/kernel/_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/_render.py` & `eradiate-0.27.0rc1/src/eradiate/kernel/_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/_versions.py` & `eradiate-0.27.0rc1/src/eradiate/kernel/_versions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/gridvolume.py` & `eradiate-0.27.0rc1/src/eradiate/kernel/gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/logging.py` & `eradiate-0.27.0rc1/src/eradiate/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/kernel/transform.py` & `eradiate-0.27.0rc1/src/eradiate/kernel/transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/notebook/__init__.py` & `eradiate-0.27.0rc1/src/eradiate/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/notebook/tutorials.py` & `eradiate-0.27.0rc1/src/eradiate/notebook/tutorials.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/pipelines/__init__.py` & `eradiate-0.27.0rc1/src/eradiate/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/pipelines/core.py` & `eradiate-0.27.0rc1/src/eradiate/pipelines/core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/pipelines/definitions.py` & `eradiate-0.27.0rc1/src/eradiate/pipelines/definitions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/pipelines/logic.py` & `eradiate-0.27.0rc1/src/eradiate/pipelines/logic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/quad.py` & `eradiate-0.27.0rc1/src/eradiate/quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/radprops/__init__.pyi` & `eradiate-0.27.0rc1/src/eradiate/radprops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/radprops/_absorption.py` & `eradiate-0.27.0rc1/src/eradiate/radprops/_absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/radprops/_atmosphere.py` & `eradiate-0.27.0rc1/src/eradiate/radprops/_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/radprops/_core.py` & `eradiate-0.27.0rc1/src/eradiate/radprops/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/radprops/rayleigh.py` & `eradiate-0.27.0rc1/src/eradiate/radprops/rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/rng.py` & `eradiate-0.27.0rc1/src/eradiate/rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/__init__.pyi` & `eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_heterogeneous.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_homogeneous.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_molecular.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_molecular.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_particle_dist.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/atmosphere/_particle_layer.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/atmosphere/_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/__init__.pyi` & `eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_canopies.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_canopies.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_canopy_loader.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_canopy_loader.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_discrete.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_leaf_cloud.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_rami_scenarios.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_rami_scenarios.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/biosphere/_tree.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/biosphere/_tree.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_black.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_checkerboard.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_hapke.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_hapke.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_lambertian.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_mqdiffuse.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_opacity_mask.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_opacity_mask.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_rpv.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/bsdfs/_rtls.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/bsdfs/_rtls.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/geometry.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/geometry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_astro_object.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_astro_object.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_constant.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_directional.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/illumination/_spot.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/illumination/_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/integrators/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/integrators/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/integrators/_path_tracers.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/integrators/_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/__init__.pyi` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/_distant.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/_distant_flux.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/_hemispherical_distant.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/_multi_distant.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/_multi_radiancemeter.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/_perspective.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/measure/_radiancemeter.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/measure/_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/phase/_blend.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/phase/_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/phase/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/phase/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/phase/_hg.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/phase/_hg.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/phase/_rayleigh.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/phase/_rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/phase/_tabulated.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/phase/_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_buffermesh.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_cuboid.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_filemesh.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_rectangle.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/shapes/_sphere.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/shapes/_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_air_scattering_coefficient.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_interpolated.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_multi_delta.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_multi_delta.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_solar_irradiance.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_solar_irradiance.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     This scene element produces the scene dictionary required to
     instantiate a kernel plugin using the Sun irradiance spectrum. The data set
     used by this element is controlled by the ``dataset`` field.
 
     See Also
     --------
 
-    :ref:`Solar irradiance spectrum data guide <sec-user_guide-data-solar_irradiance>`
+    :ref:`Solar irradiance spectrum data guide <sec-data-solar_irradiance>`
 
     Notes
     ------
 
     * The spectral range of the data sets shipped can vary and an attempt for
       use outside the supported spectral range will raise a
       :class:`ValueError` upon calling :meth:`kernel_dict`.
@@ -114,15 +114,15 @@
         "If a xarray.Dataset is passed, the dataset is used as is "
         "(refer to the data guide for the format requirements of this dataset)."
         "If a path is passed, the converter tries to open the corresponding "
         "file on the hard drive; should that fail, it queries the Eradiate data"
         "store with that path."
         "If a string is passed, it is interpreted as a Solar irradiance "
         "spectrum identifier "
-        "(see :ref:`sec-user_guide-data-solar_irradiance` for the list); ",
+        "(see :ref:`sec-data-solar_irradiance` for the list); ",
         type="Dataset",
         init_type="Dataset or str or path-like, optional",
         default='"coddington_2021-1_nm"',
     )
 
     scale: float = documented(
         attrs.field(default=1.0, converter=float, validator=validators.is_positive),
```

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/spectra/_uniform.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/spectra/_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/surface/_basic.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/surface/_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/surface/_central_patch.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/surface/_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/surface/_core.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/surface/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/scenes/surface/_dem.py` & `eradiate-0.27.0rc1/src/eradiate/scenes/surface/_dem.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 import attrs
 import mitsuba as mi
 import numpy as np
 import pint
 import xarray as xr
 
-from ._core import Surface
+from ...attrs import documented, get_doc, parse_docs
+from ...constants import EARTH_RADIUS
+from ...units import to_quantity
+from ...units import unit_context_config as ucc
+from ...units import unit_context_kernel as uck
+from ...units import unit_registry as ureg
 from ..bsdfs import BSDF, LambertianBSDF, OpacityMaskBSDF
 from ..core import SceneElement
 from ..geometry import PlaneParallelGeometry, SceneGeometry, SphericalShellGeometry
 from ..shapes import (
     BufferMeshShape,
     FileMeshShape,
     RectangleShape,
     Shape,
     SphereShape,
     shape_factory,
 )
-from ...attrs import documented, get_doc, parse_docs
-from ...constants import EARTH_RADIUS
-from ...units import to_quantity
-from ...units import unit_context_config as ucc
-from ...units import unit_context_kernel as uck
-from ...units import unit_registry as ureg
+from ._core import Surface
 
 
 def mesh_from_dem(
     da: xr.DataArray,
     geometry: str | dict | SceneGeometry,
     planet_radius: pint.Quantity | float | None = None,
 ) -> "mitsuba.Mesh":
@@ -138,17 +138,18 @@
     elif isinstance(geometry, PlaneParallelGeometry):
         vertices_new = _transform_vertices_plane_parallel(
             vertices,
             planet_radius=planet_radius.m_as(uck.get("length")),
             altitude=atmo_bottom.m_as(uck.get("length")),
         ) * uck.get("length")
         mesh = BufferMeshShape(vertices=vertices_new, faces=faces)
-
     else:
-        raise ValueError(f"Unsupported scene geometry: {geometry}")
+        raise ValueError(
+            f"geometry must be PlaneParallelGeometry or SphericalShellGeometry, got {type(geometry)}"
+        )
 
     return mesh, theta_lim * ureg.deg, phi_lim * ureg.deg
 
 
 def _generate_dem_vertices(x, y, elevation):
     """
     Generate DEM vertex positions as (latitude, longitude, elevation) triplets
@@ -367,15 +368,15 @@
                 attrs.validators.instance_of((BufferMeshShape, FileMeshShape))
             ),
             kw_only=True,
             default=None,
         ),
         doc="Shape describing the surface.",
         type=".BufferMeshShape or .FileMeshShape or None",
-        init_type=".BufferMeshShape or .OBJMeshShape or .PLYMeshShape or dict",
+        init_type=".BufferMeshShape or .FileMeshShape or dict",
         default="None",
     )
 
     shape_background: Shape = documented(
         attrs.field(
             converter=attrs.converters.optional(shape_factory.convert),
             validator=attrs.validators.optional(
@@ -467,15 +468,19 @@
         bsdf : .BSDF, optional, default: :class:`LambertianBSDF() <.LambertianBSDF>`
             Scattering model attached to the surface.
 
         Returns
         -------
         .DEMSurface
         """
-        geometry = PlaneParallelGeometry() if geometry is None else geometry
+        geometry = (
+            PlaneParallelGeometry()
+            if geometry is None
+            else SceneGeometry.convert(geometry)
+        )
         bsdf = LambertianBSDF() if bsdf is None else bsdf
         bsdf_id = f"{id}_bsdf"
         mesh = attrs.evolve(mesh, bsdf=bsdf)
 
         if isinstance(geometry, SphericalShellGeometry):
             if planet_radius is not None:
                 warnings.warn(
@@ -539,8 +544,11 @@
                 center=[0.0, 0.0, geometry.ground_altitude.m]
                 * geometry.ground_altitude.units,
                 normal=np.array([0, 0, 1]),
                 up=np.array([0, 1, 0]),
                 bsdf=opacity_bsdf,
             )
 
+        else:
+            raise TypeError(f"Scene geometry is not recognized. {geometry}")
+
         return cls(shape=mesh, shape_background=surface_background, id=id)
```

### Comparing `eradiate-0.27.0rc0/src/eradiate/spectral/ckd.py` & `eradiate-0.27.0rc1/src/eradiate/spectral/ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/spectral/index.py` & `eradiate-0.27.0rc1/src/eradiate/spectral/index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/spectral/mono.py` & `eradiate-0.27.0rc1/src/eradiate/spectral/mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/srf_tools.py` & `eradiate-0.27.0rc1/src/eradiate/srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/test_tools/data.py` & `eradiate-0.27.0rc1/src/eradiate/test_tools/data.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/test_tools/fixtures.py` & `eradiate-0.27.0rc1/src/eradiate/test_tools/fixtures.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/test_tools/plugin.py` & `eradiate-0.27.0rc1/src/eradiate/test_tools/plugin.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/test_tools/regression.py` & `eradiate-0.27.0rc1/src/eradiate/test_tools/regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/test_tools/types.py` & `eradiate-0.27.0rc1/src/eradiate/test_tools/types.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/test_tools/util.py` & `eradiate-0.27.0rc1/src/eradiate/test_tools/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/units.py` & `eradiate-0.27.0rc1/src/eradiate/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
 __all__ = [
     "symbol",
     "to_quantity",
+    "units_compatible",
     "unit_context_config",
     "unit_context_kernel",
     "unit_registry",
     "PhysicalQuantity",
 ]
 
 import enum
 import importlib
 import logging
 import typing as t
 from functools import lru_cache
+from importlib.resources import files
 
 import pint
 import pinttr
 import xarray
-from importlib_resources import files
 from pinttr.exceptions import UnitsError
 from pinttr.util import units_compatible
 
 logger = logging.getLogger(__name__)
 
 
 # -- Global data members -------------------------------------------------------
```

### Comparing `eradiate-0.27.0rc0/src/eradiate/units.txt` & `eradiate-0.27.0rc1/src/eradiate/units.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/util/deprecation.py` & `eradiate-0.27.0rc1/src/eradiate/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/util/misc.py` & `eradiate-0.27.0rc1/src/eradiate/util/misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/util/numpydoc.py` & `eradiate-0.27.0rc1/src/eradiate/util/numpydoc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/util/sys_info.py` & `eradiate-0.27.0rc1/src/eradiate/util/sys_info.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/validators.py` & `eradiate-0.27.0rc1/src/eradiate/validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/warp.py` & `eradiate-0.27.0rc1/src/eradiate/warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/xarray/_accessors.py` & `eradiate-0.27.0rc1/src/eradiate/xarray/_accessors.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/xarray/_helpers.py` & `eradiate-0.27.0rc1/src/eradiate/xarray/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate/xarray/interp.py` & `eradiate-0.27.0rc1/src/eradiate/xarray/interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/src/eradiate.egg-info/PKG-INFO` & `eradiate-0.27.0rc1/src/eradiate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.27.0rc0
+Version: 0.27.0rc1
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
@@ -14,15 +14,14 @@
 Requires-Dist: eradiate-mitsuba==0.2.1
 Requires-Dist: aenum
 Requires-Dist: attrs>=22.2
 Requires-Dist: cachetools>=5.3
 Requires-Dist: click
 Requires-Dist: dessinemoi>=23.1.0
 Requires-Dist: dynaconf>=3.2
-Requires-Dist: importlib_resources
 Requires-Dist: joseki>=2.6.0
 Requires-Dist: lazy_loader>=0.1
 Requires-Dist: matplotlib>=3.3
 Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: pint
 Requires-Dist: pinttrs>=23.2.0
@@ -47,15 +46,14 @@
 Requires-Dist: seaborn; extra == "recommended"
 Requires-Dist: aenum; extra == "recommended"
 Requires-Dist: attrs>=22.2; extra == "recommended"
 Requires-Dist: cachetools>=5.3; extra == "recommended"
 Requires-Dist: click; extra == "recommended"
 Requires-Dist: dessinemoi>=23.1.0; extra == "recommended"
 Requires-Dist: dynaconf>=3.2; extra == "recommended"
-Requires-Dist: importlib_resources; extra == "recommended"
 Requires-Dist: joseki>=2.6.0; extra == "recommended"
 Requires-Dist: lazy_loader>=0.1; extra == "recommended"
 Requires-Dist: matplotlib>=3.3; extra == "recommended"
 Requires-Dist: netcdf4; extra == "recommended"
 Requires-Dist: numpy; extra == "recommended"
 Requires-Dist: pint; extra == "recommended"
 Requires-Dist: pinttrs>=23.2.0; extra == "recommended"
```

### Comparing `eradiate-0.27.0rc0/src/eradiate.egg-info/SOURCES.txt` & `eradiate-0.27.0rc1/src/eradiate.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 .github/workflows/cd.yml
 .github/workflows/ci.yml
 docs/Makefile
 docs/conf.py
 docs/convert_figures.py
 docs/generate_md_cli.py
 docs/generate_rst_api.py
+docs/generate_rst_data.py
 docs/generate_rst_plugins.py
 docs/index.rst
 docs/index_latex.rst
 docs/make.bat
 docs/references.bib
 docs/tutorials
 docs/_ext/exec.py
@@ -92,18 +93,69 @@
 docs/fig/spectral_discretization_mono_noatm_isolated.png
 docs/fig/spherical-coordinate-system.png
 docs/fig/spherical-coordinate-system.svg
 docs/fig/thuillier_2003.png
 docs/fig/diagrams/class_diagram_biosphere.drawio
 docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
 docs/fig/diagrams/package.drawio
+docs/fig/rami_scenes/ADJACENT_CANOPIES_MEDIUM_ERECTOPHILE_SPARSE_PLANOPHILE_30_90.png
+docs/fig/rami_scenes/ADJACENT_CANOPIES_SPARSE_ERECTOPHILE_DENSE_PLANOPHILE_30_90.png
+docs/fig/rami_scenes/AGRICULTURAL_CROPS_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_ERECTOPHILE_B_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_ERECTOPHILE_C_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_DENSE_BRF_MODEL_A_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_DENSE_BRF_MODEL_B_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_DENSE_BRF_MODEL_C_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_SPARSE_BRF_MODEL_A_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_SPARSE_BRF_MODEL_B_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_OVERSTOREY_SPARSE_BRF_MODEL_C_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_PLANOPHILE_A_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_PLANOPHILE_B_30_90.png
+docs/fig/rami_scenes/ANISOTROPIC_BACKGROUND_PLANOPHILE_C_30_90.png
+docs/fig/rami_scenes/CONSTANT_SLOPE_DISTRIBUTION_DENSE_INCLINATION_15_30_90.png
+docs/fig/rami_scenes/CONSTANT_SLOPE_DISTRIBUTION_DENSE_INCLINATION_30_30_90.png
+docs/fig/rami_scenes/CONSTANT_SLOPE_DISTRIBUTION_SPARSE_INCLINATION_15_30_90.png
+docs/fig/rami_scenes/CONSTANT_SLOPE_DISTRIBUTION_SPARSE_INCLINATION_30_30_90.png
+docs/fig/rami_scenes/JARVSELJA_BIRCH_STAND_SUMMER_30_90.png
+docs/fig/rami_scenes/JARVSELJA_BIRCH_STAND_WINTER_30_90.png
+docs/fig/rami_scenes/JARVSELJA_PINE_STAND_30_90.png
+docs/fig/rami_scenes/OFENPASS_PINE_STAND_30_90.png
+docs/fig/rami_scenes/SAVANNA_PRE_FIRE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_ERECTOPHILE_SPARSE_PLANOPHILE_DENSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_ERECTOPHILE_SPARSE_PLANOPHILE_MEDIUM_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_ERECTOPHILE_SPARSE_PLANOPHILE_SPARSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_DENSE_UNDERSTORIES_DENSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_DENSE_UNDERSTORIES_SPARSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_MEDIUM_UNDERSTORIES_DENSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_MEDIUM_UNDERSTORIES_SPARSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_SPARSE_UNDERSTORIES_DENSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_OVERSTORIES_SPARSE_UNDERSTORIES_SPARSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_PLANOPHILE_SPARSE_ERECTOPHILE_DENSE_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_PLANOPHILE_SPARSE_ERECTOPHILE_MEDIUM_30_90.png
+docs/fig/rami_scenes/TWO_LAYER_CANOPY_PLANOPHILE_SPARSE_ERECTOPHILE_SPARSE_30_90.png
+docs/fig/rami_scenes/WELLINGTON_CITRUS_ORCHARD_30_90.png
+docs/fig/rami_scenes/WYTHAM_WOOD_30_90.png
+docs/resources/config/default.toml
 docs/rst/bibliography.rst
 docs/rst/contributing.rst
 docs/rst/dependencies.rst
 docs/rst/maintainer_guide.rst
+docs/rst/data/atmosphere_molecular_absorption.rst
+docs/rst/data/atmosphere_thermoprops.rst
+docs/rst/data/data_format_details.rst
+docs/rst/data/intro.rst
+docs/rst/data/solar_irradiance.rst
+docs/rst/data/srf.rst
+docs/rst/data/fig/govaerts_2021-continental-extrapolated.png
+docs/rst/data/fig/govaerts_2021-desert-extrapolated.png
+docs/rst/data/fig/p_interp_rerr_histo_65349.png
+docs/rst/data/fig/pt_points.png
+docs/rst/data/fig/w_interp_rerr_histo_101325.png
+docs/rst/data/generated/aerosols_particles.rst
+docs/rst/data/generated/rami_scenes.rst
 docs/rst/developer_guide/design_atmosphere.rst
 docs/rst/developer_guide/dev_install.rst
 docs/rst/developer_guide/factory_guide.rst
 docs/rst/developer_guide/index.rst
 docs/rst/developer_guide/lazy_loading.rst
 docs/rst/developer_guide/radiometric_kernel_interface.rst
 docs/rst/developer_guide/scene_generator.rst
@@ -134,45 +186,36 @@
 docs/rst/reference_api/test_tools.rst
 docs/rst/reference_api/units.rst
 docs/rst/reference_api/util.rst
 docs/rst/reference_api/validators.rst
 docs/rst/reference_api/warp.rst
 docs/rst/reference_api/xarray.rst
 docs/rst/reference_plugins/index.rst
+docs/rst/user_guide/atmosphere_experiment.rst
 docs/rst/user_guide/basic_concepts.rst
+docs/rst/user_guide/canopy_scene_loader.rst
+docs/rst/user_guide/config.rst
 docs/rst/user_guide/conventions.rst
+docs/rst/user_guide/dem_experiment.rst
 docs/rst/user_guide/index.rst
 docs/rst/user_guide/install.rst
-docs/rst/user_guide/onedim_experiment.rst
 docs/rst/user_guide/package_structure.rst
-docs/rst/user_guide/scene_loader.rst
 docs/rst/user_guide/spectral_discretization.rst
 docs/rst/user_guide/unit_guide_user.rst
 docs/rst/user_guide/atmosphere/absorption.rst
 docs/rst/user_guide/atmosphere/heterogeneous.rst
 docs/rst/user_guide/atmosphere/homogeneous.rst
 docs/rst/user_guide/atmosphere/index.rst
 docs/rst/user_guide/atmosphere/intro.rst
 docs/rst/user_guide/atmosphere/molecular.rst
 docs/rst/user_guide/atmosphere/particle_layer.rst
 docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
 docs/rst/user_guide/atmosphere/fig/bad_resolution.png
 docs/rst/user_guide/atmosphere/fig/good_resolution.png
 docs/rst/user_guide/atmosphere/fig/line.png
-docs/rst/user_guide/data/absorption.rst
-docs/rst/user_guide/data/atmosphere_radprops.rst
-docs/rst/user_guide/data/atmosphere_thermoprops.rst
-docs/rst/user_guide/data/index.rst
-docs/rst/user_guide/data/intro.rst
-docs/rst/user_guide/data/particle_radprops.rst
-docs/rst/user_guide/data/solar_irradiance.rst
-docs/rst/user_guide/data/srf.rst
-docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
-docs/rst/user_guide/data/fig/pt_points.png
-docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
 docs/src/reference_cli.md
 docs/src/release_notes/index.md
 docs/src/release_notes/v0.23.x_and_older.md
 docs/src/release_notes/v0.24.x.md
 docs/src/release_notes/v0.25.x.md
 docs/src/release_notes/v0.26.x.md
 docs/src/release_notes/v0.27.x.md
```

### Comparing `eradiate-0.27.0rc0/src/eradiate.egg-info/requires.txt` & `eradiate-0.27.0rc1/src/eradiate.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 eradiate-mitsuba==0.2.1
 aenum
 attrs>=22.2
 cachetools>=5.3
 click
 dessinemoi>=23.1.0
 dynaconf>=3.2
-importlib_resources
 joseki>=2.6.0
 lazy_loader>=0.1
 matplotlib>=3.3
 netcdf4
 numpy
 pint
 pinttrs>=23.2.0
@@ -35,15 +34,14 @@
 seaborn
 aenum
 attrs>=22.2
 cachetools>=5.3
 click
 dessinemoi>=23.1.0
 dynaconf>=3.2
-importlib_resources
 joseki>=2.6.0
 lazy_loader>=0.1
 matplotlib>=3.3
 netcdf4
 numpy
 pint
 pinttrs>=23.2.0
```

### Comparing `eradiate-0.27.0rc0/tests/01_unit/data/test_blind_directory.py` & `eradiate-0.27.0rc1/tests/01_unit/data/test_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/data/test_blind_online.py` & `eradiate-0.27.0rc1/tests/01_unit/data/test_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/data/test_core.py` & `eradiate-0.27.0rc1/tests/01_unit/data/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/data/test_datasets.py` & `eradiate-0.27.0rc1/tests/01_unit/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/data/test_multi.py` & `eradiate-0.27.0rc1/tests/01_unit/data/test_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/data/test_safe_directory.py` & `eradiate-0.27.0rc1/tests/01_unit/data/test_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/data/test_safe_online.py` & `eradiate-0.27.0rc1/tests/01_unit/data/test_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/experiments/test_atmosphere.py` & `eradiate-0.27.0rc1/tests/01_unit/experiments/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/experiments/test_canopy.py` & `eradiate-0.27.0rc1/tests/01_unit/experiments/test_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/experiments/test_canopy_atmosphere.py` & `eradiate-0.27.0rc1/tests/01_unit/experiments/test_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/experiments/test_core.py` & `eradiate-0.27.0rc1/tests/01_unit/experiments/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/experiments/test_dem.py` & `eradiate-0.27.0rc1/tests/01_unit/experiments/test_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/experiments/test_helpers.py` & `eradiate-0.27.0rc1/tests/01_unit/experiments/test_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/kernel/test_gridvolume.py` & `eradiate-0.27.0rc1/tests/01_unit/kernel/test_gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/kernel/test_kernel_dict.py` & `eradiate-0.27.0rc1/tests/01_unit/kernel/test_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/kernel/test_logging.py` & `eradiate-0.27.0rc1/tests/01_unit/kernel/test_logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/kernel/test_render.py` & `eradiate-0.27.0rc1/tests/01_unit/kernel/test_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/kernel/test_transform.py` & `eradiate-0.27.0rc1/tests/01_unit/kernel/test_transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/pipelines/conftest.py` & `eradiate-0.27.0rc1/tests/01_unit/pipelines/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/pipelines/test_logic.py` & `eradiate-0.27.0rc1/tests/01_unit/pipelines/test_logic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/radprops/test_absorption.py` & `eradiate-0.27.0rc1/tests/01_unit/radprops/test_absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/radprops/test_rayleigh_scattering.py` & `eradiate-0.27.0rc1/tests/01_unit/radprops/test_rayleigh_scattering.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/radprops/test_zgrid.py` & `eradiate-0.27.0rc1/tests/01_unit/radprops/test_zgrid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_heterogeneous.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_homogeneous.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_molecular_atmosphere.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_molecular_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_particle_dist.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/atmosphere/test_particle_layer.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/atmosphere/test_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_core.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_discrete.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_leaf_cloud.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_tree_abstract.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_tree_abstract.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/biosphere/test_tree_mesh.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/biosphere/test_tree_mesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_black.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_checkerboard.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_hapke.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_hapke.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_lambertian.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_mqdiffuse.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_rpv.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/bsdfs/test_rtls.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/bsdfs/test_rtls.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/test_astro_object.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/test_astro_object.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/test_constant.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/test_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/test_directional.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/test_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/illumination/test_spot.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/illumination/test_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/integrators/test_path_tracers.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/integrators/test_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_distant_flux.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_hemispherical_distant.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_multi_distant.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_multi_radiancemeter.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_perspective.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_radiancemeter.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/measure/test_target.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/measure/test_target.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/phase/test_blend.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/phase/test_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/phase/test_tabulated.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/phase/test_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_buffermesh.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_cuboid.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_filemesh.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_rectangle.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/shapes/test_sphere.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/shapes/test_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_air_scattering_coefficient.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_core.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_interpolated.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_multi_delta.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_multi_delta.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_solar_irradiance.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/spectra/test_uniform.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/spectra/test_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/surface/test_basic.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/surface/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/surface/test_central_patch.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/surface/test_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/surface/test_dem.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/surface/test_dem.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,29 +123,47 @@
                     },
                 ),
                 "geometry": "spherical_shell",
                 "planet_radius": EARTH_RADIUS,
             },
             [(-0.089832, 0.179664), (-0.269496, 0.359328)],
         ),
+        (
+            {
+                "da": make_dataarray(
+                    data=np.zeros((10, 10)) * ureg.m,
+                    coords={
+                        "x": np.linspace(-10, 20, 10) * ureg.km,
+                        "y": np.linspace(-30, 40, 10) * ureg.km,
+                    },
+                ),
+                "geometry": "invalidgeometry",
+                "planet_radius": EARTH_RADIUS,
+            },
+            [(-0.089832, 0.179664), (-0.269496, 0.359328)],
+        ),
     ],
 )
 def test_mesh_from_dem(modes_all_double, kwargs, expected_limits):
-    if (kwargs["geometry"] == "spherical_shell") and kwargs[
-        "planet_radius"
-    ] is not None:
-        with pytest.warns():
-            mesh, lat, lon = mesh_from_dem(**kwargs)
+    if kwargs["geometry"] not in ["spherical_shell", "plane_parallel"]:
+        with pytest.raises(ValueError):
+            mesh_from_dem(**kwargs)
     else:
-        mesh, lat, lon = mesh_from_dem(**kwargs)
+        if (kwargs["geometry"] == "spherical_shell") and kwargs[
+            "planet_radius"
+        ] is not None:
+            with pytest.warns():
+                mesh, lat, lon = mesh_from_dem(**kwargs)
+        else:
+            mesh, lat, lon = mesh_from_dem(**kwargs)
 
-    assert len(mesh.vertices) == 100
+        assert len(mesh.vertices) == 100
 
-    assert np.allclose(lat.m, expected_limits[0], atol=1e-4, rtol=1e-3)
-    assert np.allclose(lon.m, expected_limits[1], atol=1e-4, rtol=1e-3)
+        assert np.allclose(lat.m, expected_limits[0], atol=1e-4, rtol=1e-3)
+        assert np.allclose(lon.m, expected_limits[1], atol=1e-4, rtol=1e-3)
 
 
 @pytest.mark.parametrize(
     "geometry, expected_bg, planet_radius",
     [
         (PlaneParallelGeometry(), RectangleShape, EARTH_RADIUS),
         (SphericalShellGeometry(), SphereShape, None),
```

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/test_core.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/scenes/test_loader.py` & `eradiate-0.27.0rc1/tests/01_unit/scenes/test_loader.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/spectral/test_ckd.py` & `eradiate-0.27.0rc1/tests/01_unit/spectral/test_ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/spectral/test_index.py` & `eradiate-0.27.0rc1/tests/01_unit/spectral/test_index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/spectral/test_mono.py` & `eradiate-0.27.0rc1/tests/01_unit/spectral/test_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_factory.py` & `eradiate-0.27.0rc1/tests/01_unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_frame.py` & `eradiate-0.27.0rc1/tests/01_unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_mode.py` & `eradiate-0.27.0rc1/tests/01_unit/test_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_quad.py` & `eradiate-0.27.0rc1/tests/01_unit/test_quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_rng.py` & `eradiate-0.27.0rc1/tests/01_unit/test_rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_srf_tools.py` & `eradiate-0.27.0rc1/tests/01_unit/test_srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_tools/test_regression.py` & `eradiate-0.27.0rc1/tests/01_unit/test_tools/test_regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_units.py` & `eradiate-0.27.0rc1/tests/01_unit/test_units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_validators.py` & `eradiate-0.27.0rc1/tests/01_unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/test_warp.py` & `eradiate-0.27.0rc1/tests/01_unit/test_warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/util/test_deprecation.py` & `eradiate-0.27.0rc1/tests/01_unit/util/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/util/test_misc.py` & `eradiate-0.27.0rc1/tests/01_unit/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/01_unit/xarray_/test_interp.py` & `eradiate-0.27.0rc1/tests/01_unit/xarray_/test_interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/conftest.py` & `eradiate-0.27.0rc1/tests/02_system/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_albedo.py` & `eradiate-0.27.0rc1/tests/02_system/test_albedo.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_atmosphere_rpv.py` & `eradiate-0.27.0rc1/tests/02_system/test_atmosphere_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_basic.py` & `eradiate-0.27.0rc1/tests/02_system/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_ckd_basic.py` & `eradiate-0.27.0rc1/tests/02_system/test_ckd_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_compare_canopy_atmosphere.py` & `eradiate-0.27.0rc1/tests/02_system/test_compare_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_heterogeneous_atmosphere_expansion.py` & `eradiate-0.27.0rc1/tests/02_system/test_heterogeneous_atmosphere_expansion.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_heterogeneous_atmosphere_flags.py` & `eradiate-0.27.0rc1/tests/02_system/test_heterogeneous_atmosphere_flags.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py` & `eradiate-0.27.0rc1/tests/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_irradiance_scaling.py` & `eradiate-0.27.0rc1/tests/02_system/test_irradiance_scaling.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_kernel_render_benchmark.py` & `eradiate-0.27.0rc1/tests/02_system/test_kernel_render_benchmark.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_maximum_scene_size.py` & `eradiate-0.27.0rc1/tests/02_system/test_maximum_scene_size.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_mdistant_insitu.py` & `eradiate-0.27.0rc1/tests/02_system/test_mdistant_insitu.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_onedim_lambertian_brf.py` & `eradiate-0.27.0rc1/tests/02_system/test_onedim_lambertian_brf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_onedim_phase.py` & `eradiate-0.27.0rc1/tests/02_system/test_onedim_phase.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_onedim_symmetry.py` & `eradiate-0.27.0rc1/tests/02_system/test_onedim_symmetry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/02_system/test_spectral_loop.py` & `eradiate-0.27.0rc1/tests/02_system/test_spectral_loop.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/03_regression/atmospheres/test_rpv_afgl1986.py` & `eradiate-0.27.0rc1/tests/03_regression/atmospheres/test_rpv_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/03_regression/atmospheres/test_rpv_afgl1986_continental.py` & `eradiate-0.27.0rc1/tests/03_regression/atmospheres/test_rpv_afgl1986_continental.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py` & `eradiate-0.27.0rc1/tests/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/03_regression/romc/test_het01.py` & `eradiate-0.27.0rc1/tests/03_regression/romc/test_het01.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/03_regression/romc/test_het04.py` & `eradiate-0.27.0rc1/tests/03_regression/romc/test_het04.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/03_regression/romc/test_het06.py` & `eradiate-0.27.0rc1/tests/03_regression/romc/test_het06.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.27.0rc0/tests/conftest.py` & `eradiate-0.27.0rc1/tests/conftest.py`

 * *Files identical despite different names*

