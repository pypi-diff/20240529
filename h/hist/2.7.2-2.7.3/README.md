# Comparing `tmp/hist-2.7.2.tar.gz` & `tmp/hist-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Sep 12 16:07:16 2023, max compression
+gzip compressed data, last modified: Wed May 29 07:46:56 2024, max compression
```

## Comparing `hist-2.7.2.tar` & `hist-2.7.3.tar`

### file list

```diff
@@ -1,146 +1,147 @@
--rw-r--r--   0        0        0     3319 2023-09-12 16:07:16.000000 hist-2.7.2/.all-contributorsrc
--rw-r--r--   0        0        0      125 2023-09-12 16:07:16.000000 hist-2.7.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-09-12 16:07:16.000000 hist-2.7.2/.gitattributes
--rw-r--r--   0        0        0     1775 2023-09-12 16:07:16.000000 hist-2.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      456 2023-09-12 16:07:16.000000 hist-2.7.2/.readthedocs.yml
--rw-r--r--   0        0        0      789 2023-09-12 16:07:16.000000 hist-2.7.2/CITATION.cff
--rw-r--r--   0        0        0      412 2023-09-12 16:07:16.000000 hist-2.7.2/dev-environment.yml
--rw-r--r--   0        0        0     3153 2023-09-12 16:07:16.000000 hist-2.7.2/noxfile.py
--rw-r--r--   0        0        0     2543 2023-09-12 16:07:16.000000 hist-2.7.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-09-12 16:07:16.000000 hist-2.7.2/.github/dependabot.yml
--rw-r--r--   0        0        0      169 2023-09-12 16:07:16.000000 hist-2.7.2/.github/labeler.yml
--rw-r--r--   0        0        0      268 2023-09-12 16:07:16.000000 hist-2.7.2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      343 2023-09-12 16:07:16.000000 hist-2.7.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      399 2023-09-12 16:07:16.000000 hist-2.7.2/.github/ISSUE_TEMPLATE/docs-improvements.md
--rw-r--r--   0        0        0      537 2023-09-12 16:07:16.000000 hist-2.7.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      227 2023-09-12 16:07:16.000000 hist-2.7.2/.github/ISSUE_TEMPLATE/support.md
--rw-r--r--   0        0        0      668 2023-09-12 16:07:16.000000 hist-2.7.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      684 2023-09-12 16:07:16.000000 hist-2.7.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1377 2023-09-12 16:07:16.000000 hist-2.7.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      229 2023-09-12 16:07:16.000000 hist-2.7.2/.github/workflows/pr.yml
--rw-r--r--   0        0        0       76 2023-09-12 16:07:16.000000 hist-2.7.2/binder/postBuild
--rw-r--r--   0        0        0      633 2023-09-12 16:07:16.000000 hist-2.7.2/docs/Makefile
--rw-r--r--   0        0        0     2785 2023-09-12 16:07:16.000000 hist-2.7.2/docs/banner_slides.md
--rw-r--r--   0        0        0     9204 2023-09-12 16:07:16.000000 hist-2.7.2/docs/changelog.md
--rw-r--r--   0        0        0     2707 2023-09-12 16:07:16.000000 hist-2.7.2/docs/conf.py
--rw-r--r--   0        0        0       44 2023-09-12 16:07:16.000000 hist-2.7.2/docs/contributing.md
--rw-r--r--   0        0        0     4205 2023-09-12 16:07:16.000000 hist-2.7.2/docs/index.rst
--rw-r--r--   0        0        0      794 2023-09-12 16:07:16.000000 hist-2.7.2/docs/make.bat
--rw-r--r--   0        0        0      752 2023-09-12 16:07:16.000000 hist-2.7.2/docs/support.rst
--rw-r--r--   0        0        0     3093 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/axis_category.png
--rw-r--r--   0        0        0     5696 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/axis_circular.png
--rw-r--r--   0        0        0     2349 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/axis_integer.png
--rw-r--r--   0        0        0     2352 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/axis_regular.png
--rw-r--r--   0        0        0     2599 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/axis_variable.png
--rw-r--r--   0        0        0   278047 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/banner.gif
--rw-r--r--   0        0        0    21774 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/ex_hist_density.png
--rw-r--r--   0        0        0    62092 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/fullplot_example.png
--rw-r--r--   0        0        0    18389 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/histlogo.png
--rw-r--r--   0        0        0    94683 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/histlogo.svg
--rw-r--r--   0        0        0    17543 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/histogram_design.png
--rw-r--r--   0        0        0   301669 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/pieplot_example.png
--rw-r--r--   0        0        0   114661 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/ratioplot_example.png
--rw-r--r--   0        0        0    14396 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_images/stackplot_example.png
--rw-r--r--   0        0        0       12 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_src/images/.gitignore
--rw-r--r--   0        0        0      257 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_src/images/Makefile
--rw-r--r--   0        0        0      979 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_src/images/axis_category.tex
--rw-r--r--   0        0        0      983 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_src/images/axis_circular.tex
--rw-r--r--   0        0        0      888 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_src/images/axis_integer.tex
--rw-r--r--   0        0        0      912 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_src/images/axis_regular.tex
--rw-r--r--   0        0        0      947 2023-09-12 16:07:16.000000 hist-2.7.2/docs/_src/images/axis_variable.tex
--rw-r--r--   0        0        0     5913 2023-09-12 16:07:16.000000 hist-2.7.2/docs/examples/HistDemo.ipynb
--rw-r--r--   0        0        0      139 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.accumulators.rst
--rw-r--r--   0        0        0      130 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.axestuple.rst
--rw-r--r--   0        0        0      194 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.axis.rst
--rw-r--r--   0        0        0      145 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.axis.transform.rst
--rw-r--r--   0        0        0      127 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.basehist.rst
--rw-r--r--   0        0        0      136 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.classichist.rst
--rw-r--r--   0        0        0      130 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.dask.hist.rst
--rw-r--r--   0        0        0      145 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.dask.namedhist.rst
--rw-r--r--   0        0        0      212 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.dask.rst
--rw-r--r--   0        0        0      115 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.hist.rst
--rw-r--r--   0        0        0      130 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.intervals.rst
--rw-r--r--   0        0        0      130 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.namedhist.rst
--rw-r--r--   0        0        0      118 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.numpy.rst
--rw-r--r--   0        0        0      115 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.plot.rst
--rw-r--r--   0        0        0      150 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.quick_construct.rst
--rw-r--r--   0        0        0      506 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.rst
--rw-r--r--   0        0        0      118 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.stack.rst
--rw-r--r--   0        0        0      124 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.storage.rst
--rw-r--r--   0        0        0      127 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.svgplots.rst
--rw-r--r--   0        0        0      127 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.svgutils.rst
--rw-r--r--   0        0        0      112 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.tag.rst
--rw-r--r--   0        0        0      124 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/hist.version.rst
--rw-r--r--   0        0        0       49 2023-09-12 16:07:16.000000 hist-2.7.2/docs/reference/modules.rst
--rw-r--r--   0        0        0     5217 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/accumulators.rst
--rw-r--r--   0        0        0     1318 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/analyses.rst
--rw-r--r--   0        0        0     7451 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/axes.rst
--rw-r--r--   0        0        0      134 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/cli.rst
--rw-r--r--   0        0        0     1264 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/indexing.rst
--rw-r--r--   0        0        0      603 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/installation.rst
--rw-r--r--   0        0        0     3915 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/numpy.rst
--rw-r--r--   0        0        0     5662 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/quickstart.rst
--rw-r--r--   0        0        0     3586 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/storages.rst
--rw-r--r--   0        0        0     2784 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/subclassing.rst
--rw-r--r--   0        0        0    17509 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/notebooks/Histogram.ipynb
--rw-r--r--   0        0        0     3908 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/notebooks/Interpolation.ipynb
--rw-r--r--   0        0        0     8945 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/notebooks/Plots.ipynb
--rw-r--r--   0        0        0     1680 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/notebooks/Reprs.ipynb
--rw-r--r--   0        0        0    18737 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/notebooks/SVGHistogram.ipynb
--rw-r--r--   0        0        0     5882 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/notebooks/Stack.ipynb
--rw-r--r--   0        0        0     3853 2023-09-12 16:07:16.000000 hist-2.7.2/docs/user-guide/notebooks/Transform.ipynb
--rw-r--r--   0        0        0    50203 2023-09-12 16:07:16.000000 hist-2.7.2/notebooks/HistLogo.ipynb
--rw-r--r--   0        0        0     1717 2023-09-12 16:07:16.000000 hist-2.7.2/notebooks/axestuple-setattr.ipynb
--rw-r--r--   0        0        0     1159 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/__init__.py
--rw-r--r--   0        0        0      172 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/accumulators.py
--rw-r--r--   0        0        0     2291 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/axestuple.py
--rw-r--r--   0        0        0    22531 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/basehist.py
--rw-r--r--   0        0        0     1431 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/classichist.py
--rw-r--r--   0        0        0      126 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/hist.py
--rw-r--r--   0        0        0     4130 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/interop.py
--rw-r--r--   0        0        0     6893 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/intervals.py
--rw-r--r--   0        0        0     5187 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/namedhist.py
--rw-r--r--   0        0        0      161 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/numpy.py
--rw-r--r--   0        0        0    23012 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/plot.py
--rw-r--r--   0        0        0        0 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/py.typed
--rw-r--r--   0        0        0    11131 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/quick_construct.py
--rw-r--r--   0        0        0     5902 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/stack.py
--rw-r--r--   0        0        0      323 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/storage.py
--rw-r--r--   0        0        0     5426 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/svgplots.py
--rw-r--r--   0        0        0     2282 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/svgutils.py
--rw-r--r--   0        0        0      250 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/tag.py
--rw-r--r--   0        0        0      160 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/version.py
--rw-r--r--   0        0        0      118 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/version.pyi
--rw-r--r--   0        0        0        0 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/_compat/__init__.py
--rw-r--r--   0        0        0      759 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/_compat/builtins.py
--rw-r--r--   0        0        0      619 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/_compat/typing.py
--rw-r--r--   0        0        0     6943 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/axis/__init__.py
--rw-r--r--   0        0        0        0 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/axis/py.typed
--rw-r--r--   0        0        0      182 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/axis/transform.py
--rw-r--r--   0        0        0      392 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/dask/__init__.py
--rw-r--r--   0        0        0      290 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/dask/hist.py
--rw-r--r--   0        0        0      325 2023-09-12 16:07:16.000000 hist-2.7.2/src/hist/dask/namedhist.py
--rw-r--r--   0        0        0      742 2023-09-12 16:07:16.000000 hist-2.7.2/tests/conftest.py
--rw-r--r--   0        0        0      691 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_axestuple.py
--rw-r--r--   0        0        0     2078 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_axis.py
--rw-r--r--   0        0        0      528 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_bh.py
--rw-r--r--   0        0        0     4217 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_dask.py
--rw-r--r--   0        0        0    29800 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_general.py
--rw-r--r--   0        0        0    11430 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_interop.py
--rw-r--r--   0        0        0     6204 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_intervals.py
--rw-r--r--   0        0        0      981 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_mock_plot.py
--rw-r--r--   0        0        0    25241 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_named.py
--rw-r--r--   0        0        0    19787 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_plot.py
--rw-r--r--   0        0        0     1040 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_profile.py
--rw-r--r--   0        0        0     2714 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_reprs.py
--rw-r--r--   0        0        0    12300 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_stacks.py
--rw-r--r--   0        0        0      110 2023-09-12 16:07:16.000000 hist-2.7.2/tests/test_version.py
--rw-r--r--   0        0        0    20789 2023-09-12 16:07:16.000000 hist-2.7.2/tests/baseline/test_image_plot_pull.png
--rw-r--r--   0        0        0    19242 2023-09-12 16:07:16.000000 hist-2.7.2/tests/baseline/test_image_plot_ratio_callable.png
--rw-r--r--   0        0        0    13830 2023-09-12 16:07:16.000000 hist-2.7.2/tests/baseline/test_image_plot_ratio_hist.png
--rw-r--r--   0        0        0    19403 2023-09-12 16:07:16.000000 hist-2.7.2/tests/baseline/test_plot1d_auto_handling.png
--rw-r--r--   0        0        0     2148 2023-09-12 16:07:16.000000 hist-2.7.2/.gitignore
--rw-r--r--   0        0        0     1523 2023-09-12 16:07:16.000000 hist-2.7.2/LICENSE
--rw-r--r--   0        0        0    12956 2023-09-12 16:07:16.000000 hist-2.7.2/README.md
--rw-r--r--   0        0        0     5974 2023-09-12 16:07:16.000000 hist-2.7.2/pyproject.toml
--rw-r--r--   0        0        0    17244 2023-09-12 16:07:16.000000 hist-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0     3319 2024-05-29 07:46:56.000000 hist-2.7.3/.all-contributorsrc
+-rw-r--r--   0        0        0      125 2024-05-29 07:46:56.000000 hist-2.7.3/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-29 07:46:56.000000 hist-2.7.3/.gitattributes
+-rw-r--r--   0        0        0     1574 2024-05-29 07:46:56.000000 hist-2.7.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      456 2024-05-29 07:46:56.000000 hist-2.7.3/.readthedocs.yml
+-rw-r--r--   0        0        0      789 2024-05-29 07:46:56.000000 hist-2.7.3/CITATION.cff
+-rw-r--r--   0        0        0      412 2024-05-29 07:46:56.000000 hist-2.7.3/dev-environment.yml
+-rw-r--r--   0        0        0     3157 2024-05-29 07:46:56.000000 hist-2.7.3/noxfile.py
+-rw-r--r--   0        0        0     2543 2024-05-29 07:46:56.000000 hist-2.7.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      225 2024-05-29 07:46:56.000000 hist-2.7.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      169 2024-05-29 07:46:56.000000 hist-2.7.3/.github/labeler.yml
+-rw-r--r--   0        0        0       76 2024-05-29 07:46:56.000000 hist-2.7.3/.github/release.yml
+-rw-r--r--   0        0        0      268 2024-05-29 07:46:56.000000 hist-2.7.3/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      343 2024-05-29 07:46:56.000000 hist-2.7.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      399 2024-05-29 07:46:56.000000 hist-2.7.3/.github/ISSUE_TEMPLATE/docs-improvements.md
+-rw-r--r--   0        0        0      537 2024-05-29 07:46:56.000000 hist-2.7.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      227 2024-05-29 07:46:56.000000 hist-2.7.3/.github/ISSUE_TEMPLATE/support.md
+-rw-r--r--   0        0        0      668 2024-05-29 07:46:56.000000 hist-2.7.3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      936 2024-05-29 07:46:56.000000 hist-2.7.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1380 2024-05-29 07:46:56.000000 hist-2.7.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      229 2024-05-29 07:46:56.000000 hist-2.7.3/.github/workflows/pr.yml
+-rw-r--r--   0        0        0       76 2024-05-29 07:46:56.000000 hist-2.7.3/binder/postBuild
+-rw-r--r--   0        0        0      633 2024-05-29 07:46:56.000000 hist-2.7.3/docs/Makefile
+-rw-r--r--   0        0        0     2785 2024-05-29 07:46:56.000000 hist-2.7.3/docs/banner_slides.md
+-rw-r--r--   0        0        0    10124 2024-05-29 07:46:56.000000 hist-2.7.3/docs/changelog.md
+-rw-r--r--   0        0        0     2707 2024-05-29 07:46:56.000000 hist-2.7.3/docs/conf.py
+-rw-r--r--   0        0        0       44 2024-05-29 07:46:56.000000 hist-2.7.3/docs/contributing.md
+-rw-r--r--   0        0        0     4054 2024-05-29 07:46:56.000000 hist-2.7.3/docs/index.rst
+-rw-r--r--   0        0        0      794 2024-05-29 07:46:56.000000 hist-2.7.3/docs/make.bat
+-rw-r--r--   0        0        0      752 2024-05-29 07:46:56.000000 hist-2.7.3/docs/support.rst
+-rw-r--r--   0        0        0     3093 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/axis_category.png
+-rw-r--r--   0        0        0     5696 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/axis_circular.png
+-rw-r--r--   0        0        0     2349 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/axis_integer.png
+-rw-r--r--   0        0        0     2352 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/axis_regular.png
+-rw-r--r--   0        0        0     2599 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/axis_variable.png
+-rw-r--r--   0        0        0   278047 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/banner.gif
+-rw-r--r--   0        0        0    21774 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/ex_hist_density.png
+-rw-r--r--   0        0        0    62092 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/fullplot_example.png
+-rw-r--r--   0        0        0    18389 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/histlogo.png
+-rw-r--r--   0        0        0    94683 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/histlogo.svg
+-rw-r--r--   0        0        0    17543 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/histogram_design.png
+-rw-r--r--   0        0        0   301669 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/pieplot_example.png
+-rw-r--r--   0        0        0   114661 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/ratioplot_example.png
+-rw-r--r--   0        0        0    14396 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_images/stackplot_example.png
+-rw-r--r--   0        0        0       12 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_src/images/.gitignore
+-rw-r--r--   0        0        0      257 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_src/images/Makefile
+-rw-r--r--   0        0        0      979 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_src/images/axis_category.tex
+-rw-r--r--   0        0        0      983 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_src/images/axis_circular.tex
+-rw-r--r--   0        0        0      888 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_src/images/axis_integer.tex
+-rw-r--r--   0        0        0      912 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_src/images/axis_regular.tex
+-rw-r--r--   0        0        0      947 2024-05-29 07:46:56.000000 hist-2.7.3/docs/_src/images/axis_variable.tex
+-rw-r--r--   0        0        0     5913 2024-05-29 07:46:56.000000 hist-2.7.3/docs/examples/HistDemo.ipynb
+-rw-r--r--   0        0        0      139 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.accumulators.rst
+-rw-r--r--   0        0        0      130 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.axestuple.rst
+-rw-r--r--   0        0        0      194 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.axis.rst
+-rw-r--r--   0        0        0      145 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.axis.transform.rst
+-rw-r--r--   0        0        0      127 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.basehist.rst
+-rw-r--r--   0        0        0      136 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.classichist.rst
+-rw-r--r--   0        0        0      130 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.dask.hist.rst
+-rw-r--r--   0        0        0      145 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.dask.namedhist.rst
+-rw-r--r--   0        0        0      212 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.dask.rst
+-rw-r--r--   0        0        0      115 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.hist.rst
+-rw-r--r--   0        0        0      130 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.intervals.rst
+-rw-r--r--   0        0        0      130 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.namedhist.rst
+-rw-r--r--   0        0        0      118 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.numpy.rst
+-rw-r--r--   0        0        0      115 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.plot.rst
+-rw-r--r--   0        0        0      150 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.quick_construct.rst
+-rw-r--r--   0        0        0      506 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.rst
+-rw-r--r--   0        0        0      118 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.stack.rst
+-rw-r--r--   0        0        0      124 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.storage.rst
+-rw-r--r--   0        0        0      127 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.svgplots.rst
+-rw-r--r--   0        0        0      127 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.svgutils.rst
+-rw-r--r--   0        0        0      112 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.tag.rst
+-rw-r--r--   0        0        0      124 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/hist.version.rst
+-rw-r--r--   0        0        0       49 2024-05-29 07:46:56.000000 hist-2.7.3/docs/reference/modules.rst
+-rw-r--r--   0        0        0     5217 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/accumulators.rst
+-rw-r--r--   0        0        0     1318 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/analyses.rst
+-rw-r--r--   0        0        0     7451 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/axes.rst
+-rw-r--r--   0        0        0      134 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/cli.rst
+-rw-r--r--   0        0        0     1264 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/indexing.rst
+-rw-r--r--   0        0        0      603 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/installation.rst
+-rw-r--r--   0        0        0     3915 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/numpy.rst
+-rw-r--r--   0        0        0     5662 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/quickstart.rst
+-rw-r--r--   0        0        0     3587 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/storages.rst
+-rw-r--r--   0        0        0     2784 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/subclassing.rst
+-rw-r--r--   0        0        0    17509 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/notebooks/Histogram.ipynb
+-rw-r--r--   0        0        0     3908 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/notebooks/Interpolation.ipynb
+-rw-r--r--   0        0        0     8945 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/notebooks/Plots.ipynb
+-rw-r--r--   0        0        0     1680 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/notebooks/Reprs.ipynb
+-rw-r--r--   0        0        0    18694 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/notebooks/SVGHistogram.ipynb
+-rw-r--r--   0        0        0     5882 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/notebooks/Stack.ipynb
+-rw-r--r--   0        0        0     3853 2024-05-29 07:46:56.000000 hist-2.7.3/docs/user-guide/notebooks/Transform.ipynb
+-rw-r--r--   0        0        0    50203 2024-05-29 07:46:56.000000 hist-2.7.3/notebooks/HistLogo.ipynb
+-rw-r--r--   0        0        0     1717 2024-05-29 07:46:56.000000 hist-2.7.3/notebooks/axestuple-setattr.ipynb
+-rw-r--r--   0        0        0     1159 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/accumulators.py
+-rw-r--r--   0        0        0     2231 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/axestuple.py
+-rw-r--r--   0        0        0    22794 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/basehist.py
+-rw-r--r--   0        0        0     1431 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/classichist.py
+-rw-r--r--   0        0        0      126 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/hist.py
+-rw-r--r--   0        0        0     4114 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/interop.py
+-rw-r--r--   0        0        0     6893 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/intervals.py
+-rw-r--r--   0        0        0     5187 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/namedhist.py
+-rw-r--r--   0        0        0      161 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/numpy.py
+-rw-r--r--   0        0        0    23014 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/plot.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/py.typed
+-rw-r--r--   0        0        0    11131 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/quick_construct.py
+-rw-r--r--   0        0        0     5886 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/stack.py
+-rw-r--r--   0        0        0      323 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/storage.py
+-rw-r--r--   0        0        0     5502 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/svgplots.py
+-rw-r--r--   0        0        0     2274 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/svgutils.py
+-rw-r--r--   0        0        0      250 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/tag.py
+-rw-r--r--   0        0        0      411 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/version.py
+-rw-r--r--   0        0        0      118 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/version.pyi
+-rw-r--r--   0        0        0        0 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/_compat/__init__.py
+-rw-r--r--   0        0        0      759 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/_compat/builtins.py
+-rw-r--r--   0        0        0      619 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/_compat/typing.py
+-rw-r--r--   0        0        0     6994 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/axis/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/axis/py.typed
+-rw-r--r--   0        0        0      182 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/axis/transform.py
+-rw-r--r--   0        0        0      415 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/dask/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/dask/hist.py
+-rw-r--r--   0        0        0      325 2024-05-29 07:46:56.000000 hist-2.7.3/src/hist/dask/namedhist.py
+-rw-r--r--   0        0        0      742 2024-05-29 07:46:56.000000 hist-2.7.3/tests/conftest.py
+-rw-r--r--   0        0        0      691 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_axestuple.py
+-rw-r--r--   0        0        0     2078 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_axis.py
+-rw-r--r--   0        0        0      528 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_bh.py
+-rw-r--r--   0        0        0     4217 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_dask.py
+-rw-r--r--   0        0        0    30259 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_general.py
+-rw-r--r--   0        0        0    11430 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_interop.py
+-rw-r--r--   0        0        0     6204 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_intervals.py
+-rw-r--r--   0        0        0      981 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_mock_plot.py
+-rw-r--r--   0        0        0    25241 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_named.py
+-rw-r--r--   0        0        0    19787 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_plot.py
+-rw-r--r--   0        0        0     1040 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_profile.py
+-rw-r--r--   0        0        0     2714 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_reprs.py
+-rw-r--r--   0        0        0    12300 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_stacks.py
+-rw-r--r--   0        0        0      110 2024-05-29 07:46:56.000000 hist-2.7.3/tests/test_version.py
+-rw-r--r--   0        0        0    20789 2024-05-29 07:46:56.000000 hist-2.7.3/tests/baseline/test_image_plot_pull.png
+-rw-r--r--   0        0        0    19242 2024-05-29 07:46:56.000000 hist-2.7.3/tests/baseline/test_image_plot_ratio_callable.png
+-rw-r--r--   0        0        0    13830 2024-05-29 07:46:56.000000 hist-2.7.3/tests/baseline/test_image_plot_ratio_hist.png
+-rw-r--r--   0        0        0    19403 2024-05-29 07:46:56.000000 hist-2.7.3/tests/baseline/test_plot1d_auto_handling.png
+-rw-r--r--   0        0        0     2148 2024-05-29 07:46:56.000000 hist-2.7.3/.gitignore
+-rw-r--r--   0        0        0     1523 2024-05-29 07:46:56.000000 hist-2.7.3/LICENSE
+-rw-r--r--   0        0        0    12764 2024-05-29 07:46:56.000000 hist-2.7.3/README.md
+-rw-r--r--   0        0        0     5911 2024-05-29 07:46:56.000000 hist-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0    16988 2024-05-29 07:46:56.000000 hist-2.7.3/PKG-INFO
```

### Comparing `hist-2.7.2/.all-contributorsrc` & `hist-2.7.3/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/.pre-commit-config.yaml` & `hist-2.7.3/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,62 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
+  autoupdate_schedule: monthly
 
 repos:
