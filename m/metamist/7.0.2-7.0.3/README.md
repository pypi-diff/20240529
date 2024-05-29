# Comparing `tmp/metamist-7.0.2.tar.gz` & `tmp/metamist-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-7.0.2.tar", last modified: Fri May 24 05:48:15 2024, max compression
+gzip compressed data, was "metamist-7.0.3.tar", last modified: Wed May 29 01:11:57 2024, max compression
```

## Comparing `metamist-7.0.2.tar` & `metamist-7.0.3.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.941008 metamist-7.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-24 05:45:25.000000 metamist-7.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 05:45:25.000000 metamist-7.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-24 05:48:15.941008 metamist-7.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-24 05:45:25.000000 metamist-7.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.917008 metamist-7.0.2/metamist/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.921008 metamist-7.0.2/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56146 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/analysis_runner_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    82373 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/billing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/cohort_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    50382 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29264 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    48033 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32909 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.925008 metamist-7.0.2/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.925008 metamist-7.0.2/metamist/audit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/audit/audit_upload_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/audit/audithelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/audit/delete_assay_files_from_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/audit/generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.925008 metamist-7.0.2/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-24 05:46:52.000000 metamist-7.0.2/metamist/graphql/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.933008 metamist-7.0.2/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_batch_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_cromwell_subworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_cromwell_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_seq_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_sku.py
--rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_total.py
--rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_cost_record_wdl_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13856 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15657 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/assay.py
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/assay_query_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/billing_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/billing_cost_budget_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/billing_cost_details_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/billing_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/billing_time_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/billing_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/billing_total_cost_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/billing_total_cost_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/body_create_cohort_from_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/body_get_proportionate_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/cohort_body.py
--rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/cohort_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/cohort_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/family.py
--rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/family_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/get_samples_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/new_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/project_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/proportional_date_temporal_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/query_participant_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/seqr_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/sequencing_group_meta_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/sequencing_group_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-24 05:46:47.000000 metamist-7.0.2/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.933008 metamist-7.0.2/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.937008 metamist-7.0.2/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    55754 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-24 05:45:25.000000 metamist-7.0.2/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-24 05:46:48.000000 metamist-7.0.2/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.921008 metamist-7.0.2/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-24 05:48:15.000000 metamist-7.0.2/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-24 05:48:15.000000 metamist-7.0.2/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 05:48:15.000000 metamist-7.0.2/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-24 05:48:15.000000 metamist-7.0.2/metamist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 05:48:15.000000 metamist-7.0.2/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-24 05:48:15.000000 metamist-7.0.2/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 05:48:15.000000 metamist-7.0.2/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-24 05:45:25.000000 metamist-7.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 05:48:15.941008 metamist-7.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-24 05:45:25.000000 metamist-7.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:48:15.941008 metamist-7.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_analysis_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_api_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_audit_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_bq_billing_ar_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    32213 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_bq_billing_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_bq_billing_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_bq_billing_daily_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_bq_billing_gcp_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_bq_billing_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_bq_function_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_bq_generic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18895 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_cohort_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_generic_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_layers_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_metamist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_project_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_update_participant_family.py
--rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-05-24 05:45:25.000000 metamist-7.0.2/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-24 05:45:25.000000 metamist-7.0.2/test/testbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-24 05:45:25.000000 metamist-7.0.2/test/testbqbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.414102 metamist-7.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 01:09:04.000000 metamist-7.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 01:09:04.000000 metamist-7.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-29 01:11:57.414102 metamist-7.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-29 01:09:04.000000 metamist-7.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.394102 metamist-7.0.3/metamist/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.398102 metamist-7.0.3/metamist/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56146 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/analysis_runner_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/assay_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82373 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/billing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/cohort_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50382 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/enums_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29264 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48033 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32909 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/sequencing_group_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.398102 metamist-7.0.3/metamist/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.398102 metamist-7.0.3/metamist/audit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/audit/audit_upload_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/audit/audithelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/audit/delete_assay_files_from_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/audit/generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.398102 metamist-7.0.3/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-29 01:10:40.000000 metamist-7.0.3/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.406103 metamist-7.0.3/metamist/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_batch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_cromwell_subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_cromwell_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_seq_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_sku.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_cost_record_wdl_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15657 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/assay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/assay_query_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/assay_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/billing_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/billing_cost_budget_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/billing_cost_details_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/billing_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/billing_time_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/billing_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/billing_total_cost_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/billing_total_cost_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/body_create_cohort_from_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/body_get_proportionate_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/cohort_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/cohort_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/cohort_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/family.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/family_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/get_samples_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-05-29 01:10:34.000000 metamist-7.0.3/metamist/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/nested_sequencing_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/new_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/project_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/proportional_date_temporal_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/query_participant_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/sample_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/seqr_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/sequencing_group_meta_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/sequencing_group_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/sequencing_group_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.406103 metamist-7.0.3/metamist/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.406103 metamist-7.0.3/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55969 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-29 01:09:04.000000 metamist-7.0.3/metamist/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-29 01:10:35.000000 metamist-7.0.3/metamist/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.394102 metamist-7.0.3/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-29 01:11:57.000000 metamist-7.0.3/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-29 01:11:57.000000 metamist-7.0.3/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:11:57.000000 metamist-7.0.3/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 01:11:57.000000 metamist-7.0.3/metamist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:11:57.000000 metamist-7.0.3/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 01:11:57.000000 metamist-7.0.3/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 01:11:57.000000 metamist-7.0.3/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-29 01:09:04.000000 metamist-7.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:11:57.414102 metamist-7.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-29 01:09:04.000000 metamist-7.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:57.414102 metamist-7.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_analysis_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_api_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_bq_billing_ar_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32213 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_bq_billing_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_bq_billing_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_bq_billing_daily_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_bq_billing_gcp_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_bq_billing_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_bq_function_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_bq_generic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18895 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_cohort_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_layers_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_metamist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36851 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_project_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_update_participant_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-05-29 01:09:04.000000 metamist-7.0.3/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-29 01:09:04.000000 metamist-7.0.3/test/testbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-29 01:09:04.000000 metamist-7.0.3/test/testbqbase.py
```

### Comparing `metamist-7.0.2/LICENSE` & `metamist-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/PKG-INFO` & `metamist-7.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 7.0.2
+Version: 7.0.3
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/metamist
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-7.0.2/README.md` & `metamist-7.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/__init__.py` & `metamist-7.0.3/metamist/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `metamist-7.0.2/metamist/api/analysis_api.py` & `metamist-7.0.3/metamist/api/analysis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/analysis_runner_api.py` & `metamist-7.0.3/metamist/api/analysis_runner_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/assay_api.py` & `metamist-7.0.3/metamist/api/assay_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/billing_api.py` & `metamist-7.0.3/metamist/api/billing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/cohort_api.py` & `metamist-7.0.3/metamist/api/cohort_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/enums_api.py` & `metamist-7.0.3/metamist/api/enums_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/family_api.py` & `metamist-7.0.3/metamist/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/import_api.py` & `metamist-7.0.3/metamist/api/import_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/participant_api.py` & `metamist-7.0.3/metamist/api/participant_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/project_api.py` & `metamist-7.0.3/metamist/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/sample_api.py` & `metamist-7.0.3/metamist/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/seqr_api.py` & `metamist-7.0.3/metamist/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/sequencing_group_api.py` & `metamist-7.0.3/metamist/api/sequencing_group_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api/web_api.py` & `metamist-7.0.3/metamist/api/web_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/api_client.py` & `metamist-7.0.3/metamist/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `metamist-7.0.2/metamist/apis/__init__.py` & `metamist-7.0.3/metamist/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/audit/audit_upload_bucket.py` & `metamist-7.0.3/metamist/audit/audit_upload_bucket.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/audit/audithelper.py` & `metamist-7.0.3/metamist/audit/audithelper.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/audit/delete_assay_files_from_audit.py` & `metamist-7.0.3/metamist/audit/delete_assay_files_from_audit.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/audit/generic_auditor.py` & `metamist-7.0.3/metamist/audit/generic_auditor.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/configuration.py` & `metamist-7.0.3/metamist/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -405,15 +405,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 7.0.2\n"\
+               "Version of the API: 7.0.3\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `metamist-7.0.2/metamist/exceptions.py` & `metamist-7.0.3/metamist/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `metamist-7.0.2/metamist/graphql/__init__.py` & `metamist-7.0.3/metamist/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/graphql/schema.graphql` & `metamist-7.0.3/metamist/graphql/schema.graphql`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
   analysisRunner(arGuid: StrGraphQLFilter = null, author: StrGraphQLFilter = null, repository: StrGraphQLFilter = null, accessLevel: StrGraphQLFilter = null, environment: StrGraphQLFilter = null): [GraphQLAnalysisRunner!]!
   pedigree(internalFamilyIds: [Int!] = null, replaceWithParticipantExternalIds: Boolean! = true, replaceWithFamilyExternalIds: Boolean! = true, includeParticipantsNotInFamilies: Boolean! = false, emptyParticipantValue: String = null): [JSON!]!
   families(id: IntGraphQLFilter = null, externalId: StrGraphQLFilter = null): [GraphQLFamily!]!
   participants: [GraphQLParticipant!]!
   samples(type: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, id: StrGraphQLFilter = null, meta: JSON = null): [GraphQLSample!]!
   sequencingGroups(id: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
   analyses(type: StrGraphQLFilter = null, status: AnalysisStatusGraphQLFilter = null, active: BoolGraphQLFilter = null, meta: JSON = null, timestampCompleted: DatetimeGraphQLFilter = null): [GraphQLAnalysis!]!
-  cohorts(id: IntGraphQLFilter = null, name: StrGraphQLFilter = null, author: StrGraphQLFilter = null, templateId: StrGraphQLFilter = null, timestamp: DatetimeGraphQLFilter = null): [GraphQLCohort!]!
+  cohorts(id: StrGraphQLFilter = null, name: StrGraphQLFilter = null, author: StrGraphQLFilter = null, templateId: StrGraphQLFilter = null, timestamp: DatetimeGraphQLFilter = null): [GraphQLCohort!]!
 }
 
 type GraphQLSample {
   id: String!
   externalId: String!
   active: Boolean!
   meta: JSON!
```

