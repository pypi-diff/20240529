# Comparing `tmp/pycti-6.1.4.tar.gz` & `tmp/pycti-6.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-6.1.4.tar", last modified: Thu May 23 22:27:40 2024, max compression
+gzip compressed data, was "pycti-6.1.5.tar", last modified: Tue May 28 23:32:52 2024, max compression
```

## Comparing `pycti-6.1.4.tar` & `pycti-6.1.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.827206 pycti-6.1.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-23 22:27:27.000000 pycti-6.1.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-23 22:27:40.827206 pycti-6.1.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-23 22:27:27.000000 pycti-6.1.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.815206 pycti-6.1.4/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.815206 pycti-6.1.4/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/opencti_api_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.815206 pycti-6.1.4/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    60311 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/connector/opencti_connector_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/connector/opencti_metric_handler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.823206 pycti-6.1.4/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43249 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.823206 pycti-6.1.4/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   112457 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.823206 pycti-6.1.4/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-23 22:27:28.000000 pycti-6.1.4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-23 22:27:40.827206 pycti-6.1.4/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:52.122554 pycti-6.1.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-28 23:32:36.000000 pycti-6.1.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5353 2024-05-28 23:32:52.122554 pycti-6.1.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-28 23:32:36.000000 pycti-6.1.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:52.110554 pycti-6.1.5/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:52.110554 pycti-6.1.5/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29701 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/api/opencti_api_playbook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:52.110554 pycti-6.1.5/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60496 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/connector/opencti_connector_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/connector/opencti_metric_handler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:52.118554 pycti-6.1.5/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43249 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:52.118554 pycti-6.1.5/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/utils/opencti_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   117232 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4907 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-28 23:32:36.000000 pycti-6.1.5/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 23:32:52.118554 pycti-6.1.5/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5353 2024-05-28 23:32:52.000000 pycti-6.1.5/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-28 23:32:52.000000 pycti-6.1.5/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-28 23:32:52.000000 pycti-6.1.5/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      662 2024-05-28 23:32:52.000000 pycti-6.1.5/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-28 23:32:52.000000 pycti-6.1.5/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-28 23:32:36.000000 pycti-6.1.5/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2024-05-28 23:32:52.122554 pycti-6.1.5/setup.cfg
```

### Comparing `pycti-6.1.4/LICENSE` & `pycti-6.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/PKG-INFO` & `pycti-6.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.4
+Version: 6.1.5
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,25 +18,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datefinder~=0.7.3
-Requires-Dist: pika~=1.3.1
+Requires-Dist: pika~=1.3.0
 Requires-Dist: python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
-Requires-Dist: prometheus-client~=0.20.0
 Requires-Dist: python-magic-bin~=0.4.14; sys_platform == "win32"
 Requires-Dist: python_json_logger~=2.0.4
-Requires-Dist: pyyaml~=6.0
-Requires-Dist: requests~=2.31.0
-Requires-Dist: setuptools~=69.5.1
+Requires-Dist: PyYAML~=6.0
+Requires-Dist: requests~=2.32.2
+Requires-Dist: setuptools~=70.0.0
+Requires-Dist: cachetools~=5.3.0
+Requires-Dist: prometheus-client~=0.20.0
+Requires-Dist: opentelemetry-api~=1.22.0
+Requires-Dist: opentelemetry-sdk~=1.22.0
 Requires-Dist: filigran-sseclient~=1.0.0
 Requires-Dist: stix2~=3.0.1
-Requires-Dist: cachetools~=5.3.0
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
 Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 Requires-Dist: pytest-cases~=3.8.0; extra == "dev"
```

### Comparing `pycti-6.1.4/README.md` & `pycti-6.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/__init__.py` & `pycti-6.1.5/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "6.1.4"
+__version__ = "6.1.5"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-6.1.4/pycti/api/opencti_api_client.py` & `pycti-6.1.5/pycti/api/opencti_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,22 +347,24 @@
             if "errors" in result:
                 main_error = result["errors"][0]
                 error_name = (
                     main_error["name"]
                     if "name" in main_error
                     else main_error["message"]
                 )