-- repo: https://github.com/psf/black-pre-commit-mirror
-  rev: 23.9.1
-  hooks:
-  - id: black-jupyter
-
 - repo: https://github.com/adamchainz/blacken-docs
   rev: "1.16.0"
   hooks:
   - id: blacken-docs
-    additional_dependencies: [black==23.7.0]
+    additional_dependencies: [black==23.*]
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.6.0
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.0.288
+  rev: v0.4.5
   hooks:
   - id: ruff
     args: ["--fix", "--show-fixes"]
-
-# Notebook formatting
-- repo: https://github.com/nbQA-dev/nbQA
-  rev: 1.7.0
-  hooks:
-  - id: nbqa-ruff
-    additional_dependencies: [ruff==0.0.255]
-    args: ["--extend-ignore=B008,T20,I002,E402", "--fix", "--show-fixes"]
+    types_or: [python, pyi, jupyter]
+  - id: ruff-format
+    types_or: [python, pyi, jupyter]
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.5.1
+  rev: v1.10.0
   hooks:
   - id: mypy
     files: ^src
     args: []
-    additional_dependencies: ["numpy~=1.24.0", "matplotlib>=3.4", "boost-histogram~=1.3.1", "uhi~=0.3.1", "pandas-stubs>=2.0.1.230501"]
+    additional_dependencies: ["numpy~=1.26.0", "matplotlib>=3.4", "boost-histogram~=1.4.0", "uhi~=0.3.1", "pandas-stubs>=2.0.1.230501"]
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.5
+  rev: v2.3.0
   hooks:
   - id: codespell
     args: ["-Lhist,gaus,nd"]
     exclude: ^notebooks/HistLogo.ipynb$
 
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
   - id: python-use-type-annotations
   - id: rst-backticks
   - id: rst-directive-colons
   - id: rst-inline-touching-normal
 
 - repo: https://github.com/shellcheck-py/shellcheck-py
