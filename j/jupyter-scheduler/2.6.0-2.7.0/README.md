# Comparing `tmp/jupyter_scheduler-2.6.0.tar.gz` & `tmp/jupyter_scheduler-2.7.0.tar.gz`

## Comparing `jupyter_scheduler-2.6.0.tar` & `jupyter_scheduler-2.7.0.tar`

### file list

```diff
@@ -1,191 +1,192 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.eslintrc.js
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.prettierrc
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.readthedocs.yml
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.stylelintrc
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.yarnrc.yml
--rw-r--r--   0        0        0    47702 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/MANIFEST.in
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/babel.config.js
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/conftest.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jest.config.js
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/tsconfig.test.json
--rw-r--r--   0        0        0   429247 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/yarn.lock
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/binder/environment.yml
--rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/binder/postBuild
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/dev/seed.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/dev/templates/1.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/dev/templates/2.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/dev/templates/3.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/Makefile
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/conf.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/make.bat
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/requirements.txt
--rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/_static/jupyter_logo.png
--rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/contributors/index.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/developers/index.md
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/operators/index.md
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/index.md
--rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/actions_definition_details.png
--rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/actions_job_details.png
--rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/actions_list.png
--rw-r--r--   0        0        0   120389 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/create_job_form.png
--rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/create_job_from_filebrowser.png
--rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/create_job_from_notebook.png
--rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/custom_schedule.png
--rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/download_button.png
--rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/downloaded_files.png
--rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/headers.png
--rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/item_name.png
--rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/launcher.png
--rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/docs/users/images/run_on_schedule.png
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter-config/nb-config/jupyter_scheduler.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter-config/server-config/jupyter_scheduler.json
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/_version.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/environments.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/exceptions.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/executors.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/extension.py
--rw-r--r--   0        0        0    15516 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/handlers.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/job_files_manager.py
--rw-r--r--   0        0        0     8844 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/models.py
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/orm.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/parameterize.py
--rw-r--r--   0        0        0    34951 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/scheduler.py
--rw-r--r--   0        0        0    11623 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/task_runner.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/utils.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/package.json
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/171.d4610e21027b29e7653a.js
--rw-r--r--   0        0        0   347375 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/177.3502ccdd2c25548ad980.js
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/275.d7f03fdf77443bec5349.js
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/282.7b4e318dca2d64a434c1.js
--rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/378.34aa286b24af0577a1ce.js
--rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
--rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js.LICENSE.txt
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js.LICENSE.txt
--rw-r--r--   0        0        0    84642 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/572.7d173596605ada10b4a1.js
--rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
--rw-r--r--   0        0        0    20648 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js.LICENSE.txt
--rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/747.8e4a60162d1a81804893.js
--rw-r--r--   0        0        0    25936 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/871.5c8b68996069b5cffa43.js
--rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/remoteEntry.be10ea7cb7dfd691c1f7.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0        0        0    39580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/pydantic_v1/main.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/mocks.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_execution_manager.py
--rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_job_files_manager.py
--rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/utils.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_root_dir/job-5/import-helloworld.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_root_dir/job-5/a/b/helloworld.txt
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-4/output_side_effect.txt
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-4/side_effects.ipynb
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/schema/plugin.json
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/advanced-options.tsx
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/context.ts
--rw-r--r--   0        0        0    13264 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/handler.ts
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/hooks.ts
--rw-r--r--   0        0        0    10605 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/index.tsx
--rw-r--r--   0        0        0    13250 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/model.ts
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/notebook-jobs-panel.tsx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/size.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/svg.d.ts
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/theme-provider.ts
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/tokens.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/__tests__/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/box.tsx
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/button-bar.tsx
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/button.tsx
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/cluster.tsx
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/collapsible-panel.tsx
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/compute-type-picker.tsx
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/confirm-buttons.tsx
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/confirm-dialog-buttons.tsx
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/create-schedule-options.tsx
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/environment-picker.tsx
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/error-boundary.tsx
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/files-directory-link.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/heading.tsx
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/icon-buttons.tsx
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/icons.ts
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/input-file-snapshot.tsx
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/input-folder-checkbox.tsx
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/job-definition-row.tsx
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/job-file-link.tsx
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/job-row.tsx
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/labeled-value.tsx
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/output-format-picker.tsx
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/parameters-picker.tsx
--rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/schedule-inputs.tsx
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/stack.tsx
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/advanced-table/advanced-table-header.tsx
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/advanced-table/advanced-table.tsx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/components/advanced-table/index.tsx
--rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/mainviews/create-job-from-definition.tsx
--rw-r--r--   0        0        0    20992 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/mainviews/create-job.tsx
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/mainviews/edit-job-definition.tsx
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/mainviews/list-jobs.tsx
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/mainviews/detail-view/detail-view.tsx
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/mainviews/detail-view/index.tsx
--rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/mainviews/detail-view/job-definition.tsx
--rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/mainviews/detail-view/job-detail.tsx
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/util/errors.tsx
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/src/util/job-name-validation.tsx
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/base.css
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/box.css
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/button.css
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/cluster.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/collapsible-panel.css
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/edit-job-definitions.css
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/heading.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/index.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/labeled-value.css
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/stack.css
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/variables.css
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/icons/calendar-add-on.svg
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/icons/calendar-month.svg
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/style/icons/event-note.svg
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/.yarnrc
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/README.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/package.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   153944 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/helpers/SchedulerHelper.ts
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0    23303 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-filebrowser-linux.png
--rw-r--r--   0        0        0    23846 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-toolbar-linux.png
--rw-r--r--   0        0        0    19747 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/filebrowser-menu-linux.png
--rw-r--r--   0        0        0    26873 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    32894 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/list-view-linux.png
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/notebook-toolbar-linux.png
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/LICENSE
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/README.md
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyter_scheduler-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.eslintrc.js
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.prettierrc
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.stylelintrc
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.yarnrc.yml
+-rw-r--r--   0        0        0    48715 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/MANIFEST.in
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/babel.config.js
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/conftest.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jest.config.js
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/tsconfig.test.json
+-rw-r--r--   0        0        0   429247 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/yarn.lock
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/binder/environment.yml
+-rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/binder/postBuild
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/dev/seed.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/dev/templates/1.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/dev/templates/2.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/dev/templates/3.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/Makefile
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/conf.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/make.bat
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/requirements.txt
+-rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/_static/jupyter_logo.png
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/contributors/index.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/developers/index.md
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/operators/index.md
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/index.md
+-rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/actions_definition_details.png
+-rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/actions_job_details.png
+-rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/actions_list.png
+-rw-r--r--   0        0        0   120389 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/create_job_form.png
+-rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/create_job_from_filebrowser.png
+-rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/create_job_from_notebook.png
+-rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/custom_schedule.png
+-rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/download_button.png
+-rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/downloaded_files.png
+-rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/headers.png
+-rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/item_name.png
+-rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/launcher.png
+-rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/docs/users/images/run_on_schedule.png
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter-config/nb-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter-config/server-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/_version.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/environments.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/exceptions.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/executors.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/extension.py
+-rw-r--r--   0        0        0    15516 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/handlers.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/job_files_manager.py
+-rw-r--r--   0        0        0     8844 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/models.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/orm.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/parameterize.py
+-rw-r--r--   0        0        0    34951 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/scheduler.py
+-rw-r--r--   0        0        0    11623 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/task_runner.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/utils.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/package.json
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/171.d4610e21027b29e7653a.js
+-rw-r--r--   0        0        0   347375 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/177.3502ccdd2c25548ad980.js
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/275.d7f03fdf77443bec5349.js
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/282.7b4e318dca2d64a434c1.js
+-rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/378.34aa286b24af0577a1ce.js
+-rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
+-rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js.LICENSE.txt
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js.LICENSE.txt
+-rw-r--r--   0        0        0    84642 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/572.0790549c3c1ea44773fb.js
+-rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
+-rw-r--r--   0        0        0    20648 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js.LICENSE.txt
+-rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/747.8e4a60162d1a81804893.js
+-rw-r--r--   0        0        0    25936 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/871.5c8b68996069b5cffa43.js
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/remoteEntry.2b7950cf38f5ff22cb0a.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0        0        0    39580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/pydantic_v1/main.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/mocks.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/test_execution_manager.py
+-rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/test_job_files_manager.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/test_orm.py
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/utils.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/helloworld-1.html
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/helloworld-1.ipynb
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/helloworld.ipynb
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/helloworld.tar.gz
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/helloworld.txt
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/import-helloworld.ipynb
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/output_side_effect.txt
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/side_effects.ipynb
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/schema/plugin.json
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/advanced-options.tsx
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/context.ts
+-rw-r--r--   0        0        0    13264 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/handler.ts
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/hooks.ts
+-rw-r--r--   0        0        0    10605 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/index.tsx
+-rw-r--r--   0        0        0    13250 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/model.ts
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/notebook-jobs-panel.tsx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/size.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/svg.d.ts
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/theme-provider.ts
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/tokens.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/__tests__/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/box.tsx
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/button-bar.tsx
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/button.tsx
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/cluster.tsx
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/collapsible-panel.tsx
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/compute-type-picker.tsx
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/confirm-buttons.tsx
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/confirm-dialog-buttons.tsx
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/create-schedule-options.tsx
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/environment-picker.tsx
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/error-boundary.tsx
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/files-directory-link.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/heading.tsx
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/icon-buttons.tsx
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/icons.ts
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/input-file-snapshot.tsx
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/input-folder-checkbox.tsx
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/job-definition-row.tsx
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/job-file-link.tsx
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/job-row.tsx
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/labeled-value.tsx
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/output-format-picker.tsx
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/parameters-picker.tsx
+-rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/schedule-inputs.tsx
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/stack.tsx
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/advanced-table/advanced-table-header.tsx
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/advanced-table/advanced-table.tsx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/components/advanced-table/index.tsx
+-rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/mainviews/create-job-from-definition.tsx
+-rw-r--r--   0        0        0    20992 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/mainviews/create-job.tsx
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/mainviews/edit-job-definition.tsx
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/mainviews/list-jobs.tsx
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/mainviews/detail-view/detail-view.tsx
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/mainviews/detail-view/index.tsx
+-rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/mainviews/detail-view/job-definition.tsx
+-rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/mainviews/detail-view/job-detail.tsx
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/util/errors.tsx
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/src/util/job-name-validation.tsx
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/base.css
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/box.css
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/button.css
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/cluster.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/collapsible-panel.css
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/edit-job-definitions.css
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/heading.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/index.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/labeled-value.css
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/stack.css
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/variables.css
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/icons/calendar-add-on.svg
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/icons/calendar-month.svg
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/style/icons/event-note.svg
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/.yarnrc
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/README.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/package.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   153944 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/helpers/SchedulerHelper.ts
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0    23303 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-filebrowser-linux.png
+-rw-r--r--   0        0        0    23846 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-toolbar-linux.png
+-rw-r--r--   0        0        0    19747 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/filebrowser-menu-linux.png
+-rw-r--r--   0        0        0    26873 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    32894 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/list-view-linux.png
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/notebook-toolbar-linux.png
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/LICENSE
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/README.md
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 jupyter_scheduler-2.7.0/PKG-INFO
```

