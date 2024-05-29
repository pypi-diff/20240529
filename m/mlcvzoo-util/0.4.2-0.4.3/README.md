# Comparing `tmp/mlcvzoo_util-0.4.2.tar.gz` & `tmp/mlcvzoo_util-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_util-0.4.2.tar", last modified: Thu May 16 06:41:17 2024, max compression
+gzip compressed data, was "mlcvzoo_util-0.4.3.tar", last modified: Wed May 29 16:18:31 2024, max compression
```

## Comparing `mlcvzoo_util-0.4.2.tar` & `mlcvzoo_util-0.4.3.tar`

### file list

```diff
@@ -1,242 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.editorconfig
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.915985 mlcvzoo_util-0.4.2/.gitlab/issue_templates/
--rw-rw-rw-   0 root         (0) root         (0)      919 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.gitlab/issue_templates/Bug.md
--rw-rw-rw-   0 root         (0) root         (0)     1156 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.gitlab/issue_templates/Implementation.md
--rw-rw-rw-   0 root         (0) root         (0)      928 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.gitlab/issue_templates/Refactoring.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.915985 mlcvzoo_util-0.4.2/.gitlab/merge_request_templates/
--rw-rw-rw-   0 root         (0) root         (0)     1852 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.gitlab/merge_request_templates/Default.md
--rw-rw-rw-   0 root         (0) root         (0)     1815 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2240 2024-05-16 05:39:15.000000 mlcvzoo_util-0.4.2/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     1529 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    11412 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2317 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)     1584 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/config/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.915985 mlcvzoo_util-0.4.2/config/templates/tools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.915985 mlcvzoo_util-0.4.2/config/templates/tools/cvat_annotation_handler/
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/config/templates/tools/cvat_annotation_handler/cvat-client-config_template.yaml
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/config/templates/tools/model-timer_config_template.yaml
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/config/templates/tools/model-trainer_config_template.yaml
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/config/templates/tools/video-image-creator_template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.919985 mlcvzoo_util-0.4.2/documentation/
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/01_introduction_and_goals.adoc
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/02_architecture_constraints.adoc
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/03_system_scope_and_context.adoc
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/04_solution_strategy.adoc
--rw-rw-rw-   0 root         (0) root         (0)     1684 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/05_building_block_view.adoc
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/06_runtime_view.adoc
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/08_concepts.adoc
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/09_design_decisions.adoc
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/10_quality_scenarios.adoc
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/11_technical_risks.adoc
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/documentation/12_tutorial.adoc
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/about-arc42.adoc
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/glossary.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2394 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/index.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.919985 mlcvzoo_util-0.4.2/mlcvzoo_util/
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.923985 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7348 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     6110 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     8392 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py
--rw-rw-rw-   0 root         (0) root         (0)     9831 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12973 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/image_io_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.923985 mlcvzoo_util-0.4.2/mlcvzoo_util/logger/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/logger/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3940 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.923985 mlcvzoo_util-0.4.2/mlcvzoo_util/ls_tracking_task_converter/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/ls_tracking_task_converter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11102 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/ls_tracking_task_converter/ls_tracking_task_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     4220 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/mlcvzoo_cli_tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.923985 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3032 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     8565 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/metric_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    16735 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/model_evaluator.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/structs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.927985 mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     9776 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/model_timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.927985 mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      741 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     6628 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/model_trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.927985 mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1380 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    12700 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:41:12.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.927985 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/
--rw-rw-rw-   0 root         (0) root         (0)    28509 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_cvat_annotation_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_image_io_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    27110 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_model_evaluator.py
--rw-rw-rw-   0 root         (0) root         (0)     2935 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_model_timer.py
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_model_trainer.py
--rw-rw-rw-   0 root         (0) root         (0)     6003 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_pre_annotation_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2308 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_template.py
--rw-rw-rw-   0 root         (0) root         (0)     2653 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_templates.py
--rw-rw-rw-   0 root         (0) root         (0)    20745 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_tracking_task_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     4754 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_video_image_creator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.931985 mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    14451 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/video_image_creator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2317 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9873 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      339 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)   196676 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/poetry.lock
--rw-rw-rw-   0 root         (0) root         (0)     4581 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.931985 mlcvzoo_util-0.4.2/requirements_locked/
--rw-rw-rw-   0 root         (0) root         (0)     4577 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/requirements_locked/requirements-lock-uv-py310-all.txt
--rw-rw-rw-   0 root         (0) root         (0)     3793 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/requirements_locked/requirements-lock-uv-py310-without-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 06:41:17.963986 mlcvzoo_util-0.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.931985 mlcvzoo_util-0.4.2/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.931985 mlcvzoo_util-0.4.2/test_data/annotations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.935985 mlcvzoo_util-0.4.2/test_data/annotations/coco/
--rw-rw-rw-   0 root         (0) root         (0)     6167 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/coco/coco.json
--rw-rw-rw-   0 root         (0) root         (0)     4197 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/coco/coco_alternate.json
--rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/coco/coco_evaluation.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.935985 mlcvzoo_util-0.4.2/test_data/annotations/csv_annotations/
--rw-rw-rw-   0 root         (0) root         (0)      386 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/csv_annotations/test-evaluation.csv
--rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/csv_annotations/test-task_eval.csv
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/csv_annotations/test-task_train.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.935985 mlcvzoo_util-0.4.2/test_data/annotations/cvat/
--rw-rw-rw-   0 root         (0) root         (0)     2479 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/cvat/cvat-for-clean-annotations.xml
--rw-rw-rw-   0 root         (0) root         (0)     3973 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/cvat/cvat-for-images-annotations.xml
--rw-rw-rw-   0 root         (0) root         (0)     3568 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/cvat/cvat.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.935985 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task/
--rw-rw-rw-   0 root         (0) root         (0)     3082 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task/cars
--rw-rw-rw-   0 root         (0) root         (0)     1843 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task/person
--rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task/truck
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.939985 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_class_mapping_not_found
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_forbidden_class
--rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_no_json
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_wrong_image_path
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_wrong_label_studio_format
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.939985 mlcvzoo_util-0.4.2/test_data/annotations/mot/
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/custom_labels.txt
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/mot_ground-truth_2015.txt
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/mot_ground-truth_201617.txt
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/mot_ground-truth_2020.txt
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/mot_predictions_2020.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.939985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/cars.xml
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:41:12.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/empty.xml
--rw-rw-rw-   0 root         (0) root         (0)      716 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/person.xml
--rw-rw-rw-   0 root         (0) root         (0)     1140 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/truck.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.939985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/dummy_task/
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/dummy_task/cars.xml
--rw-rw-rw-   0 root         (0) root         (0)      519 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/dummy_task/person.xml
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/dummy_task/truck.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/
--rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/cars.xml
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/empty.xml
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/person.xml
--rw-rw-rw-   0 root         (0) root         (0)     1540 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/truck.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/dummy_task/
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/dummy_task/3b09afbd59ed52a9b82a92856c0e2e82.xml
--rw-rw-rw-   0 root         (0) root         (0)     1953 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/dummy_task/636ae56768d7733bc65d1b1b543bfb4e.xml
--rw-rw-rw-   0 root         (0) root         (0)     1205 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/dummy_task/6e443ec586208278605e6829dbdf94fd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/annotations/test_inference_task/
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/test_inference_task/test_object-detection_inference_image.xml
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/text_recognition_test_label.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/checkpoints/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/checkpoints/model.pth
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/checkpoints/model_2.pth
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class1/
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class1/black_image.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class2/
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class2/black_image.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class3/
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class3/black_image.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/images/dummy_task/
--rw-rw-rw-   0 root         (0) root         (0)     3716 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/dummy_task/cars.jpg
--rw-rw-rw-   0 root         (0) root         (0)     4307 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/dummy_task/empty.jpg
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/dummy_task/person.jpg
--rw-rw-rw-   0 root         (0) root         (0)     3740 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/dummy_task/truck.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/images/test_inference_task/
--rw-rw-rw-   0 root         (0) root         (0)  2270306 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/test_inference_task/test_object-detection_inference_image.jpg
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/test_inference_task/test_text-recognition_inference_image.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/class-mapping_coco.yaml
--rw-rw-rw-   0 root         (0) root         (0)    61627 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/class-mapping_imagenet.yaml
--rw-rw-rw-   0 root         (0) root         (0)      806 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/class-mapping_test-default-lp.yaml
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/class-mapping_test-default.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/
--rw-rw-rw-   0 root         (0) root         (0)      360 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_coco_test.yaml
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_cvat_test.yaml
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_pascal-voc_test.yaml
--rw-rw-rw-   0 root         (0) root         (0)      477 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_pascal-voc_test_annotations_only.yaml
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_pascal_voc_clean.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/cvat_password.txt
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test-download-and-upload-task.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_download/
--rw-rw-rw-   0 root         (0) root         (0)     2126 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_download/mlcvzoo-test.zip
--rw-rw-rw-   0 root         (0) root         (0)      762 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_download/test-download-task.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/
--rw-rw-rw-   0 root         (0) root         (0)     2126 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/mlcvzoo-test.zip
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/test-upload-task-predictions.yaml
--rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/test-upload-task-predictions_only-create.yaml
--rw-rw-rw-   0 root         (0) root         (0)      685 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/test-upload-task.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test-checkpoint.pth
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator.yaml
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_no_factory.yaml
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_no_object_detection_model.yaml
--rw-rw-rw-   0 root         (0) root         (0)      953 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_tensorboard.yaml
--rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow.yaml
--rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow_all-checkpoint.yaml
--rw-rw-rw-   0 root         (0) root         (0)      989 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow_best-checkpoint.yaml
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow_wrong-checkpoint.yaml
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow_wrong-model.yaml
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_without_mlflow.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_model_timer/
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_timer/model_timer-read-from-file-with-mlfow-logging.yaml
--rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_timer/model_timer-read-from-file-without-mlfow-logging.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_model_trainer/
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_trainer/test_model-trainer_config_read-from-file_coco_test.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_pre_annotation_tool/
--rw-rw-rw-   0 root         (0) root         (0)     1658 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_pre_annotation_tool/test_pre_annotation_tool.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1657 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_pre_annotation_tool/test_pre_annotation_tool_with_visualization.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1656 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_pre_annotation_tool/test_pre_annotation_tool_wrong_model.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/
--rw-rw-rw-   0 root         (0) root         (0)     3212 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations.json
--rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_empty.json
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_annotations.json
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_file_upload.json
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_labels.json
--rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_result.json
--rw-rw-rw-   0 root         (0) root         (0)      428 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_sequence.json
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_task_missing.json
--rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_wrong_annotation_format.json
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_wrong_frame_count.json
--rw-rw-rw-   0 root         (0) root         (0)     3999 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video.mp4
--rw-rw-rw-   0 root         (0) root         (0)     3999 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video_2.mp4
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/test_data/test_video_image_creator/
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video_image_creator/test_video-image-creator_no-video-files.yaml
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video_image_creator/test_video-image-creator_video-dir.yaml
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video_image_creator/test_video-image-creator_video-path.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/third-party-licenses/
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/third-party-licenses/third-party-licenses-complementary.csv
--rw-rw-rw-   0 root         (0) root         (0)     5609 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/third-party-licenses/third-party-licenses.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.173535 mlcvzoo_util-0.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)     2329 2024-05-28 07:16:40.000000 mlcvzoo_util-0.4.3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11412 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-29 16:18:25.000000 mlcvzoo_util-0.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2317 2024-05-29 16:18:31.173535 mlcvzoo_util-0.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.161534 mlcvzoo_util-0.4.3/mlcvzoo_util/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-27 08:45:48.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.165535 mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7348 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8392 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9831 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/image_io_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.165535 mlcvzoo_util-0.4.3/mlcvzoo_util/logger/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/logger/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.165535 mlcvzoo_util-0.4.3/mlcvzoo_util/ls_tracking_task_converter/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/ls_tracking_task_converter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11102 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/ls_tracking_task_converter/ls_tracking_task_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4220 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/mlcvzoo_cli_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.169535 mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2024-05-27 08:45:48.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     8565 2024-05-27 08:45:48.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/metric_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    16735 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/model_evaluator.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/structs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.169535 mlcvzoo_util-0.4.3/mlcvzoo_util/model_timer/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_timer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_timer/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     9776 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_timer/model_timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.169535 mlcvzoo_util-0.4.3/mlcvzoo_util/model_trainer/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_trainer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_trainer/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6628 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/model_trainer/model_trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.173535 mlcvzoo_util-0.4.3/mlcvzoo_util/pre_annotation_tool/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/pre_annotation_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/pre_annotation_tool/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    12700 2024-05-27 08:45:48.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 16:18:25.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.173535 mlcvzoo_util-0.4.3/mlcvzoo_util/video_image_creator/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/video_image_creator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/video_image_creator/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    14451 2024-05-27 07:01:06.000000 mlcvzoo_util-0.4.3/mlcvzoo_util/video_image_creator/video_image_creator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:31.173535 mlcvzoo_util-0.4.3/mlcvzoo_util.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-29 16:18:31.000000 mlcvzoo_util-0.4.3/mlcvzoo_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4580 2024-05-27 08:45:48.000000 mlcvzoo_util-0.4.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 16:18:31.173535 mlcvzoo_util-0.4.3/setup.cfg
```

### Comparing `mlcvzoo_util-0.4.2/CHANGELOG.md` & `mlcvzoo_util-0.4.3/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # MLCVZoo mlcvzoo-utils module Versions:
 
