# Comparing `tmp/chrfinder-0.0.3.tar.gz` & `tmp/chrfinder-1.0.0.tar.gz`

## Comparing `chrfinder-0.0.3.tar` & `chrfinder-1.0.0.tar`

### file list

```diff
@@ -1,70 +1,69 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.3/pytest
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.3/python
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.3/sphinx-build
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 chrfinder-0.0.3/tox.ini
--rw-r--r--   0        0        0  3450189 2020-02-02 00:00:00.000000 chrfinder-0.0.3/assets/Caf_Ace_Asp.gif
--rw-r--r--   0        0        0   415096 2020-02-02 00:00:00.000000 chrfinder-0.0.3/assets/Image_Chrfinder.webp
--rw-r--r--   0        0        0   772009 2020-02-02 00:00:00.000000 chrfinder-0.0.3/assets/edited-error-molecule-not-added.gif
--rw-r--r--   0        0        0   422911 2020-02-02 00:00:00.000000 chrfinder-0.0.3/assets/edited-hydrocarbure.gif
--rw-r--r--   0        0        0   695205 2020-02-02 00:00:00.000000 chrfinder-0.0.3/assets/edited-limit.gif
--rw-r--r--   0        0        0   606751 2020-02-02 00:00:00.000000 chrfinder-0.0.3/assets/edited-naphtalene-.gif
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 chrfinder-0.0.3/data/README.md
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/.buildinfo
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/genindex.html
--rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/index.html
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/objects.inv
--rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/py-modindex.html
--rw-r--r--   0        0        0    14148 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/search.html
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/searchindex.js
--rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_modules/index.html
--rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_modules/chrfinder/example_module.html
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_sources/index.md.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_sources/api/chrfinder.rst.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_sources/api/modules.rst.txt
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/basic.css
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/check-solid.svg
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/clipboard.min.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/copy-button.svg
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/copybutton.css
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/copybutton.js
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/copybutton_funcs.js
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/debug.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/doctools.js
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/plus.png
--rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/searchtools.js
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/skeleton.css
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/sphinx_highlight.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/scripts/furo-extensions.js
--rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/scripts/furo.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/scripts/furo.js.LICENSE.txt
--rw-r--r--   0        0        0    28551 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/scripts/furo.js.map
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/styles/furo-extensions.css
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/styles/furo-extensions.css.map
--rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/styles/furo.css
--rw-r--r--   0        0        0    76416 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/_static/styles/furo.css.map
--rw-r--r--   0        0        0    18411 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/api/chrfinder.html
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/docs_out/api/modules.html
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/source/conf.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/source/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/source/api/Chrfinder.rst
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 chrfinder-0.0.3/docs/source/api/modules.rst
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 chrfinder-0.0.3/notebooks/__init__.py
--rw-r--r--   0        0        0    28961 2020-02-02 00:00:00.000000 chrfinder-0.0.3/notebooks/project_report.ipynb
--rw-r--r--   0        0        0    14106 2020-02-02 00:00:00.000000 chrfinder-0.0.3/src/Chrfinder/Chrfinder.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 chrfinder-0.0.3/src/Chrfinder/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 chrfinder-0.0.3/src/Chrfinder/classify.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 chrfinder-0.0.3/src/Chrfinder/pka_lookup.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 chrfinder-0.0.3/src/Chrfinder/pubchemprops.py
--rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 chrfinder-0.0.3/src/Chrfinder/search_pka.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 chrfinder-0.0.3/tests/test_complete.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chrfinder-0.0.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 chrfinder-0.0.3/LICENSE
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 chrfinder-0.0.3/README.md
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 chrfinder-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 chrfinder-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chrfinder-1.0.0/tox.ini
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chrfinder-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0  3450189 2020-02-02 00:00:00.000000 chrfinder-1.0.0/assets/Caf_Ace_Asp.gif
+-rw-r--r--   0        0        0   415096 2020-02-02 00:00:00.000000 chrfinder-1.0.0/assets/Image_Chrfinder.webp
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 chrfinder-1.0.0/assets/coverage-badge.svg
+-rw-r--r--   0        0        0   772009 2020-02-02 00:00:00.000000 chrfinder-1.0.0/assets/edited-error-molecule-not-added.gif
+-rw-r--r--   0        0        0   422911 2020-02-02 00:00:00.000000 chrfinder-1.0.0/assets/edited-hydrocarbure.gif
+-rw-r--r--   0        0        0   695205 2020-02-02 00:00:00.000000 chrfinder-1.0.0/assets/edited-limit.gif
+-rw-r--r--   0        0        0   606751 2020-02-02 00:00:00.000000 chrfinder-1.0.0/assets/edited-naphtalene-.gif
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 chrfinder-1.0.0/data/README.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/.buildinfo
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/genindex.html
+-rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/index.html
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/objects.inv
+-rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/py-modindex.html
+-rw-r--r--   0        0        0    14148 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/search.html
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/searchindex.js
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_modules/index.html
+-rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_modules/chrfinder/example_module.html
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_sources/index.md.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_sources/api/chrfinder.rst.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_sources/api/modules.rst.txt
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/basic.css
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/check-solid.svg
+-rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/clipboard.min.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/copy-button.svg
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/copybutton.css
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/copybutton.js
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/copybutton_funcs.js
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/debug.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/doctools.js
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/plus.png
+-rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/searchtools.js
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/skeleton.css
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/scripts/furo-extensions.js
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/scripts/furo.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--   0        0        0    28551 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/scripts/furo.js.map
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/styles/furo-extensions.css
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/styles/furo-extensions.css.map
+-rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/styles/furo.css
+-rw-r--r--   0        0        0    76416 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/_static/styles/furo.css.map
+-rw-r--r--   0        0        0    18411 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/api/chrfinder.html
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/docs_out/api/modules.html
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/source/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/source/api/Chrfinder.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chrfinder-1.0.0/docs/source/api/modules.rst
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 chrfinder-1.0.0/notebooks/__init__.py
+-rw-r--r--   0        0        0    28961 2020-02-02 00:00:00.000000 chrfinder-1.0.0/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0    14106 2020-02-02 00:00:00.000000 chrfinder-1.0.0/src/Chrfinder/Chrfinder.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 chrfinder-1.0.0/src/Chrfinder/__init__.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 chrfinder-1.0.0/src/Chrfinder/classify.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 chrfinder-1.0.0/src/Chrfinder/pka_lookup.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 chrfinder-1.0.0/src/Chrfinder/pubchemprops.py
+-rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 chrfinder-1.0.0/src/Chrfinder/search_pka.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 chrfinder-1.0.0/tests/test_complete.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chrfinder-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 chrfinder-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 chrfinder-1.0.0/README.md
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 chrfinder-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 chrfinder-1.0.0/PKG-INFO
```