-                if "data" in main_error and "reason" in main_error["data"]:
-                    raise ValueError(
-                        {"name": error_name, "message": main_error["data"]["reason"]}
-                    )
-                else:
-                    raise ValueError(
-                        {"name": error_name, "message": main_error["message"]}
-                    )
+                error_detail = {
+                    "name": error_name,
+                    "error_message": main_error["message"],
+                }
+                meta_data = main_error["data"] if "data" in main_error else {}
+                # Prevent logging of input as bundle is logged differently
+                if meta_data.get("input") is not None:
+                    del meta_data["input"]
+                value_error = {**error_detail, **meta_data}
+                raise ValueError(value_error)
             else:
                 return result
         else:
             raise ValueError(r.text)
 
     def fetch_opencti_file(self, fetch_uri, binary=False, serialize=False):
         """get file from the OpenCTI API
```

### Comparing `pycti-6.1.4/pycti/api/opencti_api_connector.py` & `pycti-6.1.5/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/api/opencti_api_playbook.py` & `pycti-6.1.5/pycti/api/opencti_api_playbook.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/api/opencti_api_work.py` & `pycti-6.1.5/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/connector/opencti_connector.py` & `pycti-6.1.5/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/connector/opencti_connector_helper.py` & `pycti-6.1.5/pycti/connector/opencti_connector_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1222,25 +1222,30 @@
                 f.write(str_bundle)
             # Rename the file after full write
             final_write_file = os.path.join(bundle_send_to_directory_path, bundle_file)
             os.rename(write_file, final_write_file)
 
         if bypass_split:
             bundles = [bundle]
+            expectations_number = len(json.loads(bundle)["objects"])
         else:
             stix2_splitter = OpenCTIStix2Splitter()
-            bundles = stix2_splitter.split_bundle(bundle, True, event_version)
+            expectations_number, bundles = (
+                stix2_splitter.split_bundle_with_expectations(
+                    bundle, True, event_version
+                )
+            )
 
         if len(bundles) == 0:
             self.metric.inc("error_count")
             raise ValueError("Nothing to import")
 
         if bundle_send_to_queue:
             if work_id:
-                self.api.work.add_expectations(work_id, len(bundles))
+                self.api.work.add_expectations(work_id, expectations_number)
             if entities_types is None:
                 entities_types = []
             pika_credentials = pika.PlainCredentials(
                 self.connector_config["connection"]["user"],
                 self.connector_config["connection"]["pass"],
             )
             pika_parameters = pika.ConnectionParameters(
```

### Comparing `pycti-6.1.4/pycti/connector/opencti_metric_handler.py` & `pycti-6.1.5/pycti/connector/opencti_metric_handler.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_attack_pattern.py` & `pycti-6.1.5/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_campaign.py` & `pycti-6.1.5/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_case_incident.py` & `pycti-6.1.5/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_case_rfi.py` & `pycti-6.1.5/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_case_rft.py` & `pycti-6.1.5/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_channel.py` & `pycti-6.1.5/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_course_of_action.py` & `pycti-6.1.5/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_data_component.py` & `pycti-6.1.5/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_data_source.py` & `pycti-6.1.5/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_event.py` & `pycti-6.1.5/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_external_reference.py` & `pycti-6.1.5/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_feedback.py` & `pycti-6.1.5/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_grouping.py` & `pycti-6.1.5/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_identity.py` & `pycti-6.1.5/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_incident.py` & `pycti-6.1.5/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_indicator.py` & `pycti-6.1.5/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_infrastructure.py` & `pycti-6.1.5/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_intrusion_set.py` & `pycti-6.1.5/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_kill_chain_phase.py` & `pycti-6.1.5/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_label.py` & `pycti-6.1.5/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_language.py` & `pycti-6.1.5/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_location.py` & `pycti-6.1.5/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_malware.py` & `pycti-6.1.5/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_malware_analysis.py` & `pycti-6.1.5/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_marking_definition.py` & `pycti-6.1.5/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_narrative.py` & `pycti-6.1.5/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_note.py` & `pycti-6.1.5/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_observed_data.py` & `pycti-6.1.5/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_opinion.py` & `pycti-6.1.5/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_report.py` & `pycti-6.1.5/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_stix.py` & `pycti-6.1.5/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_stix_core_object.py` & `pycti-6.1.5/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_stix_core_relationship.py` & `pycti-6.1.5/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-6.1.5/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_stix_domain_object.py` & `pycti-6.1.5/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-6.1.5/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-6.1.5/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-6.1.5/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_task.py` & `pycti-6.1.5/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_threat_actor.py` & `pycti-6.1.5/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_threat_actor_group.py` & `pycti-6.1.5/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_threat_actor_individual.py` & `pycti-6.1.5/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_tool.py` & `pycti-6.1.5/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_vocabulary.py` & `pycti-6.1.5/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/entities/opencti_vulnerability.py` & `pycti-6.1.5/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/utils/constants.py` & `pycti-6.1.5/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/utils/opencti_logger.py` & `pycti-6.1.5/pycti/utils/opencti_logger.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/utils/opencti_stix2.py` & `pycti-6.1.5/pycti/utils/opencti_stix2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # coding: utf-8
 
 import base64
 import datetime
 import json
 import os
+import random
+import time
+import traceback
 import uuid
 from typing import Any, Dict, List, Optional, Union
 
 import datefinder
 import dateutil.parser
 import pytz
 from cachetools import LRUCache
+from opentelemetry import metrics
+from requests import RequestException, Timeout
 
 from pycti.entities.opencti_identity import Identity
 from pycti.utils.constants import (
     IdentityTypes,
     LocationTypes,
     MultipleRefRelationship,
     StixCyberObservableTypes,
@@ -28,19 +33,49 @@
 )
 
 datefinder.ValueError = ValueError, OverflowError
 utc = pytz.UTC
 
 # Spec version
 SPEC_VERSION = "2.1"
+ERROR_TYPE_LOCK = "LOCK_ERROR"
+ERROR_TYPE_MISSING_REFERENCE = "MISSING_REFERENCE_ERROR"
+ERROR_TYPE_BAD_GATEWAY = "Bad Gateway"
 
 # Extensions
 STIX_EXT_OCTI = "extension-definition--ea279b3e-5c71-4632-ac08-831c66a786ba"
 STIX_EXT_OCTI_SCO = "extension-definition--f93e2c80-4231-4f9a-af8b-95c9bd566a82"
 STIX_EXT_MITRE = "extension-definition--322b8f77-262a-4cb8-a915-1e441e00329b"
+PROCESSING_COUNT: int = 4
+
+meter = metrics.get_meter(__name__)
+bundles_timeout_error_counter = meter.create_counter(
+    name="opencti_bundles_timeout_error_counter",
+    description="number of bundles in timeout error",
+)
+bundles_lock_error_counter = meter.create_counter(
+    name="opencti_bundles_lock_error_counter",
+    description="number of bundles in lock error",
+)
+bundles_missing_reference_error_counter = meter.create_counter(
+    name="opencti_bundles_missing_reference_error_counter",
+    description="number of bundles in missing reference error",
+)
+bundles_bad_gateway_error_counter = meter.create_counter(
+    name="opencti_bundles_bad_gateway_error_counter",
+    description="number of bundles in bad gateway error",
+)
+bundles_technical_error_counter = meter.create_counter(
+    name="opencti_bundles_technical_error_counter",
+    description="number of bundles in technical error",
+)
+bundles_success_counter = meter.create_counter(
+    name="opencti_bundles_success_counter",
+    description="number of bundles successfully processed",
+)
 
 
 class OpenCTIStix2:
     """Python API for Stix2 in OpenCTI
 
     :param opencti: OpenCTI instance
     """
@@ -157,34 +192,30 @@
         return self.import_bundle(data, update, types)
 
     def import_bundle_from_json(
         self,
         json_data: Union[str, bytes],
         update: bool = False,
         types: List = None,
-        retry_number: int = None,
+        work_id: str = None,
     ) -> List:
         """import a stix2 bundle from JSON data
 
         :param json_data: JSON data
         :type json_data:
         :param update: whether to updated data in the database, defaults to False
         :type update: bool, optional
         :param types: list of stix2 types, defaults to None
         :type types: list, optional
