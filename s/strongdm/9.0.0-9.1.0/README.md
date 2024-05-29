# Comparing `tmp/strongdm-9.0.0.zip` & `tmp/strongdm-9.1.0.zip`

## zipinfo {}

```diff
@@ -1,140 +1,140 @@
-Zip file size: 398412 bytes, number of entries: 138
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:53 strongdm-9.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:53 strongdm-9.0.0/strongdm/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:53 strongdm-9.0.0/strongdm.egg-info/
--rw-r--r--  2.0 unx     1908 b- defN 24-May-22 22:53 strongdm-9.0.0/setup.py
--rw-r--r--  2.0 unx     2875 b- defN 24-May-22 22:53 strongdm-9.0.0/README.md
--rw-r--r--  2.0 unx    11342 b- defN 24-May-22 22:53 strongdm-9.0.0/LICENSE
--rw-r--r--  2.0 unx     3599 b- defN 24-May-22 22:53 strongdm-9.0.0/PKG-INFO
--rw-r--r--  2.0 unx       38 b- defN 24-May-22 22:53 strongdm-9.0.0/setup.cfg
--rw-r--r--  2.0 unx     2196 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/errors.py
--rw-r--r--  2.0 unx     8404 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflow_steps_pb2_grpc.py
--rw-r--r--  2.0 unx     3424 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/remote_identities_history_pb2_grpc.py
--rw-r--r--  2.0 unx    17204 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_approvers_pb2.py
--rw-r--r--  2.0 unx   452619 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/plumbing.py
--rw-r--r--  2.0 unx     8646 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/access_requests_history_pb2.py
--rw-r--r--  2.0 unx     8983 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/access_request_events_history_pb2.py
--rw-r--r--  2.0 unx     8773 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_resources_history_pb2.py
--rw-r--r--  2.0 unx    19580 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/identity_aliases_pb2.py
--rw-r--r--  2.0 unx     3479 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_assignments_pb2_grpc.py
--rw-r--r--  2.0 unx     7932 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/peering_groups_pb2_grpc.py
--rw-r--r--  2.0 unx     8132 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/resources_history_pb2.py
--rw-r--r--  2.0 unx     3320 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/organization_history_pb2_grpc.py
--rw-r--r--  2.0 unx    11611 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/control_panel_pb2.py
--rw-r--r--  2.0 unx    17173 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/peering_group_resources_pb2.py
--rw-r--r--  2.0 unx    16079 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_roles_pb2.py
--rw-r--r--  2.0 unx    15576 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/access_requests_pb2.py
--rw-r--r--  2.0 unx     3505 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_approvers_history_pb2_grpc.py
--rw-r--r--  2.0 unx     7818 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/roles_history_pb2.py
--rw-r--r--  2.0 unx   891281 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/drivers_pb2.py
--rw-r--r--  2.0 unx     9837 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/nodes_pb2_grpc.py
--rw-r--r--  2.0 unx     5092 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/activities_pb2_grpc.py
--rw-r--r--  2.0 unx    18385 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/roles_pb2.py
--rw-r--r--  2.0 unx    19200 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/queries_pb2.py
--rw-r--r--  2.0 unx     3198 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/accounts_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8674 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/remote_identities_history_pb2.py
--rw-r--r--  2.0 unx    94807 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/secret_store_types_pb2.py
--rw-r--r--  2.0 unx    22207 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/resources_pb2.py
--rw-r--r--  2.0 unx     7818 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/nodes_history_pb2.py
--rw-r--r--  2.0 unx    19883 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/remote_identities_pb2.py
--rw-r--r--  2.0 unx     8550 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_grants_history_pb2.py
--rw-r--r--  2.0 unx    29937 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/nodes_pb2.py
--rw-r--r--  2.0 unx     8396 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/identity_sets_history_pb2.py
--rw-r--r--  2.0 unx    14958 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/options_pb2.py
--rw-r--r--  2.0 unx     3259 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflows_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8071 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_roles_pb2_grpc.py
--rw-r--r--  2.0 unx     9042 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/roles_pb2_grpc.py
--rw-r--r--  2.0 unx    20009 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflows_pb2.py
--rw-r--r--  2.0 unx     8808 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_approvers_history_pb2.py
--rw-r--r--  2.0 unx     3465 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflows_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8546 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/peering_group_resources_pb2_grpc.py
--rw-r--r--  2.0 unx    16300 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/activities_pb2.py
--rw-r--r--  2.0 unx     9813 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/identity_aliases_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/secret_store_types_pb2_grpc.py
--rw-r--r--  2.0 unx     3557 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/access_request_events_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8320 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/replays_pb2.py
--rw-r--r--  2.0 unx    17034 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/organization_history_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/options_pb2_grpc.py
--rw-r--r--  2.0 unx     8571 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/identity_aliases_history_pb2.py
--rw-r--r--  2.0 unx     3295 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/role_resources_pb2_grpc.py
--rw-r--r--  2.0 unx    16005 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/secret_store_healths_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/spec_pb2_grpc.py
--rw-r--r--  2.0 unx    16584 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_grants_pb2.py
--rw-r--r--  2.0 unx     9376 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/secret_stores_pb2_grpc.py
--rw-r--r--  2.0 unx     3111 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx     9113 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflow_steps_history_pb2.py
--rw-r--r--  2.0 unx     8167 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/peering_group_peers_pb2_grpc.py
--rw-r--r--  2.0 unx     9051 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/remote_identity_groups_history_pb2.py
--rw-r--r--  2.0 unx     3322 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/identity_sets_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3417 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/access_requests_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8478 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/role_resources_history_pb2.py
--rw-r--r--  2.0 unx     3111 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/nodes_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8901 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_resources_pb2.py
--rw-r--r--  2.0 unx     9162 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/identity_sets_pb2.py
--rw-r--r--  2.0 unx   218807 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/svc.py
--rw-r--r--  2.0 unx     8412 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/secret_stores_history_pb2.py
--rw-r--r--  2.0 unx     8901 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_attachments_history_pb2.py
--rw-r--r--  2.0 unx    15880 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/spec_pb2.py
--rw-r--r--  2.0 unx     3353 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_grants_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3361 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/replays_pb2_grpc.py
--rw-r--r--  2.0 unx     3396 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/identity_aliases_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8961 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_assignments_history_pb2.py
--rwxr-xr-x  2.0 unx    18845 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/constants.py
--rw-r--r--  2.0 unx     9960 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflows_pb2_grpc.py
--rw-r--r--  2.0 unx     9995 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/remote_identity_groups_pb2.py
--rw-r--r--  2.0 unx     7340 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_assignments_pb2.py
--rw-r--r--  2.0 unx     3434 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8140 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflows_history_pb2.py
--rw-r--r--  2.0 unx    20122 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflows_pb2.py
--rw-r--r--  2.0 unx     3390 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx     9758 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/accounts_pb2_grpc.py
--rw-r--r--  2.0 unx    29136 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/client.py
--rw-r--r--  2.0 unx      808 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/__init__.py
--rw-r--r--  2.0 unx     3420 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/queries_pb2_grpc.py
--rw-r--r--  2.0 unx    17037 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_attachments_pb2.py
--rw-r--r--  2.0 unx    12455 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/resources_pb2_grpc.py
--rw-r--r--  2.0 unx    18708 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflow_approvers_pb2.py
--rw-r--r--  2.0 unx    16423 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/peering_group_peers_pb2.py
--rw-r--r--  2.0 unx     8138 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/accounts_history_pb2.py
--rw-r--r--  2.0 unx     3322 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/secret_stores_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3561 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_assignments_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8255 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/peering_group_nodes_pb2_grpc.py
--rw-r--r--  2.0 unx     8708 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py
--rw-r--r--  2.0 unx     3223 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx     6598 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/control_panel_pb2_grpc.py
--rw-r--r--  2.0 unx     9416 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflow_approvers_history_pb2.py
--rw-r--r--  2.0 unx     3592 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
--rw-r--r--  2.0 unx    15297 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/peering_groups_pb2.py
--rw-r--r--  2.0 unx     8102 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_attachments_pb2_grpc.py
--rw-r--r--  2.0 unx     3350 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/role_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx     4600 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/tags_pb2.py
--rw-r--r--  2.0 unx     6849 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/secret_store_healths_pb2_grpc.py
--rw-r--r--  2.0 unx     9665 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflows_pb2_grpc.py
--rw-r--r--  2.0 unx     7476 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/role_resources_pb2.py
--rw-r--r--  2.0 unx    17070 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflow_steps_pb2.py
--rw-r--r--  2.0 unx   815657 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/models.py
--rw-r--r--  2.0 unx     9790 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/remote_identities_pb2_grpc.py
--rw-r--r--  2.0 unx    29031 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/accounts_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/drivers_pb2_grpc.py
--rw-r--r--  2.0 unx     8792 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflows_history_pb2.py
--rw-r--r--  2.0 unx    17214 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/secret_stores_pb2.py
--rw-r--r--  2.0 unx     8506 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_roles_history_pb2.py
--rw-r--r--  2.0 unx    16380 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/peering_group_nodes_pb2.py
--rw-r--r--  2.0 unx     7980 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_grants_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/tags_pb2_grpc.py
--rw-r--r--  2.0 unx     3493 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_attachments_history_pb2_grpc.py
--rw-r--r--  2.0 unx     5700 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/identity_sets_pb2_grpc.py
--rw-r--r--  2.0 unx     8396 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_permissions_pb2.py
--rw-r--r--  2.0 unx     6176 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/remote_identity_groups_pb2_grpc.py
--rw-r--r--  2.0 unx     3180 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/access_requests_pb2_grpc.py
--rw-r--r--  2.0 unx     8165 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/workflow_approvers_pb2_grpc.py
--rw-r--r--  2.0 unx     3561 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3704 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3388 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_resources_pb2_grpc.py
--rw-r--r--  2.0 unx     3470 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm/account_permissions_pb2_grpc.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm.egg-info/top_level.txt
--rw-r--r--  2.0 unx       50 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm.egg-info/requires.txt
--rw-r--r--  2.0 unx     4703 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     3599 b- defN 24-May-22 22:53 strongdm-9.0.0/strongdm.egg-info/PKG-INFO
-138 files, 3604241 bytes uncompressed, 374532 bytes compressed:  89.6%
+Zip file size: 400003 bytes, number of entries: 138
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 20:44 strongdm-9.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 20:44 strongdm-9.1.0/strongdm/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 20:44 strongdm-9.1.0/strongdm.egg-info/
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-29 20:44 strongdm-9.1.0/setup.py
+-rw-r--r--  2.0 unx     2875 b- defN 24-May-29 20:44 strongdm-9.1.0/README.md
+-rw-r--r--  2.0 unx    11342 b- defN 24-May-29 20:44 strongdm-9.1.0/LICENSE
+-rw-r--r--  2.0 unx     3599 b- defN 24-May-29 20:44 strongdm-9.1.0/PKG-INFO
+-rw-r--r--  2.0 unx       38 b- defN 24-May-29 20:44 strongdm-9.1.0/setup.cfg
+-rw-r--r--  2.0 unx     2196 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/errors.py
+-rw-r--r--  2.0 unx     8404 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflow_steps_pb2_grpc.py
+-rw-r--r--  2.0 unx     3424 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/remote_identities_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    17204 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_approvers_pb2.py
+-rw-r--r--  2.0 unx   456475 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/plumbing.py
+-rw-r--r--  2.0 unx     8646 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/access_requests_history_pb2.py
+-rw-r--r--  2.0 unx     8983 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/access_request_events_history_pb2.py
+-rw-r--r--  2.0 unx     8773 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_resources_history_pb2.py
+-rw-r--r--  2.0 unx    19580 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/identity_aliases_pb2.py
+-rw-r--r--  2.0 unx     3479 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_assignments_pb2_grpc.py
+-rw-r--r--  2.0 unx     7932 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/peering_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx     8132 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/resources_history_pb2.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/organization_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    11611 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/control_panel_pb2.py
+-rw-r--r--  2.0 unx    17173 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/peering_group_resources_pb2.py
+-rw-r--r--  2.0 unx    16079 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_roles_pb2.py
+-rw-r--r--  2.0 unx    15576 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/access_requests_pb2.py
+-rw-r--r--  2.0 unx     3505 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_approvers_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     7818 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/roles_history_pb2.py
+-rw-r--r--  2.0 unx   891281 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/drivers_pb2.py
+-rw-r--r--  2.0 unx     9837 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     5092 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/activities_pb2_grpc.py
+-rw-r--r--  2.0 unx    18385 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/roles_pb2.py
+-rw-r--r--  2.0 unx    19200 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/queries_pb2.py
+-rw-r--r--  2.0 unx     3198 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/accounts_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8674 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/remote_identities_history_pb2.py
+-rw-r--r--  2.0 unx    94807 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/secret_store_types_pb2.py
+-rw-r--r--  2.0 unx    22207 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/resources_pb2.py
+-rw-r--r--  2.0 unx     7818 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/nodes_history_pb2.py
+-rw-r--r--  2.0 unx    19883 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/remote_identities_pb2.py
+-rw-r--r--  2.0 unx     8550 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_grants_history_pb2.py
+-rw-r--r--  2.0 unx    29937 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/nodes_pb2.py
+-rw-r--r--  2.0 unx     8396 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/identity_sets_history_pb2.py
+-rw-r--r--  2.0 unx    14958 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/options_pb2.py
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflows_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8071 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_roles_pb2_grpc.py
+-rw-r--r--  2.0 unx     9042 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/roles_pb2_grpc.py
+-rw-r--r--  2.0 unx    20009 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflows_pb2.py
+-rw-r--r--  2.0 unx     8808 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_approvers_history_pb2.py
+-rw-r--r--  2.0 unx     3465 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflows_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8546 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/peering_group_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    16300 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/activities_pb2.py
+-rw-r--r--  2.0 unx     9813 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/identity_aliases_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/secret_store_types_pb2_grpc.py
+-rw-r--r--  2.0 unx     3557 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/access_request_events_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8320 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/replays_pb2.py
+-rw-r--r--  2.0 unx    17034 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/organization_history_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/options_pb2_grpc.py
+-rw-r--r--  2.0 unx     8571 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/identity_aliases_history_pb2.py
+-rw-r--r--  2.0 unx     3295 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/role_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    16005 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/secret_store_healths_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/spec_pb2_grpc.py
+-rw-r--r--  2.0 unx    16584 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_grants_pb2.py
+-rw-r--r--  2.0 unx     9376 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/secret_stores_pb2_grpc.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9113 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflow_steps_history_pb2.py
+-rw-r--r--  2.0 unx     8167 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/peering_group_peers_pb2_grpc.py
+-rw-r--r--  2.0 unx     9051 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/remote_identity_groups_history_pb2.py
+-rw-r--r--  2.0 unx     3322 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/identity_sets_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3417 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/access_requests_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8478 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/role_resources_history_pb2.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/nodes_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8901 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_resources_pb2.py
+-rw-r--r--  2.0 unx    18450 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/identity_sets_pb2.py
+-rw-r--r--  2.0 unx   222641 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/svc.py
+-rw-r--r--  2.0 unx     8412 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/secret_stores_history_pb2.py
+-rw-r--r--  2.0 unx     8901 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_attachments_history_pb2.py
+-rw-r--r--  2.0 unx    15880 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/spec_pb2.py
+-rw-r--r--  2.0 unx     3353 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_grants_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3361 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/replays_pb2_grpc.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/identity_aliases_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8961 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_assignments_history_pb2.py
+-rwxr-xr-x  2.0 unx    18845 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/constants.py
+-rw-r--r--  2.0 unx     9960 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflows_pb2_grpc.py
+-rw-r--r--  2.0 unx     9995 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/remote_identity_groups_pb2.py
+-rw-r--r--  2.0 unx     7340 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_assignments_pb2.py
+-rw-r--r--  2.0 unx     3434 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8140 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflows_history_pb2.py
+-rw-r--r--  2.0 unx    20122 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflows_pb2.py
+-rw-r--r--  2.0 unx     3390 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9758 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/accounts_pb2_grpc.py
+-rw-r--r--  2.0 unx    29136 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/client.py
+-rw-r--r--  2.0 unx      808 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/__init__.py
+-rw-r--r--  2.0 unx     3420 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/queries_pb2_grpc.py
+-rw-r--r--  2.0 unx    17037 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_attachments_pb2.py
+-rw-r--r--  2.0 unx    12455 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    18708 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflow_approvers_pb2.py
+-rw-r--r--  2.0 unx    16423 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/peering_group_peers_pb2.py
+-rw-r--r--  2.0 unx     8138 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/accounts_history_pb2.py
+-rw-r--r--  2.0 unx     3322 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/secret_stores_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3561 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_assignments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8255 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/peering_group_nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     8708 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflow_approvers_pb2_grpc.py
+-rw-r--r--  2.0 unx     3223 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     6598 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/control_panel_pb2_grpc.py
+-rw-r--r--  2.0 unx     9416 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflow_approvers_history_pb2.py
+-rw-r--r--  2.0 unx     3592 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    15297 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/peering_groups_pb2.py
+-rw-r--r--  2.0 unx     8102 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_attachments_pb2_grpc.py
+-rw-r--r--  2.0 unx     3350 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/role_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     4600 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/tags_pb2.py
+-rw-r--r--  2.0 unx     6849 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/secret_store_healths_pb2_grpc.py
+-rw-r--r--  2.0 unx     9665 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflows_pb2_grpc.py
+-rw-r--r--  2.0 unx     7476 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/role_resources_pb2.py
+-rw-r--r--  2.0 unx    17070 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflow_steps_pb2.py
+-rw-r--r--  2.0 unx   819478 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/models.py
+-rw-r--r--  2.0 unx     9790 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/remote_identities_pb2_grpc.py
+-rw-r--r--  2.0 unx    29031 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/accounts_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/drivers_pb2_grpc.py
+-rw-r--r--  2.0 unx     8792 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflows_history_pb2.py
+-rw-r--r--  2.0 unx    17214 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/secret_stores_pb2.py
+-rw-r--r--  2.0 unx     8506 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_roles_history_pb2.py
+-rw-r--r--  2.0 unx    16380 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/peering_group_nodes_pb2.py
+-rw-r--r--  2.0 unx     7980 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_grants_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/tags_pb2_grpc.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_attachments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9589 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/identity_sets_pb2_grpc.py
+-rw-r--r--  2.0 unx     8396 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_permissions_pb2.py
+-rw-r--r--  2.0 unx     6176 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/remote_identity_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx     3180 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/access_requests_pb2_grpc.py
+-rw-r--r--  2.0 unx     8165 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/workflow_approvers_pb2_grpc.py
+-rw-r--r--  2.0 unx     3561 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3704 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3388 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx     3470 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm/account_permissions_pb2_grpc.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       50 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm.egg-info/requires.txt
+-rw-r--r--  2.0 unx     4703 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     3599 b- defN 24-May-29 20:44 strongdm-9.1.0/strongdm.egg-info/PKG-INFO
+138 files, 3628929 bytes uncompressed, 376123 bytes compressed:  89.7%
```

