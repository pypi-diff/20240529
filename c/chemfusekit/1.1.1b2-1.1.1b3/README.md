# Comparing `tmp/chemfusekit-1.1.1b2.tar.gz` & `tmp/chemfusekit-1.1.1b3.tar.gz`

## Comparing `chemfusekit-1.1.1b2.tar` & `chemfusekit-1.1.1b3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.python-version
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.releaserc.yml
--rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/CHANGELOG.md
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/requirements-dev.lock
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/requirements.lock
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/gh_pages.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/release.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/thesis.yml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/__init__.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/__utils.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/knn.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/lda.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/lldf.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/lr.py
--rw-r--r--   0        0        0     9783 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/pca.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/plsda.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/svm.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/README.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/babel.config.js
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docusaurus.config.js
--rw-r--r--   0        0        0  1020872 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/package-lock.json
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/package.json
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/sidebars.js
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/complete-workflow.md
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/tutorial.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/knn/_category_.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/knn/knn.md
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/knn/knnsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lda/_category_.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lda/lda.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lda/ldasettings.md
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lldf/_category_.json
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lldf/lldf.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lldf/lldfmodel.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lldf/lldfsettings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lr/_category_.json
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lr/lr.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lr/lrsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/pca/_category_.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/pca/pca.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/pca/pcasettings.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/plsda/_category_.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/plsda/plsda.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/plsda/plsdasettings.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/svm/_category_.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/svm/svm.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/svm/svmsettings.md
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/_category_.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/graphmode.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/graphoutput.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/printconfusionmatrix.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/printtable.md
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/runsplittests.md
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/css/custom.css
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/index.module.css
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/_category_.json
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/continuous-integration.md
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/index.md
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/process-model.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/project-philosophy.md
--rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/project-plan.md
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/requirements-specification.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/use-cases.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/.nojekyll
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/colab-logo.svg
--rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/favicon.ico
--rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/happy-woman.svg
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/logo.svg
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/magnifying-glass.svg
--rw-r--r--   0        0        0   241829 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/knn_notebook.ipynb
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/pca_lda_notebook.ipynb
--rw-r--r--   0        0        0  1664059 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/pca_lr_notebook.ipynb
--rw-r--r--   0        0        0   533536 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/plsda_notebook.ipynb
--rw-r--r--   0        0        0   176230 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/svm_notebook.ipynb
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Beartype.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Constructors.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Conventional Commits.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Kanban.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Logistic Regression.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/PCA-LR.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/PCA.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/PEP coding standards.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/SVM.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/To do.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Use Case Diagram.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/kNN.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/app.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/appearance.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/community-plugins.json
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/core-plugins.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/daily-notes.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/templates.json
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/workspace.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/calendar/data.json
--rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/calendar/main.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/calendar/manifest.json
--rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/main.js
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/manifest.json
--rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/styles.css
--rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/main.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/styles.css
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-04-19.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-04-20.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-04-22.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-04-23.md
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-06.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-07.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-08.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-09.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-17.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-18.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Templates/Daily devlog.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/UML/Components.md
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/UML/Process state machine.md
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/UML/Sequence.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/UML/Use cases.md
--rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/qepas.xlsx
--rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/rt.xlsx
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_knn.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_lda.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_lldf.py
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_lr.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_pca.py
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_plsda.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_svm.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/0-header.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/1-abstract.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/2-index.md.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/3-intro.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/999-ringraziamenti.md
--rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/logo-unibg.png
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.gitignore
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/pyproject.toml
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/readme.md
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/.python-version
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/.releaserc.yml
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/CHANGELOG.md
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/requirements-dev.lock
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/requirements.lock
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/.github/workflows/gh_pages.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/.github/workflows/thesis.yml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/__init__.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/__utils.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/knn.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/lda.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/lldf.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/lr.py
+-rw-r--r--   0        0        0     9783 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/pca.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/plsda.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/chemfusekit/svm.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/README.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/babel.config.js
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docusaurus.config.js
+-rw-r--r--   0        0        0  1020872 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/package-lock.json
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/package.json
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/sidebars.js
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/complete-workflow.md
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/tutorial.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/knn/_category_.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/knn/knn.md
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/knn/knnsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lda/_category_.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lda/lda.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lda/ldasettings.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lldf/_category_.json
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lldf/lldf.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lldf/lldfmodel.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lldf/lldfsettings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lr/_category_.json
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lr/lr.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/lr/lrsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/pca/_category_.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/pca/pca.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/pca/pcasettings.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/plsda/_category_.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/plsda/plsda.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/plsda/plsdasettings.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/svm/_category_.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/svm/svm.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/svm/svmsettings.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/utils/_category_.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/utils/graphmode.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/utils/graphoutput.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/utils/printconfusionmatrix.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/utils/printtable.md
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/docs/utils/runsplittests.md
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/css/custom.css
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/project/_category_.json
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/project/continuous-integration.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/project/index.md
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/project/process-model.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/project/project-philosophy.md
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/project/project-plan.md
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/project/requirements-specification.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/src/pages/project/use-cases.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/static/.nojekyll
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/static/img/colab-logo.svg
+-rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/static/img/happy-woman.svg
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/docs/static/img/magnifying-glass.svg
+-rw-r--r--   0        0        0   241811 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/examples/knn_notebook.ipynb
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/examples/pca_lda_notebook.ipynb
+-rw-r--r--   0        0        0  1664059 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/examples/pca_lr_notebook.ipynb
+-rw-r--r--   0        0        0   533536 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/examples/plsda_notebook.ipynb
+-rw-r--r--   0        0        0   176230 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/examples/svm_notebook.ipynb
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Beartype.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Constructors.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Conventional Commits.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Kanban.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Logistic Regression.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/PCA-LR.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/PCA.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/PEP coding standards.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/SVM.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/To do.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Use Case Diagram.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/kNN.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/app.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/appearance.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/community-plugins.json
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/daily-notes.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/templates.json
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/workspace.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/calendar/data.json
+-rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/calendar/main.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/calendar/manifest.json
+-rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-kanban/main.js
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-kanban/manifest.json
+-rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-kanban/styles.css
+-rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-plantuml/main.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-plantuml/styles.css
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-04-19.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-04-20.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-04-22.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-04-23.md
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-05-06.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-05-07.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-05-08.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-05-09.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-05-17.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Devlog/2024-05-18.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/Templates/Daily devlog.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/UML/Components.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/UML/Process state machine.md
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/UML/Sequence.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/notes/UML/Use cases.md
+-rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/qepas.xlsx
+-rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/rt.xlsx
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/test_knn.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/test_lda.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/test_lldf.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/test_lr.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/test_pca.py
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/test_plsda.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/tests/test_svm.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/thesis/0-header.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/thesis/1-abstract.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/thesis/2-index.md.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/thesis/3-intro.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/thesis/999-ringraziamenti.md
+-rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/thesis/logo-unibg.png
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/.gitignore
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/pyproject.toml
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/readme.md
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b3/PKG-INFO
```

### Comparing `chemfusekit-1.1.1b2/.releaserc.yml` & `chemfusekit-1.1.1b3/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/CHANGELOG.md` & `chemfusekit-1.1.1b3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [1.1.1-beta.3](https://github.com/f-aguzzi/tesi/compare/v1.1.1-beta.2...v1.1.1-beta.3) (2024-05-29)
+
+
+### Bug Fixes
+
+* docs workflow, dependency clashes, demos ([6f72ec4](https://github.com/f-aguzzi/tesi/commit/6f72ec4a0c51902e05e468b6d6f79042a3bc73e5)), closes [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28)
+
 ## [1.1.1-beta.2](https://github.com/f-aguzzi/tesi/compare/v1.1.1-beta.1...v1.1.1-beta.2) (2024-05-24)
 
 
 ### Bug Fixes
 
 * wrong training procedure in SVM ([#25](https://github.com/f-aguzzi/tesi/issues/25)) ([7f25487](https://github.com/f-aguzzi/tesi/commit/7f254876fcdbd2ba5c46278d31eb851a50659e8f))
```

### Comparing `chemfusekit-1.1.1b2/requirements-dev.lock` & `chemfusekit-1.1.1b3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/requirements.lock` & `chemfusekit-1.1.1b3/requirements.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/.github/workflows/gh_pages.yml` & `chemfusekit-1.1.1b3/.github/workflows/gh_pages.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,43 @@
   push:
     branches:
       - main
     # Review gh actions docs if you want to further define triggers, paths, etc
     # https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#on
     paths:
       - 'docs/**'
+      - '.github/workflows/gh_pages.yml'
+  pull_request:
+    branches:
+      - main
+    paths:
+      - 'docs/**'
+      - '.github/workflows/gh_pages.yml'
 
 jobs:
   build:
     name: Build Docusaurus
     runs-on: ubuntu-latest 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - uses: actions/setup-node@v4
         with:
           node-version: 18
           cache: npm
           cache-dependency-path: docs
-
       - name: Install dependencies
+        if: github.event.name == 'release'
         run: |
           cd ${GITHUB_WORKSPACE}/docs
           npm install --frozen-lockfile
+      - name: Generate new version
+        run: |
+          npm run docusaurus docs:version
       - name: Build website
         run: |
           cd ${GITHUB_WORKSPACE}/docs
           npm run build
 
       - name: Upload Build Artifact
         uses: actions/upload-pages-artifact@v3
```

### Comparing `chemfusekit-1.1.1b2/.github/workflows/pylint.yml` & `chemfusekit-1.1.1b3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/.github/workflows/release.yml` & `chemfusekit-1.1.1b3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/.github/workflows/thesis.yml` & `chemfusekit-1.1.1b3/.github/workflows/thesis.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/.github/workflows/unittest.yml` & `chemfusekit-1.1.1b3/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/chemfusekit/__utils.py` & `chemfusekit-1.1.1b3/chemfusekit/__utils.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/chemfusekit/knn.py` & `chemfusekit-1.1.1b3/chemfusekit/knn.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/chemfusekit/lda.py` & `chemfusekit-1.1.1b3/chemfusekit/lda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/chemfusekit/lldf.py` & `chemfusekit-1.1.1b3/chemfusekit/lldf.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/chemfusekit/lr.py` & `chemfusekit-1.1.1b3/chemfusekit/lr.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/chemfusekit/pca.py` & `chemfusekit-1.1.1b3/chemfusekit/pca.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/chemfusekit/plsda.py` & `chemfusekit-1.1.1b3/chemfusekit/plsda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/chemfusekit/svm.py` & `chemfusekit-1.1.1b3/chemfusekit/svm.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/README.md` & `chemfusekit-1.1.1b3/docs/README.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docusaurus.config.js` & `chemfusekit-1.1.1b3/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/package-lock.json` & `chemfusekit-1.1.1b3/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/package.json` & `chemfusekit-1.1.1b3/docs/package.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/sidebars.js` & `chemfusekit-1.1.1b3/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/complete-workflow.md` & `chemfusekit-1.1.1b3/docs/docs/complete-workflow.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/tutorial.md` & `chemfusekit-1.1.1b3/docs/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/knn/knn.md` & `chemfusekit-1.1.1b3/docs/docs/knn/knn.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/knn/knnsettings.md` & `chemfusekit-1.1.1b3/docs/docs/knn/knnsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/lda/lda.md` & `chemfusekit-1.1.1b3/docs/docs/lda/lda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/lda/ldasettings.md` & `chemfusekit-1.1.1b3/docs/docs/lda/ldasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/lldf/lldf.md` & `chemfusekit-1.1.1b3/docs/docs/lldf/lldf.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/lldf/lldfsettings.md` & `chemfusekit-1.1.1b3/docs/docs/lldf/lldfsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/lr/lr.md` & `chemfusekit-1.1.1b3/docs/docs/lr/lr.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/lr/lrsettings.md` & `chemfusekit-1.1.1b3/docs/docs/lr/lrsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/pca/pca.md` & `chemfusekit-1.1.1b3/docs/docs/pca/pca.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/pca/pcasettings.md` & `chemfusekit-1.1.1b3/docs/docs/pca/pcasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/plsda/plsda.md` & `chemfusekit-1.1.1b3/docs/docs/plsda/plsda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/plsda/plsdasettings.md` & `chemfusekit-1.1.1b3/docs/docs/plsda/plsdasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/svm/svm.md` & `chemfusekit-1.1.1b3/docs/docs/svm/svm.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/svm/svmsettings.md` & `chemfusekit-1.1.1b3/docs/docs/svm/svmsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/docs/utils/graphoutput.md` & `chemfusekit-1.1.1b3/docs/docs/utils/graphoutput.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/src/components/HomepageFeatures/index.js` & `chemfusekit-1.1.1b3/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/src/css/custom.css` & `chemfusekit-1.1.1b3/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/src/pages/index.js` & `chemfusekit-1.1.1b3/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/src/pages/project/continuous-integration.md` & `chemfusekit-1.1.1b3/docs/src/pages/project/continuous-integration.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/src/pages/project/process-model.md` & `chemfusekit-1.1.1b3/docs/src/pages/project/process-model.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/src/pages/project/project-philosophy.md` & `chemfusekit-1.1.1b3/docs/src/pages/project/project-philosophy.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/src/pages/project/project-plan.md` & `chemfusekit-1.1.1b3/docs/src/pages/project/project-plan.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 author: Federico Aguzzi
 date: apr 18, 2024
 ---
 
 # Project Plan
 
 :::note
-This project plan was written on April 18th, 2024. The project priorities have changed since then. For a constantly updated document about the philosophy and goals of this project, check out [Project Philosophy](./project-philosophy.md).
+This project plan was written on April 18th, 2024. The project priorities have changed since then. For a constantly updated document about the philosophy and goals of this project, check out [Project Philosophy](./project-philosophy).
 :::
 
 A 14-point project plan, highlighting the strategies and techniques employed in
 this project.
 
 ## 1. Introduction
```

### Comparing `chemfusekit-1.1.1b2/docs/src/pages/project/requirements-specification.md` & `chemfusekit-1.1.1b3/docs/src/pages/project/requirements-specification.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 author: Federico Aguzzi, Giorgio Felizzato
 date: apr 18, 2024
 ---
 
 # Requirements Specification
 
 :::note
-This requirements specification was written on April 18th, 2024. The project priorities have changed since then. For a constantly updated document about the philosophy and goals of this project, check out [Project Philosophy](./project-philosophy.md).
+This requirements specification was written on April 18th, 2024. The project priorities have changed since then. For a constantly updated document about the philosophy and goals of this project, check out [Project Philosophy](./project-philosophy).
 :::
 
 ## <u>Introduction</u>
 
 The purpose of this project is twofold:
 
 1. extract a library from [Dr
@@ -21,41 +21,41 @@
   user-friendly.
 
 To reuse as much code as possible from Felizzato's original scripts, the
 project should be implemented in Python.
 
 The project is partly inspired from the
 [`Spectra`](https://www.spectrapp.unito.it/app/spectrapp) web app made by the
-Univeristy of Torino, but with a twist: it will be based on an innovative _data
+University of Torino, but with a twist: it will be based on an innovative _data
 fusion_ approach that will analyze and process data from multiple sensors of
-multiple tipes, all at once, to give the best possible chemometrical
+multiple types, all at once, to give the best possible chemometrical
 classification on the given data.
 
 ## <u>Input data</u>
 
-The chemiometric data comes from two types of sensors: a gas chromatographer
-and a gas spectrometer. The chromatographer outputs a single value for each
+The chemometric data comes from two types of sensors: a gas chromatograph
+and a gas spectrometer. The chromatograph outputs a single value for each
 sample, a retention time in milliseconds. The spectrometer outputs an array of
 spectrum responses for a set of infrared wavelength bands.
 
 The data is stored in Excel files.
 
 A dataset of pre-classified sample data from lab tests is available for the
 purpose of training the classification algorithms.
 
 ### Pre-processing
 
 The gas chromatography data requires rescaling. The spectrometry data can be
 normalized, smoothed with a Savitski-Golay filter, or both.
 
-## <u>Functions</u>
+## <u>Functionality</u>
 
-### Data Analisys
+### Data Analysis
 
-The data can be analyzed with a PCA (Principal Component Analisys) pass to
+The data can be analyzed with a PCA (Principal Component Analysis) pass to
 assess whether its dimensionality can be reduced before the classification
 process.
 
 ### Classification Algorithms
 
 The available classification algorithms are:
 
@@ -97,38 +97,38 @@
 As an additional requirement, if the application will be made web-based, it
 must destroy all data stored remotely as soon as the session expires.
 
 ### Maintenance
 
 This application, being born as an undergraduate thesis project, will not be
 maintained by its original author. It is paramount, therefore, to make it as
-maintainable, well-strucutred and well-documented as possible.
+maintainable, well-structured and well-documented as possible.
 
 As an additional goal, it should be simple enough that non-programmers with a
 Python background will be able to add new classification algorithms.
 
 ## <u>Extensions</u>
 
 The first part of the project is the extraction of a library. The second is to
-make a GUI app. Both will be extensible, but the _must have_ goal is to make
+make a GUI app. Both will be extensible, but the _must-have_ goal is to make
 the library in particular as usable (and reusable) as possible.
 
 ## <u>Required Documents</u>
 
 Usage instructions must be provided.
 
 Ample and extensive documentation on the source code, the project structure and
-the chemiometric algorithms used must be also provided, to aid future updates
+the chemometric algorithms used must be also provided, to aid future updates
 and adjustments to the software.
 
 ## <u>Performance Requirements</u>
 
 Since statistical training and classification are computation-heavy tasks, the
 graphical components must be as light as possible, to avoid a further decrease
 in the processing speed.
 
 ## <u>Feasibility</u>
 
 Extracting the library is completely feasible. Making an application,
 especially one that can be easily expanded and maintained, is a much more
-complex task. In case the second will prove to be unachieavable, a good enough
+complex task. In case the second will prove to be unachievable, a good enough
 library will be acceptable on its own.
```

### Comparing `chemfusekit-1.1.1b2/docs/src/pages/project/use-cases.md` & `chemfusekit-1.1.1b3/docs/src/pages/project/use-cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/static/img/colab-logo.svg` & `chemfusekit-1.1.1b3/docs/static/img/colab-logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/static/img/docusaurus-social-card.jpg` & `chemfusekit-1.1.1b3/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/static/img/docusaurus.png` & `chemfusekit-1.1.1b3/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/static/img/favicon.ico` & `chemfusekit-1.1.1b3/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/static/img/happy-woman.svg` & `chemfusekit-1.1.1b3/docs/static/img/happy-woman.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/static/img/logo.svg` & `chemfusekit-1.1.1b3/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/docs/static/img/magnifying-glass.svg` & `chemfusekit-1.1.1b3/docs/static/img/magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/examples/knn_notebook.ipynb` & `chemfusekit-1.1.1b3/examples/knn_notebook.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997222222222222%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(6, "    qepas_path=\'qepas.xlsx\',    # (or put the name '*

 * *            'of your files)\\n"), (8, "    rt_path=\'rt.xlsx\',\\n")], delete: [8, 6]}}}'}*

```diff
@@ -46,17 +46,17 @@
             "source": [
                 "%matplotlib inline \n",
                 "\n",
                 "from chemfusekit.lldf import LLDFSettings, LLDF\n",
                 "\n",
                 "# Initialize the settings for low-level data fusion\n",
                 "lldf_settings = LLDFSettings(\n",
-                "    qepas_path='../tests/qepas.xlsx',    # (or put the name of your files)\n",
+                "    qepas_path='qepas.xlsx',    # (or put the name of your files)\n",
                 "    qepas_sheet='Sheet1',\n",
-                "    rt_path='../tests/rt.xlsx',\n",
+                "    rt_path='rt.xlsx',\n",
                 "    rt_sheet='Sheet1',\n",
                 "    preprocessing='snv'  # normalization preprocessing; other options: savgol or both\n",
                 ")\n",
                 "\n",
                 "# Initialize and run low-level data fusion\n",
                 "lldf = LLDF(lldf_settings)\n",
                 "lldf.lldf()"
```

### Comparing `chemfusekit-1.1.1b2/examples/pca_lda_notebook.ipynb` & `chemfusekit-1.1.1b3/examples/pca_lda_notebook.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997474747474747%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(6, "    qepas_path=\'qepas.xlsx\',    # (or put the name '*

 * *            'of your files)\\n"), (8, "    rt_path=\'rt.xlsx\',\\n")], delete: [8, 6]}}}'}*

```diff
@@ -46,17 +46,17 @@
             "source": [
                 "%matplotlib inline \n",
                 "\n",
                 "from chemfusekit.lldf import LLDFSettings, LLDF\n",
                 "\n",
                 "# Initialize the settings for low-level data fusion\n",
                 "lldf_settings = LLDFSettings(\n",
-                "    qepas_path='tests/qepas.xlsx',    # (or put the name of your files)\n",
+                "    qepas_path='qepas.xlsx',    # (or put the name of your files)\n",
                 "    qepas_sheet='Sheet1',\n",
-                "    rt_path='tests/rt.xlsx',\n",
+                "    rt_path='rt.xlsx',\n",
                 "    rt_sheet='Sheet1',\n",
                 "    preprocessing='snv'  # normalization preprocessing; other options: savgol or both\n",
                 ")\n",
                 "\n",
                 "# Initialize and run low-level data fusion\n",
                 "lldf = LLDF(lldf_settings)\n",
                 "lldf.lldf()"
```

### Comparing `chemfusekit-1.1.1b2/examples/pca_lr_notebook.ipynb` & `chemfusekit-1.1.1b3/examples/pca_lr_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/examples/plsda_notebook.ipynb` & `chemfusekit-1.1.1b3/examples/plsda_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/examples/svm_notebook.ipynb` & `chemfusekit-1.1.1b3/examples/svm_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Beartype.md` & `chemfusekit-1.1.1b3/notes/Beartype.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Constructors.md` & `chemfusekit-1.1.1b3/notes/Constructors.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Conventional Commits.md` & `chemfusekit-1.1.1b3/notes/Conventional Commits.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Use Case Diagram.md` & `chemfusekit-1.1.1b3/notes/Use Case Diagram.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/.obsidian/core-plugins-migration.json` & `chemfusekit-1.1.1b3/notes/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/.obsidian/workspace.json` & `chemfusekit-1.1.1b3/notes/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/.obsidian/plugins/calendar/main.js` & `chemfusekit-1.1.1b3/notes/.obsidian/plugins/calendar/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/main.js` & `chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-kanban/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/styles.css` & `chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-kanban/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/main.js` & `chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-plantuml/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/styles.css` & `chemfusekit-1.1.1b3/notes/.obsidian/plugins/obsidian-plantuml/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-04-19.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-04-19.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-04-20.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-04-20.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-04-22.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-04-22.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-04-23.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-04-23.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-05-06.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-05-06.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-05-07.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-05-07.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-05-08.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-05-08.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-05-09.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-05-09.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-05-17.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-05-17.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/Devlog/2024-05-18.md` & `chemfusekit-1.1.1b3/notes/Devlog/2024-05-18.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/UML/Process state machine.md` & `chemfusekit-1.1.1b3/notes/UML/Process state machine.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/UML/Sequence.md` & `chemfusekit-1.1.1b3/notes/UML/Sequence.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/notes/UML/Use cases.md` & `chemfusekit-1.1.1b3/notes/UML/Use cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/qepas.xlsx` & `chemfusekit-1.1.1b3/tests/qepas.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/rt.xlsx` & `chemfusekit-1.1.1b3/tests/rt.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/test_knn.py` & `chemfusekit-1.1.1b3/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/test_lda.py` & `chemfusekit-1.1.1b3/tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/test_lldf.py` & `chemfusekit-1.1.1b3/tests/test_lldf.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/test_lr.py` & `chemfusekit-1.1.1b3/tests/test_lr.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/test_pca.py` & `chemfusekit-1.1.1b3/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/test_plsda.py` & `chemfusekit-1.1.1b3/tests/test_plsda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/tests/test_svm.py` & `chemfusekit-1.1.1b3/tests/test_svm.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/thesis/0-header.md` & `chemfusekit-1.1.1b3/thesis/0-header.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/thesis/1-abstract.md` & `chemfusekit-1.1.1b3/thesis/1-abstract.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/thesis/logo-unibg.png` & `chemfusekit-1.1.1b3/thesis/logo-unibg.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/pyproject.toml` & `chemfusekit-1.1.1b3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "chemfusekit"
-version = "1.1.1b2"
+version = "1.1.1b3"
 description = "A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis."
 authors = [
     { name = "Federico Aguzzi", email = "62149513+f-aguzzi@users.noreply.github.com" }
 ]
 dependencies = [
     "numpy>=1.26.4",
     "scipy>=1.13.0",
     "matplotlib>=3.8.4",
-    "pandas>=2.2.2",
+    "pandas==2.0.3",
     "seaborn>=0.13.2",
     "openpyxl>=3.1.2",
     "scikit-learn>=1.4.2",
     "plotly>=5.22.0",
     "beartype>=0.18.5",
     "nbformat>=4.2.0",
     "tabulate>=0.9.0",
```

### Comparing `chemfusekit-1.1.1b2/readme.md` & `chemfusekit-1.1.1b3/readme.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b2/PKG-INFO` & `chemfusekit-1.1.1b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: chemfusekit
-Version: 1.1.1b2
+Version: 1.1.1b3
 Summary: A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis.
 Author-email: Federico Aguzzi <62149513+f-aguzzi@users.noreply.github.com>
 Requires-Python: >=3.8
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: nbformat>=4.2.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: openpyxl>=3.1.2
-Requires-Dist: pandas>=2.2.2
+Requires-Dist: pandas==2.0.3
 Requires-Dist: plotly>=5.22.0
 Requires-Dist: scikit-learn>=1.4.2
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: seaborn>=0.13.2
 Requires-Dist: tabulate>=0.9.0
 Description-Content-Type: text/markdown
```