### Comparing `metamist-7.0.2/metamist/model/analysis.py` & `metamist-7.0.3/metamist/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record.py` & `metamist-7.0.3/metamist/model/analysis_cost_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_batch.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_batch_job.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_batch_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_category.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_cromwell_subworkflow.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_cromwell_subworkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_cromwell_workflow.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_cromwell_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_seq_group.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_seq_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_sku.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_sku.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_topic.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_topic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_total.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_total.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_cost_record_wdl_task.py` & `metamist-7.0.3/metamist/model/analysis_cost_record_wdl_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_internal.py` & `metamist-7.0.3/metamist/model/analysis_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_query_model.py` & `metamist-7.0.3/metamist/model/analysis_query_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -79,15 +79,14 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'sequencing_group_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'projects': ([str],),  # noqa: E501
-            'sample_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'output': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'active': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
@@ -95,15 +94,14 @@
     def discriminator():
         return None
 
 
     attribute_map = {
         'sequencing_group_ids': 'sequencing_group_ids',  # noqa: E501
         'projects': 'projects',  # noqa: E501
-        'sample_ids': 'sample_ids',  # noqa: E501
         'type': 'type',  # noqa: E501
         'status': 'status',  # noqa: E501
         'meta': 'meta',  # noqa: E501
         'output': 'output',  # noqa: E501
         'active': 'active',  # noqa: E501
     }
 