### Comparing `chrfinder-0.0.3/tox.ini` & `chrfinder-1.0.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tox]
 envlist = check, docs, {py3}{,-coverage}
 
 [gh-actions]
 python =
-    3.10: check, py310
+    3.10: check, py310, py3-coverage
     3.11: py311
     3.12: py312
 
 [testenv]
 basepython =
     pypy3: pypy3
     py38: python3.8
@@ -15,26 +15,33 @@
     py310: python3.10
     py311: python3.11
     py312: python3.12
     {check,docs}: python3
 setenv =
     PYTHONUNBUFFERED = yes
     PYTEST_EXTRA_ARGS = -s
-    coverage: PYTEST_EXTRA_ARGS = --cov=src/Chrfinder.py --cov-report xml:.tox/coverage.xml --cov-report term
 passenv =
     *
 extras =
     test
 commands =
     pytest {env:PYTEST_MARKERS:} {env:PYTEST_EXTRA_ARGS:} {posargs:-vv}
-    coverage: genbadge coverage -i .tox/coverage.xml -o assets/coverage-badge.svg
+
+[testenv:coverage]
+description = Run tests and generate coverage report
+setenv =
+    PYTHONUNBUFFERED = yes
+    PYTEST_EXTRA_ARGS = --cov=src/Chrfinder --cov-report xml:.tox/coverage.xml --cov-report term
+commands =
+    pytest {env:PYTEST_EXTRA_ARGS:} {posargs:-vv}
+    genbadge coverage -i .tox/coverage.xml -o assets/coverage-badge.svg
 usedevelop = true
 
 [testenv:docs]