+        :param work_id work_id: str, optional
         :return: list of imported stix2 objects
         :rtype: List
         """
         data = json.loads(json_data)
-        return self.import_bundle(
-            data,
-            update,
-            types,
-            retry_number,
-        )
+        return self.import_bundle(data, update, types, work_id)
 
     def resolve_author(self, title: str) -> Optional[Identity]:
         if "fireeye" in title.lower() or "mandiant" in title.lower():
             return self.get_author("FireEye")
         if "eset" in title.lower():
             return self.get_author("ESET")
         if "dragos" in title.lower():
@@ -1184,15 +1215,15 @@
             "external_references_ids": external_references_ids,
             "reports": reports,
             "sample_ids": sample_refs_ids,
         }
 
         # Create the relation
 
-        ## Try to guess start_time / stop_time from external reference
+        # Try to guess start_time / stop_time from external reference
         date = None
         if "external_references" in stix_relation:
             for external_reference in stix_relation["external_references"]:
                 try:
                     if "description" in external_reference:
                         matches = datefinder.find_dates(
                             external_reference["description"],
@@ -2358,177 +2389,264 @@
                     uuids.append(x["id"])
                 bundle["objects"] = (
                     bundle["objects"] + entity_bundle_filtered
                 )  # unsupported operand type(s) for +: 'dict' and 'list'
 
         return bundle
 
+    def import_item(
+        self,
+        item,
+        update: bool = False,
+        types: List = None,
+        processing_count: int = 0,
+        work_id: str = None,
+    ):
+        worker_logger = self.opencti.logger_class("worker")
+        try:
+            self.opencti.set_retry_number(processing_count)
+            if "opencti_operation" in item:
+                if item["opencti_operation"] == "delete":
+                    delete_id = item["id"]
+                    self.opencti.stix.delete(id=delete_id)
+                if item["opencti_operation"] == "merge":
+                    target_id = item["merge_target_id"]
+                    source_ids = item["merge_source_ids"]
+                    self.opencti.stix.merge(id=target_id, object_ids=source_ids)
+                else:
+                    raise ValueError("Not supported opencti_operation")
+            elif item["type"] == "relationship":
+                # Import relationship
+                self.import_relationship(item, update, types)
+            elif item["type"] == "sighting":
+                # Resolve the to
+                to_ids = []
+                if "where_sighted_refs" in item:
+                    for where_sighted_ref in item["where_sighted_refs"]:
+                        to_ids.append(where_sighted_ref)
+                # Import sighting_of_ref
+                if "x_opencti_sighting_of_ref" in item:
+                    from_id = item["x_opencti_sighting_of_ref"]
+                    if len(to_ids) > 0:
+                        for to_id in to_ids:
+                            self.import_sighting(item, from_id, to_id, update)
+                if (
+                    self.opencti.get_attribute_in_extension("sighting_of_ref", item)
+                    is not None
+                ):
+                    from_id = self.opencti.get_attribute_in_extension(
+                        "sighting_of_ref", item
+                    )
+                    if len(to_ids) > 0:
+                        for to_id in to_ids:
+                            self.import_sighting(item, from_id, to_id, update)
+                from_id = item["sighting_of_ref"]
+                if len(to_ids) > 0:
+                    for to_id in to_ids:
+                        self.import_sighting(item, from_id, to_id, update)
+                # Import observed_data_refs
+                if "observed_data_refs" in item:
+                    for observed_data_ref in item["observed_data_refs"]:
+                        if len(to_ids) > 0:
+                            for to_id in to_ids:
+                                self.import_sighting(
+                                    item, observed_data_ref, to_id, update
+                                )
+            elif item["type"] == "label":
+                stix_ids = self.opencti.get_attribute_in_extension("stix_ids", item)
+                self.opencti.label.create(
+                    stix_id=item["id"],
+                    value=item["value"],
+                    color=item["color"],
+                    x_opencti_stix_ids=stix_ids,
+                    update=update,
+                )
+            elif item["type"] == "vocabulary":
+                stix_ids = self.opencti.get_attribute_in_extension("stix_ids", item)
+                self.opencti.vocabulary.create(
+                    stix_id=item["id"],
+                    name=item["name"],
+                    category=item["category"],
+                    description=(
+                        item["description"] if "description" in item else None
+                    ),
+                    aliases=item["aliases"] if "aliases" in item else None,
+                    x_opencti_stix_ids=stix_ids,
+                    update=update,
+                )
+            elif item["type"] == "external-reference":
+                stix_ids = self.opencti.get_attribute_in_extension("stix_ids", item)
+                self.opencti.external_reference.create(
+                    stix_id=item["id"],
+                    source_name=(
+                        item["source_name"] if "source_name" in item else None
+                    ),
+                    url=item["url"] if "url" in item else None,
+                    external_id=(
+                        item["external_id"] if "external_id" in item else None
+                    ),
+                    description=(
+                        item["description"] if "description" in item else None
+                    ),
+                    x_opencti_stix_ids=stix_ids,
+                    update=update,
+                )
+            elif item["type"] == "kill-chain-phase":
+                stix_ids = self.opencti.get_attribute_in_extension("stix_ids", item)
+                self.opencti.kill_chain_phase.create(
+                    stix_id=item["id"],
+                    kill_chain_name=item["kill_chain_name"],
+                    phase_name=item["phase_name"],
+                    x_opencti_order=item["order"] if "order" in item else 0,
+                    x_opencti_stix_ids=stix_ids,
+                    update=update,
+                )
+            elif StixCyberObservableTypes.has_value(item["type"]):
+                if types is None or len(types) == 0:
+                    self.import_observable(item, update, types)
+                elif item["type"] in types or "observable" in types:
+                    self.import_observable(item, update, types)
+            else:
+                # Check the scope
+                if (
+                    item["type"] == "marking-definition"
+                    or types is None
+                    or len(types) == 0
+                ):
+                    self.import_object(item, update, types)
+                # Handle identity & location if part of the scope
+                elif item["type"] in types:
+                    self.import_object(item, update, types)
+                else:
+                    # Specific OpenCTI scopes
+                    if item["type"] == "identity":
+                        if "identity_class" in item:
+                            if ("class" in types or "sector" in types) and item[
+                                "identity_class"
+                            ] == "class":
+                                self.import_object(item, update, types)
+                            elif item["identity_class"] in types:
+                                self.import_object(item, update, types)
+                    elif item["type"] == "location":
+                        if "x_opencti_location_type" in item:
+                            if item["x_opencti_location_type"].lower() in types:
+                                self.import_object(item, update, types)
+                        elif (
+                            self.opencti.get_attribute_in_extension(
+                                "location_type", item
+                            )
+                            is not None
+                        ):
+                            if (
+                                self.opencti.get_attribute_in_extension(
+                                    "location_type", item
+                                ).lower()
+                                in types
+                            ):
+                                self.import_object(item, update, types)
+            if work_id is not None:
+                self.opencti.work.report_expectation(work_id, None)
+            bundles_success_counter.add(1)
+            return True
+        except (RequestException, Timeout):
+            bundles_timeout_error_counter.add(1)
+            worker_logger.warning("A connection error or timeout occurred")
+            # Platform is under heavy load: wait for unlock & retry almost indefinitely.
+            sleep_jitter = round(random.uniform(10, 30), 2)
+            time.sleep(sleep_jitter)
+            return self.import_item(item, update, types, processing_count + 1, work_id)
+        except Exception as ex:  # pylint: disable=broad-except
+            error = str(ex)
+            error_msg = traceback.format_exc()
+            in_retry = processing_count < PROCESSING_COUNT
+            # Platform is under heavy load, wait for unlock & retry indefinitely.
+            if ERROR_TYPE_LOCK in error_msg:
+                worker_logger.info(
+                    "Message reprocess for lock rejection", {"count": processing_count}
+                )
+                bundles_lock_error_counter.add(1)
+                sleep_jitter = round(random.uniform(1, 3), 2)
+                time.sleep(sleep_jitter)
+                return self.import_item(
+                    item, update, types, processing_count + 1, work_id
+                )
+            # Platform detects a missing reference and have to retry
+            elif ERROR_TYPE_MISSING_REFERENCE in error_msg and in_retry:
+                worker_logger.info(
+                    "Message reprocess for missing reference",
+                    {"count": processing_count},
+                )
+                bundles_missing_reference_error_counter.add(1)
+                sleep_jitter = round(random.uniform(1, 3), 2)
+                time.sleep(sleep_jitter)
+                return self.import_item(
+                    item, update, types, processing_count + 1, work_id
+                )
+            # A bad gateway error occurs
+            elif ERROR_TYPE_BAD_GATEWAY in error_msg:
+                worker_logger.error("A connection error occurred")
+                worker_logger.info(
+                    "Message reprocess for bad gateway",
+                    {"count": processing_count},
+                )
+                bundles_bad_gateway_error_counter.add(1)
+                time.sleep(60)
+                return self.import_item(
+                    item, update, types, processing_count + 1, work_id
+                )
+            # Platform does not know what to do and raises an error:
+            # That also works for missing reference with too much execution
+            else:
+                bundles_technical_error_counter.add(1)
+                worker_logger.error(
+                    "Error executing import",
+                    {"count": processing_count, "reason": error},
+                )
+                if work_id is not None:
+                    item_str = json.dumps(item)
+                    self.opencti.work.report_expectation(
+                        work_id,
+                        {
+                            "error": error,
+                            "source": (
+                                item_str
+                                if len(item_str) < 50000
+                                else "Bundle too large"
+                            ),
+                        },
+                    )
+                return False
+
     def import_bundle(
         self,
         stix_bundle: Dict,
         update: bool = False,
         types: List = None,
-        retry_number: int = None,
+        work_id: str = None,
     ) -> List:
         # Check if the bundle is correctly formatted
         if "type" not in stix_bundle or stix_bundle["type"] != "bundle":
             raise ValueError("JSON data type is not a STIX2 bundle")
         if "objects" not in stix_bundle or len(stix_bundle["objects"]) == 0:
             raise ValueError("JSON data objects is empty")
         event_version = (
             stix_bundle["x_opencti_event_version"]
             if "x_opencti_event_version" in stix_bundle
             else None
         )
-        if retry_number is not None:
-            self.opencti.set_retry_number(retry_number)
         stix2_splitter = OpenCTIStix2Splitter()
         try:
             bundles = stix2_splitter.split_bundle(stix_bundle, False, event_version)
         except RecursionError:
             bundles = [stix_bundle]
-        # Import every elements in a specific order
+        # Import every element in a specific order
         imported_elements = []
-
-        # Marking definitions
         for bundle in bundles:
             for item in bundle["objects"]:
-                if "x_opencti_event_version" in bundle:
-                    if bundle["x_opencti_event_version"] == "3":
-                        if "x_opencti_patch" in item:
-                            self.stix2_update.process_update(item)
-                            continue
-                if item["type"] == "relationship":
-                    self.import_relationship(item, update, types)
-                elif item["type"] == "sighting":
-                    # Resolve the to
-                    to_ids = []
-                    if "where_sighted_refs" in item:
-                        for where_sighted_ref in item["where_sighted_refs"]:
-                            to_ids.append(where_sighted_ref)
-                    # Import sighting_of_ref
-                    if "x_opencti_sighting_of_ref" in item:
-                        from_id = item["x_opencti_sighting_of_ref"]
-                        if len(to_ids) > 0:
-                            for to_id in to_ids:
-                                self.import_sighting(item, from_id, to_id, update)
-                    if (
-                        self.opencti.get_attribute_in_extension("sighting_of_ref", item)
-                        is not None
-                    ):
-                        from_id = self.opencti.get_attribute_in_extension(
-                            "sighting_of_ref", item
-                        )
-                        if len(to_ids) > 0:
-                            for to_id in to_ids:
-                                self.import_sighting(item, from_id, to_id, update)
-                    from_id = item["sighting_of_ref"]
-                    if len(to_ids) > 0:
-                        for to_id in to_ids:
-                            self.import_sighting(item, from_id, to_id, update)
-                    # Import observed_data_refs
-                    if "observed_data_refs" in item:
-                        for observed_data_ref in item["observed_data_refs"]:
-                            if len(to_ids) > 0:
-                                for to_id in to_ids:
-                                    self.import_sighting(
-                                        item, observed_data_ref, to_id, update
-                                    )
-                elif item["type"] == "label":
-                    stix_ids = self.opencti.get_attribute_in_extension("stix_ids", item)
-                    self.opencti.label.create(
-                        stix_id=item["id"],
-                        value=item["value"],
-                        color=item["color"],
-                        x_opencti_stix_ids=stix_ids,
-                        update=update,
-                    )
-                elif item["type"] == "vocabulary":
-                    stix_ids = self.opencti.get_attribute_in_extension("stix_ids", item)
-                    self.opencti.vocabulary.create(
-                        stix_id=item["id"],
-                        name=item["name"],
-                        category=item["category"],
-                        description=(
-                            item["description"] if "description" in item else None
-                        ),
-                        aliases=item["aliases"] if "aliases" in item else None,
-                        x_opencti_stix_ids=stix_ids,
-                        update=update,
-                    )
-                elif item["type"] == "external-reference":
-                    stix_ids = self.opencti.get_attribute_in_extension("stix_ids", item)
-                    self.opencti.external_reference.create(
-                        stix_id=item["id"],
-                        source_name=(
-                            item["source_name"] if "source_name" in item else None
-                        ),
-                        url=item["url"] if "url" in item else None,
-                        external_id=(
-                            item["external_id"] if "external_id" in item else None
-                        ),
-                        description=(
-                            item["description"] if "description" in item else None
-                        ),
-                        x_opencti_stix_ids=stix_ids,
-                        update=update,
-                    )
-                elif item["type"] == "kill-chain-phase":
-                    stix_ids = self.opencti.get_attribute_in_extension("stix_ids", item)
-                    self.opencti.kill_chain_phase.create(
-                        stix_id=item["id"],
-                        kill_chain_name=item["kill_chain_name"],
-                        phase_name=item["phase_name"],
-                        x_opencti_order=item["order"] if "order" in item else 0,
-                        x_opencti_stix_ids=stix_ids,
-                        update=update,
-                    )
-                elif StixCyberObservableTypes.has_value(item["type"]):
-                    if types is None or len(types) == 0:
-                        self.import_observable(item, update, types)
-                    elif item["type"] in types or "observable" in types:
-                        self.import_observable(item, update, types)
-                else:
-                    # Check the scope
-                    if (
-                        item["type"] == "marking-definition"
-                        or types is None
-                        or len(types) == 0
-                    ):
-                        self.import_object(item, update, types)
-                    # Handle identity & location if part of the scope
-                    elif item["type"] in types:
-                        self.import_object(item, update, types)
-                    else:
-                        # Specific OpenCTI scopes
-                        if item["type"] == "identity":
-                            if "identity_class" in item:
-                                if ("class" in types or "sector" in types) and item[
-                                    "identity_class"
-                                ] == "class":
-                                    self.import_object(item, update, types)
-                                elif item["identity_class"] in types:
-                                    self.import_object(item, update, types)
-                        elif item["type"] == "location":
-                            if "x_opencti_location_type" in item:
-                                if item["x_opencti_location_type"].lower() in types:
-                                    self.import_object(item, update, types)
-                            elif (
-                                self.opencti.get_attribute_in_extension(
-                                    "location_type", item
-                                )
-                                is not None
-                            ):
-                                if (
-                                    self.opencti.get_attribute_in_extension(
-                                        "location_type", item
-                                    ).lower()
-                                    in types
-                                ):
-                                    self.import_object(item, update, types)
+                self.import_item(item, update, types, 0, work_id)
                 imported_elements.append({"id": item["id"], "type": item["type"]})
 
         return imported_elements
 
     @staticmethod
     def put_attribute_in_extension(
         object, extension_id, key, value, multiple=False
```

### Comparing `pycti-6.1.4/pycti/utils/opencti_stix2_splitter.py` & `pycti-6.1.5/pycti/utils/opencti_stix2_splitter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import json
 import re
 import uuid
+from typing import Tuple
+
+from typing_extensions import deprecated
 
 MITRE_X_CAPEC = (
     "x_capec_*"  # https://github.com/mitre-attack/attack-stix-data/issues/34
 )
 unsupported_ref_patterns = [MITRE_X_CAPEC]
 
 
@@ -54,24 +57,18 @@
                         nb_deps += self.enlist_element(value, raw_data)
         # Get the final dep counting and add in cache
         item["nb_deps"] = nb_deps
         self.elements.append(item)
         self.cache_index[item_id] = item  # Put in cache
         return nb_deps
 
-    def split_bundle(self, bundle, use_json=True, event_version=None) -> list:
-        """splits a valid stix2 bundle into a list of bundles
-        :param bundle: valid stix2 bundle
-        :type bundle:
-        :param use_json: is JSON?
-        :type use_json:
-        :raises Exception: if data is not valid JSON
-        :return: returns a list of bundles
-        :rtype: list
-        """
+    def split_bundle_with_expectations(
+        self, bundle, use_json=True, event_version=None
+    ) -> Tuple[int, list]:
+        """splits a valid stix2 bundle into a list of bundles"""
         if use_json:
             try:
                 bundle_data = json.loads(bundle)
             except:
                 raise Exception("File data is not a valid JSON")
         else:
             bundle_data = bundle
@@ -92,24 +89,39 @@
         # Build the bundles
         bundles = []
 
         def by_dep_size(elem):
             return elem["nb_deps"]
 
         self.elements.sort(key=by_dep_size)
-        for entity in self.elements:
+
+        elements_with_deps = list(
+            map(lambda e: {"nb_deps": e["nb_deps"], "elements": [e]}, self.elements)
+        )
+
+        number_expectations = 0
+        for entity in elements_with_deps:
+            number_expectations += len(entity["elements"])
             bundles.append(
                 self.stix2_create_bundle(
                     bundle_data["id"],
                     entity["nb_deps"],
-                    [entity],
+                    entity["elements"],
                     use_json,
                     event_version,
                 )
             )
+
+        return number_expectations, bundles
+
+    @deprecated("Use split_bundle_with_expectations instead")
+    def split_bundle(self, bundle, use_json=True, event_version=None) -> list:
+        expectations, bundles = self.split_bundle_with_expectations(
+            bundle, use_json, event_version
+        )
         return bundles
 
     @staticmethod
     def stix2_create_bundle(bundle_id, bundle_seq, items, use_json, event_version=None):
         """create a stix2 bundle with items
 
         :param items: valid stix2 items
