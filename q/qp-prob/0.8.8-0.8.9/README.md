# Comparing `tmp/qp-prob-0.8.8.tar.gz` & `tmp/qp_prob-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qp-prob-0.8.8.tar", last modified: Mon Mar 18 22:18:32 2024, max compression
+gzip compressed data, was "qp_prob-0.8.9.tar", last modified: Thu May 16 22:15:07 2024, max compression
```

## Comparing `qp-prob-0.8.8.tar` & `qp_prob-0.8.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.630167 qp-prob-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.606167 qp-prob-0.8.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.606167 qp-prob-0.8.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.606167 qp-prob-0.8.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-18 22:18:20.000000 qp-prob-0.8.8/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-18 22:18:20.000000 qp-prob-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-03-18 22:18:32.630167 qp-prob-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-18 22:18:20.000000 qp-prob-0.8.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-03-18 22:18:20.000000 qp-prob-0.8.8/do_cover.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.610167 qp-prob-0.8.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)   861344 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/demo.html
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)   757141 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/practical_example.html
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/qp.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-18 22:18:20.000000 qp-prob-0.8.8/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-18 22:18:20.000000 qp-prob-0.8.8/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.614167 qp-prob-0.8.8/nb/
--rw-r--r--   0 runner    (1001) docker     (127)    32309 2024-03-18 22:18:20.000000 qp-prob-0.8.8/nb/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-18 22:18:20.000000 qp-prob-0.8.8/nb/iterator_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-03-18 22:18:20.000000 qp-prob-0.8.8/nb/metrics_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-03-18 22:18:20.000000 qp-prob-0.8.8/nb/mixmod_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-03-18 22:18:20.000000 qp-prob-0.8.8/nb/practical_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    37404 2024-03-18 22:18:20.000000 qp-prob-0.8.8/nb/quantile_parameterization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-18 22:18:20.000000 qp-prob-0.8.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      326 2024-03-18 22:18:20.000000 qp-prob-0.8.8/render_nb.sh
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-18 22:18:20.000000 qp-prob-0.8.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 22:18:32.630167 qp-prob-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-18 22:18:20.000000 qp-prob-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.602167 qp-prob-0.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.618167 qp-prob-0.8.8/src/qp/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-18 22:18:32.000000 qp-prob-0.8.8/src/qp/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/conversion_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.618167 qp-prob-0.8.8/src/qp/data/
--rw-r--r--   0 runner    (1001) docker     (127)   161680 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/data/CFHTLens_sample.P.npy
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/data/test.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/dict_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21442 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/hist_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/interp_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/lazy_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.618167 qp-prob-0.8.8/src/qp/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/array_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/base_metric_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/brier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/concrete_metric_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/goodness_of_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18742 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/parallel_metrics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/metrics/point_estimate_metric_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/mixmod_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/packed_interp_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/packing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/pdf_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/quant_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.622167 qp-prob-0.8.8/src/qp/quantile_pdf_constructors/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/quantile_pdf_constructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/quantile_pdf_constructors/dual_spline_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/quantile_pdf_constructors/piecewise_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/quantile_pdf_constructors/piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/scipy_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/sparse_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/sparse_rep.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/spline_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24209 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-18 22:18:20.000000 qp-prob-0.8.8/src/qp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.626167 qp-prob-0.8.8/src/qp_prob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-03-18 22:18:32.000000 qp-prob-0.8.8/src/qp_prob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-18 22:18:32.000000 qp-prob-0.8.8/src/qp_prob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 22:18:32.000000 qp-prob-0.8.8/src/qp_prob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-18 22:18:32.000000 qp-prob-0.8.8/src/qp_prob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-18 22:18:32.000000 qp-prob-0.8.8/src/qp_prob.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.602167 qp-prob-0.8.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.622167 qp-prob-0.8.8/tests/qp/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.626167 qp-prob-0.8.8/tests/qp/quant_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/quant_pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/quant_pdf/test_quant_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:32.626167 qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_base_metric_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_brier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9655 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_eval_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_flex_coefs.npy
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18280 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_point_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_scipy_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-18 22:18:20.000000 qp-prob-0.8.8/tests/qp/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.233957 qp_prob-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.209957 qp_prob-0.8.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.209957 qp_prob-0.8.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.213957 qp_prob-0.8.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-16 22:14:45.000000 qp_prob-0.8.9/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 22:14:45.000000 qp_prob-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-16 22:15:07.233957 qp_prob-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-16 22:14:45.000000 qp_prob-0.8.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-05-16 22:14:45.000000 qp_prob-0.8.9/do_cover.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.217957 qp_prob-0.8.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   861344 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/demo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   757141 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/practical_example.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/qp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-16 22:14:45.000000 qp_prob-0.8.9/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-16 22:14:45.000000 qp_prob-0.8.9/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.217957 qp_prob-0.8.9/nb/
+-rw-r--r--   0 runner    (1001) docker     (127)    32309 2024-05-16 22:14:45.000000 qp_prob-0.8.9/nb/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-16 22:14:45.000000 qp_prob-0.8.9/nb/iterator_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-05-16 22:14:45.000000 qp_prob-0.8.9/nb/metrics_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-05-16 22:14:45.000000 qp_prob-0.8.9/nb/mixmod_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-05-16 22:14:45.000000 qp_prob-0.8.9/nb/practical_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    37404 2024-05-16 22:14:45.000000 qp_prob-0.8.9/nb/quantile_parameterization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-16 22:14:45.000000 qp_prob-0.8.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      326 2024-05-16 22:14:45.000000 qp_prob-0.8.9/render_nb.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 22:14:45.000000 qp_prob-0.8.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:15:07.233957 qp_prob-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 22:14:45.000000 qp_prob-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.205957 qp_prob-0.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.221957 qp_prob-0.8.9/src/qp/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 22:15:06.000000 qp_prob-0.8.9/src/qp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/conversion_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.221957 qp_prob-0.8.9/src/qp/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   161680 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/data/CFHTLens_sample.P.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/data/test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/dict_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21442 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/hist_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/interp_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/lazy_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.225957 qp_prob-0.8.9/src/qp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/array_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/base_metric_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/brier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/concrete_metric_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/goodness_of_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/parallel_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/metrics/point_estimate_metric_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/mixmod_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/packed_interp_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/packing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/pdf_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/quant_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.225957 qp_prob-0.8.9/src/qp/quantile_pdf_constructors/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/quantile_pdf_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/quantile_pdf_constructors/dual_spline_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/quantile_pdf_constructors/piecewise_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/quantile_pdf_constructors/piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/scipy_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/sparse_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/sparse_rep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/spline_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24209 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 22:14:45.000000 qp_prob-0.8.9/src/qp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.229957 qp_prob-0.8.9/src/qp_prob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-16 22:15:07.000000 qp_prob-0.8.9/src/qp_prob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-16 22:15:07.000000 qp_prob-0.8.9/src/qp_prob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:15:07.000000 qp_prob-0.8.9/src/qp_prob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-16 22:15:07.000000 qp_prob-0.8.9/src/qp_prob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-16 22:15:07.000000 qp_prob-0.8.9/src/qp_prob.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.205957 qp_prob-0.8.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.229957 qp_prob-0.8.9/tests/qp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.229957 qp_prob-0.8.9/tests/qp/quant_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/quant_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/quant_pdf/test_quant_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:15:07.229957 qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_base_metric_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_brier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9655 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_eval_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_flex_coefs.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18280 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_point_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_scipy_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-16 22:14:45.000000 qp_prob-0.8.9/tests/qp/test_utils.py
```

### Comparing `qp-prob-0.8.8/.github/ISSUE_TEMPLATE/1-bug_report.md` & `qp_prob-0.8.9/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.github/ISSUE_TEMPLATE/2-feature_request.md` & `qp_prob-0.8.9/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.github/pull_request_template.md` & `qp_prob-0.8.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.github/workflows/linting.yml` & `qp_prob-0.8.9/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.github/workflows/publish-to-pypi.yml` & `qp_prob-0.8.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.github/workflows/smoke-test.yml` & `qp_prob-0.8.9/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.github/workflows/testing-and-coverage.yml` & `qp_prob-0.8.9/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.gitignore` & `qp_prob-0.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.pre-commit-config.yaml` & `qp_prob-0.8.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.readthedocs.yaml` & `qp_prob-0.8.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/.travis.yml` & `qp_prob-0.8.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/LICENSE` & `qp_prob-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/PKG-INFO` & `qp_prob-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-prob
-Version: 0.8.8
+Version: 0.8.9
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `qp-prob-0.8.8/README.md` & `qp_prob-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/.gitignore` & `qp_prob-0.8.9/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/Makefile` & `qp_prob-0.8.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/conf.py` & `qp_prob-0.8.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/contributing.rst` & `qp_prob-0.8.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/demo.html` & `qp_prob-0.8.9/docs/demo.html`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/index.rst` & `qp_prob-0.8.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/install.rst` & `qp_prob-0.8.9/docs/install.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/practical_example.html` & `qp_prob-0.8.9/docs/practical_example.html`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/docs/qp.rst` & `qp_prob-0.8.9/docs/qp.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/nb/demo.ipynb` & `qp_prob-0.8.9/nb/demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/nb/iterator_demo.ipynb` & `qp_prob-0.8.9/nb/iterator_demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/nb/metrics_examples.ipynb` & `qp_prob-0.8.9/nb/metrics_examples.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/nb/mixmod_examples.ipynb` & `qp_prob-0.8.9/nb/mixmod_examples.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/nb/practical_example.ipynb` & `qp_prob-0.8.9/nb/practical_example.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/nb/quantile_parameterization_demo.ipynb` & `qp_prob-0.8.9/nb/quantile_parameterization_demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/pyproject.toml` & `qp_prob-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/__init__.py` & `qp_prob-0.8.9/src/qp/__init__.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/conversion_funcs.py` & `qp_prob-0.8.9/src/qp/conversion_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/data/CFHTLens_sample.P.npy` & `qp_prob-0.8.9/src/qp/data/CFHTLens_sample.P.npy`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/data/test.hdf5` & `qp_prob-0.8.9/src/qp/data/test.hdf5`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/dict_utils.py` & `qp_prob-0.8.9/src/qp/dict_utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/ensemble.py` & `qp_prob-0.8.9/src/qp/ensemble.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/factory.py` & `qp_prob-0.8.9/src/qp/factory.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/hist_pdf.py` & `qp_prob-0.8.9/src/qp/hist_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/interp_pdf.py` & `qp_prob-0.8.9/src/qp/interp_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/array_metrics.py` & `qp_prob-0.8.9/src/qp/metrics/array_metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/base_metric_classes.py` & `qp_prob-0.8.9/src/qp/metrics/base_metric_classes.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/brier.py` & `qp_prob-0.8.9/src/qp/metrics/brier.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/concrete_metric_classes.py` & `qp_prob-0.8.9/src/qp/metrics/concrete_metric_classes.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/factory.py` & `qp_prob-0.8.9/src/qp/metrics/factory.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/goodness_of_fit.py` & `qp_prob-0.8.9/src/qp/metrics/goodness_of_fit.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/metrics.py` & `qp_prob-0.8.9/src/qp/metrics/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             "Number of distributions in the Ensemble (%d) is not equal to the number of truth values (%d)"
             % (p.npdf, len(truth))
         )
 
     # Values of truth that are outside the defined limits will not appear truth_array.
     # Consider expanding the limits or using numpy.clip to restrict truth values to the limits.
     if np.any(np.less(truth, limits[0])) or np.any(np.greater(truth, limits[1])):
-        raise ValueError("Input truth values exceed the defined limits")
+        raise ValueError(f"Input truth values exceed the defined limits ({min(truth)}, {max(truth)}) ({limits[0]} {limits[1]})")
 
     # Make a grid object that defines grid values and histogram bin edges using limits and dx
     grid = _calculate_grid_parameters(limits, dx)
 
     # Evaluate the pdf of the distributions on the grid.
     # The value returned from p.gridded is a 2-tuple. The 0th index is the array of grid points,
     # the 1st index is the array of PDF values. Thus we call p.gridded(...)[1]
```