### Comparing `jupyter_scheduler-2.6.0/.eslintrc.js` & `jupyter_scheduler-2.7.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/.pre-commit-config.yaml` & `jupyter_scheduler-2.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/.stylelintrc` & `jupyter_scheduler-2.7.0/.stylelintrc`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/CHANGELOG.md` & `jupyter_scheduler-2.7.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 2.7.0
+
+([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v2.6.0...5b55901d565ad1a2894beaf1aa638dbc016bcf37))
+
+### Enhancements made
+
+- Update to SQLAlchemy 2.x [#521](https://github.com/jupyter-server/jupyter-scheduler/pull/521) ([@andrii-i](https://github.com/andrii-i))
+- Add database schema update and database migration logic [#520](https://github.com/jupyter-server/jupyter-scheduler/pull/520) ([@andrii-i](https://github.com/andrii-i))
+- Use pytest temporary folders and fixtures to create test file hierarchy at test time [#516](https://github.com/jupyter-server/jupyter-scheduler/pull/516) ([@andrii-i](https://github.com/andrii-i))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2024-04-30&to=2024-05-29&type=c))
+
+[@andrii-i](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Aandrii-i+updated%3A2024-04-30..2024-05-29&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 2.6.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v2.5.2...51a5ee4cb5681844ee4d6d2577545fb973ad7890))
 
 ### Enhancements made
 
 - Add tests for Scheduler job and job definition creation with input folder, refactor execution manager test [#513](https://github.com/jupyter-server/jupyter-scheduler/pull/513) ([@andrii-i](https://github.com/andrii-i))
@@ -21,16 +39,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2024-04-15&to=2024-04-30&type=c))
 
 [@andrii-i](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Aandrii-i+updated%3A2024-04-15..2024-04-30&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Agithub-actions+updated%3A2024-04-15..2024-04-30&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 2.5.2
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v2.5.1...b01c76088bb9acfac846727681a94c6e58493b9e))
 
 ### Bugs fixed
 
 - Changed column header to "Input file" in Notebook Job Definitions [#496](https://github.com/jupyter-server/jupyter-scheduler/pull/496) ([@srdas](https://github.com/srdas))
```

### Comparing `jupyter_scheduler-2.6.0/MANIFEST.in` & `jupyter_scheduler-2.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jest.config.js` & `jupyter_scheduler-2.7.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/package.json` & `jupyter_scheduler-2.7.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'2.7.0'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0"
+    "version": "2.7.0"
 }
```

### Comparing `jupyter_scheduler-2.6.0/tsconfig.json` & `jupyter_scheduler-2.7.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/yarn.lock` & `jupyter_scheduler-2.7.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/binder/postBuild` & `jupyter_scheduler-2.7.0/binder/postBuild`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/dev/seed.py` & `jupyter_scheduler-2.7.0/dev/seed.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/dev/templates/1.ipynb` & `jupyter_scheduler-2.7.0/dev/templates/1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/dev/templates/2.ipynb` & `jupyter_scheduler-2.7.0/dev/templates/2.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/dev/templates/3.ipynb` & `jupyter_scheduler-2.7.0/dev/templates/3.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/Makefile` & `jupyter_scheduler-2.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/conf.py` & `jupyter_scheduler-2.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/make.bat` & `jupyter_scheduler-2.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/_static/jupyter_logo.png` & `jupyter_scheduler-2.7.0/docs/_static/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/contributors/index.md` & `jupyter_scheduler-2.7.0/docs/contributors/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/developers/index.md` & `jupyter_scheduler-2.7.0/docs/developers/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/operators/index.md` & `jupyter_scheduler-2.7.0/docs/operators/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/index.md` & `jupyter_scheduler-2.7.0/docs/users/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,21 @@
 jupyter labextension list
 ```
 
 and checking that both the `jupyter_scheduler` server extension and the
 `@jupyterlab/scheduler` prebuilt lab extension are enabled.
 
 :::{attention}
+:name: sqlalchemy-2.x-requirement
+Starting with v2.7.0, Jupyter Scheduler requires SQLAlchemy 2.x instead of SQLAlchemy 1.x.
+:::
+
+:::{attention}
 :name: jupyter-lab-3-end-of-maintenance