```

### Comparing `pycti-6.1.4/pycti/utils/opencti_stix2_update.py` & `pycti-6.1.5/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti/utils/opencti_stix2_utils.py` & `pycti-6.1.5/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti.egg-info/PKG-INFO` & `pycti-6.1.5/pycti.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.4
+Version: 6.1.5
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,25 +18,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datefinder~=0.7.3
-Requires-Dist: pika~=1.3.1
+Requires-Dist: pika~=1.3.0
 Requires-Dist: python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
-Requires-Dist: prometheus-client~=0.20.0
 Requires-Dist: python-magic-bin~=0.4.14; sys_platform == "win32"
 Requires-Dist: python_json_logger~=2.0.4
-Requires-Dist: pyyaml~=6.0
-Requires-Dist: requests~=2.31.0
-Requires-Dist: setuptools~=69.5.1
+Requires-Dist: PyYAML~=6.0
+Requires-Dist: requests~=2.32.2
+Requires-Dist: setuptools~=70.0.0
+Requires-Dist: cachetools~=5.3.0
+Requires-Dist: prometheus-client~=0.20.0
+Requires-Dist: opentelemetry-api~=1.22.0
+Requires-Dist: opentelemetry-sdk~=1.22.0
 Requires-Dist: filigran-sseclient~=1.0.0
 Requires-Dist: stix2~=3.0.1
