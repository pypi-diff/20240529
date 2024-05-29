# Comparing `tmp/orange3_singlecell-1.7.0.tar.gz` & `tmp/orange3_singlecell-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange3_singlecell-1.7.0.tar", last modified: Wed May 29 11:18:52 2024, max compression
+gzip compressed data, was "orange3_singlecell-1.7.1.tar", last modified: Wed May 29 12:23:47 2024, max compression
```

## Comparing `orange3_singlecell-1.7.0.tar` & `orange3_singlecell-1.7.1.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.774114 orange3_singlecell-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.734114 orange3_singlecell-1.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.734114 orange3_singlecell-1.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.734114 orange3_singlecell-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.github/workflows/rebase.yml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.774114 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-29 11:18:52.000000 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-29 11:18:52.000000 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:18:52.000000 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 11:18:52.000000 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 11:18:52.000000 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:18:52.000000 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-29 11:18:52.000000 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 11:18:52.000000 orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-29 11:18:52.774114 orange3_singlecell-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/README.pypi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.738113 orange3_singlecell-1.7.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.738113 orange3_singlecell-1.7.0/doc/static/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.738113 orange3_singlecell-1.7.0/doc/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/align_datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/batch_effect_removal.md
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/dot_matrix.md
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/filter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.742113 orange3_singlecell-1.7.0/doc/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/AlignDatasets.png
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/BatchEffectRemoval.png
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/DotMatrix.png
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/Filter.png
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/LoadData.png
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/LouvainClustering.png
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/MarkerGenes.png
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/Normalize.png
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/ScoreGenes.png
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/SingleCellDatasets.png
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/SingleCellPreprocess.png
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/icons/scorecells.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.746114 orange3_singlecell-1.7.0/doc/widgets/images/
--rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/Align_Datasets-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/Batch_Effect_Removal-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/Dot_Matrix-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)   452301 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/Filter-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)   413527 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/Filter-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)    24654 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/Load Data-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)   184974 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/LouvainClustering-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/LouvainClustering-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)    30841 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/Marker Genes-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/Normalize-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/ScoreCells-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)    73536 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/ScoreGenes-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)    59612 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/SingleCellDatasets-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)   187776 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/SpatialAutocorrelation-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    62116 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/SpatialAutocorrelation-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)   270259 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/images/tSNE-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/load_data.md
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/score_cells.md
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/score_genes.md
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/single_cell_datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/single_cell_preprocess.md
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets/spatial_autocorrelation.md
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/doc/widgets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.746114 orange3_singlecell-1.7.0/orangecontrib/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.746114 orange3_singlecell-1.7.0/orangecontrib/single_cell/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.746114 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/biweight.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/cca.py
--rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/clusteranalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.746114 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/data/
--rw-r--r--   0 runner    (1001) docker     (127)  8268912 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/data/bone_marrow_louvain.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/scbnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/scpreprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.762113 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.762113 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.730114 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.762113 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/barcodes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/genes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/matrix.mtx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.762113 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/barcodes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/genes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/matrix.mtx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.762113 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/barcodes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/genes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/matrix.mtx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.730114 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.766113 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/hg19/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/hg19/barcodes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/hg19/genes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/hg19/matrix.mtx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.766113 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/mm10/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/mm10/barcodes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/mm10/genes.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/10x/mm10/matrix.mtx
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/DATA_MATRIX_LOG_TPM.txt
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.loom
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)    27648 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.xls
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data_dense.h5ad
--rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data_sparse.h5ad
--rw-r--r--   0 runner    (1001) docker     (127)    31682 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/dermatology.tab
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/lib.cell.count
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/lib.cell.meta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.766113 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/test_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/test_cca.py
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/test_scbnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/test_scpreprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owaligndatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owbatchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owdatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owdotmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owdropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owgenerank.py
--rw-r--r--   0 runner    (1001) docker     (127)    17487 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owloaddata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owmultisample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owscorecells.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owscoregenes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owscpreprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owspatialautocorrelation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.770113 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17883 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/contingency_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:18:52.774114 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/AlignDatasets.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/BatchEffectRemoval.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Binarize.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/DotMatrix.svg
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Dropout.svg
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Filter.svg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/LoadData.svg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/LogarithmicScale.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/MarkerGenes.svg
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/MultiSample.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Normalize.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Rank.svg
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/ScoreCells.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/ScoreGenes.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/SelectGenes.svg
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/SingleCellDatasets.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/SingleCellPreprocess.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/SpatialAutocorrelation.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Standardize.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/VCFFile.svg
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/category.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28320 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21556 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owaligndatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owbatchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owdotmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owdropout.py
--rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25860 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owloaddata.py
--rw-r--r--   0 runner    (1001) docker     (127)    17828 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owmultisample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owscdatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owscorecells.py
--rw-r--r--   0 runner    (1001) docker     (127)    26130 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owscoregenes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23729 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owscpreprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owspatialautocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-29 11:18:52.774114 orange3_singlecell-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-29 11:18:48.000000 orange3_singlecell-1.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.149793 orange3_singlecell-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.109793 orange3_singlecell-1.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.109793 orange3_singlecell-1.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.109793 orange3_singlecell-1.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.github/workflows/rebase.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.149793 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-29 12:23:47.000000 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-29 12:23:47.000000 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:23:47.000000 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 12:23:47.000000 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 12:23:47.000000 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:23:47.000000 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-29 12:23:47.000000 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 12:23:47.000000 orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-29 12:23:47.149793 orange3_singlecell-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/README.pypi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.113793 orange3_singlecell-1.7.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.113793 orange3_singlecell-1.7.1/doc/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.113793 orange3_singlecell-1.7.1/doc/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/align_datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/batch_effect_removal.md
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/dot_matrix.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/filter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.117793 orange3_singlecell-1.7.1/doc/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/AlignDatasets.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/BatchEffectRemoval.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/DotMatrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/Filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/LoadData.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/LouvainClustering.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/MarkerGenes.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/Normalize.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/ScoreGenes.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/SingleCellDatasets.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/SingleCellPreprocess.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/icons/scorecells.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.121793 orange3_singlecell-1.7.1/doc/widgets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/Align_Datasets-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/Batch_Effect_Removal-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/Dot_Matrix-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)   452301 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/Filter-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)   413527 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/Filter-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24654 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/Load Data-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)   184974 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/LouvainClustering-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/LouvainClustering-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30841 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/Marker Genes-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/Normalize-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/ScoreCells-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73536 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/ScoreGenes-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59612 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/SingleCellDatasets-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)   187776 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/SpatialAutocorrelation-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62116 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/SpatialAutocorrelation-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)   270259 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/images/tSNE-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/load_data.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/score_cells.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/score_genes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/single_cell_datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/single_cell_preprocess.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets/spatial_autocorrelation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/doc/widgets.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.121793 orange3_singlecell-1.7.1/orangecontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.121793 orange3_singlecell-1.7.1/orangecontrib/single_cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.125793 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/biweight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/clusteranalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.125793 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  8268912 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/data/bone_marrow_louvain.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/scbnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/scpreprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.137793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.137793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.105793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.137793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/barcodes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/genes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/matrix.mtx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.141793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/barcodes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/genes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/matrix.mtx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.141793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/barcodes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/genes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/matrix.mtx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.105793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.141793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/hg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/hg19/barcodes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/hg19/genes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/hg19/matrix.mtx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.141793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/mm10/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/mm10/barcodes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/mm10/genes.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/10x/mm10/matrix.mtx
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/DATA_MATRIX_LOG_TPM.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.loom
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    27648 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data_dense.h5ad
+-rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data_sparse.h5ad
+-rw-r--r--   0 runner    (1001) docker     (127)    31682 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/dermatology.tab
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/lib.cell.count
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/lib.cell.meta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.141793 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/test_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/test_cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/test_scbnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/test_scpreprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owaligndatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owbatchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owdatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owdotmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owdropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owgenerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17487 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owloaddata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owmultisample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owscorecells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owscoregenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owscpreprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owspatialautocorrelation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.145793 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17883 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/contingency_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:23:47.149793 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/AlignDatasets.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/BatchEffectRemoval.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Binarize.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/DotMatrix.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Dropout.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Filter.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/LoadData.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/LogarithmicScale.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/MarkerGenes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/MultiSample.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Normalize.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Rank.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/ScoreCells.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/ScoreGenes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/SelectGenes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/SingleCellDatasets.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/SingleCellPreprocess.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/SpatialAutocorrelation.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Standardize.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/VCFFile.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/category.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29156 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21556 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owaligndatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owbatchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owdotmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owdropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25960 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owloaddata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17828 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owmultisample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owscdatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owscorecells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26130 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owscoregenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23729 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owscpreprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owspatialautocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-29 12:23:47.149793 orange3_singlecell-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-29 12:23:38.000000 orange3_singlecell-1.7.1/tox.ini
```

### Comparing `orange3_singlecell-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `orange3_singlecell-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `orange3_singlecell-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/.gitignore` & `orange3_singlecell-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/CHANGELOG.md` & `orange3_singlecell-1.7.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/CODE_OF_CONDUCT.md` & `orange3_singlecell-1.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/LICENSE` & `orange3_singlecell-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/PKG-INFO` & `orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-SingleCell
-Version: 1.7.0
+Version: 1.7.1
 Summary: Add-on for bioinformatics analysis of single cell data.
 Home-page: https://github.com/biolab/orange3-single-cell
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: info@biolab.si
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/biolab/orange3-single-cell/issues
 Project-URL: Documentation, https://singlecell.biolab.si/docs/