-JupyterLab 3 will reach its end of maintenance date on May 15, 2024, anywhere on Earth. As a result, we will not backport new features to the v1 branch supporting JupyterLab 3 after this date. Fixes for critical issues will still be backported until December 31, 2024. If you are still using JupyterLab 3, we strongly encourage you to **upgrade to JupyterLab 4 as soon as possible**. For more information, see [JupyterLab 3 end of maintenance](https://blog.jupyter.org/jupyterlab-3-end-of-maintenance-879778927db2) on the Jupyter Blog.
+JupyterLab 3 reached its end of maintenance date on May 15, 2024. As a result, we will not backport new features to the v1 branch supporting JupyterLab 3 after this date. Fixes for critical issues will still be backported until December 31, 2024. If you are still using JupyterLab 3, we strongly encourage you to **upgrade to JupyterLab 4 as soon as possible**. For more information, see [JupyterLab 3 end of maintenance](https://blog.jupyter.org/jupyterlab-3-end-of-maintenance-879778927db2) on the Jupyter Blog.
 :::
 
 ## Use
 
 Jupyter Scheduler runs Jupyter notebooks in the background, either once or on a schedule. You can create _jobs_ (single run of an individual notebook) and _job definitions_ (scheduled recurring notebook jobs). When the scheduler runs your notebook, it makes a copy of the input file. The scheduler uses unique names for the input and output files so that rerunning the same notebook produces new files every time.
 
 ### Creating a job or job definition
```

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/actions_definition_details.png` & `jupyter_scheduler-2.7.0/docs/users/images/actions_definition_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/actions_job_details.png` & `jupyter_scheduler-2.7.0/docs/users/images/actions_job_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/actions_list.png` & `jupyter_scheduler-2.7.0/docs/users/images/actions_list.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/create_job_form.png` & `jupyter_scheduler-2.7.0/docs/users/images/create_job_form.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/create_job_from_filebrowser.png` & `jupyter_scheduler-2.7.0/docs/users/images/create_job_from_filebrowser.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/create_job_from_notebook.png` & `jupyter_scheduler-2.7.0/docs/users/images/create_job_from_notebook.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/custom_schedule.png` & `jupyter_scheduler-2.7.0/docs/users/images/custom_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/download_button.png` & `jupyter_scheduler-2.7.0/docs/users/images/download_button.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/downloaded_files.png` & `jupyter_scheduler-2.7.0/docs/users/images/downloaded_files.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/headers.png` & `jupyter_scheduler-2.7.0/docs/users/images/headers.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/item_name.png` & `jupyter_scheduler-2.7.0/docs/users/images/item_name.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/launcher.png` & `jupyter_scheduler-2.7.0/docs/users/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/docs/users/images/run_on_schedule.png` & `jupyter_scheduler-2.7.0/docs/users/images/run_on_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/environments.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/exceptions.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/executors.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/executors.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/extension.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/handlers.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/job_files_manager.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/models.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/orm.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/orm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
-import os
 from sqlite3 import OperationalError
 from uuid import uuid4
 
 import sqlalchemy.types as types
-from sqlalchemy import Boolean, Column, Integer, String, create_engine
+from sqlalchemy import Boolean, Column, Integer, String, create_engine, inspect
 from sqlalchemy.orm import declarative_base, declarative_mixin, registry, sessionmaker
+from sqlalchemy.sql import text
 
 from jupyter_scheduler.models import EmailNotifications, Status
 from jupyter_scheduler.utils import get_utc_timestamp
 
 Base = declarative_base()
 
 
@@ -81,43 +81,79 @@
     timeout_seconds = Column(Integer, default=600)
     retry_on_timeout = Column(Boolean, default=False)
     max_retries = Column(Integer, default=0)
     min_retry_interval_millis = Column(Integer, default=0)
     output_filename_template = Column(String(256))
     update_time = Column(Integer, default=get_utc_timestamp, onupdate=get_utc_timestamp)
     create_time = Column(Integer, default=get_utc_timestamp)
+    # All new columns added to this table must be nullable to ensure compatibility during database migrations.
+    # Any default values specified for new columns will be ignored during the migration process.
     package_input_folder = Column(Boolean)
     packaged_files = Column(JsonType, default=[])
 
 
 class Job(CommonColumns, Base):
     __tablename__ = "jobs"
+    __table_args__ = {"extend_existing": True}
     job_id = Column(String(36), primary_key=True, default=generate_uuid)
     job_definition_id = Column(String(36))
     status = Column(String(64), default=Status.STOPPED)
     status_message = Column(String(1024))
     start_time = Column(Integer)
     end_time = Column(Integer)
     url = Column(String(256), default=generate_jobs_url)
     pid = Column(Integer)
     idempotency_token = Column(String(256))
+    # All new columns added to this table must be nullable to ensure compatibility during database migrations.
+    # Any default values specified for new columns will be ignored during the migration process.
 
 
 class JobDefinition(CommonColumns, Base):
     __tablename__ = "job_definitions"
+    __table_args__ = {"extend_existing": True}
     job_definition_id = Column(String(36), primary_key=True, default=generate_uuid)
     schedule = Column(String(256))
     timezone = Column(String(36))
     url = Column(String(256), default=generate_job_definitions_url)
     create_time = Column(Integer, default=get_utc_timestamp)
     active = Column(Boolean, default=True)
+    # All new columns added to this table must be nullable to ensure compatibility during database migrations.
+    # Any default values specified for new columns will be ignored during the migration process.
 
 
-def create_tables(db_url, drop_tables=False):
+def update_db_schema(engine, Base):
+    inspector = inspect(engine)
+    alter_statements = []
+
+    for table_name, model in Base.metadata.tables.items():
+        if not inspector.has_table(table_name):
+            continue
+        columns_db = inspector.get_columns(table_name)
+        columns_db_names = {col["name"] for col in columns_db}
+
+        for column_model_name, column_model in model.c.items():
+            if column_model_name in columns_db_names:
+                continue
+            column_type = str(column_model.type.compile(dialect=engine.dialect))
+            alter_statement = text(
+                f"ALTER TABLE {table_name} ADD COLUMN {column_model_name} {column_type} NULL"
+            )
+            alter_statements.append(alter_statement)
+
+    if not alter_statements:
+        return
+    with engine.connect() as connection:
+        for alter_statement in alter_statements:
+            connection.execute(alter_statement)
+
+
+def create_tables(db_url, drop_tables=False, Base=Base):
     engine = create_engine(db_url)
+    update_db_schema(engine, Base)
+
     try:
         if drop_tables:
             Base.metadata.drop_all(engine)
     except OperationalError:
         pass
     finally:
         Base.metadata.create_all(engine)
```

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/parameterize.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/parameterize.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/scheduler.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/task_runner.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/task_runner.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/utils.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/package.json` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2b7950cf38f5ff22cb0a.js'}}",*

 * * "'version'": "'2.7.0'"}*

```diff
@@ -71,15 +71,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.be10ea7cb7dfd691c1f7.js",
+            "load": "static/remoteEntry.2b7950cf38f5ff22cb0a.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_scheduler"
                 },
@@ -141,9 +141,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0"
+    "version": "2.7.0"
 }