+0.4.3 (2024-05-27):
+-------------------
+Fix typo in "include" section in pyproject.toml
+
 0.4.2 (2024-05-16):
 -------------------
 Implement uv as the python package manager
 
 0.4.1 (2024-02-07):
 -------------------
 Updated links in pyproject.toml
```

### Comparing `mlcvzoo_util-0.4.2/LICENSE` & `mlcvzoo_util-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/PKG-INFO` & `mlcvzoo_util-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo_util
-Version: 0.4.2
+Version: 0.4.3
 Summary: MLCVZoo Util Package
 Author: Maximilian Otten, email =  <maximilian.otten@iml.fraunhofer.de>, Christian Hoppe, email =  <christian.hoppe@iml.fraunhofer.de>, Oliver Bredtmann, email =  <oliver.bredtmann@dbschenker.com>, Thilo Bauer, email =  <thilo.bauer@dbschenker.com>, Oliver Urbann, email =  <oliver.urbann@iml.fraunhofer.de>, Jan Basrawi, email =  <jan.basrawi@dbschenker.com>, Luise Weickhmann, email =  <luise.weickhmann@iml.fraunhofer.de>, Luca Kotulla, email =  <luca.kotulla@iml.fraunhofer.de>
 License: Open Logistics Foundation License 1.3
 Project-URL: homepage, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util
 Project-URL: repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util
 Project-URL: documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util/-/blob/main/documentation/index.adoc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/configuration.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/utils.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/cvat_annotation_handler/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/image_io_utils.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/image_io_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/logger/logger.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/logger/logger.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/ls_tracking_task_converter/ls_tracking_task_converter.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/ls_tracking_task_converter/ls_tracking_task_converter.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/mlcvzoo_cli_tool.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/mlcvzoo_cli_tool.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/configuration.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/metric_factory.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/metric_factory.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/model_evaluator.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/structs.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/model_evaluator/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/configuration.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/model_timer/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/model_timer.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/model_timer/model_timer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/configuration.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/model_trainer/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/model_trainer.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/model_trainer/model_trainer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/configuration.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/pre_annotation_tool/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/configuration.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/video_image_creator/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/video_image_creator.py` & `mlcvzoo_util-0.4.3/mlcvzoo_util/video_image_creator/video_image_creator.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.2/pyproject.toml` & `mlcvzoo_util-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 version = {attr = "mlcvzoo_util.__version__"}
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 where = ["."]  # list of folders that contain the packages (["."] by default)
-include = ["mlcvzoo_utile*"]  # package names should match these glob patterns (["*"] by default)
+include = ["mlcvzoo_util*"]  # package names should match these glob patterns (["*"] by default)
 exclude = ["mlcvzoo_util.tests*"]  # exclude packages matching these glob patterns (empty by default)
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = [
     "setuptools>=42",
```