-description = build HTML docs
+description = Build HTML docs
 setenv =
     READTHEDOCS_PROJECT = Chrfinder
     READTHEDOCS_VERSION = latest
 extras =
     doc
 commands =
     sphinx-build -d "{toxworkdir}/docs_doctree" docs/source "docs/docs_out" --color -vW -b html
```

### Comparing `chrfinder-0.0.3/assets/Caf_Ace_Asp.gif` & `chrfinder-1.0.0/assets/Caf_Ace_Asp.gif`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/assets/Image_Chrfinder.webp` & `chrfinder-1.0.0/assets/Image_Chrfinder.webp`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/assets/edited-error-molecule-not-added.gif` & `chrfinder-1.0.0/assets/edited-error-molecule-not-added.gif`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/assets/edited-hydrocarbure.gif` & `chrfinder-1.0.0/assets/edited-hydrocarbure.gif`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/assets/edited-limit.gif` & `chrfinder-1.0.0/assets/edited-limit.gif`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/assets/edited-naphtalene-.gif` & `chrfinder-1.0.0/assets/edited-naphtalene-.gif`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/genindex.html` & `chrfinder-1.0.0/docs/docs_out/genindex.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/index.html` & `chrfinder-1.0.0/docs/docs_out/index.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/py-modindex.html` & `chrfinder-1.0.0/docs/docs_out/py-modindex.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/search.html` & `chrfinder-1.0.0/docs/docs_out/search.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/searchindex.js` & `chrfinder-1.0.0/docs/docs_out/searchindex.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_modules/index.html` & `chrfinder-1.0.0/docs/docs_out/_modules/index.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_modules/chrfinder/example_module.html` & `chrfinder-1.0.0/docs/docs_out/_modules/chrfinder/example_module.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/basic.css` & `chrfinder-1.0.0/docs/docs_out/_static/basic.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/clipboard.min.js` & `chrfinder-1.0.0/docs/docs_out/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/copybutton.css` & `chrfinder-1.0.0/docs/docs_out/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/copybutton.js` & `chrfinder-1.0.0/docs/docs_out/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/copybutton_funcs.js` & `chrfinder-1.0.0/docs/docs_out/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/debug.css` & `chrfinder-1.0.0/docs/docs_out/_static/debug.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/doctools.js` & `chrfinder-1.0.0/docs/docs_out/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/language_data.js` & `chrfinder-1.0.0/docs/docs_out/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/pygments.css` & `chrfinder-1.0.0/docs/docs_out/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/searchtools.js` & `chrfinder-1.0.0/docs/docs_out/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/skeleton.css` & `chrfinder-1.0.0/docs/docs_out/_static/skeleton.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/sphinx_highlight.js` & `chrfinder-1.0.0/docs/docs_out/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/scripts/furo.js` & `chrfinder-1.0.0/docs/docs_out/_static/scripts/furo.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/scripts/furo.js.map` & `chrfinder-1.0.0/docs/docs_out/_static/scripts/furo.js.map`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/styles/furo-extensions.css` & `chrfinder-1.0.0/docs/docs_out/_static/styles/furo-extensions.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/styles/furo-extensions.css.map` & `chrfinder-1.0.0/docs/docs_out/_static/styles/furo-extensions.css.map`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/styles/furo.css` & `chrfinder-1.0.0/docs/docs_out/_static/styles/furo.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/_static/styles/furo.css.map` & `chrfinder-1.0.0/docs/docs_out/_static/styles/furo.css.map`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/api/chrfinder.html` & `chrfinder-1.0.0/docs/docs_out/api/chrfinder.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/docs_out/api/modules.html` & `chrfinder-1.0.0/docs/docs_out/api/modules.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/docs/source/conf.py` & `chrfinder-1.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/notebooks/project_report.ipynb` & `chrfinder-1.0.0/notebooks/project_report.ipynb`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/src/Chrfinder/Chrfinder.py` & `chrfinder-1.0.0/src/Chrfinder/Chrfinder.py`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/src/Chrfinder/__init__.py` & `chrfinder-1.0.0/src/Chrfinder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The package finds the best chromatography based on properties of the mixture."""
 
-__version__ = "0.0.1"
+__version__ = "0.0.3"
 
 from .pubchemprops import get_cid_by_name, get_first_layer_props, get_second_layer_props
 from .pka_lookup import pka_lookup_pubchem
 from .Chrfinder import add_molecule, find_pka, find_boiling_point, get_df_properties, det_chromato, update_results, main
 
 __all__ = [
     'get_cid_by_name',
```