@@ -148,15 +146,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             output (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
@@ -241,15 +238,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             output (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
```

### Comparing `metamist-7.0.2/metamist/model/analysis_runner.py` & `metamist-7.0.3/metamist/model/analysis_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_status.py` & `metamist-7.0.3/metamist/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/analysis_update_model.py` & `metamist-7.0.3/metamist/model/analysis_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/assay.py` & `metamist-7.0.3/metamist/model/assay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/assay_query_criteria.py` & `metamist-7.0.3/metamist/model/assay_query_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/assay_upsert.py` & `metamist-7.0.3/metamist/model/assay_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/billing_column.py` & `metamist-7.0.3/metamist/model/billing_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/billing_cost_budget_record.py` & `metamist-7.0.3/metamist/model/billing_cost_budget_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/billing_cost_details_record.py` & `metamist-7.0.3/metamist/model/billing_cost_details_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/billing_source.py` & `metamist-7.0.3/metamist/model/billing_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/billing_time_column.py` & `metamist-7.0.3/metamist/model/billing_time_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/billing_time_periods.py` & `metamist-7.0.3/metamist/model/billing_time_periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/billing_total_cost_query_model.py` & `metamist-7.0.3/metamist/model/billing_total_cost_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/billing_total_cost_record.py` & `metamist-7.0.3/metamist/model/billing_total_cost_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/body_create_cohort_from_criteria.py` & `metamist-7.0.3/metamist/model/body_create_cohort_from_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/body_get_latest_complete_analysis_for_type_post.py` & `metamist-7.0.3/metamist/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/body_get_proportionate_map.py` & `metamist-7.0.3/metamist/model/body_get_proportionate_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/cohort_body.py` & `metamist-7.0.3/metamist/model/cohort_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/cohort_criteria.py` & `metamist-7.0.3/metamist/model/cohort_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/cohort_template.py` & `metamist-7.0.3/metamist/model/cohort_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/error_response.py` & `metamist-7.0.3/metamist/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/export_type.py` & `metamist-7.0.3/metamist/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/extra_participant_importer_handler.py` & `metamist-7.0.3/metamist/model/extra_participant_importer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/family.py` & `metamist-7.0.3/metamist/model/family.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/family_search_response_data.py` & `metamist-7.0.3/metamist/model/family_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/family_simple.py` & `metamist-7.0.3/metamist/model/family_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/family_update_model.py` & `metamist-7.0.3/metamist/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/get_samples_criteria.py` & `metamist-7.0.3/metamist/model/get_samples_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/http_validation_error.py` & `metamist-7.0.3/metamist/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/meta_search_entity_prefix.py` & `metamist-7.0.3/metamist/model/meta_search_entity_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/nested_participant.py` & `metamist-7.0.3/metamist/model/nested_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/nested_sample.py` & `metamist-7.0.3/metamist/model/nested_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/nested_sequencing_group.py` & `metamist-7.0.3/metamist/model/nested_sequencing_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/new_cohort.py` & `metamist-7.0.3/metamist/model/new_cohort.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/paging_links.py` & `metamist-7.0.3/metamist/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/participant_search_response_data.py` & `metamist-7.0.3/metamist/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/participant_upsert.py` & `metamist-7.0.3/metamist/model/participant_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/project.py` & `metamist-7.0.3/metamist/model/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/project_summary.py` & `metamist-7.0.3/metamist/model/project_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/proportional_date_temporal_method.py` & `metamist-7.0.3/metamist/model/proportional_date_temporal_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/query_participant_criteria.py` & `metamist-7.0.3/metamist/model/query_participant_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/sample_search_response_data.py` & `metamist-7.0.3/metamist/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/sample_upsert.py` & `metamist-7.0.3/metamist/model/sample_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/search_item.py` & `metamist-7.0.3/metamist/model/search_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/search_response.py` & `metamist-7.0.3/metamist/model/search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/search_response_model.py` & `metamist-7.0.3/metamist/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/search_response_type.py` & `metamist-7.0.3/metamist/model/search_response_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/seqr_dataset_type.py` & `metamist-7.0.3/metamist/model/seqr_dataset_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/sequencing_group_meta_update_model.py` & `metamist-7.0.3/metamist/model/sequencing_group_meta_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/sequencing_group_search_response_data.py` & `metamist-7.0.3/metamist/model/sequencing_group_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/sequencing_group_upsert.py` & `metamist-7.0.3/metamist/model/sequencing_group_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/validation_error.py` & `metamist-7.0.3/metamist/model/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model/web_project.py` & `metamist-7.0.3/metamist/model/web_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.2/metamist/model_utils.py` & `metamist-7.0.3/metamist/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `metamist-7.0.2/metamist/models/__init__.py` & `metamist-7.0.3/metamist/models/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/parser/cloudhelper.py` & `metamist-7.0.3/metamist/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/parser/generic_metadata_parser.py` & `metamist-7.0.3/metamist/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/parser/generic_parser.py` & `metamist-7.0.3/metamist/parser/generic_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1082,15 +1082,17 @@
                     'sequencing_facility',
                     'sequencing_library',
                     'read_end_type',
                     'read_length',
                 )
             elif assay.meta.get('sequencing_technology') == 'long-read':
                 # lift all assay meta into the sequencing group meta for long-read
-                keys = [k for k in assay.meta.keys() if k not in ('reads', 'reads_type')]
+                # except for assay reads, and keys that are already top-level sequencing group fields
+                keys_to_avoid = ('reads', 'reads_type', 'sequencing_type', 'sequencing_technology', 'sequencing_platform')
+                keys = [k for k in assay.meta.keys() if k not in keys_to_avoid]
             else:
                 continue
             for key in keys:
                 if assay.meta.get(key) is not None:
                     meta[key] = assay.meta[key]
         return meta
```

### Comparing `metamist-7.0.2/metamist/parser/sample_file_map_parser.py` & `metamist-7.0.3/metamist/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/metamist/rest.py` & `metamist-7.0.3/metamist/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.2
+    The version of the OpenAPI document: 7.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `metamist-7.0.2/metamist.egg-info/PKG-INFO` & `metamist-7.0.3/metamist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 7.0.2
+Version: 7.0.3
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/metamist
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-7.0.2/metamist.egg-info/SOURCES.txt` & `metamist-7.0.3/metamist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/pyproject.toml` & `metamist-7.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/setup.py` & `metamist-7.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='7.0.2',
+    version='7.0.3',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/metamist',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `metamist-7.0.2/test/test_analysis.py` & `metamist-7.0.3/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_analysis_runner.py` & `metamist-7.0.3/test/test_analysis_runner.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_api_billing.py` & `metamist-7.0.3/test/test_api_billing.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_api_utils.py` & `metamist-7.0.3/test/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_assay.py` & `metamist-7.0.3/test/test_assay.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_audit_log.py` & `metamist-7.0.3/test/test_audit_log.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_bq_billing_ar_batch.py` & `metamist-7.0.3/test/test_bq_billing_ar_batch.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_bq_billing_base.py` & `metamist-7.0.3/test/test_bq_billing_base.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_bq_billing_daily.py` & `metamist-7.0.3/test/test_bq_billing_daily.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_bq_billing_daily_extended.py` & `metamist-7.0.3/test/test_bq_billing_daily_extended.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_bq_billing_gcp_daily.py` & `metamist-7.0.3/test/test_bq_billing_gcp_daily.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_bq_billing_raw.py` & `metamist-7.0.3/test/test_bq_billing_raw.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_bq_function_filter.py` & `metamist-7.0.3/test/test_bq_function_filter.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_bq_generic_filter.py` & `metamist-7.0.3/test/test_bq_generic_filter.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_cohort.py` & `metamist-7.0.3/test/test_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_cohort_builder.py` & `metamist-7.0.3/test/test_cohort_builder.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_generate_data.py` & `metamist-7.0.3/test/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_generic_auditor.py` & `metamist-7.0.3/test/test_generic_auditor.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_generic_filters.py` & `metamist-7.0.3/test/test_generic_filters.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_get_participants.py` & `metamist-7.0.3/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_graphql.py` & `metamist-7.0.3/test/test_graphql.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_import_individual_metadata.py` & `metamist-7.0.3/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_layers_billing.py` & `metamist-7.0.3/test/test_layers_billing.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_metamist.py` & `metamist-7.0.3/test/test_metamist.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_models.py` & `metamist-7.0.3/test/test_models.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_parse_existing_cohort.py` & `metamist-7.0.3/test/test_parse_existing_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_parse_file_map.py` & `metamist-7.0.3/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_parse_generic_metadata.py` & `metamist-7.0.3/test/test_parse_generic_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -486,15 +486,15 @@
     @run_as_sync
     @patch('metamist.parser.generic_parser.query_async')
     async def test_lrs_rows_with_arbitrary_assay_meta_columns(
         self,
         mock_graphql_query
     ):
         """
-        Test importing a single row of long read sequencing data with arbitrary assay metadata columns
+        Test importing rows of long read sequencing data with arbitrary assay metadata columns
         """
         mock_graphql_query.side_effect = self.run_graphql_query_async
         self.maxDiff = None
         rows = [
             'Individual ID\tSample ID\tFilename\tAssay Meta 1\tAssay Meta 2',
             'Athena\tsample_id003\t"sample_id003.filename-01-R1.fastq.gz,sample_id003.filename-01-R2.fastq.gz"\tTrue\tsome_value',
             'Athena\tsample_id003\t"sample_id003.filename-02-R1.fastq.gz,sample_id003.filename-02-R2.fastq.gz"\t5\tFalse',
@@ -582,17 +582,14 @@
             'sequencing_technology': 'long-read',
             'sequencing_type': 'genome',
             'assay_meta1': [5, True],
             'assay_meta2': [False, 'some_value'],
         }
 
         expected_sg_dict = {
-            'sequencing_platform': 'pacbio',
-            'sequencing_technology': 'long-read',
-            'sequencing_type': 'genome',
             'assay_meta1': [5, True],
             'assay_meta2': [False, 'some_value'],
         }
 
         assay_1 = participants[0].samples[0].sequencing_groups[0].assays[0]
         assay_2 = participants[0].samples[0].sequencing_groups[0].assays[1]
         sg = participants[0].samples[0].sequencing_groups[0]
```

### Comparing `metamist-7.0.2/test/test_parse_ont_processor.py` & `metamist-7.0.3/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_parse_ont_sheet.py` & `metamist-7.0.3/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_pedigree.py` & `metamist-7.0.3/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_project_groups.py` & `metamist-7.0.3/test/test_project_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_sample.py` & `metamist-7.0.3/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_search.py` & `metamist-7.0.3/test/test_search.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_sequencing_groups.py` & `metamist-7.0.3/test/test_sequencing_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_update_participant_family.py` & `metamist-7.0.3/test/test_update_participant_family.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_upsert.py` & `metamist-7.0.3/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/test_web.py` & `metamist-7.0.3/test/test_web.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/testbase.py` & `metamist-7.0.3/test/testbase.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.2/test/testbqbase.py` & `metamist-7.0.3/test/testbqbase.py`

 * *Files identical despite different names*