-  rev: v0.9.0.5
+  rev: v0.10.0.1
   hooks:
   - id: shellcheck
```

### Comparing `hist-2.7.2/CITATION.cff` & `hist-2.7.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/noxfile.py` & `hist-2.7.3/noxfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import argparse
 import shutil
 import sys
 from pathlib import Path
 
 import nox
 
-ALL_PYTHONS = ["3.7", "3.8", "3.9", "3.10", "3.11"]
-
+nox.needs_version = ">=2024.3.2"
 nox.options.sessions = ["lint", "tests"]
-
+nox.options.default_venv_backend = "uv|virtualenv"
 
 DIR = Path(__file__).parent.resolve()
 
 
 @nox.session(reuse_venv=True)
 def lint(session):
     """
@@ -31,15 +30,15 @@
     """
 
     session.install("pylint~=2.17.0")
     session.install("-e.")
     session.run("pylint", "hist", *session.posargs)
 
 
-@nox.session(python=ALL_PYTHONS, reuse_venv=True)
+@nox.session(reuse_venv=True)
 def tests(session):
     """
     Run the unit and regular tests.
     """
     session.install("-e", ".[test,plot]")
     args = ["--mpl"] if sys.platform.startswith("linux") else []
     session.run("pytest", *args, *session.posargs)