### Comparing `chrfinder-0.0.3/src/Chrfinder/classify.py` & `chrfinder-1.0.0/src/Chrfinder/classify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 import re
 
 def classify(identifier: str) -> str:
-    """Determine the type of chemical indentifier (CAS, smiles, inchi, inchikey)
+    """Determine the type of chemical identifier (CAS, smiles, inchi, inchikey)
     
     Parameters
     ----------
-    indentifier : str
-        a string of chemical indentifier
+    identifier : str
+        a string of chemical identifier
     
     Returns
     -------
     str
         one of (CAS, smiles, inchi, inchikey)
     """
 
     # https://www.ebi.ac.uk/miriam/main/collections/MIR:00000237
-    cas_pattern = re.compile(r'^\d{1,7}\-\d{2}\-\d$')
+    cas_pattern = re.compile(r'^\d{1,7}-\d{2}-\d$')
 
     '''
     The first is reference from: https://gist.github.com/lsauer/1312860/264ae813c2bd2c27a769d261c8c6b38da34e22fb#file-smiles_inchi_annotated-js
     However, this can be matched with CAS or InChIKey as well
     >>> smiles_pattern = re.compile(r'^(?!InChI=)[^J][a-zA-Z0-9@+\-\[\]\(\)\\\/%=#$]{1,}$')
     This will not match CAS or InChIKey.
     Even then, the solution below can match a lot more strings: 
         'some non sense'
         '123456789',
         1234567,
         'qwertyui'
     '''
-    smiles_pattern = re.compile(r'^(?!InChI=)(?!\d{1,7}\-\d{2}\-\d)(?![A-Z]{14}\-[A-Z]{10}(\-[A-Z])?)[^J][a-zA-Z0-9@+\-\[\]\(\)\\\/%=#$]{1,}$')
+    smiles_pattern = re.compile(r'^(?!InChI=)(?!\d{1,7}-\d{2}-\d)(?![A-Z]{14}-[A-Z]{10}(-[A-Z])?)[^J][a-zA-Z0-9@+\-\[\]\(\)\\\/%=#$]{1,}$')
 
     # https://www.ebi.ac.uk/miriam/main/collections/MIR:00000383
-    inchi_pattern = re.compile(r'^InChI\=1S?\/[A-Za-z0-9\.]+(\+[0-9]+)?(\/[cnpqbtmsih][A-Za-z0-9\-\+\(\)\,\/\?\;\.]+)*$')
+    inchi_pattern = re.compile(r'^InChI=1S?/[A-Za-z0-9\.]+(\+[0-9]+)?(/[cnpqbtmsih][A-Za-z0-9\-+\(\),\/\?;\.]+)*$')
 
     # https://www.ebi.ac.uk/miriam/main/collections/MIR:00000387
-    inchikey_pattern = re.compile(r'^[A-Z]{14}\-[A-Z]{10}(\-[A-Z])?')
+    inchikey_pattern = re.compile(r'^[A-Z]{14}-[A-Z]{10}(-[A-Z])?')
 
     # IMPORTANT: careful with the order of the dict since one regex might match more than 1 type
     # See smiles_pattern above
     lookup = {
         'cas': lambda x: cas_pattern.search(x),
         'inchi': lambda x: inchi_pattern.search(x),
         'inchikey': lambda x: inchikey_pattern.search(x),
         'smiles': lambda x: smiles_pattern.search(x),
     }
 
     for key, value in lookup.items():
         if value(identifier):
             return key
 
-
 if __name__ == "__main__":
     print(classify('106-54-7'))
     # print(classify('InChI=1S/C6H12O6/c7-1-2-3(8)4(9)5(10)6(11)12-2/h2-11H,1H2/t2-,3-,4+,5+,6?/m1/s1'))
     # print(classify('VZXOZSQDJJNBRC-UHFFFAOYSA-N'))
-    # print(classify('C1=CC(=CC=C1F)S'))
+    # print(classify('C1=CC(=CC=C1F)S'))
```

### Comparing `chrfinder-0.0.3/src/Chrfinder/pka_lookup.py` & `chrfinder-1.0.0/src/Chrfinder/pka_lookup.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,184 +26,134 @@
 from .classify import classify
 
 
 debug = False
 
 
 def pka_lookup_pubchem(identifier, namespace=None, domain='compound') -> Optional[str]:
-     """
+    """
     Lookup the pKa value of a compound from PubChem.
 
-    This function uses the PubChem API to find the pKa value of a compound based on a given identifier. 
+    This function uses the PubChem API to find the pKa value of a compound based on a given identifier.
     The identifier can be a name, CAS number, SMILES, InChI, or InChIKey. The function also supports debugging mode.
 
     Args:
         identifier (str): The identifier for the compound. This can be a chemical name, CAS number, SMILES, InChI, or InChIKey.
-        namespace (str, optional): The namespace of the identifier. This can be 'name', 'cas', 'smiles', 'inchi', or 'inchikey'. 
+        namespace (str, optional): The namespace of the identifier. This can be 'name', 'cas', 'smiles', 'inchi', or 'inchikey'.
                                    If not provided, the function will attempt to classify the identifier.
         domain (str, optional): The domain to search within. Default is 'compound'.
 
     Returns:
         Optional[str]: A dictionary with the pKa value and other relevant information if found, otherwise None.
 
     Raises:
         ValueError: If an exact match for the identifier is not found on PubChem.
         RuntimeError: If the compound or pKa value is not found in PubChem.
-    
     """
     global debug
 
     if len(sys.argv) == 2 and sys.argv[1] in ['--debug=True', '--debug=true', '--debug', '-d']:
         debug = True
 