```

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'2.7.0'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0"
+    "version": "2.7.0"
 }
```

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/171.d4610e21027b29e7653a.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/171.d4610e21027b29e7653a.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/177.3502ccdd2c25548ad980.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/177.3502ccdd2c25548ad980.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/275.d7f03fdf77443bec5349.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/275.d7f03fdf77443bec5349.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/282.7b4e318dca2d64a434c1.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/282.7b4e318dca2d64a434c1.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/378.34aa286b24af0577a1ce.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/378.34aa286b24af0577a1ce.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/572.7d173596605ada10b4a1.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/572.0790549c3c1ea44773fb.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,32 +5,32 @@
             n.r(t), n.d(t, {
                 CommandIDs: () => _t,
                 JobsView: () => E,
                 NotebookJobsPanelId: () => gt,
                 Scheduler: () => vt,
                 default: () => Et
             });
-            var o = n(2677),
-                a = n(7756),
-                l = n(5018),
-                r = n(8428),
-                i = n(9184),
-                s = n(7520),
-                c = n(7560),
+            var o = n(3039),
+                a = n(8690),
+                l = n(3779),
+                r = n(8140),
+                i = n(9282),
+                s = n(4481),
+                c = n(9954),
                 d = n(6029),
                 u = n.n(d),
                 m = n(296);
 
             function p(e) {
                 let t = "jp-jobs-Cluster";
                 return t += ` justify-content-${e.justifyContent||"flex-start"}`, t += ` align-items-${e.alignItems||"center"}`, t += ` gap-${e.gap||1}`, u().createElement("div", {
                     className: t
                 }, e.children)
             }