@@ -98,20 +97,17 @@
 
 @nox.session(reuse_venv=True)
 def build(session):
     """
     Build an SDist and wheel.
     """
 
-    build_p = DIR.joinpath("build")
-    if build_p.exists():
-        shutil.rmtree(build_p)
-
-    session.install("build")
-    session.run("python", "-m", "build")
+    args = [] if shutil.which("uv") else ["uv"]
+    session.install("build==1.2.0", *args)
+    session.run("python", "-m", "build", "--installer=uv")
 
 
 @nox.session()
 def boost(session):
     """
     Build against latest boost-histogram.
     """
@@ -126,10 +122,10 @@
             "--recursive",
             "https://github.com/scikit-hep/boost-histogram",
             external=True,
         )
         session.chdir("boost-histogram")
         session.install(".")
     session.chdir(DIR)
-    session.install("-e.[test,plot]")
+    session.install("-e.[test,plot]", "pip")
     session.run("pip", "list")
     session.run("pytest", *session.posargs)
```

### Comparing `hist-2.7.2/.github/CONTRIBUTING.md` & `hist-2.7.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/.github/ISSUE_TEMPLATE/feature_request.md` & `hist-2.7.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/.github/matchers/pylint.json` & `hist-2.7.3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/.github/workflows/cd.yml` & `hist-2.7.3/.github/workflows/cd.yml`

 * *Files 26% similar despite different names*

```diff
@@ -13,27 +13,34 @@
   dist:
     runs-on: ubuntu-22.04
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
-    - uses: hynek/build-and-inspect-python-package@v1
+    - uses: hynek/build-and-inspect-python-package@v2
 
 
   publish:
     needs: [dist]
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
     environment:
       name: pypi
       url: https://pypi.org/p/hist
     permissions:
       id-token: write
+      attestations: write
+      contents: read
 
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
       with:
         name: Packages
         path: dist
 
+    - name: Generate artifact attestation for sdist and wheel
+      uses: actions/attest-build-provenance@173725a1209d09b31f9d30a3890cf2757ebbff0d # v1.1.2
+      with:
+        subject-path: "dist/hist-*"
+
     - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `hist-2.7.2/.github/workflows/ci.yml` & `hist-2.7.3/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -10,56 +10,62 @@
   FORCE_COLOR: 3
 
 concurrency:
   group: ${ github.workflow }-${ github.ref }
   cancel-in-progress: true
 
 jobs:
-  pre-commit:
+  pylint:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
-    - uses: actions/setup-python@v4
+    - name: Setup uv
+      uses: yezz123/setup-uv@v4
       with:
-        python-version: "3.x"
-    - uses: pre-commit/action@v3.0.0
+        uv-venv: ".venv"
+    - name: Install nox
+      run: uv pip install nox
     - name: PyLint
       run: |
         echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"
-        pipx run nox -s pylint
+        nox -s pylint
 
   checks:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version:
         - "3.7"
         - "3.8"
         - "3.9"
         - "3.10"
         - "3.11"
         - "3.12"
+
     name: Check Python ${{ matrix.python-version }}
     steps:
     - uses: actions/checkout@v4
 
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         allow-prereleases: true
 
+    - name: Setup uv
+      uses: yezz123/setup-uv@v4
+      with:
+        uv-venv: ".venv"
+
     - name: Requirements check
-      run: python -m pip list
+      run: uv pip list
 
     - name: Install package
-      run: python -m pip install -e ".[test]"
+      run: uv pip install -e ".[test]"
 
     - name: Test package
       run: python -m pytest
 
     - name: Install plotting requirements too
-      if: matrix.python-version != '3.12'
-      run: python -m pip install -e ".[test,plot]"
+      run: uv pip install -e ".[test,plot]"
 
     - name: Test plotting too
-      if: matrix.python-version != '3.12'
       run: python -m pytest --mpl
```

### Comparing `hist-2.7.2/docs/Makefile` & `hist-2.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/banner_slides.md` & `hist-2.7.3/docs/banner_slides.md`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/changelog.md` & `hist-2.7.3/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,40 @@
 # Changelog
 