### Comparing `qp-prob-0.8.8/src/qp/metrics/parallel_metrics.ipynb` & `qp_prob-0.8.9/src/qp/metrics/parallel_metrics.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/pit.py` & `qp_prob-0.8.9/src/qp/metrics/pit.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/metrics/point_estimate_metric_classes.py` & `qp_prob-0.8.9/src/qp/metrics/point_estimate_metric_classes.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/mixmod_pdf.py` & `qp_prob-0.8.9/src/qp/mixmod_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/packed_interp_pdf.py` & `qp_prob-0.8.9/src/qp/packed_interp_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/packing_utils.py` & `qp_prob-0.8.9/src/qp/packing_utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/pdf_gen.py` & `qp_prob-0.8.9/src/qp/pdf_gen.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/plotting.py` & `qp_prob-0.8.9/src/qp/plotting.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/quant_pdf.py` & `qp_prob-0.8.9/src/qp/quant_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py` & `qp_prob-0.8.9/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py` & `qp_prob-0.8.9/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/quantile_pdf_constructors/dual_spline_average.py` & `qp_prob-0.8.9/src/qp/quantile_pdf_constructors/dual_spline_average.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/quantile_pdf_constructors/piecewise_constant.py` & `qp_prob-0.8.9/src/qp/quantile_pdf_constructors/piecewise_constant.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/quantile_pdf_constructors/piecewise_linear.py` & `qp_prob-0.8.9/src/qp/quantile_pdf_constructors/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/scipy_pdfs.py` & `qp_prob-0.8.9/src/qp/scipy_pdfs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/sparse_pdf.py` & `qp_prob-0.8.9/src/qp/sparse_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/sparse_rep.py` & `qp_prob-0.8.9/src/qp/sparse_rep.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/spline_pdf.py` & `qp_prob-0.8.9/src/qp/spline_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/test_data.py` & `qp_prob-0.8.9/src/qp/test_data.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/test_funcs.py` & `qp_prob-0.8.9/src/qp/test_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp/utils.py` & `qp_prob-0.8.9/src/qp/utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/src/qp_prob.egg-info/PKG-INFO` & `qp_prob-0.8.9/src/qp_prob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-prob
-Version: 0.8.8
+Version: 0.8.9
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `qp-prob-0.8.8/src/qp_prob.egg-info/SOURCES.txt` & `qp_prob-0.8.9/src/qp_prob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/.gitignore` & `qp_prob-0.8.9/tests/qp/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/benchmark.py` & `qp_prob-0.8.9/tests/qp/benchmark.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/fidelity.py` & `qp_prob-0.8.9/tests/qp/fidelity.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/quant_pdf/test_quant_pdf.py` & `qp_prob-0.8.9/tests/qp/quant_pdf/test_quant_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py` & `qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py` & `qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py` & `qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py` & `qp_prob-0.8.9/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_auto.py` & `qp_prob-0.8.9/tests/qp/test_auto.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_base_metric_classes.py` & `qp_prob-0.8.9/tests/qp/test_base_metric_classes.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_brier.py` & `qp_prob-0.8.9/tests/qp/test_brier.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_ensemble.py` & `qp_prob-0.8.9/tests/qp/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_eval_funcs.py` & `qp_prob-0.8.9/tests/qp/test_eval_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_flex_coefs.npy` & `qp_prob-0.8.9/tests/qp/test_flex_coefs.npy`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_infrastructure.py` & `qp_prob-0.8.9/tests/qp/test_infrastructure.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_metric_factory.py` & `qp_prob-0.8.9/tests/qp/test_metric_factory.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_metrics.py` & `qp_prob-0.8.9/tests/qp/test_metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_parallel.py` & `qp_prob-0.8.9/tests/qp/test_parallel.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_pit.py` & `qp_prob-0.8.9/tests/qp/test_pit.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_point_metrics.py` & `qp_prob-0.8.9/tests/qp/test_point_metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_scipy_vectorization.py` & `qp_prob-0.8.9/tests/qp/test_scipy_vectorization.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.8/tests/qp/test_utils.py` & `qp_prob-0.8.9/tests/qp/test_utils.py`

 * *Files identical despite different names*