-            var h = n(1731);
+            var h = n(3764);
             const b = {
                 lineHeight: 0
             };
 
             function v(e) {
                 return u().createElement(m.IconButton, {
                     "aria-label": "delete",
@@ -292,15 +292,15 @@
                     name: "jupyterlab-scheduler:calendar-month",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 18" height="16px" width="16px">\n  <path fill="#0097A7" d="M10 12q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q10.312 12 10 12Zm-3.25 0q-.312 0-.531-.219Q6 11.562 6 11.25q0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q7.062 12 6.75 12Zm6.5 0q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531-.219.219-.531.219ZM10 15q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q10.312 15 10 15Zm-3.25 0q-.312 0-.531-.219Q6 14.562 6 14.25q0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q7.062 15 6.75 15Zm6.5 0q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531-.219.219-.531.219ZM4.5 18q-.625 0-1.062-.448Q3 17.104 3 16.5v-11q0-.604.438-1.052Q3.875 4 4.5 4H6V2h1.5v2h5V2H14v2h1.5q.625 0 1.062.448Q17 4.896 17 5.5v11q0 .604-.438 1.052Q16.125 18 15.5 18Zm0-1.5h11V9h-11v7.5Z"/>\n</svg>\n'
                 }),
                 I = new h.LabIcon({
                     name: "jupyterlab-scheduler:event-note",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 48 48" height="48" width="48">\n  <path fill="#0097A7" d="M14 27v-3h20v3Zm0 9v-3h13.95v3Zm-5 8q-1.2 0-2.1-.9Q6 42.2 6 41V10q0-1.2.9-2.1Q7.8 7 9 7h3.25V4h3.25v3h17V4h3.25v3H39q1.2 0 2.1.9.9.9.9 2.1v31q0 1.2-.9 2.1-.9.9-2.1.9Zm0-3h30V19.5H9V41Z"/>\n</svg>\n'
                 });
-            var T, O = n(1363);
+            var T, O = n(4705);
             class P {
                 constructor(e) {
                     this.serverSettings = e.serverSettings || s.ServerConnection.makeSettings()
                 }
                 serializeToQueryString(e) {
                     return "?" + Object.keys(e).map((t => {
                         if ("sort_by" === t) {
```

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/747.8e4a60162d1a81804893.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/747.8e4a60162d1a81804893.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/871.5c8b68996069b5cffa43.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/871.5c8b68996069b5cffa43.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/remoteEntry.be10ea7cb7dfd691c1f7.js` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/remoteEntry.2b7950cf38f5ff22cb0a.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, l, i, u, d, c, f, s, p, h, b, m, v, y, g, j, w = {
+    var e, r, t, a, n, o, l, i, d, u, c, f, s, p, b, h, m, v, y, g, j, w = {
             947: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(687), t.e(470), t.e(29), t.e(222), t.e(899), t.e(572)]).then((() => () => t(9572))),
                         "./extension": () => Promise.all([t.e(687), t.e(470), t.e(29), t.e(222), t.e(899), t.e(572)]).then((() => () => t(9572))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -55,15 +55,15 @@
         222: "1321ce1c143fee47b94a",
         275: "d7f03fdf77443bec5349",
         282: "7b4e318dca2d64a434c1",
         378: "34aa286b24af0577a1ce",
         458: "d59c5307102faf5c19a8",
         470: "da7e4fe7177a2696e6be",
         506: "7bbbaea2be6a025277aa",
-        572: "7d173596605ada10b4a1",
+        572: "0790549c3c1ea44773fb",
         613: "17512dda5aad1f2a390f",
         687: "e4421b30aab66f8929fd",
         747: "8e4a60162d1a81804893",
         799: "9152e8d30dd44c1e40a4",
         871: "5c8b68996069b5cffa43",
         899: "9bd742e2a50cf7cc1631"
     } [e] + ".js?v=" + {
@@ -75,15 +75,15 @@
         222: "1321ce1c143fee47b94a",
         275: "d7f03fdf77443bec5349",
         282: "7b4e318dca2d64a434c1",
         378: "34aa286b24af0577a1ce",
         458: "d59c5307102faf5c19a8",
         470: "da7e4fe7177a2696e6be",
         506: "7bbbaea2be6a025277aa",
-        572: "7d173596605ada10b4a1",
+        572: "0790549c3c1ea44773fb",
         613: "17512dda5aad1f2a390f",
         687: "e4421b30aab66f8929fd",
         747: "8e4a60162d1a81804893",
         799: "9152e8d30dd44c1e40a4",
         871: "5c8b68996069b5cffa43",
         899: "9bd742e2a50cf7cc1631"
     } [e], S.g = function() {
@@ -94,16 +94,16 @@
             if ("object" == typeof window) return window
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/scheduler:", S.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var l, i;
             if (void 0 !== n)
-                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var c = u[d];
+                for (var d = document.getElementsByTagName("script"), u = 0; u < d.length; u++) {
+                    var c = d[u];
                     if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + n) {
                         l = c;
                         break
                     }
                 }
             l || (i = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, S.nc && l.setAttribute("nonce", S.nc), l.setAttribute("data-webpack", r + n), l.src = t), e[t] = [a];
             var f = (r, a) => {
@@ -140,16 +140,16 @@
                             i = n[r];
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
-                    u = [];
-                return "default" === t && (i("@emotion/react", "11.10.4", (() => Promise.all([S.e(275), S.e(506), S.e(29), S.e(171)]).then((() => () => S(5506))))), i("@emotion/styled", "11.10.4", (() => Promise.all([S.e(378), S.e(29), S.e(211), S.e(799), S.e(122)]).then((() => () => S(4378))))), i("@jupyterlab/scheduler", "2.6.0", (() => Promise.all([S.e(687), S.e(470), S.e(29), S.e(222), S.e(899), S.e(572)]).then((() => () => S(9572))))), i("@mui/material", "5.10.6", (() => Promise.all([S.e(687), S.e(177), S.e(470), S.e(29), S.e(222), S.e(899)]).then((() => () => S(4177))))), i("@mui/system", "5.10.6", (() => Promise.all([S.e(275), S.e(687), S.e(871), S.e(29), S.e(211), S.e(222)]).then((() => () => S(1871))))), i("cronstrue", "2.12.0", (() => S.e(458).then((() => () => S(2458))))), i("tzdata", "1.0.33", (() => S.e(613).then((() => () => S(8613)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    d = [];
+                return "default" === t && (i("@emotion/react", "11.10.4", (() => Promise.all([S.e(275), S.e(506), S.e(29), S.e(171)]).then((() => () => S(5506))))), i("@emotion/styled", "11.10.4", (() => Promise.all([S.e(378), S.e(29), S.e(211), S.e(799), S.e(122)]).then((() => () => S(4378))))), i("@jupyterlab/scheduler", "2.7.0", (() => Promise.all([S.e(687), S.e(470), S.e(29), S.e(222), S.e(899), S.e(572)]).then((() => () => S(9572))))), i("@mui/material", "5.10.6", (() => Promise.all([S.e(687), S.e(177), S.e(470), S.e(29), S.e(222), S.e(899)]).then((() => () => S(4177))))), i("@mui/system", "5.10.6", (() => Promise.all([S.e(275), S.e(687), S.e(871), S.e(29), S.e(211), S.e(222)]).then((() => () => S(1871))))), i("cronstrue", "2.12.0", (() => S.e(458).then((() => () => S(2458))))), i("tzdata", "1.0.33", (() => S.e(613).then((() => () => S(8613)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,107 +185,107 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(i = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, i);
             return t
         }
         var l = [];
         for (o = 1; o < e.length; o++) {
             var i = e[o];
-            l.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? l.pop() + " " + l.pop() : n(i))
+            l.push(0 === i ? "not(" + d() + ")" : 1 === i ? "(" + d() + " || " + d() + ")" : 2 === i ? l.pop() + " " + l.pop() : n(i))
         }
-        return u();
+        return d();
 
-        function u() {
+        function d() {
             return l.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
-            for (var l = 0, i = 1, u = !0;; i++, l++) {
-                var d, c, f = i < e.length ? (typeof e[i])[0] : "";
-                if (l >= r.length || "o" == (c = (typeof(d = r[l]))[0])) return !u || ("u" == f ? i > a && !n : "" == f != n);
+            for (var l = 0, i = 1, d = !0;; i++, l++) {
+                var u, c, f = i < e.length ? (typeof e[i])[0] : "";
+                if (l >= r.length || "o" == (c = (typeof(u = r[l]))[0])) return !d || ("u" == f ? i > a && !n : "" == f != n);
                 if ("u" == c) {
-                    if (!u || "u" != f) return !1
-                } else if (u)
+                    if (!d || "u" != f) return !1
+                } else if (d)
                     if (f == c)
                         if (i <= a) {
-                            if (d != e[i]) return !1
+                            if (u != e[i]) return !1
                         } else {
-                            if (n ? d > e[i] : d < e[i]) return !1;
-                            d != e[i] && (u = !1)
+                            if (n ? u > e[i] : u < e[i]) return !1;
+                            u != e[i] && (d = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (n || i <= a) return !1;
-                    u = !1, i--
+                    d = !1, i--
                 } else {
                     if (i <= a || c < f != n) return !1;
-                    u = !1
-                } else "s" != f && "n" != f && (u = !1, i--)
+                    d = !1
+                } else "s" != f && "n" != f && (d = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (l = 1; l < e.length; l++) {
-            var h = e[l];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            var b = e[l];
+            s.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? o(b, r) : !p())
         }
         return !!p()
     }, l = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, i = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
-    }, u = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", c = (e, r, t, a) => {
-        var n = u(e, t);
-        return o(a, n) || s(d(e, t, n, a)), p(e[t][n])
+    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", c = (e, r, t, a) => {
+        var n = d(e, t);
+        return o(a, n) || s(u(e, t, n, a)), p(e[t][n])
     }, f = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), b = (h = e => function(r, t, a, n) {
+    }, p = e => (e.loaded = 1, e.get()), h = (b = e => function(r, t, a, n) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
-    })(((e, r, t, a) => r && S.o(r, t) ? p(i(r, t)) : a())), m = h(((e, r, t, a) => (l(e, t), c(r, 0, t, a)))), v = h(((e, r, t, a, n) => {
+    })(((e, r, t, a) => r && S.o(r, t) ? p(i(r, t)) : a())), m = b(((e, r, t, a) => (l(e, t), c(r, 0, t, a)))), v = b(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && f(r, t, a);
         return o ? p(o) : n()
     })), y = {}, g = {
         6029: () => m("default", "react", [1, 18, 2, 0]),
         2148: () => v("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([S.e(275), S.e(506), S.e(282)]).then((() => () => S(5506))))),
         8800: () => v("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([S.e(378), S.e(211), S.e(799)]).then((() => () => S(4378))))),
         7313: () => v("default", "@mui/system", [1, 5, 10, 6], (() => Promise.all([S.e(275), S.e(871), S.e(211)]).then((() => () => S(1871))))),
         7704: () => m("default", "react-dom", [1, 18, 2, 0]),
         296: () => v("default", "@mui/material", [1, 5, 10, 6], (() => S.e(177).then((() => () => S(4177))))),
         763: () => v("default", "tzdata", [1, 1, 0, 33], (() => S.e(613).then((() => () => S(8613))))),
-        1363: () => m("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
-        1731: () => m("default", "@jupyterlab/ui-components", [1, 4, 1, 8]),
         2344: () => v("default", "cronstrue", [1, 2, 12, 0], (() => S.e(458).then((() => () => S(2458))))),
-        2677: () => m("default", "@jupyterlab/application", [1, 4, 1, 8]),
+        3039: () => m("default", "@jupyterlab/application", [1, 4, 2, 1]),
+        3764: () => m("default", "@jupyterlab/ui-components", [1, 4, 2, 1]),
+        3779: () => m("default", "@jupyterlab/filebrowser", [1, 4, 2, 1]),
+        4481: () => m("default", "@jupyterlab/services", [1, 7, 2, 1]),
+        4705: () => m("default", "@jupyterlab/coreutils", [1, 6, 2, 1]),
         4901: () => m("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5018: () => m("default", "@jupyterlab/filebrowser", [1, 4, 1, 8]),
-        7520: () => m("default", "@jupyterlab/services", [1, 7, 1, 8]),
-        7560: () => m("default", "@jupyterlab/translation", [1, 4, 1, 8]),
-        7756: () => m("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
         7930: () => m("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        8428: () => m("default", "@jupyterlab/launcher", [1, 4, 1, 8]),
-        9184: () => m("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
-        5211: () => b("default", "@emotion/react", (() => Promise.all([S.e(275), S.e(506), S.e(282)]).then((() => () => S(5506))))),
+        8140: () => m("default", "@jupyterlab/launcher", [1, 4, 2, 1]),
+        8690: () => m("default", "@jupyterlab/apputils", [1, 4, 3, 1]),
+        9282: () => m("default", "@jupyterlab/notebook", [1, 4, 2, 1]),
+        9954: () => m("default", "@jupyterlab/translation", [1, 4, 2, 1]),
+        5211: () => h("default", "@emotion/react", (() => Promise.all([S.e(275), S.e(506), S.e(282)]).then((() => () => S(5506))))),
         799: () => v("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([S.e(275), S.e(506)]).then((() => () => S(5506)))))
     }, j = {
         29: [6029],
         211: [5211],
         222: [2148, 8800],
-        572: [296, 763, 1363, 1731, 2344, 2677, 4901, 5018, 7520, 7560, 7756, 7930, 8428, 9184],
+        572: [296, 763, 2344, 3039, 3764, 3779, 4481, 4705, 4901, 7930, 8140, 8690, 9282, 9954],
         799: [799],
         899: [7313, 7704]
     }, S.f.consumes = (e, r) => {
         S.o(j, e) && j[e].forEach((e => {
             if (S.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, S.m[e] = t => {
@@ -325,20 +325,20 @@
                         l.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", l.name = "ChunkLoadError", l.type = n, l.request = o, a[1](l)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
                 var a, n, [o, l, i] = t,
-                    u = 0;
+                    d = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (a in l) S.o(l, a) && (S.m[a] = l[a]);
                     i && i(S)
                 }
-                for (r && r(t); u < o.length; u++) n = o[u], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_jupyterlab_scheduler = self.webpackChunk_jupyterlab_scheduler || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
     var E = S(947);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab/scheduler"] = E
 })();
```

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/labextension/static/third-party-licenses.json` & `jupyter_scheduler-2.7.0/jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/mocks.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_handlers.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_job_files_manager.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/test_job_files_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,73 +56,96 @@
                     staging_paths=staging_paths,
                     output_dir=output_dir,
                     redownload=False,
                     include_staging_files=None,
                 )
 
 
-HERE = Path(__file__).parent.resolve()
-OUTPUTS_DIR = os.path.join(HERE, "test_files_output")
+@pytest.fixture
+def staging_dir_with_notebook_job(static_test_files_dir, jp_scheduler_staging_dir):
+    staging_dir = jp_scheduler_staging_dir / "job-1"
+    job_filenames = ["helloworld-1.ipynb", "helloworld-1.html", "helloworld.ipynb"]
+
+    staged_job_files = []
+    staging_dir.mkdir()
+    for job_filename in job_filenames:
+        staged_job_file = shutil.copy2(static_test_files_dir / job_filename, staging_dir)
+        staged_job_files.append(staged_job_file)
+
+    return staged_job_files
 
 
 @pytest.fixture
-def clear_outputs_dir():
-    yield
-    shutil.rmtree(OUTPUTS_DIR)
-    # rmtree() is not synchronous; wait until it has finished running
-    while os.path.isdir(OUTPUTS_DIR):
-        time.sleep(0.01)
+def staging_dir_with_tar_job(static_test_files_dir, jp_scheduler_staging_dir):
+    staging_dir = jp_scheduler_staging_dir / "job-2"
+    job_tar_file = static_test_files_dir / "helloworld.tar.gz"
+
+    staging_dir.mkdir()
+    staged_tar_file = shutil.copy2(job_tar_file, staging_dir)
 
+    return staged_tar_file
 
-@pytest.mark.parametrize(
-    "output_formats, output_filenames, staging_paths, output_dir, redownload",
-    [
-        (
-            ["ipynb", "html"],
-            {
+
+@pytest.fixture
+def downloader_parameters(
+    staging_dir_with_notebook_job,
+    staging_dir_with_tar_job,
+    request,
+    jp_scheduler_output_dir,
+):
+    job_1_ipynb_file_path, job_1_html_file_path, job_1_input_file_path = (
+        staging_dir_with_notebook_job
+    )
+    job_2_tar_file_path = staging_dir_with_tar_job
+    index = request.param
+    parameters = [
+        {
+            "output_formats": ["ipynb", "html"],
+            "output_filenames": {
                 "ipynb": "job-1/helloworld-out.ipynb",
                 "html": "job-1/helloworld-out.html",
                 "input": "job-1/helloworld-input.ipynb",
             },
-            {
-                "ipynb": os.path.join(HERE, "test_staging_dir", "job-1", "helloworld-1.ipynb"),
-                "html": os.path.join(HERE, "test_staging_dir", "job-1", "helloworld-1.html"),
-                "input": os.path.join(HERE, "test_staging_dir", "job-1", "helloworld.ipynb"),
+            "staging_paths": {
+                "ipynb": job_1_ipynb_file_path,
+                "html": job_1_html_file_path,
+                "input": job_1_input_file_path,
             },
-            OUTPUTS_DIR,
-            False,
-        ),
-        (
-            ["ipynb", "html"],
-            {
+            "output_dir": jp_scheduler_output_dir,
+            "redownload": False,
+        },
+        {
+            "output_formats": ["ipynb", "html"],
+            "output_filenames": {
                 "ipynb": "job-2/helloworld-1.ipynb",
                 "html": "job-2/helloworld-1.html",
                 "input": "job-2/helloworld.ipynb",
             },
-            {
-                "tar.gz": os.path.join(HERE, "test_staging_dir", "job-2", "helloworld.tar.gz"),
+            "staging_paths": {
+                "tar.gz": job_2_tar_file_path,
                 "ipynb": "job-2/helloworld-1.ipynb",
                 "html": "job-2/helloworld-1.html",
                 "input": "job-2/helloworld.ipynb",
             },
-            OUTPUTS_DIR,
-            False,
-        ),
-    ],
-)
-def test_downloader_download(
-    clear_outputs_dir, output_formats, output_filenames, staging_paths, output_dir, redownload
-):
-    downloader = Downloader(
-        output_formats=output_formats,
-        output_filenames=output_filenames,
-        staging_paths=staging_paths,
-        output_dir=output_dir,
-        redownload=redownload,
+            "output_dir": jp_scheduler_output_dir,
+            "redownload": False,
+        },
+    ]
+    return parameters[index]
+
+
+@pytest.mark.parametrize("downloader_parameters", [0, 1], indirect=True)
+def test_downloader_download(downloader_parameters):
+    output_formats, output_filenames, staging_paths, output_dir = (
+        downloader_parameters["output_formats"],
+        downloader_parameters["output_filenames"],
+        downloader_parameters["staging_paths"],
+        downloader_parameters["output_dir"],
     )
+    downloader = Downloader(**downloader_parameters)
     downloader.download()
 
     assert os.path.exists(output_dir)
     for format in output_formats:
         # get path to output file corresponding to this format
         out_filepath = os.path.join(output_dir, output_filenames[format])
```

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_scheduler.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/test_scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Tests for scheduler"""
 
+import shutil
+from pathlib import Path
 from unittest import mock
 from unittest.mock import patch
 
 import pytest
 
 from jupyter_scheduler.models import (
     CreateJob,
@@ -12,14 +14,28 @@
     SortDirection,
     SortField,
     UpdateJobDefinition,
 )
 from jupyter_scheduler.orm import Job, JobDefinition
 
 
+@pytest.fixture
+def root_dir_with_input_folder(static_test_files_dir, jp_scheduler_root_dir):
+    notebook_file_path = static_test_files_dir / "import-helloworld.ipynb"
+    dependency_file_path = static_test_files_dir / "helloworld.txt"
+    job_root_dir = jp_scheduler_root_dir / "job-5"
+    dependency_root_dir = job_root_dir / "a" / "b"
+
+    dependency_root_dir.mkdir(parents=True)
+    shutil.copy2(notebook_file_path, job_root_dir)
+    shutil.copy2(dependency_file_path, dependency_root_dir)
+
+    return Path(job_root_dir.name) / notebook_file_path.name
+
+
 def test_create_job_definition(jp_scheduler):
     with patch("jupyter_scheduler.scheduler.fsspec") as mock_fsspec:
         with patch("jupyter_scheduler.scheduler.Scheduler.file_exists") as mock_file_exists:
             mock_file_exists.return_value = True
             job_definition_id = jp_scheduler.create_job_definition(
                 CreateJobDefinition(
                     input_uri="helloworld.ipynb",
@@ -36,18 +52,18 @@
         assert job_definition_id
         assert job_definition_id == definition.job_definition_id
         assert "helloworld.ipynb" == definition.input_filename
         assert "default" == definition.runtime_environment_name
         assert "hello world" == definition.name
 
 
-def test_create_job_definition_with_input_folder(jp_scheduler):
+def test_create_job_definition_with_input_folder(jp_scheduler, root_dir_with_input_folder):
     job_definition_id = jp_scheduler.create_job_definition(
         CreateJobDefinition(
-            input_uri="job-5/import-helloworld.ipynb",
+            input_uri=str(root_dir_with_input_folder),
             runtime_environment_name="default",
             name="import hello world",
             output_formats=["ipynb"],
             package_input_folder=True,
         )
     )
 
@@ -57,18 +73,18 @@
         definition = definitions[0]
         assert job_definition_id
         assert job_definition_id == definition.job_definition_id
         assert "import hello world" == definition.name
         assert "a/b/helloworld.txt" in definition.packaged_files
 
 
-def test_create_job_with_input_folder(jp_scheduler):
+def test_create_job_with_input_folder(jp_scheduler, root_dir_with_input_folder):
     job_id = jp_scheduler.create_job(
         CreateJob(
-            input_uri="job-5/import-helloworld.ipynb",
+            input_uri=str(root_dir_with_input_folder),
             runtime_environment_name="default",
             name="import hello world",
             output_formats=["ipynb"],
             package_input_folder=True,
         )
     )
 
@@ -123,19 +139,18 @@
     "tags": ["tag_3"],
     "packaged_files": [],
 }
 
 
 @pytest.fixture
 def load_job_definitions(jp_scheduler_db):
-    with jp_scheduler_db() as session:
-        session.add(JobDefinition(**job_definition_1))
-        session.add(JobDefinition(**job_definition_2))
-        session.add(JobDefinition(**job_definition_3))
-        session.commit()
+    jp_scheduler_db.add(JobDefinition(**job_definition_1))
+    jp_scheduler_db.add(JobDefinition(**job_definition_2))
+    jp_scheduler_db.add(JobDefinition(**job_definition_3))
+    jp_scheduler_db.commit()
 
 
 @pytest.mark.parametrize(
     "list_query,expected_response",
     [
         (
             {
@@ -178,54 +193,50 @@
 
 
 def test_pause_jobs(jp_scheduler, load_job_definitions, jp_scheduler_db):
     job_definition_id = job_definition_2["job_definition_id"]
     with patch("jupyter_scheduler.scheduler.Scheduler.task_runner") as mock_task_runner:
         jp_scheduler.update_job_definition(job_definition_id, UpdateJobDefinition(active=False))
 
-    with jp_scheduler_db() as session:
-        active = (
-            session.query(JobDefinition.active)
-            .filter(JobDefinition.job_definition_id == job_definition_id)
-            .one()
-            .active
-        )
-        assert not active
+    active = (
+        jp_scheduler_db.query(JobDefinition.active)
+        .filter(JobDefinition.job_definition_id == job_definition_id)
+        .one()
+        .active
+    )
+    assert not active
 
 
 def test_resume_jobs(jp_scheduler, load_job_definitions, jp_scheduler_db):
     job_definition_id = job_definition_3["job_definition_id"]
     with patch("jupyter_scheduler.scheduler.Scheduler.task_runner") as mock_task_runner:
         jp_scheduler.update_job_definition(job_definition_id, UpdateJobDefinition(active=True))
 
-    with jp_scheduler_db() as session:
-        active = (
-            session.query(JobDefinition.active)
-            .filter(JobDefinition.job_definition_id == job_definition_id)
-            .one()
-            .active
-        )
-        assert active
+    active = (
+        jp_scheduler_db.query(JobDefinition.active)
+        .filter(JobDefinition.job_definition_id == job_definition_id)
+        .one()
+        .active
+    )
+    assert active
 
 
 def test_update_job_definition(jp_scheduler, load_job_definitions, jp_scheduler_db):
     job_definition_id = job_definition_1["job_definition_id"]
     schedule = "*/5 * * * *"
     timezone = "America/New_York"
     with patch("jupyter_scheduler.scheduler.Scheduler.task_runner") as mock_task_runner:
         update = UpdateJobDefinition(
             job_definition_id=job_definition_id, schedule=schedule, timezone=timezone
         )
         jp_scheduler.update_job_definition(job_definition_id, update)
 
-    with jp_scheduler_db() as session:
-        definition = session.get(JobDefinition, job_definition_id)
-        assert schedule == definition.schedule
-        assert timezone == definition.timezone
+    definition = jp_scheduler_db.get(JobDefinition, job_definition_id)
+    assert schedule == definition.schedule
+    assert timezone == definition.timezone
 
 
 def test_delete_job_definition(jp_scheduler, load_job_definitions, jp_scheduler_db):
     job_definition_id = job_definition_1["job_definition_id"]
     jp_scheduler.delete_job_definition(job_definition_id)
-    with jp_scheduler_db() as session:
-        definition = session.get(JobDefinition, job_definition_id)
-        assert not definition
+    definition = jp_scheduler_db.get(JobDefinition, job_definition_id)
+    assert not definition
```

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/utils.py` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_root_dir/job-5/import-helloworld.ipynb` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/import-helloworld.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/helloworld-1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/helloworld.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/helloworld.tar.gz`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/jupyter_scheduler/tests/test_staging_dir/job-4/side_effects.ipynb` & `jupyter_scheduler-2.7.0/jupyter_scheduler/tests/static/side_effects.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/schema/plugin.json` & `jupyter_scheduler-2.7.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/advanced-options.tsx` & `jupyter_scheduler-2.7.0/src/advanced-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/handler.ts` & `jupyter_scheduler-2.7.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/index.tsx` & `jupyter_scheduler-2.7.0/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/model.ts` & `jupyter_scheduler-2.7.0/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/notebook-jobs-panel.tsx` & `jupyter_scheduler-2.7.0/src/notebook-jobs-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/theme-provider.ts` & `jupyter_scheduler-2.7.0/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/tokens.ts` & `jupyter_scheduler-2.7.0/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/cluster.tsx` & `jupyter_scheduler-2.7.0/src/components/cluster.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/collapsible-panel.tsx` & `jupyter_scheduler-2.7.0/src/components/collapsible-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/compute-type-picker.tsx` & `jupyter_scheduler-2.7.0/src/components/compute-type-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/confirm-buttons.tsx` & `jupyter_scheduler-2.7.0/src/components/confirm-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/confirm-dialog-buttons.tsx` & `jupyter_scheduler-2.7.0/src/components/confirm-dialog-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/create-schedule-options.tsx` & `jupyter_scheduler-2.7.0/src/components/create-schedule-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/environment-picker.tsx` & `jupyter_scheduler-2.7.0/src/components/environment-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/error-boundary.tsx` & `jupyter_scheduler-2.7.0/src/components/error-boundary.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/files-directory-link.tsx` & `jupyter_scheduler-2.7.0/src/components/files-directory-link.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/heading.tsx` & `jupyter_scheduler-2.7.0/src/components/heading.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/icon-buttons.tsx` & `jupyter_scheduler-2.7.0/src/components/icon-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/icons.ts` & `jupyter_scheduler-2.7.0/src/components/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/input-file-snapshot.tsx` & `jupyter_scheduler-2.7.0/src/components/input-file-snapshot.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/input-folder-checkbox.tsx` & `jupyter_scheduler-2.7.0/src/components/input-folder-checkbox.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/job-definition-row.tsx` & `jupyter_scheduler-2.7.0/src/components/job-definition-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/job-file-link.tsx` & `jupyter_scheduler-2.7.0/src/components/job-file-link.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/job-row.tsx` & `jupyter_scheduler-2.7.0/src/components/job-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/labeled-value.tsx` & `jupyter_scheduler-2.7.0/src/components/labeled-value.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/output-format-picker.tsx` & `jupyter_scheduler-2.7.0/src/components/output-format-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/parameters-picker.tsx` & `jupyter_scheduler-2.7.0/src/components/parameters-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/schedule-inputs.tsx` & `jupyter_scheduler-2.7.0/src/components/schedule-inputs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/advanced-table/advanced-table-header.tsx` & `jupyter_scheduler-2.7.0/src/components/advanced-table/advanced-table-header.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/components/advanced-table/advanced-table.tsx` & `jupyter_scheduler-2.7.0/src/components/advanced-table/advanced-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/mainviews/create-job-from-definition.tsx` & `jupyter_scheduler-2.7.0/src/mainviews/create-job-from-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/mainviews/create-job.tsx` & `jupyter_scheduler-2.7.0/src/mainviews/create-job.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/mainviews/edit-job-definition.tsx` & `jupyter_scheduler-2.7.0/src/mainviews/edit-job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/mainviews/list-jobs.tsx` & `jupyter_scheduler-2.7.0/src/mainviews/list-jobs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/mainviews/detail-view/detail-view.tsx` & `jupyter_scheduler-2.7.0/src/mainviews/detail-view/detail-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/mainviews/detail-view/job-definition.tsx` & `jupyter_scheduler-2.7.0/src/mainviews/detail-view/job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/mainviews/detail-view/job-detail.tsx` & `jupyter_scheduler-2.7.0/src/mainviews/detail-view/job-detail.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/util/errors.tsx` & `jupyter_scheduler-2.7.0/src/util/errors.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/src/util/job-name-validation.tsx` & `jupyter_scheduler-2.7.0/src/util/job-name-validation.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/style/base.css` & `jupyter_scheduler-2.7.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/style/button.css` & `jupyter_scheduler-2.7.0/style/button.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/style/cluster.css` & `jupyter_scheduler-2.7.0/style/cluster.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/style/stack.css` & `jupyter_scheduler-2.7.0/style/stack.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/style/icons/calendar-add-on.svg` & `jupyter_scheduler-2.7.0/style/icons/calendar-add-on.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/style/icons/calendar-month.svg` & `jupyter_scheduler-2.7.0/style/icons/calendar-month.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/README.md` & `jupyter_scheduler-2.7.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/yarn.lock` & `jupyter_scheduler-2.7.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/helpers/SchedulerHelper.ts` & `jupyter_scheduler-2.7.0/ui-tests/helpers/SchedulerHelper.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts` & `jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-filebrowser-linux.png` & `jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-filebrowser-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-toolbar-linux.png` & `jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-toolbar-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/filebrowser-menu-linux.png` & `jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/filebrowser-menu-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/launcher-linux.png` & `jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/list-view-linux.png` & `jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/list-view-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/notebook-toolbar-linux.png` & `jupyter_scheduler-2.7.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/notebook-toolbar-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/.gitignore` & `jupyter_scheduler-2.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/LICENSE` & `jupyter_scheduler-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.6.0/README.md` & `jupyter_scheduler-2.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
 ## Requirements
 
 - JupyterLab 4.x (for newer Jupyter Scheduler versions)
 - JupyterLab 3.x (for Jupyter Scheduler 1.x)
 
 > [!IMPORTANT]
-> JupyterLab 3 will reach its end of maintenance date on May 15, 2024, anywhere on Earth. As a result, we will not backport new features to the v1 branch supporting JupyterLab 3 after this date. Fixes for critical issues will still be backported until December 31, 2024. If you are still using JupyterLab 3, we strongly encourage you to **upgrade to JupyterLab 4 as soon as possible**. For more information, see [JupyterLab 3 end of maintenance](https://blog.jupyter.org/jupyterlab-3-end-of-maintenance-879778927db2) on the Jupyter Blog.
+> Starting with v2.7.0, Jupyter Scheduler requires SQLAlchemy 2.x instead of SQLAlchemy 1.x.
+
+> [!IMPORTANT]
+> JupyterLab 3 reached its end of maintenance date on May 15, 2024. As a result, we will not backport new features to the v1 branch supporting JupyterLab 3 after this date. Fixes for critical issues will still be backported until December 31, 2024. If you are still using JupyterLab 3, we strongly encourage you to **upgrade to JupyterLab 4 as soon as possible**. For more information, see [JupyterLab 3 end of maintenance](https://blog.jupyter.org/jupyterlab-3-end-of-maintenance-879778927db2) on the Jupyter Blog.
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyter_scheduler
```

### Comparing `jupyter_scheduler-2.6.0/pyproject.toml` & `jupyter_scheduler-2.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.3.1", "jupyterlab~=4.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_scheduler"
-version = "2.6.0"
+version = "2.7.0"
 description = "A JupyterLab extension for running notebook jobs"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Project Jupyter" },
 ]
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "jupyter_server>=1.6,<3",
     "traitlets~=5.0",
     "nbconvert~=7.0",
     "pydantic>=1.10,<3",
-    "sqlalchemy~=1.0",
+    "sqlalchemy>=2.0,<3",
     "croniter~=1.4",
     "pytz==2023.3",
     "fsspec==2023.6.0",
     "psutil~=5.9"
 ]
 
 [project.optional-dependencies]
@@ -89,15 +89,15 @@
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
 build_dir = "jupyter_scheduler/labextension"
 
 [tool.tbump.version]
-current = "2.6.0"
+current = "2.7.0"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
 version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\""
 
 [[tool.tbump.file]]
```

### Comparing `jupyter_scheduler-2.6.0/PKG-INFO` & `jupyter_scheduler-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter_scheduler
-Version: 2.6.0
+Version: 2.7.0
 Summary: A JupyterLab extension for running notebook jobs
 Project-URL: Homepage, https://github.com/jupyter-server/jupyter-scheduler
 Author: Project Jupyter
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Project Jupyter
         All rights reserved.
@@ -52,15 +52,15 @@
 Requires-Dist: croniter~=1.4
 Requires-Dist: fsspec==2023.6.0
 Requires-Dist: jupyter-server<3,>=1.6
 Requires-Dist: nbconvert~=7.0
 Requires-Dist: psutil~=5.9
 Requires-Dist: pydantic<3,>=1.10
 Requires-Dist: pytz==2023.3
-Requires-Dist: sqlalchemy~=1.0
+Requires-Dist: sqlalchemy<3,>=2.0
 Requires-Dist: traitlets~=5.0
 Provides-Extra: dev
 Requires-Dist: click; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
@@ -86,15 +86,18 @@
 
 ## Requirements
 
 - JupyterLab 4.x (for newer Jupyter Scheduler versions)
 - JupyterLab 3.x (for Jupyter Scheduler 1.x)
 
 > [!IMPORTANT]
-> JupyterLab 3 will reach its end of maintenance date on May 15, 2024, anywhere on Earth. As a result, we will not backport new features to the v1 branch supporting JupyterLab 3 after this date. Fixes for critical issues will still be backported until December 31, 2024. If you are still using JupyterLab 3, we strongly encourage you to **upgrade to JupyterLab 4 as soon as possible**. For more information, see [JupyterLab 3 end of maintenance](https://blog.jupyter.org/jupyterlab-3-end-of-maintenance-879778927db2) on the Jupyter Blog.
+> Starting with v2.7.0, Jupyter Scheduler requires SQLAlchemy 2.x instead of SQLAlchemy 1.x.
+
+> [!IMPORTANT]
+> JupyterLab 3 reached its end of maintenance date on May 15, 2024. As a result, we will not backport new features to the v1 branch supporting JupyterLab 3 after this date. Fixes for critical issues will still be backported until December 31, 2024. If you are still using JupyterLab 3, we strongly encourage you to **upgrade to JupyterLab 4 as soon as possible**. For more information, see [JupyterLab 3 end of maintenance](https://blog.jupyter.org/jupyterlab-3-end-of-maintenance-879778927db2) on the Jupyter Blog.
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyter_scheduler
```