```

### Comparing `orange3_singlecell-1.7.0/Orange3_SingleCell.egg-info/SOURCES.txt` & `orange3_singlecell-1.7.1/Orange3_SingleCell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/PKG-INFO` & `orange3_singlecell-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-SingleCell
-Version: 1.7.0
+Version: 1.7.1
 Summary: Add-on for bioinformatics analysis of single cell data.
 Home-page: https://github.com/biolab/orange3-single-cell
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: info@biolab.si
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/biolab/orange3-single-cell/issues
 Project-URL: Documentation, https://singlecell.biolab.si/docs/
```

### Comparing `orange3_singlecell-1.7.0/README.md` & `orange3_singlecell-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/README.pypi` & `orange3_singlecell-1.7.1/README.pypi`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/Makefile` & `orange3_singlecell-1.7.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/conf.py` & `orange3_singlecell-1.7.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/make.bat` & `orange3_singlecell-1.7.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/static/custom.css` & `orange3_singlecell-1.7.1/doc/static/custom.css`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/align_datasets.md` & `orange3_singlecell-1.7.1/doc/widgets/align_datasets.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/filter.md` & `orange3_singlecell-1.7.1/doc/widgets/filter.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/AlignDatasets.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/AlignDatasets.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/BatchEffectRemoval.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/BatchEffectRemoval.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/DotMatrix.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/DotMatrix.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/Filter.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/Filter.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/LoadData.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/LoadData.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/LouvainClustering.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/LouvainClustering.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/MarkerGenes.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/MarkerGenes.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/Normalize.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/Normalize.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/ScoreGenes.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/ScoreGenes.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/SingleCellDatasets.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/SingleCellDatasets.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/SingleCellPreprocess.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/SingleCellPreprocess.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/icons/scorecells.png` & `orange3_singlecell-1.7.1/doc/widgets/icons/scorecells.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/Align_Datasets-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/Align_Datasets-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/Batch_Effect_Removal-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/Batch_Effect_Removal-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/Dot_Matrix-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/Dot_Matrix-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/Filter-Example.png` & `orange3_singlecell-1.7.1/doc/widgets/images/Filter-Example.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/Filter-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/Filter-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/Load Data-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/Load Data-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/LouvainClustering-Example.png` & `orange3_singlecell-1.7.1/doc/widgets/images/LouvainClustering-Example.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/LouvainClustering-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/LouvainClustering-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/Marker Genes-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/Marker Genes-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/Normalize-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/Normalize-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/ScoreCells-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/ScoreCells-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/ScoreGenes-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/ScoreGenes-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/SingleCellDatasets-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/SingleCellDatasets-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/SpatialAutocorrelation-Example.png` & `orange3_singlecell-1.7.1/doc/widgets/images/SpatialAutocorrelation-Example.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/SpatialAutocorrelation-stamped.png` & `orange3_singlecell-1.7.1/doc/widgets/images/SpatialAutocorrelation-stamped.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/images/tSNE-Example.png` & `orange3_singlecell-1.7.1/doc/widgets/images/tSNE-Example.png`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/score_cells.md` & `orange3_singlecell-1.7.1/doc/widgets/score_cells.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/score_genes.md` & `orange3_singlecell-1.7.1/doc/widgets/score_genes.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/single_cell_datasets.md` & `orange3_singlecell-1.7.1/doc/widgets/single_cell_datasets.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets/spatial_autocorrelation.md` & `orange3_singlecell-1.7.1/doc/widgets/spatial_autocorrelation.md`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/doc/widgets.json` & `orange3_singlecell-1.7.1/doc/widgets.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {'0': "{1: {insert: [(10, OrderedDict([('text', 'Spatial Autocorrelation Scorer'), ('doc', "*

 * *      "'widgets/spatial_autocorrelation.md'), ('icon', "*

 * *      "'../orangecontrib/single_cell/widgets/icons/SpatialAutocorrelation.svg'), ('background', "*

 * *      "'light-blue'), ('keywords', [])]))]}}"}*