-    # if debug:
-    #     print(f'In DEBUG mode: {debug}')
-
     # Identify lookup source (Pubchem in this case)
     lookup_source = 'Pubchem'
 
     try:
         headers = {
             'user-agent': 'Mozilla/5.0 (X11; CentOS; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/73.0.3683.75 Safari/537.36'}
 
-        # print('Searching Pubchem...')
-
-        # Using pubchem api for python
-        # Getting CID number, the result of this, by default is exact match. The result is returned as a list.
         cids = []
         identifier_type = ''
 
         if not namespace:
             identifier_type = classify(identifier)
-            # print(f'identifier_type determined by classify() is: {identifier_type}')
 
-            # If the input is inchi, inchikey or smiles (this could be a false smiles):
             if identifier_type in ['smiles', 'inchi', 'inchikey']:
                 lookup = pcp.get_cids(identifier, namespace=identifier_type)
                 if lookup:
                     cids.append(lookup[0])
             else:
                 lookup = pcp.get_cids(identifier, namespace='name')
                 if lookup:
                     cids.append(lookup[0])
-                    # print(f'namespace from pubchem lookup is: {namespace}')
         elif namespace == 'cas':
             cids = pcp.get_cids(identifier, namespace='name')
         else:
             cids = pcp.get_cids(identifier, namespace=namespace)
 
         if not cids:
             lookup = pcp.get_cids(identifier, namespace='name')
             if lookup:
                 cids.append(lookup[0])
-
-            # cids = pcp.get_cids(identifier, namespace=namespace)
             identifier_type = namespace
 
-        # print(cids)
-
-        #  this api return an empty list if it cannot find cas_nr. This is to check if pubchem has this chemical.
         if len(cids) > 0:
-            # if Pubchem found the result, get the first result of the list
             cid = cids[0]
-            # print('Compound ID (CID) from PubChem is: {} and type is: {}'.format(cid, type(cid)))
-
             exact_match = True
-
-            # synonyms = []
             synonyms = pcp.get_synonyms(cid)[0]['Synonym'] or []
-            
-            # Extract CAS number from the list of synonyms
+
             returned_cas = ''
             for synonym in synonyms:
                 cas_nr = re.search(r'^\d{2,7}-\d{2}-\d$', synonym)
                 if cas_nr:
                     cas_nr = cas_nr.group()
                     returned_cas = cas_nr
                     break
 