-Requires-Dist: cachetools~=5.3.0
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
 Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 Requires-Dist: pytest-cases~=3.8.0; extra == "dev"
```

### Comparing `pycti-6.1.4/pycti.egg-info/SOURCES.txt` & `pycti-6.1.5/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/pycti.egg-info/requires.txt` & `pycti-6.1.5/pycti.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 datefinder~=0.7.3
-pika~=1.3.1
-prometheus-client~=0.20.0
+pika~=1.3.0
 python_json_logger~=2.0.4
-pyyaml~=6.0
-requests~=2.31.0
-setuptools~=69.5.1
+PyYAML~=6.0
+requests~=2.32.2
+setuptools~=70.0.0
+cachetools~=5.3.0
+prometheus-client~=0.20.0
+opentelemetry-api~=1.22.0
+opentelemetry-sdk~=1.22.0
 filigran-sseclient~=1.0.0
 stix2~=3.0.1
-cachetools~=5.3.0
 
 [:sys_platform == "linux" or sys_platform == "darwin"]
 python-magic~=0.4.27
 
 [:sys_platform == "win32"]
 python-magic-bin~=0.4.14
```

### Comparing `pycti-6.1.4/pyproject.toml` & `pycti-6.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-6.1.4/setup.cfg` & `pycti-6.1.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -29,25 +29,27 @@
 	pycti.api
 	pycti.connector
 	pycti.entities
 	pycti.utils
 include_package_data = True
 install_requires = 
 	datefinder~=0.7.3
-	pika~=1.3.1
-	python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
-	prometheus-client~=0.20.0
-	python-magic-bin~=0.4.14; sys_platform == "win32"
+	pika~=1.3.0
+	python-magic~=0.4.27; sys_platform == 'linux' or sys_platform == 'darwin'
+	python-magic-bin~=0.4.14; sys_platform == 'win32'
 	python_json_logger~=2.0.4
-	pyyaml~=6.0
-	requests~=2.31.0
-	setuptools~=69.5.1
+	PyYAML~=6.0
+	requests~=2.32.2
+	setuptools~=70.0.0
+	cachetools~=5.3.0
+	prometheus-client~=0.20.0
+	opentelemetry-api~=1.22.0
+	opentelemetry-sdk~=1.22.0
 	filigran-sseclient~=1.0.0
 	stix2~=3.0.1
-	cachetools~=5.3.0
 
 [options.extras_require]
 dev = 
 	black~=24.4.0
 	build~=1.2.1
 	isort~=5.13.0
 	types-pytz~=2024.1.0.20240203
```