```diff
@@ -71,11 +71,18 @@
             },
             {
                 "background": "light-blue",
                 "doc": "widgets/dot_matrix.md",
                 "icon": "../orangecontrib/single_cell/widgets/icons/DotMatrix.svg",
                 "keywords": [],
                 "text": "Dot Matrix"
+            },
+            {
+                "background": "light-blue",
+                "doc": "widgets/spatial_autocorrelation.md",
+                "icon": "../orangecontrib/single_cell/widgets/icons/SpatialAutocorrelation.svg",
+                "keywords": [],
+                "text": "Spatial Autocorrelation Scorer"
             }
         ]
     ]
 ]
```

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/alignment.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/alignment.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/biweight.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/biweight.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/cca.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/cca.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/clusteranalysis.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/clusteranalysis.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/data/bone_marrow_louvain.pickle` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/data/bone_marrow_louvain.pickle`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/scbnorm.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/scbnorm.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/preprocess/scpreprocess.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/preprocess/scpreprocess.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/reader.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/reader.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/genes.tsv` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/genes.tsv`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/matrix.mtx` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-A/matrix.mtx`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/genes.tsv` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/genes.tsv`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/matrix.mtx` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-B/matrix.mtx`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/barcodes.tsv` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/barcodes.tsv`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/genes.tsv` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/genes.tsv`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/matrix.mtx` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/010-Showcase-LoadDataM-Data/batch-C/matrix.mtx`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/DATA_MATRIX_LOG_TPM.txt` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/DATA_MATRIX_LOG_TPM.txt`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.csv` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.csv`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.loom` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.loom`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.pkl` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.pkl`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.xls` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.xls`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data.xlsx` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data.xlsx`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data_dense.h5ad` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data_dense.h5ad`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/data_sparse.h5ad` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/data_sparse.h5ad`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/dermatology.tab` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/dermatology.tab`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/data/lib.cell.meta` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/data/lib.cell.meta`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/test_alignment.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/test_alignment.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/test_cca.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/test_cca.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/test_scbnorm.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/test_scbnorm.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/preprocess/test_scpreprocess.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/preprocess/test_scpreprocess.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_load_data.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_load_data.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owaligndatasets.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owaligndatasets.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owbatchnorm.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owbatchnorm.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owdatasets.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owdatasets.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owdotmatrix.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owdotmatrix.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owdropout.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owdropout.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owfilter.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owfilter.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owgenerank.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owgenerank.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owloaddata.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owloaddata.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owmultisample.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owmultisample.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owscorecells.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owscorecells.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owscoregenes.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owscoregenes.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owscpreprocess.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owscpreprocess.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/tests/test_owspatialautocorrelation.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/tests/test_owspatialautocorrelation.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/__init__.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/contingency_table.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/contingency_table.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/AlignDatasets.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/AlignDatasets.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/BatchEffectRemoval.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/BatchEffectRemoval.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Binarize.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Binarize.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/DotMatrix.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/DotMatrix.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Dropout.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Dropout.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Filter.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Filter.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/LoadData.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/LoadData.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/LogarithmicScale.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/LogarithmicScale.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/MarkerGenes.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/MarkerGenes.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/MultiSample.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/MultiSample.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Normalize.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Normalize.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Rank.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Rank.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/ScoreCells.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/ScoreCells.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/ScoreGenes.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/ScoreGenes.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/SelectGenes.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/SelectGenes.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/SingleCellDatasets.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/SingleCellDatasets.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/SingleCellPreprocess.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/SingleCellPreprocess.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/SpatialAutocorrelation.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/SpatialAutocorrelation.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/Standardize.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/Standardize.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/VCFFile.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/VCFFile.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/icons/category.svg` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/load_data.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/load_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,20 +484,26 @@
 
     @leading_cols.setter
     def leading_cols(self, value):
         self._leading_cols = 0
 
     def _set_annotation_files(self):
         dir_name, _ = os.path.split(self._file_name)
-        genes_path = os.path.join(dir_name, "genes.tsv")
-        if os.path.isfile(genes_path):
-            self.col_annotation_file = RecentPath.create(genes_path, [])
-        barcodes_path = os.path.join(dir_name, "barcodes.tsv")
-        if os.path.isfile(barcodes_path):
-            self.row_annotation_file = RecentPath.create(barcodes_path, [])
+        genes_paths = ['genes.tsv', 'features.tsv', 'genes.tsv.gz', 'features.tsv.gz']
+        for genes_path in genes_paths:
+            genes_path = os.path.join(dir_name, genes_path)
+            if os.path.isfile(genes_path):
+                self.col_annotation_file = RecentPath.create(genes_path, [])
+                break
+        barcodes_paths = ['barcodes.tsv', 'barcodes.tsv.gz']
+        for barcodes_path in barcodes_paths:
+            barcodes_path = os.path.join(dir_name, barcodes_path)
+            if os.path.isfile(barcodes_path):
+                self.row_annotation_file = RecentPath.create(barcodes_path, [])
+                break
 
     def _set_enable_annotations(self):
         # 10x gene-barcode matrix
         # TODO: The genes/barcodes files should be unconditionally loaded
         # alongside the mtx. The row/col annotations might be used to
         # specify additional sources. For the time being they are put in
         # the corresponding comboboxes and made uneditable.
@@ -752,21 +758,29 @@
             def key(var):
                 return var.name if isinstance(var.name, str) else ""
 
             domain = Domain(sorted(attrs, key=key),
                             metas=sorted(metas, key=key))
             concat_data_t = concat_data.transform(domain)
             data_t = data.transform(domain)
-            source_var.values + (source_name, )
+
+            new_values = source_var.values + (source_name,)
+            new_source_var = DiscreteVariable(source_var.name, values=new_values)
+            new_metas = tuple(var if var.name != source_var.name else new_source_var for var in domain.metas)
+            new_domain = Domain(domain.attributes, metas=new_metas)
+            concat_data_t = concat_data_t.transform(new_domain)
+            data_t = data_t.transform(new_domain)
+            source_var_index = new_source_var.values.index(source_name)
             # metas can be unlocked, source_var added to metas by append_source_name
             with data_t.unlocked(data_t.metas):
-                data_t[:, source_var] = np.full(
-                    (len(data), 1), len(source_var.values) - 1, dtype=object
+                data_t[:, new_source_var] = np.full(
+                    (len(data_t), 1), source_var_index, dtype=object
                 )
             concat_data = Table.concatenate((concat_data_t, data_t), axis=0)
+            source_var = new_source_var # Update source_var for the next iteration
         return concat_data
 
     @staticmethod
     def append_source_name(data, name):
         source_var = DiscreteVariable("source", values=[name])
         metas = data.domain.metas + (source_var,)
         domain = Domain(data.domain.attributes, metas=metas)
```

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owaligndatasets.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owaligndatasets.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owbatchnorm.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owbatchnorm.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owdotmatrix.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owdotmatrix.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owdropout.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owdropout.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owfilter.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owfilter.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owloaddata.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owloaddata.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,14 +609,15 @@
             dlg.selectNameFilter(filters[0])
         if dlg.exec_() == QFileDialog.Accepted:
             filename = dlg.selectedFiles()[0]
             m = self.row_annotations_combo.model()  # type: QStandardItemModel
             pathitem = RecentPath.create(filename, [])
             index = insert_recent_path(m, pathitem)
             self.row_annotations_combo.setCurrentIndex(index)