-            # lookup_result = []
             lookup_result = pcp.get_properties(['inchi', 'inchikey',
-                                        'canonical_smiles', 'isomeric_smiles',
-                                        'iupac_name'],
-                                cid)
+                                                'canonical_smiles', 'isomeric_smiles',
+                                                'iupac_name'],
+                                               cid)
 
             if identifier_type == 'cas':
-                # To double check if the CAS number is correct:
-                # using pubchem api, get a list of synonym. The result is a list of dict.
-                # choose the first result and check all values for 'Synonym' key:
                 exact_match = identifier in synonyms
-
             elif identifier_type in ['inchi', 'inchikey']:
-
                 if identifier_type == 'inchi':
-                    # print(lookup_result[0].get('InChI', False))
-                    # print(f'input:\n{identifier}')
                     exact_match = (identifier == lookup_result[0].get('InChI', False))
-                
                 elif identifier_type == 'inchikey':
                     exact_match = (identifier == lookup_result[0].get('InChIKey', False))
 
             if not exact_match:
                 if debug:
                     print(f'Exact match between input and Pubchem return value? {identifier in synonyms}')
                 raise ValueError('This is not an exact match on Pubchem!')
 
-            '''
-            get url from Pubchem to get pka lookup result
-            'XML' can be replaced with 'JSON' but it is harder to parse later on
-            for more info about Pubchem output types: https://pubchemdocs.ncbi.nlm.nih.gov/pug-rest$_Toc494865558
-            '''
             pka_lookup_result_xml = 'https://pubchem.ncbi.nlm.nih.gov/rest/pug_view/data/compound/{}/XML?heading=Dissociation+Constants'.format(cid)
 
-            # Get the html request info using CID number from pubchem
             r = requests.get(pka_lookup_result_xml, headers=headers, timeout=15)
-            # Check to see if give OK status (200) and not redirect
             if r.status_code == 200 and len(r.history) == 0:
-                # print(r.text)
-                # Use python XML to parse the return result
                 tree = ET.fromstring(r.text)
-            
-                # Get the XML tree of <Information> only
                 info_node = tree.find('.//*{http://pubchem.ncbi.nlm.nih.gov/pug_view}Information')
-
-                # Get the pKa reference:
                 original_source = info_node.find('{http://pubchem.ncbi.nlm.nih.gov/pug_view}Reference').text
-                # Get the pKa result:
                 pka_result = info_node.find('.//*{http://pubchem.ncbi.nlm.nih.gov/pug_view}String').text
-                pka_result = re.sub(r'^pKa = ', '', pka_result)    # remove 'pka = ' part out of the string answer
-                # print(pka_result)
-                # print(original_source)
-                # print(lookup_result)
+                pka_result = re.sub(r'^pKa = ', '', pka_result)
 
                 core_result = {
                     'source': lookup_source,
                     'Pubchem_CID': str(cid),
                     'pKa': pka_result,
                     'reference': original_source,
                     'Substance_CASRN': returned_cas,
                 }
                 extra_info = lookup_result[0]
-                extra_info.pop('CID', None)    # Remove 'CID': ... from lookup_result[0]
+                extra_info.pop('CID', None)
 
-                # Merge 2 dict: https://treyhunner.com/2016/02/how-to-merge-dictionaries-in-python/
                 result = {**core_result, **extra_info}
-                # Rename some keys in the dict
                 s = pd.Series(result)
                 s = s.rename({
                     'CanonicalSMILES': 'Canonical_SMILES',
                     'IsomericSMILES': 'Isomeric_SMILES',
                     'IUPACName': 'IUPAC_Name'
                 })
-                result = s.to_dict()            
+                result = s.to_dict()
                 return result
 
             else:
                 raise RuntimeError('pKa not found in Pubchem.')
-    
+
         else:
             raise RuntimeError('Compound not found in Pubchem.')
 
     except Exception as error:
         if debug:
             traceback_str = ''.join(traceback.format_exception(etype=type(error), value=error, tb=error.__traceback__))
             print(traceback_str)