+## Version 2.7.3
+
+This release fixes an issue with Python 3.12 pulling in NumPy 2 pre-releases.
+
+Fixes:
+
+* Sample required error message
+  [#538](https://github.com/scikit-hep/hist/pull/538)
+* `hist.dask.new` to match top-level package
+  [#563](https://github.com/scikit-hep/hist/pull/563)
+
+Docs:
+
+* Clarify sample term required for Mean storage
+  [#536](https://github.com/scikit-hep/hist/pull/536)
+
+CI:
+
+* Move to using Ruff Jupyter support
+  [#543](https://github.com/scikit-hep/hist/pull/543)
+* Move to using Ruff formatter
+  [#544](https://github.com/scikit-hep/hist/pull/544)
+* Group dependabot updates
+  [#554](https://github.com/scikit-hep/hist/pull/554)
+* Use uv
+  [#564](https://github.com/scikit-hep/hist/pull/564)
+* Add GitHub artifact attestations to package distribution
+  [#568](https://github.com/scikit-hep/hist/pull/568)
+* Reduce update frequency
+  [#571](https://github.com/scikit-hep/hist/pull/571)
+
 ## Version 2.7.2
 
 * Support boost-histogram 1.4.0 in addition to 1.3.x, including Python 3.12,
   flow disabling for categories, and integer arrays required for integer axes
   [#535](https://github.com/scikit-hep/hist/pull/535) and
   [#532](https://github.com/scikit-hep/hist/pull/532)
 * Add a `.T` shortcut
```

### Comparing `hist-2.7.2/docs/conf.py` & `hist-2.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/index.rst` & `hist-2.7.3/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    :width: 60%
    :alt: Hist logo
    :align: center
 
 Welcome to Hist's documentation!
 ================================
 
-|Actions Status| |Documentation Status| |pre-commit.ci Status| |Code style: black| |PyPI version|
+|Actions Status| |Documentation Status| |pre-commit.ci Status| |PyPI version|
 |Conda-Forge| |PyPI platforms| |DOI| |License| |GitHub Discussion| |Gitter| |Binder| |Scikit-HEP|
 
 Introduction
 ------------
 
 `Hist <https://github.com/scikit-hep/hist>`_ is a powerful Histogramming tool for analysis based on `boost-histogram <https://boost-histogram.readthedocs.io/en/latest/index.html>`_ (the Python binding of the Histogram library in Boost). It is a friendly analysis-focused project that uses `boost-histogram <https://boost-histogram.readthedocs.io/en/latest/index.html>`_ as a backend to do the work, but provides plotting tools, shortcuts, and new ideas.
 
@@ -77,16 +77,14 @@
 
 .. |Actions Status| image:: https://github.com/scikit-hep/hist/workflows/CI/badge.svg
    :target: https://github.com/scikit-hep/hist/actions
 .. |Documentation Status| image:: https://readthedocs.org/projects/hist/badge/?version=latest
    :target: https://hist.readthedocs.io/en/latest/?badge=latest
 .. |pre-commit.ci Status| image:: https://results.pre-commit.ci/badge/github/scikit-hep/hist/main.svg
    :target: https://results.pre-commit.ci/repo/github/scikit-hep/hist
-.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
 .. |PyPI version| image:: https://badge.fury.io/py/hist.svg
    :target: https://pypi.org/project/hist/
 .. |Conda-Forge| image:: https://img.shields.io/conda/vn/conda-forge/hist
    :target: https://github.com/conda-forge/hist-feedstock
 .. |PyPI platforms| image:: https://img.shields.io/pypi/pyversions/hist
    :target: https://pypi.org/project/hist/
 .. |DOI| image:: https://zenodo.org/badge/239605861.svg
```

### Comparing `hist-2.7.2/docs/make.bat` & `hist-2.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/support.rst` & `hist-2.7.3/docs/support.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/axis_category.png` & `hist-2.7.3/docs/_images/axis_category.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/axis_circular.png` & `hist-2.7.3/docs/_images/axis_circular.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/axis_integer.png` & `hist-2.7.3/docs/_images/axis_integer.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/axis_regular.png` & `hist-2.7.3/docs/_images/axis_regular.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/axis_variable.png` & `hist-2.7.3/docs/_images/axis_variable.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/banner.gif` & `hist-2.7.3/docs/_images/banner.gif`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/ex_hist_density.png` & `hist-2.7.3/docs/_images/ex_hist_density.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/fullplot_example.png` & `hist-2.7.3/docs/_images/fullplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/histlogo.png` & `hist-2.7.3/docs/_images/histlogo.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/histlogo.svg` & `hist-2.7.3/docs/_images/histlogo.svg`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/histogram_design.png` & `hist-2.7.3/docs/_images/histogram_design.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/pieplot_example.png` & `hist-2.7.3/docs/_images/pieplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/ratioplot_example.png` & `hist-2.7.3/docs/_images/ratioplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_images/stackplot_example.png` & `hist-2.7.3/docs/_images/stackplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_src/images/axis_category.tex` & `hist-2.7.3/docs/_src/images/axis_category.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_src/images/axis_circular.tex` & `hist-2.7.3/docs/_src/images/axis_circular.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_src/images/axis_integer.tex` & `hist-2.7.3/docs/_src/images/axis_integer.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_src/images/axis_regular.tex` & `hist-2.7.3/docs/_src/images/axis_regular.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/_src/images/axis_variable.tex` & `hist-2.7.3/docs/_src/images/axis_variable.tex`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/examples/HistDemo.ipynb` & `hist-2.7.3/docs/examples/HistDemo.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/accumulators.rst` & `hist-2.7.3/docs/user-guide/accumulators.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/analyses.rst` & `hist-2.7.3/docs/user-guide/analyses.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/axes.rst` & `hist-2.7.3/docs/user-guide/axes.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/indexing.rst` & `hist-2.7.3/docs/user-guide/indexing.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/installation.rst` & `hist-2.7.3/docs/user-guide/installation.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/numpy.rst` & `hist-2.7.3/docs/user-guide/numpy.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/quickstart.rst` & `hist-2.7.3/docs/user-guide/quickstart.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/storages.rst` & `hist-2.7.3/docs/user-guide/storages.rst`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,14 @@
 
 
 Mean
 ^^^^
 
 This storage tracks a "Profile", that is, the mean value of the accumulation instead of the sum.
 It stores the count (as a double), the mean, and a term that is used to compute the variance. When
-filling, you can add a ``sample=`` term.
+filling, you must add a ``sample=`` term.
 
 
 WeightedMean
 ^^^^^^^^^^^^
 
 This is similar to Mean, but also keeps track a sum of weights like term as well.
```

### Comparing `hist-2.7.2/docs/user-guide/subclassing.rst` & `hist-2.7.3/docs/user-guide/subclassing.rst`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/notebooks/Histogram.ipynb` & `hist-2.7.3/docs/user-guide/notebooks/Histogram.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/notebooks/Interpolation.ipynb` & `hist-2.7.3/docs/user-guide/notebooks/Interpolation.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/notebooks/Plots.ipynb` & `hist-2.7.3/docs/user-guide/notebooks/Plots.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/notebooks/Reprs.ipynb` & `hist-2.7.3/docs/user-guide/notebooks/Reprs.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/notebooks/SVGHistogram.ipynb` & `hist-2.7.3/docs/user-guide/notebooks/SVGHistogram.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999666666666667%*

 * *Differences: {"'cells'": "{22: {'source': {insert: [(56, '    return svg(*polygons, *texts, *circles, "*

 * *            "width=800, height=250)')], delete: [58, 57, 56]}}}"}*

```diff
@@ -571,17 +571,15 @@
                 "            ),\n",
                 "            x=140,\n",
                 "            y=125 + 100 * max(norm_vals),\n",
                 "            style=\"font-family: monospace\",\n",
                 "        ),\n",
                 "    ]\n",
                 "\n",
-                "    return svg(*polygons, *texts, *circles, width=800, height=250)\n",
-                "    pass\n",
-                "    return None"
+                "    return svg(*polygons, *texts, *circles, width=800, height=250)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `hist-2.7.2/docs/user-guide/notebooks/Stack.ipynb` & `hist-2.7.3/docs/user-guide/notebooks/Stack.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/docs/user-guide/notebooks/Transform.ipynb` & `hist-2.7.3/docs/user-guide/notebooks/Transform.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/notebooks/HistLogo.ipynb` & `hist-2.7.3/notebooks/HistLogo.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/notebooks/axestuple-setattr.ipynb` & `hist-2.7.3/notebooks/axestuple-setattr.ipynb`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/src/hist/__init__.py` & `hist-2.7.3/src/hist/__init__.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/src/hist/axestuple.py` & `hist-2.7.3/src/hist/axestuple.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         return super().__getitem__(item)
 
     @property
     def name(self) -> tuple[str]:
         """
         The names of the axes. May be empty strings.
         """
-        return tuple(ax.name for ax in self)  # type: ignore[return-value]
+        return tuple(ax.name for ax in self)
 
     @name.setter
     def name(self, values: Iterable[str]) -> None:
         # strict = True from Python 3.10
         for ax, val in zip(self, values, strict=True):
             ax._ax.metadata["name"] = val
 
@@ -68,8 +68,8 @@
 
     @property
     def label(self) -> tuple[str]:
         """
         The labels of the axes. Defaults to name if label not given, or Axis N
         if neither was given.
         """
-        return tuple(ax.label for ax in self)  # type: ignore[return-value]
+        return tuple(ax.label for ax in self)
```

### Comparing `hist-2.7.2/src/hist/basehist.py` & `hist-2.7.3/src/hist/basehist.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     import matplotlib.axes
     from mplhep.plot import Hist1DArtists, Hist2DArtists
 
     from .plot import FitResultArtists, MainAxisArtists, RatiolikeArtists
 
 
 class SupportsLessThan(Protocol):
-    def __lt__(self, __other: Any) -> bool:
-        ...
+    def __lt__(self, __other: Any) -> bool: ...
 
 
 InnerIndexing = Union[
     SupportsIndex, str, Callable[[bh.axis.Axis], int], slice, "ellipsis"
 ]
 IndexingWithMapping = Union[InnerIndexing, Mapping[Union[int, str], InnerIndexing]]
 IndexingExpr = Union[IndexingWithMapping, Tuple[IndexingWithMapping, ...]]
@@ -227,14 +226,21 @@
         **kwargs: ArrayLike,
     ) -> Self:
         """
         Insert data into the histogram using names and indices, return
         a Hist object.
         """
 
+        if (
+            issubclass(self.storage_type, (bh.storage.Mean, bh.storage.WeightedMean))
+            and sample is None
+        ):
+            msg = "A Mean-based storage requires a sample= argument with the values to average"
+            raise TypeError(msg)
+
         data_dict = {
             self._name_to_index(k) if isinstance(k, str) else k: v  # type: ignore[redundant-expr]
             for k, v in kwargs.items()
         }
 
         if set(data_dict) != set(range(len(args), self.ndim)):
             raise TypeError(
```

### Comparing `hist-2.7.2/src/hist/classichist.py` & `hist-2.7.3/src/hist/classichist.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/src/hist/interop.py` & `hist-2.7.3/src/hist/interop.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,21 +9,19 @@
 
 T_contra = TypeVar("T_contra", contravariant=True)
 U = TypeVar("U")
 V = TypeVar("V")
 
 
 class HistogramModuleProtocol(Protocol[T_contra, U]):
-    def unpack(self, obj: T_contra) -> dict[str, U] | None:
-        ...
+    def unpack(self, obj: T_contra) -> dict[str, U] | None: ...
 
     def broadcast_and_flatten(
         self, objects: Sequence[U | ArrayLike]
-    ) -> tuple[np.typing.NDArray[Any], ...]:
-        ...
+    ) -> tuple[np.typing.NDArray[Any], ...]: ...
 
 
 _histogram_modules: dict[type, HistogramModuleProtocol[Any, Any]] = {}
 
 
 def histogram_module_for(
     cls: type,
```

### Comparing `hist-2.7.2/src/hist/intervals.py` & `hist-2.7.3/src/hist/intervals.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/src/hist/namedhist.py` & `hist-2.7.3/src/hist/namedhist.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/src/hist/plot.py` & `hist-2.7.3/src/hist/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             continue
         if ix < len(g) - 1 and g[ix + 1][1] in {".", "("}:
             continue
         varnames.append(tokval)
     varnames = list(OrderedDict.fromkeys([name for name in varnames if name != "x"]))
     lambdastr = f"lambda x,{','.join(varnames)}: {expr}"
     # pylint: disable-next=eval-used
-    return eval(lambdastr)  # type: ignore[no-any-return]  # noqa: PGH001
+    return eval(lambdastr)  # type: ignore[no-any-return]
 
 
 def _curve_fit_wrapper(
     func: Callable[..., Any],
     xdata: np.typing.NDArray[Any],
     ydata: np.typing.NDArray[Any],
     yerr: np.typing.NDArray[Any],
@@ -189,15 +189,15 @@
 def _plot_keywords_wrapper(ax: matplotlib.axes.Axes, legend: bool | None) -> None:
     """
     Pandas-like wrapper that wrap several useful mpl keyword arguments.
     """
     # Todo: more keywords here
     if legend:
         if ax.get_legend_handles_labels()[0]:
-            legend = ax.legend()
+            ax.legend()
         else:
             raise ValueError("No labels to legend")
 
 
 def plot2d_full(
     self: hist.BaseHist,
     *,
@@ -513,15 +513,16 @@
         )
         ax.add_patch(upRect)
         downRect_startpoint = (left_edge, -(i + 1) * patch_height)
         downRect = patches.Rectangle(
             downRect_startpoint, patch_width, patch_height, **pp_kwargs
         )
         ax.add_patch(downRect)
-        patch_artists.append((downRect, upRect))
+        patch_artists.append(downRect)
+        patch_artists.append(upRect)
 
     ax.set_xlim(left_edge, right_edge)
 
     ax.set_xlabel(__hist.axes[0].label)
     ax.set_ylabel("Pull")
 
     return PullArtists(bar_artists, patch_artists)
```

### Comparing `hist-2.7.2/src/hist/quick_construct.py` & `hist-2.7.3/src/hist/quick_construct.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/src/hist/stack.py` & `hist-2.7.3/src/hist/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,20 +68,18 @@
         for n, h in enumerate(self._stack):
             if h.name == name:
                 return n
 
         raise IndexError(f"Name not found: {name}")
 
     @typing.overload
-    def __getitem__(self, val: int | str) -> BaseHist:
-        ...
+    def __getitem__(self, val: int | str) -> BaseHist: ...
 
     @typing.overload
-    def __getitem__(self, val: slice) -> Self:
-        ...
+    def __getitem__(self, val: slice) -> Self: ...
 
     def __getitem__(self, val: int | slice | str) -> BaseHist | Self:
         if isinstance(val, str):
             val = self._get_index(val)
         if isinstance(val, slice):
             my_slice = slice(
                 self._get_index(val.start), self._get_index(val.stop), val.step
```

### Comparing `hist-2.7.2/src/hist/svgplots.py` & `hist-2.7.3/src/hist/svgplots.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 
     (edges,) = h.axes.edges
     norm_edges = (edges - edges[0]) / (edges[-1] - edges[0])
     density = h.density()
     max_dens = np.amax(density) or 1
     norm_vals: np.typing.NDArray[Any] = density / max_dens
 
-    arr = np.empty((2, len(norm_vals) * 2 + 2), dtype=float)
+    arr: np.typing.NDArray[np.float64] = np.empty(
+        (2, len(norm_vals) * 2 + 2), dtype=float
+    )
     arr[0, 0:-1:2] = arr[0, 1::2] = width * norm_edges
     arr[1, 1:-2:2] = arr[1, 2:-1:2] = -height * norm_vals
     arr[1, 0] = arr[1, -1] = 0
 
     points = " ".join(f"{x:3g},{y:.3g}" for x, y in arr.T)
     bins = polyline(points=points, style="fill:none; stroke:currentColor;")
 
@@ -118,15 +120,15 @@
 
     (edges,) = h.axes.edges
     norm_edges = (edges - edges[0]) / (edges[-1] - edges[0]) * np.pi * 2
     density = h.density()
     max_dens = np.amax(density) or 1
     norm_vals: np.typing.NDArray[Any] = density / max_dens
 
-    arr = np.empty((2, len(norm_vals) * 2), dtype=float)
+    arr: np.typing.NDArray[np.float64] = np.empty((2, len(norm_vals) * 2), dtype=float)
     arr[0, :-1:2] = arr[0, 1::2] = norm_edges[:-1]
     arr[1, :-1:2] = arr[1, 1::2] = inner_radius + norm_vals * (radius - inner_radius)
     arr[1] = np.roll(arr[1], shift=1)
 
     xs = arr[1] * np.cos(arr[0])
     ys = arr[1] * np.sin(arr[0])
```

### Comparing `hist-2.7.2/src/hist/svgutils.py` & `hist-2.7.3/src/hist/svgutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from ._compat.typing import Protocol, Self
 
 
 class SupportsStr(Protocol):
-    def __str__(self) -> str:
-        ...
+    def __str__(self) -> str: ...
 
 
 class XML:
     def __init__(self, *contents: XML | SupportsStr, **kargs: SupportsStr) -> None:
         self.properties = kargs
         self.contents = contents
```

### Comparing `hist-2.7.2/src/hist/_compat/builtins.py` & `hist-2.7.3/src/hist/_compat/builtins.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/src/hist/_compat/typing.py` & `hist-2.7.3/src/hist/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/src/hist/axis/__init__.py` & `hist-2.7.3/src/hist/axis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
-from typing import Any, Iterable
+import typing
+from collections.abc import Iterable
+from typing import Any
 
 import boost_histogram as bh
 import boost_histogram.axis as bha
 
 import hist
 
 from .._compat.typing import Protocol
@@ -34,16 +36,15 @@
     metadata: dict[str, Any]
 
 
 class AxisProtocol(Protocol):
     metadata: Any
 
     @property
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
     label: str
     _ax: CoreAxisProtocol
 
 
 class AxesMixin:
     __slots__ = ()
@@ -53,15 +54,15 @@
         super().__init_subclass__(**kwargs)
 
     @property
     def name(self: AxisProtocol) -> str:
         """
         Get the name for the Regular axis
         """
-        return self._ax.metadata.get("name", "")
+        return typing.cast(str, self._ax.metadata.get("name", ""))
 
     @property
     def label(self: AxisProtocol) -> str:
         """
         Get or set the label for the Regular axis
         """
         return self._ax.metadata.get("label", "") or self.name
```

### Comparing `hist-2.7.2/tests/conftest.py` & `hist-2.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_axestuple.py` & `hist-2.7.3/tests/test_axestuple.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_axis.py` & `hist-2.7.3/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_bh.py` & `hist-2.7.3/tests/test_bh.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_dask.py` & `hist-2.7.3/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_general.py` & `hist-2.7.3/tests/test_general.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import numpy as np
 import pytest
 from pytest import approx
 
 import hist
 from hist import Hist, axis, storage
 
+BHV = tuple(int(x) for x in bh.__version__.split(".")[:2])
+
 # TODO: specify what error is raised
 
 
 def test_init_and_fill(unnamed_hist):
     """
     Test general init -- whether Hist can be properly initialized.
     Also tests filling.
@@ -107,15 +109,15 @@
 
     with pytest.raises(Exception):
         named_hist(
             axis.StrCategory("TF", name="y"), axis.StrCategory(["T", "F"], name="y")
         )
 
 
-def test_general_fill():
+def test_general_fill_regular():
     """
     Test general fill -- whether Hist can be properly filled.
     """
 
     # Regular
     h = Hist(
         axis.Regular(10, 0, 1, name="x"),
@@ -133,14 +135,16 @@
             if idx_x == 3 and idx_y == 4 or idx_x == 4 and idx_y == 4:
                 assert z_one_only[idx_x, idx_y] == 1
             elif idx_x == 5 and idx_y == 4:
                 assert z_one_only[idx_x, idx_y] == 3
             else:
                 assert z_one_only[idx_x, idx_y] == 0
 
+
+def test_general_fill_bool():
     # Boolean
     h = Hist(
         axis.Boolean(name="x"),
         axis.Boolean(name="y"),
         axis.Boolean(name="z"),
     ).fill(
         [True, True, True, True, True, False, True],
@@ -150,15 +154,16 @@
 
     z_one_only = h[{2: bh.loc(True)}]
     assert z_one_only[False, False] == 0
     assert z_one_only[False, True] == 1
     assert z_one_only[True, False] == 3
     assert z_one_only[True, True] == 1
 
-    # Variable
+
+def test_general_fill_variable():
     h = Hist(
         axis.Variable(range(11), name="x"),
         axis.Variable(range(11), name="y"),
         axis.Variable(range(3), name="z"),
     ).fill(
         x=[3.5, 3.5, 3.5, 4.5, 5.5, 5.5, 5.5],
         y=[3.5, 3.5, 4.5, 4.5, 4.5, 4.5, 4.5],
@@ -171,15 +176,16 @@
             if idx_x == 3 and idx_y == 4 or idx_x == 4 and idx_y == 4:
                 assert z_one_only[idx_x, idx_y] == 1
             elif idx_x == 5 and idx_y == 4:
                 assert z_one_only[idx_x, idx_y] == 3
             else:
                 assert z_one_only[idx_x, idx_y] == 0
 
-    # Integer
+
+def test_general_fill_integer():
     h = Hist(
         axis.Integer(0, 10, name="x"),
         axis.Integer(0, 10, name="y"),
         axis.Integer(0, 2, name="z"),
     ).fill(
         [3, 3, 3, 4, 5, 5, 5],
         [3, 3, 4, 4, 4, 4, 4],
@@ -192,61 +198,72 @@
             if idx_x == 3 and idx_y == 4 or idx_x == 4 and idx_y == 4:
                 assert z_one_only[idx_x, idx_y] == 1
             elif idx_x == 5 and idx_y == 4:
                 assert z_one_only[idx_x, idx_y] == 3
             else:
                 assert z_one_only[idx_x, idx_y] == 0
 
-    # IntCategory
+
+def test_general_fill_int_cat():
     h = Hist(
-        axis.IntCategory(range(10), name="x", flow=False),
-        axis.IntCategory(range(10), name="y", overflow=False),
+        axis.IntCategory(range(10), name="x", flow=BHV < (1, 4)),
+        axis.IntCategory(range(10), name="y", overflow=BHV < (1, 4)),
         axis.IntCategory(range(2), name="z"),
     ).fill(
         x=[3, 3, 3, 4, 5, 5, 5],
         y=[3, 3, 4, 4, 4, 4, 4],
         z=[0, 0, 1, 1, 1, 1, 1],
     )
 
-    assert not h.axes[0].traits.overflow
-    assert not h.axes[1].traits.overflow
+    if BHV < (1, 4):
+        assert h.axes[0].traits.overflow
+        assert h.axes[1].traits.overflow
+    else:
+        assert not h.axes[0].traits.overflow
+        assert not h.axes[1].traits.overflow
     assert h.axes[2].traits.overflow
 
     z_one_only = h[{2: bh.loc(1)}]
     for idx_x in range(10):
         for idx_y in range(10):
             if idx_x == 3 and idx_y == 4 or idx_x == 4 and idx_y == 4:
                 assert z_one_only[idx_x, idx_y] == 1
             elif idx_x == 5 and idx_y == 4:
                 assert z_one_only[idx_x, idx_y] == 3
             else:
                 assert z_one_only[idx_x, idx_y] == 0
 
-    # StrCategory
+
+def test_general_fill_str_cat():
     h = Hist(
-        axis.StrCategory("FT", name="x", flow=False),
-        axis.StrCategory(list("FT"), name="y", overflow=False),
+        axis.StrCategory("FT", name="x", flow=BHV < (1, 4)),
+        axis.StrCategory(list("FT"), name="y", overflow=BHV < (1, 4)),
         axis.StrCategory(["F", "T"], name="z"),
     ).fill(
         ["T", "T", "T", "T", "T", "F", "T"],
         ["F", "T", "T", "F", "F", "T", "F"],
         ["F", "F", "T", "T", "T", "T", "T"],
     )
 
-    assert not h.axes[0].traits.overflow
-    assert not h.axes[1].traits.overflow
+    if BHV < (1, 4):
+        assert h.axes[0].traits.overflow
+        assert h.axes[1].traits.overflow
+    else:
+        assert not h.axes[0].traits.overflow
+        assert not h.axes[1].traits.overflow
     assert h.axes[2].traits.overflow
 
     z_one_only = h[{2: bh.loc("T")}]
     assert z_one_only[bh.loc("F"), bh.loc("F")] == 0
     assert z_one_only[bh.loc("F"), bh.loc("T")] == 1
     assert z_one_only[bh.loc("T"), bh.loc("F")] == 3
     assert z_one_only[bh.loc("T"), bh.loc("T")] == 1
 
-    # with names
+
+def test_general_fill_names():
     assert Hist(
         axis.Regular(50, -3, 3, name="x"), axis.Regular(50, -3, 3, name="y")
     ).fill(x=np.random.randn(10), y=np.random.randn(10))
 
     assert Hist(axis.Boolean(name="x"), axis.Boolean(name="y")).fill(
         x=[True, False, True], y=[True, False, True]
     )
@@ -264,15 +281,15 @@
         axis.IntCategory(range(-3, 3), name="y"),
     ).fill(x=np.random.randint(-3, 3, 10), y=np.random.randint(-3, 3, 10))
 
     assert Hist(
         axis.StrCategory(["F", "T"], name="x"), axis.StrCategory("FT", name="y")
     ).fill(x=["T", "F", "T"], y=["T", "F", "T"])
 
-    h = Hist(
+    Hist(
         axis.Regular(
             50, -4, 4, name="X", label="s [units]", underflow=False, overflow=False
         )
     ).fill(np.random.normal(size=10))
 
 
 def test_general_access():
@@ -286,15 +303,15 @@
 
     assert h[6] == h[bh.loc(1)] == h[1j] == h[0j + 1] == h[-3j + 4] == h[bh.loc(1, 0)]
     h[6] = h[bh.loc(1)] = h[1j] = h[0j + 1] = h[-3j + 4] = h[bh.loc(1, 0)] = 0
 
     h = Hist(
         axis.Regular(50, -5, 5, name="Norm", label="normal distribution"),
         axis.Regular(50, -5, 5, name="Unif", label="uniform distribution"),
-        axis.StrCategory(["hi", "hello"], name="Greet", flow=False),
+        axis.StrCategory(["hi", "hello"], name="Greet", flow=BHV < (1, 4)),
         axis.Boolean(name="Yes"),
         axis.Integer(0, 1000, name="Int"),
     ).fill(
         np.random.normal(size=1000),
         np.random.uniform(size=1000),
         ["hi"] * 800 + ["hello"] * 200,
         [True] * 600 + [False] * 400,
```

### Comparing `hist-2.7.2/tests/test_interop.py` & `hist-2.7.3/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_intervals.py` & `hist-2.7.3/tests/test_intervals.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_mock_plot.py` & `hist-2.7.3/tests/test_mock_plot.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_named.py` & `hist-2.7.3/tests/test_named.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_plot.py` & `hist-2.7.3/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_profile.py` & `hist-2.7.3/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_reprs.py` & `hist-2.7.3/tests/test_reprs.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/test_stacks.py` & `hist-2.7.3/tests/test_stacks.py`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/baseline/test_image_plot_pull.png` & `hist-2.7.3/tests/baseline/test_image_plot_pull.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/baseline/test_image_plot_ratio_callable.png` & `hist-2.7.3/tests/baseline/test_image_plot_ratio_callable.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/baseline/test_image_plot_ratio_hist.png` & `hist-2.7.3/tests/baseline/test_image_plot_ratio_hist.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/tests/baseline/test_plot1d_auto_handling.png` & `hist-2.7.3/tests/baseline/test_plot1d_auto_handling.png`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/.gitignore` & `hist-2.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/LICENSE` & `hist-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hist-2.7.2/README.md` & `hist-2.7.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 <img alt="histogram" width="200" src="https://raw.githubusercontent.com/scikit-hep/hist/main/docs/_images/histlogo.png"/>
 
 # Hist
 
 [![Actions Status][actions-badge]][actions-link]
 [![Documentation Status][rtd-badge]][rtd-link]
 [![pre-commit.ci status][pre-commit-badge]][pre-commit-link]
-[![Code style: black][black-badge]][black-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda-Forge][conda-badge]][conda-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 [![DOI][doi-badge]][doi-link]
 [![License][license-badge]][license-link]
 
@@ -178,16 +177,14 @@
 
 Support for this work was provided by the National Science Foundation cooperative agreement OAC-1836650 (IRIS-HEP) and OAC-1450377 (DIANA/HEP). Any opinions, findings, conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
 [actions-badge]:            https://github.com/scikit-hep/hist/workflows/CI/badge.svg
 [actions-link]:             https://github.com/scikit-hep/hist/actions
 [binder-badge]:             https://mybinder.org/badge_logo.svg
 [binder-link]:              https://mybinder.org/v2/gh/scikit-hep/hist/HEAD
-[black-badge]:              https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]:               https://github.com/psf/black
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/hist
 [conda-link]:               https://github.com/conda-forge/hist-feedstock
 [doi-badge]:                https://zenodo.org/badge/239605861.svg
 [doi-link]:                 https://zenodo.org/badge/latestdoi/239605861
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  https://github.com/scikit-hep/hist/discussions
 [gitter-badge]:             https://badges.gitter.im/HSF/PyHEP-histogramming.svg
```

### Comparing `hist-2.7.2/pyproject.toml` & `hist-2.7.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     "boost-histogram",
     "dask-histogram",
 ]
 requires-python = ">=3.7"
 dependencies = [
     "boost-histogram>=1.3.1,<1.5",
     "histoprint>=2.2.0",
-    'numpy>=1.14.5;python_version<"3.12"',
-    'numpy>=1.26.0b1;python_version>="3.12"',
+    'numpy>=1.14.5',
     'typing-extensions>=4;python_version<"3.11"',
 ]
 dynamic = ["version"]
 
 [project.scripts]
 hist = "hist.classichist:main"
 
@@ -129,15 +128,14 @@
 ]
 
 [tool.mypy]
 warn_unused_configs = true
 files = "src"
 python_version = "3.8"
 strict = true
-show_error_codes = true
 enable_error_code = ["ignore-without-code", "truthy-bool", "redundant-expr"]
 warn_unreachable = true
 
 [[tool.mypy.overrides]]
 module = [
     "histoprint.*",
     "scipy.optimize.*",
@@ -146,14 +144,15 @@
     "scipy.*",
     "iminuit.*",
     "mplhep.*",
     "dask_histogram.*",
 ]
 ignore_missing_imports = true
 
+
 [tool.pylint]
 py-version = "3.7"
 extension-pkg-allow-list = ["boost_histogram._core"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 jobs = "0"
 messages_control.enable = [
@@ -180,17 +179,20 @@
   "import-error",
   "disallowed-name",
   "cyclic-import",
   "redefined-builtin",
   "unused-argument",  # Handled better by Ruff
 ]
 
+
 [tool.ruff]
-select = [
-  "E", "F", "W", # flake8
+src = ["src"]
+
+[tool.ruff.lint]
+extend-select = [
   "B",           # flake8-bugbear
   "I",           # isort
   "ARG",         # flake8-unused-arguments
   "C4",          # flake8-comprehensions
   "ICN",         # flake8-import-conventions
   "ISC",         # flake8-implicit-str-concat
   "PGH",         # pygrep-hooks
@@ -201,19 +203,17 @@
   "RET",         # flake8-return
   "RUF",         # Ruff-specific
   "SIM",         # flake8-simplify
   "T20",         # flake8-print
   "UP",          # pyupgrade
   "YTT",         # flake8-2020
 ]
-extend-ignore = ["PLR", "E501", "PT011", "PT013", "PT004", "B017"]
+ignore = ["PLR", "E501", "PT011", "PT013", "PT004", "B017", "ISC001"]
 typing-modules = ["hist._compat.typing"]
-src = ["src"]
-unfixable = ["T20", "F841"]
-exclude = []
 isort.required-imports = ["from __future__ import annotations"]
 flake8-unused-arguments.ignore-variadic-names = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/test_plot.py" = ["B008"]
 "docs/conf.py" = ["ARG001", "PTH"]
 "noxfile.py" = ["T20"]
+"**.ipynb" = ["B008", "T20", "I002", "E402", "E703", "B018"]
```

### Comparing `hist-2.7.2/PKG-INFO` & `hist-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hist
-Version: 2.7.2
+Version: 2.7.3
 Summary: Hist classes and utilities
 Project-URL: Homepage, https://github.com/scikit-hep/hist
 Project-URL: Documentation, https://hist.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/scikit-hep/hist/issues
 Project-URL: Discussions, https://github.com/scikit-hep/hist/discussions
 Project-URL: Changelog, https://hist.readthedocs.io/en/latest/changelog.html
 Author-email: Henry Schreiner <henry.schreiner@cern.ch>
@@ -29,33 +29,32 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: boost-histogram<1.5,>=1.3.1
 Requires-Dist: histoprint>=2.2.0
-Requires-Dist: numpy>=1.14.5; python_version < '3.12'
-Requires-Dist: numpy>=1.26.0b1; python_version >= '3.12'
+Requires-Dist: numpy>=1.14.5
 Requires-Dist: typing-extensions>=4; python_version < '3.11'
 Provides-Extra: dask
-Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and extra == 'dask'
-Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and extra == 'dask'
+Requires-Dist: dask-histogram>=2023.1; (python_version >= '3.8') and extra == 'dask'
+Requires-Dist: dask[dataframe]>=2022; (python_version >= '3.8') and extra == 'dask'
 Provides-Extra: dev
-Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and extra == 'dev'
-Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and extra == 'dev'
-Requires-Dist: iminuit>=2; python_version < '3.11' and extra == 'dev'
+Requires-Dist: dask-histogram>=2023.1; (python_version >= '3.8') and extra == 'dev'
+Requires-Dist: dask[dataframe]>=2022; (python_version >= '3.8') and extra == 'dev'
+Requires-Dist: iminuit>=2; (python_version < '3.11') and extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: matplotlib>=3.0; extra == 'dev'
 Requires-Dist: mplhep>=0.2.16; extra == 'dev'
 Requires-Dist: pytest-mpl>=0.12; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: scipy>=1.4; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and extra == 'docs'
-Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and extra == 'docs'
+Requires-Dist: dask-histogram>=2023.1; (python_version >= '3.8') and extra == 'docs'
+Requires-Dist: dask[dataframe]>=2022; (python_version >= '3.8') and extra == 'docs'
 Requires-Dist: graphviz>=0.20.1; extra == 'docs'
 Requires-Dist: iminuit>=2; extra == 'docs'
 Requires-Dist: ipykernel; extra == 'docs'
 Requires-Dist: ipython; extra == 'docs'
 Requires-Dist: ipython-genutils; extra == 'docs'
 Requires-Dist: matplotlib>=3.0; extra == 'docs'
 Requires-Dist: mplhep>=0.2.16; extra == 'docs'
@@ -76,28 +75,27 @@
 Provides-Extra: mpl
 Requires-Dist: matplotlib>=3.0; extra == 'mpl'
 Requires-Dist: mplhep>=0.2.16; extra == 'mpl'
 Provides-Extra: plot
 Requires-Dist: matplotlib>=3.0; extra == 'plot'
 Requires-Dist: mplhep>=0.2.16; extra == 'plot'
 Provides-Extra: test
-Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and python_version < '3.12' and extra == 'test'
-Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and python_version < '3.12' and extra == 'test'
+Requires-Dist: dask-histogram>=2023.1; (python_version >= '3.8' and python_version < '3.12') and extra == 'test'
+Requires-Dist: dask[dataframe]>=2022; (python_version >= '3.8' and python_version < '3.12') and extra == 'test'
 Requires-Dist: pytest-mpl>=0.12; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 <img alt="histogram" width="200" src="https://raw.githubusercontent.com/scikit-hep/hist/main/docs/_images/histlogo.png"/>
 
 # Hist
 
 [![Actions Status][actions-badge]][actions-link]
 [![Documentation Status][rtd-badge]][rtd-link]
 [![pre-commit.ci status][pre-commit-badge]][pre-commit-link]
-[![Code style: black][black-badge]][black-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda-Forge][conda-badge]][conda-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 [![DOI][doi-badge]][doi-link]
 [![License][license-badge]][license-link]
 
@@ -266,16 +264,14 @@
 
 Support for this work was provided by the National Science Foundation cooperative agreement OAC-1836650 (IRIS-HEP) and OAC-1450377 (DIANA/HEP). Any opinions, findings, conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
 [actions-badge]:            https://github.com/scikit-hep/hist/workflows/CI/badge.svg
 [actions-link]:             https://github.com/scikit-hep/hist/actions
 [binder-badge]:             https://mybinder.org/badge_logo.svg
 [binder-link]:              https://mybinder.org/v2/gh/scikit-hep/hist/HEAD
-[black-badge]:              https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]:               https://github.com/psf/black
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/hist
 [conda-link]:               https://github.com/conda-forge/hist-feedstock
 [doi-badge]:                https://zenodo.org/badge/239605861.svg
 [doi-link]:                 https://zenodo.org/badge/latestdoi/239605861
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  https://github.com/scikit-hep/hist/discussions
 [gitter-badge]:             https://badges.gitter.im/HSF/PyHEP-histogramming.svg
```