+            self._row_annotations_combo_changed()
             self._invalidate()
 
     @Slot()
     def browse_col_annotations(self):
         dlg = QFileDialog(
             self, acceptMode=QFileDialog.AcceptOpen,
             fileMode=QFileDialog.ExistingFile
@@ -628,14 +629,15 @@
             dlg.selectNameFilter(filters[0])
         if dlg.exec_() == QFileDialog.Accepted:
             filename = dlg.selectedFiles()[0]
             m = self.col_annotations_combo.model()  # type: QStandardItemModel
             pathitem = RecentPath.create(filename, [])
             index = insert_recent_path(m, pathitem)
             self.col_annotations_combo.setCurrentIndex(index)
+            self._col_annotations_combo_changed()
             self._invalidate()
 
     def _invalidate(self):
         self.set_modified(True)
 
     def set_modified(self, modified):
         if modified:
```

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owmultisample.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owmultisample.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owscdatasets.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owscdatasets.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owscorecells.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owscorecells.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owscoregenes.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owscoregenes.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owscpreprocess.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owscpreprocess.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/orangecontrib/single_cell/widgets/owspatialautocorrelation.py` & `orange3_singlecell-1.7.1/orangecontrib/single_cell/widgets/owspatialautocorrelation.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/setup.cfg` & `orange3_singlecell-1.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/setup.py` & `orange3_singlecell-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `orange3_singlecell-1.7.0/tox.ini` & `orange3_singlecell-1.7.1/tox.ini`

 * *Files identical despite different names*