```

### Comparing `chrfinder-0.0.3/src/Chrfinder/pubchemprops.py` & `chrfinder-1.0.0/src/Chrfinder/pubchemprops.py`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/src/Chrfinder/search_pka.py` & `chrfinder-1.0.0/src/Chrfinder/search_pka.py`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/tests/test_complete.py` & `chrfinder-1.0.0/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/.gitignore` & `chrfinder-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/LICENSE` & `chrfinder-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.3/README.md` & `chrfinder-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,167 @@
+Metadata-Version: 2.3
+Name: Chrfinder
+Version: 1.0.0
+Summary: The package find the best chromatography based on properties of the mixture
+Project-URL: source, https://github.com/Averhv/Chrfinder
+Project-URL: tracker, https://github.com/Averhv/Chrfinder/issues
+Author-email: Anthony Verhoeven <anthony.verhoeven@epfl.ch>
+License: MIT License
+        
+        Copyright (c) 2024 by Diogo Santos Martins <diogo.santosmartins@epfl.ch>
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Requires-Dist: pandas
+Requires-Dist: pubchempy
+Requires-Dist: tk
+Provides-Extra: doc
+Requires-Dist: furo; extra == 'doc'
+Requires-Dist: myst-parser; extra == 'doc'
+Requires-Dist: sphinx-copybutton; extra == 'doc'
+Requires-Dist: sphinx>=5; extra == 'doc'
+Provides-Extra: test
+Requires-Dist: genbadge[coverage]; extra == 'test'
+Requires-Dist: hypothesis; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: tox; extra == 'test'
+Description-Content-Type: text/markdown
+
 <p align="center">
   <img src="assets/Image_Chrfinder.webp" alt="Project Logo" width="650"/>
 </p>
 
 # Chrfinder
 
 ## <ins>Project overview</ins>
 
 <h1 align="center">
     