## zipnote {}

```diff
@@ -1,415 +1,415 @@
-Filename: strongdm-9.0.0/
+Filename: strongdm-9.1.0/
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/
+Filename: strongdm-9.1.0/strongdm/
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm.egg-info/
+Filename: strongdm-9.1.0/strongdm.egg-info/
 Comment: 
 
-Filename: strongdm-9.0.0/setup.py
+Filename: strongdm-9.1.0/setup.py
 Comment: 
 
-Filename: strongdm-9.0.0/README.md
+Filename: strongdm-9.1.0/README.md
 Comment: 
 
-Filename: strongdm-9.0.0/LICENSE
+Filename: strongdm-9.1.0/LICENSE
 Comment: 
 
-Filename: strongdm-9.0.0/PKG-INFO
+Filename: strongdm-9.1.0/PKG-INFO
 Comment: 
 
-Filename: strongdm-9.0.0/setup.cfg
+Filename: strongdm-9.1.0/setup.cfg
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/errors.py
+Filename: strongdm-9.1.0/strongdm/errors.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflow_steps_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/approval_workflow_steps_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/remote_identities_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/remote_identities_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_approvers_pb2.py
+Filename: strongdm-9.1.0/strongdm/workflow_approvers_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/plumbing.py
+Filename: strongdm-9.1.0/strongdm/plumbing.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/access_requests_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/access_requests_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/access_request_events_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/access_request_events_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_resources_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/account_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/identity_aliases_pb2.py
+Filename: strongdm-9.1.0/strongdm/identity_aliases_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_assignments_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/workflow_assignments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/peering_groups_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/peering_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/resources_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/organization_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/organization_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/control_panel_pb2.py
+Filename: strongdm-9.1.0/strongdm/control_panel_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/peering_group_resources_pb2.py
+Filename: strongdm-9.1.0/strongdm/peering_group_resources_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_roles_pb2.py
+Filename: strongdm-9.1.0/strongdm/workflow_roles_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/access_requests_pb2.py
+Filename: strongdm-9.1.0/strongdm/access_requests_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_approvers_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/workflow_approvers_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/roles_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/drivers_pb2.py
+Filename: strongdm-9.1.0/strongdm/drivers_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/nodes_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/activities_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/activities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/roles_pb2.py
+Filename: strongdm-9.1.0/strongdm/roles_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/queries_pb2.py
+Filename: strongdm-9.1.0/strongdm/queries_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/accounts_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/accounts_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/remote_identities_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/remote_identities_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/secret_store_types_pb2.py
+Filename: strongdm-9.1.0/strongdm/secret_store_types_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/resources_pb2.py
+Filename: strongdm-9.1.0/strongdm/resources_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/nodes_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/nodes_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/remote_identities_pb2.py
+Filename: strongdm-9.1.0/strongdm/remote_identities_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_grants_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/account_grants_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/nodes_pb2.py
+Filename: strongdm-9.1.0/strongdm/nodes_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/identity_sets_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/identity_sets_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/options_pb2.py
+Filename: strongdm-9.1.0/strongdm/options_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflows_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/workflows_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_roles_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/workflow_roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/roles_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflows_pb2.py
+Filename: strongdm-9.1.0/strongdm/approval_workflows_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_approvers_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/workflow_approvers_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflows_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/approval_workflows_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/peering_group_resources_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/peering_group_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/activities_pb2.py
+Filename: strongdm-9.1.0/strongdm/activities_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/identity_aliases_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/identity_aliases_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/secret_store_types_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/secret_store_types_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/access_request_events_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/access_request_events_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/replays_pb2.py
+Filename: strongdm-9.1.0/strongdm/replays_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/organization_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/organization_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/options_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/options_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/identity_aliases_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/identity_aliases_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/role_resources_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/role_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/secret_store_healths_pb2.py
+Filename: strongdm-9.1.0/strongdm/secret_store_healths_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/spec_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/spec_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_grants_pb2.py
+Filename: strongdm-9.1.0/strongdm/account_grants_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/secret_stores_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/secret_stores_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/roles_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflow_steps_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/approval_workflow_steps_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/peering_group_peers_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/peering_group_peers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/remote_identity_groups_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/remote_identity_groups_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/identity_sets_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/identity_sets_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/access_requests_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/access_requests_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/role_resources_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/role_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/nodes_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/nodes_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_resources_pb2.py
+Filename: strongdm-9.1.0/strongdm/account_resources_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/identity_sets_pb2.py
+Filename: strongdm-9.1.0/strongdm/identity_sets_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/svc.py
+Filename: strongdm-9.1.0/strongdm/svc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/secret_stores_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/secret_stores_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_attachments_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/account_attachments_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/spec_pb2.py
+Filename: strongdm-9.1.0/strongdm/spec_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_grants_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/account_grants_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/replays_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/replays_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/identity_aliases_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/identity_aliases_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_assignments_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/workflow_assignments_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/constants.py
+Filename: strongdm-9.1.0/strongdm/constants.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflows_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/approval_workflows_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/remote_identity_groups_pb2.py
+Filename: strongdm-9.1.0/strongdm/remote_identity_groups_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_assignments_pb2.py
+Filename: strongdm-9.1.0/strongdm/workflow_assignments_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_resources_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/account_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflows_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/workflows_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflows_pb2.py
+Filename: strongdm-9.1.0/strongdm/workflows_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_roles_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/workflow_roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/accounts_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/accounts_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/client.py
+Filename: strongdm-9.1.0/strongdm/client.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/__init__.py
+Filename: strongdm-9.1.0/strongdm/__init__.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/queries_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/queries_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_attachments_pb2.py
+Filename: strongdm-9.1.0/strongdm/account_attachments_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/resources_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflow_approvers_pb2.py
+Filename: strongdm-9.1.0/strongdm/approval_workflow_approvers_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/peering_group_peers_pb2.py
+Filename: strongdm-9.1.0/strongdm/peering_group_peers_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/accounts_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/accounts_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/secret_stores_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/secret_stores_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_assignments_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/workflow_assignments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/peering_group_nodes_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/peering_group_nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/approval_workflow_approvers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/resources_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/control_panel_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/control_panel_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflow_approvers_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/approval_workflow_approvers_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/peering_groups_pb2.py
+Filename: strongdm-9.1.0/strongdm/peering_groups_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_attachments_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/account_attachments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/role_resources_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/role_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/tags_pb2.py
+Filename: strongdm-9.1.0/strongdm/tags_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/secret_store_healths_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/secret_store_healths_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflows_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/workflows_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/role_resources_pb2.py
+Filename: strongdm-9.1.0/strongdm/role_resources_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflow_steps_pb2.py
+Filename: strongdm-9.1.0/strongdm/approval_workflow_steps_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/models.py
+Filename: strongdm-9.1.0/strongdm/models.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/remote_identities_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/remote_identities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/accounts_pb2.py
+Filename: strongdm-9.1.0/strongdm/accounts_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/drivers_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/drivers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflows_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/approval_workflows_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/secret_stores_pb2.py
+Filename: strongdm-9.1.0/strongdm/secret_stores_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_roles_history_pb2.py
+Filename: strongdm-9.1.0/strongdm/workflow_roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/peering_group_nodes_pb2.py
+Filename: strongdm-9.1.0/strongdm/peering_group_nodes_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_grants_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/account_grants_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/tags_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/tags_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_attachments_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/account_attachments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/identity_sets_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/identity_sets_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_permissions_pb2.py
+Filename: strongdm-9.1.0/strongdm/account_permissions_pb2.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/remote_identity_groups_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/remote_identity_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/access_requests_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/access_requests_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/workflow_approvers_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/workflow_approvers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_resources_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/account_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm/account_permissions_pb2_grpc.py
+Filename: strongdm-9.1.0/strongdm/account_permissions_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm.egg-info/dependency_links.txt
+Filename: strongdm-9.1.0/strongdm.egg-info/dependency_links.txt
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm.egg-info/top_level.txt
+Filename: strongdm-9.1.0/strongdm.egg-info/top_level.txt
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm.egg-info/requires.txt
+Filename: strongdm-9.1.0/strongdm.egg-info/requires.txt
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm.egg-info/SOURCES.txt
+Filename: strongdm-9.1.0/strongdm.egg-info/SOURCES.txt
 Comment: 
 
-Filename: strongdm-9.0.0/strongdm.egg-info/PKG-INFO
+Filename: strongdm-9.1.0/strongdm.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `strongdm-9.0.0/setup.py` & `strongdm-9.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 from setuptools import setup
 setup(
     name='strongdm',
     packages=['strongdm'],
-    version='9.0.0',
+    version='9.1.0',
     license='apache-2.0',
     description='strongDM SDK for the Python programming language.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='strongDM Team',
     author_email='sdk-feedback@strongdm.com',
     url='https://github.com/strongdm/strongdm-sdk-python',
     download_url=
-    'https://github.com/strongdm/strongdm-sdk-python/archive/v9.0.0.tar.gz',
+    'https://github.com/strongdm/strongdm-sdk-python/archive/v9.1.0.tar.gz',
     keywords=[
         'strongDM', 'sdm', 'api', 'automation', 'security', 'audit',
         'database', 'server', 'ssh', 'rdp'
     ],
     install_requires=[
         'grpcio>=1.42.0',
         'googleapis-common-protos>1.56.2,<2',
```

## Comparing `strongdm-9.0.0/README.md` & `strongdm-9.1.0/README.md`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/LICENSE` & `strongdm-9.1.0/LICENSE`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/PKG-INFO` & `strongdm-9.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 9.0.0
+Version: 9.1.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v9.0.0.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v9.1.0.tar.gz
 Keywords: strongDM,sdm,api,automation,security,audit,database,server,ssh,rdp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongdm-9.0.0/strongdm/errors.py` & `strongdm-9.1.0/strongdm/errors.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflow_steps_pb2_grpc.py` & `strongdm-9.1.0/strongdm/approval_workflow_steps_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/remote_identities_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/remote_identities_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_approvers_pb2.py` & `strongdm-9.1.0/strongdm/workflow_approvers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/plumbing.py` & `strongdm-9.1.0/strongdm/plumbing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5304,14 +5304,90 @@
 
 def convert_repeated_identity_set_to_porcelain(plumbings):
     return [
         convert_identity_set_to_porcelain(plumbing) for plumbing in plumbings
     ]
 
 
+def convert_identity_set_create_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.IdentitySetCreateResponse()
+    porcelain.identity_set = convert_identity_set_to_porcelain(
+        plumbing.identity_set)
+    porcelain.meta = convert_create_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_identity_set_create_response_to_plumbing(porcelain):
+    plumbing = IdentitySetCreateResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.identity_set.CopyFrom(
+        convert_identity_set_to_plumbing(porcelain.identity_set))
+    plumbing.meta.CopyFrom(
+        convert_create_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_identity_set_create_response_to_plumbing(porcelains):
+    return [
+        convert_identity_set_create_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_identity_set_create_response_to_porcelain(plumbings):
+    return [
+        convert_identity_set_create_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_identity_set_delete_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.IdentitySetDeleteResponse()
+    porcelain.meta = convert_delete_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_identity_set_delete_response_to_plumbing(porcelain):
+    plumbing = IdentitySetDeleteResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.meta.CopyFrom(
+        convert_delete_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_identity_set_delete_response_to_plumbing(porcelains):
+    return [
+        convert_identity_set_delete_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_identity_set_delete_response_to_porcelain(plumbings):
+    return [
+        convert_identity_set_delete_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
 def convert_identity_set_get_response_to_porcelain(plumbing):
     if plumbing is None:
         return None
     porcelain = models.IdentitySetGetResponse()
     porcelain.identity_set = convert_identity_set_to_porcelain(
         plumbing.identity_set)
     porcelain.meta = convert_get_response_metadata_to_porcelain(plumbing.meta)
@@ -5383,14 +5459,54 @@
 def convert_repeated_identity_set_history_to_porcelain(plumbings):
     return [
         convert_identity_set_history_to_porcelain(plumbing)
         for plumbing in plumbings
     ]
 
 
+def convert_identity_set_update_response_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.IdentitySetUpdateResponse()
+    porcelain.identity_set = convert_identity_set_to_porcelain(
+        plumbing.identity_set)
+    porcelain.meta = convert_update_response_metadata_to_porcelain(
+        plumbing.meta)
+    porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
+        plumbing.rate_limit)
+    return porcelain
+
+
+def convert_identity_set_update_response_to_plumbing(porcelain):
+    plumbing = IdentitySetUpdateResponse()
+    if porcelain is None:
+        return plumbing
+    plumbing.identity_set.CopyFrom(
+        convert_identity_set_to_plumbing(porcelain.identity_set))
+    plumbing.meta.CopyFrom(
+        convert_update_response_metadata_to_plumbing(porcelain.meta))
+    plumbing.rate_limit.CopyFrom(
+        convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    return plumbing
+
+
+def convert_repeated_identity_set_update_response_to_plumbing(porcelains):
+    return [
+        convert_identity_set_update_response_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_identity_set_update_response_to_porcelain(plumbings):
+    return [
+        convert_identity_set_update_response_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
 def convert_keyfactor_ssh_store_to_porcelain(plumbing):
     if plumbing is None:
         return None
     porcelain = models.KeyfactorSSHStore()
     porcelain.ca_file_path = (plumbing.ca_file_path)
     porcelain.certificate_file_path = (plumbing.certificate_file_path)
     porcelain.default_certificate_authority_name = (
```

## Comparing `strongdm-9.0.0/strongdm/access_requests_history_pb2.py` & `strongdm-9.1.0/strongdm/access_requests_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/access_request_events_history_pb2.py` & `strongdm-9.1.0/strongdm/access_request_events_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_resources_history_pb2.py` & `strongdm-9.1.0/strongdm/account_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/identity_aliases_pb2.py` & `strongdm-9.1.0/strongdm/identity_aliases_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_assignments_pb2_grpc.py` & `strongdm-9.1.0/strongdm/workflow_assignments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/peering_groups_pb2_grpc.py` & `strongdm-9.1.0/strongdm/peering_groups_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/resources_history_pb2.py` & `strongdm-9.1.0/strongdm/resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/organization_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/organization_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/control_panel_pb2.py` & `strongdm-9.1.0/strongdm/control_panel_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/peering_group_resources_pb2.py` & `strongdm-9.1.0/strongdm/peering_group_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_roles_pb2.py` & `strongdm-9.1.0/strongdm/workflow_roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/access_requests_pb2.py` & `strongdm-9.1.0/strongdm/access_requests_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_approvers_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/workflow_approvers_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/roles_history_pb2.py` & `strongdm-9.1.0/strongdm/roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/drivers_pb2.py` & `strongdm-9.1.0/strongdm/drivers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/nodes_pb2_grpc.py` & `strongdm-9.1.0/strongdm/nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/activities_pb2_grpc.py` & `strongdm-9.1.0/strongdm/activities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/roles_pb2.py` & `strongdm-9.1.0/strongdm/roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/queries_pb2.py` & `strongdm-9.1.0/strongdm/queries_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/accounts_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/accounts_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/remote_identities_history_pb2.py` & `strongdm-9.1.0/strongdm/remote_identities_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/secret_store_types_pb2.py` & `strongdm-9.1.0/strongdm/secret_store_types_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/resources_pb2.py` & `strongdm-9.1.0/strongdm/resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/nodes_history_pb2.py` & `strongdm-9.1.0/strongdm/nodes_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/remote_identities_pb2.py` & `strongdm-9.1.0/strongdm/remote_identities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_grants_history_pb2.py` & `strongdm-9.1.0/strongdm/account_grants_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/nodes_pb2.py` & `strongdm-9.1.0/strongdm/nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/identity_sets_history_pb2.py` & `strongdm-9.1.0/strongdm/identity_sets_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/options_pb2.py` & `strongdm-9.1.0/strongdm/options_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflows_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/workflows_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_roles_pb2_grpc.py` & `strongdm-9.1.0/strongdm/workflow_roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/roles_pb2_grpc.py` & `strongdm-9.1.0/strongdm/roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflows_pb2.py` & `strongdm-9.1.0/strongdm/approval_workflows_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_approvers_history_pb2.py` & `strongdm-9.1.0/strongdm/workflow_approvers_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflows_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/approval_workflows_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/peering_group_resources_pb2_grpc.py` & `strongdm-9.1.0/strongdm/peering_group_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/activities_pb2.py` & `strongdm-9.1.0/strongdm/activities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/identity_aliases_pb2_grpc.py` & `strongdm-9.1.0/strongdm/identity_aliases_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/secret_store_types_pb2_grpc.py` & `strongdm-9.1.0/strongdm/secret_store_types_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/access_request_events_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/access_request_events_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/replays_pb2.py` & `strongdm-9.1.0/strongdm/replays_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/organization_history_pb2.py` & `strongdm-9.1.0/strongdm/organization_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/options_pb2_grpc.py` & `strongdm-9.1.0/strongdm/options_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/identity_aliases_history_pb2.py` & `strongdm-9.1.0/strongdm/identity_aliases_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/role_resources_pb2_grpc.py` & `strongdm-9.1.0/strongdm/role_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/secret_store_healths_pb2.py` & `strongdm-9.1.0/strongdm/secret_store_healths_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/spec_pb2_grpc.py` & `strongdm-9.1.0/strongdm/spec_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_grants_pb2.py` & `strongdm-9.1.0/strongdm/account_grants_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/secret_stores_pb2_grpc.py` & `strongdm-9.1.0/strongdm/secret_stores_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/roles_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflow_steps_history_pb2.py` & `strongdm-9.1.0/strongdm/approval_workflow_steps_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/peering_group_peers_pb2_grpc.py` & `strongdm-9.1.0/strongdm/peering_group_peers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/remote_identity_groups_history_pb2.py` & `strongdm-9.1.0/strongdm/remote_identity_groups_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/identity_sets_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/identity_sets_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/access_requests_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/access_requests_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/role_resources_history_pb2.py` & `strongdm-9.1.0/strongdm/role_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/nodes_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/nodes_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_resources_pb2.py` & `strongdm-9.1.0/strongdm/account_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/svc.py` & `strongdm-9.1.0/strongdm/svc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2324,14 +2324,49 @@
      An Account's relationship to a IdentitySet is defined via IdentityAlias objects.
     See `strongdm.models.IdentitySet`.
     '''
     def __init__(self, channel, client):
         self.parent = client
         self.stub = IdentitySetsStub(channel)
 
+    def create(self, identity_set, timeout=None):
+        '''
+         Create registers a new IdentitySet.
+        '''
+        req = IdentitySetCreateRequest()
+
+        if identity_set is not None:
+            req.identity_set.CopyFrom(
+                plumbing.convert_identity_set_to_plumbing(identity_set))
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Create(
+                    req,
+                    metadata=self.parent.get_metadata('IdentitySets.Create',
+                                                      req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.IdentitySetCreateResponse()
+        resp.identity_set = plumbing.convert_identity_set_to_porcelain(
+            plumbing_response.identity_set)
+        resp.meta = plumbing.convert_create_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
     def get(self, id, timeout=None):
         '''
          Get reads one IdentitySet by ID.
         '''
         req = IdentitySetGetRequest()
         if self.parent.snapshot_datetime is not None:
             req.meta.CopyFrom(GetRequestMetadata())
@@ -2359,14 +2394,80 @@
             plumbing_response.identity_set)
         resp.meta = plumbing.convert_get_response_metadata_to_porcelain(
             plumbing_response.meta)
         resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
             plumbing_response.rate_limit)
         return resp
 
+    def update(self, identity_set, timeout=None):
+        '''
+         Update replaces all the fields of a IdentitySet by ID.
+        '''
+        req = IdentitySetUpdateRequest()
+
+        if identity_set is not None:
+            req.identity_set.CopyFrom(
+                plumbing.convert_identity_set_to_plumbing(identity_set))
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Update(
+                    req,
+                    metadata=self.parent.get_metadata('IdentitySets.Update',
+                                                      req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.IdentitySetUpdateResponse()
+        resp.identity_set = plumbing.convert_identity_set_to_porcelain(
+            plumbing_response.identity_set)
+        resp.meta = plumbing.convert_update_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
+    def delete(self, id, timeout=None):
+        '''
+         Delete removes a IdentitySet by ID.
+        '''
+        req = IdentitySetDeleteRequest()
+
+        req.id = (id)
+        tries = 0
+        plumbing_response = None
+        while True:
+            try:
+                plumbing_response = self.stub.Delete(
+                    req,
+                    metadata=self.parent.get_metadata('IdentitySets.Delete',
+                                                      req),
+                    timeout=timeout)
+            except Exception as e:
+                if self.parent.shouldRetry(tries, e):
+                    tries += 1
+                    self.parent.jitterSleep(tries)
+                    continue
+                raise plumbing.convert_error_to_porcelain(e) from e
+            break
+
+        resp = models.IdentitySetDeleteResponse()
+        resp.meta = plumbing.convert_delete_response_metadata_to_porcelain(
+            plumbing_response.meta)
+        resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
+            plumbing_response.rate_limit)
+        return resp
+
     def list(self, filter, *args, timeout=None):
         '''
          List gets a list of IdentitySets matching a given set of criteria.
         '''
         req = IdentitySetListRequest()
         req.meta.CopyFrom(ListRequestMetadata())
         if self.parent.page_limit > 0:
```

## Comparing `strongdm-9.0.0/strongdm/secret_stores_history_pb2.py` & `strongdm-9.1.0/strongdm/secret_stores_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_attachments_history_pb2.py` & `strongdm-9.1.0/strongdm/account_attachments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/spec_pb2.py` & `strongdm-9.1.0/strongdm/spec_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_grants_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/account_grants_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/replays_pb2_grpc.py` & `strongdm-9.1.0/strongdm/replays_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/identity_aliases_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/identity_aliases_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_assignments_history_pb2.py` & `strongdm-9.1.0/strongdm/workflow_assignments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/constants.py` & `strongdm-9.1.0/strongdm/constants.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflows_pb2_grpc.py` & `strongdm-9.1.0/strongdm/approval_workflows_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/remote_identity_groups_pb2.py` & `strongdm-9.1.0/strongdm/remote_identity_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_assignments_pb2.py` & `strongdm-9.1.0/strongdm/workflow_assignments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_resources_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/account_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflows_history_pb2.py` & `strongdm-9.1.0/strongdm/workflows_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflows_pb2.py` & `strongdm-9.1.0/strongdm/workflows_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_roles_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/workflow_roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/accounts_pb2_grpc.py` & `strongdm-9.1.0/strongdm/accounts_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/client.py` & `strongdm-9.1.0/strongdm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # These defaults are taken from AWS. Customization of these values
 # is a future step in the API.
 DEFAULT_MAX_RETRIES = 3
 DEFAULT_BASE_RETRY_DELAY = 0.0030  # 30 ms
 DEFAULT_MAX_RETRY_DELAY = 300  # 300 seconds
 API_VERSION = '2024-03-28'
-USER_AGENT = 'strongdm-sdk-python/9.0.0'
+USER_AGENT = 'strongdm-sdk-python/9.1.0'
 
 
 class Client:
     '''Client interacts with the strongDM API.'''
     def __init__(self,
                  api_access_key,
                  api_secret,
```

## Comparing `strongdm-9.0.0/strongdm/__init__.py` & `strongdm-9.1.0/strongdm/__init__.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/queries_pb2_grpc.py` & `strongdm-9.1.0/strongdm/queries_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_attachments_pb2.py` & `strongdm-9.1.0/strongdm/account_attachments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/resources_pb2_grpc.py` & `strongdm-9.1.0/strongdm/resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflow_approvers_pb2.py` & `strongdm-9.1.0/strongdm/approval_workflow_approvers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/peering_group_peers_pb2.py` & `strongdm-9.1.0/strongdm/peering_group_peers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/accounts_history_pb2.py` & `strongdm-9.1.0/strongdm/accounts_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/secret_stores_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/secret_stores_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_assignments_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/workflow_assignments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/peering_group_nodes_pb2_grpc.py` & `strongdm-9.1.0/strongdm/peering_group_nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py` & `strongdm-9.1.0/strongdm/approval_workflow_approvers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/resources_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/control_panel_pb2_grpc.py` & `strongdm-9.1.0/strongdm/control_panel_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflow_approvers_history_pb2.py` & `strongdm-9.1.0/strongdm/approval_workflow_approvers_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/approval_workflow_steps_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/peering_groups_pb2.py` & `strongdm-9.1.0/strongdm/peering_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_attachments_pb2_grpc.py` & `strongdm-9.1.0/strongdm/account_attachments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/role_resources_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/role_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/tags_pb2.py` & `strongdm-9.1.0/strongdm/tags_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/secret_store_healths_pb2_grpc.py` & `strongdm-9.1.0/strongdm/secret_store_healths_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflows_pb2_grpc.py` & `strongdm-9.1.0/strongdm/workflows_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/role_resources_pb2.py` & `strongdm-9.1.0/strongdm/role_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflow_steps_pb2.py` & `strongdm-9.1.0/strongdm/approval_workflow_steps_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/models.py` & `strongdm-9.1.0/strongdm/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10838,14 +10838,110 @@
     def from_dict(cls, d):
         return cls(
             id=d.get('id'),
             name=d.get('name'),
         )
 
 
+class IdentitySetCreateResponse:
+    '''
+         IdentitySetCreateResponse reports how the IdentitySets were created in the system. It can
+     communicate partial successes or failures.
+    '''
+    __slots__ = [
+        'identity_set',
+        'meta',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        identity_set=None,
+        meta=None,
+        rate_limit=None,
+    ):
+        self.identity_set = identity_set if identity_set is not None else None
+        '''
+         The created IdentitySet.
+        '''
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.IdentitySetCreateResponse ' + \
+            'identity_set: ' + repr(self.identity_set) + ' ' +\
+            'meta: ' + repr(self.meta) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'identity_set': self.identity_set,
+            'meta': self.meta,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            identity_set=d.get('identity_set'),
+            meta=d.get('meta'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
+class IdentitySetDeleteResponse:
+    '''
+         IdentitySetDeleteResponse returns information about a IdentitySet that was deleted.
+    '''
+    __slots__ = [
+        'meta',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        meta=None,
+        rate_limit=None,
+    ):
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.IdentitySetDeleteResponse ' + \
+            'meta: ' + repr(self.meta) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'meta': self.meta,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            meta=d.get('meta'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
 class IdentitySetGetResponse:
     '''
          IdentitySetGetResponse returns a requested IdentitySet.
     '''
     __slots__ = [
         'identity_set',
         'meta',
@@ -10954,14 +11050,67 @@
             activity_id=d.get('activity_id'),
             deleted_at=d.get('deleted_at'),
             identity_set=d.get('identity_set'),
             timestamp=d.get('timestamp'),
         )
 
 
+class IdentitySetUpdateResponse:
+    '''
+         IdentitySetUpdateResponse returns the fields of a IdentitySet after it has been updated by
+     a IdentitySetUpdateRequest.
+    '''
+    __slots__ = [
+        'identity_set',
+        'meta',
+        'rate_limit',
+    ]
+
+    def __init__(
+        self,
+        identity_set=None,
+        meta=None,
+        rate_limit=None,
+    ):
+        self.identity_set = identity_set if identity_set is not None else None
+        '''
+         The updated IdentitySet.
+        '''
+        self.meta = meta if meta is not None else None
+        '''
+         Reserved for future use.
+        '''
+        self.rate_limit = rate_limit if rate_limit is not None else None
+        '''
+         Rate limit information.
+        '''
+
+    def __repr__(self):
+        return '<sdm.IdentitySetUpdateResponse ' + \
+            'identity_set: ' + repr(self.identity_set) + ' ' +\
+            'meta: ' + repr(self.meta) + ' ' +\
+            'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'identity_set': self.identity_set,
+            'meta': self.meta,
+            'rate_limit': self.rate_limit,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            identity_set=d.get('identity_set'),
+            meta=d.get('meta'),
+            rate_limit=d.get('rate_limit'),
+        )
+
+
 class KeyfactorSSHStore:
     __slots__ = [
         'ca_file_path',
         'certificate_file_path',
         'default_certificate_authority_name',
         'default_certificate_profile_name',
         'default_end_entity_profile_name',
```

## Comparing `strongdm-9.0.0/strongdm/remote_identities_pb2_grpc.py` & `strongdm-9.1.0/strongdm/remote_identities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/accounts_pb2.py` & `strongdm-9.1.0/strongdm/accounts_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/drivers_pb2_grpc.py` & `strongdm-9.1.0/strongdm/drivers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflows_history_pb2.py` & `strongdm-9.1.0/strongdm/approval_workflows_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/secret_stores_pb2.py` & `strongdm-9.1.0/strongdm/secret_stores_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_roles_history_pb2.py` & `strongdm-9.1.0/strongdm/workflow_roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/peering_group_nodes_pb2.py` & `strongdm-9.1.0/strongdm/peering_group_nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_grants_pb2_grpc.py` & `strongdm-9.1.0/strongdm/account_grants_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/tags_pb2_grpc.py` & `strongdm-9.1.0/strongdm/tags_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_attachments_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/account_attachments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/identity_sets_pb2_grpc.py` & `strongdm-9.1.0/strongdm/remote_identity_groups_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,128 +12,128 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # 
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import identity_sets_pb2 as identity__sets__pb2
+from . import remote_identity_groups_pb2 as remote__identity__groups__pb2
 
 
-class IdentitySetsStub(object):
-    """A IdentitySet is a named grouping of Identity Aliases for Accounts.
-    An Account's relationship to a IdentitySet is defined via IdentityAlias objects.
+class RemoteIdentityGroupsStub(object):
+    """A RemoteIdentityGroup is a named grouping of Remote Identities for Accounts.
+    An Account's relationship to a RemoteIdentityGroup is defined via RemoteIdentity objects.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Get = channel.unary_unary(
-                '/v1.IdentitySets/Get',
-                request_serializer=identity__sets__pb2.IdentitySetGetRequest.SerializeToString,
-                response_deserializer=identity__sets__pb2.IdentitySetGetResponse.FromString,
+                '/v1.RemoteIdentityGroups/Get',
+                request_serializer=remote__identity__groups__pb2.RemoteIdentityGroupGetRequest.SerializeToString,
+                response_deserializer=remote__identity__groups__pb2.RemoteIdentityGroupGetResponse.FromString,
                 )
         self.List = channel.unary_unary(
-                '/v1.IdentitySets/List',
-                request_serializer=identity__sets__pb2.IdentitySetListRequest.SerializeToString,
-                response_deserializer=identity__sets__pb2.IdentitySetListResponse.FromString,
+                '/v1.RemoteIdentityGroups/List',
+                request_serializer=remote__identity__groups__pb2.RemoteIdentityGroupListRequest.SerializeToString,
+                response_deserializer=remote__identity__groups__pb2.RemoteIdentityGroupListResponse.FromString,
                 )
 
 
-class IdentitySetsServicer(object):
-    """A IdentitySet is a named grouping of Identity Aliases for Accounts.
-    An Account's relationship to a IdentitySet is defined via IdentityAlias objects.
+class RemoteIdentityGroupsServicer(object):
+    """A RemoteIdentityGroup is a named grouping of Remote Identities for Accounts.
+    An Account's relationship to a RemoteIdentityGroup is defined via RemoteIdentity objects.
     """
 
     def Get(self, request, context):
-        """// Create registers a new IdentitySet.
-        rpc Create(IdentitySetCreateRequest) returns (IdentitySetCreateResponse) {
+        """// Create registers a new RemoteIdentityGroup.
+        rpc Create(RemoteIdentityGroupCreateRequest) returns (RemoteIdentityGroupCreateResponse) {
         option (v1.method_options).method = "post";
-        option (v1.method_options).url = "/v1/identity-sets";
+        option (v1.method_options).url = "/v1/remote-identity-groups";
         }
 
-        Get reads one IdentitySet by ID.
+        Get reads one RemoteIdentityGroup by ID.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def List(self, request, context):
-        """// Update replaces all the fields of a IdentitySet by ID.
-        rpc Update(IdentitySetUpdateRequest) returns (IdentitySetUpdateResponse) {
+        """// Update replaces all the fields of a RemoteIdentityGroup by ID.
+        rpc Update(RemoteIdentityGroupUpdateRequest) returns (RemoteIdentityGroupUpdateResponse) {
         option (v1.method_options).method = "put";
-        option (v1.method_options).url = "/v1/identity-sets/{id}";
+        option (v1.method_options).url = "/v1/remote-identity-groups/{id}";
         }
 
-        // Delete removes a IdentitySet by ID.
-        rpc Delete(IdentitySetDeleteRequest) returns (IdentitySetDeleteResponse) {
+        // Delete removes a RemoteIdentityGroup by ID.
+        rpc Delete(RemoteIdentityGroupDeleteRequest) returns (RemoteIdentityGroupDeleteResponse) {
         option (v1.method_options).method = "delete";
-        option (v1.method_options).url = "/v1/identity-sets/{id}";
+        option (v1.method_options).url = "/v1/remote-identity-groups/{id}";
         }
 
-        List gets a list of IdentitySets matching a given set of criteria.
+        List gets a list of RemoteIdentityGroups matching a given set of criteria.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_IdentitySetsServicer_to_server(servicer, server):
+def add_RemoteIdentityGroupsServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Get': grpc.unary_unary_rpc_method_handler(
                     servicer.Get,
-                    request_deserializer=identity__sets__pb2.IdentitySetGetRequest.FromString,
-                    response_serializer=identity__sets__pb2.IdentitySetGetResponse.SerializeToString,
+                    request_deserializer=remote__identity__groups__pb2.RemoteIdentityGroupGetRequest.FromString,
+                    response_serializer=remote__identity__groups__pb2.RemoteIdentityGroupGetResponse.SerializeToString,
             ),
             'List': grpc.unary_unary_rpc_method_handler(
                     servicer.List,
-                    request_deserializer=identity__sets__pb2.IdentitySetListRequest.FromString,
-                    response_serializer=identity__sets__pb2.IdentitySetListResponse.SerializeToString,
+                    request_deserializer=remote__identity__groups__pb2.RemoteIdentityGroupListRequest.FromString,
+                    response_serializer=remote__identity__groups__pb2.RemoteIdentityGroupListResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'v1.IdentitySets', rpc_method_handlers)
+            'v1.RemoteIdentityGroups', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class IdentitySets(object):
-    """A IdentitySet is a named grouping of Identity Aliases for Accounts.
-    An Account's relationship to a IdentitySet is defined via IdentityAlias objects.
+class RemoteIdentityGroups(object):
+    """A RemoteIdentityGroup is a named grouping of Remote Identities for Accounts.
+    An Account's relationship to a RemoteIdentityGroup is defined via RemoteIdentity objects.
     """
 
     @staticmethod
     def Get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/v1.IdentitySets/Get',
-            identity__sets__pb2.IdentitySetGetRequest.SerializeToString,
-            identity__sets__pb2.IdentitySetGetResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/v1.RemoteIdentityGroups/Get',
+            remote__identity__groups__pb2.RemoteIdentityGroupGetRequest.SerializeToString,
+            remote__identity__groups__pb2.RemoteIdentityGroupGetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def List(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/v1.IdentitySets/List',
-            identity__sets__pb2.IdentitySetListRequest.SerializeToString,
-            identity__sets__pb2.IdentitySetListResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/v1.RemoteIdentityGroups/List',
+            remote__identity__groups__pb2.RemoteIdentityGroupListRequest.SerializeToString,
+            remote__identity__groups__pb2.RemoteIdentityGroupListResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## Comparing `strongdm-9.0.0/strongdm/account_permissions_pb2.py` & `strongdm-9.1.0/strongdm/account_permissions_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/access_requests_pb2_grpc.py` & `strongdm-9.1.0/strongdm/access_requests_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/workflow_approvers_pb2_grpc.py` & `strongdm-9.1.0/strongdm/workflow_approvers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py` & `strongdm-9.1.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_resources_pb2_grpc.py` & `strongdm-9.1.0/strongdm/account_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm/account_permissions_pb2_grpc.py` & `strongdm-9.1.0/strongdm/account_permissions_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm.egg-info/SOURCES.txt` & `strongdm-9.1.0/strongdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `strongdm-9.0.0/strongdm.egg-info/PKG-INFO` & `strongdm-9.1.0/strongdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 9.0.0
+Version: 9.1.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v9.0.0.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v9.1.0.tar.gz
 Keywords: strongDM,sdm,api,automation,security,audit,database,server,ssh,rdp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