-[![PyPI version](https://img.shields.io/pypi/v/Chrfinder?style=plastic&color=blue)](https://pypi.python.org/pypi/Chrfinder) [![License](https://img.shields.io/github/license/Averhv/Chrfinder?style=plastic&color=Orange)](https://github.com/Averhv/Chrfinder/blob/master/LICENSE) <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/Chrfinder?style=plastic" />
+[![PyPI version](https://img.shields.io/pypi/v/Chrfinder?style=plastic&color=blue)](https://pypi.python.org/pypi/Chrfinder) 
+[![License](https://img.shields.io/github/license/Averhv/Chrfinder?style=plastic&color=Orange)](https://github.com/Averhv/Chrfinder/blob/master/LICENSE) 
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/Chrfinder?style=plastic" /> 
+[![Coverage Badge](https://github.com/Averhv/Chrfinder/blob/main/assets/coverage-badge.svg?short_path=eb9c651)](https://github.com/Averhv/Chrfinder)
+
+
 </h1>
 
 Welcome to **Chrfinder**! This project **automates the selection of the most suitable chromatography** technique . By simply providing the **names** of the molecules in the mixture, the code retrieves their physicochemical properties from **PubChem** (web source) and determines the optimal chromatography method based on these properties. It also gives the optimal conditions.
 
 ## ✅ <ins>Benefits</ins>
 
 - **🚀 Efficiency**: Automates the property retrieval and decision-making process, saving time and reducing manual effort.
 - **🎯 Accuracy**: Utilizes precise physicochemical data to ensure the most suitable chromatography technique is chosen.
 - **🌐 Versatility**: Supports a wide range of organic compounds and chromatography methods (PubChem database).
 
 
 ## ⚙ <ins>Installation</ins>
 
+To get started with Chrfinder, you can follow these steps:
 Create a new environment, you may also give the environment a different name. 
 
 ```bash
 conda create -n Chrfinder python=3.10 
 ```
-
+Then install it through pypi (easy, recommended):
 ```bash
 conda activate Chrfinder
+```
+```bash
 pip install Chrfinder
 ```
+You also have the choice to install it without pypi:
 
-## 🛠️ <ins>Installation for Development</ins>
-
-To get started with Chrfinder, you can follow these steps:
 ```bash
 git clone https://github.com/Averhv/Chrfinder.git
 cd Chrfinder
 pip install .
-pip install jupyterlab
-jupyter lab
 ```
-#### Optional: Installing for Development and Testing
-If you want to contribute to Chrfinder or run the tests and get coverage, you can install the package in editable mode along with the necessary dependencies for testing and documentation:
+
+## 🛠️ <ins>Installation for Development</ins>
+
+If you want to contribute to Chrfinder or run the tests and get coverage, you can install the package in editable mode along with the necessary dependencies for testing and documentation. The following script allows the changes to be reflected immediately:
 ```bash
 git clone https://github.com/Averhv/Chrfinder.git
 cd Chrfinder
 pip install -e ".[test,doc]"
-pip install jupyterlab
-jupyter lab
 ```
 
 Then you need to run the tests as follow in your terminal:
 ```bash
 pip install tox
 tox
 ```
-One can also run the following to get better **readability**:
-- runs tests for the Chrfinder.py file
-- measures code coverage
-- generates coverage reports in both XML and terminal formats
-- provides verbose output during test execution.
-```bash
-pytest --cov=src/Chrfinder.py --cov-report xml:.tox/coverage.xml --cov-report term -vv
-```
 Test result: 15 passed in ~20s
 ## 📒 <ins>Features</ins>
 
+The following should be written in the terminal in python mode:
 ```python
 from Chrfinder import main
-
-# Running the whole file ask for molecules through Tkinter and returns the best chromatography
+```
+Running the main file asks for molecules through Tkinter and returns the best chromatography.
+```python
 main()
 ```
 
 #### 🌐 Optional functions
 
-##### find_pka(inchikey)
+- find_pka(inchikey)
 Finds the pKa value for a compound using its InChIKey.
 ```python
 from Chrfinder import find_pka
 
 inchikey = "XEFQLINVKFYRCS-UHFFFAOYSA-N"
 find_pka(inchikey)
 ```
 
-##### find_boiling_point(name)
+- find_boiling_point(name)
 Finds the boiling point for a compound by name.
 ```python
 from Chrfinder import find_boiling_point
 
 compound_name = "Ethanol"
 find_boiling_point(compound_name)
 ```
 
-##### get_df_properties()
+- get_df_properties()
 Get a DataFrame of properties for a mixture of compounds.
 ```python
 from Chrfinder import get_df_properties
 
 mixture = ["Acetone", "Ethanol", "Methanol"]
 get_df_properties(mixture, verbose=True)
 ```
-
-## <ins>How It Works</ins>
-
-1. **Input**: User provides the names of the molecules present in the mixture through a Tkinter interface.
-
-2. **Data Retrieval**: Finds the following key physicochemical properties for each molecule in Pubchem:
-     - **Boiling temperature (°C)**
-     - **logP (partition coefficient)**
-     - **pKa (acid dissociation constants)**
-     - **Molecular mass**
-
-3. **Chromatography Type Decision**: Follows logical conditions to determine best chromatography and conditions
-   - **Gas Chromatography (GC)**: if the Boiling Point is low (T<sub>eb</sub> <250°C).
-   - **Ion Chromatography (IC)**: for small molecules (M<2000g/mol) and a negative maximum LogP negative
-     - Selected if the maximum molecular mass is less than or equal to 2000, and the maximum logP is negative, with a proposed pH derived from the pKa values.
-   - **High-Performance Liquid Chromatography (HPLC)**: Chosen for different conditions. Stationary phases and eluent natures are suggested.
-   - **Size Exclusion Chromatography (SEC)**: For big molecules (M>2000g/mol). From LogP, it suggest gel permeation or gel filtration, with corresponding eluant.
-
-4. **Output**:
-   - The code outputs the advisable chromatography type, the nature of the eluent (gas, aqueous, or organic), and the proposed pH for the eluent if applicable through the Tkinter interface.
   
 ## <ins>Work in progress...</ins>
 - **Efficiency: build a database**;
 - **Research thermostability** in lab to improve precision
 - Taking into account **multiple pKa values** for polyacids for exemple;
 - **Optimize the research**: search only one time the same name;
```

### Comparing `chrfinder-0.0.3/pyproject.toml` & `chrfinder-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Chrfinder"
-version = "0.0.3"
+version = "1.0.0"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 description = "The package find the best chromatography based on properties of the mixture"
 dependencies = [
     "pandas",
     "pubchempy",
```

