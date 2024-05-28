# Comparing `tmp/pypanther-0.1.1a3.tar.gz` & `tmp/pypanther-0.1.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypanther-0.1.1a3.tar", max compression
+gzip compressed data, was "pypanther-0.1.1a8.tar", max compression
```

## Comparing `pypanther-0.1.1a3.tar` & `pypanther-0.1.1a8.tar`

### file list

```diff
@@ -1,565 +1,566 @@
--rw-r--r--   0        0        0    34523 2024-05-22 19:16:21.930547 pypanther-0.1.1a3/LICENSE.txt
--rw-r--r--   0        0        0       80 2024-05-03 18:47:26.705553 pypanther-0.1.1a3/README.md
--rw-r--r--   0        0        0      185 2024-05-23 22:00:33.237693 pypanther-0.1.1a3/pypanther/__init__.py
--rw-r--r--   0        0        0    24586 2024-05-24 15:16:21.423666 pypanther-0.1.1a3/pypanther/base.py
--rw-r--r--   0        0        0      490 2024-05-23 22:00:33.238107 pypanther-0.1.1a3/pypanther/cache.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:14.952849 pypanther-0.1.1a3/pypanther/data_models/__init__.py
--rw-r--r--   0        0        0     1387 2024-05-24 12:40:14.944512 pypanther-0.1.1a3/pypanther/data_models/asana_data_model.py
--rw-r--r--   0        0        0     1544 2024-05-24 12:40:14.933036 pypanther-0.1.1a3/pypanther/data_models/atlassian_data_model.py
--rw-r--r--   0        0        0      607 2024-05-24 12:40:14.942246 pypanther-0.1.1a3/pypanther/data_models/aws_alb_data_model.py
--rw-r--r--   0        0        0     2214 2024-05-24 12:40:14.938734 pypanther-0.1.1a3/pypanther/data_models/aws_cloudtrail_data_model.py
--rw-r--r--   0        0        0     1465 2024-05-24 12:40:14.929894 pypanther-0.1.1a3/pypanther/data_models/aws_eks_data_model.py
--rw-r--r--   0        0        0      630 2024-05-24 12:40:14.936327 pypanther-0.1.1a3/pypanther/data_models/aws_s3_data_model.py
--rw-r--r--   0        0        0      593 2024-05-24 12:40:14.939270 pypanther-0.1.1a3/pypanther/data_models/aws_vpcdns_data_model.py
--rw-r--r--   0        0        0      742 2024-05-24 12:40:14.928634 pypanther-0.1.1a3/pypanther/data_models/aws_vpcflow_data_model.py
--rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.927521 pypanther-0.1.1a3/pypanther/data_models/azure_signin_data_model.py
--rw-r--r--   0        0        0      941 2024-05-24 12:40:14.941146 pypanther-0.1.1a3/pypanther/data_models/box_data_model.py
--rw-r--r--   0        0        0      873 2024-05-24 12:40:14.939822 pypanther-0.1.1a3/pypanther/data_models/cisco_umbrella_data_model.py
--rw-r--r--   0        0        0      653 2024-05-24 12:40:14.943897 pypanther-0.1.1a3/pypanther/data_models/cloudflare_firewall_data_model.py
--rw-r--r--   0        0        0      729 2024-05-24 12:40:14.928057 pypanther-0.1.1a3/pypanther/data_models/cloudflare_httpreq_data_model.py
--rw-r--r--   0        0        0     1853 2024-05-24 12:40:14.943403 pypanther-0.1.1a3/pypanther/data_models/crowdstrike_fdr_data_model.py
--rw-r--r--   0        0        0     5215 2024-05-24 12:40:14.934292 pypanther-0.1.1a3/pypanther/data_models/gcp_data_model.py
--rw-r--r--   0        0        0     1613 2024-05-24 12:40:14.937900 pypanther-0.1.1a3/pypanther/data_models/github_data_model.py
--rw-r--r--   0        0        0     1669 2024-05-24 12:40:14.935584 pypanther-0.1.1a3/pypanther/data_models/gsuite_data_model.py
--rw-r--r--   0        0        0     1864 2024-05-24 12:40:14.940562 pypanther-0.1.1a3/pypanther/data_models/notion_data_model.py
--rw-r--r--   0        0        0     2070 2024-05-24 12:40:14.937166 pypanther-0.1.1a3/pypanther/data_models/okta_data_model.py
--rw-r--r--   0        0        0     1467 2024-05-24 12:40:14.932330 pypanther-0.1.1a3/pypanther/data_models/onelogin_data_model.py
--rw-r--r--   0        0        0      730 2024-05-24 12:40:14.934876 pypanther-0.1.1a3/pypanther/data_models/onepassword_itemusage_data_model.py
--rw-r--r--   0        0        0     1058 2024-05-24 12:40:14.941731 pypanther-0.1.1a3/pypanther/data_models/onepassword_signinattempt_data_model.py
--rw-r--r--   0        0        0     1742 2024-05-24 12:40:14.930685 pypanther-0.1.1a3/pypanther/data_models/panther_audit_data_model.py
--rw-r--r--   0        0        0      613 2024-05-24 12:40:14.929135 pypanther-0.1.1a3/pypanther/data_models/slack_accesslogs_data_model.py
--rw-r--r--   0        0        0      711 2024-05-24 12:40:14.942793 pypanther-0.1.1a3/pypanther/data_models/slack_auditlogs_data_model.py
--rw-r--r--   0        0        0      500 2024-05-24 12:40:14.926474 pypanther-0.1.1a3/pypanther/data_models/slack_integrationlogs_data_model.py
--rw-r--r--   0        0        0     2714 2024-05-24 12:40:14.931651 pypanther-0.1.1a3/pypanther/data_models/zendesk_data_model.py
--rw-r--r--   0        0        0      886 2024-05-24 12:40:14.926019 pypanther-0.1.1a3/pypanther/data_models/zoom_activity_data_model.py
--rw-r--r--   0        0        0     1887 2024-05-24 12:40:14.925345 pypanther-0.1.1a3/pypanther/data_models/zoom_operation_data_model.py
--rw-r--r--   0        0        0     2682 2024-05-23 22:00:33.243958 pypanther-0.1.1a3/pypanther/get.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:13.778915 pypanther-0.1.1a3/pypanther/helpers/__init__.py
--rw-r--r--   0        0        0     2107 2024-05-24 12:40:14.169513 pypanther-0.1.1a3/pypanther/helpers/gcp_base_helpers.py
--rw-r--r--   0        0        0      781 2024-05-24 12:40:14.303335 pypanther-0.1.1a3/pypanther/helpers/gcp_environment.py
--rw-r--r--   0        0        0     1417 2024-05-24 12:40:13.948393 pypanther-0.1.1a3/pypanther/helpers/panther_asana_helpers.py
--rw-r--r--   0        0        0     1597 2024-05-24 12:40:14.156772 pypanther-0.1.1a3/pypanther/helpers/panther_audit.py
--rw-r--r--   0        0        0      555 2024-05-24 12:40:13.952837 pypanther-0.1.1a3/pypanther/helpers/panther_auth0_helpers.py
--rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.099017 pypanther-0.1.1a3/pypanther/helpers/panther_azuresignin_helpers.py
--rw-r--r--   0        0        0    19692 2024-05-24 12:40:14.264799 pypanther-0.1.1a3/pypanther/helpers/panther_base_helpers.py
--rw-r--r--   0        0        0     4529 2024-05-24 12:40:14.146111 pypanther-0.1.1a3/pypanther/helpers/panther_box_helpers.py
--rw-r--r--   0        0        0     2267 2024-05-24 12:40:13.916642 pypanther-0.1.1a3/pypanther/helpers/panther_cloudflare_helpers.py
--rw-r--r--   0        0        0      507 2024-05-24 12:40:14.148779 pypanther-0.1.1a3/pypanther/helpers/panther_config.py
--rw-r--r--   0        0        0      891 2024-05-24 12:40:14.103142 pypanther-0.1.1a3/pypanther/helpers/panther_config_defaults.py
--rw-r--r--   0        0        0     1043 2024-05-24 12:40:13.795713 pypanther-0.1.1a3/pypanther/helpers/panther_config_overrides.py
--rw-r--r--   0        0        0     3465 2024-05-24 12:40:13.831736 pypanther-0.1.1a3/pypanther/helpers/panther_default.py
--rw-r--r--   0        0        0     1288 2024-05-24 12:40:13.811022 pypanther-0.1.1a3/pypanther/helpers/panther_duo_helpers.py
--rw-r--r--   0        0        0     1118 2024-05-24 12:40:14.384435 pypanther-0.1.1a3/pypanther/helpers/panther_event_type_helpers.py
--rw-r--r--   0        0        0    12436 2024-05-24 12:40:14.482779 pypanther-0.1.1a3/pypanther/helpers/panther_greynoise_helpers.py
--rw-r--r--   0        0        0    38305 2024-05-24 12:40:13.902461 pypanther-0.1.1a3/pypanther/helpers/panther_iocs.py
--rw-r--r--   0        0        0     6497 2024-05-24 12:40:14.002454 pypanther-0.1.1a3/pypanther/helpers/panther_ipinfo_helpers.py
--rw-r--r--   0        0        0     2154 2024-05-24 12:40:14.015836 pypanther-0.1.1a3/pypanther/helpers/panther_lookuptable_helpers.py
--rw-r--r--   0        0        0      387 2024-05-24 12:40:14.270284 pypanther-0.1.1a3/pypanther/helpers/panther_mongodb_helpers.py
--rw-r--r--   0        0        0      340 2024-05-24 12:40:13.834434 pypanther-0.1.1a3/pypanther/helpers/panther_notion_helpers.py
--rw-r--r--   0        0        0    13096 2024-05-24 12:40:14.370655 pypanther-0.1.1a3/pypanther/helpers/panther_oss_helpers.py
--rw-r--r--   0        0        0      610 2024-05-24 12:40:13.801982 pypanther-0.1.1a3/pypanther/helpers/panther_snyk_helpers.py
--rw-r--r--   0        0        0      492 2024-05-24 12:40:14.307780 pypanther-0.1.1a3/pypanther/helpers/panther_tailscale_helpers.py
--rw-r--r--   0        0        0      567 2024-05-24 12:40:14.312664 pypanther-0.1.1a3/pypanther/helpers/panther_tines_helpers.py
--rw-r--r--   0        0        0     1542 2024-05-24 12:40:14.379643 pypanther-0.1.1a3/pypanther/helpers/panther_tor_helpers.py
--rw-r--r--   0        0        0     3084 2024-05-24 12:40:13.935600 pypanther-0.1.1a3/pypanther/helpers/panther_zoom_helpers.py
--rw-r--r--   0        0        0    13022 2024-05-23 22:06:29.350498 pypanther-0.1.1a3/pypanther/log_types.py
--rw-r--r--   0        0        0     1322 2024-05-24 13:47:47.094872 pypanther-0.1.1a3/pypanther/main.py
--rw-r--r--   0        0        0      824 2024-05-23 22:00:33.250813 pypanther-0.1.1a3/pypanther/register.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.351956 pypanther-0.1.1a3/pypanther/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356408 pypanther-0.1.1a3/pypanther/rules/asana_rules/__init__.py
--rw-r--r--   0        0        0     4055 2024-05-24 15:16:21.424215 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_service_account_created.py
--rw-r--r--   0        0        0     3227 2024-05-24 15:16:21.424547 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_team_privacy_public.py
--rw-r--r--   0        0        0     3249 2024-05-24 15:16:21.425052 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py
--rw-r--r--   0        0        0     3218 2024-05-24 15:16:21.425432 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py
--rw-r--r--   0        0        0     3406 2024-05-24 15:16:21.425777 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py
--rw-r--r--   0        0        0     3385 2024-05-24 15:16:21.426151 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py
--rw-r--r--   0        0        0     3733 2024-05-24 15:16:21.426488 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_new_admin.py
--rw-r--r--   0        0        0     3228 2024-05-24 15:16:21.426739 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_org_export.py
--rw-r--r--   0        0        0     3711 2024-05-24 15:16:21.427013 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py
--rw-r--r--   0        0        0     3615 2024-05-24 15:16:21.427323 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py
--rw-r--r--   0        0        0     3484 2024-05-24 15:16:21.427559 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_saml_optional.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355786 pypanther-0.1.1a3/pypanther/rules/atlassian_rules/__init__.py
--rw-r--r--   0        0        0     4877 2024-05-24 15:16:21.428031 pypanther-0.1.1a3/pypanther/rules/atlassian_rules/user_logged_in_as_user.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352374 pypanther-0.1.1a3/pypanther/rules/auth0_rules/__init__.py
--rw-r--r--   0        0        0    44986 2024-05-24 15:16:21.428415 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_custom_role_created.py
--rw-r--r--   0        0        0    15412 2024-05-24 15:16:21.428810 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_integration_installed.py
--rw-r--r--   0        0        0    23138 2024-05-24 15:16:21.429303 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py
--rw-r--r--   0        0        0    23488 2024-05-24 15:16:21.429696 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py
--rw-r--r--   0        0        0    34159 2024-05-24 15:16:21.430104 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py
--rw-r--r--   0        0        0    23642 2024-05-24 15:16:21.430380 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py
--rw-r--r--   0        0        0    22663 2024-05-24 15:16:21.430665 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py
--rw-r--r--   0        0        0    19817 2024-05-24 15:16:21.431047 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py
--rw-r--r--   0        0        0    17279 2024-05-24 15:16:21.431316 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_user_invitation_created.py
--rw-r--r--   0        0        0    18166 2024-05-24 15:16:21.431594 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354895 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/__init__.py
--rw-r--r--   0        0        0    11009 2024-05-24 15:16:21.431991 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py
--rw-r--r--   0        0        0     8189 2024-05-24 15:16:21.432404 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py
--rw-r--r--   0        0        0     7038 2024-05-24 15:16:21.432638 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py
--rw-r--r--   0        0        0     3373 2024-05-24 15:16:21.432859 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py
--rw-r--r--   0        0        0     7212 2024-05-24 15:16:21.433158 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py
--rw-r--r--   0        0        0     4460 2024-05-24 12:40:19.072096 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py
--rw-r--r--   0        0        0     6992 2024-05-24 15:16:21.433498 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py
--rw-r--r--   0        0        0     6551 2024-05-24 15:16:21.433773 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py
--rw-r--r--   0        0        0     6538 2024-05-24 15:16:21.434033 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py
--rw-r--r--   0        0        0    20551 2024-05-24 15:16:21.434298 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py
--rw-r--r--   0        0        0     4027 2024-05-24 12:40:19.137363 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py
--rw-r--r--   0        0        0     5596 2024-05-24 15:16:21.434553 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py
--rw-r--r--   0        0        0     5699 2024-05-24 15:16:21.434870 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py
--rw-r--r--   0        0        0     2281 2024-05-24 15:16:21.435209 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py
--rw-r--r--   0        0        0     6712 2024-05-24 15:16:21.435527 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py
--rw-r--r--   0        0        0    17193 2024-05-24 12:40:19.013686 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py
--rw-r--r--   0        0        0    22406 2024-05-24 15:16:21.435872 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py
--rw-r--r--   0        0        0     7244 2024-05-24 15:16:21.436155 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py
--rw-r--r--   0        0        0     6874 2024-05-24 15:16:21.436423 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py
--rw-r--r--   0        0        0     8171 2024-05-24 15:16:21.436705 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py
--rw-r--r--   0        0        0     5159 2024-05-24 15:16:21.436966 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py
--rw-r--r--   0        0        0    30269 2024-05-24 15:16:21.437319 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py
--rw-r--r--   0        0        0     8600 2024-05-24 15:16:21.437710 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py
--rw-r--r--   0        0        0    39729 2024-05-24 15:16:21.437986 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py
--rw-r--r--   0        0        0    27319 2024-05-24 12:40:19.153333 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py
--rw-r--r--   0        0        0    26728 2024-05-24 12:40:19.048210 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py
--rw-r--r--   0        0        0     7262 2024-05-24 15:16:21.438351 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py
--rw-r--r--   0        0        0     8581 2024-05-24 12:40:19.131595 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py
--rw-r--r--   0        0        0     6105 2024-05-24 15:16:21.438771 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py
--rw-r--r--   0        0        0    12705 2024-05-24 12:40:19.146336 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py
--rw-r--r--   0        0        0    13749 2024-05-24 12:40:19.032961 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py
--rw-r--r--   0        0        0     7140 2024-05-24 15:16:21.439018 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py
--rw-r--r--   0        0        0    10477 2024-05-24 15:16:21.439288 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py
--rw-r--r--   0        0        0     9036 2024-05-24 15:16:21.439564 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py
--rw-r--r--   0        0        0     3375 2024-05-24 15:16:21.439795 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py
--rw-r--r--   0        0        0     5202 2024-05-24 15:16:21.440052 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py
--rw-r--r--   0        0        0    11250 2024-05-24 15:16:21.440309 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py
--rw-r--r--   0        0        0     5716 2024-05-24 12:40:19.030090 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py
--rw-r--r--   0        0        0     9720 2024-05-24 15:16:21.440570 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py
--rw-r--r--   0        0        0    26986 2024-05-24 12:40:19.164857 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py
--rw-r--r--   0        0        0     7813 2024-05-24 15:16:21.440884 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py
--rw-r--r--   0        0        0    16362 2024-05-24 15:16:21.441210 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py
--rw-r--r--   0        0        0    14625 2024-05-24 15:16:21.441626 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py
--rw-r--r--   0        0        0    17386 2024-05-24 15:16:21.441875 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py
--rw-r--r--   0        0        0     7466 2024-05-24 15:16:21.442158 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py
--rw-r--r--   0        0        0    18968 2024-05-24 15:16:21.442383 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py
--rw-r--r--   0        0        0     4655 2024-05-24 15:16:21.442623 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py
--rw-r--r--   0        0        0    10739 2024-05-24 15:16:21.442885 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py
--rw-r--r--   0        0        0     3920 2024-05-24 15:16:21.443092 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py
--rw-r--r--   0        0        0     5811 2024-05-24 15:16:21.443361 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py
--rw-r--r--   0        0        0     7502 2024-05-24 15:16:21.443687 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py
--rw-r--r--   0        0        0    12275 2024-05-24 15:16:21.443990 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py
--rw-r--r--   0        0        0    11502 2024-05-24 15:16:21.444278 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py
--rw-r--r--   0        0        0     5556 2024-05-24 15:16:21.444534 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py
--rw-r--r--   0        0        0     7544 2024-05-24 15:16:21.444768 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py
--rw-r--r--   0        0        0     5177 2024-05-24 12:40:19.036764 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py
--rw-r--r--   0        0        0     6464 2024-05-24 15:16:21.445000 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py
--rw-r--r--   0        0        0     8683 2024-05-24 12:40:19.124611 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py
--rw-r--r--   0        0        0     5962 2024-05-24 15:16:21.445244 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py
--rw-r--r--   0        0        0     6768 2024-05-24 15:16:21.445508 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py
--rw-r--r--   0        0        0     7010 2024-05-24 15:16:21.445747 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352785 pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/__init__.py
--rw-r--r--   0        0        0     9686 2024-05-24 15:16:21.446020 pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py
--rw-r--r--   0        0        0    17799 2024-05-24 15:16:21.446254 pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354748 pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/__init__.py
--rw-r--r--   0        0        0     5356 2024-05-24 15:16:21.446559 pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py
--rw-r--r--   0        0        0     5377 2024-05-24 15:16:21.446848 pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py
--rw-r--r--   0        0        0     5403 2024-05-24 15:16:21.447130 pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355307 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/__init__.py
--rw-r--r--   0        0        0     4688 2024-05-24 15:16:21.447407 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_access_error.py
--rw-r--r--   0        0        0     2546 2024-05-24 12:40:19.231135 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py
--rw-r--r--   0        0        0     6263 2024-05-24 15:16:21.447657 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py
--rw-r--r--   0        0        0     1983 2024-05-24 12:40:19.239787 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py
--rw-r--r--   0        0        0     8734 2024-05-24 12:40:19.236359 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355429 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/__init__.py
--rw-r--r--   0        0        0     6776 2024-05-24 15:16:21.447901 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py
--rw-r--r--   0        0        0     1326 2024-05-24 15:16:21.448149 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py
--rw-r--r--   0        0        0     2524 2024-05-24 12:40:19.241211 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py
--rw-r--r--   0        0        0     2484 2024-05-24 12:40:19.248154 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py
--rw-r--r--   0        0        0     2913 2024-05-24 12:40:19.246794 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355171 pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/__init__.py
--rw-r--r--   0        0        0     7964 2024-05-24 15:16:21.448405 pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_failed_signins.py
--rw-r--r--   0        0        0    15752 2024-05-24 15:16:21.448657 pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_legacyauth.py
--rw-r--r--   0        0        0    17539 2024-05-24 15:16:21.448880 pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353050 pypanther-0.1.1a3/pypanther/rules/box_rules/__init__.py
--rw-r--r--   0        0        0     2120 2024-05-24 15:16:21.449114 pypanther-0.1.1a3/pypanther/rules/box_rules/box_access_granted.py
--rw-r--r--   0        0        0     2855 2024-05-24 15:16:21.449326 pypanther-0.1.1a3/pypanther/rules/box_rules/box_anomalous_download.py
--rw-r--r--   0        0        0     2730 2024-05-24 12:40:18.694430 pypanther-0.1.1a3/pypanther/rules/box_rules/box_event_triggered_externally.py
--rw-r--r--   0        0        0     3638 2024-05-24 12:40:18.687439 pypanther-0.1.1a3/pypanther/rules/box_rules/box_item_shared_externally.py
--rw-r--r--   0        0        0     4252 2024-05-24 15:16:21.449561 pypanther-0.1.1a3/pypanther/rules/box_rules/box_malicious_content.py
--rw-r--r--   0        0        0     2110 2024-05-24 15:16:21.449767 pypanther-0.1.1a3/pypanther/rules/box_rules/box_new_login.py
--rw-r--r--   0        0        0     2808 2024-05-24 15:16:21.449973 pypanther-0.1.1a3/pypanther/rules/box_rules/box_policy_violation.py
--rw-r--r--   0        0        0     4201 2024-05-24 15:16:21.450221 pypanther-0.1.1a3/pypanther/rules/box_rules/box_suspicious_login_or_session.py
--rw-r--r--   0        0        0     2212 2024-05-24 15:16:21.450435 pypanther-0.1.1a3/pypanther/rules/box_rules/box_untrusted_device.py
--rw-r--r--   0        0        0     2352 2024-05-24 15:16:21.450657 pypanther-0.1.1a3/pypanther/rules/box_rules/box_user_downloads.py
--rw-r--r--   0        0        0     3165 2024-05-24 15:16:21.450863 pypanther-0.1.1a3/pypanther/rules/box_rules/box_user_permission_updates.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355655 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/__init__.py
--rw-r--r--   0        0        0     3299 2024-05-24 15:16:21.451080 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py
--rw-r--r--   0        0        0     3023 2024-05-24 15:16:21.451306 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py
--rw-r--r--   0        0        0     3473 2024-05-24 15:16:21.451550 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py
--rw-r--r--   0        0        0     2248 2024-05-24 15:16:21.451767 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_flagged.py
--rw-r--r--   0        0        0     2577 2024-05-24 15:16:21.451988 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py
--rw-r--r--   0        0        0    11303 2024-05-24 15:16:21.452260 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355556 pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/__init__.py
--rw-r--r--   0        0        0     1787 2024-05-24 15:16:21.452540 pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py
--rw-r--r--   0        0        0     1414 2024-05-24 12:40:19.250591 pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py
--rw-r--r--   0        0        0     1903 2024-05-24 12:40:19.253188 pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354017 pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/__init__.py
--rw-r--r--   0        0        0     4969 2024-05-24 15:16:21.452875 pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py
--rw-r--r--   0        0        0     7563 2024-05-24 12:40:18.920956 pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355030 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/__init__.py
--rw-r--r--   0        0        0    29385 2024-05-24 15:16:21.453267 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py
--rw-r--r--   0        0        0     8177 2024-05-24 15:16:21.453668 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py
--rw-r--r--   0        0        0     9893 2024-05-24 15:16:21.453945 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py
--rw-r--r--   0        0        0     9855 2024-05-24 15:16:21.454211 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py
--rw-r--r--   0        0        0    10420 2024-05-24 15:16:21.454477 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py
--rw-r--r--   0        0        0    12177 2024-05-24 12:40:19.187772 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py
--rw-r--r--   0        0        0    11711 2024-05-24 12:40:19.205936 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py
--rw-r--r--   0        0        0    18680 2024-05-24 15:16:21.454710 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py
--rw-r--r--   0        0        0    18887 2024-05-24 15:16:21.454956 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py
--rw-r--r--   0        0        0    15614 2024-05-24 15:16:21.455287 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py
--rw-r--r--   0        0        0     7208 2024-05-24 15:16:21.455541 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py
--rw-r--r--   0        0        0     9722 2024-05-24 15:16:21.455811 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py
--rw-r--r--   0        0        0    13594 2024-05-24 15:16:21.456062 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py
--rw-r--r--   0        0        0     9703 2024-05-24 15:16:21.456322 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py
--rw-r--r--   0        0        0    10006 2024-05-24 15:16:21.456575 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py
--rw-r--r--   0        0        0    17357 2024-05-24 15:16:21.456795 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354190 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/__init__.py
--rw-r--r--   0        0        0     6793 2024-05-24 15:16:21.457052 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py
--rw-r--r--   0        0        0     9494 2024-05-24 15:16:21.457293 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_external_share.py
--rw-r--r--   0        0        0     8238 2024-05-24 15:16:21.457569 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py
--rw-r--r--   0        0        0    11142 2024-05-24 15:16:21.457840 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py
--rw-r--r--   0        0        0     5131 2024-05-24 15:16:21.458095 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353471 pypanther-0.1.1a3/pypanther/rules/duo_rules/__init__.py
--rw-r--r--   0        0        0     2088 2024-05-24 15:16:21.458537 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py
--rw-r--r--   0        0        0     2175 2024-05-24 15:16:21.460660 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py
--rw-r--r--   0        0        0     2244 2024-05-24 15:16:21.460989 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py
--rw-r--r--   0        0        0     2241 2024-05-24 15:16:21.461264 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_create_admin.py
--rw-r--r--   0        0        0     2508 2024-05-24 15:16:21.461517 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_lockout.py
--rw-r--r--   0        0        0     2658 2024-05-24 15:16:21.461765 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py
--rw-r--r--   0        0        0     1968 2024-05-24 15:16:21.461984 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py
--rw-r--r--   0        0        0     3144 2024-05-24 15:16:21.462206 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py
--rw-r--r--   0        0        0     2208 2024-05-24 15:16:21.462435 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_policy_updated.py
--rw-r--r--   0        0        0     3376 2024-05-24 15:16:21.462674 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py
--rw-r--r--   0        0        0     2902 2024-05-24 15:16:21.462911 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py
--rw-r--r--   0        0        0     2028 2024-05-24 15:16:21.463155 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_action_fraudulent.py
--rw-r--r--   0        0        0     3152 2024-05-24 15:16:21.463423 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_anomalous_push.py
--rw-r--r--   0        0        0     3058 2024-05-24 15:16:21.463696 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_bypass_code_used.py
--rw-r--r--   0        0        0     5450 2024-05-24 15:16:21.463967 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353698 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/__init__.py
--rw-r--r--   0        0        0     9839 2024-05-24 15:16:21.464276 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py
--rw-r--r--   0        0        0    12333 2024-05-24 15:16:21.464557 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py
--rw-r--r--   0        0        0     7045 2024-05-24 15:16:21.464840 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py
--rw-r--r--   0        0        0     7839 2024-05-24 15:16:21.465105 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py
--rw-r--r--   0        0        0     4127 2024-05-24 15:16:21.465357 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py
--rw-r--r--   0        0        0     4127 2024-05-24 15:16:21.465626 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py
--rw-r--r--   0        0        0    19128 2024-05-24 15:16:21.465900 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py
--rw-r--r--   0        0        0    10432 2024-05-24 15:16:21.466320 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py
--rw-r--r--   0        0        0    15433 2024-05-24 15:16:21.466688 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py
--rw-r--r--   0        0        0     9149 2024-05-24 15:16:21.467069 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py
--rw-r--r--   0        0        0     6818 2024-05-24 15:16:21.467438 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py
--rw-r--r--   0        0        0     8941 2024-05-24 15:16:21.467837 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py
--rw-r--r--   0        0        0     3831 2024-05-24 15:16:21.468230 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py
--rw-r--r--   0        0        0     4527 2024-05-24 15:16:21.468564 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py
--rw-r--r--   0        0        0    15793 2024-05-24 15:16:21.468870 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py
--rw-r--r--   0        0        0     5269 2024-05-24 15:16:21.469204 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py
--rw-r--r--   0        0        0     9941 2024-05-24 15:16:21.469591 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py
--rw-r--r--   0        0        0     3579 2024-05-24 15:16:21.469975 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py
--rw-r--r--   0        0        0     4115 2024-05-24 15:16:21.470322 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py
--rw-r--r--   0        0        0     6785 2024-05-24 15:16:21.470690 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py
--rw-r--r--   0        0        0     6585 2024-05-24 15:16:21.471079 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py
--rw-r--r--   0        0        0     7304 2024-05-24 15:16:21.471358 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py
--rw-r--r--   0        0        0     9263 2024-05-24 15:16:21.471651 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py
--rw-r--r--   0        0        0    11294 2024-05-24 15:16:21.471923 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py
--rw-r--r--   0        0        0     7615 2024-05-24 15:16:21.472188 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py
--rw-r--r--   0        0        0     7079 2024-05-24 15:16:21.472435 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py
--rw-r--r--   0        0        0    10607 2024-05-24 15:16:21.472706 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py
--rw-r--r--   0        0        0     4068 2024-05-24 15:16:21.473027 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py
--rw-r--r--   0        0        0     7714 2024-05-24 15:16:21.473395 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py
--rw-r--r--   0        0        0    11742 2024-05-24 15:16:21.473678 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py
--rw-r--r--   0        0        0    10816 2024-05-24 15:16:21.473953 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py
--rw-r--r--   0        0        0     2275 2024-05-24 15:16:21.474180 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py
--rw-r--r--   0        0        0     2911 2024-05-24 15:16:21.474491 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py
--rw-r--r--   0        0        0    13058 2024-05-24 12:40:18.866059 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py
--rw-r--r--   0        0        0    10910 2024-05-24 15:16:21.474877 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py
--rw-r--r--   0        0        0     9626 2024-05-24 15:16:21.475160 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py
--rw-r--r--   0        0        0    10164 2024-05-24 15:16:21.475430 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py
--rw-r--r--   0        0        0    11767 2024-05-24 15:16:21.475792 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352868 pypanther-0.1.1a3/pypanther/rules/gcp_http_lb_rules/__init__.py
--rw-r--r--   0        0        0     5908 2024-05-24 15:16:21.476184 pypanther-0.1.1a3/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356266 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/__init__.py
--rw-r--r--   0        0        0     4559 2024-05-24 15:16:21.476451 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py
--rw-r--r--   0        0        0     6701 2024-05-24 12:40:19.340583 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py
--rw-r--r--   0        0        0     2251 2024-05-24 15:16:21.476747 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py
--rw-r--r--   0        0        0     3530 2024-05-24 15:16:21.477098 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py
--rw-r--r--   0        0        0     3433 2024-05-24 15:16:21.477323 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py
--rw-r--r--   0        0        0    12867 2024-05-24 15:16:21.477684 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py
--rw-r--r--   0        0        0     3499 2024-05-24 15:16:21.477988 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py
--rw-r--r--   0        0        0    14878 2024-05-24 15:16:21.478411 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py
--rw-r--r--   0        0        0    11462 2024-05-24 15:16:21.478669 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352570 pypanther-0.1.1a3/pypanther/rules/github_rules/__init__.py
--rw-r--r--   0        0        0     5241 2024-05-24 12:40:18.616900 pypanther-0.1.1a3/pypanther/rules/github_rules/github_action_failed.py
--rw-r--r--   0        0        0    14192 2024-05-24 15:16:21.478946 pypanther-0.1.1a3/pypanther/rules/github_rules/github_advanced_security_change.py
--rw-r--r--   0        0        0     2028 2024-05-24 15:16:21.479163 pypanther-0.1.1a3/pypanther/rules/github_rules/github_branch_policy_override.py
--rw-r--r--   0        0        0     2030 2024-05-24 15:16:21.479385 pypanther-0.1.1a3/pypanther/rules/github_rules/github_branch_protection_disabled.py
--rw-r--r--   0        0        0     2223 2024-05-24 15:16:21.479616 pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_auth_modified.py
--rw-r--r--   0        0        0     2409 2024-05-24 15:16:21.479861 pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_ip_allowlist.py
--rw-r--r--   0        0        0     2212 2024-05-24 15:16:21.480172 pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_moderators_add.py
--rw-r--r--   0        0        0     2302 2024-05-24 15:16:21.480396 pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_modified.py
--rw-r--r--   0        0        0     3381 2024-05-24 15:16:21.480613 pypanther-0.1.1a3/pypanther/rules/github_rules/github_organization_app_integration_installed.py
--rw-r--r--   0        0        0     2847 2024-05-24 15:16:21.480830 pypanther-0.1.1a3/pypanther/rules/github_rules/github_public_repository_created.py
--rw-r--r--   0        0        0     2762 2024-05-24 15:16:21.481050 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_collaborator_change.py
--rw-r--r--   0        0        0     1446 2024-05-24 15:16:21.481310 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_created.py
--rw-r--r--   0        0        0     2501 2024-05-24 15:16:21.481577 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_hook_modified.py
--rw-r--r--   0        0        0     4211 2024-05-24 15:16:21.482079 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_initial_access.py
--rw-r--r--   0        0        0     1890 2024-05-24 15:16:21.482329 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_visibility_change.py
--rw-r--r--   0        0        0     5328 2024-05-24 15:16:21.482612 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repository_transfer.py
--rw-r--r--   0        0        0     3320 2024-05-24 15:16:21.482858 pypanther-0.1.1a3/pypanther/rules/github_rules/github_secret_scanning_alert_created.py
--rw-r--r--   0        0        0     3326 2024-05-24 15:16:21.483159 pypanther-0.1.1a3/pypanther/rules/github_rules/github_team_modified.py
--rw-r--r--   0        0        0     1622 2024-05-24 15:16:21.483409 pypanther-0.1.1a3/pypanther/rules/github_rules/github_user_access_key_created.py
--rw-r--r--   0        0        0     1725 2024-05-24 15:16:21.483706 pypanther-0.1.1a3/pypanther/rules/github_rules/github_user_role_updated.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356132 pypanther-0.1.1a3/pypanther/rules/gitlab_rules/__init__.py
--rw-r--r--   0        0        0     2333 2024-05-24 15:16:21.484015 pypanther-0.1.1a3/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py
--rw-r--r--   0        0        0     2789 2024-05-24 15:16:21.484312 pypanther-0.1.1a3/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352688 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/__init__.py
--rw-r--r--   0        0        0     2521 2024-05-24 15:16:21.484638 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py
--rw-r--r--   0        0        0     2631 2024-05-24 15:16:21.484883 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py
--rw-r--r--   0        0        0     3188 2024-05-24 15:16:21.485119 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py
--rw-r--r--   0        0        0     2947 2024-05-24 15:16:21.485352 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py
--rw-r--r--   0        0        0     1749 2024-05-24 15:16:21.485594 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py
--rw-r--r--   0        0        0     6365 2024-05-24 15:16:21.485875 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py
--rw-r--r--   0        0        0     4716 2024-05-24 15:16:21.486157 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py
--rw-r--r--   0        0        0     1593 2024-05-24 15:16:21.486399 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py
--rw-r--r--   0        0        0     2190 2024-05-24 15:16:21.486639 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py
--rw-r--r--   0        0        0     1614 2024-05-24 15:16:21.486861 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py
--rw-r--r--   0        0        0     2739 2024-05-24 15:16:21.487116 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py
--rw-r--r--   0        0        0     4429 2024-05-24 15:16:21.487415 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py
--rw-r--r--   0        0        0     3205 2024-05-24 15:16:21.487780 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354403 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/__init__.py
--rw-r--r--   0        0        0     4360 2024-05-24 15:16:21.488109 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py
--rw-r--r--   0        0        0     6479 2024-05-24 15:16:21.488371 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py
--rw-r--r--   0        0        0     6692 2024-05-24 15:16:21.488623 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py
--rw-r--r--   0        0        0     5269 2024-05-24 15:16:21.488868 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py
--rw-r--r--   0        0        0     4631 2024-05-24 15:16:21.489112 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py
--rw-r--r--   0        0        0     1947 2024-05-24 15:16:21.489391 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py
--rw-r--r--   0        0        0     5772 2024-05-24 15:16:21.489802 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py
--rw-r--r--   0        0        0     2325 2024-05-24 12:40:18.988544 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py
--rw-r--r--   0        0        0     4324 2024-05-24 12:40:18.990649 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py
--rw-r--r--   0        0        0     1451 2024-05-24 15:16:21.490098 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py
--rw-r--r--   0        0        0     1984 2024-05-24 15:16:21.490412 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py
--rw-r--r--   0        0        0     1949 2024-05-24 15:16:21.490708 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py
--rw-r--r--   0        0        0     3035 2024-05-24 15:16:21.491052 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py
--rw-r--r--   0        0        0     3459 2024-05-24 12:40:18.954789 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py
--rw-r--r--   0        0        0     2728 2024-05-24 15:16:21.491353 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py
--rw-r--r--   0        0        0     3373 2024-05-24 15:16:21.491620 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py
--rw-r--r--   0        0        0     2006 2024-05-24 15:16:21.491969 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py
--rw-r--r--   0        0        0     3443 2024-05-24 15:16:21.492331 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py
--rw-r--r--   0        0        0     2573 2024-05-24 15:16:21.492593 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py
--rw-r--r--   0        0        0     2189 2024-05-24 15:16:21.492877 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py
--rw-r--r--   0        0        0     2707 2024-05-24 15:16:21.493162 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py
--rw-r--r--   0        0        0     6820 2024-05-24 15:16:21.493443 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py
--rw-r--r--   0        0        0     4999 2024-05-24 15:16:21.493742 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py
--rw-r--r--   0        0        0     6038 2024-05-24 15:16:21.493994 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py
--rw-r--r--   0        0        0     5438 2024-05-24 15:16:21.494274 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py
--rw-r--r--   0        0        0     5208 2024-05-24 15:16:21.494563 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py
--rw-r--r--   0        0        0     5158 2024-05-24 15:16:21.494909 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py
--rw-r--r--   0        0        0     4963 2024-05-24 15:16:21.495174 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py
--rw-r--r--   0        0        0     5209 2024-05-24 15:16:21.495453 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353938 pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/__init__.py
--rw-r--r--   0        0        0    10537 2024-05-24 12:40:18.909156 pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py
--rw-r--r--   0        0        0     4546 2024-05-24 15:16:21.495759 pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py
--rw-r--r--   0        0        0    25444 2024-05-24 12:40:18.913974 pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354103 pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/__init__.py
--rw-r--r--   0        0        0     4649 2024-05-24 15:16:21.496043 pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py
--rw-r--r--   0        0        0     4396 2024-05-24 15:16:21.496301 pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/new_user_account_logging.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353568 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/__init__.py
--rw-r--r--   0        0        0     4569 2024-05-24 15:16:21.496570 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py
--rw-r--r--   0        0        0     9668 2024-05-24 15:16:21.496852 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py
--rw-r--r--   0        0        0     6301 2024-05-24 15:16:21.497132 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py
--rw-r--r--   0        0        0    10170 2024-05-24 15:16:21.497409 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py
--rw-r--r--   0        0        0     5158 2024-05-24 15:16:21.497661 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352474 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/__init__.py
--rw-r--r--   0        0        0     3349 2024-05-24 15:16:21.497893 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py
--rw-r--r--   0        0        0     2854 2024-05-24 15:16:21.498106 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py
--rw-r--r--   0        0        0     2697 2024-05-24 15:16:21.498314 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py
--rw-r--r--   0        0        0     4160 2024-05-24 15:16:21.498569 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py
--rw-r--r--   0        0        0     4357 2024-05-24 15:16:21.498812 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py
--rw-r--r--   0        0        0     3944 2024-05-24 15:16:21.499034 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py
--rw-r--r--   0        0        0     2270 2024-05-24 15:16:21.499318 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py
--rw-r--r--   0        0        0     3341 2024-05-24 15:16:21.499611 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py
--rw-r--r--   0        0        0     3201 2024-05-24 15:16:21.499917 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py
--rw-r--r--   0        0        0     4756 2024-05-24 15:16:21.500167 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py
--rw-r--r--   0        0        0     3421 2024-05-24 15:16:21.500388 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352276 pypanther-0.1.1a3/pypanther/rules/netskope_rules/__init__.py
--rw-r--r--   0        0        0     2974 2024-05-24 15:16:21.500620 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_admin_logged_out.py
--rw-r--r--   0        0        0     3556 2024-05-24 15:16:21.500849 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_admin_user_change.py
--rw-r--r--   0        0        0     2713 2024-05-24 15:16:21.501051 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_many_deletes.py
--rw-r--r--   0        0        0     2902 2024-05-24 15:16:21.501271 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_personnel_action.py
--rw-r--r--   0        0        0     3159 2024-05-24 15:16:21.501490 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353782 pypanther-0.1.1a3/pypanther/rules/notion_rules/__init__.py
--rw-r--r--   0        0        0    16708 2024-05-24 15:16:21.501785 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_account_changed_after_login.py
--rw-r--r--   0        0        0     1529 2024-05-24 12:40:18.870179 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py
--rw-r--r--   0        0        0    15410 2024-05-24 15:16:21.502697 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_login_from_new_location.py
--rw-r--r--   0        0        0     3273 2024-05-24 15:16:21.503542 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_many_pages_deleted.py
--rw-r--r--   0        0        0     3269 2024-05-24 15:16:21.503922 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_many_pages_exported.py
--rw-r--r--   0        0        0     1747 2024-05-24 15:16:21.504555 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_accessible_to_api.py
--rw-r--r--   0        0        0     5395 2024-05-24 15:16:21.504913 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py
--rw-r--r--   0        0        0     1641 2024-05-24 15:16:21.505220 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_shared_to_web.py
--rw-r--r--   0        0        0     2869 2024-05-24 15:16:21.505506 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_scim_token_generated.py
--rw-r--r--   0        0        0     3872 2024-05-24 15:16:21.505825 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_sharing_settings_updated.py
--rw-r--r--   0        0        0     4470 2024-05-24 15:16:21.506092 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_teamspace_owner_added.py
--rw-r--r--   0        0        0     2995 2024-05-24 15:16:21.506343 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py
--rw-r--r--   0        0        0     3264 2024-05-24 15:16:21.506586 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_exported.py
--rw-r--r--   0        0        0     4548 2024-05-24 15:16:21.506857 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py
--rw-r--r--   0        0        0     4402 2024-05-24 15:16:21.507127 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356572 pypanther-0.1.1a3/pypanther/rules/okta_rules/__init__.py
--rw-r--r--   0        0        0     3624 2024-05-24 15:16:21.507388 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_account_support_access.py
--rw-r--r--   0        0        0     3475 2024-05-24 15:16:21.507645 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py
--rw-r--r--   0        0        0     7243 2024-05-24 15:16:21.507905 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_admin_role_assigned.py
--rw-r--r--   0        0        0     7625 2024-05-24 15:16:21.508163 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py
--rw-r--r--   0        0        0     2638 2024-05-24 15:16:21.508396 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_api_key_created.py
--rw-r--r--   0        0        0     2483 2024-05-24 15:16:21.508645 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_api_key_revoked.py
--rw-r--r--   0        0        0     9042 2024-05-24 15:16:21.508933 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py
--rw-r--r--   0        0        0     7515 2024-05-24 15:16:21.509199 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py
--rw-r--r--   0        0        0     7396 2024-05-24 15:16:21.509456 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py
--rw-r--r--   0        0        0     8132 2024-05-24 15:16:21.509731 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_idp_create_modify.py
--rw-r--r--   0        0        0     8222 2024-05-24 12:40:19.414785 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_idp_signin.py
--rw-r--r--   0        0        0    13813 2024-05-24 15:16:21.510023 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py
--rw-r--r--   0        0        0    13457 2024-05-24 15:16:21.510285 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_org2org_creation_modification.py
--rw-r--r--   0        0        0    10936 2024-05-24 15:16:21.510562 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_password_accessed.py
--rw-r--r--   0        0        0     7709 2024-05-24 15:16:21.510819 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py
--rw-r--r--   0        0        0     7652 2024-05-24 15:16:21.511084 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py
--rw-r--r--   0        0        0    19397 2024-05-24 15:16:21.511361 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_potentially_stolen_session.py
--rw-r--r--   0        0        0    10687 2024-05-24 15:16:21.511669 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_rate_limits.py
--rw-r--r--   0        0        0     4995 2024-05-24 15:16:21.511930 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_support_reset.py
--rw-r--r--   0        0        0     9198 2024-05-24 15:16:21.512255 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py
--rw-r--r--   0        0        0     6846 2024-05-24 15:16:21.512684 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_account_locked.py
--rw-r--r--   0        0        0     7006 2024-05-24 15:16:21.513054 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py
--rw-r--r--   0        0        0     4170 2024-05-24 15:16:21.513390 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_reset.py
--rw-r--r--   0        0        0     5452 2024-05-24 15:16:21.513642 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py
--rw-r--r--   0        0        0     8388 2024-05-24 15:16:21.513988 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352956 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/__init__.py
--rw-r--r--   0        0        0     3840 2024-05-24 15:16:21.514248 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py
--rw-r--r--   0        0        0     1955 2024-05-24 15:16:21.514508 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py
--rw-r--r--   0        0        0     2473 2024-05-24 15:16:21.514744 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py
--rw-r--r--   0        0        0     2280 2024-05-24 15:16:21.514994 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_password_accessed.py
--rw-r--r--   0        0        0     2187 2024-05-24 15:16:21.515230 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_password_changed.py
--rw-r--r--   0        0        0     2656 2024-05-24 15:16:21.515454 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py
--rw-r--r--   0        0        0     1879 2024-05-24 15:16:21.515683 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py
--rw-r--r--   0        0        0     1921 2024-05-24 15:16:21.515917 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py
--rw-r--r--   0        0        0     1848 2024-05-24 15:16:21.516156 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py
--rw-r--r--   0        0        0     2545 2024-05-24 15:16:21.516389 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py
--rw-r--r--   0        0        0     1995 2024-05-24 15:16:21.516648 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_user_assumed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353133 pypanther-0.1.1a3/pypanther/rules/onepassword_rules/__init__.py
--rw-r--r--   0        0        0     4565 2024-05-24 12:40:18.700457 pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py
--rw-r--r--   0        0        0     3917 2024-05-24 12:40:18.705317 pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py
--rw-r--r--   0        0        0     4427 2024-05-24 15:16:21.516925 pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_unusual_client.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356027 pypanther-0.1.1a3/pypanther/rules/osquery_rules/__init__.py
--rw-r--r--   0        0        0     4038 2024-05-24 15:16:21.517176 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py
--rw-r--r--   0        0        0     3398 2024-05-24 12:40:19.326027 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py
--rw-r--r--   0        0        0     3580 2024-05-24 15:16:21.517419 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py
--rw-r--r--   0        0        0     2965 2024-05-24 15:16:21.517652 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py
--rw-r--r--   0        0        0     2596 2024-05-24 15:16:21.517917 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py
--rw-r--r--   0        0        0     2203 2024-05-24 15:16:21.518208 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py
--rw-r--r--   0        0        0     4057 2024-05-24 15:16:21.518697 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py
--rw-r--r--   0        0        0     3670 2024-05-24 15:16:21.519188 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py
--rw-r--r--   0        0        0     3472 2024-05-24 15:16:21.519514 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_ossec.py
--rw-r--r--   0        0        0     3545 2024-05-24 15:16:21.519928 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_outdated.py
--rw-r--r--   0        0        0     3674 2024-05-24 15:16:21.520400 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_outdated_macos.py
--rw-r--r--   0        0        0     3730 2024-05-24 15:16:21.520712 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_ssh_listener.py
--rw-r--r--   0        0        0     5583 2024-05-24 15:16:21.521025 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_suspicious_cron.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353388 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/__init__.py
--rw-r--r--   0        0        0     4572 2024-05-24 15:16:21.521335 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_detection_deleted.py
--rw-r--r--   0        0        0     2520 2024-05-24 15:16:21.521649 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_saml_modified.py
--rw-r--r--   0        0        0     8355 2024-05-24 15:16:21.521983 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py
--rw-r--r--   0        0        0     9712 2024-05-24 15:16:21.522331 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_user_modified.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354643 pypanther-0.1.1a3/pypanther/rules/salesforce_rules/__init__.py
--rw-r--r--   0        0        0     4572 2024-05-24 15:16:21.522688 pypanther-0.1.1a3/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353299 pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/__init__.py
--rw-r--r--   0        0        0     7210 2024-05-24 15:16:21.522968 pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py
--rw-r--r--   0        0        0     6468 2024-05-24 15:16:21.523217 pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/sentinelone_threats.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355907 pypanther-0.1.1a3/pypanther/rules/slack_rules/__init__.py
--rw-r--r--   0        0        0    10097 2024-05-24 15:16:21.523488 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_access_expanded.py
--rw-r--r--   0        0        0     8839 2024-05-24 15:16:21.523750 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_added.py
--rw-r--r--   0        0        0     6576 2024-05-24 15:16:21.524038 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_removed.py
--rw-r--r--   0        0        0     4668 2024-05-24 15:16:21.524305 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_application_dos.py
--rw-r--r--   0        0        0     4933 2024-05-24 15:16:21.524549 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_dlp_modified.py
--rw-r--r--   0        0        0     3472 2024-05-24 15:16:21.524759 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_config_changed.py
--rw-r--r--   0        0        0     3415 2024-05-24 15:16:21.524967 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py
--rw-r--r--   0        0        0     3320 2024-05-24 15:16:21.525183 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_unenrolled.py
--rw-r--r--   0        0        0     5881 2024-05-24 15:16:21.525433 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_idp_configuration_change.py
--rw-r--r--   0        0        0     4687 2024-05-24 15:16:21.525677 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_information_barrier_modified.py
--rw-r--r--   0        0        0     3317 2024-05-24 15:16:21.525905 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py
--rw-r--r--   0        0        0     6985 2024-05-24 15:16:21.526152 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py
--rw-r--r--   0        0        0     3440 2024-05-24 15:16:21.526377 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_mfa_settings_changed.py
--rw-r--r--   0        0        0     2829 2024-05-24 15:16:21.526613 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_org_created.py
--rw-r--r--   0        0        0     2829 2024-05-24 15:16:21.526854 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_org_deleted.py
--rw-r--r--   0        0        0     3301 2024-05-24 15:16:21.527063 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_passthrough_anomaly.py
--rw-r--r--   0        0        0     3398 2024-05-24 15:16:21.527272 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py
--rw-r--r--   0        0        0     3578 2024-05-24 15:16:21.527470 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_private_channel_made_public.py
--rw-r--r--   0        0        0     4137 2024-05-24 15:16:21.527694 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py
--rw-r--r--   0        0        0     3543 2024-05-24 15:16:21.527892 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_service_owner_transferred.py
--rw-r--r--   0        0        0     3385 2024-05-24 15:16:21.528118 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_sso_settings_changed.py
--rw-r--r--   0        0        0     7385 2024-05-24 15:16:21.528386 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_user_privilege_escalation.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356824 pypanther-0.1.1a3/pypanther/rules/snyk_rules/__init__.py
--rw-r--r--   0        0        0     2612 2024-05-24 15:16:21.528608 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_misc_settings.py
--rw-r--r--   0        0        0     4557 2024-05-24 15:16:21.528844 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_org_settings.py
--rw-r--r--   0        0        0     4554 2024-05-24 15:16:21.529080 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_ou_change.py
--rw-r--r--   0        0        0     4870 2024-05-24 15:16:21.529343 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_project_settings.py
--rw-r--r--   0        0        0     5423 2024-05-24 15:16:21.529632 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_role_change.py
--rw-r--r--   0        0        0    12013 2024-05-24 15:16:21.529916 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_svcacct_change.py
--rw-r--r--   0        0        0     3957 2024-05-24 15:16:21.530136 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_externalaccess.py
--rw-r--r--   0        0        0     6252 2024-05-24 15:16:21.530401 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_policysetting.py
--rw-r--r--   0        0        0     2564 2024-05-24 15:16:21.530613 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_sso.py
--rw-r--r--   0        0        0     5837 2024-05-24 15:16:21.530857 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_user_mgmt.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352089 pypanther-0.1.1a3/pypanther/rules/standard_rules/__init__.py
--rw-r--r--   0        0        0    10977 2024-05-24 15:16:21.531147 pypanther-0.1.1a3/pypanther/rules/standard_rules/admin_assigned.py
--rw-r--r--   0        0        0    16941 2024-05-24 15:16:21.531423 pypanther-0.1.1a3/pypanther/rules/standard_rules/brute_force_by_ip.py
--rw-r--r--   0        0        0    36744 2024-05-24 15:16:21.531830 pypanther-0.1.1a3/pypanther/rules/standard_rules/impossible_travel_login.py
--rw-r--r--   0        0        0     9765 2024-05-24 12:40:18.497546 pypanther-0.1.1a3/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py
--rw-r--r--   0        0        0     8211 2024-05-24 15:16:21.532115 pypanther-0.1.1a3/pypanther/rules/standard_rules/mfa_disabled.py
--rw-r--r--   0        0        0     9929 2024-05-24 12:40:18.501241 pypanther-0.1.1a3/pypanther/rules/standard_rules/standard_dns_base64.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353861 pypanther-0.1.1a3/pypanther/rules/tailscale_rules/__init__.py
--rw-r--r--   0        0        0     4635 2024-05-24 15:16:21.532365 pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_https_disabled.py
--rw-r--r--   0        0        0     4871 2024-05-24 15:16:21.532637 pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py
--rw-r--r--   0        0        0     4652 2024-05-24 15:16:21.532895 pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356684 pypanther-0.1.1a3/pypanther/rules/tines_rules/__init__.py
--rw-r--r--   0        0        0     2570 2024-05-24 15:16:21.533184 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_actions_disabled_changes.py
--rw-r--r--   0        0        0     2810 2024-05-24 15:16:21.533820 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_custom_ca.py
--rw-r--r--   0        0        0     3526 2024-05-24 15:16:21.534457 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py
--rw-r--r--   0        0        0     2873 2024-05-24 15:16:21.534800 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_global_resource_destruction.py
--rw-r--r--   0        0        0     2933 2024-05-24 15:16:21.535126 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_sso_settings.py
--rw-r--r--   0        0        0     2751 2024-05-24 15:16:21.535504 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_story_items_destruction.py
--rw-r--r--   0        0        0     2721 2024-05-24 15:16:21.535880 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_story_jobs_clearance.py
--rw-r--r--   0        0        0     2666 2024-05-24 15:16:21.536177 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_team_destruction.py
--rw-r--r--   0        0        0     3973 2024-05-24 15:16:21.536516 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_tenant_authtoken.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352185 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/__init__.py
--rw-r--r--   0        0        0     3761 2024-05-24 15:16:21.536795 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py
--rw-r--r--   0        0        0     2958 2024-05-24 15:16:21.537085 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_new_api_token.py
--rw-r--r--   0        0        0     3194 2024-05-24 15:16:21.537365 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_new_owner.py
--rw-r--r--   0        0        0     3703 2024-05-24 15:16:21.537713 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py
--rw-r--r--   0        0        0     2948 2024-05-24 15:16:21.538004 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_assumption.py
--rw-r--r--   0        0        0     2760 2024-05-24 15:16:21.538287 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_role.py
--rw-r--r--   0        0        0     3913 2024-05-24 15:16:21.538522 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_suspension.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353216 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/__init__.py
--rw-r--r--   0        0        0     2676 2024-05-24 15:16:21.538757 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py
--rw-r--r--   0        0        0     2345 2024-05-24 15:16:21.538977 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py
--rw-r--r--   0        0        0     2816 2024-05-24 15:16:21.539207 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py
--rw-r--r--   0        0        0     2746 2024-05-24 15:16:21.539448 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py
--rw-r--r--   0        0        0     3344 2024-05-24 15:16:21.539654 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py
--rw-r--r--   0        0        0     3544 2024-05-24 15:16:21.539868 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py
--rw-r--r--   0        0        0     2606 2024-05-24 15:16:21.540096 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py
--rw-r--r--   0        0        0     4606 2024-05-24 15:16:21.540333 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py
--rw-r--r--   0        0        0     4490 2024-05-24 13:47:47.095050 pypanther-0.1.1a3/pypanther/upload.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095097 pypanther-0.1.1a3/pypanther/vendor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095354 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095410 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/__init__.py
--rw-r--r--   0        0        0    16541 2024-05-24 13:47:47.095519 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/client.py
--rw-r--r--   0        0        0      624 2024-05-24 13:47:47.095629 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/errors.py
--rw-r--r--   0        0        0      159 2024-05-24 13:47:47.095796 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload.graphql
--rw-r--r--   0        0        0      802 2024-05-24 13:47:47.095929 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql
--rw-r--r--   0        0        0     1439 2024-05-24 17:25:24.652928 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql
--rw-r--r--   0        0        0    13035 2024-05-24 13:47:47.096074 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/lambda_client.py
--rw-r--r--   0        0        0    25446 2024-05-24 13:47:47.096146 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py
--rw-r--r--   0        0        0     1606 2024-05-24 13:47:47.096405 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/cli_output.py
--rw-r--r--   0        0        0      738 2024-05-24 13:47:47.096498 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/command/standard_args.py
--rw-r--r--   0        0        0      676 2024-05-24 13:47:47.096574 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/constants.py
--rw-r--r--   0        0        0     2541 2024-05-24 13:47:47.096824 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/util.py
--rw-r--r--   0        0        0      274 2024-05-23 22:00:33.355426 pypanther-0.1.1a3/pypanther/wrap.py
--rw-r--r--   0        0        0     1720 2024-05-24 17:25:24.653486 pypanther-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 pypanther-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-22 19:16:21.930547 pypanther-0.1.1a8/LICENSE.txt
+-rw-r--r--   0        0        0       80 2024-05-03 18:47:26.705553 pypanther-0.1.1a8/README.md
+-rw-r--r--   0        0        0      185 2024-05-23 22:00:33.237693 pypanther-0.1.1a8/pypanther/__init__.py
+-rw-r--r--   0        0        0    24670 2024-05-28 19:11:58.339442 pypanther-0.1.1a8/pypanther/base.py
+-rw-r--r--   0        0        0      490 2024-05-23 22:00:33.238107 pypanther-0.1.1a8/pypanther/cache.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:14.952849 pypanther-0.1.1a8/pypanther/data_models/__init__.py
+-rw-r--r--   0        0        0     1387 2024-05-24 12:40:14.944512 pypanther-0.1.1a8/pypanther/data_models/asana_data_model.py
+-rw-r--r--   0        0        0     1544 2024-05-24 12:40:14.933036 pypanther-0.1.1a8/pypanther/data_models/atlassian_data_model.py
+-rw-r--r--   0        0        0      607 2024-05-24 12:40:14.942246 pypanther-0.1.1a8/pypanther/data_models/aws_alb_data_model.py
+-rw-r--r--   0        0        0     2214 2024-05-24 12:40:14.938734 pypanther-0.1.1a8/pypanther/data_models/aws_cloudtrail_data_model.py
+-rw-r--r--   0        0        0     1465 2024-05-24 12:40:14.929894 pypanther-0.1.1a8/pypanther/data_models/aws_eks_data_model.py
+-rw-r--r--   0        0        0      630 2024-05-24 12:40:14.936327 pypanther-0.1.1a8/pypanther/data_models/aws_s3_data_model.py
+-rw-r--r--   0        0        0      593 2024-05-24 12:40:14.939270 pypanther-0.1.1a8/pypanther/data_models/aws_vpcdns_data_model.py
+-rw-r--r--   0        0        0      742 2024-05-24 12:40:14.928634 pypanther-0.1.1a8/pypanther/data_models/aws_vpcflow_data_model.py
+-rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.927521 pypanther-0.1.1a8/pypanther/data_models/azure_signin_data_model.py
+-rw-r--r--   0        0        0      941 2024-05-24 12:40:14.941146 pypanther-0.1.1a8/pypanther/data_models/box_data_model.py
+-rw-r--r--   0        0        0      873 2024-05-24 12:40:14.939822 pypanther-0.1.1a8/pypanther/data_models/cisco_umbrella_data_model.py
+-rw-r--r--   0        0        0      653 2024-05-24 12:40:14.943897 pypanther-0.1.1a8/pypanther/data_models/cloudflare_firewall_data_model.py
+-rw-r--r--   0        0        0      729 2024-05-24 12:40:14.928057 pypanther-0.1.1a8/pypanther/data_models/cloudflare_httpreq_data_model.py
+-rw-r--r--   0        0        0     1853 2024-05-24 12:40:14.943403 pypanther-0.1.1a8/pypanther/data_models/crowdstrike_fdr_data_model.py
+-rw-r--r--   0        0        0     5215 2024-05-24 12:40:14.934292 pypanther-0.1.1a8/pypanther/data_models/gcp_data_model.py
+-rw-r--r--   0        0        0     1613 2024-05-24 12:40:14.937900 pypanther-0.1.1a8/pypanther/data_models/github_data_model.py
+-rw-r--r--   0        0        0     1669 2024-05-24 12:40:14.935584 pypanther-0.1.1a8/pypanther/data_models/gsuite_data_model.py
+-rw-r--r--   0        0        0     1864 2024-05-24 12:40:14.940562 pypanther-0.1.1a8/pypanther/data_models/notion_data_model.py
+-rw-r--r--   0        0        0     2070 2024-05-24 12:40:14.937166 pypanther-0.1.1a8/pypanther/data_models/okta_data_model.py
+-rw-r--r--   0        0        0     1467 2024-05-24 12:40:14.932330 pypanther-0.1.1a8/pypanther/data_models/onelogin_data_model.py
+-rw-r--r--   0        0        0      730 2024-05-24 12:40:14.934876 pypanther-0.1.1a8/pypanther/data_models/onepassword_itemusage_data_model.py
+-rw-r--r--   0        0        0     1058 2024-05-24 12:40:14.941731 pypanther-0.1.1a8/pypanther/data_models/onepassword_signinattempt_data_model.py
+-rw-r--r--   0        0        0     1742 2024-05-24 12:40:14.930685 pypanther-0.1.1a8/pypanther/data_models/panther_audit_data_model.py
+-rw-r--r--   0        0        0      613 2024-05-24 12:40:14.929135 pypanther-0.1.1a8/pypanther/data_models/slack_accesslogs_data_model.py
+-rw-r--r--   0        0        0      711 2024-05-24 12:40:14.942793 pypanther-0.1.1a8/pypanther/data_models/slack_auditlogs_data_model.py
+-rw-r--r--   0        0        0      500 2024-05-24 12:40:14.926474 pypanther-0.1.1a8/pypanther/data_models/slack_integrationlogs_data_model.py
+-rw-r--r--   0        0        0     2714 2024-05-24 12:40:14.931651 pypanther-0.1.1a8/pypanther/data_models/zendesk_data_model.py
+-rw-r--r--   0        0        0      886 2024-05-24 12:40:14.926019 pypanther-0.1.1a8/pypanther/data_models/zoom_activity_data_model.py
+-rw-r--r--   0        0        0     1887 2024-05-24 12:40:14.925345 pypanther-0.1.1a8/pypanther/data_models/zoom_operation_data_model.py
+-rw-r--r--   0        0        0     2682 2024-05-23 22:00:33.243958 pypanther-0.1.1a8/pypanther/get.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:13.778915 pypanther-0.1.1a8/pypanther/helpers/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-24 12:40:14.169513 pypanther-0.1.1a8/pypanther/helpers/gcp_base_helpers.py
+-rw-r--r--   0        0        0      781 2024-05-24 12:40:14.303335 pypanther-0.1.1a8/pypanther/helpers/gcp_environment.py
+-rw-r--r--   0        0        0     1417 2024-05-24 12:40:13.948393 pypanther-0.1.1a8/pypanther/helpers/panther_asana_helpers.py
+-rw-r--r--   0        0        0     1597 2024-05-24 12:40:14.156772 pypanther-0.1.1a8/pypanther/helpers/panther_audit.py
+-rw-r--r--   0        0        0      555 2024-05-24 12:40:13.952837 pypanther-0.1.1a8/pypanther/helpers/panther_auth0_helpers.py
+-rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.099017 pypanther-0.1.1a8/pypanther/helpers/panther_azuresignin_helpers.py
+-rw-r--r--   0        0        0    19692 2024-05-24 12:40:14.264799 pypanther-0.1.1a8/pypanther/helpers/panther_base_helpers.py
+-rw-r--r--   0        0        0     4529 2024-05-24 12:40:14.146111 pypanther-0.1.1a8/pypanther/helpers/panther_box_helpers.py
+-rw-r--r--   0        0        0     2267 2024-05-24 12:40:13.916642 pypanther-0.1.1a8/pypanther/helpers/panther_cloudflare_helpers.py
+-rw-r--r--   0        0        0      507 2024-05-24 12:40:14.148779 pypanther-0.1.1a8/pypanther/helpers/panther_config.py
+-rw-r--r--   0        0        0      891 2024-05-24 12:40:14.103142 pypanther-0.1.1a8/pypanther/helpers/panther_config_defaults.py
+-rw-r--r--   0        0        0     1043 2024-05-24 12:40:13.795713 pypanther-0.1.1a8/pypanther/helpers/panther_config_overrides.py
+-rw-r--r--   0        0        0     3465 2024-05-24 12:40:13.831736 pypanther-0.1.1a8/pypanther/helpers/panther_default.py
+-rw-r--r--   0        0        0     1288 2024-05-24 12:40:13.811022 pypanther-0.1.1a8/pypanther/helpers/panther_duo_helpers.py
+-rw-r--r--   0        0        0     1118 2024-05-24 12:40:14.384435 pypanther-0.1.1a8/pypanther/helpers/panther_event_type_helpers.py
+-rw-r--r--   0        0        0    12436 2024-05-24 12:40:14.482779 pypanther-0.1.1a8/pypanther/helpers/panther_greynoise_helpers.py
+-rw-r--r--   0        0        0    38305 2024-05-24 12:40:13.902461 pypanther-0.1.1a8/pypanther/helpers/panther_iocs.py
+-rw-r--r--   0        0        0     6497 2024-05-24 12:40:14.002454 pypanther-0.1.1a8/pypanther/helpers/panther_ipinfo_helpers.py
+-rw-r--r--   0        0        0     2154 2024-05-24 12:40:14.015836 pypanther-0.1.1a8/pypanther/helpers/panther_lookuptable_helpers.py
+-rw-r--r--   0        0        0      387 2024-05-24 12:40:14.270284 pypanther-0.1.1a8/pypanther/helpers/panther_mongodb_helpers.py
+-rw-r--r--   0        0        0      340 2024-05-24 12:40:13.834434 pypanther-0.1.1a8/pypanther/helpers/panther_notion_helpers.py
+-rw-r--r--   0        0        0    13096 2024-05-24 12:40:14.370655 pypanther-0.1.1a8/pypanther/helpers/panther_oss_helpers.py
+-rw-r--r--   0        0        0      610 2024-05-24 12:40:13.801982 pypanther-0.1.1a8/pypanther/helpers/panther_snyk_helpers.py
+-rw-r--r--   0        0        0      492 2024-05-24 12:40:14.307780 pypanther-0.1.1a8/pypanther/helpers/panther_tailscale_helpers.py
+-rw-r--r--   0        0        0      567 2024-05-24 12:40:14.312664 pypanther-0.1.1a8/pypanther/helpers/panther_tines_helpers.py
+-rw-r--r--   0        0        0     1542 2024-05-24 12:40:14.379643 pypanther-0.1.1a8/pypanther/helpers/panther_tor_helpers.py
+-rw-r--r--   0        0        0     3084 2024-05-24 12:40:13.935600 pypanther-0.1.1a8/pypanther/helpers/panther_zoom_helpers.py
+-rw-r--r--   0        0        0    13022 2024-05-23 22:06:29.350498 pypanther-0.1.1a8/pypanther/log_types.py
+-rw-r--r--   0        0        0     1134 2024-05-28 18:40:51.829160 pypanther-0.1.1a8/pypanther/main.py
+-rw-r--r--   0        0        0        0 2024-05-28 18:40:51.829203 pypanther-0.1.1a8/pypanther/py.typed
+-rw-r--r--   0        0        0      824 2024-05-23 22:00:33.250813 pypanther-0.1.1a8/pypanther/register.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.351956 pypanther-0.1.1a8/pypanther/rules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356408 pypanther-0.1.1a8/pypanther/rules/asana_rules/__init__.py
+-rw-r--r--   0        0        0     4069 2024-05-28 19:11:58.340050 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_service_account_created.py
+-rw-r--r--   0        0        0     3241 2024-05-28 19:11:58.340466 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_team_privacy_public.py
+-rw-r--r--   0        0        0     3263 2024-05-28 19:11:58.340767 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py
+-rw-r--r--   0        0        0     3232 2024-05-28 19:11:58.341082 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py
+-rw-r--r--   0        0        0     3420 2024-05-28 19:11:58.341520 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py
+-rw-r--r--   0        0        0     3399 2024-05-28 19:11:58.341677 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py
+-rw-r--r--   0        0        0     3747 2024-05-28 19:11:58.342105 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_new_admin.py
+-rw-r--r--   0        0        0     3242 2024-05-28 19:11:58.342563 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_org_export.py
+-rw-r--r--   0        0        0     3725 2024-05-28 19:11:58.342710 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py
+-rw-r--r--   0        0        0     3629 2024-05-28 19:11:58.342855 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py
+-rw-r--r--   0        0        0     3498 2024-05-28 19:11:58.343001 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_saml_optional.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355786 pypanther-0.1.1a8/pypanther/rules/atlassian_rules/__init__.py
+-rw-r--r--   0        0        0     4891 2024-05-28 19:11:58.343684 pypanther-0.1.1a8/pypanther/rules/atlassian_rules/user_logged_in_as_user.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352374 pypanther-0.1.1a8/pypanther/rules/auth0_rules/__init__.py
+-rw-r--r--   0        0        0    45000 2024-05-28 19:11:58.344253 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_custom_role_created.py
+-rw-r--r--   0        0        0    15426 2024-05-28 19:11:58.344617 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_integration_installed.py
+-rw-r--r--   0        0        0    23152 2024-05-28 19:11:58.344806 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py
+-rw-r--r--   0        0        0    23502 2024-05-28 19:11:58.345555 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py
+-rw-r--r--   0        0        0    34173 2024-05-28 19:11:58.345780 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py
+-rw-r--r--   0        0        0    23656 2024-05-28 19:11:58.346271 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py
+-rw-r--r--   0        0        0    22677 2024-05-28 19:11:58.346886 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py
+-rw-r--r--   0        0        0    19831 2024-05-28 19:11:58.347527 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py
+-rw-r--r--   0        0        0    17293 2024-05-28 19:11:58.347839 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_user_invitation_created.py
+-rw-r--r--   0        0        0    18180 2024-05-28 19:11:58.348413 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354895 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/__init__.py
+-rw-r--r--   0        0        0    11023 2024-05-28 19:11:58.349277 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py
+-rw-r--r--   0        0        0     8203 2024-05-28 19:11:58.349480 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py
+-rw-r--r--   0        0        0     7052 2024-05-28 19:11:58.349705 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py
+-rw-r--r--   0        0        0     3387 2024-05-28 19:11:58.349922 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py
+-rw-r--r--   0        0        0     7226 2024-05-28 19:11:58.350335 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py
+-rw-r--r--   0        0        0     4474 2024-05-28 19:11:58.350937 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py
+-rw-r--r--   0        0        0     7006 2024-05-28 19:11:58.351155 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py
+-rw-r--r--   0        0        0     6565 2024-05-28 19:11:58.351374 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py
+-rw-r--r--   0        0        0     6552 2024-05-28 19:11:58.351972 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py
+-rw-r--r--   0        0        0    20565 2024-05-28 19:11:58.352382 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py
+-rw-r--r--   0        0        0     4041 2024-05-28 19:11:58.352970 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py
+-rw-r--r--   0        0        0     5610 2024-05-28 19:11:58.353229 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py
+-rw-r--r--   0        0        0     5713 2024-05-28 19:11:58.353455 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py
+-rw-r--r--   0        0        0     2295 2024-05-28 19:11:58.353621 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py
+-rw-r--r--   0        0        0     6726 2024-05-28 19:11:58.354018 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py
+-rw-r--r--   0        0        0    17207 2024-05-28 19:11:58.354349 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py
+-rw-r--r--   0        0        0    22420 2024-05-28 19:11:58.354703 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py
+-rw-r--r--   0        0        0     7258 2024-05-28 19:11:58.354938 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py
+-rw-r--r--   0        0        0     6888 2024-05-28 19:11:58.355449 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py
+-rw-r--r--   0        0        0     8185 2024-05-28 19:11:58.355672 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py
+-rw-r--r--   0        0        0     5173 2024-05-28 19:11:58.355869 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py
+-rw-r--r--   0        0        0    30283 2024-05-28 19:11:58.356080 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py
+-rw-r--r--   0        0        0     8614 2024-05-28 19:11:58.356309 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py
+-rw-r--r--   0        0        0    39743 2024-05-28 19:11:58.356657 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py
+-rw-r--r--   0        0        0    27333 2024-05-28 19:11:58.357147 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py
+-rw-r--r--   0        0        0    26742 2024-05-28 19:11:58.357329 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py
+-rw-r--r--   0        0        0     7276 2024-05-28 19:11:58.357539 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py
+-rw-r--r--   0        0        0     8595 2024-05-28 19:11:58.357722 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py
+-rw-r--r--   0        0        0     6119 2024-05-28 19:11:58.358232 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py
+-rw-r--r--   0        0        0    12719 2024-05-28 19:11:58.358560 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py
+-rw-r--r--   0        0        0    13763 2024-05-28 19:11:58.358785 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py
+-rw-r--r--   0        0        0     7154 2024-05-28 19:11:58.358990 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py
+-rw-r--r--   0        0        0    10491 2024-05-28 19:11:58.359146 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py
+-rw-r--r--   0        0        0     9050 2024-05-28 19:11:58.359334 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py
+-rw-r--r--   0        0        0     3389 2024-05-28 19:11:58.359556 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py
+-rw-r--r--   0        0        0     5216 2024-05-28 19:11:58.359740 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py
+-rw-r--r--   0        0        0    11264 2024-05-28 19:11:58.360006 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py
+-rw-r--r--   0        0        0     5730 2024-05-28 19:11:58.360189 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py
+-rw-r--r--   0        0        0     9734 2024-05-28 19:11:58.360403 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py
+-rw-r--r--   0        0        0    27000 2024-05-28 19:11:58.360729 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py
+-rw-r--r--   0        0        0     7827 2024-05-28 19:11:58.360968 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py
+-rw-r--r--   0        0        0    16376 2024-05-28 19:11:58.361181 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py
+-rw-r--r--   0        0        0    14639 2024-05-28 19:11:58.361366 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py
+-rw-r--r--   0        0        0    17400 2024-05-28 19:11:58.361535 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py
+-rw-r--r--   0        0        0     7480 2024-05-28 19:11:58.361741 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py
+-rw-r--r--   0        0        0    18982 2024-05-28 19:11:58.361903 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py
+-rw-r--r--   0        0        0     4669 2024-05-28 19:11:58.362111 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py
+-rw-r--r--   0        0        0    10753 2024-05-28 19:11:58.362414 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py
+-rw-r--r--   0        0        0     3934 2024-05-28 19:11:58.362563 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py
+-rw-r--r--   0        0        0     5825 2024-05-28 19:11:58.362754 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py
+-rw-r--r--   0        0        0     7516 2024-05-28 19:11:58.362968 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py
+-rw-r--r--   0        0        0    12289 2024-05-28 19:11:58.363162 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py
+-rw-r--r--   0        0        0    11516 2024-05-28 19:11:58.363357 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py
+-rw-r--r--   0        0        0     5570 2024-05-28 19:11:58.363567 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py
+-rw-r--r--   0        0        0     7558 2024-05-28 19:11:58.363804 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py
+-rw-r--r--   0        0        0     5191 2024-05-28 19:11:58.364017 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py
+-rw-r--r--   0        0        0     6478 2024-05-28 19:11:58.364344 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py
+-rw-r--r--   0        0        0     8697 2024-05-28 19:11:58.364595 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py
+-rw-r--r--   0        0        0     5976 2024-05-28 19:11:58.364841 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py
+-rw-r--r--   0        0        0     6782 2024-05-28 19:11:58.365067 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py
+-rw-r--r--   0        0        0     7024 2024-05-28 19:11:58.365361 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352785 pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/__init__.py
+-rw-r--r--   0        0        0     9700 2024-05-28 19:11:58.365585 pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py
+-rw-r--r--   0        0        0    17813 2024-05-28 19:11:58.365877 pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354748 pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/__init__.py
+-rw-r--r--   0        0        0     5370 2024-05-28 19:11:58.366101 pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py
+-rw-r--r--   0        0        0     5391 2024-05-28 19:11:58.366424 pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py
+-rw-r--r--   0        0        0     5417 2024-05-28 19:11:58.366618 pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355307 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/__init__.py
+-rw-r--r--   0        0        0     4702 2024-05-28 19:11:58.366952 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_access_error.py
+-rw-r--r--   0        0        0     2560 2024-05-28 19:11:58.367226 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py
+-rw-r--r--   0        0        0     6277 2024-05-28 19:11:58.367425 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py
+-rw-r--r--   0        0        0     1997 2024-05-28 19:11:58.367601 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py
+-rw-r--r--   0        0        0     8748 2024-05-28 19:11:58.367853 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355429 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/__init__.py
+-rw-r--r--   0        0        0     6790 2024-05-28 19:11:58.368287 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py
+-rw-r--r--   0        0        0     1340 2024-05-28 19:11:58.368494 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py
+-rw-r--r--   0        0        0     2538 2024-05-28 19:11:58.368664 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py
+-rw-r--r--   0        0        0     2498 2024-05-28 19:11:58.368815 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py
+-rw-r--r--   0        0        0     2927 2024-05-28 19:11:58.368969 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355171 pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/__init__.py
+-rw-r--r--   0        0        0     7978 2024-05-28 19:11:58.369185 pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_failed_signins.py
+-rw-r--r--   0        0        0    15766 2024-05-28 19:11:58.369374 pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_legacyauth.py
+-rw-r--r--   0        0        0    17553 2024-05-28 19:11:58.369593 pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353050 pypanther-0.1.1a8/pypanther/rules/box_rules/__init__.py
+-rw-r--r--   0        0        0     2134 2024-05-28 19:11:58.369784 pypanther-0.1.1a8/pypanther/rules/box_rules/box_access_granted.py
+-rw-r--r--   0        0        0     2869 2024-05-28 19:11:58.369971 pypanther-0.1.1a8/pypanther/rules/box_rules/box_anomalous_download.py
+-rw-r--r--   0        0        0     2744 2024-05-28 19:11:58.370506 pypanther-0.1.1a8/pypanther/rules/box_rules/box_event_triggered_externally.py
+-rw-r--r--   0        0        0     3652 2024-05-28 19:11:58.370679 pypanther-0.1.1a8/pypanther/rules/box_rules/box_item_shared_externally.py
+-rw-r--r--   0        0        0     4266 2024-05-28 19:11:58.371060 pypanther-0.1.1a8/pypanther/rules/box_rules/box_malicious_content.py
+-rw-r--r--   0        0        0     2124 2024-05-28 19:11:58.371239 pypanther-0.1.1a8/pypanther/rules/box_rules/box_new_login.py
+-rw-r--r--   0        0        0     2822 2024-05-28 19:11:58.371408 pypanther-0.1.1a8/pypanther/rules/box_rules/box_policy_violation.py
+-rw-r--r--   0        0        0     4215 2024-05-28 19:11:58.371707 pypanther-0.1.1a8/pypanther/rules/box_rules/box_suspicious_login_or_session.py
+-rw-r--r--   0        0        0     2226 2024-05-28 19:11:58.371941 pypanther-0.1.1a8/pypanther/rules/box_rules/box_untrusted_device.py
+-rw-r--r--   0        0        0     2366 2024-05-28 19:11:58.372118 pypanther-0.1.1a8/pypanther/rules/box_rules/box_user_downloads.py
+-rw-r--r--   0        0        0     3179 2024-05-28 19:11:58.372430 pypanther-0.1.1a8/pypanther/rules/box_rules/box_user_permission_updates.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355655 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/__init__.py
+-rw-r--r--   0        0        0     3313 2024-05-28 19:11:58.372652 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py
+-rw-r--r--   0        0        0     3037 2024-05-28 19:11:58.372849 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py
+-rw-r--r--   0        0        0     3487 2024-05-28 19:11:58.373044 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py
+-rw-r--r--   0        0        0     2262 2024-05-28 19:11:58.373233 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_flagged.py
+-rw-r--r--   0        0        0     2591 2024-05-28 19:11:58.373422 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py
+-rw-r--r--   0        0        0    11317 2024-05-28 19:11:58.373640 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355556 pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/__init__.py
+-rw-r--r--   0        0        0     1801 2024-05-28 19:11:58.373825 pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py
+-rw-r--r--   0        0        0     1428 2024-05-28 19:11:58.374022 pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py
+-rw-r--r--   0        0        0     1917 2024-05-28 19:11:58.374212 pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354017 pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/__init__.py
+-rw-r--r--   0        0        0     4983 2024-05-28 19:11:58.374471 pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py
+-rw-r--r--   0        0        0     7577 2024-05-28 19:11:58.374729 pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355030 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/__init__.py
+-rw-r--r--   0        0        0    29399 2024-05-28 19:11:58.374939 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py
+-rw-r--r--   0        0        0     8191 2024-05-28 19:11:58.375218 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py
+-rw-r--r--   0        0        0     9907 2024-05-28 19:11:58.375469 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py
+-rw-r--r--   0        0        0     9869 2024-05-28 19:11:58.375719 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py
+-rw-r--r--   0        0        0    10434 2024-05-28 19:11:58.376157 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py
+-rw-r--r--   0        0        0    12191 2024-05-28 19:11:58.376404 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py
+-rw-r--r--   0        0        0    11725 2024-05-28 19:11:58.376639 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py
+-rw-r--r--   0        0        0    18694 2024-05-28 19:11:58.376794 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py
+-rw-r--r--   0        0        0    18901 2024-05-28 19:11:58.376982 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py
+-rw-r--r--   0        0        0    15628 2024-05-28 19:11:58.377171 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py
+-rw-r--r--   0        0        0     7222 2024-05-28 19:11:58.377382 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py
+-rw-r--r--   0        0        0     9736 2024-05-28 19:11:58.377566 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py
+-rw-r--r--   0        0        0    13608 2024-05-28 19:11:58.377757 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py
+-rw-r--r--   0        0        0     9717 2024-05-28 19:11:58.377927 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py
+-rw-r--r--   0        0        0    10020 2024-05-28 19:11:58.378100 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py
+-rw-r--r--   0        0        0    17371 2024-05-28 19:11:58.378268 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354190 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/__init__.py
+-rw-r--r--   0        0        0     6807 2024-05-28 19:11:58.378520 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py
+-rw-r--r--   0        0        0     9508 2024-05-28 19:11:58.378771 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_external_share.py
+-rw-r--r--   0        0        0     8252 2024-05-28 19:11:58.379036 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py
+-rw-r--r--   0        0        0    11156 2024-05-28 19:11:58.379219 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py
+-rw-r--r--   0        0        0     5145 2024-05-28 19:11:58.379541 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353471 pypanther-0.1.1a8/pypanther/rules/duo_rules/__init__.py
+-rw-r--r--   0        0        0     2102 2024-05-28 19:11:58.379913 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py
+-rw-r--r--   0        0        0     2189 2024-05-28 19:11:58.380116 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py
+-rw-r--r--   0        0        0     2258 2024-05-28 19:11:58.380276 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py
+-rw-r--r--   0        0        0     2255 2024-05-28 19:11:58.380442 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_create_admin.py
+-rw-r--r--   0        0        0     2522 2024-05-28 19:11:58.380597 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_lockout.py
+-rw-r--r--   0        0        0     2672 2024-05-28 19:11:58.380740 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py
+-rw-r--r--   0        0        0     1982 2024-05-28 19:11:58.380887 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py
+-rw-r--r--   0        0        0     3158 2024-05-28 19:11:58.381045 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py
+-rw-r--r--   0        0        0     2222 2024-05-28 19:11:58.381189 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_policy_updated.py
+-rw-r--r--   0        0        0     3390 2024-05-28 19:11:58.381334 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py
+-rw-r--r--   0        0        0     2916 2024-05-28 19:11:58.381485 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py
+-rw-r--r--   0        0        0     2042 2024-05-28 19:11:58.381623 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_action_fraudulent.py
+-rw-r--r--   0        0        0     3166 2024-05-28 19:11:58.381800 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_anomalous_push.py
+-rw-r--r--   0        0        0     3072 2024-05-28 19:11:58.381953 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_bypass_code_used.py
+-rw-r--r--   0        0        0     5464 2024-05-28 19:11:58.382162 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353698 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/__init__.py
+-rw-r--r--   0        0        0     9853 2024-05-28 19:11:58.382382 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py
+-rw-r--r--   0        0        0    12347 2024-05-28 19:11:58.382595 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py
+-rw-r--r--   0        0        0     7059 2024-05-28 19:11:58.382832 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py
+-rw-r--r--   0        0        0     7853 2024-05-28 19:11:58.383041 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py
+-rw-r--r--   0        0        0     4141 2024-05-28 19:11:58.383240 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py
+-rw-r--r--   0        0        0     4141 2024-05-28 19:11:58.383531 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py
+-rw-r--r--   0        0        0    19142 2024-05-28 19:11:58.383866 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py
+-rw-r--r--   0        0        0    10446 2024-05-28 19:11:58.384113 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py
+-rw-r--r--   0        0        0    15447 2024-05-28 19:11:58.384321 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py
+-rw-r--r--   0        0        0     9163 2024-05-28 19:11:58.384509 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py
+-rw-r--r--   0        0        0     6832 2024-05-28 19:11:58.384716 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py
+-rw-r--r--   0        0        0     8955 2024-05-28 19:11:58.384901 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py
+-rw-r--r--   0        0        0     3845 2024-05-28 19:11:58.385062 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py
+-rw-r--r--   0        0        0     4541 2024-05-28 19:11:58.385247 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py
+-rw-r--r--   0        0        0    15807 2024-05-28 19:11:58.385445 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py
+-rw-r--r--   0        0        0     5283 2024-05-28 19:11:58.385683 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py
+-rw-r--r--   0        0        0     9955 2024-05-28 19:11:58.385873 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py
+-rw-r--r--   0        0        0     3593 2024-05-28 19:11:58.386054 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py
+-rw-r--r--   0        0        0     4129 2024-05-28 19:11:58.386250 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py
+-rw-r--r--   0        0        0     6799 2024-05-28 19:11:58.386458 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py
+-rw-r--r--   0        0        0     6599 2024-05-28 19:11:58.386658 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py
+-rw-r--r--   0        0        0     7318 2024-05-28 19:11:58.386850 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py
+-rw-r--r--   0        0        0     9277 2024-05-28 19:11:58.387038 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py
+-rw-r--r--   0        0        0    11308 2024-05-28 19:11:58.387279 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py
+-rw-r--r--   0        0        0     7629 2024-05-28 19:11:58.387601 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py
+-rw-r--r--   0        0        0     7093 2024-05-28 19:11:58.387853 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py
+-rw-r--r--   0        0        0    10621 2024-05-28 19:11:58.388047 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py
+-rw-r--r--   0        0        0     4082 2024-05-28 19:11:58.388203 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py
+-rw-r--r--   0        0        0     7728 2024-05-28 19:11:58.388401 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py
+-rw-r--r--   0        0        0    11756 2024-05-28 19:11:58.389095 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py
+-rw-r--r--   0        0        0    10830 2024-05-28 19:11:58.389332 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py
+-rw-r--r--   0        0        0     2289 2024-05-28 19:11:58.389500 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py
+-rw-r--r--   0        0        0     2925 2024-05-28 19:11:58.389669 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py
+-rw-r--r--   0        0        0    13072 2024-05-28 19:11:58.389871 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py
+-rw-r--r--   0        0        0    10924 2024-05-28 19:11:58.390057 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py
+-rw-r--r--   0        0        0     9640 2024-05-28 19:11:58.390240 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py
+-rw-r--r--   0        0        0    10178 2024-05-28 19:11:58.390442 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py
+-rw-r--r--   0        0        0    11781 2024-05-28 19:11:58.390626 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352868 pypanther-0.1.1a8/pypanther/rules/gcp_http_lb_rules/__init__.py
+-rw-r--r--   0        0        0     5922 2024-05-28 19:11:58.390838 pypanther-0.1.1a8/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356266 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/__init__.py
+-rw-r--r--   0        0        0     4573 2024-05-28 19:11:58.391039 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py
+-rw-r--r--   0        0        0     6715 2024-05-28 19:11:58.391235 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py
+-rw-r--r--   0        0        0     2265 2024-05-28 19:11:58.391388 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py
+-rw-r--r--   0        0        0     3544 2024-05-28 19:11:58.391522 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py
+-rw-r--r--   0        0        0     3447 2024-05-28 19:11:58.391661 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py
+-rw-r--r--   0        0        0    12881 2024-05-28 19:11:58.391861 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py
+-rw-r--r--   0        0        0     3513 2024-05-28 19:11:58.391996 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py
+-rw-r--r--   0        0        0    14892 2024-05-28 19:11:58.392170 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py
+-rw-r--r--   0        0        0    11476 2024-05-28 19:11:58.392357 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352570 pypanther-0.1.1a8/pypanther/rules/github_rules/__init__.py
+-rw-r--r--   0        0        0     5255 2024-05-28 19:11:58.392814 pypanther-0.1.1a8/pypanther/rules/github_rules/github_action_failed.py
+-rw-r--r--   0        0        0    14206 2024-05-28 19:11:58.393090 pypanther-0.1.1a8/pypanther/rules/github_rules/github_advanced_security_change.py
+-rw-r--r--   0        0        0     2042 2024-05-28 19:11:58.393231 pypanther-0.1.1a8/pypanther/rules/github_rules/github_branch_policy_override.py
+-rw-r--r--   0        0        0     2044 2024-05-28 19:11:58.393360 pypanther-0.1.1a8/pypanther/rules/github_rules/github_branch_protection_disabled.py
+-rw-r--r--   0        0        0     2237 2024-05-28 19:11:58.393500 pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_auth_modified.py
+-rw-r--r--   0        0        0     2423 2024-05-28 19:11:58.393637 pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_ip_allowlist.py
+-rw-r--r--   0        0        0     2226 2024-05-28 19:11:58.393773 pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_moderators_add.py
+-rw-r--r--   0        0        0     2316 2024-05-28 19:11:58.393920 pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_modified.py
+-rw-r--r--   0        0        0     3395 2024-05-28 19:11:58.394066 pypanther-0.1.1a8/pypanther/rules/github_rules/github_organization_app_integration_installed.py
+-rw-r--r--   0        0        0     2861 2024-05-28 19:11:58.394265 pypanther-0.1.1a8/pypanther/rules/github_rules/github_public_repository_created.py
+-rw-r--r--   0        0        0     2776 2024-05-28 19:11:58.394683 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_collaborator_change.py
+-rw-r--r--   0        0        0     1460 2024-05-28 19:11:58.394854 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_created.py
+-rw-r--r--   0        0        0     2515 2024-05-28 19:11:58.395035 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_hook_modified.py
+-rw-r--r--   0        0        0     4225 2024-05-28 19:11:58.395329 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_initial_access.py
+-rw-r--r--   0        0        0     1904 2024-05-28 19:11:58.395491 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_visibility_change.py
+-rw-r--r--   0        0        0     5342 2024-05-28 19:11:58.395698 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repository_transfer.py
+-rw-r--r--   0        0        0     3334 2024-05-28 19:11:58.395864 pypanther-0.1.1a8/pypanther/rules/github_rules/github_secret_scanning_alert_created.py
+-rw-r--r--   0        0        0     3340 2024-05-28 19:11:58.396000 pypanther-0.1.1a8/pypanther/rules/github_rules/github_team_modified.py
+-rw-r--r--   0        0        0     1636 2024-05-28 19:11:58.396133 pypanther-0.1.1a8/pypanther/rules/github_rules/github_user_access_key_created.py
+-rw-r--r--   0        0        0     1739 2024-05-28 19:11:58.396258 pypanther-0.1.1a8/pypanther/rules/github_rules/github_user_role_updated.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356132 pypanther-0.1.1a8/pypanther/rules/gitlab_rules/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-28 19:11:58.396411 pypanther-0.1.1a8/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py
+-rw-r--r--   0        0        0     2803 2024-05-28 19:11:58.396546 pypanther-0.1.1a8/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352688 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/__init__.py
+-rw-r--r--   0        0        0     2535 2024-05-28 19:11:58.396680 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py
+-rw-r--r--   0        0        0     2645 2024-05-28 19:11:58.396805 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py
+-rw-r--r--   0        0        0     3202 2024-05-28 19:11:58.396937 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py
+-rw-r--r--   0        0        0     2961 2024-05-28 19:11:58.397073 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py
+-rw-r--r--   0        0        0     1763 2024-05-28 19:11:58.397238 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py
+-rw-r--r--   0        0        0     6379 2024-05-28 19:11:58.397430 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py
+-rw-r--r--   0        0        0     4730 2024-05-28 19:11:58.397617 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py
+-rw-r--r--   0        0        0     1607 2024-05-28 19:11:58.397747 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py
+-rw-r--r--   0        0        0     2204 2024-05-28 19:11:58.397872 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py
+-rw-r--r--   0        0        0     1628 2024-05-28 19:11:58.397997 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py
+-rw-r--r--   0        0        0     2753 2024-05-28 19:11:58.398125 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py
+-rw-r--r--   0        0        0     4443 2024-05-28 19:11:58.398297 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py
+-rw-r--r--   0        0        0     3219 2024-05-28 19:11:58.398429 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354403 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/__init__.py
+-rw-r--r--   0        0        0     4374 2024-05-28 19:11:58.398625 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py
+-rw-r--r--   0        0        0     6493 2024-05-28 19:11:58.398814 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py
+-rw-r--r--   0        0        0     6706 2024-05-28 19:11:58.399004 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py
+-rw-r--r--   0        0        0     5283 2024-05-28 19:11:58.399187 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py
+-rw-r--r--   0        0        0     4645 2024-05-28 19:11:58.399359 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py
+-rw-r--r--   0        0        0     1961 2024-05-28 19:11:58.399479 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py
+-rw-r--r--   0        0        0     5786 2024-05-28 19:11:58.399651 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py
+-rw-r--r--   0        0        0     2339 2024-05-28 19:11:58.399800 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py
+-rw-r--r--   0        0        0     4338 2024-05-28 19:11:58.399992 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py
+-rw-r--r--   0        0        0     1465 2024-05-28 19:11:58.400185 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py
+-rw-r--r--   0        0        0     1998 2024-05-28 19:11:58.400339 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py
+-rw-r--r--   0        0        0     1963 2024-05-28 19:11:58.400491 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py
+-rw-r--r--   0        0        0     3049 2024-05-28 19:11:58.400629 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py
+-rw-r--r--   0        0        0     3473 2024-05-28 19:11:58.400857 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py
+-rw-r--r--   0        0        0     2742 2024-05-28 19:11:58.401165 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py
+-rw-r--r--   0        0        0     3387 2024-05-28 19:11:58.401491 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py
+-rw-r--r--   0        0        0     2020 2024-05-28 19:11:58.401680 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py
+-rw-r--r--   0        0        0     3457 2024-05-28 19:11:58.401841 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py
+-rw-r--r--   0        0        0     2587 2024-05-28 19:11:58.402024 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py
+-rw-r--r--   0        0        0     2203 2024-05-28 19:11:58.402185 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py
+-rw-r--r--   0        0        0     2721 2024-05-28 19:11:58.402352 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py
+-rw-r--r--   0        0        0     6834 2024-05-28 19:11:58.402566 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py
+-rw-r--r--   0        0        0     5013 2024-05-28 19:11:58.402760 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py
+-rw-r--r--   0        0        0     6052 2024-05-28 19:11:58.402956 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py
+-rw-r--r--   0        0        0     5452 2024-05-28 19:11:58.403242 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py
+-rw-r--r--   0        0        0     5222 2024-05-28 19:11:58.403587 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py
+-rw-r--r--   0        0        0     5172 2024-05-28 19:11:58.404059 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py
+-rw-r--r--   0        0        0     4977 2024-05-28 19:11:58.404328 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py
+-rw-r--r--   0        0        0     5223 2024-05-28 19:11:58.404574 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353938 pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/__init__.py
+-rw-r--r--   0        0        0    10551 2024-05-28 19:11:58.404828 pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py
+-rw-r--r--   0        0        0     4560 2024-05-28 19:11:58.405036 pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py
+-rw-r--r--   0        0        0    25458 2024-05-28 19:11:58.405273 pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354103 pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/__init__.py
+-rw-r--r--   0        0        0     4663 2024-05-28 19:11:58.405686 pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py
+-rw-r--r--   0        0        0     4410 2024-05-28 19:11:58.405924 pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/new_user_account_logging.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353568 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/__init__.py
+-rw-r--r--   0        0        0     4583 2024-05-28 19:11:58.406125 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py
+-rw-r--r--   0        0        0     9682 2024-05-28 19:11:58.406310 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py
+-rw-r--r--   0        0        0     6315 2024-05-28 19:11:58.406504 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py
+-rw-r--r--   0        0        0    10184 2024-05-28 19:11:58.406678 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py
+-rw-r--r--   0        0        0     5172 2024-05-28 19:11:58.406886 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352474 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/__init__.py
+-rw-r--r--   0        0        0     3363 2024-05-28 19:11:58.407204 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py
+-rw-r--r--   0        0        0     2868 2024-05-28 19:11:58.407445 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py
+-rw-r--r--   0        0        0     2711 2024-05-28 19:11:58.407846 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py
+-rw-r--r--   0        0        0     4174 2024-05-28 19:11:58.408092 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py
+-rw-r--r--   0        0        0     4371 2024-05-28 19:11:58.408451 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py
+-rw-r--r--   0        0        0     3958 2024-05-28 19:11:58.408751 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py
+-rw-r--r--   0        0        0     2284 2024-05-28 19:11:58.408958 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py
+-rw-r--r--   0        0        0     3355 2024-05-28 19:11:58.409180 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py
+-rw-r--r--   0        0        0     3215 2024-05-28 19:11:58.409325 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py
+-rw-r--r--   0        0        0     4770 2024-05-28 19:11:58.409546 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py
+-rw-r--r--   0        0        0     3435 2024-05-28 19:11:58.409835 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352276 pypanther-0.1.1a8/pypanther/rules/netskope_rules/__init__.py
+-rw-r--r--   0        0        0     2988 2024-05-28 19:11:58.410032 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_admin_logged_out.py
+-rw-r--r--   0        0        0     3570 2024-05-28 19:11:58.410170 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_admin_user_change.py
+-rw-r--r--   0        0        0     2727 2024-05-28 19:11:58.410319 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_many_deletes.py
+-rw-r--r--   0        0        0     2916 2024-05-28 19:11:58.410475 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_personnel_action.py
+-rw-r--r--   0        0        0     3173 2024-05-28 19:11:58.410622 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353782 pypanther-0.1.1a8/pypanther/rules/notion_rules/__init__.py
+-rw-r--r--   0        0        0    16722 2024-05-28 19:11:58.410853 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_account_changed_after_login.py
+-rw-r--r--   0        0        0     1543 2024-05-28 19:11:58.411187 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py
+-rw-r--r--   0        0        0    15424 2024-05-28 19:11:58.411442 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_login_from_new_location.py
+-rw-r--r--   0        0        0     3287 2024-05-28 19:11:58.411704 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_many_pages_deleted.py
+-rw-r--r--   0        0        0     3283 2024-05-28 19:11:58.412121 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_many_pages_exported.py
+-rw-r--r--   0        0        0     1761 2024-05-28 19:11:58.412326 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_accessible_to_api.py
+-rw-r--r--   0        0        0     5409 2024-05-28 19:11:58.412576 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py
+-rw-r--r--   0        0        0     1655 2024-05-28 19:11:58.412968 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_shared_to_web.py
+-rw-r--r--   0        0        0     2883 2024-05-28 19:11:58.413158 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_scim_token_generated.py
+-rw-r--r--   0        0        0     3886 2024-05-28 19:11:58.413330 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_sharing_settings_updated.py
+-rw-r--r--   0        0        0     4484 2024-05-28 19:11:58.413592 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_teamspace_owner_added.py
+-rw-r--r--   0        0        0     3009 2024-05-28 19:11:58.413814 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py
+-rw-r--r--   0        0        0     3278 2024-05-28 19:11:58.413989 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_exported.py
+-rw-r--r--   0        0        0     4562 2024-05-28 19:11:58.414314 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py
+-rw-r--r--   0        0        0     4416 2024-05-28 19:11:58.414728 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356572 pypanther-0.1.1a8/pypanther/rules/okta_rules/__init__.py
+-rw-r--r--   0        0        0     3638 2024-05-28 19:11:58.414960 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_account_support_access.py
+-rw-r--r--   0        0        0     3489 2024-05-28 19:11:58.415273 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py
+-rw-r--r--   0        0        0     7257 2024-05-28 19:11:58.416148 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_admin_role_assigned.py
+-rw-r--r--   0        0        0     7639 2024-05-28 19:11:58.416517 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py
+-rw-r--r--   0        0        0     2652 2024-05-28 19:11:58.416755 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_api_key_created.py
+-rw-r--r--   0        0        0     2497 2024-05-28 19:11:58.416957 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_api_key_revoked.py
+-rw-r--r--   0        0        0     9056 2024-05-28 19:11:58.417202 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py
+-rw-r--r--   0        0        0     7529 2024-05-28 19:11:58.417433 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py
+-rw-r--r--   0        0        0     7410 2024-05-28 19:11:58.417649 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py
+-rw-r--r--   0        0        0     8146 2024-05-28 19:11:58.417952 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_idp_create_modify.py
+-rw-r--r--   0        0        0     8236 2024-05-28 19:11:58.418501 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_idp_signin.py
+-rw-r--r--   0        0        0    13827 2024-05-28 19:11:58.418766 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py
+-rw-r--r--   0        0        0    13471 2024-05-28 19:11:58.419167 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_org2org_creation_modification.py
+-rw-r--r--   0        0        0    10950 2024-05-28 19:11:58.419468 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_password_accessed.py
+-rw-r--r--   0        0        0     7723 2024-05-28 19:11:58.419752 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py
+-rw-r--r--   0        0        0     7666 2024-05-28 19:11:58.420097 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py
+-rw-r--r--   0        0        0    19411 2024-05-28 19:11:58.420288 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_potentially_stolen_session.py
+-rw-r--r--   0        0        0    10701 2024-05-28 19:11:58.420516 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_rate_limits.py
+-rw-r--r--   0        0        0     5009 2024-05-28 19:11:58.420734 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_support_reset.py
+-rw-r--r--   0        0        0     9212 2024-05-28 19:11:58.421054 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py
+-rw-r--r--   0        0        0     6860 2024-05-28 19:11:58.421255 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_account_locked.py
+-rw-r--r--   0        0        0     7020 2024-05-28 19:11:58.421463 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py
+-rw-r--r--   0        0        0     4184 2024-05-28 19:11:58.422724 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_reset.py
+-rw-r--r--   0        0        0     5466 2024-05-28 19:11:58.422989 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py
+-rw-r--r--   0        0        0     8402 2024-05-28 19:11:58.423208 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352956 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/__init__.py
+-rw-r--r--   0        0        0     3854 2024-05-28 19:11:58.423401 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py
+-rw-r--r--   0        0        0     1969 2024-05-28 19:11:58.423550 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py
+-rw-r--r--   0        0        0     2487 2024-05-28 19:11:58.423749 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py
+-rw-r--r--   0        0        0     2294 2024-05-28 19:11:58.424100 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_password_accessed.py
+-rw-r--r--   0        0        0     2201 2024-05-28 19:11:58.424332 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_password_changed.py
+-rw-r--r--   0        0        0     2670 2024-05-28 19:11:58.424491 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py
+-rw-r--r--   0        0        0     1893 2024-05-28 19:11:58.424643 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py
+-rw-r--r--   0        0        0     1935 2024-05-28 19:11:58.424964 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py
+-rw-r--r--   0        0        0     1862 2024-05-28 19:11:58.425132 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py
+-rw-r--r--   0        0        0     2559 2024-05-28 19:11:58.425286 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py
+-rw-r--r--   0        0        0     2009 2024-05-28 19:11:58.425435 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_user_assumed.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353133 pypanther-0.1.1a8/pypanther/rules/onepassword_rules/__init__.py
+-rw-r--r--   0        0        0     4579 2024-05-28 19:11:58.425658 pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py
+-rw-r--r--   0        0        0     3931 2024-05-28 19:11:58.425810 pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py
+-rw-r--r--   0        0        0     4441 2024-05-28 19:11:58.426008 pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_unusual_client.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356027 pypanther-0.1.1a8/pypanther/rules/osquery_rules/__init__.py
+-rw-r--r--   0        0        0     4052 2024-05-28 19:11:58.426279 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py
+-rw-r--r--   0        0        0     3412 2024-05-28 19:11:58.426542 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py
+-rw-r--r--   0        0        0     3594 2024-05-28 19:11:58.426693 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py
+-rw-r--r--   0        0        0     2979 2024-05-28 19:11:58.426836 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py
+-rw-r--r--   0        0        0     2610 2024-05-28 19:11:58.426984 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py
+-rw-r--r--   0        0        0     2217 2024-05-28 19:11:58.427130 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py
+-rw-r--r--   0        0        0     4071 2024-05-28 19:11:58.427265 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py
+-rw-r--r--   0        0        0     3684 2024-05-28 19:11:58.427400 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py
+-rw-r--r--   0        0        0     3486 2024-05-28 19:11:58.427530 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_ossec.py
+-rw-r--r--   0        0        0     3559 2024-05-28 19:11:58.427665 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_outdated.py
+-rw-r--r--   0        0        0     3688 2024-05-28 19:11:58.427798 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_outdated_macos.py
+-rw-r--r--   0        0        0     3744 2024-05-28 19:11:58.428233 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_ssh_listener.py
+-rw-r--r--   0        0        0     5597 2024-05-28 19:11:58.428534 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_suspicious_cron.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353388 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/__init__.py
+-rw-r--r--   0        0        0     4586 2024-05-28 19:11:58.428863 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_detection_deleted.py
+-rw-r--r--   0        0        0     2534 2024-05-28 19:11:58.429364 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_saml_modified.py
+-rw-r--r--   0        0        0     8369 2024-05-28 19:11:58.429670 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py
+-rw-r--r--   0        0        0     9726 2024-05-28 19:11:58.429882 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_user_modified.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354643 pypanther-0.1.1a8/pypanther/rules/salesforce_rules/__init__.py
+-rw-r--r--   0        0        0     4586 2024-05-28 19:11:58.430146 pypanther-0.1.1a8/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353299 pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/__init__.py
+-rw-r--r--   0        0        0     7224 2024-05-28 19:11:58.430367 pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py
+-rw-r--r--   0        0        0     6482 2024-05-28 19:11:58.430577 pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/sentinelone_threats.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355907 pypanther-0.1.1a8/pypanther/rules/slack_rules/__init__.py
+-rw-r--r--   0        0        0    10111 2024-05-28 19:11:58.430815 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_access_expanded.py
+-rw-r--r--   0        0        0     8853 2024-05-28 19:11:58.431014 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_added.py
+-rw-r--r--   0        0        0     6590 2024-05-28 19:11:58.431418 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_removed.py
+-rw-r--r--   0        0        0     4682 2024-05-28 19:11:58.431767 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_application_dos.py
+-rw-r--r--   0        0        0     4947 2024-05-28 19:11:58.432063 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_dlp_modified.py
+-rw-r--r--   0        0        0     3486 2024-05-28 19:11:58.432310 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_config_changed.py
+-rw-r--r--   0        0        0     3429 2024-05-28 19:11:58.432516 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py
+-rw-r--r--   0        0        0     3334 2024-05-28 19:11:58.432687 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_unenrolled.py
+-rw-r--r--   0        0        0     5895 2024-05-28 19:11:58.432918 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_idp_configuration_change.py
+-rw-r--r--   0        0        0     4701 2024-05-28 19:11:58.433301 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_information_barrier_modified.py
+-rw-r--r--   0        0        0     3331 2024-05-28 19:11:58.433529 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py
+-rw-r--r--   0        0        0     6999 2024-05-28 19:11:58.433717 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py
+-rw-r--r--   0        0        0     3454 2024-05-28 19:11:58.433852 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_mfa_settings_changed.py
+-rw-r--r--   0        0        0     2843 2024-05-28 19:11:58.434062 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_org_created.py
+-rw-r--r--   0        0        0     2843 2024-05-28 19:11:58.434228 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_org_deleted.py
+-rw-r--r--   0        0        0     3315 2024-05-28 19:11:58.434385 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_passthrough_anomaly.py
+-rw-r--r--   0        0        0     3412 2024-05-28 19:11:58.434559 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py
+-rw-r--r--   0        0        0     3592 2024-05-28 19:11:58.434722 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_private_channel_made_public.py
+-rw-r--r--   0        0        0     4151 2024-05-28 19:11:58.434937 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py
+-rw-r--r--   0        0        0     3557 2024-05-28 19:11:58.435086 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_service_owner_transferred.py
+-rw-r--r--   0        0        0     3399 2024-05-28 19:11:58.435367 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_sso_settings_changed.py
+-rw-r--r--   0        0        0     7399 2024-05-28 19:11:58.435556 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_user_privilege_escalation.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356824 pypanther-0.1.1a8/pypanther/rules/snyk_rules/__init__.py
+-rw-r--r--   0        0        0     2626 2024-05-28 19:11:58.435716 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_misc_settings.py
+-rw-r--r--   0        0        0     4571 2024-05-28 19:11:58.435902 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_org_settings.py
+-rw-r--r--   0        0        0     4568 2024-05-28 19:11:58.436140 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_ou_change.py
+-rw-r--r--   0        0        0     4884 2024-05-28 19:11:58.436378 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_project_settings.py
+-rw-r--r--   0        0        0     5437 2024-05-28 19:11:58.436604 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_role_change.py
+-rw-r--r--   0        0        0    12027 2024-05-28 19:11:58.436827 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_svcacct_change.py
+-rw-r--r--   0        0        0     3971 2024-05-28 19:11:58.436998 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_externalaccess.py
+-rw-r--r--   0        0        0     6266 2024-05-28 19:11:58.437211 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_policysetting.py
+-rw-r--r--   0        0        0     2578 2024-05-28 19:11:58.437380 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_sso.py
+-rw-r--r--   0        0        0     5851 2024-05-28 19:11:58.437713 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_user_mgmt.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352089 pypanther-0.1.1a8/pypanther/rules/standard_rules/__init__.py
+-rw-r--r--   0        0        0    10991 2024-05-28 19:11:58.437955 pypanther-0.1.1a8/pypanther/rules/standard_rules/admin_assigned.py
+-rw-r--r--   0        0        0    16955 2024-05-28 19:11:58.438292 pypanther-0.1.1a8/pypanther/rules/standard_rules/brute_force_by_ip.py
+-rw-r--r--   0        0        0    36758 2024-05-28 19:11:58.438611 pypanther-0.1.1a8/pypanther/rules/standard_rules/impossible_travel_login.py
+-rw-r--r--   0        0        0     9779 2024-05-28 19:11:58.439137 pypanther-0.1.1a8/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py
+-rw-r--r--   0        0        0     8225 2024-05-28 19:11:58.439339 pypanther-0.1.1a8/pypanther/rules/standard_rules/mfa_disabled.py
+-rw-r--r--   0        0        0     9943 2024-05-28 19:11:58.439546 pypanther-0.1.1a8/pypanther/rules/standard_rules/standard_dns_base64.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353861 pypanther-0.1.1a8/pypanther/rules/tailscale_rules/__init__.py
+-rw-r--r--   0        0        0     4649 2024-05-28 19:11:58.439749 pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_https_disabled.py
+-rw-r--r--   0        0        0     4885 2024-05-28 19:11:58.439960 pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py
+-rw-r--r--   0        0        0     4666 2024-05-28 19:11:58.440234 pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356684 pypanther-0.1.1a8/pypanther/rules/tines_rules/__init__.py
+-rw-r--r--   0        0        0     2584 2024-05-28 19:11:58.440442 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_actions_disabled_changes.py
+-rw-r--r--   0        0        0     2824 2024-05-28 19:11:58.440763 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_custom_ca.py
+-rw-r--r--   0        0        0     3540 2024-05-28 19:11:58.440948 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py
+-rw-r--r--   0        0        0     2887 2024-05-28 19:11:58.441094 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_global_resource_destruction.py
+-rw-r--r--   0        0        0     2947 2024-05-28 19:11:58.441254 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_sso_settings.py
+-rw-r--r--   0        0        0     2765 2024-05-28 19:11:58.441427 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_story_items_destruction.py
+-rw-r--r--   0        0        0     2735 2024-05-28 19:11:58.441579 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_story_jobs_clearance.py
+-rw-r--r--   0        0        0     2680 2024-05-28 19:11:58.441739 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_team_destruction.py
+-rw-r--r--   0        0        0     3987 2024-05-28 19:11:58.441908 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_tenant_authtoken.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352185 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/__init__.py
+-rw-r--r--   0        0        0     3775 2024-05-28 19:11:58.442062 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py
+-rw-r--r--   0        0        0     2972 2024-05-28 19:11:58.442217 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_new_api_token.py
+-rw-r--r--   0        0        0     3208 2024-05-28 19:11:58.442377 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_new_owner.py
+-rw-r--r--   0        0        0     3717 2024-05-28 19:11:58.442531 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py
+-rw-r--r--   0        0        0     2962 2024-05-28 19:11:58.442682 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_assumption.py
+-rw-r--r--   0        0        0     2774 2024-05-28 19:11:58.442830 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_role.py
+-rw-r--r--   0        0        0     3927 2024-05-28 19:11:58.442983 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_suspension.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353216 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-28 19:11:58.443143 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py
+-rw-r--r--   0        0        0     2359 2024-05-28 19:11:58.443509 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py
+-rw-r--r--   0        0        0     2830 2024-05-28 19:11:58.443740 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py
+-rw-r--r--   0        0        0     2760 2024-05-28 19:11:58.443955 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py
+-rw-r--r--   0        0        0     3358 2024-05-28 19:11:58.444132 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py
+-rw-r--r--   0        0        0     3558 2024-05-28 19:11:58.444298 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py
+-rw-r--r--   0        0        0     2620 2024-05-28 19:11:58.444442 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py
+-rw-r--r--   0        0        0     4620 2024-05-28 19:11:58.444656 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py
+-rw-r--r--   0        0        0     4251 2024-05-28 18:40:51.829617 pypanther-0.1.1a8/pypanther/upload.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095097 pypanther-0.1.1a8/pypanther/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095354 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095410 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/__init__.py
+-rw-r--r--   0        0        0    16541 2024-05-24 13:47:47.095519 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/client.py
+-rw-r--r--   0        0        0      624 2024-05-24 13:47:47.095629 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/errors.py
+-rw-r--r--   0        0        0      159 2024-05-24 13:47:47.095796 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload.graphql
+-rw-r--r--   0        0        0      802 2024-05-24 13:47:47.095929 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql
+-rw-r--r--   0        0        0     1439 2024-05-24 17:25:24.652928 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql
+-rw-r--r--   0        0        0    25446 2024-05-24 13:47:47.096146 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py
+-rw-r--r--   0        0        0     1606 2024-05-24 13:47:47.096405 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/cli_output.py
+-rw-r--r--   0        0        0      493 2024-05-28 18:40:51.830002 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/command/standard_args.py
+-rw-r--r--   0        0        0     1308 2024-05-28 18:40:51.830341 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/config.py
+-rw-r--r--   0        0        0      714 2024-05-28 18:40:51.830732 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/constants.py
+-rw-r--r--   0        0        0     2008 2024-05-28 18:40:51.831059 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/util.py
+-rw-r--r--   0        0        0      274 2024-05-23 22:00:33.355426 pypanther-0.1.1a8/pypanther/wrap.py
+-rw-r--r--   0        0        0     1746 2024-05-28 19:11:58.444950 pypanther-0.1.1a8/pyproject.toml
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 pypanther-0.1.1a8/PKG-INFO
```

### Comparing `pypanther-0.1.1a3/LICENSE.txt` & `pypanther-0.1.1a8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/base.py` & `pypanther-0.1.1a8/pypanther/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,35 +134,35 @@
     if isinstance(item, Enum):
         return item.value
     return item
 
 
 # pylint: disable=invalid-name
 @total_ordering
-class Severity(str, Enum):
+class PantherSeverity(str, Enum):
     Info = "Info"
     Low = "Low"
     Medium = "Medium"
     High = "High"
     Critical = "Critical"
 
     def __lt__(self, other):
-        return Severity.as_int(self.value) < Severity.as_int(other.value)
+        return PantherSeverity.as_int(self.value) < PantherSeverity.as_int(other.value)
 
     @staticmethod
-    def as_int(value: "Severity") -> int:
-        if value.upper() == Severity.Info.upper():
+    def as_int(value: "PantherSeverity") -> int:
+        if value.upper() == PantherSeverity.Info.upper():
             return 0
-        if value.upper() == Severity.Low.upper():
+        if value.upper() == PantherSeverity.Low.upper():
             return 1
-        if value.upper() == Severity.Medium.upper():
+        if value.upper() == PantherSeverity.Medium.upper():
             return 2
-        if value.upper() == Severity.High.upper():
+        if value.upper() == PantherSeverity.High.upper():
             return 3
-        if value.upper() == Severity.Critical.upper():
+        if value.upper() == PantherSeverity.Critical.upper():
             return 4
         raise ValueError(f"Unknown severity: {value}")
 
     def __str__(self) -> str:
         """Returns a string representation of the class' value."""
         return self.value
 
@@ -218,15 +218,15 @@
     LogTypes: List[str]
     OutputIds: List[str]
     Reference: str
     Reports: Dict[str, List[str]]
     Runbook: str
     RuleID: str
     ScheduledQueries: List[str]
-    Severity: Severity
+    Severity: PantherSeverity
     SummaryAttributes: List[str]
     Tags: List[str]
     Tests: List[PantherRuleTest]
     Threshold: PositiveInt
 
 
 PantherRuleAdapter = TypeAdapter(PantherRuleModel)
@@ -250,24 +250,24 @@
     if len(s) > max_size:
         # If generated field exceeds max size, truncate it
         num_characters_to_keep = max_size - len(TRUNCATED_STRING_SUFFIX)
         return s[:num_characters_to_keep] + TRUNCATED_STRING_SUFFIX
     return s
 
 
-SeverityType = Union[Severity | Literal["DEFAULT"]]
+SeverityType = Union[PantherSeverity | Literal["DEFAULT"]]
 
 
 # pylint: disable=unused-argument
 class PantherRule:
     """A Panther rule class. This class should be subclassed to create a new rule."""
 
     LogTypes: List[str]
     RuleID: str
-    Severity: Severity
+    Severity: PantherSeverity
     Enabled: bool = True
     Tags: List[str] = DEFAULT_TAGS
     DedupPeriodMinutes: NonNegativeInt = DEFAULT_DEDUP_PERIOD_MINUTES
     Description: str = DEFAULT_DESCRIPTION
     DisplayName: str = DEFAULT_DISPLAY_NAME
     OutputIds: List[str] = DEFAULT_OUTPUT_IDS
     Reference: str = DEFAULT_REFERENCE
```

### Comparing `pypanther-0.1.1a3/pypanther/data_models/asana_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/asana_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/atlassian_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/atlassian_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/aws_alb_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/aws_alb_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/aws_cloudtrail_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/aws_cloudtrail_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/aws_eks_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/aws_eks_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/aws_s3_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/aws_s3_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/aws_vpcdns_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/aws_vpcdns_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/aws_vpcflow_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/aws_vpcflow_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/azure_signin_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/azure_signin_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/box_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/box_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/cisco_umbrella_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/cisco_umbrella_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/cloudflare_firewall_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/cloudflare_firewall_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/cloudflare_httpreq_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/cloudflare_httpreq_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/crowdstrike_fdr_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/crowdstrike_fdr_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/gcp_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/gcp_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/github_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/github_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/gsuite_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/gsuite_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/notion_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/notion_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/okta_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/okta_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/onelogin_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/onelogin_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/onepassword_itemusage_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/onepassword_itemusage_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/onepassword_signinattempt_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/onepassword_signinattempt_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/panther_audit_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/panther_audit_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/slack_accesslogs_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/slack_accesslogs_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/slack_auditlogs_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/slack_auditlogs_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/zendesk_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/zendesk_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/zoom_activity_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/zoom_activity_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/data_models/zoom_operation_data_model.py` & `pypanther-0.1.1a8/pypanther/data_models/zoom_operation_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/get.py` & `pypanther-0.1.1a8/pypanther/get.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/gcp_base_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/gcp_base_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/gcp_environment.py` & `pypanther-0.1.1a8/pypanther/helpers/gcp_environment.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_asana_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_asana_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_audit.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_audit.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_auth0_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_auth0_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_azuresignin_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_azuresignin_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_base_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_base_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_box_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_box_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_cloudflare_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_cloudflare_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_config_defaults.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_config_defaults.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_config_overrides.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_config_overrides.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_default.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_default.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_duo_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_duo_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_event_type_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_event_type_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_greynoise_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_greynoise_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_iocs.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_iocs.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_ipinfo_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_ipinfo_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_lookuptable_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_lookuptable_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_oss_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_oss_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_snyk_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_snyk_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_tines_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_tines_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_tor_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_tor_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/helpers/panther_zoom_helpers.py` & `pypanther-0.1.1a8/pypanther/helpers/panther_zoom_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/log_types.py` & `pypanther-0.1.1a8/pypanther/log_types.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/main.py` & `pypanther-0.1.1a8/pypanther/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import argparse
-from typing import Any, Dict
 
 from pypanther.upload import run as upload
 from pypanther.vendor.panther_analysis_tool import util
 from pypanther.vendor.panther_analysis_tool.command import standard_args
+from pypanther.vendor.panther_analysis_tool.config import dynaconf_argparse_merge, setup_dynaconf
 
 
 def run():
     parser = argparse.ArgumentParser(description="Command line tool for uploading files.")
     subparsers = parser.add_subparsers(dest="command", help="Available commands")
 
     # Upload command
     upload_parser = subparsers.add_parser("upload", help="Upload a file")
-    no_async_uploads_name = "--no-async"
-    no_async_uploads_arg: Dict[str, Any] = {
-        "action": "store_true",
-        "default": False,
-        "required": False,
-        "help": "When set your upload will be synchronous",
-    }
+
     standard_args.for_public_api(upload_parser, required=False)
-    standard_args.using_aws_profile(upload_parser)
     upload_parser.set_defaults(func=util.func_with_backend(upload))
-    upload_parser.add_argument(no_async_uploads_name, **no_async_uploads_arg)
     upload_parser.add_argument(
         "--max-retries",
         help="Retry to upload on a failure for a maximum number of times",
         default=10,
         type=int,
         required=False,
     )
 
     args = parser.parse_args()
     if args.command is None:
         parser.print_help()
         return
+
+    config_file_settings = setup_dynaconf()
+    dynaconf_argparse_merge(vars(args), config_file_settings)
+
     args.func(args)
```

### Comparing `pypanther-0.1.1a3/pypanther/register.py` & `pypanther-0.1.1a8/pypanther/register.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_service_account_created.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_service_account_created.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_service_account_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="New domain created",
         ExpectedResult=False,
@@ -82,15 +82,15 @@
 
 
 class AsanaServiceAccountCreated(PantherRule):
     Description = "An Asana service account was created by someone in your organization."
     DisplayName = "Asana Service Account Created"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://help.asana.com/hc/en-us/articles/14217496838427-Service-Accounts"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Service.Account.Created-prototype"
     Tests = asana_service_account_created_tests
 
     def rule(self, event):
         return event.get("event_type", "<NO_EVENT_TYPE_FOUND>") == "service_account_created"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_team_privacy_public.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_team_privacy_public.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_team_privacy_public_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Team made public",
         ExpectedResult=True,
@@ -61,15 +61,15 @@
 ]
 
 
 class AsanaTeamPrivacyPublic(PantherRule):
     Description = "An Asana team's privacy setting was changed to public to the organization (not public to internet)"
     DisplayName = "Asana Team Privacy Public"
     Reference = "https://help.asana.com/hc/en-us/articles/14211433439387-Team-permissions"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Team.Privacy.Public-prototype"
     Tests = asana_team_privacy_public_tests
 
     def rule(self, event):
         return (
             event.get("event_type") == "team_privacy_settings_changed"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_default_session_duration_never_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Session Duration Never",
         ExpectedResult=True,
@@ -54,15 +54,15 @@
 ]
 
 
 class AsanaWorkspaceDefaultSessionDurationNever(PantherRule):
     Description = "An Asana workspace's default session duration (how often users need to re-authenticate) has been changed to never. "
     DisplayName = "Asana Workspace Default Session Duration Never"
     Reference = "https://help.asana.com/hc/en-us/articles/14218320495899-Manage-Session-Duration"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.Default.Session.Duration.Never-prototype"
     Tests = asana_workspace_default_session_duration_never_tests
 
     def rule(self, event):
         return (
             event.get("event_type") == "workspace_default_session_duration_changed"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_email_domain_added_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="new domain",
         ExpectedResult=True,
@@ -54,15 +54,15 @@
 ]
 
 
 class AsanaWorkspaceEmailDomainAdded(PantherRule):
     Description = "A new email domain has been added to an Asana workspace. Reviewer should validate that the new domain is a part of the organization. "
     DisplayName = "Asana Workspace Email Domain Added"
     Reference = "https://help.asana.com/hc/en-us/articles/15901227439515-Email-domain-management-for-Asana-organizations"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.Email.Domain.Added-prototype"
     Tests = asana_workspace_email_domain_added_tests
 
     def rule(self, event):
         return event.get("event_type") == "workspace_associated_email_domain_added"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_form_link_auth_requirement_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="form auth requirement disabled",
         ExpectedResult=True,
@@ -54,15 +54,15 @@
 ]
 
 
 class AsanaWorkspaceFormLinkAuthRequirementDisabled(PantherRule):
     Description = "An Asana Workspace Form Link is a unique URL that allows you to create a task directly within a specific Workspace or Project in Asana, using a web form. Disabling authentication requirements may allow unauthorized users to create tasks. "
     DisplayName = "Asana Workspace Form Link Auth Requirement Disabled"
     Reference = "https://help.asana.com/hc/en-us/articles/14111697664923-Forms-access-permissions#:~:text=SSO%2C%20SAML%2C%20or-,no%20authentication%20method,-).%20If%20no%20authentication"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.Form.Link.Auth.Requirement.Disabled-prototype"
     Tests = asana_workspace_form_link_auth_requirement_disabled_tests
 
     def rule(self, event):
         return event.get("event_type") == "workspace_form_link_authentication_required_disabled"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_guest_invite_permissions_anyone_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Anyone Allowed Guest Invite",
         ExpectedResult=True,
@@ -54,15 +54,15 @@
 ]
 
 
 class AsanaWorkspaceGuestInvitePermissionsAnyone(PantherRule):
     Description = "Typically inviting guests to Asana is permitted by few users. Enabling anyone to invite guests can potentially lead to unauthorized users gaining access to Asana."
     DisplayName = "Asana Workspace Guest Invite Permissions Anyone"
     Reference = "https://help.asana.com/hc/en-us/articles/14109494654875-Admin-console#:~:text=Google%20SSO%20password.-,Guest%20invite%20controls,-Super%20admins%20of"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.Guest.Invite.Permissions.Anyone-prototype"
     Tests = asana_workspace_guest_invite_permissions_anyone_tests
 
     def rule(self, event):
         return (
             event.get("event_type") == "workspace_guest_invite_permissions_changed"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_new_admin.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_new_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_asana_helpers import asana_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_new_admin_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Team made public",
@@ -66,15 +66,15 @@
 ]
 
 
 class AsanaWorkspaceNewAdmin(PantherRule):
     Description = "Admin role was granted to the user who previously did not have admin permissions"
     DisplayName = "Asana Workspace New Admin"
     Reference = "https://help.asana.com/hc/en-us/articles/14141552580635-Admin-and-super-admin-roles-in-Asana"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.New.Admin-prototype"
     Tests = asana_workspace_new_admin_tests
 
     def rule(self, event):
         new = deep_get(event, "details", "new_value", default="")
         old = deep_get(event, "details", "old_value", default="")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_org_export.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_org_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_org_export_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Web App Approvals On",
         ExpectedResult=False,
@@ -55,15 +55,15 @@
 
 
 class AsanaWorkspaceOrgExport(PantherRule):
     Description = "An Asana user started an org export."
     DisplayName = "Asana Workspace Org Export"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://help.asana.com/hc/en-us/articles/14139896860955-Privacy-and-security#:~:text=like%20to%20see.-,Full%20export%20of%20an%20organization,-Available%20on%20Asana"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.Org.Export-prototype"
     Tests = asana_workspace_org_export_tests
 
     def rule(self, event):
         return event.get("event_type", "<NO_EVENT_TYPE_FOUND>") == "workspace_export_started"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_password_requirements_simple_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Simple",
         ExpectedResult=True,
@@ -59,15 +59,15 @@
 
 
 class AsanaWorkspacePasswordRequirementsSimple(PantherRule):
     Description = "An asana user made your organization's password requirements less strict."
     DisplayName = "Asana Workspace Password Requirements Simple"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://help.asana.com/hc/en-us/articles/14075208738587-Authentication-and-access-management-options-for-paid-plans"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.Password.Requirements.Simple-prototype"
     Tests = asana_workspace_password_requirements_simple_tests
 
     def rule(self, event):
         new_val = deep_get(event, "details", "new_value", default="<NEW_VAL_NOT_FOUND>")
         return all(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_require_app_approvals_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Web Reqs On",
         ExpectedResult=False,
@@ -55,15 +55,15 @@
 
 
 class AsanaWorkspaceRequireAppApprovalsDisabled(PantherRule):
     Description = "An Asana user turned off app approval requirements for an application type for your organization."
     DisplayName = "Asana Workspace Require App Approvals Disabled"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://help.asana.com/hc/en-us/articles/14109494654875-Admin-console#:~:text=used%20by%20default-,Require%20app%20approval,-Admins%20manage%20a"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.Require.App.Approvals.Disabled-prototype"
     Tests = asana_workspace_require_app_approvals_disabled_tests
 
     def rule(self, event):
         new_val = deep_get(event, "details", "new_value", default="<NEW_VAL_NOT_FOUND>")
         return all(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_saml_optional.py` & `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_saml_optional.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 asana_workspace_saml_optional_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="SAML required",
         ExpectedResult=False,
@@ -55,15 +55,15 @@
 
 
 class AsanaWorkspaceSAMLOptional(PantherRule):
     Description = "An Asana user made SAML optional for your organization."
     DisplayName = "Asana Workspace SAML Optional"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://help.asana.com/hc/en-us/articles/14075208738587-Premium-Business-and-Enterprise-authentication#gl-saml:~:text=to%20your%20organization.-,SAML,-If%20your%20company"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Asana_Audit]
     RuleID = "Asana.Workspace.SAML.Optional-prototype"
     Tests = asana_workspace_saml_optional_tests
 
     def rule(self, event):
         old_val = deep_get(event, "details", "old_value", default="<OLD_VAL_NOT_FOUND>")
         new_val = deep_get(event, "details", "new_value", default="<NEW_VAL_NOT_FOUND>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/atlassian_rules/user_logged_in_as_user.py` & `pypanther-0.1.1a8/pypanther/rules/atlassian_rules/user_logged_in_as_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 atlassian_user_logged_in_as_user_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Admin impersonated user successfully",
         ExpectedResult=True,
@@ -83,15 +83,15 @@
     ),
 ]
 
 
 class AtlassianUserLoggedInAsUser(PantherRule):
     DisplayName = "Atlassian admin impersonated another user"
     RuleID = "Atlassian.User.LoggedInAsUser-prototype"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Atlassian_Audit]
     Tags = ["Atlassian", "User impersonation"]
     Description = "Reports when an Atlassian user logs in (impersonates) another user.\n"
     Runbook = "Validate that the Atlassian admin did log in (impersonate) as another user.\n"
     Reference = "https://support.atlassian.com/user-management/docs/log-in-as-another-user/"
     Tests = atlassian_user_logged_in_as_user_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_custom_role_created.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_custom_role_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_custom_role_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
@@ -763,15 +763,15 @@
 class Auth0CustomRoleCreated(PantherRule):
     Description = "An Auth0 User created a role in your organization's tenant."
     DisplayName = "Auth0 Custom Role Created"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant if a user created a role without proper authorization."
     Reference = (
         "https://auth0.com/docs/manage-users/access-control/configure-core-rbac/roles/create-roles"
     )
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.Custom.Role.Created-prototype"
     Tests = auth0_custom_role_created_tests
 
     def rule(self, event):
         data_description = deep_get(
             event, "data", "description", default="<NO_DATA_DESCRIPTION_FOUND>"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_integration_installed.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_integration_installed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_integration_installed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Auth0 Integration Installed",
@@ -254,15 +254,15 @@
 
 
 class Auth0IntegrationInstalled(PantherRule):
     Description = "An Auth0 integration was installed from the auth0 action library."
     DisplayName = "Auth0 Integration Installed"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant to re-enable this setting as it's in the best security interest for your organization's security posture."
     Reference = "https://auth0.com/blog/actions-integrations-are-now-ga/"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.Integration.Installed-prototype"
     Tests = auth0_integration_installed_tests
 
     def rule(self, event):
         data_description = deep_get(
             event, "data", "description", default="<NO_DATA_DESCRIPTION_FOUND>"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_mfa_factor_setting_enabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="MFA Enabled",
@@ -382,15 +382,15 @@
 
 
 class Auth0MFAFactorSettingEnabled(PantherRule):
     Description = "An Auth0 user enabled an mfa factor in your organization's mfa settings."
     DisplayName = "Auth0 mfa factor enabled"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant to re-enable this setting as it's in the best security interest for your organization's security posture."
     Reference = "https://auth0.com/docs/secure/multi-factor-authentication/multi-factor-authentication-factors"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.MFA.Factor.Setting.Enabled-prototype"
     Tests = auth0_mfa_factor_setting_enabled_tests
 
     def rule(self, event):
         description = deep_get(event, "data", "description", default="<NO_DESCRIPTION_FOUND>")
         enabled = deep_get(event, "data", "details", "response", "body", "enabled")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_mfa_policy_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
@@ -389,15 +389,15 @@
 
 
 class Auth0MFAPolicyDisabled(PantherRule):
     Description = "An Auth0 User disabled MFA for your organization's tenant."
     DisplayName = "Auth0 MFA Policy Disabled"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant to re-enable this setting as it's in the best security interest for your organization's security posture."
     Reference = "https://auth0.com/docs/secure/multi-factor-authentication/enable-mfa#:~:text=prompted%20for%20MFA.-,Never,-%3A%20MFA%20is%20not"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.MFA.Policy.Disabled-prototype"
     Tests = auth0_mfa_policy_disabled_tests
 
     def rule(self, event):
         data_description = deep_get(
             event, "data", "description", default="<NO_DATA_DESCRIPTION_FOUND>"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_mfa_policy_enabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="MFA Policy Enabled First",
@@ -575,15 +575,15 @@
 
 
 class Auth0MFAPolicyEnabled(PantherRule):
     Description = "An Auth0 User enabled MFA Policy for your organization's tenant."
     DisplayName = "Auth0 MFA Policy Enabled"
     Runbook = "Assess if this was done by the user for a valid business reason and was expected. This alert indicates a setting change that aligns with best security practices, follow-up may be unnecessary."
     Reference = "https://auth0.com/docs/secure/multi-factor-authentication/enable-mfa#:~:text=In%20the-,Define%20policies,-section%2C%20select%20a"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.MFA.Policy.Enabled-prototype"
     Tests = auth0_mfa_policy_enabled_tests
 
     def rule(self, event):
         data_description = deep_get(
             event, "data", "description", default="<NO_DATA_DESCRIPTION_FOUND>"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_mfa_risk_assessment_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
@@ -391,15 +391,15 @@
 class Auth0MFARiskAssessmentDisabled(PantherRule):
     Description = (
         "An Auth0 User disabled the mfa risk assessment setting for your organization's tenant."
     )
     DisplayName = "Auth0 MFA Risk Assessment Disabled"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant to re-enable this setting as it's in the best security interest for your organization's security posture."
     Reference = "https://auth0.com/docs/secure/multi-factor-authentication/enable-mfa#:~:text=Always%20policy%2C%20the-,MFA%20Risk%20Assessors,-section%20appears.%20By"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.MFA.Risk.Assessment.Disabled-prototype"
     Tests = auth0_mfa_risk_assessment_disabled_tests
 
     def rule(self, event):
         data_description = deep_get(
             event, "data", "description", default="<NO_DATA_DESCRIPTION_FOUND>"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_mfa_risk_assessment_enabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
@@ -373,15 +373,15 @@
 class Auth0MFARiskAssessmentEnabled(PantherRule):
     Description = (
         "An Auth0 User enabled the mfa risk assessment setting for your organization's tenant."
     )
     DisplayName = "Auth0 MFA Risk Assessment Enabled"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant when enabling this setting as it's in the best security interest for your organization's security posture."
     Reference = "https://auth0.com/docs/secure/multi-factor-authentication/enable-mfa#:~:text=Always%20policy%2C%20the-,MFA%20Risk%20Assessors,-section%20appears.%20By"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.MFA.Risk.Assessment.Enabled-prototype"
     Tests = auth0_mfa_risk_assessment_enabled_tests
 
     def rule(self, event):
         data_description = deep_get(
             event, "data", "description", default="<NO_DATA_DESCRIPTION_FOUND>"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_post_login_action_flow_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
@@ -303,15 +303,15 @@
 
 
 class Auth0PostLoginActionFlow(PantherRule):
     Description = "An Auth0 User updated a post login action flow for your organization's tenant."
     DisplayName = "Auth0 Post Login Action Flow Updated"
     Runbook = "Assess if this was done by the user for a valid business reason. Be sure to replace any steps that were removed without authorization."
     Reference = "https://auth0.com/docs/customize/actions/flows-and-triggers/login-flow/api-object"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.Post.Login.Action.Flow-prototype"
     Tests = auth0_post_login_action_flow_tests
 
     def rule(self, event):
         data_description = deep_get(
             event, "data", "description", default="<NO_DATA_DESCRIPTION_FOUND>"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_user_invitation_created.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_user_invitation_created.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_user_invitation_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Test-org",
@@ -315,15 +315,15 @@
 
 
 class Auth0UserInvitationCreated(PantherRule):
     DisplayName = "Auth0 User Invitation Created"
     Reference = (
         "https://auth0.com/docs/manage-users/organizations/configure-organizations/invite-members"
     )
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.Auth0_Events]
     RuleID = "Auth0.User.Invitation.Created-prototype"
     Tests = auth0_user_invitation_created_tests
     org_re = re.compile("^/api/v2/organizations/[^/\\s]+/invitations$")
 
     def rule(self, event):
         if not any([True, is_auth0_config_event(event)]):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py` & `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_auth0_helpers import auth0_alert_context, is_auth0_config_event
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 auth0_user_joined_tenant_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User accepted an invitation",
@@ -315,15 +315,15 @@
 
 
 class Auth0UserJoinedTenant(PantherRule):
     DisplayName = "Auth0 User Joined Tenant"
     Description = "User accepted invitation from Auth0 member to join an Auth0 tenant."
     RuleID = "Auth0.User.Joined.Tenant-prototype"
     Reference = "https://auth0.com/docs/manage-users/organizations/configure-organizations/invite-members#send-membership-invitations:~:text=.-,Send%20membership%20invitations,-You%20can"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.Auth0_Events]
     Tests = auth0_user_joined_tenant_tests
 
     def rule(self, event):
         data_description = deep_get(
             event, "data", "description", default="<NO_DATA_DESCRIPTION_FOUND>"
         )
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_ami_modified_for_public_access_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="AMI Made Public",
@@ -231,15 +231,15 @@
 
 
 class AWSCloudTrailAMIModifiedForPublicAccess(PantherRule):
     RuleID = "AWS.CloudTrail.AMIModifiedForPublicAccess-prototype"
     DisplayName = "Amazon Machine Image (AMI) Modified to Allow Public Access"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Exfiltration:Transfer Data to Cloud Account"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0010:T1537"]}
     Description = "An Amazon Machine Image (AMI) was modified to allow it to be launched by anyone. Any sensitive configuration or application data stored in the AMI's block devices is at risk.\n"
     Runbook = "Determine if the AMI is intended to be publicly accessible. If not, first modify the AMI to not be publicly accessible then change any sensitive data stored in the block devices associated to the AMI (as they may be compromised).\n"
     Reference = "https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/sharingamis-intro.html"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_cloud_trail_ami_modified_for_public_access_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 aws_cloud_trail_account_discovery_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="DescribeAccount",
         ExpectedResult=True,
@@ -154,15 +154,15 @@
 
 
 class AWSCloudTrailAccountDiscovery(PantherRule):
     Description = "Adversaries may attempt to get a listing of accounts on a system or within an environment. This information can help adversaries determine which accounts exist to aid in follow-on behavior."
     DisplayName = "AWS CloudTrail Account Discovery"
     Reference = "https://attack.mitre.org/techniques/T1087/"
     Reports = {"MITRE ATT&CK": ["TA0007:T1087"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.CloudTrail.Account.Discovery-prototype"
     Tests = aws_cloud_trail_account_discovery_tests
     DISCOVERY_EVENTS = [
         "GetAlternateContact",
         "GetContactInformation",
         "PutAlternateContact",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CloudTrail Was Created",
@@ -149,15 +149,15 @@
 
 class AWSCloudTrailCreated(PantherRule):
     RuleID = "AWS.CloudTrail.Created-prototype"
     DisplayName = "A CloudTrail Was Created or Updated"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Discovery:Cloud Service Dashboard"]
     Reports = {"CIS": ["3.5"], "MITRE ATT&CK": ["TA0007:T1538"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A CloudTrail Trail was created, updated, or enabled.\n"
     Runbook = "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-cloudtrail-modified"
     Reference = "https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-create-and-update-a-trail.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_cloud_trail_password_policy_discovery_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Non-Discovery Event",
         ExpectedResult=False,
@@ -57,15 +57,15 @@
 
 
 class AWSCloudTrailPasswordPolicyDiscovery(PantherRule):
     Description = "This detection looks for *AccountPasswordPolicy events in AWS CloudTrail logs. If these events occur in a short period of time from the same ARN, it could constitute Password Policy reconnaissance."
     DisplayName = "AWS CloudTrail Password Policy Discovery"
     Reports = {"MITRE ATT&CK": ["TA0007:T1201"]}
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_account-policy.html"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     DedupPeriodMinutes = 30
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.CloudTrail.Password.Policy.Discovery-prototype"
     Threshold = 2
     Tests = aws_cloud_trail_password_policy_discovery_tests
     PASSWORD_DISCOVERY_EVENTS = [
         "GetAccountPasswordPolicy",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success, lookup_aws_account_name
 from pypanther.log_types import LogType
 
 aws_cloud_trail_stopped_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CloudTrail Was Stopped",
@@ -149,15 +149,15 @@
 
 class AWSCloudTrailStopped(PantherRule):
     RuleID = "AWS.CloudTrail.Stopped-prototype"
     DisplayName = "CloudTrail Stopped"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "DemoThreatHunting", "Defense Evasion:Impair Defenses"]
     Reports = {"CIS": ["3.5"], "MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A CloudTrail Trail was modified.\n"
     Runbook = "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-cloudtrail-modified"
     Reference = "https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-delete-trails-console.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_unsuccessful_mf_aattempt_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Successful Login w/ MFA",
         ExpectedResult=False,
@@ -73,15 +73,15 @@
 class AWSUnsuccessfulMFAattempt(PantherRule):
     Description = "Monitor application logs for suspicious events including repeated MFA failures that may indicate user's primary credentials have been compromised."
     DisplayName = "AWS Unsuccessful MFA attempt"
     Enabled = False
     Reference = "https://attack.mitre.org/techniques/T1621/"
     Tags = ["Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1621"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     DedupPeriodMinutes = 15
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.Unsuccessful.MFA.attempt-prototype"
     Threshold = 2
     Tests = aws_unsuccessful_mf_aattempt_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import lookup_aws_account_name
 from pypanther.log_types import LogType
 
 aws_cloud_trail_codebuild_project_made_public_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CodeBuild Project Made Public",
@@ -129,15 +129,15 @@
 
 class AWSCloudTrailCodebuildProjectMadePublic(PantherRule):
     RuleID = "AWS.CloudTrail.CodebuildProjectMadePublic-prototype"
     DisplayName = "CodeBuild Project made Public"
     LogTypes = [LogType.AWS_CloudTrail]
     Reports = {"MITRE ATT&CK": ["TA0010:T1567"]}
     Tags = ["AWS", "Security Control", "Exfiltration:Exfiltration Over Web Service"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "An AWS CodeBuild Project was made publicly accessible\n"
     Runbook = "TBD"
     Reference = "https://docs.aws.amazon.com/codebuild/latest/userguide/public-builds.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_config_service_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Config Recorder Delivery Channel Created",
@@ -132,15 +132,15 @@
 
 class AWSConfigServiceCreated(PantherRule):
     RuleID = "AWS.ConfigService.Created-prototype"
     DisplayName = "AWS Config Service Created"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Discovery:Cloud Service Discovery"]
     Reports = {"CIS": ["3.9"], "MITRE ATT&CK": ["TA0007:T1526"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "An AWS Config Recorder or Delivery Channel was created\n"
     Runbook = "Verify that the Config Service changes were authorized. If not, revert them and investigate who caused the change. Consider altering permissions to prevent this from happening again in the future.\n"
     Reference = "https://aws.amazon.com/config/"
     SummaryAttributes = [
         "eventName",
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_config_service_disabled_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Config Recorder Delivery Channel Created",
@@ -132,15 +132,15 @@
 
 class AWSConfigServiceDisabledDeleted(PantherRule):
     RuleID = "AWS.ConfigService.DisabledDeleted-prototype"
     DisplayName = "AWS Config Service Disabled"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Defense Evasion:Impair Defenses"]
     Reports = {"CIS": ["3.9"], "MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An AWS Config Recorder or Delivery Channel was disabled or deleted\n"
     Runbook = "Verify that the Config Service changes were authorized. If not, revert them and investigate who caused the change. Consider altering permissions to prevent this from happening again in the future.\n"
     Reference = "https://aws.amazon.com/config/"
     SummaryAttributes = [
         "eventName",
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import List
 
 from panther_detection_helpers.caching import check_account_age
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import lookup_aws_account_name
 from pypanther.log_types import LogType
 
 aws_console_login_without_mfa_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="No MFA Login - IAM User",
@@ -386,15 +386,15 @@
     Tags = [
         "AWS",
         "Identity & Access Management",
         "Authentication",
         "Initial Access:Valid Accounts",
     ]
     Reports = {"CIS": ["3.2"], "MITRE ATT&CK": ["TA0001:T1078"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A console login was made without multi-factor authentication."
     Runbook = (
         "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-console-login-without-mfa"
     )
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa.html"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_console_login_without_mfa_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import lookup_aws_account_name
 from pypanther.log_types import LogType
 
 aws_console_login_without_saml_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Login with SAML",
@@ -79,15 +79,15 @@
     Tags = [
         "AWS",
         "Configuration Required",
         "Identity & Access Management",
         "Authentication",
         "Initial Access:Valid Accounts",
     ]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "An AWS console login was made without SAML/SSO."
     Runbook = "Modify the AWS account configuration."
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_providers_enable-console-saml.html"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_console_login_without_saml_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_default import lookup_aws_account_name
 from pypanther.helpers.panther_oss_helpers import geoinfo_from_ip_formatted
 from pypanther.log_types import LogType
 
 aws_console_root_login_tests: List[PantherRuleTest] = [
     PantherRuleTest(
@@ -104,15 +104,15 @@
         "AWS",
         "Identity & Access Management",
         "Authentication",
         "DemoThreatHunting",
         "Privilege Escalation:Valid Accounts",
     ]
     Reports = {"CIS": ["3.6"], "MITRE ATT&CK": ["TA0004:T1078"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "The root account has been logged into."
     Runbook = "Investigate the usage of the root account. If this root activity was not authorized, immediately change the root credentials and investigate what actions the root account took.\n"
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_console_root_login_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import lookup_aws_account_name
 from pypanther.log_types import LogType
 
 aws_console_root_login_failed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Failed Root Login",
@@ -128,15 +128,15 @@
         "Identity & Access Management",
         "Authentication",
         "DemoThreatHunting",
         "Credential Access:Brute Force",
     ]
     Threshold = 5
     Reports = {"CIS": ["3.6"], "MITRE ATT&CK": ["TA0006:T1110"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A Root console login failed."
     Runbook = "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-console-login-failed"
     Reference = "https://amzn.to/3aMSmTd"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_console_root_login_failed_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsec2_ebs_encryption_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="DisableEbsEncryptionByDefault Event",
         ExpectedResult=True,
@@ -38,15 +38,15 @@
     Description = "Identifies disabling of default EBS encryption. Disabling default encryption does not change the encryption status of existing volumes. "
     DisplayName = "AWS EC2 EBS Encryption Disabled"
     Reports = {"MITRE ATT&CK": ["TA0040:T1486", "TA0040:T1565"]}
     Runbook = (
         "Verify this action was intended and if any EBS volumes were created after the change."
     )
     Reference = "https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html#encryption-by-default"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.EC2.EBS.Encryption.Disabled-prototype"
     Tests = awsec2_ebs_encryption_disabled_tests
 
     def rule(self, event):
         return (
             event.get("eventSource") == "ec2.amazonaws.com"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsec2_gateway_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Network Gateway Modified",
@@ -135,15 +135,15 @@
 
 class AWSEC2GatewayModified(PantherRule):
     RuleID = "AWS.EC2.GatewayModified-prototype"
     DisplayName = "EC2 Network Gateway Modified"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Defense Evasion:Impair Defenses"]
     Reports = {"CIS": ["3.12"], "MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "An EC2 Network Gateway was modified."
     Runbook = "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-ec2-gateway-modified"
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get, pattern_match_list
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsec2_manual_security_group_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="AWS Console - Ingress SG Authorization",
@@ -324,15 +324,15 @@
 class AWSEC2ManualSecurityGroupChange(PantherRule):
     RuleID = "AWS.EC2.ManualSecurityGroupChange-prototype"
     DisplayName = "AWS EC2 Manual Security Group Change"
     Enabled = False
     LogTypes = [LogType.AWS_CloudTrail]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
     Tags = ["AWS", "Security Control", "Configuration Required", "Defense Evasion:Impair Defenses"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An EC2 security group was manually updated without abiding by the organization's accepted processes. This rule expects organizations to either use the Console, CloudFormation, or Terraform, configurable in the rule's ALLOWED_USER_AGENTS.\n"
     Runbook = "Identify the actor who changed the security group and validate it was legitimate"
     Reference = (
         "https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/working-with-security-groups.html"
     )
     Tests = awsec2_manual_security_group_change_tests
     PROD_ACCOUNT_IDS = {"11111111111111", "112233445566"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 awsec2_monitoring_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CopyImage",
         ExpectedResult=True,
@@ -416,15 +416,15 @@
 
 class AWSEC2Monitoring(PantherRule):
     Description = "Checks CloudTrail for occurrences of EC2 Image Actions."
     DisplayName = "AWS EC2 Image Monitoring"
     Reports = {"MITRE ATT&CK": ["TA0002:T1204"]}
     Runbook = "Verify that the action was not taken by a malicious actor."
     Reference = "https://docs.aws.amazon.com/service-authorization/latest/reference/list_amazonec2imagebuilder.html#amazonec2imagebuilder-actions-as-permissions"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Tags = ["ec2"]
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.EC2.Monitoring-prototype"
     Tests = awsec2_monitoring_tests
     # AWS CloudTrail API eventNames for EC2 Image Actions
     EC2_IMAGE_ACTIONS = [
         "CopyFpgaImage",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsec2_network_acl_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Network ACL Modified",
@@ -153,15 +153,15 @@
 
 class AWSEC2NetworkACLModified(PantherRule):
     RuleID = "AWS.EC2.NetworkACLModified-prototype"
     DisplayName = "EC2 Network ACL Modified"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Defense Evasion:Impair Defenses"]
     Reports = {"CIS": ["3.11"], "MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "An EC2 Network ACL was modified."
     Runbook = (
         "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-ec2-network-acl-modified"
     )
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html#nacl-tasks"
     SummaryAttributes = [
         "eventName",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsec2_route_table_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Route Table Modified",
@@ -143,15 +143,15 @@
 
 class AWSEC2RouteTableModified(PantherRule):
     RuleID = "AWS.EC2.RouteTableModified-prototype"
     DisplayName = "EC2 Route Table Modified"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Exfiltration:Exfiltration Over Alternative Protocol"]
     Reports = {"CIS": ["3.13"], "MITRE ATT&CK": ["TA0010:T1048"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "An EC2 Route Table was modified."
     Runbook = (
         "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-ec2-route-table-modified"
     )
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/WorkWithRouteTables.html"
     SummaryAttributes = [
         "eventName",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsec2_security_group_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Security Group Modified",
@@ -172,15 +172,15 @@
 
 class AWSEC2SecurityGroupModified(PantherRule):
     RuleID = "AWS.EC2.SecurityGroupModified-prototype"
     DisplayName = "EC2 Security Group Modified"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Defense Evasion:Impair Defenses"]
     Reports = {"CIS": ["3.1"], "MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     DedupPeriodMinutes = 720
     Description = "An EC2 Security Group was modified.\n"
     Runbook = (
         "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-ec2-securitygroup-modified"
     )
     Reference = (
         "https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/working-with-security-groups.html"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 awsec2_startup_script_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="ModifyInstanceAttribute-NoUserData",
         ExpectedResult=False,
@@ -103,15 +103,15 @@
 class AWSEC2StartupScriptChange(PantherRule):
     Description = "Detects changes to the EC2 instance startup script. The shell script will be executed as root/SYSTEM every time the specific instances are booted up."
     DisplayName = "AWS EC2 Startup Script Change"
     Reports = {"MITRE ATT&CK": ["TA0002:T1059"]}
     Reference = (
         "https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html#user-data-shell-scripts"
     )
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.EC2.Startup.Script.Change-prototype"
     Tests = awsec2_startup_script_change_tests
 
     def rule(self, event):
         if event.get("eventName") == "ModifyInstanceAttribute" and deep_get(
             event, "requestParameters", "userData"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 awsec2_traffic_mirroring_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CreateTrafficMirrorFilter",
         ExpectedResult=True,
@@ -605,15 +605,15 @@
 
 
 class AWSEC2TrafficMirroring(PantherRule):
     Description = "This rule captures multiple traffic mirroring events in AWS Cloudtrail."
     DisplayName = "AWS EC2 Traffic Mirroring"
     Reference = "https://attack.mitre.org/techniques/T1040/"
     Runbook = "Examine other activities done by this user to determine whether or not activity is suspicious. If your network traffic is not encrypted, we recommend changing the severity to high or critical."
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Tags = ["AWS", "Cloudtrail", "MITRE"]
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.EC2.Traffic.Mirroring-prototype"
     SummaryAttributes = ["userIdentity.type"]
     Tests = awsec2_traffic_mirroring_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsec2_vpc_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="VPC Modified",
@@ -184,15 +184,15 @@
 
 class AWSEC2VPCModified(PantherRule):
     RuleID = "AWS.EC2.VPCModified-prototype"
     DisplayName = "EC2 VPC Modified"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Defense Evasion:Impair Defenses"]
     Reports = {"CIS": ["3.14"], "MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     DedupPeriodMinutes = 720
     Description = "An EC2 VPC was modified."
     Runbook = "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-ec2-vpc-modified"
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/configure-your-vpc.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.helpers.panther_iocs import XZ_AMIS
 from pypanther.log_types import LogType
 
 awsec2_vulnerable_xz_image_launched_tests: List[PantherRuleTest] = [
     PantherRuleTest(
@@ -720,15 +720,15 @@
 ]
 
 
 class AWSEC2VulnerableXZImageLaunched(PantherRule):
     Description = "Detecting EC2 instances launched with AMIs containing potentially vulnerable versions of XZ (CVE-2024-3094)\n"
     DisplayName = "AWS EC2 Vulnerable XZ Image Launched"
     Reference = "https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-3094"
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Tags = ["AWS", "Linux", "Emerging Threats", "Supply Chain Compromise"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195.001"]}
     Runbook = "- Verify that the AMI is indeed vulnerable to CVE-2024-3094 (xz -V being 5.6.0 or 5.6.1) - If the AMI is vulnerable, terminate the instance and launch a new instance with a non-vulnerable AMI\n"
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.EC2.Vulnerable.XZ.Image.Launched-prototype"
     Tests = awsec2_vulnerable_xz_image_launched_tests
     # AMIs published by Fedora between 2024-03-26 and 2024-04-02
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fnmatch import fnmatch
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 awsecrcrud_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Authorized account, unauthorized region",
         ExpectedResult=True,
@@ -174,15 +174,15 @@
 class AWSECRCRUD(PantherRule):
     RuleID = "AWS.ECR.CRUD-prototype"
     DisplayName = "ECR CRUD Actions"
     Enabled = False
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Configuration Required"]
     Reports = {"CIS": ["3.12"], "MITRE ATT&CK": ["TA0005:T1525"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Unauthorized ECR Create, Read, Update, or Delete event occurred."
     Runbook = "https://docs.aws.amazon.com/AmazonECR/latest/userguide/logging-using-cloudtrail.html"
     Reference = "https://docs.aws.amazon.com/AmazonECR/latest/userguide/security-iam.html#security_iam_authentication"
     SummaryAttributes = [
         "eventSource",
         "eventName",
         "recipientAccountId",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 awsecrevents_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Authorized account, unauthorized region",
         ExpectedResult=True,
@@ -173,15 +173,15 @@
 class AWSECREVENTS(PantherRule):
     RuleID = "AWS.ECR.EVENTS-prototype"
     DisplayName = "AWS ECR Events"
     Enabled = False
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1535"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An ECR event occurred outside of an expected account or region"
     Runbook = "https://docs.aws.amazon.com/AmazonECR/latest/userguide/logging-using-cloudtrail.html"
     Reference = "https://aws.amazon.com/blogs/containers/amazon-ecr-in-multi-account-and-multi-region-architectures/"
     SummaryAttributes = ["eventSource", "recipientAccountId", "awsRegion", "p_any_aws_arns"]
     Tests = awsecrevents_tests
     # CONFIGURATION REQUIRED: Update with your expected AWS Accounts/Regions
     AWS_ACCOUNTS_AND_REGIONS = {
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_iam_anything_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="IAM Change",
@@ -140,15 +140,15 @@
 
 
 class AWSCloudTrailIAMAnythingChanged(PantherRule):
     RuleID = "AWS.CloudTrail.IAMAnythingChanged-prototype"
     DisplayName = "IAM Change"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Identity and Access Management"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     DedupPeriodMinutes = 720
     Description = "A change occurred in the IAM configuration. This could be a resource being created, deleted, or modified. This is a high level view of changes, helfpul to indicate how dynamic a certain IAM environment is.\n"
     Runbook = "Ensure this was an approved IAM configuration change.\n"
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/cloudtrail-integration.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_iam_assume_role_blacklist_ignored_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="IAM Blocklisted Role Assumed",
@@ -186,15 +186,15 @@
     Tags = [
         "AWS",
         "Configuration Required",
         "Identity and Access Management",
         "Privilege Escalation:Abuse Elevation Control Mechanism",
     ]
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "A user assumed a role that was explicitly blocklisted for manual user assumption.\n"
     )
     Runbook = "Verify that this was an approved assume role action. If not, consider revoking the access immediately and updating the AssumeRolePolicyDocument to prevent this from happening again.\n"
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_boundaries.html"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_cloud_trail_iam_assume_role_blacklist_ignored_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 aws_cloud_trail_iam_compromised_key_quarantine_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="AttachUserPolicy AWSCompromisedKeyQuarantineV2-true",
         ExpectedResult=True,
         Log={
@@ -103,15 +103,15 @@
 
 
 class AWSCloudTrailIAMCompromisedKeyQuarantine(PantherRule):
     LogTypes = [LogType.AWS_CloudTrail]
     Description = "Detects when an IAM user has the AWSCompromisedKeyQuarantineV2 policy attached to their account."
     DisplayName = "AWS Compromised IAM Key Quarantine"
     RuleID = "AWS.CloudTrail.IAMCompromisedKeyQuarantine-prototype"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = [
         "AWS",
         "Identity and Access Management",
         "Initial Access:Valid Accounts",
         "Credential Access:Unsecured Credentials",
     ]
     Reports = {"MITRE ATT&CK": ["TA0001:T1078.004", "TA0006:T1552.001"]}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_iam_entity_created_without_cloud_formation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="IAM Entity Created Automatically",
@@ -255,15 +255,15 @@
     Reports = {"MITRE ATT&CK": ["TA0003:T1136"]}
     Tags = [
         "AWS",
         "Configuration Required",
         "Identity and Access Management",
         "Persistence:Create Account",
     ]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An IAM Entity (Group, Policy, Role, or User) was created manually. IAM entities should be created in code to ensure that permissions are tracked and managed correctly.\n"
     Runbook = "Verify whether IAM entity needs to exist. If so, re-create it in an appropriate CloudFormation, Terraform, or other template. Delete the original manually created entity.\n"
     Reference = "https://blog.awsfundamentals.com/aws-iam-roles-with-aws-cloudformation"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_cloud_trail_iam_entity_created_without_cloud_formation_tests
     # The role dedicated for IAM administration
     IAM_ADMIN_ROLES = {"arn:aws:iam::123456789012:role/IdentityCFNServiceRole"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsiam_group_read_only_events_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Get Group",
         ExpectedResult=True,
@@ -268,15 +268,15 @@
 
 class AWSIAMGroupReadOnlyEvents(PantherRule):
     Description = "This rule captures multiple read/list events related to IAM group management in AWS Cloudtrail."
     DisplayName = "AWS IAM Group Read Only Events"
     Enabled = False
     Reference = "https://attack.mitre.org/techniques/T1069/"
     Runbook = "Examine other activities done by this user to determine whether or not activity is suspicious."
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Tags = ["AWS", "Cloudtrail", "Configuration Required", "IAM", "MITRE"]
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.IAM.Group.Read.Only.Events-prototype"
     Threshold = 2
     Tests = awsiam_group_read_only_events_tests
     # arn allow list to suppress alerts
     ARN_ALLOW_LIST = []
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsiam_policy_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="IAM Policy Change",
@@ -143,15 +143,15 @@
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = [
         "AWS",
         "Identity & Access Management",
         "Privilege Escalation:Abuse Elevation Control Mechanism",
     ]
     Reports = {"CIS": ["3.4"], "MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     DedupPeriodMinutes = 720
     Description = "An IAM Policy was changed.\n"
     Runbook = "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-iam-policy-modified"
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsiam_backdoor_user_keys_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="user1 create keys for user1",
@@ -233,15 +233,15 @@
 
 
 class AWSIAMBackdoorUserKeys(PantherRule):
     Description = "Detects AWS API key creation for a user by another user. Backdoored users can be used to obtain persistence in the AWS environment."
     DisplayName = "AWS User API Key Created"
     Reports = {"MITRE ATT&CK": ["TA0003:T1098", "TA0005:T1108", "TA0005:T1550", "TA0008:T1550"]}
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.IAM.Backdoor.User.Keys-prototype"
     Tests = awsiam_backdoor_user_keys_tests
 
     def rule(self, event):
         return (
             aws_cloudtrail_success(event)
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ipaddress import ip_address
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import lookup_aws_account_name
 from pypanther.log_types import LogType
 
 awsiam_user_recon_access_denied_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Unauthorized API Call",
@@ -154,15 +154,15 @@
 
 class AWSIAMUserReconAccessDenied(PantherRule):
     RuleID = "AWS.IAMUser.ReconAccessDenied-prototype"
     DisplayName = "Detect Reconnaissance from IAM Users"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Discovery:Cloud Service Discovery"]
     Reports = {"MITRE ATT&CK": ["TA0007:T1526"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Threshold = 15
     DedupPeriodMinutes = 10
     Description = "An IAM user has a high volume of access denied API calls."
     Runbook = "Analyze the IP they came from, and other actions taken before/after."
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/troubleshoot_access-denied.html"
     SummaryAttributes = [
         "eventName",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsip_set_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CreateIPSet Event",
         ExpectedResult=True,
@@ -63,15 +63,15 @@
 
 
 class AWSIPSetModified(PantherRule):
     Description = "Detects creation and updates of the list of trusted IPs used by GuardDuty and WAF. Potentially to disable security alerts against malicious IPs."
     DisplayName = "AWS Trusted IPSet Modified"
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
     Reference = "https://docs.aws.amazon.com/managedservices/latest/ctref/management-monitoring-guardduty-ip-set-update-review-required.html"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.IPSet.Modified-prototype"
     Tests = awsip_set_modified_tests
     IPSET_ACTIONS = ["CreateIPSet", "UpdateIPSet"]
 
     def rule(self, event):
         if (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 awsiam_access_key_compromised_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="An AWS Access Key was Uploaded to Github",
         ExpectedResult=True,
@@ -68,15 +68,15 @@
 
 class AWSIAMAccessKeyCompromised(PantherRule):
     RuleID = "AWS.IAM.AccessKeyCompromised-prototype"
     DisplayName = "AWS Access Key Uploaded to Github"
     LogTypes = [LogType.AWS_CloudTrail]
     Reports = {"MITRE ATT&CK": ["TA0006:T1552"]}
     Tags = ["AWS", "Credential Access:Unsecured Credentials"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A users static AWS API key was uploaded to a public github repo."
     Runbook = "Determine the key owner, disable/delete key, and delete the user to resolve the AWS case. If user needs a new IAM give them a stern talking to first."
     Reference = "https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning"
     Tests = awsiam_access_key_compromised_tests
     EXPOSED_CRED_POLICY = "AWSExposedCredentialPolicy_DO_NOT_REMOVE"
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awskms_customer_managed_key_loss_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="KMS Key Disabled",
@@ -260,15 +260,15 @@
 
 class AWSKMSCustomerManagedKeyLoss(PantherRule):
     RuleID = "AWS.KMS.CustomerManagedKeyLoss-prototype"
     DisplayName = "KMS CMK Disabled or Deleted"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Identity & Access Management", "Impact:Data Destruction"]
     Reports = {"CIS": ["3.7"], "MITRE ATT&CK": ["TA0040:T1485"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A KMS Customer Managed Key was disabled or scheduled for deletion. This could potentially lead to permanent loss of encrypted data.\n"
     Runbook = "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-kms-cmk-loss"
     Reference = "https://docs.aws.amazon.com/kms/latest/developerguide/deleting-keys.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fnmatch import fnmatch
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 awslambdacrud_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Lambda DeleteFunction Unauthorized Account",
         ExpectedResult=True,
@@ -93,15 +93,15 @@
 class AWSLAMBDACRUD(PantherRule):
     RuleID = "AWS.LAMBDA.CRUD-prototype"
     DisplayName = "Lambda CRUD Actions"
     Enabled = False
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Security Control", "Configuration Required"]
     Reports = {"CIS": ["3.12"], "MITRE ATT&CK": ["TA0005:T1525"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Unauthorized lambda Create, Read, Update, or Delete event occurred."
     Runbook = "https://docs.aws.amazon.com/lambda/latest/dg/logging-using-cloudtrail.html"
     Reference = "https://docs.aws.amazon.com/lambda/latest/dg/logging-using-cloudtrail.html"
     SummaryAttributes = [
         "eventSource",
         "eventName",
         "recipientAccountId",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, pattern_match
 from pypanther.log_types import LogType
 
 aws_macie_evasion_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="ListMembers",
         ExpectedResult=False,
@@ -174,15 +174,15 @@
 
 
 class AWSMacieEvasion(PantherRule):
     RuleID = "AWS.Macie.Evasion-prototype"
     DisplayName = "AWS Macie Disabled/Updated"
     LogTypes = [LogType.AWS_CloudTrail]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Amazon Macie is a data security and data privacy service to discover and protect sensitive data. Security teams use Macie to detect open S3 Buckets that could have potentially sensitive data in it along with  policy violations, such as missing Encryption. If an attacker disables Macie, it could potentially hide data exfiltration.\n"
     Reference = "https://aws.amazon.com/macie/"
     Runbook = "Analyze the events to ensure it's not normal maintenance. If it's abnormal, run the Indicator Search on the UserIdentity:Arn for the past hour and analyze other services accessed/changed.\n"
     Threshold = 5
     SummaryAttributes = [
         "awsRegion",
         "eventName",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 aws_modify_cloud_compute_infrastructure_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Terminate Instance from AssumedRole",
         ExpectedResult=True,
@@ -465,15 +465,15 @@
 
 
 class AWSModifyCloudComputeInfrastructure(PantherRule):
     Description = "Detection when EC2 compute infrastructure is modified outside of expected automation methods."
     DisplayName = "AWS Modify Cloud Compute Infrastructure"
     Enabled = False
     Reference = "https://attack.mitre.org/techniques/T1578/"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0005:T1578"]}
     Tags = ["Configuration Required"]
     Runbook = "This detection reports on eventSource ec2 Change events. This detection excludes Cross-Service change events.  As such, this detection will perform well in environments where changes are  expected to originate only from AWS service entities.\nThis detection will emit alerts frequently in environments where users are making ec2 related changes.\n"
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.Modify.Cloud.Compute.Infrastructure-prototype"
     Tests = aws_modify_cloud_compute_infrastructure_tests
     EC2_CRUD_ACTIONS = {
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_network_acl_permissive_entry_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Overly Permissive Entry Added",
@@ -158,15 +158,15 @@
 
 
 class AWSCloudTrailNetworkACLPermissiveEntry(PantherRule):
     RuleID = "AWS.CloudTrail.NetworkACLPermissiveEntry-prototype"
     DisplayName = "AWS Network ACL Overly Permissive Entry Created"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Persistence:Account Manipulation"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Description = "A Network ACL entry that allows access from anywhere was added.\n"
     Runbook = "Remove the overly permissive Network ACL entry and add a new entry with more restrictive permissions.\n"
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html#nacl-rules"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_cloud_trail_network_acl_permissive_entry_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsrds_manual_snapshot_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Manual Snapshot Created",
         ExpectedResult=True,
@@ -314,15 +314,15 @@
 
 class AWSRDSManualSnapshotCreated(PantherRule):
     RuleID = "AWS.RDS.ManualSnapshotCreated-prototype"
     DisplayName = "AWS RDS Manual/Public Snapshot Created"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Exfiltration", "Transfer Data to Cloud Account"]
     Reports = {"MITRE ATT&CK": ["TA0010:T1537"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A manual snapshot of an RDS database was created.  An attacker may use this to exfiltrate the DB contents to another account; use this as a correlation rule.\n"
     Runbook = "Ensure the snapshot was shared with an allowed AWS account. If not, delete the snapshot and quarantine the compromised IAM user.\n"
     Reference = "https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_CreateSnapshot.html"
     SummaryAttributes = ["eventSource", "recipientAccountId", "awsRegion", "p_any_aws_arns"]
     Tests = awsrds_manual_snapshot_created_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 awsrds_master_password_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Allocated storage modified",
         ExpectedResult=False,
@@ -290,15 +290,15 @@
 
 class AWSRDSMasterPasswordUpdated(PantherRule):
     Description = "A sensitive database operation that should be performed carefully or rarely"
     DisplayName = "AWS RDS Master Password Updated"
     Reference = (
         "https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Overview.DBInstance.Modifying.html"
     )
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     SummaryAttributes = [
         "awsRegion",
         "userIdentity:arn",
         "responseElements:dBInstanceIdentifier",
         "p_any_aws_arns",
         "p_any_aws_account_ids",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 awsrds_public_restore_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Not-Restore-RDS-Request",
         ExpectedResult=False,
@@ -353,15 +353,15 @@
 class AWSRDSPublicRestore(PantherRule):
     Description = "Detects the recovery of a new public database instance from a snapshot. It may be part of data exfiltration."
     DisplayName = "AWS Public RDS Restore"
     Reports = {"MITRE ATT&CK": ["TA0010:T1020"]}
     Reference = (
         "https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_RestoreFromSnapshot.html"
     )
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.RDS.PublicRestore-prototype"
     Tests = awsrds_public_restore_tests
 
     def rule(self, event):
         if (
             event.get("eventSource", "") == "rds.amazonaws.com"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsrds_snapshot_shared_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snapshot shared with another account",
         ExpectedResult=True,
@@ -121,15 +121,15 @@
 
 
 class AWSRDSSnapshotShared(PantherRule):
     RuleID = "AWS.RDS.SnapshotShared-prototype"
     DisplayName = "AWS RDS Snapshot Shared"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Exfiltration", "Transfer Data to Cloud Account"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reports = {"MITRE ATT&CK": ["TA0010:T1537"]}
     Description = "An RDS snapshot was shared with another account. This could be an indicator of exfiltration.\n"
     Runbook = "Ensure that the snapshot was shared intentionally and with an approved account. If not, remove the snapshot and quarantine the compromised IAM user.\n"
     Reference = "https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_ShareSnapshot.html"
     SummaryAttributes = ["eventSource", "recipientAccountId", "awsRegion", "p_any_aws_arns"]
     Tests = awsrds_snapshot_shared_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import List
 
 from policyuniverse.policy import Policy
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_resource_made_public_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="ECR Made Public",
@@ -360,15 +360,15 @@
 
 
 class AWSCloudTrailResourceMadePublic(PantherRule):
     RuleID = "AWS.CloudTrail.ResourceMadePublic-prototype"
     DisplayName = "AWS Resource Made Public"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Exfiltration:Transfer Data to Cloud Account"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0010:T1537"]}
     Description = "Some AWS resource was made publicly accessible over the internet. Checks ECR, Elasticsearch, KMS, S3, S3 Glacier, SNS, SQS, and Secrets Manager.\n"
     Runbook = "Adjust the policy so that the resource is no longer publicly accessible"
     Reference = "https://aws.amazon.com/blogs/security/identifying-publicly-accessible-resources-with-amazon-vpc-network-access-analyzer/"
     SummaryAttributes = [
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_cloud_trail_root_access_key_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Root Access Key Created",
         ExpectedResult=True,
@@ -89,15 +89,15 @@
 
 class AWSCloudTrailRootAccessKeyCreated(PantherRule):
     RuleID = "AWS.CloudTrail.RootAccessKeyCreated-prototype"
     DisplayName = "Root Account Access Key Created"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Identity and Access Management", "Persistence:Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Description = "An access key was created for the Root account"
     Runbook = "Verify that the root access key was created for legitimate reasons. If not, immediately revoke it and change the root login credentials. If it was created for legitimate reasons, monitor its use and ensure it is revoked when its need is gone.\n"
     Reference = "https://docs.aws.amazon.com/general/latest/gr/managing-aws-access-keys.html"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_cloud_trail_root_access_key_created_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success, lookup_aws_account_name
 from pypanther.log_types import LogType
 
 aws_root_activity_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Root Activity - CreateServiceLinkedRole",
@@ -226,15 +226,15 @@
     Tags = [
         "AWS",
         "Identity & Access Management",
         "DemoThreatHunting",
         "Privilege Escalation:Valid Accounts",
     ]
     Reports = {"CIS": ["3.3"], "MITRE ATT&CK": ["TA0004:T1078"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Root account activity was detected.\n"
     Runbook = "Investigate the usage of the root account. If this root activity was not authorized, immediately change the root credentials and investigate what actions the root account took.\n"
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html"
     SummaryAttributes = [
         "awsRegion",
         "eventName",
         "eventSource",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_cloud_trail_root_password_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Root Password Changed",
         ExpectedResult=True,
@@ -63,15 +63,15 @@
 
 
 class AWSCloudTrailRootPasswordChanged(PantherRule):
     RuleID = "AWS.CloudTrail.RootPasswordChanged-prototype"
     DisplayName = "Root Password Changed"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Identity and Access Management", "Persistence:Account Manipulation"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Description = "Someone manually changed the Root console login password.\n"
     Runbook = "Verify that the root password change was authorized. If not, AWS support should be contacted immediately as the root account cannot be recovered through normal means and grants complete access to the account.\n"
     Reference = (
         "https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_change-root.html"
     )
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awss3_bucket_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="An S3 Bucket was deleted",
@@ -94,15 +94,15 @@
 
 class AWSS3BucketDeleted(PantherRule):
     RuleID = "AWS.S3.BucketDeleted-prototype"
     DisplayName = "S3 Bucket Deleted"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Impact:Data Destruction"]
     Reports = {"MITRE ATT&CK": ["TA0040:T1485"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A S3 Bucket, Policy, or Website was deleted"
     Runbook = "Explore if this bucket deletion was potentially destructive"
     Reference = "https://docs.aws.amazon.com/AmazonS3/latest/userguide/DeletingObjects.html"
     SummaryAttributes = ["sourceIpAddress", "userAgent", "recipientAccountId", "vpcEndpointId"]
     Tests = awss3_bucket_deleted_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awss3_bucket_policy_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="S3 Bucket Policy Modified",
@@ -158,15 +158,15 @@
 
 class AWSS3BucketPolicyModified(PantherRule):
     RuleID = "AWS.S3.BucketPolicyModified-prototype"
     DisplayName = "AWS S3 Bucket Policy Modified"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Identity & Access Management", "Exfiltration:Exfiltration Over Web Service"]
     Reports = {"CIS": ["3.8"], "MITRE ATT&CK": ["TA0010:T1567"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     DedupPeriodMinutes = 720
     Description = "An S3 Bucket was modified.\n"
     Runbook = (
         "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-s3-bucket-policy-modified"
     )
     Reference = "https://docs.aws.amazon.com/AmazonS3/latest/dev/using-iam-policies.html"
     SummaryAttributes = ["eventName", "userAgent", "sourceIpAddress", "p_any_aws_arns"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_suspicious_saml_activity_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CreateSAMLProvider",
         ExpectedResult=True,
@@ -257,15 +257,15 @@
 ]
 
 
 class AWSSuspiciousSAMLActivity(PantherRule):
     Description = "Identifies when SAML activity has occurred in AWS. An adversary could gain backdoor access via SAML."
     DisplayName = "AWS SAML Activity"
     Reference = "https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-managing-saml-idp-console.html"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.Suspicious.SAML.Activity-prototype"
     Tests = aws_suspicious_saml_activity_tests
     SAML_ACTIONS = ["UpdateSAMLProvider", "CreateSAMLProvider", "DeleteSAMLProvider"]
 
     def rule(self, event):
         # Allow AWSSSO to manage
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fnmatch import fnmatch
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_security_configuration_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Security Configuration Changed",
@@ -222,15 +222,15 @@
 
 
 class AWSCloudTrailSecurityConfigurationChange(PantherRule):
     RuleID = "AWS.CloudTrail.SecurityConfigurationChange-prototype"
     DisplayName = "Account Security Configuration Changed"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Defense Evasion:Impair Defenses"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
     Description = "An account wide security configuration was changed."
     Runbook = "Verify that this change was planned. If not, revert the change and update the access control policies to ensure this doesn't happen again.\n"
     Reference = "https://docs.aws.amazon.com/prescriptive-guidance/latest/aws-startup-security-baseline/controls-acct.html"
     SummaryAttributes = [
         "eventName",
         "userAgent",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 aws_security_hub_finding_evasion_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CreateInsight",
         ExpectedResult=False,
@@ -111,15 +111,15 @@
 
 
 class AWSSecurityHubFindingEvasion(PantherRule):
     Description = "Detections modification of findings in SecurityHub"
     DisplayName = "AWS SecurityHub Finding Evasion"
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
     Reference = "https://docs.aws.amazon.com/securityhub/latest/userguide/securityhub-insights-view-take-action.html"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.SecurityHub.Finding.Evasion-prototype"
     Tests = aws_security_hub_finding_evasion_tests
     EVASION_OPERATIONS = ["BatchUpdateFindings", "DeleteInsight", "UpdateFindings", "UpdateInsight"]
 
     def rule(self, event):
         if (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Mapping
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 aws_cloud_trail_snapshot_made_public_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snapshot Made Publicly Accessible",
@@ -145,15 +145,15 @@
 
 class AWSCloudTrailSnapshotMadePublic(PantherRule):
     RuleID = "AWS.CloudTrail.SnapshotMadePublic-prototype"
     DisplayName = "AWS Snapshot Made Public"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Exfiltration:Transfer Data to Cloud Account"]
     Reports = {"MITRE ATT&CK": ["TA0010:T1537"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An AWS storage snapshot was made public."
     Runbook = "Adjust the snapshot configuration so that it is no longer public."
     Reference = "https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-modifying-snapshot-permissions.html"
     SummaryAttributes = ["userAgent", "sourceIpAddress", "recipientAccountId", "p_any_aws_arns"]
     Tests = aws_cloud_trail_snapshot_made_public_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_software_discovery_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Discovery Event Names",
         ExpectedResult=True,
@@ -84,15 +84,15 @@
 class AWSSoftwareDiscovery(PantherRule):
     Description = "A user is obtaining a list of security software, configurations, defensive tools, and sensors that are in AWS."
     DisplayName = "AWS Software Discovery"
     Enabled = False
     Reference = "https://attack.mitre.org/techniques/T1518/001/"
     Tags = ["Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0007:T1518"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     DedupPeriodMinutes = 360
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.Software.Discovery-prototype"
     Threshold = 50
     Tests = aws_software_discovery_tests
     DISCOVERY_EVENTS = [
         "ListDocuments",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ipaddress import ip_address
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_cloud_trail_unauthorized_api_call_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Unauthorized API Call from Within AWS (IP)",
         ExpectedResult=True,
@@ -118,15 +118,15 @@
 class AWSCloudTrailUnauthorizedAPICall(PantherRule):
     RuleID = "AWS.CloudTrail.UnauthorizedAPICall-prototype"
     DisplayName = "Monitor Unauthorized API Calls"
     DedupPeriodMinutes = 1440
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Discovery:Cloud Service Discovery"]
     Reports = {"CIS": ["3.1"], "MITRE ATT&CK": ["TA0007:T1526"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "An unauthorized AWS API call was made"
     Runbook = "https://docs.runpanther.io/alert-runbooks/built-in-rules/aws-unauthorized-api-call"
     Reference = "https://amzn.to/3aOukaA"
     SummaryAttributes = [
         "eventName",
         "userAgent",
         "sourceIpAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_unused_region_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Authorized region",
         ExpectedResult=False,
@@ -155,15 +155,15 @@
 class AWSUnusedRegion(PantherRule):
     RuleID = "AWS.UnusedRegion-prototype"
     DisplayName = "Unused AWS Region"
     Enabled = False
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["AWS", "Defense Evasion:Unused/Unsupported Cloud Regions", "Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1535"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "CloudTrail logged non-read activity from a verboten AWS region."
     Runbook = "https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_examples_aws-enable-disable-regions.html"
     Reference = "https://attack.mitre.org/techniques/T1535/"
     SummaryAttributes = [
         "eventSource",
         "eventName",
         "recipientAccountId",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.helpers.panther_default import aws_cloudtrail_success
 from pypanther.log_types import LogType
 
 awsiam_credentials_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User Password Was Changed",
@@ -117,15 +117,15 @@
 
 class AWSIAMCredentialsUpdated(PantherRule):
     RuleID = "AWS.IAM.CredentialsUpdated-prototype"
     DisplayName = "New IAM Credentials Updated"
     LogTypes = [LogType.AWS_CloudTrail]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Tags = ["AWS", "Identity & Access Management", "Persistence:Account Manipulation"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A console password, access key, or user has been created."
     Runbook = "This rule is purely informational, there is no action needed."
     Reference = (
         "https://docs.aws.amazon.com/IAM/latest/UserGuide/list_identityandaccessmanagement.html"
     )
     SummaryAttributes = [
         "eventName",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, deep_get
 from pypanther.log_types import LogType
 
 aws_user_login_profile_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="ChangeOwnPassword",
         ExpectedResult=False,
@@ -135,15 +135,15 @@
 
 
 class AWSUserLoginProfileModified(PantherRule):
     Description = "An attacker with iam:UpdateLoginProfile permission on other users can change the password used to login to the AWS console. May be legitimate account administration."
     DisplayName = "AWS User Login Profile Modified"
     Reports = {"MITRE ATT&CK": ["TA0003:T1098", "TA0005:T1108", "TA0005:T1550", "TA0008:T1550"]}
     Reference = "https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_examples_aws_my-sec-creds-self-manage-pass-accesskeys-ssh.html"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.User.Login.Profile.Modified-prototype"
     Tests = aws_user_login_profile_modified_tests
 
     def rule(self, event):
         return (
             event.get("eventSource", "") == "iam.amazonaws.com"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py` & `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 awswaf_disassociation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="WAF-Disassociate",
         ExpectedResult=True,
@@ -128,15 +128,15 @@
 ]
 
 
 class AWSWAFDisassociation(PantherRule):
     Description = "Detection to alert when a WAF disassociates from a source."
     DisplayName = "AWS WAF Disassociation"
     Reference = "https://attack.mitre.org/techniques/T1078/"
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Reports = {"MITRE ATT&CK": ["TA0004:T1498"]}
     LogTypes = [LogType.AWS_CloudTrail]
     RuleID = "AWS.WAF.Disassociation-prototype"
     Tests = awswaf_disassociation_tests
 
     def rule(self, event):
         return event.get("eventName") == "DisassociateWebACL"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py` & `pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ipaddress import ip_address
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import eks_panther_obj_ref
 from pypanther.log_types import LogType
 
 amazon_eks_audit_multiple403_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Not 403",
         ExpectedResult=False,
@@ -167,15 +167,15 @@
 class AmazonEKSAuditMultiple403(PantherRule):
     RuleID = "Amazon.EKS.Audit.Multiple403-prototype"
     DisplayName = "EKS Audit Log based single sourceIP is generating multiple 403s"
     LogTypes = [LogType.Amazon_EKS_Audit]
     Tags = ["EKS"]
     Reports = {"MITRE ATT&CK": ["TA0007:T1613"]}
     Reference = "https://aws.github.io/aws-eks-best-practices/security/docs/detective/"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "This detection identifies if a public sourceIP is generating multiple 403s with the Kubernetes API server.\n"
     DedupPeriodMinutes = 30
     Threshold = 10
     SummaryAttributes = ["user:username", "p_any_ip_addresses", "p_source_label"]
     Tests = amazon_eks_audit_multiple403_tests
     # Alert if
     #   state is ResponseComplete
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py` & `pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ipaddress import ip_address
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, eks_panther_obj_ref
 from pypanther.log_types import LogType
 
 amazon_eks_audit_system_namespace_from_public_ip_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="non-system username",
         ExpectedResult=False,
@@ -324,15 +324,15 @@
 class AmazonEKSAuditSystemNamespaceFromPublicIP(PantherRule):
     RuleID = "Amazon.EKS.Audit.SystemNamespaceFromPublicIP-prototype"
     DisplayName = "EKS Audit Log Reporting system Namespace is Used From A Public IP"
     LogTypes = [LogType.Amazon_EKS_Audit]
     Tags = ["EKS"]
     Reports = {"MITRE ATT&CK": ["TA0027:T1475"]}
     Reference = "https://docs.aws.amazon.com/eks/latest/userguide/network_reqs.html"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = 'This detection identifies if an activity is recorded in the Kubernetes audit log where  the user:username attribute begins with "system:" or "eks:" and the requests originating  IP Address is a Public IP Address\n'
     DedupPeriodMinutes = 1440
     SummaryAttributes = ["user:username", "p_source_label"]
     Tests = amazon_eks_audit_system_namespace_from_public_ip_tests
     # Explicitly ignore eks:node-manager and eks:addon-manager
     #  which are run as Lambdas and originate from public IPs
     AMZ_PUBLICS = {"eks:addon-manager", "eks:node-manager"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py` & `pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_guardduty_context, deep_get
 from pypanther.log_types import LogType
 
 aws_guard_duty_high_severity_finding_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="High Sev Finding",
         ExpectedResult=True,
@@ -91,15 +91,15 @@
 
 
 class AWSGuardDutyHighSeverityFinding(PantherRule):
     RuleID = "AWS.GuardDuty.HighSeverityFinding-prototype"
     DisplayName = "AWS GuardDuty High Severity Finding"
     LogTypes = [LogType.AWS_GuardDuty]
     Tags = ["AWS"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A high-severity GuardDuty finding has been identified.\n"
     Runbook = "Search related logs to understand the root cause of the activity.\n"
     Reference = "https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_findings.html#guardduty_findings-severity"
     SummaryAttributes = [
         "severity",
         "type",
         "title",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py` & `pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_guardduty_context, deep_get
 from pypanther.log_types import LogType
 
 aws_guard_duty_low_severity_finding_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Low Sev Finding",
         ExpectedResult=True,
@@ -91,15 +91,15 @@
 
 
 class AWSGuardDutyLowSeverityFinding(PantherRule):
     RuleID = "AWS.GuardDuty.LowSeverityFinding-prototype"
     DisplayName = "AWS GuardDuty Low Severity Finding"
     LogTypes = [LogType.AWS_GuardDuty]
     Tags = ["AWS"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     DedupPeriodMinutes = 1440
     Description = "A low-severity GuardDuty finding has been identified.\n"
     Runbook = "Search related logs to understand the root cause of the activity.\n"
     Reference = "https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_findings.html#guardduty_findings-severity"
     SummaryAttributes = [
         "severity",
         "type",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py` & `pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_guardduty_context, deep_get
 from pypanther.log_types import LogType
 
 aws_guard_duty_medium_severity_finding_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Medium Sev Finding",
         ExpectedResult=True,
@@ -91,15 +91,15 @@
 
 
 class AWSGuardDutyMediumSeverityFinding(PantherRule):
     RuleID = "AWS.GuardDuty.MediumSeverityFinding-prototype"
     DisplayName = "AWS GuardDuty Medium Severity Finding"
     LogTypes = [LogType.AWS_GuardDuty]
     Tags = ["AWS"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     DedupPeriodMinutes = 480
     Description = "A medium-severity GuardDuty finding has been identified.\n"
     Runbook = "Search related logs to understand the root cause of the activity.\n"
     Reference = "https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_findings.html#guardduty_findings-severity"
     SummaryAttributes = [
         "severity",
         "type",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_access_error.py` & `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_access_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, pattern_match
 from pypanther.log_types import LogType
 
 awss3_server_access_error_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Amazon Access Error",
         ExpectedResult=False,
@@ -82,15 +82,15 @@
     RuleID = "AWS.S3.ServerAccess.Error-prototype"
     DisplayName = "AWS S3 Access Error"
     DedupPeriodMinutes = 180
     Threshold = 5
     LogTypes = [LogType.AWS_S3ServerAccess]
     Tags = ["AWS", "Security Control", "Discovery:Cloud Storage Object Discovery"]
     Reports = {"MITRE ATT&CK": ["TA0007:T1619"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "Checks for errors during S3 Object access. This could be due to insufficient access permissions, non-existent buckets, or other reasons.\n"
     Runbook = "Investigate the specific error and determine if it is an ongoing issue that needs to be addressed or a one off or transient error that can be ignored.\n"
     Reference = "https://docs.aws.amazon.com/AmazonS3/latest/dev/ErrorCode.html"
     SummaryAttributes = ["bucket", "key", "requester", "remoteip", "operation", "errorCode"]
     Tests = awss3_server_access_error_tests
     # https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html
     # Forbidden
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py` & `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ipaddress import ip_network
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awss3_server_access_ip_whitelist_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Access From Approved IP",
         ExpectedResult=False,
@@ -27,15 +27,15 @@
     Tags = [
         "AWS",
         "Configuration Required",
         "Identity & Access Management",
         "Collection:Data From Cloud Storage Object",
     ]
     Reports = {"MITRE ATT&CK": ["TA0009:T1530"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Checks that the remote IP accessing the S3 bucket is in the IP allowlist.\n"
     Runbook = "Verify whether unapproved access of S3 objects occurred, and take appropriate steps to remediate damage (for example, informing related parties of unapproved access and potentially invalidating data that was accessed). Consider updating the access policies of the S3 bucket to prevent future unapproved access.\n"
     Reference = "https://aws.amazon.com/premiumsupport/knowledge-center/block-s3-traffic-vpc-ip/"
     SummaryAttributes = ["bucket", "key", "remoteip"]
     Tests = awss3_server_access_ip_whitelist_tests
     # Example bucket names to watch go here
     BUCKETS_TO_MONITOR = {}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py` & `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context, pattern_match
 from pypanther.log_types import LogType
 
 awss3_server_access_insecure_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Secure Access to S3 Bucket",
         ExpectedResult=False,
@@ -99,15 +99,15 @@
     Tags = [
         "AWS",
         "Configuration Required",
         "Security Control",
         "Collection:Data From Cloud Storage Object",
     ]
     Reports = {"MITRE ATT&CK": ["TA0009:T1530"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Checks if HTTP (unencrypted) was used to access objects in an S3 bucket, as opposed to HTTPS (encrypted).\n"
     Runbook = "Add a condition on the S3 bucket policy that denies access via http.\n"
     Reference = (
         "https://aws.amazon.com/premiumsupport/knowledge-center/s3-bucket-policy-for-config-rule/"
     )
     SummaryAttributes = [
         "bucket",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py` & `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awss3_server_access_unauthenticated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Authenticated Access",
         ExpectedResult=False,
@@ -27,15 +27,15 @@
     Tags = [
         "AWS",
         "Configuration Required",
         "Security Control",
         "Collection:Data From Cloud Storage Object",
     ]
     Reports = {"MITRE ATT&CK": ["TA0009:T1530"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = (
         "Checks for S3 access attempts where the requester is not an authenticated AWS user.\n"
     )
     Runbook = "If unauthenticated S3 access is not expected for this bucket, update its access policies.\n"
     Reference = "https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-control-auth-workflow-bucket-operation.html"
     SummaryAttributes = ["bucket", "key", "requester"]
     Tests = awss3_server_access_unauthenticated_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py` & `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fnmatch import fnmatch
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awss3_server_access_unknown_requester_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Expected Access",
         ExpectedResult=False,
@@ -119,15 +119,15 @@
     Tags = [
         "AWS",
         "Configuration Required",
         "Security Control",
         "Collection:Data From Cloud Storage Object",
     ]
     Reports = {"Panther": ["Data Access"], "MITRE ATT&CK": ["TA0009:T1530"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Validates that proper IAM entities are accessing sensitive data buckets."
     Runbook = "If the S3 access is not expected for this bucket, investigate the requester's other traffic."
     Reference = "https://docs.aws.amazon.com/AmazonS3/latest/userguide/walkthrough1.html"
     SummaryAttributes = [
         "bucket",
         "key",
         "operation",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py` & `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_iocs import CRYPTO_MINING_DOMAINS
 from pypanther.log_types import LogType
 
 awsdns_crypto_domain_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Non Crypto Query",
         ExpectedResult=False,
@@ -169,15 +169,15 @@
 
 
 class AWSDNSCryptoDomain(PantherRule):
     Description = "Identifies clients that may be performing DNS lookups associated with common currency mining pools."
     DisplayName = "AWS DNS Crypto Domain"
     Reports = {"MITRE ATT&CK": ["TA0040:T1496"]}
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.AWS_VPCDns]
     RuleID = "AWS.DNS.Crypto.Domain-prototype"
     Tests = awsdns_crypto_domain_tests
 
     def rule(self, event):
         query_name = event.get("query_name")
         for domain in CRYPTO_MINING_DOMAINS:
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py` & `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsvpc_healthy_log_status_tests: List[PantherRuleTest] = [
     PantherRuleTest(Name="Healthy Log Status", ExpectedResult=False, Log={"log-status": "OK"}),
     PantherRuleTest(
         Name="Unhealthy Log Status", ExpectedResult=True, Log={"log-status": "SKIPDATA"}
@@ -13,15 +13,15 @@
 
 
 class AWSVPCHealthyLogStatus(PantherRule):
     RuleID = "AWS.VPC.HealthyLogStatus-prototype"
     DisplayName = "AWS VPC Healthy Log Status"
     LogTypes = [LogType.AWS_VPCFlow]
     Tags = ["AWS", "Security Control"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Checks for the log status `SKIP-DATA`, which indicates that data was lost either to an internal server error or due to capacity constraints.\n"
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html#flow-log-records"
     Runbook = "Determine if the cause of the issue is capacity constraints, and consider adjusting VPC Flow Log configurations accordingly.\n"
     Tests = awsvpc_healthy_log_status_tests
 
     def rule(self, event):
         return event.get("log-status") == "SKIPDATA"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py` & `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ipaddress import ip_network
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsvpc_inbound_port_whitelist_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Public to Private IP on Restricted Port",
         ExpectedResult=True,
@@ -33,15 +33,15 @@
         "AWS",
         "Configuration Required",
         "Security Control",
         "Command and Control:Non-Standard Port",
     ]
     Reports = {"MITRE ATT&CK": ["TA0011:T1571"]}
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "VPC Flow Logs observed inbound traffic violating the port allowlist.\n"
     Runbook = "Block the unapproved traffic, or update the approved ports list.\n"
     SummaryAttributes = ["srcaddr", "dstaddr", "dstport"]
     Tests = awsvpc_inbound_port_whitelist_tests
     APPROVED_PORTS = {80, 443}
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py` & `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ipaddress import ip_network
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsvpc_inbound_port_blacklist_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Public to Private IP on Restricted Port",
         ExpectedResult=True,
@@ -33,15 +33,15 @@
         "AWS",
         "Configuration Required",
         "Security Control",
         "Command and Control:Non-Standard Port",
     ]
     Reports = {"MITRE ATT&CK": ["TA0011:T1571"]}
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "VPC Flow Logs observed inbound traffic violating the port blocklist.\n"
     Runbook = "Block the unapproved traffic, or update the unapproved ports list.\n"
     SummaryAttributes = ["srcaddr", "dstaddr", "dstport"]
     Tests = awsvpc_inbound_port_blacklist_tests
     CONTROLLED_PORTS = {22, 3389}
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py` & `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ipaddress import ip_network
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import aws_rule_context
 from pypanther.log_types import LogType
 
 awsvpc_unapproved_outbound_dns_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Approved Outbound DNS Traffic",
         ExpectedResult=False,
@@ -33,15 +33,15 @@
         "AWS",
         "Configuration Required",
         "Security Control",
         "Command and Control:Application Layer Protocol",
     ]
     Reports = {"MITRE ATT&CK": ["TA0011:T1071"]}
     Reference = "https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Alerts if outbound DNS traffic is detected to a non-approved DNS server. DNS is often used as a means to exfiltrate data or perform command and control for compromised hosts. All DNS traffic should be routed through internal DNS servers or trusted 3rd parties.\n"
     Runbook = "Investigate the host sending unapproved DNS activity for signs of compromise or other malicious activity. Update network configurations appropriately to ensure all DNS traffic is routed to approved DNS servers.\n"
     SummaryAttributes = ["srcaddr", "dstaddr", "dstport"]
     Tests = awsvpc_unapproved_outbound_dns_tests  # CloudFlare DNS
     # Google DNS
     # '10.0.0.1', # Internal DNS
     APPROVED_DNS_SERVERS = {"1.1.1.1", "8.8.8.8"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_failed_signins.py` & `pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_failed_signins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_azuresignin_helpers import (
     actor_user,
     azure_signin_alert_context,
     is_sign_in_event,
 )
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
@@ -142,15 +142,15 @@
 
 class AzureAuditManyFailedSignIns(PantherRule):
     RuleID = "Azure.Audit.ManyFailedSignIns-prototype"
     DisplayName = "Azure Many Failed SignIns"
     Threshold = 10
     DedupPeriodMinutes = 10
     LogTypes = [LogType.Azure_Audit]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "This detection looks for a number of failed sign-ins for the same ServicePrincipalName or UserPrincipalName\n"
     Reports = {"MITRE ATT&CK": ["TA0006:T1110", "TA0001:T1078"]}
     Runbook = "Querying Sign-In logs for the ServicePrincipalName or UserPrincipalName may indicate that the principal is under attack, or that a sign-in credential rolled and some  user of the credential didn't get updated.\n"
     Reference = (
         "https://learn.microsoft.com/en-us/entra/identity/authentication/overview-authentication"
     )
     SummaryAttributes = [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_legacyauth.py` & `pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_legacyauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import List
 from unittest.mock import MagicMock
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_azuresignin_helpers import (
     actor_user,
     azure_signin_alert_context,
     is_sign_in_event,
 )
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
@@ -281,15 +281,15 @@
 
 
 class AzureAuditLegacyAuth(PantherRule):
     RuleID = "Azure.Audit.LegacyAuth-prototype"
     DisplayName = "Azure SignIn via Legacy Authentication Protocol"
     DedupPeriodMinutes = 10
     LogTypes = [LogType.Azure_Audit]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "This detection looks for Successful Logins that have used legacy authentication protocols\n"
     Reference = "https://learn.microsoft.com/en-us/azure/active-directory/reports-monitoring/workbook-legacy-authentication"
     Runbook = "Based on Microsoft's analysis more than 97 percent of credential stuffing attacks use legacy authentication and more than 99 percent of password spray attacks use legacy authentication protocols. These attacks would stop with basic authentication disabled or blocked. see https://learn.microsoft.com/en-us/azure/active-directory/conditional-access/block-legacy-authentication\nIf you are aware of this Legacy Auth need, and need to continue using this mechanism, add the principal name to KNOWN_EXCEPTIONS. The Reference link contains additional material hosted on Microsoft.com\n"
     SummaryAttributes = [
         "properties:ServicePrincipalName",
         "properties:UserPrincipalName",
         "properties:ipAddress",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py` & `pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_azuresignin_helpers import (
     actor_user,
     azure_signin_alert_context,
     is_sign_in_event,
 )
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
@@ -323,15 +323,15 @@
 
 
 class AzureAuditRiskLevelPassthrough(PantherRule):
     RuleID = "Azure.Audit.RiskLevelPassthrough-prototype"
     DisplayName = "Azure RiskLevel Passthrough"
     DedupPeriodMinutes = 10
     LogTypes = [LogType.Azure_Audit]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "This detection surfaces an alert based on  riskLevelAggregated, riskLevelDuringSignIn, and riskState.\nriskLevelAggregated and riskLevelDuringSignIn are only  expected for Azure AD Premium P2 customers.\n"
     Reference = "https://learn.microsoft.com/en-us/azure/active-directory/identity-protection/howto-identity-protection-risk-feedback"
     Reports = {"MITRE ATT&CK": ["TA0006:T1110", "TA0001:T1078"]}
     Runbook = "There are a variety of potential responses to these sign-in risks.  MSFT has provided an in-depth reference material at https://learn.microsoft.com/en-us/azure/active-directory/identity-protection/howto-identity-protection-risk-feedback\n"
     SummaryAttributes = [
         "properties:ServicePrincipalName",
         "properties:UserPrincipalName",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_access_granted.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_access_granted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 box_access_granted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -45,15 +45,15 @@
 
 
 class BoxAccessGranted(PantherRule):
     RuleID = "Box.Access.Granted-prototype"
     DisplayName = "Box Access Granted"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A user granted access to their box account to Box technical support from account settings.\n"
     Reference = "https://support.box.com/hc/en-us/articles/7039943421715-Enabling-and-Disabling-Access-for-Box-Support"
     Runbook = "Investigate whether the user purposefully granted access to their account.\n"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = box_access_granted_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_anomalous_download.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_anomalous_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import box_parse_additional_details, deep_get
 from pypanther.log_types import LogType
 
 box_shield_anomalous_download_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -41,15 +41,15 @@
 
 class BoxShieldAnomalousDownload(PantherRule):
     RuleID = "Box.Shield.Anomalous.Download-prototype"
     DisplayName = "Box Shield Detected Anomalous Download Activity"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Exfiltration:Exfiltration Over Web Service"]
     Reports = {"MITRE ATT&CK": ["TA0010:T1567"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A user's download activity has altered significantly.\n"
     Reference = "https://developer.box.com/guides/events/shield-alert-events/"
     Runbook = "Investigate whether this was triggered by expected user download activity.\n"
     SummaryAttributes = ["event_type", "ip_address"]
     Tests = box_shield_anomalous_download_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_event_triggered_externally.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_event_triggered_externally.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_config import config
 from pypanther.log_types import LogType
 
 box_event_triggered_externally_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
@@ -42,15 +42,15 @@
 class BoxEventTriggeredExternally(PantherRule):
     RuleID = "Box.Event.Triggered.Externally-prototype"
     DisplayName = "Box event triggered by unknown or external user"
     Enabled = False
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Exfiltration:Exfiltration Over Web Service", "Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0010:T1567"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An external user has triggered a box enterprise event.\n"
     Reference = (
         "https://support.box.com/hc/en-us/articles/8391393127955-Using-the-Enterprise-Event-Stream"
     )
     Runbook = "Investigate whether this user's activity is expected.\n"
     SummaryAttributes = ["ip_address"]
     Threshold = 10
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_item_shared_externally.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_item_shared_externally.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_box_helpers import (
     is_box_sdk_enabled,
     lookup_box_file,
     lookup_box_folder,
 )
 from pypanther.log_types import LogType
@@ -48,15 +48,15 @@
 class BoxItemSharedExternally(PantherRule):
     RuleID = "Box.Item.Shared.Externally-prototype"
     DisplayName = "Box item shared externally"
     Enabled = False
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Exfiltration:Exfiltration Over Web Service", "Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0010:T1567"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A user has shared an item and it is accessible to anyone with the share link (internal or external to the company). This rule requires that the boxsdk[jwt] be installed in the environment.\n"
     Reference = "https://support.box.com/hc/en-us/articles/4404822772755-Enterprise-Settings-Content-Sharing-Tab"
     Runbook = "Investigate whether this user's activity is expected.\n"
     SummaryAttributes = ["ip_address"]
     Threshold = 10
     Tests = box_item_shared_externally_tests
     ALLOWED_SHARED_ACCESS = {"collaborators", "company"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_malicious_content.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_malicious_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import box_parse_additional_details, deep_get
 from pypanther.log_types import LogType
 
 box_malicious_content_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -74,15 +74,15 @@
 
 class BoxMaliciousContent(PantherRule):
     RuleID = "Box.Malicious.Content-prototype"
     DisplayName = "Malicious Content Detected"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Execution:User Execution"]
     Reports = {"MITRE ATT&CK": ["TA0002:T1204"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Box has detect malicious content, such as a virus.\n"
     Reference = "https://developer.box.com/guides/events/shield-alert-events/\n"
     Runbook = "Investigate whether this is a false positive or if the virus needs to be contained appropriately.\n"
     SummaryAttributes = ["event_type"]
     Tests = box_malicious_content_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_new_login.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_new_login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 box_new_login_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -41,15 +41,15 @@
 
 class BoxNewLogin(PantherRule):
     RuleID = "Box.New.Login-prototype"
     DisplayName = "Box New Login"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Initial Access:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1078"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A user logged in from a new device.\n"
     Reference = "https://support.box.com/hc/en-us/articles/360043691914-Controlling-Devices-Used-to-Access-Box"
     Runbook = "Investigate whether this is a valid user login.\n"
     SummaryAttributes = ["ip_address"]
     Tests = box_new_login_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_policy_violation.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_policy_violation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 box_content_workflow_policy_violation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -56,15 +56,15 @@
 
 
 class BoxContentWorkflowPolicyViolation(PantherRule):
     RuleID = "Box.Content.Workflow.Policy.Violation-prototype"
     DisplayName = "Box Content Workflow Policy Violation"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A user violated the content workflow policy.\n"
     Reference = "https://support.box.com/hc/en-us/articles/360043692594-Creating-a-Security-Policy"
     Runbook = "Investigate whether the user continues to violate the policy and take measure to ensure they understand policy.\n"
     SummaryAttributes = ["event_type"]
     Tests = box_content_workflow_policy_violation_tests
     POLICY_VIOLATIONS = {
         "CONTENT_WORKFLOW_UPLOAD_POLICY_VIOLATION",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_suspicious_login_or_session.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_suspicious_login_or_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import box_parse_additional_details, deep_get
 from pypanther.log_types import LogType
 
 box_shield_suspicious_alert_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -73,15 +73,15 @@
 
 class BoxShieldSuspiciousAlert(PantherRule):
     RuleID = "Box.Shield.Suspicious.Alert-prototype"
     DisplayName = "Box Shield Suspicious Alert Triggered"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Initial Access:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1078"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "A user login event or session event was tagged as medium to high severity by Box Shield.\n"
     )
     Reference = "https://developer.box.com/guides/events/shield-alert-events/"
     Runbook = "Investigate whether this was triggered by an expected user event.\n"
     SummaryAttributes = ["event_type", "ip_address"]
     Tests = box_shield_suspicious_alert_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_untrusted_device.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_untrusted_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 box_untrusted_device_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -41,15 +41,15 @@
 
 class BoxUntrustedDevice(PantherRule):
     RuleID = "Box.Untrusted.Device-prototype"
     DisplayName = "Box Untrusted Device Login"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Initial Access:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1078"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A user attempted to login from an untrusted device.\n"
     Reference = "https://support.box.com/hc/en-us/articles/360044194993-Setting-Up-Device-Trust-Security-Requirements"
     Runbook = "Investigate whether this is a valid user attempting to login to box.\n"
     SummaryAttributes = ["ip_address"]
     Tests = box_untrusted_device_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_user_downloads.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_user_downloads.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 box_large_number_downloads_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -46,15 +46,15 @@
 
 class BoxLargeNumberDownloads(PantherRule):
     RuleID = "Box.Large.Number.Downloads-prototype"
     DisplayName = "Box Large Number of Downloads"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Exfiltration:Exfiltration Over Web Service"]
     Reports = {"MITRE ATT&CK": ["TA0010:T1567"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = (
         "A user has exceeded the threshold for number of downloads within a single time frame.\n"
     )
     Reference = (
         "https://support.box.com/hc/en-us/articles/360043697134-Download-Files-and-Folders-from-Box"
     )
     Runbook = "Investigate whether this user's download activity is expected.  Investigate the cause of this download activity.\n"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/box_rules/box_user_permission_updates.py` & `pypanther-0.1.1a8/pypanther/rules/box_rules/box_user_permission_updates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 box_large_number_permission_updates_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Regular Event",
         ExpectedResult=False,
@@ -67,15 +67,15 @@
 
 class BoxLargeNumberPermissionUpdates(PantherRule):
     RuleID = "Box.Large.Number.Permission.Updates-prototype"
     DisplayName = "Box Large Number of Permission Changes"
     LogTypes = [LogType.Box_Event]
     Tags = ["Box", "Privilege Escalation:Abuse Elevation Control Mechanism"]
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A user has exceeded the threshold for number of folder permission changes within a single time frame.\n"
     Reference = (
         "https://support.box.com/hc/en-us/articles/360043697254-Understanding-Folder-Permissions"
     )
     Runbook = "Investigate whether this user's activity is expected.\n"
     SummaryAttributes = ["ip_address"]
     Threshold = 100
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py` & `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 carbon_black_audit_admin_grant_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Super Admin granted",
         ExpectedResult=True,
         Log={
@@ -53,15 +53,15 @@
 
 
 class CarbonBlackAuditAdminGrant(PantherRule):
     RuleID = "CarbonBlack.Audit.Admin.Grant-prototype"
     LogTypes = [LogType.CarbonBlack_Audit]
     Description = "Detects when a user is granted Admin or Super Admin permissions."
     DisplayName = "Carbon Black Admin Role Granted"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["Privilege Escalation", "Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0004:T1098"]}
     Reference = "https://docs.vmware.com/en/VMware-Carbon-Black-Cloud/services/carbon-black-cloud-user-guide/GUID-CF5ACD2C-A534-46C8-AE06-E1884DB37B58.html"
     Tests = carbon_black_audit_admin_grant_tests
     PREFIXES = ("Updated grant: ", "Created grant: ")
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py` & `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 carbon_black_audit_api_key_created_retrieved_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="API Key Retrieved",
         ExpectedResult=True,
         Log={
@@ -51,15 +51,15 @@
 
 
 class CarbonBlackAuditAPIKeyCreatedRetrieved(PantherRule):
     RuleID = "CarbonBlack.Audit.API.Key.Created.Retrieved-prototype"
     LogTypes = [LogType.CarbonBlack_Audit]
     Description = "Detects when a user creates a new API key or retrieves an existing key."
     DisplayName = "Carbon Black API Key Created or Retrieved"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Tags = ["Persistence", "Create Account"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1136"]}
     Reference = "https://docs.vmware.com/en/VMware-Carbon-Black-Cloud/services/carbon-black-cloud-user-guide/GUID-F3816FB5-969F-4113-80FC-03981C65F969.html"
     Tests = carbon_black_audit_api_key_created_retrieved_tests
     PATTERNS = (
         " retrieved secret for API ID ",
         "Added API ID ",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py` & `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 carbon_black_audit_data_forwarder_stopped_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Endpoint event forwarder disabled",
         ExpectedResult=True,
         Log={
@@ -38,15 +38,15 @@
 
 
 class CarbonBlackAuditDataForwarderStopped(PantherRule):
     RuleID = "CarbonBlack.Audit.Data.Forwarder.Stopped-prototype"
     LogTypes = [LogType.CarbonBlack_Audit]
     Description = "Detects when a user disables or deletes a Data Forwarder."
     DisplayName = "Carbon Black Data Forwarder Stopped"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["Defense Evasion", "Impair Defenses", "Disable or Modify Cloud Logs"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562.008"]}
     Reference = "https://docs.vmware.com/en/VMware-Carbon-Black-Cloud/services/carbon-black-cloud-user-guide/GUID-E8D33F72-BABB-4157-A908-D8BBDB5AF349.html"
     Tests = carbon_black_audit_data_forwarder_stopped_tests
     ACTION = ""
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_flagged.py` & `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_flagged.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 carbon_black_audit_flagged_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Flagged",
         ExpectedResult=True,
         Log={
@@ -37,15 +37,15 @@
 
 
 class CarbonBlackAuditFlagged(PantherRule):
     RuleID = "CarbonBlack.Audit.Flagged-prototype"
     LogTypes = [LogType.CarbonBlack_Audit]
     Description = "Detects when Carbon Black has flagged a log as important, such as failed login attempts and locked accounts."
     DisplayName = "Carbon Black Log Entry Flagged"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["Credential Access", "Brute Force"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
     Reference = "https://docs.vmware.com/en/VMware-Carbon-Black-Cloud/services/carbon-black-cloud-user-guide/GUID-FB61E4E3-6431-4226-A4E3-5949FB75922B.html"
     Tests = carbon_black_audit_flagged_tests
 
     def rule(self, event):
         return event.get("flagged", False)
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py` & `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 carbon_black_audit_user_added_outside_org_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Outside org",
         ExpectedResult=True,
         Log={
@@ -36,15 +36,15 @@
 
 
 class CarbonBlackAuditUserAddedOutsideOrg(PantherRule):
     RuleID = "CarbonBlack.Audit.User.Added.Outside.Org-prototype"
     LogTypes = [LogType.CarbonBlack_Audit]
     Description = "Detects when a user from a different organization is added to Carbon Black."
     DisplayName = "Carbon Black User Added Outside Org"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["Persistence", "Create Account"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1136"]}
     Reference = "https://docs.vmware.com/en/VMware-Carbon-Black-Cloud/services/carbon-black-cloud-user-guide/GUID-516BAF8C-A13D-4FC7-AA92-923159C13083.html"
     Tests = carbon_black_audit_user_added_outside_org_tests
     PATTERNS = ("Added user ",)
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_passthrough.py` & `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_passthrough.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 carbon_black_alert_v2_passthrough_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="True Positive",
         ExpectedResult=True,
         Log={
@@ -182,15 +182,15 @@
 class CarbonBlackAlertV2Passthrough(PantherRule):
     RuleID = "CarbonBlack.AlertV2.Passthrough-prototype"
     Description = "This rule enriches and contextualizes security alerts generated by Carbon Black.  The alert title and description are dynamically updated based on data included in the alert log."
     DisplayName = "Carbon Black Passthrough Rule"
     Runbook = "Review the Carbon Black alert details to determine what malicious behavior was detected, and whether or not it was blocked.  Use the Reference link to view the alert in the Carbon Black console and take remediating actions if necessary."
     Reference = "https://docs.vmware.com/en/VMware-Carbon-Black-Cloud/services/carbon-black-cloud-user-guide/GUID-0B68199D-6411-45D1-AE0D-2AB9B7A28513.html"
     LogTypes = [LogType.CarbonBlack_AlertV2]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     DedupPeriodMinutes = 30
     SummaryAttributes = [
         "attack_tactic",
         "blocked_name",
         "device_name",
         "device_username",
         "primary_event_id",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py` & `pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 cisco_umbrella_dns_blocked_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Domain Blocked",
         ExpectedResult=True,
         Log={
@@ -33,15 +33,15 @@
 
 class CiscoUmbrellaDNSBlocked(PantherRule):
     RuleID = "CiscoUmbrella.DNS.Blocked-prototype"
     DisplayName = "Cisco Umbrella Domain Blocked"
     DedupPeriodMinutes = 480
     LogTypes = [LogType.CiscoUmbrella_DNS]
     Tags = ["DNS"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Monitor blocked domains"
     Runbook = "Inspect the blocked domain and lookup for malware"
     Reference = "https://support.umbrella.com/hc/en-us/articles/230563627-How-to-determine-if-a-domain-or-resource-is-being-blocked-using-Chrome-Net-Internals"
     SummaryAttributes = ["action", "internalIp", "externalIp", "domain", "responseCode"]
     Tests = cisco_umbrella_dns_blocked_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py` & `pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from difflib import SequenceMatcher
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 
 class CiscoUmbrellaDNSFuzzyMatching(PantherRule):
     RuleID = "CiscoUmbrella.DNS.FuzzyMatching-prototype"
     DisplayName = "Cisco Umbrella Domain Name Fuzzy Matching"
     Enabled = False
     DedupPeriodMinutes = 15
     LogTypes = [LogType.CiscoUmbrella_DNS]
     Tags = ["Configuration Required", "DNS"]
     Reference = "https://umbrella.cisco.com/blog/abcs-of-dns"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Identify lookups to suspicious domains that could indicate a phishing attack."
     Runbook = "Validate if your organization owns the domain, otherwise investigate the host that made the domain resolution.\n"
     DOMAIN = ""  # The domain to monitor for phishing, for example "google.com"
     # List all of your known-good domains here
     ALLOW_SET = {}
     SIMILARITY_RATIO = 0.7
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py` & `pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 cisco_umbrella_dns_suspicious_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Suspicious Domain",
         ExpectedResult=True,
         Log={
@@ -35,15 +35,15 @@
     RuleID = "CiscoUmbrella.DNS.Suspicious-prototype"
     DisplayName = "Cisco Umbrella Suspicious Domains"
     Enabled = False
     DedupPeriodMinutes = 480
     LogTypes = [LogType.CiscoUmbrella_DNS]
     Tags = ["DNS", "Configuration Required"]
     Reference = "https://umbrella.cisco.com/blog/abcs-of-dns"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Monitor suspicious or known malicious domains"
     Runbook = "Inspect the domain and check the host for other indicators of compromise"
     SummaryAttributes = ["action", "internalIp", "externalIp", "domain", "responseCode"]
     Tests = cisco_umbrella_dns_suspicious_tests
     DOMAINS_TO_MONITOR = {"photoscape.ch"}  # Sample malware domain
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py` & `pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_cloudflare_helpers import cloudflare_fw_alert_context
 from pypanther.log_types import LogType
 
 cloudflare_firewall_l7_d_do_s_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Traffic Marked as L7DDoS",
         ExpectedResult=True,
@@ -96,15 +96,15 @@
 
 
 class CloudflareFirewallL7DDoS(PantherRule):
     RuleID = "Cloudflare.Firewall.L7DDoS-prototype"
     DisplayName = "Cloudflare L7 DDoS"
     LogTypes = [LogType.Cloudflare_Firewall]
     Tags = ["Cloudflare", "Variable Severity"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Layer 7 Distributed Denial of Service (DDoS) detected"
     Runbook = "Inspect and monitor internet-facing services for potential outages"
     Reference = "https://www.cloudflare.com/en-gb/learning/ddos/application-layer-ddos-attack/"
     Threshold = 100
     SummaryAttributes = ["Action", "ClientCountry", "ClientIP", "ClientRequestUserAgent"]
     Tests = cloudflare_firewall_l7_d_do_s_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py` & `pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_cloudflare_helpers import cloudflare_http_alert_context
 from pypanther.log_types import LogType
 
 cloudflare_http_request_bot_high_volume_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Likely Human",
         ExpectedResult=False,
@@ -150,15 +150,15 @@
 
 class CloudflareHttpRequestBotHighVolume(PantherRule):
     RuleID = "Cloudflare.HttpRequest.BotHighVolume-prototype"
     DisplayName = "Cloudflare Bot High Volume"
     Enabled = False
     LogTypes = [LogType.Cloudflare_HttpRequest]
     Tags = ["Cloudflare"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Monitors for bots making HTTP Requests at a rate higher than 2req/sec"
     Runbook = "Inspect and monitor internet-facing services for potential outages"
     Reference = "https://developers.cloudflare.com/waf/rate-limiting-rules/request-rate/"
     Threshold = 7560
     SummaryAttributes = [
         "ClientIP",
         "ClientRequestUserAgent",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_process_alert_context, is_base64
 from pypanther.log_types import LogType
 
 crowdstrike_base64_encoded_args_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Command Line Tool Execution with Base64 Argument (Positive)",
         ExpectedResult=True,
@@ -556,15 +556,15 @@
 
 
 class CrowdstrikeBase64EncodedArgs(PantherRule):
     RuleID = "Crowdstrike.Base64EncodedArgs-prototype"
     DisplayName = "Execution of Command Line Tool with Base64 Encoded Arguments"
     LogTypes = [LogType.Crowdstrike_FDREvent]
     Tags = ["Execution", "Obfuscation"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects the execution of common command line tools (e.g., PowerShell, cmd.exe) with Base64 encoded arguments, which could indicate an attempt to obfuscate malicious commands."
     Runbook = "Investigate the endpoint for signs of command line tool execution with Base64 encoded arguments. Review the executed command, decode the Base64 string, and analyze the original content."
     Reference = "https://www.crowdstrike.com/blog/blocking-fileless-script-based-attacks-using-falcon-script-control-feature/"
     Tests = crowdstrike_base64_encoded_args_tests
     DECODED = ""
     # List of command line tools to monitor for execution with Base64 encoded arguments
     COMMAND_LINE_TOOLS = {"powershell.exe", "cmd.exe", "cscript.exe", "wscript.exe", "rundll32.exe"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import (
     crowdstrike_network_detection_alert_context,
     deep_get,
 )
 from pypanther.log_types import LogType
 
 connectionto_embargoed_country_tests: List[PantherRuleTest] = [
@@ -157,15 +157,15 @@
 
 class ConnectiontoEmbargoedCountry(PantherRule):
     Description = "Detection to alert when internal asset is communicating with an sanctioned destination. This detection leverages Panther UDM and IPInfo enrichment."
     Reference = "U.S. Sanctioned Destinations - https://www.bis.doc.gov/index.php/policy-guidance/country-guidance/sanctioned-destinations"
     DisplayName = "Connection to Embargoed Country"
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Connection.to.Embargoed.Country-prototype"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Tests = connectionto_embargoed_country_tests
     # U.S. Gov Sanctioned Destinations
     # Cuba
     # Iran
     # DPRK
     # Syria
     EMBARGO_COUNTRY_CODES = {"CU", "IR", "KP", "SY"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_detection_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_credential_dumping_tool_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="mimikatz",
         ExpectedResult=True,
@@ -172,15 +172,15 @@
 ]
 
 
 class CrowdstrikeCredentialDumpingTool(PantherRule):
     Description = "Detects usage of tools commonly used for credential dumping."
     DisplayName = "Crowdstrike Credential Dumping Tool"
     Reference = "https://www.crowdstrike.com/blog/adversary-credential-theft/"
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Crowdstrike.Credential.Dumping.Tool-prototype"
     Tests = crowdstrike_credential_dumping_tool_tests
     CREDENTIAL_DUMPING_TOOLS = {
         "mimikatz.exe",
         "secretsdump.py",
         "pwdump.exe",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_detection_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_cryptomining_tools_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Crypto tool",
         ExpectedResult=True,
@@ -172,15 +172,15 @@
 ]
 
 
 class CrowdstrikeCryptominingTools(PantherRule):
     Description = "Detects the execution of known crytocurrency mining tools."
     DisplayName = "Crowdstrike Cryptomining Tools "
     Reference = "https://www.crowdstrike.com/cybersecurity-101/cryptojacking/"
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Crowdstrike.Cryptomining.Tools-prototype"
     Tests = crowdstrike_cryptomining_tools_tests
     CRYPTOCURRENCY_MINING_TOOLS = {
         "xmrig.exe",
         "cgminer.exe",
         "bfgminer.exe",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import (
     crowdstrike_detection_alert_context,
     get_crowdstrike_field,
 )
 from pypanther.log_types import LogType
 
 crowdstrike_detectionpassthrough_tests: List[PantherRuleTest] = [
@@ -172,15 +172,15 @@
     ),
 ]
 
 
 class CrowdstrikeDetectionpassthrough(PantherRule):
     RuleID = "Crowdstrike.Detection.passthrough-prototype"
     DisplayName = "Crowdstrike Detection Passthrough"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Crowdstrike_DetectionSummary, LogType.Crowdstrike_FDREvent]
     Tags = ["Crowdstrike"]
     Description = "Crowdstrike Falcon has detected malicious activity on a host."
     Runbook = "Follow the Falcon console link and follow the IR process as needed."
     Reference = "https://www.crowdstrike.com/blog/tech-center/hunt-threat-activity-falcon-endpoint-protection/"
     DedupPeriodMinutes = 0
     SummaryAttributes = ["p_any_ip_addresses"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import (
     filter_crowdstrike_fdr_event_type,
     get_crowdstrike_field,
 )
 from pypanther.log_types import LogType
 
 crowdstrike_dns_request_tests: List[PantherRuleTest] = [
@@ -245,15 +245,15 @@
 
 class CrowdstrikeDNSRequest(PantherRule):
     RuleID = "Crowdstrike.DNS.Request-prototype"
     DisplayName = "DNS request to denylisted domain"
     Enabled = False
     LogTypes = [LogType.Crowdstrike_DNSRequest, LogType.Crowdstrike_FDREvent]
     Tags = ["Crowdstrike", "Initial Access:Phishing", "Configuration Required"]
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Reports = {"MITRE ATT&CK": ["TA0001:T1566"]}
     Description = "A DNS request was made to a domain on an explicit denylist"
     Reference = "https://docs.runpanther.io/data-onboarding/supported-logs/crowdstrike#crowdstrike-dnsrequest"
     Runbook = "Filter for host ID in title in Crowdstrike Host Management console to identify the system that queried the domain."
     DedupPeriodMinutes = 15
     SummaryAttributes = ["DomainName", "aid", "p_any_domain_names", "p_any_ip_addresses"]
     Tests = crowdstrike_dns_request_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_process_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_fdrlolbas_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="At Usage (Positive)",
         ExpectedResult=True,
@@ -174,15 +174,15 @@
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Crowdstrike.FDR.LOLBAS-prototype"
     DisplayName = "Crowdstrike FDR LOLBAS"
     Description = "Living off the land binaries and script usage"
     Reference = "https://lolbas-project.github.io/"
     DedupPeriodMinutes = 1440
     Enabled = False
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Tags = ["Configuration Required"]
     Tests = crowdstrike_fdrlolbas_tests
     LOLBAS_EXE = {
         "AppInstaller.exe",
         "At.exe",
         "Atbroker.exe",
         "Bash.exe",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_process_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_macos_add_trusted_cert_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Added root cert",
         ExpectedResult=True,
@@ -389,15 +389,15 @@
 
 
 class CrowdstrikeMacosAddTrustedCert(PantherRule):
     DisplayName = "CrowdStrike MacOS Added Trusted Cert"
     Description = "Detects attempt to install a root certificate on MacOS"
     RuleID = "Crowdstrike.Macos.Add.Trusted.Cert-prototype"
     Reference = "https://docs.panther.com/data-onboarding/supported-logs/crowdstrike#crowdstrike.processrollup2"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Crowdstrike_FDREvent]
     Tests = crowdstrike_macos_add_trusted_cert_tests
 
     def rule(self, event):
         event_platform = deep_get(event, "event_platform", default="<UNKNOWN_PLATFORM>")
         fdr_event_type = deep_get(event, "fdr_event_type", default="<UNKNOWN_FDR_EVENT_TYPE>")
         image_filename = deep_get(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_process_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_macos_osascript_administrator_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Ran Osascript with administrator privileges",
         ExpectedResult=True,
@@ -391,15 +391,15 @@
 class CrowdstrikeMacosOsascriptAdministrator(PantherRule):
     DisplayName = "CrowdStrike MacOS Osascript as Administrator"
     Description = "Detects usage of osascript with administrator privileges"
     RuleID = "Crowdstrike.Macos.Osascript.Administrator-prototype"
     Reference = (
         "https://www.sentinelone.com/blog/how-offensive-actors-use-applescript-for-attacking-macos/"
     )
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Crowdstrike_FDREvent]
     Tests = crowdstrike_macos_osascript_administrator_tests
 
     def rule(self, event):
         event_platform = deep_get(event, "event_platform", default="<UNKNOWN_PLATFORM>")
         event_simplename = deep_get(event, "event_simplename", default="<UNKNOWN_EVENT_SIMPLENAME>")
         image_filename = deep_get(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_process_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_macos_plutil_usage_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Plutil used",
         ExpectedResult=True,
@@ -313,15 +313,15 @@
 
 
 class CrowdstrikeMacosPlutilUsage(PantherRule):
     DisplayName = "CrowdStrike MacOS plutil Usage"
     Description = "Detects the usage of plutil to modify plist files. Plist files run on start up and are often used by attackers to maintain persistence."
     RuleID = "Crowdstrike.Macos.Plutil.Usage-prototype"
     Reference = "https://www.crowdstrike.com/blog/reconstructing-command-line-activity-on-macos/#:~:text=Terminal.savedState/.-,Windows.plist,-The%20file%20windows"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Crowdstrike_FDREvent]
     Tests = crowdstrike_macos_plutil_usage_tests
 
     def rule(self, event):
         command_line = deep_get(event, "event", "CommandLine", default="<UNKNOWN_COMMAND_LINE>")
         if (
             command_line
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import get_crowdstrike_field
 from pypanther.log_types import LogType
 
 crowdstrike_real_time_response_session_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="RTS session start event",
         ExpectedResult=True,
@@ -127,15 +127,15 @@
     ),
 ]
 
 
 class CrowdstrikeRealTimeResponseSession(PantherRule):
     DisplayName = "Crowdstrike Real Time Response (RTS) Session"
     RuleID = "Crowdstrike.RealTimeResponse.Session-prototype"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Crowdstrike_Unknown, LogType.Crowdstrike_FDREvent]
     Tags = ["Crowdstrike"]
     Description = "Alert when someone uses Crowdstrike’s RTR (real-time response) capability to access a machine remotely to run commands.\n"
     Runbook = "Validate the real-time response session started by the Actor.\n"
     Reference = "https://falcon.us-2.crowdstrike.com/documentation/71/real-time-response-and-network-containment#reviewing-real-time-response-audit-logs"
     Tests = crowdstrike_real_time_response_session_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_detection_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_remote_access_tool_execution_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Remote Access Tool",
         ExpectedResult=True,
@@ -172,15 +172,15 @@
 ]
 
 
 class CrowdstrikeRemoteAccessToolExecution(PantherRule):
     Description = "Detects usage of common remote access tools."
     DisplayName = "Crowdstrike Remote Access Tool Execution"
     Reference = "https://attack.mitre.org/techniques/T1219/"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Crowdstrike.Remote.Access.Tool.Execution-prototype"
     Tests = crowdstrike_remote_access_tool_execution_tests
     REMOTE_ACCESS_EXECUTABLES = {
         "teamviewer_service.exe",
         "winvnc.exe",
         "racwinvnc.exe",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_detection_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_reverse_shell_tool_executed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Malicious Netcat",
         ExpectedResult=True,
@@ -244,15 +244,15 @@
 
 class CrowdstrikeReverseShellToolExecuted(PantherRule):
     Description = (
         "Detects usage of tools commonly used to to establish reverse shells on Windows machines."
     )
     DisplayName = "Crowdstrike Reverse Shell Tool Executed"
     Reference = "https://attack.mitre.org/techniques/T1059/"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Crowdstrike.Reverse.Shell.Tool.Executed-prototype"
     Tests = crowdstrike_reverse_shell_tool_executed_tests
     #   process name: reverse shell signature
     REMOTE_SHELL_TOOLS = {
         "nc.exe": ["cmd.exe", "powershell.exe", "command.exe"],
         "ncat.exe": ["cmd.exe", "powershell.exe", "command.exe"],
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_detection_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_systemlog_tampering_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Clear Log Event",
         ExpectedResult=True,
@@ -172,15 +172,15 @@
 ]
 
 
 class CrowdstrikeSystemlogTampering(PantherRule):
     Description = "Detects when a user attempts to clear system logs. "
     DisplayName = "Crowdstrike Systemlog Tampering"
     Reference = "https://attack.mitre.org/techniques/T1070/001/"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Crowdstrike.Systemlog.Tampering-prototype"
     Tests = crowdstrike_systemlog_tampering_tests
     CLEARING_SYSTEM_LOG_TOOLS = {
         "wevtutil.exe": ["cl", "clear-log"],
         "powershell.exe": ["clear-eventlog"],
     }
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_detection_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_unusual_parent_child_processes_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Suspicious Event",
         ExpectedResult=True,
@@ -172,15 +172,15 @@
 ]
 
 
 class CrowdstrikeUnusualParentChildProcesses(PantherRule):
     Description = "Detects unusual parent child process pairings."
     DisplayName = "Crowdstrike Unusual Parent Child Processes"
     Reference = "https://medium.com/falconforce/falconfriday-e4554e9e6665"
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Crowdstrike.Unusual.Parent.Child.Processes-prototype"
     Tests = crowdstrike_unusual_parent_child_processes_tests
     SUSPICIOUS_PARENT_CHILD_COMBINATIONS_WINDOWS = {
         ("svchost.exe", "cmd.exe"),
         ("explorer.exe", "powershell.exe"),
         ("winword.exe", "cmd.exe"),
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py` & `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import crowdstrike_detection_alert_context, deep_get
 from pypanther.log_types import LogType
 
 crowdstrike_wmi_query_detection_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Benign wmic",
         ExpectedResult=False,
@@ -337,15 +337,15 @@
 
 
 class CrowdstrikeWMIQueryDetection(PantherRule):
     Description = "Detects execution of WMI queries involving information gathering or actions on remote systems, which could indicate reconnaissance or lateral movement."
     DisplayName = "Crowdstrike WMI Query Detection"
     Runbook = "Investigate the endpoint for signs of WMI query execution. Review the executed query and the associated user account."
     Reference = "https://learn.microsoft.com/en-us/windows/win32/wmisdk/querying-wmi"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Crowdstrike_FDREvent]
     RuleID = "Crowdstrike.WMI.Query.Detection-prototype"
     Tests = crowdstrike_wmi_query_detection_tests
     WMIC_SIGNATURES = [
         "get",
         "list",
         "process call create",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py` & `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 dropbox_adminsigninas_session_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other",
         ExpectedResult=False,
@@ -148,15 +148,15 @@
 ]
 
 
 class DropboxAdminsigninasSession(PantherRule):
     Description = "Alerts when an admin starts a sign-in-as session."
     DisplayName = "Dropbox Admin sign-in-as Session"
     Reference = "https://help.dropbox.com/security/sign-in-as-user"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Dropbox_TeamEvent]
     RuleID = "Dropbox.Admin.sign.in.as.Session-prototype"
     Tests = dropbox_adminsigninas_session_tests
 
     def rule(self, event):
         return deep_get(event, "event_type", "_tag", default="") == "sign_in_as_session_start"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_external_share.py` & `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_external_share.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import List
 from unittest.mock import MagicMock
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_config import config
 from pypanther.log_types import LogType
 
 dropbox_external_share_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Domain in Allowlist",
@@ -184,15 +184,15 @@
 ]
 
 
 class DropboxExternalShare(PantherRule):
     Description = "Dropbox item shared externally"
     DisplayName = "Dropbox External Share"
     Reference = "https://help.dropbox.com/share/share-outside-dropbox"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Dropbox_TeamEvent]
     RuleID = "Dropbox.External.Share-prototype"
     Tests = dropbox_external_share_tests
     DROPBOX_ALLOWED_SHARE_DOMAINS = config.DROPBOX_ALLOWED_SHARE_DOMAINS
 
     def rule(self, event):
         if isinstance(self.DROPBOX_ALLOWED_SHARE_DOMAINS, MagicMock):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py` & `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 dropbox_linked_team_application_added_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="App linked for team is LOW severity",
         ExpectedResult=True,
@@ -132,15 +132,15 @@
 
 
 class DropboxLinkedTeamApplicationAdded(PantherRule):
     Description = "An application was linked to your Dropbox Account"
     DisplayName = "Dropbox Linked Team Application Added"
     Reference = "https://help.dropbox.com/integrations/app-integrations"
     Runbook = "Ensure that the application is valid and not malicious. Verify that this is expected. If not, determine other actions taken by this user recently and reach out to the user. If the event involved a non-team member, consider disabling the user's access while investigating.\n"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Tags = ["dropbox"]
     LogTypes = [LogType.Dropbox_TeamEvent]
     RuleID = "Dropbox.Linked.Team.Application.Added-prototype"
     Tests = dropbox_linked_team_application_added_tests
 
     def rule(self, event):
         return all(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py` & `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import List
 from unittest.mock import MagicMock
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_config import config
 from pypanther.log_types import LogType
 
 dropbox_ownership_transfer_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Folder Ownership Transfer to External",
@@ -240,15 +240,15 @@
 ]
 
 
 class DropboxOwnershipTransfer(PantherRule):
     Description = "Dropbox ownership of a document or folder has been transferred."
     DisplayName = "Dropbox Document/Folder Ownership Transfer"
     Reference = "https://help.dropbox.com/share/owner"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Dropbox_TeamEvent]
     RuleID = "Dropbox.Ownership.Transfer-prototype"
     Tests = dropbox_ownership_transfer_tests
     DROPBOX_TRUSTED_OWNERSHIP_DOMAINS = config.DROPBOX_TRUSTED_OWNERSHIP_DOMAINS
 
     def rule(self, event):
         return "Transferred ownership " in deep_get(event, "event_type", "description", default="")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py` & `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 dropbox_user_disabled2_fa_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="2FA Disabled",
         ExpectedResult=True,
@@ -110,15 +110,15 @@
 ]
 
 
 class DropboxUserDisabled2FA(PantherRule):
     Description = "Dropbox user has disabled 2fa login"
     DisplayName = "Dropbox User Disabled 2FA"
     Reference = "https://help.dropbox.com/account-access/enable-two-step-verification"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Dropbox_TeamEvent]
     RuleID = "Dropbox.User.Disabled.2FA-prototype"
     Tests = dropbox_user_disabled2_fa_tests
 
     def rule(self, event):
         return all(
             [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 duo_admin_app_integration_secret_key_viewed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Generic Skey View",
         ExpectedResult=True,
         Log={
@@ -30,15 +30,15 @@
 
 
 class DuoAdminAppIntegrationSecretKeyViewed(PantherRule):
     Description = "An administrator viewed a Secret Key for an Application Integration"
     DisplayName = "Duo Admin App Integration Secret Key Viewed"
     Reference = "https://duo.com/docs/adminapi"
     Runbook = "The security of your Duo application is tied to the security of your secret key (skey). Secure it as you would any sensitive credential. Don't share it with unauthorized individuals or email it to anyone under any circumstances!"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.App.Integration.Secret.Key.Viewed-prototype"
     Tests = duo_admin_app_integration_secret_key_viewed_tests
 
     def rule(self, event):
         # Return True to match the log event and trigger an alert.
         return event.get("action", "") == "integration_skey_view"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 duo_admin_bypass_code_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Bypass Create",
         ExpectedResult=True,
         Log={
@@ -32,15 +32,15 @@
 
 
 class DuoAdminBypassCodeCreated(PantherRule):
     Description = "A Duo administrator created an MFA bypass code for an application."
     DisplayName = "Duo Admin Bypass Code Created"
     Runbook = "Confirm this was authorized and necessary behavior."
     Reference = "https://duo.com/docs/administration-users#generating-a-bypass-code"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.Bypass.Code.Created-prototype"
     Tests = duo_admin_bypass_code_created_tests
 
     def rule(self, event):
         # Return True to match the log event and trigger an alert.
         return event.get("action", "") == "bypass_create"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 duo_admin_bypass_code_viewed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Bypass View",
         ExpectedResult=True,
         Log={
@@ -32,15 +32,15 @@
 
 
 class DuoAdminBypassCodeViewed(PantherRule):
     Description = "An administrator viewed the MFA bypass code for a user."
     DisplayName = "Duo Admin Bypass Code Viewed"
     Reference = "https://duo.com/docs/adminapi"
     Runbook = "Confirm this behavior is authorized. The security of your Duo application is tied to the security of your secret key (skey). Secure it as you would any sensitive credential. You should not share it with unauthorized individuals or email it to anyone under any circumstances!"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.Bypass.Code.Viewed-prototype"
     Tests = duo_admin_bypass_code_viewed_tests
 
     def rule(self, event):
         # Return True to match the log event and trigger an alert.
         return event.get("action", "") == "bypass_view"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_create_admin.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_create_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_duo_helpers import (
     deserialize_administrator_log_event_description,
     duo_alert_context,
 )
 from pypanther.log_types import LogType
 
 duo_admin_create_admin_tests: List[PantherRuleTest] = [
@@ -34,15 +34,15 @@
 ]
 
 
 class DuoAdminCreateAdmin(PantherRule):
     Description = "A new Duo Administrator was created. "
     DisplayName = "Duo Admin Create Admin"
     Reference = "https://duo.com/docs/administration-admins#add-an-administrator"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.Create.Admin-prototype"
     Tests = duo_admin_create_admin_tests
 
     def rule(self, event):
         return event.get("action") == "admin_create"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_lockout.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_lockout.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 duo_admin_lockout_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Admin lockout- invalid json",
         ExpectedResult=True,
         Log={
@@ -42,15 +42,15 @@
 ]
 
 
 class DuoAdminLockout(PantherRule):
     Description = "Alert when a duo administrator is locked out of their account."
     DisplayName = "Duo Admin Lockout"
     Reference = "https://duo.com/docs/adminapi"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.Lockout-prototype"
     Tests = duo_admin_lockout_tests
 
     def rule(self, event):
         # Return True to match the log event and trigger an alert.
         return event.get("action", "") == "admin_lockout"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_duo_helpers import deserialize_administrator_log_event_description
 from pypanther.log_types import LogType
 
 duo_admin_action_marked_fraudulent_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="marked_fraud",
         ExpectedResult=True,
@@ -32,15 +32,15 @@
 
 class DUOAdminActionMarkedFraudulent(PantherRule):
     RuleID = "DUO.Admin.Action.MarkedFraudulent-prototype"
     DisplayName = "Duo Admin Marked Push Fraudulent"
     DedupPeriodMinutes = 15
     LogTypes = [LogType.Duo_Administrator]
     Tags = ["Duo"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Duo push was marked fraudulent by an admin."
     Reference = "https://duo.com/docs/adminapi#administrator-logs"
     Runbook = "Follow up with the administrator to determine reasoning for marking fraud."
     Tests = duo_admin_action_marked_fraudulent_tests
 
     def rule(self, event):
         event_description = deserialize_administrator_log_event_description(event)
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_duo_helpers import duo_alert_context
 from pypanther.log_types import LogType
 
 duo_admin_mfa_restrictions_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Admin MFA Update Event",
         ExpectedResult=True,
@@ -32,15 +32,15 @@
 
 class DuoAdminMFARestrictionsUpdated(PantherRule):
     Description = (
         "Detects changes to allowed MFA factors administrators can use to log into the admin panel."
     )
     DisplayName = "Duo Admin MFA Restrictions Updated"
     Reference = "https://duo.com/docs/essentials-overview"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.MFA.Restrictions.Updated-prototype"
     Tests = duo_admin_mfa_restrictions_updated_tests
 
     def rule(self, event):
         return event.get("action") == "update_admin_factor_restrictions"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_duo_helpers import (
     deserialize_administrator_log_event_description,
     duo_alert_context,
 )
 from pypanther.log_types import LogType
 
 duo_admin_new_admin_api_app_integration_tests: List[PantherRuleTest] = [
@@ -47,15 +47,15 @@
 ]
 
 
 class DuoAdminNewAdminAPIAppIntegration(PantherRule):
     Description = "Identifies creation of new Admin API integrations for Duo."
     DisplayName = "Duo Admin New Admin API App Integration"
     Reference = "https://duo.com/docs/adminapi#overview"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.New.Admin.API.App.Integration-prototype"
     Tests = duo_admin_new_admin_api_app_integration_tests
 
     def rule(self, event):
         if event.get("action") == "integration_create":
             description = deserialize_administrator_log_event_description(event)
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_policy_updated.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_policy_updated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_duo_helpers import duo_alert_context
 from pypanther.log_types import LogType
 
 duo_admin_policy_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Policy Update",
         ExpectedResult=True,
@@ -31,15 +31,15 @@
 ]
 
 
 class DuoAdminPolicyUpdated(PantherRule):
     Description = "A Duo Administrator updated a Policy, which governs how users authenticate."
     DisplayName = "Duo Admin Policy Updated"
     Reference = "https://duo.com/docs/policy#authenticators-policy-settings"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.Policy.Updated-prototype"
     Tests = duo_admin_policy_updated_tests
 
     def rule(self, event):
         return event.get("action") == "policy_update"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_duo_helpers import (
     deserialize_administrator_log_event_description,
     duo_alert_context,
 )
 from pypanther.log_types import LogType
 
 duo_admin_ssosaml_requirement_disabled_tests: List[PantherRuleTest] = [
@@ -57,15 +57,15 @@
 
 class DuoAdminSSOSAMLRequirementDisabled(PantherRule):
     Description = (
         "Detects when SAML Authentication for Administrators is marked as Disabled or Optional."
     )
     DisplayName = "Duo Admin SSO SAML Requirement Disabled"
     Reference = "https://duo.com/docs/sso#saml:~:text=Modify%20Authentication%20Sources"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.SSO.SAML.Requirement.Disabled-prototype"
     Tests = duo_admin_ssosaml_requirement_disabled_tests
 
     def rule(self, event):
         if event.get("action") == "admin_single_sign_on_update":
             description = deserialize_administrator_log_event_description(event)
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_duo_helpers import (
     deserialize_administrator_log_event_description,
     duo_alert_context,
 )
 from pypanther.log_types import LogType
 
 duo_admin_user_mfa_bypass_enabled_tests: List[PantherRuleTest] = [
@@ -59,15 +59,15 @@
 ]
 
 
 class DuoAdminUserMFABypassEnabled(PantherRule):
     Description = "An Administrator enabled a user to authenticate without MFA."
     DisplayName = "Duo Admin User MFA Bypass Enabled"
     Reference = "https://duo.com/docs/policy#authentication-policy"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Duo_Administrator]
     RuleID = "Duo.Admin.User.MFA.Bypass.Enabled-prototype"
     Tests = duo_admin_user_mfa_bypass_enabled_tests
 
     def rule(self, event):
         if event.get("action") == "user_update":
             description = deserialize_administrator_log_event_description(event)
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_action_fraudulent.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_action_fraudulent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 duo_user_action_fraudulent_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="user_marked_fraud",
         ExpectedResult=True,
@@ -24,15 +24,15 @@
 
 class DUOUserActionFraudulent(PantherRule):
     RuleID = "DUO.User.Action.Fraudulent-prototype"
     DisplayName = "Duo User Action Reported as Fraudulent"
     DedupPeriodMinutes = 15
     LogTypes = [LogType.Duo_Authentication]
     Tags = ["Duo"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Alert when a user reports a Duo action as fraudulent.\n"
     Reference = "https://duo.com/docs/adminapi#authentication-logs"
     Runbook = "Follow up with the user to confirm."
     Tests = duo_user_action_fraudulent_tests
 
     def rule(self, event):
         return event.get("result") == "fraud"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_anomalous_push.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_anomalous_push.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 duo_user_denied_anomalous_push_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="anomalous_push_occurred",
         ExpectedResult=True,
@@ -52,15 +52,15 @@
 
 class DUOUserDeniedAnomalousPush(PantherRule):
     RuleID = "DUO.User.Denied.AnomalousPush-prototype"
     DisplayName = "Duo User Auth Denied For Anomalous Push"
     DedupPeriodMinutes = 15
     LogTypes = [LogType.Duo_Authentication]
     Tags = ["Duo"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Duo authentication was denied due to an anomalous 2FA push.\n"
     Reference = "https://duo.com/docs/adminapi#authentication-logs"
     Runbook = "Follow up with the user to confirm they intended several pushes in quick succession."
     Tests = duo_user_denied_anomalous_push_tests
 
     def rule(self, event):
         return event.get("reason") == "anomalous_push" and event.get("result") == "denied"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_bypass_code_used.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_bypass_code_used.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 duo_user_bypass_code_used_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="bypass_code_used",
         ExpectedResult=True,
@@ -52,15 +52,15 @@
 
 class DUOUserBypassCodeUsed(PantherRule):
     RuleID = "DUO.User.BypassCode.Used-prototype"
     DisplayName = "Duo User Bypass Code Used"
     DedupPeriodMinutes = 5
     LogTypes = [LogType.Duo_Authentication]
     Tags = ["Duo"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A Duo user's bypass code was used to authenticate"
     Reference = "https://duo.com/docs/adminapi#authentication-logs"
     Runbook = "Follow up with the user to confirm they used the bypass code themselves."
     Tests = duo_user_bypass_code_used_tests
 
     def rule(self, event):
         return event.get("reason") == "bypass_user" and event.get("result") == "success"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py` & `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 duo_user_endpoint_failure_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="endpoint_is_not_in_management_system",
         ExpectedResult=True,
@@ -108,15 +108,15 @@
 
 class DUOUserEndpointFailure(PantherRule):
     RuleID = "DUO.User.Endpoint.Failure-prototype"
     DisplayName = "Duo User Denied For Endpoint Error"
     DedupPeriodMinutes = 15
     LogTypes = [LogType.Duo_Authentication]
     Tags = ["Duo"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Duo user's authentication was denied due to a suspicious error on the endpoint"
     Reference = "https://duo.com/docs/adminapi#authentication-logs"
     Runbook = (
         "Follow up with the endpoint owner to see status. Follow up with user to verify attempts."
     )
     Tests = duo_user_endpoint_failure_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcp_access_attempts_violating_vpc_service_controls_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -170,15 +170,15 @@
 ]
 
 
 class GCPAccessAttemptsViolatingVPCServiceControls(PantherRule):
     Description = "An access attempt violating VPC service controls (such as Perimeter controls) has been made."
     DisplayName = "GCP Access Attempts Violating VPC Service Controls"
     Reference = "https://cloud.google.com/vpc-service-controls/docs/troubleshooting#debugging"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.Access.Attempts.Violating.VPC.Service.Controls-prototype"
     Tests = gcp_access_attempts_violating_vpc_service_controls_tests
 
     def rule(self, event):
         severity = deep_get(event, "severity", default="")
         status_code = deep_get(event, "protoPayload", "status", "code", default="")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_big_query_large_scan_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="small query",
         ExpectedResult=False,
@@ -176,15 +176,15 @@
 ]
 
 
 class GCPBigQueryLargeScan(PantherRule):
     Description = "Detect any BigQuery query that is doing a very large scan (> 1 GB)."
     DisplayName = "GCP BigQuery Large Scan"
     Reference = "https://cloud.google.com/bigquery/docs/running-queries"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.BigQuery.Large.Scan-prototype"
     Tests = gcp_big_query_large_scan_tests
     # 1.07 GB
     QUERY_THRESHOLD_BYTES = 1073741824
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_cloud_storage_buckets_modified_or_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="other event",
         ExpectedResult=False,
@@ -117,15 +117,15 @@
 ]
 
 
 class GCPCloudStorageBucketsModifiedOrDeleted(PantherRule):
     Description = "Detects GCP cloud storage bucket updates and deletes."
     DisplayName = "GCP Cloud Storage Buckets Modified Or Deleted"
     Reference = "https://cloud.google.com/storage/docs/buckets"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.Cloud.Storage.Buckets.Modified.Or.Deleted-prototype"
     Tests = gcp_cloud_storage_buckets_modified_or_deleted_tests
     BUCKET_OPERATIONS = ["storage.buckets.delete", "storage.buckets.update"]
 
     def rule(self, event):
         return all(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcp_cloud_build_potential_privilege_escalation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GCP CloudBuild - Build with Potentially Privileged Access",
@@ -118,15 +118,15 @@
     LogTypes = [LogType.GCP_AuditLog]
     Description = "Detects privilege escalation attacks designed to gain access to the Cloud Build Service Account. A user with permissions to start a new build with Cloud Build can gain access to the Cloud Build Service Account and abuse it for more access to the environment."
     DisplayName = "GCP CloudBuild Potential Privilege Escalation"
     RuleID = "GCP.CloudBuild.Potential.Privilege.Escalation-prototype"
     Reference = "https://rhinosecuritylabs.com/gcp/iam-privilege-escalation-gcp-cloudbuild/"
     Runbook = "Confirm this was authorized and necessary behavior. To defend against this privilege escalation attack, it is necessary to restrict the permissions granted to the Cloud Build Service Account and to be careful granting the cloudbuild.builds.create permission to any users in your Organization. Most importantly, you need to know that any user who is granted cloudbuild.builds.create, is also indirectly granted all the permissions granted to the Cloud Build Service Account. If that’s alright with you, then you may not need to worry about this attack vector, but it is still highly recommended to modify the default permissions granted to the Cloud Build Service Account."
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tests = gcp_cloud_build_potential_privilege_escalation_tests
 
     def rule(self, event):
         if not deep_get(event, "protoPayload", "methodName", default="METHOD_NOT_FOUND").endswith(
             "CloudBuild.CreateBuild"
         ):
             return False
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcp_cloudfunctions_functions_create_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="privilege-escalation",
@@ -50,15 +50,15 @@
 
 
 class GCPCloudfunctionsFunctionsCreate(PantherRule):
     RuleID = "GCP.Cloudfunctions.Functions.Create-prototype"
     DisplayName = "GCP cloudfunctions functions create"
     Description = "The Identity and Access Management (IAM) service manages authorization and authentication for a GCP environment. This means that there are very likely multiple privilege escalation methods that use the IAM service and/or its permissions."
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Runbook = "Confirm this was authorized and necessary behavior. This is not a vulnerability in GCP, it is a vulnerability in how GCP environment is configured, so it is necessary to be aware of these attack vectors and to defend against them. It’s also important to remember that privilege escalation does not necessarily need to pass through the IAM service to be effective. Make sure to follow the principle of least-privilege in your environments to help mitigate these security risks."
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
     Tests = gcp_cloudfunctions_functions_create_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcp_cloudfunctions_functions_update_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="privilege-escalation",
@@ -50,15 +50,15 @@
 
 
 class GCPCloudfunctionsFunctionsUpdate(PantherRule):
     RuleID = "GCP.Cloudfunctions.Functions.Update-prototype"
     DisplayName = "GCP cloudfunctions functions update"
     Description = "The Identity and Access Management (IAM) service manages authorization and authentication for a GCP environment. This means that there are very likely multiple privilege escalation methods that use the IAM service and/or its permissions."
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Runbook = "Confirm this was authorized and necessary behavior. This is not a vulnerability in GCP, it is a vulnerability in how GCP environment is configured, so it is necessary to be aware of these attack vectors and to defend against them. It’s also important to remember that privilege escalation does not necessarily need to pass through the IAM service to be effective. Make sure to follow the principle of least-privilege in your environments to help mitigate these security risks."
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
     Tests = gcp_cloudfunctions_functions_update_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gc_pcomputeinstancescreate_privilege_escalation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GCP compute.instances - Potential Privilege Escalation",
@@ -339,15 +339,15 @@
     DisplayName = "GCP compute.instances.create Privilege Escalation"
     RuleID = "GCP.compute.instances.create.Privilege.Escalation-prototype"
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Runbook = "Confirm this was authorized and necessary behavior."
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tests = gc_pcomputeinstancescreate_privilege_escalation_tests
     REQUIRED_PERMISSIONS = [
         "compute.disks.create",
         "compute.instances.create",
         "compute.instances.setMetadata",
         "compute.instances.setServiceAccount",
         "compute.subnetworks.use",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_destructive_queries_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Drop Table Event",
         ExpectedResult=True,
@@ -138,15 +138,15 @@
 ]
 
 
 class GCPDestructiveQueries(PantherRule):
     Description = "Detect any destructive BigQuery queries or jobs such as update, delete, drop, alter or truncate."
     DisplayName = "GCP Destructive Queries"
     Reference = "https://cloud.google.com/bigquery/docs/managing-tables"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.Destructive.Queries-prototype"
     Tests = gcp_destructive_queries_tests
     DESTRUCTIVE_STATEMENTS = ["UPDATE", "DELETE", "DROP_TABLE", "ALTER_TABLE", "TRUNCATE_TABLE"]
 
     def rule(self, event):
         if all(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpdns_zone_modifiedor_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="dns.managedZones.delete-should-alert",
@@ -308,15 +308,15 @@
 
 
 class GCPDNSZoneModifiedorDeleted(PantherRule):
     Description = "Detection for GCP DNS zones that are deleted, patched, or updated."
     DisplayName = "GCP DNS Zone Modified or Deleted"
     Runbook = "Verify that this modification or deletion was expected. These operations are high-impact events and can result in downtimes or total outages."
     Reference = "https://cloud.google.com/dns/docs/zones"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.DNS.Zone.Modified.or.Deleted-prototype"
     Tests = gcpdns_zone_modifiedor_deleted_tests
 
     def rule(self, event):
         methods = (
             "dns.changes.create",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_firewall_rule_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="compute.firewalls.create-should-alert",
@@ -163,15 +163,15 @@
     ),
 ]
 
 
 class GCPFirewallRuleCreated(PantherRule):
     DisplayName = "GCP Firewall Rule Created"
     RuleID = "GCP.Firewall.Rule.Created-prototype"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Firewall", "Networking", "Infrastructure"]
     Description = "This rule detects creations of GCP firewall rules.\n"
     Runbook = "Ensure that the rule creation was expected. Firewall rule creations can expose [vulnerable] resoures to the internet.\n"
     Reference = "https://cloud.google.com/firewall/docs/about-firewalls"
     Tests = gcp_firewall_rule_created_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_firewall_rule_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="compute.firewalls-delete-should-alert",
@@ -119,15 +119,15 @@
     ),
 ]
 
 
 class GCPFirewallRuleDeleted(PantherRule):
     DisplayName = "GCP Firewall Rule Deleted"
     RuleID = "GCP.Firewall.Rule.Deleted-prototype"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Firewall", "Networking", "Infrastructure"]
     Description = "This rule detects deletions of GCP firewall rules.\n"
     Runbook = "Ensure that the rule deletion was expected. Firewall rule deletions can cause service interruptions or outages.\n"
     Reference = "https://cloud.google.com/firewall/docs/about-firewalls"
     Tests = gcp_firewall_rule_deleted_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_firewall_rule_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="compute.firewalls.update-should-alert",
@@ -163,15 +163,15 @@
     ),
 ]
 
 
 class GCPFirewallRuleModified(PantherRule):
     DisplayName = "GCP Firewall Rule Modified"
     RuleID = "GCP.Firewall.Rule.Modified-prototype"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Firewall", "Networking", "Infrastructure"]
     Description = "This rule detects modifications to GCP firewall rules.\n"
     Runbook = "Ensure that the rule modification was expected. Firewall rule changes can cause service interruptions or outages.\n"
     Reference = "https://cloud.google.com/firewall/docs/about-firewalls"
     Tests = gcp_firewall_rule_modified_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpgcsiam_changes_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GCS IAM Change",
         ExpectedResult=True,
@@ -64,15 +64,15 @@
 
 class GCPGCSIAMChanges(PantherRule):
     RuleID = "GCP.GCS.IAMChanges-prototype"
     DisplayName = "GCP GCS IAM Permission Changes"
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Google Cloud Storage", "Collection:Data From Cloud Storage Object"]
     Reports = {"CIS": ["2.1"], "MITRE ATT&CK": ["TA0009:T1530"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Monitoring changes to Cloud Storage bucket permissions may reduce time to detect and correct permissions on sensitive Cloud Storage bucket and objects inside the bucket.\n"
     Runbook = "Validate the GCS bucket change was safe."
     Reference = "https://cloud.google.com/storage/docs/access-control/iam-permissions"
     SummaryAttributes = ["severity", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = gcpgcsiam_changes_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpgcs_public_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GCS AllUsers Read Permission",
         ExpectedResult=True,
@@ -65,15 +65,15 @@
 class GCPGCSPublic(PantherRule):
     RuleID = "GCP.GCS.Public-prototype"
     DisplayName = "GCS Bucket Made Public"
     DedupPeriodMinutes = 15
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Google Cloud Storage", "Collection:Data From Cloud Storage Object"]
     Reports = {"MITRE ATT&CK": ["TA0009:T1530"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Adversaries may access data objects from improperly secured cloud storage."
     Runbook = "Validate the GCS bucket change was safe."
     Reference = "https://cloud.google.com/storage/docs/access-control/making-data-public"
     SummaryAttributes = ["severity", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = gcpgcs_public_tests
     GCS_READ_ROLES = {
         "roles/storage.objectAdmin",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpiam_corporate_email_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Gmail account added",
         ExpectedResult=True,
@@ -289,15 +289,15 @@
 class GCPIAMCorporateEmail(PantherRule):
     RuleID = "GCP.IAM.CorporateEmail-prototype"
     DisplayName = "GCP Corporate Email Not Used"
     DedupPeriodMinutes = 720
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Identity & Access Management", "Persistence:Create Account"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1136"], "CIS": ["1.1"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A Gmail account is being used instead of a corporate email"
     Runbook = "Remove the user"
     Reference = "https://cloud.google.com/iam/docs/service-account-overview"
     SummaryAttributes = ["severity", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = gcpiam_corporate_email_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpiam_custom_role_changes_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Custom Role Created",
         ExpectedResult=True,
@@ -94,15 +94,15 @@
 class GCPIAMCustomRoleChanges(PantherRule):
     RuleID = "GCP.IAM.CustomRoleChanges-prototype"
     DisplayName = "GCP IAM Role Has Changed"
     DedupPeriodMinutes = 1440
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Identity & Access Management", "Privilege Escalation:Valid Accounts"]
     Reports = {"CIS": ["2.6"], "MITRE ATT&CK": ["TA0004:T1078"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A custom role has been created, deleted, or updated."
     Runbook = "No action needed, informational"
     Reference = "https://cloud.google.com/iam/docs/creating-custom-roles"
     SummaryAttributes = ["severity", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = gcpiam_custom_role_changes_tests
     ROLE_METHODS = {
         "google.iam.admin.v1.CreateRole",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpiam_org_folder_iam_changes_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Terraform User Agent",
         ExpectedResult=True,
@@ -167,15 +167,15 @@
 class GCPIAMOrgFolderIAMChanges(PantherRule):
     RuleID = "GCP.IAM.OrgFolderIAMChanges-prototype"
     DisplayName = "GCP Org or Folder Policy Was Changed Manually"
     DedupPeriodMinutes = 1440
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Identity & Access Management"]
     Reports = {"GCP_CIS_1.3": ["1.8"], "MITRE ATT&CK": ["Privilege Escalation:Valid Accounts"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Alert if a GCP Org or Folder Policy Was Changed Manually.\n"
     Runbook = "Contact the party that made the change. If it was intended to be temporary, ask for a window for rollback (< 24 hours).  If it must be permanent, ask for change-management doc explaining why it was needed.  Direct them to make the change in Terraform to avoid automated rollback. Grep for google_org and google_folder in terraform repos for places to  put your new policy bindings.\n"
     Reference = "https://cloud.google.com/iam/docs/granting-changing-revoking-access"
     SummaryAttributes = ["severity", "p_any_ip_addresses"]
     Tests = gcpiam_org_folder_iam_changes_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gc_piamrolesupdate_privilege_escalation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Test-876cde",
@@ -45,15 +45,15 @@
 
 class GCPiamrolesupdatePrivilegeEscalation(PantherRule):
     RuleID = "GCP.iam.roles.update.Privilege.Escalation-prototype"
     DisplayName = "GCP iam.roles.update Privilege Escalation"
     Description = "If your user is assigned a custom IAM role, then iam.roles.update will allow you to update the “includedPermissons” on that role. Because it is assigned to you, you will gain the additional privileges, which could be anything you desire."
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reports = {"TA0004": ["T1548"]}
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Runbook = "Confirm this was authorized and necessary behavior. This is not a vulnerability in GCP, it is a vulnerability in how GCP environment is configured, so it is necessary to be aware of these attack vectors and to defend against them. It’s also important to remember that privilege escalation does not necessarily need to pass through the IAM service to be effective. Make sure to follow the principle of least-privilege in your environments to help mitigate these security risks."
     Tests = gc_piamrolesupdate_privilege_escalation_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gc_piamservice_account_keyscreate_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="privilege-escalation",
@@ -50,15 +50,15 @@
 
 
 class GCPiamserviceAccountKeyscreate(PantherRule):
     RuleID = "GCP.iam.serviceAccountKeys.create-prototype"
     DisplayName = "GCP.Iam.ServiceAccountKeys.Create"
     Description = "If your user is assigned a custom IAM role, then iam.roles.update will allow you to update the “includedPermissons” on that role. Because it is assigned to you, you will gain the additional privileges, which could be anything you desire."
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Runbook = "Confirm this was authorized and necessary behavior. This is not a vulnerability in GCP, it is a vulnerability in how GCP environment is configured, so it is necessary to be aware of these attack vectors and to defend against them. It’s also important to remember that privilege escalation does not necessarily need to pass through the IAM service to be effective. Make sure to follow the principle of least-privilege in your environments to help mitigate these security risks."
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
     Tests = gc_piamservice_account_keyscreate_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpia_mservice_accountsget_access_token_privilege_escalation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="iam.serviceAccounts.getAccessToken granted",
@@ -104,15 +104,15 @@
 
 
 class GCPIAMserviceAccountsgetAccessTokenPrivilegeEscalation(PantherRule):
     RuleID = "GCP.IAM.serviceAccounts.getAccessToken.Privilege.Escalation-prototype"
     DisplayName = "GCP IAM serviceAccounts getAccessToken Privilege Escalation"
     LogTypes = [LogType.GCP_AuditLog]
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "The Identity and Access Management (IAM) service manages authorization and authentication for a GCP environment. This means that there are very likely multiple privilege escalation methods that use the IAM service and/or its permissions."
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Tests = gcpia_mservice_accountsget_access_token_privilege_escalation_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpia_mservice_accountssign_blob_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="iam.serviceAccounts.signBlob granted",
@@ -104,15 +104,15 @@
 
 
 class GCPIAMserviceAccountssignBlob(PantherRule):
     RuleID = "GCP.IAM.serviceAccounts.signBlob-prototype"
     DisplayName = "GCP IAM serviceAccounts signBlob"
     LogTypes = [LogType.GCP_AuditLog]
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = 'The iam.serviceAccounts.signBlob permission "allows signing of arbitrary payloads" in GCP. This means we can create a signed blob that requests an access token from the Service Account we are targeting.'
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Tests = gcpia_mservice_accountssign_blob_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcpia_mservice_accountssign_jwt_privilege_escalation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="JWT Signed",
@@ -104,15 +104,15 @@
 
 
 class GCPIAMserviceAccountssignJwtPrivilegeEscalation(PantherRule):
     RuleID = "GCP.IAM.serviceAccounts.signJwt.Privilege.Escalation-prototype"
     DisplayName = "GCP IAM serviceAccounts.signJwt Privilege Escalation"
     LogTypes = [LogType.GCP_AuditLog]
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects iam.serviceAccounts.signJwt method for privilege escalation in GCP. This method works by signing well-formed JSON web tokens (JWTs). The script for this method will sign a well-formed JWT and request a new access token belonging to the Service Account with it."
     Runbook = "These is not a vulnerability in GCP, this is a vulnerability in how you have configured your GCP environment, so it is your responsibility to be aware of these attack vectors and to defend against them. Make sure to follow the principle of least-privilege in your environments to help mitigate these security risks."
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Tests = gcpia_mservice_accountssign_jwt_privilege_escalation_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 gcp_inbound_sso_profile_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="InboundSsoProfileDeleted-False",
         ExpectedResult=False,
         Log={
@@ -159,15 +159,15 @@
 
 class GCPInboundSSOProfileCreated(PantherRule):
     RuleID = "GCP.Inbound.SSO.Profile.Created-prototype"
     DisplayName = "GCP Inbound SSO Profile Created"
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["Account Manipulation", "Additional Cloud Roles", "GCP", "Privilege Escalation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1136.003", "TA0003:T1098.003", "TA0004:T1098.003"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Runbook = "Ensure that the SSO profile creation or modification was expected. Adversaries may use this to persist or allow additional access or escalate their privilege.\n"
     Reference = "https://medium.com/google-cloud/detection-of-inbound-sso-persistence-techniques-in-gcp-c56f7b2a588b"
     Tests = gcp_inbound_sso_profile_created_tests
     METHODS = [
         "google.admin.AdminService.inboundSsoProfileCreated",
         "google.admin.AdminService.inboundSsoProfileUpdated",
     ]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcp_log_bucket_or_sink_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="logging-bucket.deleted-should-alert",
@@ -201,15 +201,15 @@
     ),
 ]
 
 
 class GCPLogBucketOrSinkDeleted(PantherRule):
     DisplayName = "GCP Log Bucket or Sink Deleted"
     RuleID = "GCP.Log.Bucket.Or.Sink.Deleted-prototype"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Logging", "Bucket", "Sink", "Infrastructure"]
     Description = "This rule detects deletions of GCP Log Buckets or Sinks.\n"
     Runbook = "Ensure that the bucket or sink deletion was expected. Adversaries may do this to cover their tracks.\n"
     Reference = "https://cloud.google.com/logging/docs"
     Tests = gcp_log_bucket_or_sink_deleted_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_logging_settings_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -124,15 +124,15 @@
 ]
 
 
 class GCPLoggingSettingsModified(PantherRule):
     Description = "Detects any changes made to logging settings"
     DisplayName = "GCP Logging Settings Modified"
     Reference = "https://cloud.google.com/logging/docs/default-settings"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.Logging.Settings.Modified-prototype"
     Tests = gcp_logging_settings_modified_tests
 
     def rule(self, event):
         return all(
             [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_logging_sink_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="logging-sink.modifed-should-alert",
@@ -121,15 +121,15 @@
     ),
 ]
 
 
 class GCPLoggingSinkModified(PantherRule):
     DisplayName = "GCP Logging Sink Modified"
     RuleID = "GCP.Logging.Sink.Modified-prototype"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Logging", "Sink", "Infrastructure"]
     Description = "This rule detects modifications to GCP Log Sinks.\n"
     Runbook = "Ensure that the modification was valid or expected. Adversaries may do this to exfiltrate logs or evade detection.\n"
     Reference = "https://cloud.google.com/logging/docs"
     Tests = gcp_logging_sink_modified_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcp_permissions_grantedto_createor_manage_service_account_key_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="other event",
         ExpectedResult=False,
@@ -176,15 +176,15 @@
 ]
 
 
 class GCPPermissionsGrantedtoCreateorManageServiceAccountKey(PantherRule):
     Description = "Permissions granted to impersonate a service account. This includes predefined service account IAM roles granted at the parent project, folder or organization-level."
     DisplayName = "GCP Permissions Granted to Create or Manage Service Account Key"
     Reference = "https://cloud.google.com/iam/docs/keys-create-delete"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.Permissions.Granted.to.Create.or.Manage.Service.Account.Key-prototype"
     Tests = gcp_permissions_grantedto_createor_manage_service_account_key_tests
     SERVICE_ACCOUNT_MANAGE_ROLES = [
         "roles/iam.serviceAccountTokenCreator",
         "roles/iam.serviceAccountUser",
     ]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcp_privilege_escalation_by_deployments_create_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="privilege-escalation",
@@ -50,15 +50,15 @@
 
 
 class GCPPrivilegeEscalationByDeploymentsCreate(PantherRule):
     RuleID = "GCP.Privilege.Escalation.By.Deployments.Create-prototype"
     DisplayName = "GCP.Privilege.Escalation.By.Deployments.Create"
     Description = "Detects privilege escalation in GCP by taking over the deploymentsmanager.deployments.create permission"
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reference = (
         "https://rhinosecuritylabs.com/gcp/privilege-escalation-google-cloud-platform-part-1/"
     )
     Runbook = "Confirm this was authorized and necessary behavior. This is not a vulnerability in GCP, it is a vulnerability in how GCP environment is configured, so it is necessary to be aware of these attack vectors and to defend against them. It’s also important to remember that privilege escalation does not necessarily need to pass through the IAM service to be effective. Make sure to follow the principle of least-privilege in your environments to help mitigate these security risks."
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
     Tests = gcp_privilege_escalation_by_deployments_create_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_walk
 from pypanther.log_types import LogType
 
 gcp_service_account_access_denied_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="service-account.access-denied-should-alert",
@@ -127,15 +127,15 @@
 
 
 class GCPServiceAccountAccessDenied(PantherRule):
     DedupPeriodMinutes = 5
     Threshold = 30
     DisplayName = "GCP Service Account Access Denied"
     RuleID = "GCP.Service.Account.Access.Denied-prototype"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Service Account", "Access"]
     Description = "This rule detects deletions of GCP Log Buckets or Sinks.\n"
     Runbook = "Ensure that the bucket or sink deletion was expected. Adversaries may do this to cover their tracks.\n"
     Reference = "https://cloud.google.com/iam/docs/service-account-overview"
     Tests = gcp_service_account_access_denied_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_service_accountor_keys_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Created Service Account Key",
         ExpectedResult=True,
@@ -204,15 +204,15 @@
 ]
 
 
 class GCPServiceAccountorKeysCreated(PantherRule):
     Description = "Detects when a service account or key is created manually by a user instead of an automated workflow."
     DisplayName = "GCP Service Account or Keys Created "
     Reference = "https://cloud.google.com/iam/docs/keys-create-delete"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.Service.Account.or.Keys.Created-prototype"
     Tests = gcp_service_accountor_keys_created_tests
 
     def rule(self, event):
         return all(
             [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gc_pserviceusageapi_keyscreate_privilege_escalation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GCP API Key Created",
@@ -178,15 +178,15 @@
     LogTypes = [LogType.GCP_AuditLog]
     Description = "Detects serviceusage.apiKeys.create method for privilege escalation in GCP. By default, API Keys are created with no restrictions, which means they have access to the entire GCP project they were created in. We can capitalize on that fact by creating a new API key that may have more privileges than our own user."
     DisplayName = "GCP serviceusage.apiKeys.create Privilege Escalation"
     RuleID = "GCP.serviceusage.apiKeys.create.Privilege.Escalation-prototype"
     Reference = "https://rhinosecuritylabs.com/cloud-security/privilege-escalation-google-cloud-platform-part-2/"
     Runbook = "Confirm this was authorized and necessary behavior. This is not a vulnerability in GCP, it is a vulnerability in how GCP environment is configured, so it is necessary to be aware of these attack vectors and to defend against them. It’s also important to remember that privilege escalation does not necessarily need to pass through the IAM service to be effective. Make sure to follow the principle of least-privilege in your environments to help mitigate these security risks."
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tests = gc_pserviceusageapi_keyscreate_privilege_escalation_tests
 
     def rule(self, event):
         if not deep_get(event, "protoPayload", "methodName", default="METHOD_NOT_FOUND").endswith(
             "ApiKeys.CreateKey"
         ):
             return False
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpsql_config_changes_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Sql Instance Change",
         ExpectedResult=True,
@@ -34,15 +34,15 @@
 class GCPSQLConfigChanges(PantherRule):
     RuleID = "GCP.SQL.ConfigChanges-prototype"
     DisplayName = "GCP SQL Config Changes"
     DedupPeriodMinutes = 720
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Database"]
     Reports = {"CIS": ["2.11"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Monitoring changes to Sql Instance configuration may reduce time to detect and correct misconfigurations done on sql server.\n"
     Runbook = "Validate the Sql Instance configuration change was safe"
     Reference = "https://cloud.google.com/sql/docs/mysql/instance-settings"
     SummaryAttributes = ["severity", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = gcpsql_config_changes_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 gcp_storage_hmac_keys_create_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="privilege-escalation",
         ExpectedResult=True,
         Log={
@@ -44,15 +44,15 @@
 
 
 class GCPStorageHmacKeysCreate(PantherRule):
     RuleID = "GCP.Storage.Hmac.Keys.Create-prototype"
     DisplayName = "GCP storage hmac keys create"
     Description = "There is a feature of Cloud Storage, “interoperability”, that provides a way for Cloud Storage to interact with storage offerings from other cloud providers, like AWS S3. As part of that, there are HMAC keys that can be created for both Service Accounts and regular users. We can escalate Cloud Storage permissions by creating an HMAC key for a higher-privileged Service Account."
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reference = "https://rhinosecuritylabs.com/cloud-security/privilege-escalation-google-cloud-platform-part-2/"
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
     Tests = gcp_storage_hmac_keys_create_tests
 
     def rule(self, event):
         auth_info = event.deep_walk("protoPayload", "authorizationInfo", default=[])
         auth_info = auth_info if isinstance(auth_info, list) else [auth_info]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_unused_regions_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GCE Instance Terminated",
         ExpectedResult=False,
@@ -238,15 +238,15 @@
     Tags = [
         "GCP",
         "Database",
         "Configuration Required",
         "Defense Evasion:Unused/Unsupported Cloud Regions",
     ]
     Reports = {"MITRE ATT&CK": ["TA0005:T1535"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Adversaries may create cloud instances in unused geographic service regions in order to evade detection.\n"
     Runbook = "Validate the user making the request and the resource created."
     Reference = "https://cloud.google.com/docs/geography-and-regions"
     SummaryAttributes = ["severity", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = gcp_unused_regions_tests
     # 'asia',
     # 'australia',
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_user_addedto_iap_protected_service_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="other",
         ExpectedResult=False,
@@ -196,15 +196,15 @@
 
 
 class GCPUserAddedtoIAPProtectedService(PantherRule):
     Description = "A user has been granted access to a IAP protected service."
     DisplayName = "GCP User Added to IAP Protected Service"
     Runbook = "Note: GCP logs all bindings everytime this event occurs, not just changes. Bindings should be reviewed to ensure no unintended users have been added. "
     Reference = "https://cloud.google.com/iap/docs/managing-access"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.User.Added.to.IAP.Protected.Service-prototype"
     Tests = gcp_user_addedto_iap_protected_service_tests
 
     def rule(self, event):
         return (
             deep_get(event, "protoPayload", "methodName", default="")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpvpc_flow_logs_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Disable Flow Logs Event",
         ExpectedResult=True,
@@ -172,15 +172,15 @@
 ]
 
 
 class GCPVPCFlowLogsDisabled(PantherRule):
     Description = "VPC flow logs were disabled for a subnet."
     DisplayName = "GCP VPC Flow Logs Disabled"
     Reference = "https://cloud.google.com/vpc/docs/using-flow-logs"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.GCP_AuditLog]
     RuleID = "GCP.VPC.Flow.Logs.Disabled-prototype"
     Tests = gcpvpc_flow_logs_disabled_tests
 
     def rule(self, event):
         return all(
             [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 gcp_workforce_pool_createdor_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="DeleteWorkforcePool-False",
         ExpectedResult=False,
         Log={
@@ -180,15 +180,15 @@
 
 class GCPWorkforcePoolCreatedorUpdated(PantherRule):
     RuleID = "GCP.Workforce.Pool.Created.or.Updated-prototype"
     DisplayName = "GCP Workforce Pool Created or Updated"
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["Account Manipulation", "Additional Cloud Roles", "GCP", "Privilege Escalation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1136.003", "TA0003:T1098.003", "TA0004:T1098.003"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Runbook = "Ensure that the Workforce Pool creation or modification was expected. Adversaries may use this to persist or allow additional access or escalate their privilege.\n"
     Reference = "https://medium.com/google-cloud/detection-of-inbound-sso-persistence-techniques-in-gcp-c56f7b2a588b"
     Tests = gcp_workforce_pool_createdor_updated_tests
     METHODS = [
         "google.iam.admin.v1.WorkforcePools.CreateWorkforcePool",
         "google.iam.admin.v1.WorkforcePools.UpdateWorkforcePool",
     ]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 gcp_workload_identity_pool_createdor_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="DeleteWorkloadIdentityPoolProvider-False",
         ExpectedResult=False,
         Log={
@@ -188,15 +188,15 @@
 
 class GCPWorkloadIdentityPoolCreatedorUpdated(PantherRule):
     RuleID = "GCP.Workload.Identity.Pool.Created.or.Updated-prototype"
     DisplayName = "GCP Workload Identity Pool Created or Updated"
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["Account Manipulation", "Additional Cloud Roles", "GCP", "Privilege Escalation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1136.003", "TA0003:T1098.003", "TA0004:T1098.003"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Runbook = "Ensure that the Workload Identity Pool creation or modification was expected. Adversaries may use this to persist or allow additional access or escalate their privilege.\n"
     Reference = "https://medium.com/google-cloud/detection-of-inbound-sso-persistence-techniques-in-gcp-c56f7b2a588b"
     Tests = gcp_workload_identity_pool_createdor_updated_tests
     METHODS = [
         "google.iam.v1.WorkloadIdentityPools.CreateWorkloadIdentityPoolProvider",
         "google.iam.v1.WorkloadIdentityPools.UpdateWorkloadIdentityPoolProvider",
     ]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcp_access_attempts_violating_iap_access_controls_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Blocked By IAP",
         ExpectedResult=True,
@@ -104,15 +104,15 @@
 ]
 
 
 class GCPAccessAttemptsViolatingIAPAccessControls(PantherRule):
     Description = "GCP Access Attempts Violating IAP Access Controls"
     DisplayName = "GCP Access Attempts Violating IAP Access Controls"
     Reference = "https://cloud.google.com/iap/docs/concepts-overview"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.GCP_HTTPLoadBalancer]
     RuleID = "GCP.Access.Attempts.Violating.IAP.Access.Controls-prototype"
     Tests = gcp_access_attempts_violating_iap_access_controls_tests
 
     def rule(self, event):
         return all(
             [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcpgke_kubernetes_cron_job_created_or_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="create",
@@ -70,15 +70,15 @@
 
 
 class GCPGKEKubernetesCronJobCreatedOrModified(PantherRule):
     RuleID = "GCP.GKE.Kubernetes.Cron.Job.Created.Or.Modified-prototype"
     DisplayName = "GCP GKE Kubernetes Cron Job Created Or Modified"
     Description = "This detection monitor for any modifications or creations of a cron job in GKE. Attackers may create or modify an existing scheduled job in order to achieve cluster persistence."
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reference = "https://medium.com/snowflake/from-logs-to-detection-using-snowflake-and-panther-to-detect-k8s-threats-d72f70a504d7"
     Runbook = "Investigate a reason of creating or modifying a cron job in GKE. Create ticket if appropriate."
     Reports = {"MITRE ATT&CK": ["T1053.003"]}
     Tests = gcpgke_kubernetes_cron_job_created_or_modified_tests
 
     def rule(self, event):
         authorization_info = deep_walk(event, "protoPayload", "authorizationInfo")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import get_k8s_info
 from pypanther.helpers.gcp_environment import PRODUCTION_PROJECT_IDS, rule_exceptions
 from pypanther.helpers.panther_base_helpers import deep_walk
 from pypanther.log_types import LogType
 
 gcpk8s_exec_into_pod_tests: List[PantherRuleTest] = [
     PantherRuleTest(
@@ -83,15 +83,15 @@
 
 class GCPK8sExecIntoPod(PantherRule):
     RuleID = "GCP.K8s.ExecIntoPod-prototype"
     DisplayName = "Exec into Pod"
     Enabled = False
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Security Control", "Configuration Required"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Alerts when users exec into pod. Possible to specify specific projects and allowed users.\n"
     Runbook = "Investigate the user and determine why. Advise that it is discouraged practice. Create ticket if appropriate.\n"
     Reference = (
         "https://cloud.google.com/migrate/containers/docs/troubleshooting/executing-shell-commands"
     )
     Tests = gcpk8s_exec_into_pod_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpk8s_ioc_activity_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="triggers",
@@ -20,15 +20,15 @@
 
 
 class GCPK8sIOCActivity(PantherRule):
     RuleID = "GCP.K8s.IOC.Activity-prototype"
     DisplayName = "GCP K8s IOCActivity"
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Optional"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "This detection monitors for any kuberentes API Request originating from an Indicator of Compromise."
     Reports = {"MITRE ATT&CK": ["T1573.002"]}
     Runbook = "Add IP address the request is originated from to banned addresses."
     Reference = "https://medium.com/snowflake/from-logs-to-detection-using-snowflake-and-panther-to-detect-k8s-threats-d72f70a504d7"
     Tests = gcpk8s_ioc_activity_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcpk8s_new_daemonset_deployed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="privilege-escalation",
@@ -50,15 +50,15 @@
 
 
 class GCPK8sNewDaemonsetDeployed(PantherRule):
     RuleID = "GCP.K8s.New.Daemonset.Deployed-prototype"
     DisplayName = "GCP K8s New Daemonset Deployed"
     Description = "Detects Daemonset creation in GCP Kubernetes clusters."
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reference = "https://medium.com/snowflake/from-logs-to-detection-using-snowflake-and-panther-to-detect-k8s-threats-d72f70a504d7"
     Runbook = "Investigate a reason of creating Daemonset. Create ticket if appropriate."
     Reports = {"MITRE ATT&CK": ["TA0002:T1610"]}
     Tests = gcpk8s_new_daemonset_deployed_tests
 
     def rule(self, event):
         authorization_info = deep_walk(event, "protoPayload", "authorizationInfo")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcpk8s_pod_attached_to_node_host_network_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="triggers",
@@ -44,15 +44,15 @@
 
 
 class GCPK8sPodAttachedToNodeHostNetwork(PantherRule):
     RuleID = "GCP.K8s.Pod.Attached.To.Node.Host.Network-prototype"
     DisplayName = "GCP K8s Pod Attached To Node Host Network"
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Optional"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "This detection monitor for the creation of pods which are attached to the host's network. This allows a pod to listen to all network traffic for all deployed computer on that particular node and communicate with other compute on the network namespace. Attackers can use this to capture secrets passed in arguments or connections."
     Reports = {"MITRE ATT&CK": ["TA0004:T1611"]}
     Runbook = "Investigate a reason of creating a pod which is attached to the host's network. Advise that it is discouraged practice. Create ticket if appropriate."
     Reference = "https://medium.com/snowflake/from-logs-to-detection-using-snowflake-and-panther-to-detect-k8s-threats-d72f70a504d7"
     Tests = gcpk8s_pod_attached_to_node_host_network_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcpk8_s_pot_create_or_modify_host_path_volume_mount_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Pod With Suspicious Volume Mount Created",
@@ -222,15 +222,15 @@
 ]
 
 
 class GCPK8SPotCreateOrModifyHostPathVolumeMount(PantherRule):
     RuleID = "GCP.K8S.Pot.Create.Or.Modify.Host.Path.Volume.Mount-prototype"
     DisplayName = "GCP K8S Pot Create Or Modify Host Path Volume Mount"
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "This detection monitors for pod creation with a hostPath volume mount. The attachment to a node's volume can allow  for privilege escalation through underlying vulnerabilities or it can open up possibilities for data exfiltration  or unauthorized file access. It is very rare to see this being a pod requirement.\n"
     Runbook = "Investigate the reason of adding hostPath volume mount. Advise that it is discouraged practice.  Create ticket if appropriate.\n"
     Reference = "https://linuxhint.com/kubernetes-hostpath-volumes/"
     Reports = {"MITRE ATT&CK": ["TA0001", "TA0002"]}
     Tests = gcpk8_s_pot_create_or_modify_host_path_volume_mount_tests
     SUSPICIOUS_PATHS = [
         "/var/run/docker.sock",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 gcpk8s_pod_using_host_pid_namespace_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="triggers",
@@ -44,15 +44,15 @@
 
 
 class GCPK8sPodUsingHostPIDNamespace(PantherRule):
     RuleID = "GCP.K8s.Pod.Using.Host.PID.Namespace-prototype"
     DisplayName = "GCP K8s Pod Using Host PID Namespace"
     LogTypes = [LogType.GCP_AuditLog]
     Tags = ["GCP", "Optional"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "This detection monitors for any pod creation or modification using the host PID namespace. The Host PID namespace enables a pod and its containers to have direct access and share the same view as of the host’s processes. This can offer a powerful escape hatch to the underlying host."
     Runbook = "Investigate a reason of creating a pod using the host PID namespace. Advise that it is discouraged practice. Create ticket if appropriate."
     Reports = {"MITRE ATT&CK": ["TA0004:T1611", "TA0002:T1610"]}
     Reference = "https://medium.com/snowflake/from-logs-to-detection-using-snowflake-and-panther-to-detect-k8s-threats-d72f70a504d7"
     Tests = gcpk8s_pod_using_host_pid_namespace_tests
     METHODS_TO_CHECK = [
         "io.k8s.core.v1.pods.create",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcpk8_s_privileged_pod_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Privileged Pod Created",
@@ -289,15 +289,15 @@
 ]
 
 
 class GCPK8SPrivilegedPodCreated(PantherRule):
     RuleID = "GCP.K8S.Privileged.Pod.Created-prototype"
     DisplayName = "GCP K8S Privileged Pod Created"
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Alerts when a user creates privileged pod. These particular pods have full access to the host’s namespace and  devices, have the ability to exploit the kernel, have dangerous linux capabilities, and can be a powerful launching  point for further attacks. In the event of a successful container escape where a user is operating with root  privileges, the attacker retains this role on the node.\n"
     Runbook = "Investigate the reason of creating privileged pod. Advise that it is discouraged practice.  Create ticket if appropriate.\n"
     Reference = "https://www.golinuxcloud.com/kubernetes-privileged-pod-examples/"
     Reports = {"MITRE ATT&CK": ["TA0004:T1548"]}
     Tests = gcpk8_s_privileged_pod_created_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py` & `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.gcp_base_helpers import gcp_alert_context
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.log_types import LogType
 
 gcpk8_s_service_type_node_port_deployed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Service Created",
@@ -220,15 +220,15 @@
 ]
 
 
 class GCPK8SServiceTypeNodePortDeployed(PantherRule):
     RuleID = "GCP.K8S.Service.Type.NodePort.Deployed-prototype"
     DisplayName = "GCP K8S Service Type NodePort Deployed"
     LogTypes = [LogType.GCP_AuditLog]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "This detection monitors for any kubernetes service deployed with type node port. A Node Port service allows  an attacker to expose a set of pods hosting the service to the internet by opening their port and redirecting  traffic here. This can be used to bypass network controls and intercept traffic, creating a direct line to  the outside network.\n"
     Runbook = "Investigate the reason of creating NodePort service. Advise that it is discouraged practice.  Create ticket if appropriate.\n"
     Reference = "https://kubernetes.io/docs/tutorials/kubernetes-basics/expose/expose-intro/"
     Reports = {"MITRE ATT&CK": ["T1190"]}
     Tests = gcpk8_s_service_type_node_port_deployed_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_action_failed.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_action_failed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import List
 from unittest.mock import MagicMock
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get, github_alert_context
 from pypanther.log_types import LogType
 
 git_hub_action_failed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Branch Protection Disabled",
         ExpectedResult=False,
@@ -86,15 +86,15 @@
 
 class GitHubActionFailed(PantherRule):
     RuleID = "GitHub.Action.Failed-prototype"
     DisplayName = "GitHub Action Failed"
     Enabled = False
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Configuration Required"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A monitored github action has failed."
     Runbook = "Inspect the action failure link and take appropriate response. There are no general plans of response for this activity.\n"
     Reference = "https://docs.github.com/en/actions/creating-actions/setting-exit-codes-for-actions#about-exit-codes"
     Tests = git_hub_action_failed_tests
     # The keys for MONITORED_ACTIONS are gh_org/repo_name
     # The values for MONITORED_ACTIONS are a list of ["action_names"]
     MONITORED_ACTIONS = {}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_advanced_security_change.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_advanced_security_change.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import github_alert_context
 from pypanther.log_types import LogType
 
 git_hub_advanced_security_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Secret Scanning Disabled on a Repo",
         ExpectedResult=True,
@@ -154,15 +154,15 @@
 
 class GitHubAdvancedSecurityChange(PantherRule):
     RuleID = "GitHub.Advanced.Security.Change-prototype"
     DisplayName = "GitHub Security Change, includes GitHub Advanced Security"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = (
         "The rule alerts when GitHub Security tools (Dependabot, Secret Scanner, etc) are disabled."
     )
     Runbook = "Confirm with GitHub administrators and re-enable the tools as applicable."
     Reference = "https://docs.github.com/en/code-security/getting-started/auditing-security-alerts"
     Tests = git_hub_advanced_security_change_tests
     # List of actions in markdown format
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_branch_policy_override.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_branch_policy_override.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_branch_policy_override_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Branch Protection Policy Override",
         ExpectedResult=True,
         Log={
@@ -33,15 +33,15 @@
 
 class GitHubBranchPolicyOverride(PantherRule):
     RuleID = "GitHub.Branch.PolicyOverride-prototype"
     DisplayName = "GitHub Branch Protection Policy Override"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Initial Access:Supply Chain Compromise"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Bypassing branch protection controls could indicate malicious use of admin credentials in an attempt to hide activity."
     Runbook = "Verify that the GitHub admin performed this activity and validate its use."
     Reference = "https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule"
     Tests = git_hub_branch_policy_override_tests
 
     def rule(self, event):
         return event.get("action") == "protected_branch.policy_override"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_branch_protection_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_branch_protection_disabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_branch_protection_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Branch Protection Disabled",
         ExpectedResult=True,
         Log={
@@ -33,15 +33,15 @@
 
 class GitHubBranchProtectionDisabled(PantherRule):
     RuleID = "GitHub.Branch.ProtectionDisabled-prototype"
     DisplayName = "GitHub Branch Protection Disabled"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Initial Access:Supply Chain Compromise"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Disabling branch protection controls could indicate malicious use of admin credentials in an attempt to hide activity."
     Runbook = "Verify that branch protection should be disabled on the repository and re-enable as necessary."
     Reference = "https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule"
     Tests = git_hub_branch_protection_disabled_tests
 
     def rule(self, event):
         return event.get("action") == "protected_branch.destroy"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_auth_modified.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_auth_modified.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_org_auth_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Authentication Method Changed",
         ExpectedResult=True,
         Log={
@@ -33,15 +33,15 @@
 
 class GitHubOrgAuthChange(PantherRule):
     RuleID = "GitHub.Org.AuthChange-prototype"
     DisplayName = "GitHub Org Authentication Method Changed"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Persistence:Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     SummaryAttributes = ["actor", "action"]
     Description = "Detects changes to GitHub org authentication changes."
     Runbook = "Verify that the GitHub admin performed this activity and validate its use."
     Reference = "https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github"
     Tests = git_hub_org_auth_change_tests
     AUTH_CHANGE_EVENTS = [
         "org.saml_disabled",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_ip_allowlist.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_ip_allowlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_org_ip_allowlist_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - IP Allow list modified",
         ExpectedResult=True,
         Log={
@@ -42,15 +42,15 @@
 
 class GitHubOrgIpAllowlist(PantherRule):
     RuleID = "GitHub.Org.IpAllowlist-prototype"
     DisplayName = "GitHub Org IP Allow List modified"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Persistence:Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     SummaryAttributes = ["actor", "action"]
     Description = "Detects changes to a GitHub Org IP Allow List"
     Runbook = "Verify that the change was authorized and appropriate."
     Reference = "https://docs.github.com/en/apps/maintaining-github-apps/managing-allowed-ip-addresses-for-a-github-app"
     Tests = git_hub_org_ip_allowlist_tests
     ALLOWLIST_ACTIONS = [
         "ip_allow_list.enable",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_moderators_add.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_moderators_add.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import github_alert_context
 from pypanther.log_types import LogType
 
 git_hub_org_moderators_add_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Org Moderator Added",
         ExpectedResult=True,
@@ -37,15 +37,15 @@
 
 
 class GitHubOrgModeratorsAdd(PantherRule):
     RuleID = "GitHub.Org.Moderators.Add-prototype"
     DisplayName = "GitHub User Added to Org Moderators"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Initial Access:Supply Chain Compromise"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when a user is added to a GitHub org's list of moderators."
     Reference = "https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/managing-moderators-in-your-organization"
     Tests = git_hub_org_moderators_add_tests
 
     def rule(self, event):
         return event.get("action") == "organization_moderators.add_user"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_modified.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_org_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Team Deleted",
         ExpectedResult=False,
         Log={
@@ -47,15 +47,15 @@
 class GitHubOrgModified(PantherRule):
     RuleID = "GitHub.Org.Modified-prototype"
     DisplayName = "GitHub User Added or Removed from Org"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Initial Access:Supply Chain Compromise"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195"]}
     Reference = "https://docs.github.com/en/organizations/managing-membership-in-your-organization"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "Detects when a user is added or removed from a GitHub Org."
     Tests = git_hub_org_modified_tests
 
     def rule(self, event):
         return event.get("action") == "org.add_member" or event.get("action") == "org.remove_member"
 
     def title(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_organization_app_integration_installed.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_organization_app_integration_installed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import github_alert_context
 from pypanther.log_types import LogType
 
 github_organization_app_integration_installed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="App Integration Installation",
         ExpectedResult=True,
@@ -50,15 +50,15 @@
 
 
 class GithubOrganizationAppIntegrationInstalled(PantherRule):
     Description = "An application integration was installed to your organization's Github account by someone in your organization."
     DisplayName = "Github Organization App Integration Installed"
     Reference = "https://docs.github.com/en/enterprise-server@3.4/developers/apps/managing-github-apps/installing-github-apps"
     Runbook = "Confirm that the app integration installation was a desired behavior."
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Tags = ["Application Installation", "Github"]
     LogTypes = [LogType.GitHub_Audit]
     RuleID = "Github.Organization.App.Integration.Installed-prototype"
     SummaryAttributes = ["actor", "name"]
     Tests = github_organization_app_integration_installed_tests
     # def dedup(event):
     #  (Optional) Return a string which will be used to deduplicate similar alerts.
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_public_repository_created.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_public_repository_created.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import github_alert_context
 from pypanther.log_types import LogType
 
 github_public_repository_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Public Repo Created",
         ExpectedResult=True,
@@ -41,15 +41,15 @@
 class GithubPublicRepositoryCreated(PantherRule):
     Description = "A public Github repository was created."
     DisplayName = "Github Public Repository Created"
     Runbook = (
         "Confirm this github repository was intended to be created as 'public' versus 'private'."
     )
     Reference = "https://docs.github.com/en/get-started/quickstart/create-a-repo"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Tags = ["Github Repository", "Public", "Repository Created"]
     LogTypes = [LogType.GitHub_Audit]
     RuleID = "Github.Public.Repository.Created-prototype"
     SummaryAttributes = ["actor", "repository", "visibility"]
     Tests = github_public_repository_created_tests
     # def dedup(event):
     #  (Optional) Return a string which will be used to deduplicate similar alerts.
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_collaborator_change.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_collaborator_change.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 github_repo_collaborator_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Collaborator Added",
         ExpectedResult=True,
         Log={
@@ -48,15 +48,15 @@
 
 class GithubRepoCollaboratorChange(PantherRule):
     RuleID = "Github.Repo.CollaboratorChange-prototype"
     DisplayName = "GitHub Repository Collaborator Change"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Initial Access:Supply Chain Compromise"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when a repository collaborator is added or removed."
     Runbook = "Determine if the new collaborator is authorized to access the repository."
     Reference = "https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/managing-an-individuals-access-to-an-organization-repository"
     Tests = github_repo_collaborator_change_tests
 
     def rule(self, event):
         return event.get("action") in ("repo.add_member", "repo.remove_member")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_created.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_created.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 github_repo_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Repo Created",
         ExpectedResult=True,
         Log={
@@ -33,15 +33,15 @@
 
 class GithubRepoCreated(PantherRule):
     RuleID = "Github.Repo.Created-prototype"
     DisplayName = "GitHub Repository Created"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub"]
     Reference = "https://docs.github.com/en/get-started/quickstart/create-a-repo"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "Detects when a repository is created."
     Tests = github_repo_created_tests
 
     def rule(self, event):
         return event.get("action") == "repo.create"
 
     def title(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_hook_modified.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_hook_modified.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_repo_hook_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Webhook Created",
         ExpectedResult=True,
         Log={
@@ -51,15 +51,15 @@
 class GitHubRepoHookModified(PantherRule):
     RuleID = "GitHub.Repo.HookModified-prototype"
     DisplayName = "GitHub Web Hook Modified"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Exfiltration:Automated Exfiltration"]
     Reports = {"MITRE ATT&CK": ["TA0010:T1020"]}
     Reference = "https://docs.github.com/en/webhooks/about-webhooks"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "Detects when a web hook is added, modified, or deleted in an org repository."
     Tests = git_hub_repo_hook_modified_tests
 
     def rule(self, event):
         return event.get("action").startswith("hook.")
 
     def title(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_initial_access.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_initial_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from panther_detection_helpers.caching import get_string_set, put_string_set
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.log_types import LogType
 
 git_hub_repo_initial_access_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Initial Access",
         ExpectedResult=True,
         Mocks=[
@@ -88,15 +88,15 @@
 
 class GitHubRepoInitialAccess(PantherRule):
     RuleID = "GitHub.Repo.InitialAccess-prototype"
     DisplayName = "GitHub User Initial Access to Private Repo"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub"]
     Reference = "https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/managing-an-individuals-access-to-an-organization-repository"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "Detects when a user initially accesses a private organization repository."
     Tests = git_hub_repo_initial_access_tests
     CODE_ACCESS_ACTIONS = ["git.clone", "git.push", "git.fetch"]
 
     def rule(self, event):
         # if the actor field is empty, short circuit the rule
         if not event.udm("actor_user"):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_visibility_change.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_visibility_change.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 github_repo_visibility_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Repo Visibility Change",
         ExpectedResult=True,
         Log={
@@ -34,15 +34,15 @@
 class GithubRepoVisibilityChange(PantherRule):
     RuleID = "Github.Repo.VisibilityChange-prototype"
     DisplayName = "GitHub Repository Visibility Change"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Exfiltration:Exfiltration Over Web Service"]
     Reports = {"MITRE ATT&CK": ["TA0010:T1567"]}
     Reference = "https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/setting-repository-visibility"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when an organization repository visibility changes."
     Tests = github_repo_visibility_change_tests
 
     def rule(self, event):
         return event.get("action") == "repo.access"
 
     def title(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repository_transfer.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repository_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import github_alert_context
 from pypanther.log_types import LogType
 
 github_repository_transfer_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Public Repo Created",
         ExpectedResult=False,
@@ -69,15 +69,15 @@
 
 
 class GithubRepositoryTransfer(PantherRule):
     Description = "A user accepted a request to receive a transferred Github repository, a  Github repository was transferred to another repository network, or a user sent a request to transfer a repository to another user or organization."
     DisplayName = "Github Repository Transfer"
     Reference = "https://docs.github.com/en/enterprise-server@3.3/repositories/creating-and-managing-repositories/transferring-a-repository\n\nhttps://docs.github.com/en/enterprise-cloud@latest/admin/monitoring-activity-in-your-enterprise/reviewing-audit-logs-for-your-enterprise/audit-log-events-for-your-enterprise#repo-category-actions"
     Runbook = "Please check with the referenced users or their supervisors to ensure the transferring of this repository is expected and allowed."
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Tags = ["Github Repository", "Github Repository Transfer", "Repository", "Transfer"]
     LogTypes = [LogType.GitHub_Audit]
     RuleID = "Github.Repository.Transfer-prototype"
     SummaryAttributes = ["action"]
     Tests = github_repository_transfer_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_secret_scanning_alert_created.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_secret_scanning_alert_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_secret_scanning_alert_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="secret_scanning_alert.create-true",
         ExpectedResult=True,
         Log={
@@ -56,15 +56,15 @@
 
 class GitHubSecretScanningAlertCreated(PantherRule):
     RuleID = "GitHub.Secret.Scanning.Alert.Created-prototype"
     DisplayName = "GitHub Secret Scanning Alert Created"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1552"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "GitHub detected a secret and created a secret scanning alert."
     Runbook = "Review the secret to determine if it needs to be revoked or the alert suppressed."
     Reference = "https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning"
     Tests = git_hub_secret_scanning_alert_created_tests
 
     def rule(self, event):
         return event.get("action", "") == "secret_scanning_alert.create"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_team_modified.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_team_modified.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_team_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Team Deleted",
         ExpectedResult=True,
         Log={
@@ -49,15 +49,15 @@
 class GitHubTeamModified(PantherRule):
     RuleID = "GitHub.Team.Modified-prototype"
     DisplayName = "GitHub Team Modified"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Initial Access:Supply Chain Compromise"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195"]}
     Reference = "https://docs.github.com/en/organizations/organizing-members-into-teams"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "Detects when a team is modified in some way, such as adding a new team, deleting a team, modifying members, or a change in repository control."
     Tests = git_hub_team_modified_tests
 
     def rule(self, event):
         if not event.get("action").startswith("team"):
             return False
         return (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_user_access_key_created.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_user_access_key_created.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_user_access_key_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - User Access Key Created",
         ExpectedResult=True,
         Log={
@@ -32,15 +32,15 @@
 class GitHubUserAccessKeyCreated(PantherRule):
     RuleID = "GitHub.User.AccessKeyCreated-prototype"
     DisplayName = "GitHub User Access Key Created"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Persistence:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1078"]}
     Reference = "https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "Detects when a GitHub user access key is created."
     Tests = git_hub_user_access_key_created_tests
 
     def rule(self, event):
         return event.get("action") == "public_key.create"
 
     def title(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/github_rules/github_user_role_updated.py` & `pypanther-0.1.1a8/pypanther/rules/github_rules/github_user_role_updated.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_hub_user_role_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Member Updated",
         ExpectedResult=True,
         Log={
@@ -34,15 +34,15 @@
 class GitHubUserRoleUpdated(PantherRule):
     RuleID = "GitHub.User.RoleUpdated-prototype"
     DisplayName = "GitHub User Role Updated"
     LogTypes = [LogType.GitHub_Audit]
     Tags = ["GitHub", "Persistence:Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Reference = "https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "Detects when a GitHub user role is upgraded to an admin or downgraded to a member"
     )
     Tests = git_hub_user_role_updated_tests
 
     def rule(self, event):
         return event.get("action") == "org.update_member"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py` & `pypanther-0.1.1a8/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 git_lab_audit_password_reset_multiple_emails_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="not a password reset",
         ExpectedResult=False,
         Log={"detail": {"custom_message": "hello world"}},
@@ -35,15 +35,15 @@
 
 class GitLabAuditPasswordResetMultipleEmails(PantherRule):
     RuleID = "GitLab.Audit.Password.Reset.Multiple.Emails-prototype"
     DisplayName = "CVE-2023-7028 - GitLab Audit Password Reset Multiple Emails"
     LogTypes = [LogType.GitLab_Audit]
     Tags = ["GitLab", "CVE-2023-7028"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195", "TA0001:T1190", "TA0003:T1098"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Attackers are exploiting a Critical (CVSS 10.0) GitLab vulnerability in which user account password reset emails could be delivered to an unverified email address."
     Reference = "https://about.gitlab.com/releases/2024/01/11/critical-security-release-gitlab-16-7-2-released/"
     Tests = git_lab_audit_password_reset_multiple_emails_tests
 
     def rule(self, event):
         custom_message = event.deep_get("detail", "custom_message", default="")
         emails_raw = event.deep_get("detail", "target_details", default="")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py` & `pypanther-0.1.1a8/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from panther_core.immutable import ImmutableList
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 git_lab_production_password_reset_multiple_emails_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="not a password reset",
         ExpectedResult=False,
@@ -45,15 +45,15 @@
 
 class GitLabProductionPasswordResetMultipleEmails(PantherRule):
     RuleID = "GitLab.Production.Password.Reset.Multiple.Emails-prototype"
     DisplayName = "CVE-2023-7028 - GitLab Production Password Reset Multiple Emails"
     LogTypes = [LogType.GitLab_Production]
     Tags = ["GitLab", "CVE-2023-7028"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195", "TA0001:T1190", "TA0003:T1098"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Attackers are exploiting a Critical (CVSS 10.0) GitLab vulnerability in which user account password reset emails could be delivered to an unverified email address."
     Reference = "https://about.gitlab.com/releases/2024/01/11/critical-security-release-gitlab-16-7-2-released/"
     Tests = git_lab_production_password_reset_multiple_emails_tests
 
     def rule(self, event):
         path = event.get("path", default="")
         if path != "/users/password":
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_auth_errors_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="SSH Errors",
         ExpectedResult=True,
         Log={
@@ -44,15 +44,15 @@
 
 
 class TeleportAuthErrors(PantherRule):
     RuleID = "Teleport.AuthErrors-prototype"
     DisplayName = "Teleport SSH Auth Errors"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["SSH", "Credential Access:Brute Force"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
     Description = "A high volume of SSH errors could indicate a brute-force attack"
     Threshold = 10
     DedupPeriodMinutes = 15
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "Check that the user making the failed requests legitimately tried logging in that many times.\n"
     SummaryAttributes = [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_config import config
 from pypanther.log_types import LogType
 
 teleport_company_domain_login_without_saml_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="A User from the company domain(s) logged in with SAML",
         ExpectedResult=False,
@@ -41,15 +41,15 @@
 
 
 class TeleportCompanyDomainLoginWithoutSAML(PantherRule):
     RuleID = "Teleport.CompanyDomainLoginWithoutSAML-prototype"
     DisplayName = "A User from the company domain(s) Logged in without SAML"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["Teleport"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A User from the company domain(s) Logged in without SAML"
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "A User from the company domain(s) Logged in without SAML\n"
     SummaryAttributes = ["event", "code", "user", "method", "mfa_device"]
     Tests = teleport_company_domain_login_without_saml_tests
     TELEPORT_ORGANIZATION_DOMAINS_REGEX = (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import pattern_match_list
 from pypanther.log_types import LogType
 
 teleport_create_user_accounts_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Echo command",
         ExpectedResult=False,
@@ -56,15 +56,15 @@
 
 class TeleportCreateUserAccounts(PantherRule):
     RuleID = "Teleport.CreateUserAccounts-prototype"
     DisplayName = "Teleport Create User Accounts"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["SSH", "Persistence:Create Account"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1136"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A user has been manually created, modified, or deleted"
     DedupPeriodMinutes = 15
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "Analyze why it was manually created and delete it if necessary."
     SummaryAttributes = [
         "event",
         "code",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_local_user_login_without_mfa_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User logged in with MFA",
         ExpectedResult=False,
         Log={
@@ -47,15 +47,15 @@
 
 
 class TeleportLocalUserLoginWithoutMFA(PantherRule):
     RuleID = "Teleport.LocalUserLoginWithoutMFA-prototype"
     DisplayName = "User Logged in wihout MFA"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["Teleport"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A local User logged in without MFA"
     Reports = {"MITRE ATT&CK": ["TA0001:T1078"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "A local user logged in without Multi-Factor Authentication\n"
     SummaryAttributes = ["event", "code", "user", "success", "mfa_device"]
     Tests = teleport_local_user_login_without_mfa_tests
     SENSITIVE_LOCAL_USERS = ["breakglass"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_lock_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="A Lock was created",
         ExpectedResult=True,
         Log={
@@ -25,15 +25,15 @@
 
 
 class TeleportLockCreated(PantherRule):
     RuleID = "Teleport.LockCreated-prototype"
     DisplayName = "A Teleport Lock was created"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["Teleport"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A Teleport Lock was created"
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "A Teleport Lock was created; this is an unusual administrative action. Investigate to understand why a Lock was created.\n"
     SummaryAttributes = ["event", "code", "time", "identity"]
     Tests = teleport_lock_created_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime, timedelta
 from typing import Dict, List, Tuple
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import (
     golang_nanotime_to_python_datetime,
     panther_nanotime_to_python_datetime,
 )
 from pypanther.log_types import LogType
 
 teleport_long_lived_certs_tests: List[PantherRuleTest] = [
@@ -73,15 +73,15 @@
 
 
 class TeleportLongLivedCerts(PantherRule):
     RuleID = "Teleport.LongLivedCerts-prototype"
     DisplayName = "A long-lived cert was created"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["Teleport"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An unusually long-lived Teleport certificate was created"
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "Teleport certificates are usually issued for a short period of time. Alert if long-lived certificates were created.\n"
     SummaryAttributes = ["event", "code", "time", "identity"]
     Tests = teleport_long_lived_certs_tests
     PANTHER_TIME_FORMAT = "%Y-%m-%d %H:%M:%S.%f"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_network_scanning_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Echo command",
         ExpectedResult=False,
         Log={
@@ -100,15 +100,15 @@
 
 
 class TeleportNetworkScanning(PantherRule):
     RuleID = "Teleport.NetworkScanning-prototype"
     DisplayName = "Teleport Network Scan Initiated"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["SSH", "Discovery:Network Service Discovery"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A user has invoked a network scan that could potentially indicate enumeration of the network."
     Reports = {"MITRE ATT&CK": ["TA0007:T1046"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "Find related commands within the time window and determine if the command was invoked legitimately. Examine the arguments to determine how the command was used.\n"
     SummaryAttributes = [
         "event",
         "code",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_role_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="A role was created",
         ExpectedResult=True,
         Log={
@@ -23,15 +23,15 @@
 
 
 class TeleportRoleCreated(PantherRule):
     RuleID = "Teleport.RoleCreated-prototype"
     DisplayName = "A Teleport Role was modified or created"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["Teleport"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Teleport Role was modified or created"
     Reports = {"MITRE ATT&CK": ["TA0003:T1098.001"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "A Teleport Role was modified or created. Validate its legitimacy.\n"
     SummaryAttributes = ["event", "code", "user", "name"]
     Tests = teleport_role_created_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_root_login_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User logged in as root",
         ExpectedResult=True,
         Log={
@@ -32,15 +32,15 @@
 
 
 class TeleportRootLogin(PantherRule):
     RuleID = "Teleport.RootLogin-prototype"
     DisplayName = "User Logged in as root"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["SSH", "Execution:Command and Scripting Interpreter", "Teleport"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A User logged in as root"
     Reports = {"MITRE ATT&CK": ["TA0002:T1059"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "Use user accounts and policies, rather than root when logging in. With access to root, it is possible to evade auditing and logging.\n"
     SummaryAttributes = ["event", "code", "user", "login", "server_hostname", "server_labels"]
     Tests = teleport_root_login_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_saml_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="SAML Auth Connector modified",
         ExpectedResult=True,
         Log={
@@ -22,15 +22,15 @@
 
 
 class TeleportSAMLCreated(PantherRule):
     RuleID = "Teleport.SAMLCreated-prototype"
     DisplayName = "A SAML Connector was created or modified"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["Teleport"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A SAML connector was created or modified"
     Reports = {"MITRE ATT&CK": ["TA0042:T1585"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "When a SAML connector is modified, it can potentially change the trust model of the Teleport Cluster. Validate that these changes were expected and correct.\n"
     SummaryAttributes = ["event", "code", "user", "name"]
     Tests = teleport_saml_created_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_config import config
 from pypanther.log_types import LogType
 
 teleport_saml_login_without_company_domain_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="A user authenticated with SAML, but from a known company domain",
         ExpectedResult=False,
@@ -41,15 +41,15 @@
 
 
 class TeleportSAMLLoginWithoutCompanyDomain(PantherRule):
     RuleID = "Teleport.SAMLLoginWithoutCompanyDomain-prototype"
     DisplayName = "A user authenticated with SAML, but from an unknown company domain"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["Teleport"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A user authenticated with SAML, but from an unknown company domain"
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "A user authenticated with SAML, but from an unknown company domain\n"
     SummaryAttributes = ["event", "code", "user", "method", "mfa_device"]
     Tests = teleport_saml_login_without_company_domain_tests
     TELEPORT_COMPANY_DOMAINS_REGEX = "@(" + "|".join(config.TELEPORT_ORGANIZATION_DOMAINS) + ")$"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_scheduled_jobs_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Crontab no args",
         ExpectedResult=True,
         Log={
@@ -100,15 +100,15 @@
 
 
 class TeleportScheduledJobs(PantherRule):
     RuleID = "Teleport.ScheduledJobs-prototype"
     DisplayName = "Teleport Scheduled Jobs"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["SSH", "Execution:Scheduled Task/Job"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0002:T1053"]}
     Description = "A user has manually edited the Linux crontab"
     Threshold = 10
     DedupPeriodMinutes = 15
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "Validate the user behavior and rotate the host if necessary."
     SummaryAttributes = [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py` & `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 teleport_suspicious_commands_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Echo command",
         ExpectedResult=False,
         Log={
@@ -54,15 +54,15 @@
 
 
 class TeleportSuspiciousCommands(PantherRule):
     RuleID = "Teleport.SuspiciousCommands-prototype"
     DisplayName = "Teleport Suspicious Commands Executed"
     LogTypes = [LogType.Gravitational_TeleportAudit]
     Tags = ["SSH", "Execution:Command and Scripting Interpreter"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A user has invoked a suspicious command that could lead to a host compromise"
     Reports = {"MITRE ATT&CK": ["TA0002:T1059"]}
     Reference = "https://goteleport.com/docs/management/admin/"
     Runbook = "Find related commands within the time window and determine if the command was invoked legitimately. Examine the arguments to determine how the command was used and reach out to the user to verify the intentions.\n"
     SummaryAttributes = [
         "event",
         "code",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 google_workspace_admin_custom_role_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Delete Role",
         ExpectedResult=False,
         Log={
@@ -76,15 +76,15 @@
 
 
 class GoogleWorkspaceAdminCustomRole(PantherRule):
     Description = "A Google Workspace administrator created a new custom administrator role."
     DisplayName = "Google Workspace Admin Custom Role"
     Runbook = "Please review this activity with the administrator and ensure this behavior was authorized."
     Reference = "https://support.google.com/a/answer/2406043?hl=en#:~:text=under%20the%20limit.-,Create%20a%20custom%20role,-Before%20you%20begin"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Tags = ["admin", "administrator", "google workspace", "role"]
     LogTypes = [LogType.GSuite_ActivityEvent]
     RuleID = "Google.Workspace.Admin.Custom.Role-prototype"
     SummaryAttributes = ["name", "type"]
     Tests = google_workspace_admin_custom_role_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 google_workspace_advanced_protection_program_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="parameters json key set to null value",
         ExpectedResult=False,
@@ -131,15 +131,15 @@
 class GoogleWorkspaceAdvancedProtectionProgram(PantherRule):
     Description = (
         "Your organization's Google Workspace Advanced Protection Program settings were modified."
     )
     DisplayName = "Google Workspace Advanced Protection Program"
     Runbook = "Confirm the changes made were authorized for your organization."
     Reference = "https://support.google.com/a/answer/9378686?hl=en"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.GSuite_ActivityEvent]
     RuleID = "Google.Workspace.Advanced.Protection.Program-prototype"
     Tests = google_workspace_advanced_protection_program_tests
 
     def rule(self, event):
         # Return True to match the log event and trigger an alert.
         setting_name = (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 google_workspace_apps_marketplace_allowlist_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="parameters json key set to null value",
         ExpectedResult=False,
@@ -127,15 +127,15 @@
 
 
 class GoogleWorkspaceAppsMarketplaceAllowlist(PantherRule):
     Description = "Google Workspace Marketplace application allowlist settings were modified."
     DisplayName = "Google Workspace Apps Marketplace Allowlist"
     Runbook = "Confirm with the acting user that this change was authorized."
     Reference = "https://support.google.com/a/answer/6089179?hl=en"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.GSuite_ActivityEvent]
     RuleID = "Google.Workspace.Apps.Marketplace.Allowlist-prototype"
     Tests = google_workspace_apps_marketplace_allowlist_tests
 
     def rule(self, event):
         # Return True to match the log event and trigger an alert.
         setting_name = deep_get(event, "parameters", "SETTING_NAME", default="<NO_SETTING_NAME>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 google_workspace_apps_marketplace_new_domain_application_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Change Email Setting Default",
         ExpectedResult=False,
         Log={
@@ -105,15 +105,15 @@
 
 
 class GoogleWorkspaceAppsMarketplaceNewDomainApplication(PantherRule):
     Description = "A Google Workspace User configured a new domain application from the Google Workspace Apps Marketplace."
     DisplayName = "Google Workspace Apps Marketplace New Domain Application"
     Runbook = "Confirm this was the intended behavior."
     Reference = "https://developers.google.com/workspace/marketplace/overview"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.GSuite_ActivityEvent]
     RuleID = "Google.Workspace.Apps.Marketplace.New.Domain.Application-prototype"
     Tests = google_workspace_apps_marketplace_new_domain_application_tests
 
     def rule(self, event):
         # Return True to match the log event and trigger an alert.
         return (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 google_workspace_apps_new_mobile_app_installed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Android Calculator",
         ExpectedResult=True,
         Log={
@@ -87,15 +87,15 @@
 
 
 class GoogleWorkspaceAppsNewMobileAppInstalled(PantherRule):
     Description = "A new mobile application was added to your organization's mobile apps whitelist in Google Workspace Apps."
     DisplayName = "Google Workspace Apps New Mobile App Installed"
     Runbook = "https://admin.google.com/ac/apps/unified"
     Reference = "https://support.google.com/a/answer/6089179?hl=en"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.GSuite_ActivityEvent]
     RuleID = "Google.Workspace.Apps.New.Mobile.App.Installed-prototype"
     Tests = google_workspace_apps_new_mobile_app_installed_tests
 
     def rule(self, event):
         # Return True to match the log event and trigger an alert.
         return event.get("name", "") == "ADD_MOBILE_APPLICATION_TO_WHITELIST"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_advanced_protection_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Advanced Protection Enabled",
         ExpectedResult=False,
@@ -30,15 +30,15 @@
 
 class GSuiteAdvancedProtection(PantherRule):
     RuleID = "GSuite.AdvancedProtection-prototype"
     DisplayName = "GSuite User Advanced Protection Change"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite", "Defense Evasion:Impair Defenses"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A user disabled advanced protection for themselves.\n"
     Reference = "https://support.google.com/a/answer/9378686?hl=en&sjid=864417124752637253-EU"
     Runbook = "Have the user re-enable Google Advanced Protection\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_advanced_protection_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_calendar_made_public_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User Publically Shared a Calendar",
         ExpectedResult=True,
@@ -116,15 +116,15 @@
 
 class GSuiteCalendarMadePublic(PantherRule):
     RuleID = "GSuite.CalendarMadePublic-prototype"
     DisplayName = "GSuite Calendar Has Been Made Public"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
     Reports = {"MITRE ATT&CK": ["TA0007:T1087"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A User or Admin Has Modified A Calendar To Be Public\n"
     Reference = "https://support.google.com/calendar/answer/37083?hl=en&sjid=864417124752637253-EU"
     Runbook = "Follow up with user about this calendar share.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_calendar_made_public_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_config import config
 from pypanther.log_types import LogType
 
 g_suite_doc_ownership_transfer_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Ownership Transferred Within Organization",
@@ -30,15 +30,15 @@
 class GSuiteDocOwnershipTransfer(PantherRule):
     RuleID = "GSuite.DocOwnershipTransfer-prototype"
     DisplayName = "GSuite Document External Ownership Transfer"
     Enabled = False
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite", "Configuration Required", "Collection:Data from Information Repositories"]
     Reports = {"MITRE ATT&CK": ["TA0009:T1213"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A GSuite document's ownership was transferred to an external party.\n"
     Reference = "https://support.google.com/drive/answer/2494892?hl=en&co=GENIE.Platform%3DDesktop&sjid=864417124752637253-EU"
     Runbook = (
         "Verify that this document did not contain sensitive or private company information.\n"
     )
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_doc_ownership_transfer_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_config import config
 from pypanther.log_types import LogType
 
 g_suite_external_mail_forwarding_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Forwarding to External Address",
@@ -76,15 +76,15 @@
 class GSuiteExternalMailForwarding(PantherRule):
     RuleID = "GSuite.ExternalMailForwarding-prototype"
     DisplayName = "Gsuite Mail forwarded to external domain"
     Enabled = False
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite", "Collection:Email Collection", "Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0009:T1114"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A user has configured mail forwarding to an external domain\n"
     Reference = "https://support.google.com/mail/answer/10957?hl=en&sjid=864417124752637253-EU"
     Runbook = "Follow up with user to remove this forwarding rule if not allowed.\n"
     SummaryAttributes = ["p_any_emails"]
     Tests = g_suite_external_mail_forwarding_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_google_access_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
@@ -19,15 +19,15 @@
 
 
 class GSuiteGoogleAccess(PantherRule):
     RuleID = "GSuite.GoogleAccess-prototype"
     DisplayName = "Google Accessed a GSuite Resource"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Google accessed one of your GSuite resources directly, most likely in response to a support incident.\n"
     Reference = "https://support.google.com/a/answer/9230474?hl=en"
     Runbook = "Your GSuite Super Admin can visit the Access Transparency report in the GSuite Admin Dashboard to see more details about the access.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_google_access_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_government_backed_attack_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
@@ -31,15 +31,15 @@
 
 
 class GSuiteGovernmentBackedAttack(PantherRule):
     RuleID = "GSuite.GovernmentBackedAttack-prototype"
     DisplayName = "GSuite Government Backed Attack"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Description = (
         "GSuite reported that it detected a government backed attack against your account.\n"
     )
     Reference = "https://support.google.com/a/answer/9007870?hl=en"
     Runbook = "Followup with GSuite support for more details.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_government_backed_attack_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_group_banned_user_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User Added",
         ExpectedResult=False,
@@ -29,15 +29,15 @@
 
 
 class GSuiteGroupBannedUser(PantherRule):
     RuleID = "GSuite.GroupBannedUser-prototype"
     DisplayName = "GSuite User Banned from Group"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A GSuite user was banned from an enterprise group by moderator action.\n"
     Reference = "https://support.google.com/a/users/answer/9303224?hl=en&sjid=864417124752637253-EU"
     Runbook = (
         "Investigate the banned user to see if further disciplinary action needs to be taken.\n"
     )
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_group_banned_user_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_leaked_password_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
@@ -40,15 +40,15 @@
 
 class GSuiteLeakedPassword(PantherRule):
     RuleID = "GSuite.LeakedPassword-prototype"
     DisplayName = "GSuite User Password Leaked"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite", "Credential Access:Unsecured Credentials"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1552"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "GSuite reported a user's password has been compromised, so they disabled the account.\n"
     )
     Reference = "https://support.google.com/a/answer/2984349?hl=en#zippy=%2Cstep-temporarily-suspend-the-suspected-compromised-user-account%2Cstep-investigate-the-account-for-unauthorized-activity%2Cstep-revoke-access-to-the-affected-account%2Cstep-return-access-to-the-user-again%2Cstep-enroll-in--step-verification-with-security-keys%2Cstep-add-secure-or-update-recovery-options%2Cstep-enable-account-activity-alerts"
     Runbook = "GSuite has already disabled the compromised user's account. Consider investigating how the user's account was compromised, and reset their account and password. Advise the user to change any other passwords in use that are the sae as the compromised password.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_leaked_password_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_login_type_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Login With Approved Type",
         ExpectedResult=False,
@@ -62,15 +62,15 @@
 class GSuiteLoginType(PantherRule):
     RuleID = "GSuite.LoginType-prototype"
     DisplayName = "GSuite Login Type"
     Enabled = False
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite", "Configuration Required", "Initial Access:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1078"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A login of a non-approved type was detected for this user.\n"
     Reference = "https://support.google.com/a/answer/9039184?hl=en&sjid=864417124752637253-EU"
     Runbook = (
         "Correct the user account settings so that only logins of approved types are available.\n"
     )
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_login_type_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_device_compromise_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Mobile Event",
         ExpectedResult=False,
@@ -48,15 +48,15 @@
 
 
 class GSuiteDeviceCompromise(PantherRule):
     RuleID = "GSuite.DeviceCompromise-prototype"
     DisplayName = "GSuite User Device Compromised"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "GSuite reported a user's device has been compromised.\n"
     Reference = "https://support.google.com/a/answer/7562165?hl=en&sjid=864417124752637253-EU"
     Runbook = "Have the user change their passwords and reset the device.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_device_compromise_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_device_unlock_failure_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Mobile Event",
         ExpectedResult=False,
@@ -57,15 +57,15 @@
 
 class GSuiteDeviceUnlockFailure(PantherRule):
     RuleID = "GSuite.DeviceUnlockFailure-prototype"
     DisplayName = "GSuite User Device Unlock Failures"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite", "Credential Access:Brute Force"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Someone failed to unlock a user's device multiple times in quick succession.\n"
     Reference = "https://support.google.com/a/answer/6350074?hl=en"
     Runbook = "Verify that these unlock attempts came from the user, and not a malicious actor which has acquired the user's device.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_device_unlock_failure_tests
     MAX_UNLOCK_ATTEMPTS = 10
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_device_suspicious_activity_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Mobile Event",
         ExpectedResult=False,
@@ -31,15 +31,15 @@
 
 
 class GSuiteDeviceSuspiciousActivity(PantherRule):
     RuleID = "GSuite.DeviceSuspiciousActivity-prototype"
     DisplayName = "GSuite Device Suspicious Activity"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "GSuite reported a suspicious activity on a user's device.\n"
     Reference = "https://support.google.com/a/answer/7562460?hl=en&sjid=864417124752637253-EU"
     Runbook = "Validate that the suspicious activity was expected by the user.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_device_suspicious_activity_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_rule_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Non Triggered Rule",
         ExpectedResult=False,
@@ -69,15 +69,15 @@
 
 
 class GSuiteRule(PantherRule):
     RuleID = "GSuite.Rule-prototype"
     DisplayName = "GSuite Passthrough Rule Triggered"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A GSuite rule was triggered.\n"
     Reference = "https://support.google.com/a/answer/9420866"
     Runbook = "Investigate what triggered the rule.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_rule_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_suspicious_logins_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
@@ -42,15 +42,15 @@
 
 
 class GSuiteSuspiciousLogins(PantherRule):
     RuleID = "GSuite.SuspiciousLogins-prototype"
     DisplayName = "Suspicious GSuite Login"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "GSuite reported a suspicious login for this user.\n"
     Reference = "https://support.google.com/a/answer/7102416?hl=en"
     Runbook = "Checkout the details of the login and verify this behavior with the user to ensure the account wasn't compromised.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_suspicious_logins_tests
     SUSPICIOUS_LOGIN_TYPES = {
         "suspicious_login",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_two_step_verification_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Two Step Verification Enabled",
         ExpectedResult=False,
@@ -32,15 +32,15 @@
 
 class GSuiteTwoStepVerification(PantherRule):
     RuleID = "GSuite.TwoStepVerification-prototype"
     DisplayName = "GSuite User Two Step Verification Change"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite", "Defense Evasion:Modify Authentication Process"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1556"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A user disabled two step verification for themselves.\n"
     Reference = "https://support.google.com/mail/answer/185839?hl=en&co=GENIE.Platform%3DDesktop&sjid=864417124752637253-EU"
     Runbook = "Depending on company policy, either suggest or require the user re-enable two step verification.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_two_step_verification_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_user_suspended_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
@@ -42,15 +42,15 @@
 
 
 class GSuiteUserSuspended(PantherRule):
     RuleID = "GSuite.UserSuspended-prototype"
     DisplayName = "GSuite User Suspended"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "A GSuite user was suspended, the account may have been compromised by a spam network.\n"
     )
     Reference = "https://support.google.com/drive/answer/40695?hl=en&sjid=864417124752637253-EU"
     Runbook = "Investigate the behavior that got the account suspended. Verify with the user that this intended behavior. If not, the account may have been compromised.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_user_suspended_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_workspace_calendar_external_sharing_setting_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Admin Set Default Calendar SHARING_OUTSIDE_DOMAIN Setting to READ_ONLY_ACCESS",
         ExpectedResult=True,
@@ -135,15 +135,15 @@
 
 class GSuiteWorkspaceCalendarExternalSharingSetting(PantherRule):
     RuleID = "GSuite.Workspace.CalendarExternalSharingSetting-prototype"
     DisplayName = "GSuite Workspace Calendar External Sharing Setting Change"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
     Reports = {"MITRE ATT&CK": ["TA0007:T1087"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Workspace Admin Changed The Sharing Settings for Primary Calendars\n"
     Reference = "https://support.google.com/a/answer/60765?hl=en"
     Runbook = "Restore the calendar sharing setting to the previous value. If unplanned, use indicator search to identify other activity from this administrator.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_workspace_calendar_external_sharing_setting_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_workspace_data_export_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Workspace Admin Data Export Created",
         ExpectedResult=True,
@@ -107,15 +107,15 @@
 
 
 class GSuiteWorkspaceDataExportCreated(PantherRule):
     RuleID = "GSuite.Workspace.DataExportCreated-prototype"
     DisplayName = "GSuite Workspace Data Export Has Been Created"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Workspace Admin Has Created a Data Export\n"
     Reference = "https://support.google.com/a/answer/100458?hl=en&sjid=864417124752637253-EU"
     Runbook = "Verify the intent of this Data Export. If intent cannot be verified, then a search on the actor's other activities is advised.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_workspace_data_export_created_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_workspace_gmail_default_routing_rule_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Workspace Admin Creates Default Routing Rule",
         ExpectedResult=True,
@@ -116,15 +116,15 @@
 
 class GSuiteWorkspaceGmailDefaultRoutingRuleModified(PantherRule):
     RuleID = "GSuite.Workspace.GmailDefaultRoutingRuleModified-prototype"
     DisplayName = "GSuite Workspace Gmail Default Routing Rule Modified"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A Workspace Admin Has Modified A Default Routing Rule In Gmail\n"
     Reference = "https://support.google.com/a/answer/2368153?hl=en"
     Runbook = "Administrators use Default Routing to set up how inbound email is delivered within an organization. The configuration of the default routing rule needs to be inspected in order to verify the intent of the rule is benign.\nIf this change was not planned, inspect the other actions taken by this actor.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_workspace_gmail_default_routing_rule_modified_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_workspace_gmail_predelivery_scanning_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Workspace Admin Disables Enhanced Pre-Delivery Scanning",
         ExpectedResult=True,
@@ -90,15 +90,15 @@
 
 class GSuiteWorkspaceGmailPredeliveryScanningDisabled(PantherRule):
     RuleID = "GSuite.Workspace.GmailPredeliveryScanningDisabled-prototype"
     DisplayName = "GSuite Workspace Gmail Pre-Delivery Message Scanning Disabled"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1566"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Workspace Admin Has Disabled Pre-Delivery Scanning For Gmail.\n"
     Reference = "https://support.google.com/a/answer/7380368"
     Runbook = "Pre-delivery scanning is a feature in Gmail that subjects suspicious emails to additional automated scrutiny by Google.\nIf this change was not intentional, inspect the other actions taken by this actor.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_workspace_gmail_predelivery_scanning_disabled_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_workspace_gmail_security_sandbox_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Workspace Admin Disables Security Sandbox",
         ExpectedResult=True,
@@ -90,15 +90,15 @@
 
 class GSuiteWorkspaceGmailSecuritySandboxDisabled(PantherRule):
     RuleID = "GSuite.Workspace.GmailSecuritySandboxDisabled-prototype"
     DisplayName = "GSuite Workspace Gmail Security Sandbox Disabled"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1566"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Workspace Admin Has Disabled The Security Sandbox\n"
     Reference = "https://support.google.com/a/answer/7676854?hl=en#zippy=%2Cfind-security-sandbox-settings%2Cabout-security-sandbox-rules-and-other-scans"
     Runbook = "Gmail's Security Sandbox enables rule based scanning of email content.\nIf this change was not intentional, inspect the other actions taken by this actor.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_workspace_gmail_security_sandbox_disabled_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_workspace_password_enforce_strong_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Workspace Admin Disabled Strong Password Enforcement",
         ExpectedResult=True,
@@ -94,15 +94,15 @@
 
 
 class GSuiteWorkspacePasswordEnforceStrongDisabled(PantherRule):
     RuleID = "GSuite.Workspace.PasswordEnforceStrongDisabled-prototype"
     DisplayName = "GSuite Workspace Strong Password Enforcement Has Been Disabled"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
     Description = "A Workspace Admin Has Disabled The Enforcement Of Strong Passwords\n"
     Reference = "https://support.google.com/a/answer/139399?hl=en"
     Runbook = "Verify the intent of this Password Strength Setting Change. If intent cannot be verified, then a search on the actor's other activities is advised.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_workspace_password_enforce_strong_disabled_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_workspace_password_reuse_enabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Workspace Admin Enabled Password Reuse",
         ExpectedResult=True,
@@ -90,15 +90,15 @@
 
 
 class GSuiteWorkspacePasswordReuseEnabled(PantherRule):
     RuleID = "GSuite.Workspace.PasswordReuseEnabled-prototype"
     DisplayName = "GSuite Workspace Password Reuse Has Been Enabled"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
     Description = "A Workspace Admin Has Enabled Password Reuse\n"
     Reference = "https://support.google.com/a/answer/139399?hl=en#"
     Runbook = "Verify the intent of this Password Reuse Setting Change. If intent cannot be verified, then a search on the actor's other activities is advised.\n"
     SummaryAttributes = ["actor:email"]
     Tests = g_suite_workspace_password_reuse_enabled_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 g_suite_workspace_trusted_domains_allowlist_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Workspace Admin Remove Trusted Domain",
         ExpectedResult=True,
@@ -108,15 +108,15 @@
 
 
 class GSuiteWorkspaceTrustedDomainsAllowlist(PantherRule):
     RuleID = "GSuite.Workspace.TrustedDomainsAllowlist-prototype"
     DisplayName = "GSuite Workspace Trusted Domain Allowlist Modified"
     LogTypes = [LogType.GSuite_ActivityEvent]
     Tags = ["GSuite"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Workspace Admin Has Modified The Trusted Domains List\n"
     Reference = "https://support.google.com/a/answer/6160020?hl=en&sjid=864417124752637253-EU"
     Runbook = "Verify the intent of this modification. If intent cannot be verified, then an indicator search on the actor is advised.\n"
     SummaryAttributes = ["actor:email"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Tests = g_suite_workspace_trusted_domains_allowlist_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import (
     PantherUnexpectedAlert,
     deep_get,
     pattern_match,
     pattern_match_list,
 )
 from pypanther.log_types import LogType
@@ -128,15 +128,15 @@
     Tags = [
         "GSuite",
         "Security Control",
         "Configuration Required",
         "Collection:Data from Information Repositories",
     ]
     Reports = {"MITRE ATT&CK": ["TA0009:T1213"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "An employee shared a sensitive file externally with another organization"
     Runbook = "Contact the employee who made the share and make sure they redact the access. If the share was legitimate, add to the EXCEPTION_PATTERNS in the detection.\n"
     Reference = "https://support.google.com/docs/answer/2494822?hl=en&co=GENIE.Platform%3DiOS&sjid=864417124752637253-EU"
     Tests = g_suite_drive_external_file_share_tests
     COMPANY_DOMAIN = "your-company-name.com"
     # The glob pattern for the document title (lowercased)
     # All actors allowed to receive the file share
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_base_helpers import gsuite_details_lookup as details_lookup
 from pypanther.helpers.panther_base_helpers import gsuite_parameter_lookup as param_lookup
 from pypanther.log_types import LogType
 
 g_suite_drive_overly_visible_tests: List[PantherRuleTest] = [
     PantherRuleTest(
@@ -76,15 +76,15 @@
 
 class GSuiteDriveOverlyVisible(PantherRule):
     RuleID = "GSuite.DriveOverlyVisible-prototype"
     DisplayName = "GSuite Overly Visible Drive Document"
     LogTypes = [LogType.GSuite_Reports]
     Tags = ["GSuite", "Collection:Data from Information Repositories"]
     Reports = {"MITRE ATT&CK": ["TA0009:T1213"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A Google drive resource that is overly visible has been modified.\n"
     Reference = "https://support.google.com/docs/answer/2494822?hl=en&co=GENIE.Platform%3DDesktop&sjid=864417124752637253-EU"
     Runbook = "Investigate whether the drive document is appropriate to be this visible.\n"
     SummaryAttributes = ["actor:email"]
     DedupPeriodMinutes = 360
     Tests = g_suite_drive_overly_visible_tests
     RESOURCE_CHANGE_EVENTS = {"create", "move", "upload", "edit"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py` & `pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import List
 from unittest.mock import MagicMock
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_base_helpers import gsuite_parameter_lookup as param_lookup
 from pypanther.log_types import LogType
 
 g_suite_drive_visibility_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Access Event",
@@ -371,15 +371,15 @@
 class GSuiteDriveVisibilityChanged(PantherRule):
     RuleID = "GSuite.DriveVisibilityChanged-prototype"
     DisplayName = "GSuite External Drive Document"
     Enabled = False
     LogTypes = [LogType.GSuite_Reports]
     Tags = ["GSuite", "Collection:Data from Information Repositories", "Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0009:T1213"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A Google drive resource became externally accessible.\n"
     Reference = (
         "https://support.google.com/a/users/answer/12380484?hl=en&sjid=864417124752637253-EU"
     )
     Runbook = "Investigate whether the drive document is appropriate to be publicly accessible.\n"
     SummaryAttributes = ["actor:email"]
     DedupPeriodMinutes = 360
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py` & `pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from datetime import timedelta
 from typing import List
 
 from panther_detection_helpers.caching import put_string_set
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_oss_helpers import resolve_timestamp_string
 from pypanther.log_types import LogType
 
 standard_new_aws_account_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="AWS Account created",
         ExpectedResult=True,
@@ -55,15 +55,15 @@
 
 
 class StandardNewAWSAccountCreated(PantherRule):
     RuleID = "Standard.NewAWSAccountCreated-prototype"
     DisplayName = "New AWS Account Created"
     LogTypes = [LogType.AWS_CloudTrail]
     Tags = ["DataModel", "Indicator Collection", "Persistence:Create Account"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Reports = {"MITRE ATT&CK": ["TA0003:T1136"]}
     Description = "A new AWS account was created"
     Runbook = "A new AWS account was created, ensure it was created through standard practice and is for a valid purpose."
     Reference = "https://docs.aws.amazon.com/organizations/latest/userguide/orgs_security_incident-response.html#:~:text=AWS%20Organizations%20information%20in%20CloudTrail"
     SummaryAttributes = ["p_any_aws_account_ids"]
     Tests = standard_new_aws_account_created_tests
     # Days an account is considered new
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/new_user_account_logging.py` & `pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/new_user_account_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import timedelta
 from typing import List
 
 from panther_detection_helpers.caching import put_string_set
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_oss_helpers import resolve_timestamp_string
 from pypanther.log_types import LogType
 
 standard_new_user_account_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User Creation Event - OneLogin",
         ExpectedResult=True,
@@ -79,15 +79,15 @@
 
 
 class StandardNewUserAccountCreated(PantherRule):
     RuleID = "Standard.NewUserAccountCreated-prototype"
     DisplayName = "New User Account Created"
     LogTypes = [LogType.OneLogin_Events, LogType.AWS_CloudTrail, LogType.Zoom_Operation]
     Tags = ["DataModel", "Indicator Collection", "OneLogin", "Persistence:Create Account"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Reports = {"MITRE ATT&CK": ["TA0003:T1136"]}
     Description = "A new account was created"
     Runbook = "A new user account was created, ensure it was created through standard practice and is for a valid purpose."
     Reference = "https://attack.mitre.org/techniques/T1136/001/"
     SummaryAttributes = ["p_any_usernames"]
     Tests = standard_new_user_account_created_tests
     # Days an account is considered new
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py` & `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import m365_alert_context
 from pypanther.log_types import LogType
 
 microsoft365_brute_force_loginby_user_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Failed Login event",
         ExpectedResult=True,
@@ -89,15 +89,15 @@
 
 class Microsoft365BruteForceLoginbyUser(PantherRule):
     Description = "A Microsoft365 user was denied login access several times"
     DisplayName = "Microsoft365 Brute Force Login by User"
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
     Runbook = "Analyze the IP they came from and actions taken before/after."
     Reference = "https://learn.microsoft.com/en-us/microsoft-365/troubleshoot/authentication/access-denied-when-connect-to-office-365"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Microsoft365_Audit_AzureActiveDirectory]
     RuleID = "Microsoft365.Brute.Force.Login.by.User-prototype"
     Threshold = 10
     Tests = microsoft365_brute_force_loginby_user_tests
 
     def rule(self, event):
         return event.get("Operation", "") == "UserLoginFailed"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py` & `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from fnmatch import fnmatch
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import m365_alert_context
 from pypanther.log_types import LogType
 
 microsoft365_external_document_sharing_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Allowed Domain",
         ExpectedResult=False,
@@ -157,15 +157,15 @@
 
 class Microsoft365ExternalDocumentSharing(PantherRule):
     Description = "Document shared externally"
     DisplayName = "Microsoft365 External Document Sharing"
     Reports = {"MITRE ATT&CK": ["TA0009:T1039"]}
     Runbook = "Check the document metadata to ensure it is not a sensitive document."
     Reference = "https://support.microsoft.com/en-us/topic/manage-sharing-with-external-users-in-microsoft-365-small-business-2951a85f-c970-4375-aa4f-6b0d7035fe35#:~:text=Top%20of%20Page-,Turn%20external%20sharing%20on%20or%20off,-The%20ability%20to"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Microsoft365_Audit_SharePoint]
     RuleID = "Microsoft365.External.Document.Sharing-prototype"
     Tests = microsoft365_external_document_sharing_tests
     email_regex = re.compile("([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\\.[A-Z|a-z]{2,})+")
     ALLOWED_DOMAINS = ["mycompany.com", "alloweddomain.com"]  # should be in lowercase
     ALLOWED_USERS = ["exception@outsider.com"]  # should be in lowercase
     ALLOWED_PATHS = ["*/External/*", "External/*"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import m365_alert_context
 from pypanther.log_types import LogType
 
 microsoft365_mfa_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="MFA Add Event",
         ExpectedResult=False,
@@ -119,15 +119,15 @@
 
 class Microsoft365MFADisabled(PantherRule):
     Description = "A user's MFA has been removed"
     DisplayName = "Microsoft365 MFA Disabled"
     Reports = {"MITRE ATT&CK": ["TA003:T1556", "TA005:T1556", "TA006:T1556"]}
     Runbook = "Depending on company policy, either suggest or require the user re-enable two step verification."
     Reference = "https://learn.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Microsoft365_Audit_AzureActiveDirectory]
     RuleID = "Microsoft365.MFA.Disabled-prototype"
     Tests = microsoft365_mfa_disabled_tests
 
     def rule(self, event):
         if event.get("Operation", "") == "Update user.":
             modified_properties = event.get("ModifiedProperties", [])
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py` & `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_config import config
 from pypanther.log_types import LogType
 
 microsoft365_exchange_external_forwarding_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Forwarding Enabled",
         ExpectedResult=True,
@@ -208,15 +208,15 @@
 
 
 class Microsoft365ExchangeExternalForwarding(PantherRule):
     Description = "Detects creation of forwarding rule to external domains"
     DisplayName = "Microsoft Exchange External Forwarding"
     Reports = {"MITRE ATT&CK": ["TA0009:T1114"]}
     Reference = "https://learn.microsoft.com/en-us/microsoft-365/security/office-365-security/outbound-spam-policies-external-email-forwarding?view=o365-worldwide"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Microsoft365_Audit_Exchange]
     RuleID = "Microsoft365.Exchange.External.Forwarding-prototype"
     Tests = microsoft365_exchange_external_forwarding_tests
 
     def rule(self, event):
         if event.get("operation", "") in ("Set-Mailbox", "New-InboxRule"):
             for param in event.get("parameters", []):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py` & `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import msft_graph_alert_context
 from pypanther.log_types import LogType
 
 microsoft_graph_passthrough_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Anonymous Login Event",
         ExpectedResult=True,
@@ -95,15 +95,15 @@
 ]
 
 
 class MicrosoftGraphPassthrough(PantherRule):
     Description = "The Microsoft Graph security API federates queries to all onboarded security providers, including Azure AD Identity Protection, Microsoft 365, Microsoft Defender (Cloud, Endpoint, Identity) and Microsoft Sentinel"
     Reference = "https://learn.microsoft.com/en-us/graph/api/resources/security-api-overview"
     DisplayName = "Microsoft Graph Passthrough"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.MicrosoftGraph_SecurityAlert]
     RuleID = "Microsoft.Graph.Passthrough-prototype"
     Tests = microsoft_graph_passthrough_tests
 
     def rule(self, event):
         return event.get("status") == "newAlert"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db2_fa_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="2FA ebabled",
         ExpectedResult=False,
@@ -65,15 +65,15 @@
     ),
 ]
 
 
 class MongoDB2FADisabled(PantherRule):
     Description = "2FA was disabled."
     DisplayName = "MongoDB 2FA Disabled"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reference = "https://www.mongodb.com/docs/atlas/security-multi-factor-authentication/"
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.2FA.Disabled-prototype"
     Tests = mongo_db2_fa_disabled_tests
 
     def rule(self, event):
         return event.deep_get("eventTypeName", default="") == "ORG_TWO_FACTOR_AUTH_OPTIONAL"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_access_allowed_from_anywhere_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Allowed access from anywhere",
         ExpectedResult=True,
@@ -41,15 +41,15 @@
 
 
 class MongoDBAccessAllowedFromAnywhere(PantherRule):
     Description = "Atlas only allows client connections to the database deployment from entries in the project's IP access list. This rule detects when 0.0.0.0/0 is added to that list, which allows access from anywhere."
     DisplayName = "MongoDB access allowed from anywhere"
     LogTypes = [LogType.MongoDB_ProjectEvent]
     RuleID = "MongoDB.Access.Allowed.From.Anywhere-prototype"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reports = {"MITRE ATT&CK": ["T1021"]}
     Reference = "https://www.mongodb.com/docs/atlas/security/ip-access-list/"
     Runbook = "Check if this activity was legitimate. If not, delete 0.0.0.0/0 from the list of allowed ips."
     Tests = mongo_db_access_allowed_from_anywhere_tests
 
     def rule(self, event):
         if (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_alerting_disabled_or_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Alert added",
         ExpectedResult=False,
@@ -43,15 +43,15 @@
 
 
 class MongoDBAlertingDisabledOrDeleted(PantherRule):
     Description = "MongoDB provides security alerting policies for notifying admins when certain conditions are met. This rule detects when these policies are disabled or deleted."
     DisplayName = "MongoDB security alerts disabled or deleted"
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.Alerting.Disabled.Or.Deleted-prototype"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reports = {"MITRE ATT&CK": ["TA0005:T1562.001"]}
     Reference = "https://www.mongodb.com/docs/atlas/configure-alerts/"
     Runbook = "Re-enable security alerts"
     Tests = mongo_db_alerting_disabled_or_deleted_tests
 
     def rule(self, event):
         return event.deep_get("eventTypeName", default="") in [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_atlas_api_key_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="API Key Deleted",
@@ -68,15 +68,15 @@
     ),
 ]
 
 
 class MongoDBAtlasApiKeyCreated(PantherRule):
     Description = "A MongoDB Atlas api key's access list was updated"
     DisplayName = "MongoDB Atlas API Key Created"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reference = (
         "https://www.mongodb.com/docs/atlas/configure-api-access/#std-label-about-org-api-keys"
     )
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.Atlas.ApiKeyCreated-prototype"
     Tests = mongo_db_atlas_api_key_created_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import List
 from unittest.mock import MagicMock
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_external_user_invited_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Internal Invite",
@@ -70,15 +70,15 @@
     ),
 ]
 
 
 class MongoDBExternalUserInvited(PantherRule):
     Description = "An external user has been invited to a MongoDB org. "
     DisplayName = "MongoDB External User Invited"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reference = "https://www.mongodb.com/docs/v4.2/tutorial/create-users/"
     Tags = ["Configuration Required"]
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.External.UserInvited-prototype"
     Tests = mongo_db_external_user_invited_tests
     # Set domains allowed to join the organization ie. company.com
     ALLOWED_DOMAINS = []
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_external_user_invited_no_config_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Internal Invite",
         ExpectedResult=False,
@@ -65,15 +65,15 @@
     ),
 ]
 
 
 class MongoDBExternalUserInvitedNoConfig(PantherRule):
     Description = "An external user has been invited to a MongoDB org (no config)."
     DisplayName = "MongoDB External User Invited (no config)"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reference = "https://www.mongodb.com/docs/v4.2/tutorial/create-users/"
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.External.UserInvited.NoConfig-prototype"
     Tests = mongo_db_external_user_invited_no_config_tests
 
     def rule(self, event):
         if event.deep_get("eventTypeName", default="") != "INVITED_TO_ORG":
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_identity_provider_activity_tests: List[PantherRuleTest] = [
     PantherRuleTest(Name="Random event", ExpectedResult=False, Log={"eventTypeName": "cat_jumped"}),
     PantherRuleTest(
         Name="FEDERATION_SETTINGS_CREATED",
@@ -18,15 +18,15 @@
     ),
 ]
 
 
 class MongoDBIdentityProviderActivity(PantherRule):
     Description = "Changes to identity provider settings are privileged activities that should be carefully audited.  Attackers may add or change IDP integrations to gain persistence to environments"
     DisplayName = "MongoDB Identity Provider Activity"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reference = "https://attack.mitre.org/techniques/T1556/007/"
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.Identity.Provider.Activity-prototype"
     Tests = mongo_db_identity_provider_activity_tests
 
     def rule(self, event):
         important_event_types = {
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_logging_toggled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Random event",
         ExpectedResult=False,
@@ -65,15 +65,15 @@
     ),
 ]
 
 
 class MongoDBLoggingToggled(PantherRule):
     Description = "MongoDB logging toggled"
     DisplayName = "MongoDB logging toggled"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Reference = "https://attack.mitre.org/techniques/T1562/008/"
     LogTypes = [LogType.MongoDB_ProjectEvent]
     RuleID = "MongoDB.Logging.Toggled-prototype"
     Tests = mongo_db_logging_toggled_tests
 
     def rule(self, event):
         return event.deep_get("eventTypeName", default="") == "AUDIT_LOG_CONFIGURATION_UPDATED"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_d_borg_membership_restriction_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Restriction disabled",
         ExpectedResult=True,
@@ -56,15 +56,15 @@
 
 
 class MongoDBorgMembershipRestrictionDisabled(PantherRule):
     Description = "You can configure Atlas to require API access lists at the organization level. When you enable IP access list for the Atlas Administration API, all API calls in that organization must originate from a valid entry in the associated Atlas Administration API key access list. This rule detects when IP access list is disabled"
     DisplayName = "MongoDB org membership restriction disabled"
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.org.Membership.Restriction.Disabled-prototype"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reports = {"MITRE ATT&CK": ["T1556"]}
     Reference = "https://www.mongodb.com/docs/atlas/tutorial/manage-organizations/"
     Runbook = "Check if this activity is legitimate. If not, re-enable IP access list for the Atlas Administration API"
     Tests = mongo_d_borg_membership_restriction_disabled_tests
 
     def rule(self, event):
         return (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_user_created_or_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Random event",
         ExpectedResult=False,
@@ -94,15 +94,15 @@
     ),
 ]
 
 
 class MongoDBUserCreatedOrDeleted(PantherRule):
     Description = "User was created or deleted."
     DisplayName = "MongoDB user was created or deleted"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reference = "https://www.mongodb.com/docs/v4.2/tutorial/create-users/"
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.User.Created.Or.Deleted-prototype"
     Tests = mongo_db_user_created_or_deleted_tests
 
     def rule(self, event):
         return event.deep_get("eventTypeName", default="") in ("JOINED_ORG", "REMOVED_FROM_ORG")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py` & `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_mongodb_helpers import mongodb_alert_context
 from pypanther.log_types import LogType
 
 mongo_db_user_roles_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Random event",
         ExpectedResult=False,
@@ -65,15 +65,15 @@
     ),
 ]
 
 
 class MongoDBUserRolesChanged(PantherRule):
     Description = "User roles changed."
     DisplayName = "MongoDB user roles changed"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Reference = "https://www.mongodb.com/docs/v4.2/tutorial/create-users/"
     LogTypes = [LogType.MongoDB_OrganizationEvent]
     RuleID = "MongoDB.User.Roles.Changed-prototype"
     Tests = mongo_db_user_roles_changed_tests
 
     def rule(self, event):
         return event.deep_get("eventTypeName") == "USER_ROLES_CHANGED_AUDIT"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_admin_logged_out.py` & `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_admin_logged_out.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 netskope_admin_logged_out_login_failures_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="True positive",
         ExpectedResult=True,
         Log={
@@ -56,15 +56,15 @@
 
 class NetskopeAdminLoggedOutLoginFailures(PantherRule):
     RuleID = "Netskope.AdminLoggedOutLoginFailures-prototype"
     DisplayName = "Admin logged out because of successive login failures"
     LogTypes = [LogType.Netskope_Audit]
     Tags = ["Netskope", "Brute Force"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An admin was logged out because of successive login failures."
     Runbook = "An admin was logged out because of successive login failures.  This could indicate brute force activity against this account."
     Reference = "https://docs.netskope.com/en/netskope-help/admin-console/administration/audit-log/"
     Tests = netskope_admin_logged_out_login_failures_tests
 
     def rule(self, event):
         if event.get("audit_log_event") == "Admin logged out because of successive login failures":
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_admin_user_change.py` & `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_admin_user_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 netskope_admin_user_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="True positive",
         ExpectedResult=True,
         Log={
@@ -56,15 +56,15 @@
 
 class NetskopeAdminUserChange(PantherRule):
     RuleID = "Netskope.AdminUserChange-prototype"
     DisplayName = "An administrator account was created, deleted, or modified."
     LogTypes = [LogType.Netskope_Audit]
     Tags = ["Netskope", "Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0004:T1098"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Reference = "https://docs.netskope.com/en/netskope-help/admin-console/administration/managing-administrators/"
     Description = "An administrator account was created, deleted, or modified."
     Runbook = "An administrator account was created, deleted, or modified.  Validate that this activity is expected and authorized."
     Tests = netskope_admin_user_change_tests
     ADMIN_USER_CHANGE_EVENTS = [
         "Created new admin",
         "Added SSO Admin",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_many_deletes.py` & `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_many_deletes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 netskope_many_deletes_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="True positive",
         ExpectedResult=True,
         Log={
@@ -52,15 +52,15 @@
 
 class NetskopeManyDeletes(PantherRule):
     RuleID = "Netskope.ManyDeletes-prototype"
     DisplayName = "Netskope Many Objects Deleted"
     LogTypes = [LogType.Netskope_Audit]
     Tags = ["Netskope", "Configuration Required", "Data Destruction"]
     Reports = {"MITRE ATT&CK": ["TA0040:T1485"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A user deleted a large number of objects in a short period of time."
     Threshold = 10
     Runbook = "A user deleted a large number of objects in a short period of time.  Validate that this activity is expected and authorized."
     Reference = "https://docs.netskope.com/en/netskope-help/admin-console/administration/audit-log/"
     Tests = netskope_many_deletes_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_personnel_action.py` & `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_personnel_action.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 netskope_netskope_personnel_activity_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="True positive",
         ExpectedResult=True,
         Log={
@@ -56,15 +56,15 @@
 
 class NetskopeNetskopePersonnelActivity(PantherRule):
     RuleID = "Netskope.NetskopePersonnelActivity-prototype"
     DisplayName = "Action Performed by Netskope Personnel"
     LogTypes = [LogType.Netskope_Audit]
     Tags = ["Netskope", "Supply Chain Compromise"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An action was performed by Netskope personnel."
     Runbook = "Action taken by Netskope Personnel.  Validate that this action was authorized."
     Reference = "https://docs.netskope.com/en/netskope-help/admin-console/administration/audit-log/#filters-1"
     Tests = netskope_netskope_personnel_activity_tests
 
     def rule(self, event):
         if event.get("is_netskope_personnel") is True:
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py` & `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_walk
 from pypanther.log_types import LogType
 
 netskope_unauthorized_api_calls_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="True positive",
         ExpectedResult=True,
@@ -62,15 +62,15 @@
 
 class NetskopeUnauthorizedAPICalls(PantherRule):
     RuleID = "Netskope.UnauthorizedAPICalls-prototype"
     DisplayName = "Netskope Many Unauthorized API Calls"
     LogTypes = [LogType.Netskope_Audit]
     Tags = ["Netskope", "Configuration Required", "Brute Force"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Many unauthorized API calls were observed for a user in a short period of time."
     Threshold = 10
     Runbook = "An account is making many unauthorized API calls.  This could indicate brute force activity, or expired service account credentials."
     Reference = "https://docs.netskope.com/en/netskope-help/data-security/netskope-private-access/private-access-rest-apis/"
     Tests = netskope_unauthorized_api_calls_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_account_changed_after_login.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_account_changed_after_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.helpers.panther_oss_helpers import get_string_set, put_string_set
 from pypanther.log_types import LogType
 
 notion_account_changed_after_login_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Login event",
@@ -320,15 +320,15 @@
 
 
 class NotionAccountChangedAfterLogin(PantherRule):
     RuleID = "Notion.AccountChangedAfterLogin-prototype"
     DisplayName = "Notion Account Changed Shortly After Login"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Identity & Access Management", "Persistence"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Notion User logged in then changed their account details."
     Runbook = "Possible account takeover. Follow up with the Notion User to determine if this email change is genuine."
     Reference = "https://www.notion.so/help/account-settings"
     Tests = notion_account_changed_after_login_tests
     # Length of time in minutes. If a user logs in, then changes their email within this many
     # minutes, raise an alert.
     DEFAULT_EMAIL_CHANGE_WINDOW_MINUTES = 10
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 
 class NotionLoginFromBlockedIP(PantherRule):
     RuleID = "Notion.LoginFromBlockedIP-prototype"
     DisplayName = "Notion Login From Blocked IP"
@@ -12,15 +12,15 @@
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = [
         "Notion",
         "Network Security Monitoring",
         "Malicious Connections",
         "Configuration Required",
     ]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A user attempted to access Notion from a blocked IP address. Note: before deployinh, make sure to add Rule Filters checking if event.ip_address is in a certain CIDR range(s)."
     Runbook = (
         "Confirm with user if the login was legitimate. If so, determine why the IP is blocked."
     )
     Reference = "https://www.notion.so/help/allowlist-ip"
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_login_from_new_location.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_login_from_new_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import json
 import time
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_ipinfo_helpers import IPInfoLocation
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.helpers.panther_oss_helpers import get_dictionary, put_dictionary
 from pypanther.log_types import LogType
 
 notion_login_from_new_location_tests: List[PantherRuleTest] = [
     PantherRuleTest(
@@ -277,15 +277,15 @@
 
 
 class NotionLoginFromNewLocation(PantherRule):
     RuleID = "Notion.LoginFromNewLocation-prototype"
     DisplayName = "Notion Login from New Location"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Identity & Access Management", "Login & Access Patterns"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Notion User logged in from a new location."
     Runbook = "Possible account takeover. Follow up with the Notion User to determine if this login is genuine."
     Reference = "https://ipinfo.io/products/ip-geolocation-api"
     Tests = notion_login_from_new_location_tests
     # How long (in seconds) to keep previous login locations in cached memory
     DEFAULT_CACHE_PERIOD = 2419200
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_many_pages_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_many_pages_deleted.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_many_pages_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -60,15 +60,15 @@
 
 
 class NotionManyPagesDeleted(PantherRule):
     RuleID = "Notion.Many.Pages.Deleted-prototype"
     DisplayName = "Notion Many Pages Deleted"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Security", "Data Destruction"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Notion User deleted multiple pages."
     Threshold = 10
     Runbook = "Possible Data Destruction. Follow up with the Notion User to determine if this was done for a valid business reason."
     Reference = "https://www.notion.so/help/duplicate-delete-and-restore-content"
     Tests = notion_many_pages_deleted_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_many_pages_exported.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_many_pages_exported.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_many_pages_exported_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -60,15 +60,15 @@
 
 
 class NotionManyPagesExported(PantherRule):
     RuleID = "Notion.Many.Pages.Exported-prototype"
     DisplayName = "Notion Many Pages Exported"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Security", "Data Exfiltration"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A Notion User exported multiple pages."
     Threshold = 10
     Runbook = "Possible Data Exfiltration. Follow up with the Notion User to determine if this was done for a valid business reason."
     Reference = "https://www.notion.so/help/export-your-content"
     Tests = notion_many_pages_exported_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_accessible_to_api.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_accessible_to_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 
 class NotionPagePermsAPIPermsChanged(PantherRule):
     DisplayName = "Notion Page API Permissions Changed"
     RuleID = "Notion.PagePerms.APIPermsChanged-prototype"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Security", "Unapproved 3rd Party Apps"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = (
         "A new API integration was added to a Notion page, or it's permissions were changed."
     )
     Runbook = "Potential information exposure - review the shared page and rectify if needed."
     Reference = "https://www.notion.so/help/sharing-and-permissions"
     # These event types correspond to users adding or editing the default role on a public page
     event_types = (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_page_perms_guest_perms_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Guest Role Added",
@@ -76,15 +76,15 @@
 
 
 class NotionPagePermsGuestPermsChanged(PantherRule):
     RuleID = "Notion.PagePerms.GuestPermsChanged-prototype"
     DisplayName = "Notion Page Guest Permissions Changed"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Security", "Information Disclosure"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "The external guest permissions for a Notion page have been altered."
     Runbook = "Potential information exposure - review the shared page and rectify if needed."
     Reference = "https://www.notion.so/help/sharing-and-permissions"
     Tests = notion_page_perms_guest_perms_changed_tests
     # These event types correspond to users adding or editing the default role on a public page
     event_types = ("page.permissions.guest_role_added", "page.permissions.guest_role_updated")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_shared_to_web.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_shared_to_web.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 
 class NotionPageSharedToWeb(PantherRule):
     RuleID = "Notion.PageSharedToWeb-prototype"
     DisplayName = "Notion Page Published to Web"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Security", "Information Disclosure"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A Notion User published a page to the web."
     Runbook = "Potential information exposure - review the shared page and rectify if needed."
     Reference = "https://www.notion.so/help/public-pages-and-web-publishing"
     # These event types correspond to users adding or editing the default role on a public page
     event_types = (
         "page.permissions.shared_to_public_role_added",
         "page.permissions.shared_to_public_role_updated",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_scim_token_generated.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_scim_token_generated.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_workspace_scim_token_generated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="other event",
         ExpectedResult=False,
@@ -52,15 +52,15 @@
 
 class NotionWorkspaceSCIMTokenGenerated(PantherRule):
     RuleID = "Notion.Workspace.SCIM.Token.Generated-prototype"
     DisplayName = "Notion SCIM Token Generated"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Application Security", "Supply Chain Attack"]
     Description = "A Notion User generated a SCIM token."
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Runbook = "Possible Initial Access. Follow up with the Notion User to determine if this was done for a valid business reason."
     Reference = "https://www.notion.so/help/provision-users-and-groups-with-scim"
     Tests = notion_workspace_scim_token_generated_tests
 
     def rule(self, event):
         event_type = event.deep_get("event", "type", default="<NO_EVENT_TYPE_FOUND>")
         return event_type == "workspace.scim_token_generated"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_sharing_settings_updated.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_sharing_settings_updated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_sharing_settings_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Sharing Enabled",
         ExpectedResult=True,
@@ -59,15 +59,15 @@
 
 class NotionSharingSettingsUpdated(PantherRule):
     RuleID = "Notion.SharingSettingsUpdated-prototype"
     DisplayName = "Notion Sharing Settings Updated"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Exfiltration"]
     Description = "A Notion User enabled sharing for a Workspace or Teamspace."
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Runbook = "Possible Data Exfiltration. Follow up with the Notion User to determine if this was done for a valid business reason."
     Tests = notion_sharing_settings_updated_tests
     EVENTS = (
         "teamspace.settings.allow_public_page_sharing_setting_updated",
         "teamspace.settings.allow_guests_setting_updated",
         "teamspace.settings.allow_content_export_setting_updated",
         "workspace.settings.allow_public_page_sharing_setting_updated",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_teamspace_owner_added.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_teamspace_owner_added.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_teamspace_owner_added_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Member Added",
         ExpectedResult=False,
@@ -78,15 +78,15 @@
 
 class NotionTeamspaceOwnerAdded(PantherRule):
     RuleID = "Notion.TeamspaceOwnerAdded-prototype"
     DisplayName = "Notion Teamspace Owner Added"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Privilege Escalation"]
     Description = "A Notion User was added as a Teamspace owner."
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Runbook = "Possible Privilege Escalation. Follow up with the Notion User to determine if this was done for a valid business reason."
     Tests = notion_teamspace_owner_added_tests
 
     def rule(self, event):
         added = (
             event.deep_get("event", "type", default="") == "teamspace.permissions.member_added"
             and event.deep_get("event", "details", "role", default="") == "owner"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_audit_log_exported_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -51,15 +51,15 @@
 
 
 class NotionAuditLogExported(PantherRule):
     RuleID = "Notion.Audit.Log.Exported-prototype"
     DisplayName = "Notion Audit Log Exported"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Security", "Data Exfiltration"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Notion User exported audit logs for your organization’s workspace."
     Runbook = "Possible Data Exfiltration. Follow up with the Notion User to determine if this was done for a valid business reason."
     Reference = "https://www.notion.so/help/audit-log#export-your-audit-log"
     Tests = notion_audit_log_exported_tests
 
     def rule(self, event):
         event_type = event.deep_get("event", "type", default="<NO_EVENT_TYPE_FOUND>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_exported.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_exported.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_workspace_exported_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Workspace Exported",
         ExpectedResult=True,
@@ -60,15 +60,15 @@
 
 
 class NotionWorkspaceExported(PantherRule):
     RuleID = "Notion.Workspace.Exported-prototype"
     DisplayName = "Notion Workspace Exported"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Security", "Data Exfiltration"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A Notion User exported an existing workspace."
     Runbook = "Possible Data Exfiltration. Follow up with the Notion User to determine if this was done for a valid business reason."
     Reference = "https://www.notion.so/help/workspace-settings#export-an-entire-workspace"
     Tests = notion_workspace_exported_tests
 
     def rule(self, event):
         event_type = event.deep_get("event", "type", default="<NO_EVENT_TYPE_FOUND>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_samlsso_configuration_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
@@ -73,15 +73,15 @@
 
 
 class NotionSAMLSSOConfigurationChanged(PantherRule):
     RuleID = "Notion.SAML.SSO.Configuration.Changed-prototype"
     DisplayName = "Notion SAML SSO Configuration Changed"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Identity & Access Management", "Credential Security"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "A Notion User changed settings to enforce SAML SSO configurations for your organization."
     )
     Runbook = "Follow up with the Notion User to determine if this was done for a valid business reason and to ensure these settings get re-enabled quickly for best security practices."
     Reference = "https://www.notion.so/help/saml-sso-configuration"
     Tests = notion_samlsso_configuration_changed_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py` & `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_notion_helpers import notion_alert_context
 from pypanther.log_types import LogType
 
 notion_workspace_public_page_added_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Public page added",
@@ -66,15 +66,15 @@
 
 
 class NotionWorkspacePublicPageAdded(PantherRule):
     RuleID = "Notion.Workspace.Public.Page.Added-prototype"
     DisplayName = "Notion Workspace public page added"
     LogTypes = [LogType.Notion_AuditLogs]
     Tags = ["Notion", "Data Security", "Information Disclosure"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A Notion page was set to public in your worksace."
     Runbook = "A Notion page was made public. Check with the author to determine why this page was made public."
     Reference = "https://www.notion.so/help/public-pages-and-web-publishing"
     Tests = notion_workspace_public_page_added_tests
 
     def rule(self, event):
         event_type = event.deep_get("event", "type", default="<NO_EVENT_TYPE_FOUND>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_account_support_access.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_account_support_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 okta_support_access_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Support Access Granted",
         ExpectedResult=True,
         Log={
@@ -70,15 +70,15 @@
     Tags = [
         "Identity & Access Management",
         "DataModel",
         "Okta",
         "Initial Access:Trusted Relationship",
     ]
     Reports = {"MITRE ATT&CK": ["TA0001:T1199"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An admin user has granted access to Okta Support to your account"
     Reference = "https://help.okta.com/en/prod/Content/Topics/Settings/settings-support-access.htm"
     Runbook = "Contact Admin to ensure this was sanctioned activity"
     DedupPeriodMinutes = 15
     SummaryAttributes = ["eventType", "severity", "displayMessage", "p_any_ip_addresses"]
     Tests = okta_support_access_tests
     OKTA_SUPPORT_ACCESS_EVENTS = [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 okta_global_mfa_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="MFA Disabled",
         ExpectedResult=True,
         Log={
@@ -69,15 +69,15 @@
     Tags = [
         "Identity & Access Management",
         "DataModel",
         "Okta",
         "Defense Evasion:Modify Authentication Process",
     ]
     Reports = {"MITRE ATT&CK": ["TA0005:T1556"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "An admin user has disabled the MFA requirement for your Okta account"
     Reference = "https://help.okta.com/oie/en-us/content/topics/identity-engine/authenticators/about-authenticators.htm"
     Runbook = "Contact Admin to ensure this was sanctioned activity"
     DedupPeriodMinutes = 15
     SummaryAttributes = ["eventType", "severity", "displayMessage", "p_any_ip_addresses"]
     Tests = okta_global_mfa_disabled_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_admin_role_assigned.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_admin_role_assigned.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_admin_role_assigned_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Admin Access Assigned",
         ExpectedResult=True,
@@ -127,15 +127,15 @@
 
 class OktaAdminRoleAssigned(PantherRule):
     RuleID = "Okta.AdminRoleAssigned-prototype"
     DisplayName = "Okta Admin Role Assigned"
     LogTypes = [LogType.Okta_SystemLog]
     Tags = ["Identity & Access Management", "Okta", "Privilege Escalation:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0004:T1078"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A user has been granted administrative privileges in Okta"
     Reference = (
         "https://help.okta.com/en/prod/Content/Topics/Security/administrators-admin-comparison.htm"
     )
     Runbook = "Reach out to the user if needed to validate the activity"
     DedupPeriodMinutes = 15
     SummaryAttributes = ["eventType", "severity", "displayMessage", "p_any_ip_addresses"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_anonymizing_vpn_login_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -161,15 +161,15 @@
 
 
 class OktaAnonymizingVPNLogin(PantherRule):
     RuleID = "Okta.Anonymizing.VPN.Login-prototype"
     DisplayName = "Okta Sign-In from VPN Anonymizer"
     LogTypes = [LogType.Okta_SystemLog]
     Reports = {"MITRE ATT&CK": ["TA0006:T1556"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A user is attempting to sign-in to Okta from a known VPN anonymizer.  The threat actor would access the compromised account using anonymizing proxy services.\n"
     Runbook = "Restrict this access to trusted Network Zones and deny access from anonymizing proxies in policy using a Dynamic Network Zone.\n"
     Reference = "https://sec.okta.com/articles/2023/08/cross-tenant-impersonation-prevention-and-detection\n"
     DedupPeriodMinutes = 360
     Tests = okta_anonymizing_vpn_login_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_api_key_created.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_api_key_created.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_api_key_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="API Key Created",
         ExpectedResult=True,
@@ -45,15 +45,15 @@
     LogTypes = [LogType.Okta_SystemLog]
     Tags = [
         "Identity & Access Management",
         "Okta",
         "Credential Access:Steal Application Access Token",
     ]
     Reports = {"MITRE ATT&CK": ["TA0006:T1528"]}
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A user created an API Key in Okta"
     Reference = "https://help.okta.com/en/prod/Content/Topics/Security/API.htm"
     Runbook = "Reach out to the user if needed to validate the activity."
     SummaryAttributes = ["eventType", "severity", "displayMessage", "p_any_ip_addresses"]
     Tests = okta_api_key_created_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_api_key_revoked.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_api_key_revoked.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_api_key_revoked_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="API Key Revoked",
         ExpectedResult=True,
@@ -40,15 +40,15 @@
 
 
 class OktaAPIKeyRevoked(PantherRule):
     RuleID = "Okta.APIKeyRevoked-prototype"
     DisplayName = "Okta API Key Revoked"
     LogTypes = [LogType.Okta_SystemLog]
     Tags = ["Identity & Access Management", "Okta"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A user has revoked an API Key in Okta"
     Reference = "https://help.okta.com/en/prod/Content/Topics/Security/API.htm"
     Runbook = "Validate this action was authorized."
     SummaryAttributes = ["eventType", "severity", "displayMessage", "p_any_ip_addresses"]
     Tests = okta_api_key_revoked_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import okta_alert_context
 from pypanther.log_types import LogType
 
 okta_refresh_access_token_reuse_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Non-event",
         ExpectedResult=False,
@@ -183,15 +183,15 @@
 class OktaRefreshAccessTokenReuse(PantherRule):
     Description = "When a client wants to renew an access token, it sends the refresh token with the access token request to the /token Okta endpoint. \nOkta validates the incoming refresh token, issues a new set of tokens and invalidates the refresh token that was passed with the initial request.\nThis detection alerts when a previously used refresh token is used again with the token request"
     Reference = (
         "https://developer.okta.com/docs/guides/refresh-tokens/main/#refresh-token-reuse-detection"
     )
     DisplayName = "Okta App Refresh Access Token Reuse"
     Runbook = "Determine if the clientip is anomalous. Revoke tokens if deemed suspicious."
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.Refresh.Access.Token.Reuse-prototype"
     Tests = okta_refresh_access_token_reuse_tests
 
     def rule(self, event):
         return event.get("eventtype") in (
             "app.oauth2.as.token.detect_reuse",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_app_unauthorized_access_attempt_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Unauthorized Access Event",
         ExpectedResult=True,
@@ -167,15 +167,15 @@
     ),
 ]
 
 
 class OktaAppUnauthorizedAccessAttempt(PantherRule):
     Description = "Detects when a user is denied access to an Okta application"
     DisplayName = "Okta App Unauthorized Access Attempt"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Reference = "https://support.okta.com/help/s/article/App-Sign-on-Error-403-User-attempted-unauthorized-access-to-app?language=en_US"
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.App.Unauthorized.Access.Attempt-prototype"
     Threshold = 5
     Tests = okta_app_unauthorized_access_attempt_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import okta_alert_context
 from pypanther.log_types import LogType
 
 okta_group_admin_role_assigned_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Group Privilege Grant",
         ExpectedResult=True,
@@ -168,15 +168,15 @@
 ]
 
 
 class OktaGroupAdminRoleAssigned(PantherRule):
     Description = "Detect when an admin role is assigned to a group"
     DisplayName = "Okta Group Admin Role Assigned"
     Reference = "https://support.okta.com/help/s/article/How-to-assign-Administrator-roles-to-groups?language=en_US#:~:text=Log%20in%20to%20the%20Admin,user%20and%20click%20Save%20changes"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.Group.Admin.Role.Assigned-prototype"
     Tests = okta_group_admin_role_assigned_tests
 
     def rule(self, event):
         return event.get("eventtype", "") == "group.privilege.grant"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_idp_create_modify.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_idp_create_modify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_identity_provider_created_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -161,15 +161,15 @@
 
 
 class OktaIdentityProviderCreatedModified(PantherRule):
     RuleID = "Okta.Identity.Provider.Created.Modified-prototype"
     DisplayName = "Okta Identity Provider Created or Modified"
     LogTypes = [LogType.Okta_SystemLog]
     Reports = {"MITRE ATT&CK": ["TA0006:T1556", "TA0001:T1199", "TA0003:T1098"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = 'A new 3rd party Identity Provider has been created or modified.   Attackers have been observed configuring a second Identity Provider to act as an "impersonation app"  to access applications within the compromised Org on behalf of other users. This second Identity Provider,  also controlled by the attacker, would act as a “source” IdP in an inbound federation relationship  (sometimes called “Org2Org”) with the target.\n'
     Runbook = "Delegate access to this feature to a Custom Admin Role with the minimum required permissions. Constrain these roles to groups that exclude highly privileged administrators.\n"
     Reference = "https://sec.okta.com/articles/2023/08/cross-tenant-impersonation-prevention-and-detection\n"
     DedupPeriodMinutes = 30
     Tests = okta_identity_provider_created_modified_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_idp_signin.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_idp_signin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_identity_provider_sign_in_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -163,15 +163,15 @@
 class OktaIdentityProviderSignIn(PantherRule):
     RuleID = "Okta.Identity.Provider.SignIn-prototype"
     DisplayName = "Okta Identity Provider Sign-in"
     Enabled = False
     LogTypes = [LogType.Okta_SystemLog]
     Tags = ["Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1199", "TA0003:T1098"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = 'A user has signed in using a 3rd party Identity Provider.   Attackers have been observed configuring a second Identity Provider to act as an "impersonation app"  to access applications within the compromised Org on behalf of other users. This second Identity Provider,  also controlled by the attacker, would act as a “source” IdP in an inbound federation relationship  (sometimes called “Org2Org”) with the target. From this “source” IdP, the threat actor manipulated the username parameter for targeted users in the second  “source” Identity Provider to match a real user in the compromised “target” Identity Provider.  This provided the ability to Single sign-on (SSO) into applications in the target IdP as the targeted user. Do not use this rule if your organization uses legitimate 3rd-party Identity Providers.\n'
     Reference = "https://sec.okta.com/articles/2023/08/cross-tenant-impersonation-prevention-and-detection\n"
     DedupPeriodMinutes = 30
     Tests = okta_identity_provider_sign_in_tests
 
     def rule(self, event):
         return event.get("eventType") == "user.authentication.auth_via_IDP"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_new_behavior_accessing_admin_console_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="New Behavior Accessing Admin Console (behavior)",
         ExpectedResult=True,
@@ -293,15 +293,15 @@
 
 
 class OktaNewBehaviorAccessingAdminConsole(PantherRule):
     RuleID = "Okta.New.Behavior.Accessing.Admin.Console-prototype"
     DisplayName = "Okta New Behaviors Acessing Admin Console"
     LogTypes = [LogType.Okta_SystemLog]
     Reports = {"MITRE ATT&CK": ["TA0001:T1078.004"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "New Behaviors Observed while Accessing Okta Admin Console. A user attempted to access the Okta Admin Console from a new device with a new IP.\n"
     Runbook = "Configure Authentication Policies (Application Sign-on Policies) for access to privileged applications, including the Admin Console, to require re-authentication “at every sign-in”. Turn on and test New Device and Suspicious Activity end-user notifications.\n"
     Reference = "https://sec.okta.com/articles/2023/08/cross-tenant-impersonation-prevention-and-detection\n"
     Tests = okta_new_behavior_accessing_admin_console_tests
 
     def rule(self, event):
         if event.get("eventtype") != "policy.evaluate_sign_on":
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_org2org_creation_modification.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_org2org_creation_modification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_org2org_creation_modification_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Org2Org modified",
         ExpectedResult=True,
@@ -293,15 +293,15 @@
 
 
 class OktaOrg2orgCreationModification(PantherRule):
     RuleID = "Okta.Org2org.Creation.Modification-prototype"
     DisplayName = "Okta Org2Org application created of modified"
     LogTypes = [LogType.Okta_SystemLog]
     Reports = {"MITRE ATT&CK": ["TA0006:T1556", "TA0004:T1078.004"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "An Okta Org2Org application has been created or modified. Okta's Org2Org applications instances are used to push and match users from one Okta organization to another. A malicious actor can add an Org2Org application instance and create a user in the source organization (controlled by the attacker)  with the same identifier as a Super Administrator in the target organization.\n"
     Reference = "https://www.authomize.com/blog/authomize-discovers-password-stealing-and-impersonation-risks-to-in-okta/\n"
     Tests = okta_org2org_creation_modification_tests
     APP_LIFECYCLE_EVENTS = (
         "application.lifecycle.update",
         "application.lifecycle.create",
         "application.lifecycle.activate",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_password_accessed.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_password_accessed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, get_val_from_list
 from pypanther.log_types import LogType
 
 okta_password_access_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User accessed their own password",
         ExpectedResult=False,
@@ -243,15 +243,15 @@
 
 class OktaPasswordAccess(PantherRule):
     RuleID = "Okta.PasswordAccess-prototype"
     DisplayName = "Okta Password Accessed"
     LogTypes = [LogType.Okta_SystemLog]
     Tags = ["Okta", "Credential Access:Unsecured Credentials"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1552"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "User accessed another user's application password\n"
     Reference = "https://help.okta.com/en-us/content/topics/apps/apps_revealing_the_password.htm"
     Runbook = "Investigate whether this was authorized access.\n"
     Tests = okta_password_access_tests
 
     def rule(self, event):
         if event.get("eventType") != "application.user_membership.show_password":
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, deep_walk, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_password_extractionvia_scim_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -161,15 +161,15 @@
 
 
 class OktaPasswordExtractionviaSCIM(PantherRule):
     RuleID = "Okta.Password.Extraction.via.SCIM-prototype"
     DisplayName = "Okta Cleartext Passwords Extracted via SCIM Application"
     LogTypes = [LogType.Okta_SystemLog]
     Reports = {"MITRE ATT&CK": ["TA0006:T1556"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "An application admin has extracted cleartext user passwords via SCIM app. Malcious actors can extract plaintext passwords by creating a SCIM application under their control and configuring it to sync passwords from Okta.\n"
     Reference = "https://www.authomize.com/blog/authomize-discovers-password-stealing-and-impersonation-risks-to-in-okta/\n"
     DedupPeriodMinutes = 30
     Tests = okta_password_extractionvia_scim_tests
 
     def rule(self, event):
         return event.get(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_phishing_attempt_blocked_fast_pass_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -161,15 +161,15 @@
 
 
 class OktaPhishingAttemptBlockedFastPass(PantherRule):
     RuleID = "Okta.Phishing.Attempt.Blocked.FastPass-prototype"
     DisplayName = "Okta AiTM Phishing Attempt Blocked by FastPass"
     LogTypes = [LogType.Okta_SystemLog]
     Reports = {"MITRE ATT&CK": ["TA0001:T1566", "TA0006:T1556", "TA0003:T1078.004"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "Okta FastPass detected a user targeted by attackers wielding real-time (AiTM) proxies.\n"
     )
     Runbook = "Protect sign-in flows by enforcing phishing-resistant authentication with Okta FastPass and FIDO2 WebAuthn.\n"
     Reference = "https://sec.okta.com/fastpassphishingdetection\n"
     DedupPeriodMinutes = 30
     Tests = okta_phishing_attempt_blocked_fast_pass_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_potentially_stolen_session.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_potentially_stolen_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from datetime import timedelta
 from difflib import SequenceMatcher
 from typing import List
 
 from panther_detection_helpers.caching import get_string_set, put_string_set
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_potentially_stolen_session_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Same device and OS",
         ExpectedResult=False,
@@ -349,15 +349,15 @@
 
 class OktaPotentiallyStolenSession(PantherRule):
     RuleID = "Okta.PotentiallyStolenSession-prototype"
     DisplayName = "Okta Potentially Stolen Session"
     LogTypes = [LogType.Okta_SystemLog]
     Tags = ["Identity & Access Management", "Okta"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1539"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "This rule looks for the same session being used from two devices, indicating a compromised session token."
     Runbook = "Confirm the session is used on two devices, one of which is unknown. Lock the users Okta account and clear the users sessions in down stream apps."
     Reference = "https://sec.okta.com/sessioncookietheft"
     SummaryAttributes = ["eventType", "severity", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = okta_potentially_stolen_session_tests
     FUZZ_RATIO_MIN = 0.95
     PREVIOUS_SESSION = {}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_rate_limits.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_rate_limits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fnmatch import fnmatch
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import okta_alert_context
 from pypanther.log_types import LogType
 
 okta_rate_limits_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="system.org.ratelimit.warning",
         ExpectedResult=True,
@@ -222,15 +222,15 @@
     ),
 ]
 
 
 class OktaRateLimits(PantherRule):
     Description = "Potential DoS/Bruteforce attack or hitting limits (system degradation)"
     DisplayName = "Okta Rate Limits"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["Credential Access", "Brute Force", "Impact", "Network Denial of Service"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1110", "TA0040:T1498"]}
     Reference = "https://developer.okta.com/docs/reference/rl-system-log-events/"
     DedupPeriodMinutes = 360
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.Rate.Limits-prototype"
     Tests = okta_rate_limits_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_support_reset.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_support_reset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_support_reset_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Support Reset Credential",
         ExpectedResult=True,
@@ -96,15 +96,15 @@
     Tags = [
         "Identity & Access Management",
         "DataModel",
         "Okta",
         "Initial Access:Trusted Relationship",
     ]
     Reports = {"MITRE ATT&CK": ["TA0001:T1199"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A Password or MFA factor was reset by Okta Support"
     Reference = "https://help.okta.com/en/prod/Content/Topics/Directory/get-support.htm#:~:text=Visit%20the%20Okta%20Help%20Center,1%2D800%2D219%2D0964"
     Runbook = "Contact Admin to ensure this was sanctioned activity"
     DedupPeriodMinutes = 15
     SummaryAttributes = ["eventType", "severity", "p_any_ip_addresses"]
     Tests = okta_support_reset_tests
     OKTA_SUPPORT_RESET_EVENTS = [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, okta_alert_context
 from pypanther.log_types import LogType
 
 okta_threat_insight_security_threat_detected_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -181,15 +181,15 @@
 ]
 
 
 class OktaThreatInsightSecurityThreatDetected(PantherRule):
     Description = "Okta ThreatInsight identified request from potentially malicious IP address"
     Reference = "https://help.okta.com/en-us/Content/Topics/Security/threat-insight/configure-threatinsight-system-log.htm"
     DisplayName = "Okta ThreatInsight Security Threat Detected"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.ThreatInsight.Security.Threat.Detected-prototype"
     Tests = okta_threat_insight_security_threat_detected_tests
 
     def severity_from_threat_string(self, threat_detection):
         # threat detection is a string but contains json data
         # can contain multiple threats detected with multiple severities
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_account_locked.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_account_locked.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import okta_alert_context
 from pypanther.log_types import LogType
 
 okta_user_account_locked_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Account Lock Event",
         ExpectedResult=True,
@@ -155,15 +155,15 @@
 ]
 
 
 class OktaUserAccountLocked(PantherRule):
     Description = "An Okta user has locked their account."
     DisplayName = "Okta User Account Locked"
     Reference = "https://support.okta.com/help/s/article/How-to-Configure-the-Number-of-Failed-Login-Attempts-Before-User-Lockout?language=en_US"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.User.Account.Locked-prototype"
     Tests = okta_user_account_locked_tests
 
     def rule(self, event):
         return event.get("eventtype") in ("user.account.lock", "user.account.lock.limit")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import okta_alert_context
 from pypanther.log_types import LogType
 
 okta_user_mfa_factor_suspend_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Suspend Event",
         ExpectedResult=True,
@@ -159,15 +159,15 @@
 ]
 
 
 class OktaUserMFAFactorSuspend(PantherRule):
     Description = "Suspend factor or authenticator enrollment method for user."
     DisplayName = "Okta User MFA Factor Suspend"
     Reference = "https://help.okta.com/en-us/content/topics/security/mfa/mfa-factors.htm"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.User.MFA.Factor.Suspend-prototype"
     Tests = okta_user_mfa_factor_suspend_tests
 
     def rule(self, event):
         return (
             event.get("eventtype") == "user.mfa.factor.suspend"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_reset.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_reset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import okta_alert_context
 from pypanther.log_types import LogType
 
 okta_user_mfa_reset_single_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User reset own MFA factor",
         ExpectedResult=True,
@@ -81,15 +81,15 @@
 
 
 class OktaUserMFAResetSingle(PantherRule):
     Description = "User has reset one of their own MFA factors"
     DisplayName = "Okta User MFA Own Reset"
     RuleID = "Okta.User.MFA.Reset.Single-prototype"
     Reference = "https://support.okta.com/help/s/article/How-to-avoid-lockouts-and-reset-your-Multifactor-Authentication-MFA-for-Okta-Admins?language=en_US"
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.Okta_SystemLog]
     Tests = okta_user_mfa_reset_single_tests
 
     def rule(self, event):
         return event.udm("event_type") == event_type.MFA_RESET
 
     def title(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import okta_alert_context
 from pypanther.log_types import LogType
 
 okta_user_mfa_reset_all_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Reset All Event",
         ExpectedResult=True,
@@ -117,15 +117,15 @@
 ]
 
 
 class OktaUserMFAResetAll(PantherRule):
     Description = "All MFA factors have been reset for a user."
     DisplayName = "Okta User MFA Reset All"
     Reference = "https://help.okta.com/en-us/content/topics/security/mfa/mfa-reset-users.htm#:~:text=the%20Admin%20Console%3A-,In%20the%20Admin%20Console%2C%20go%20to%20DirectoryPeople.,Selected%20Factors%20or%20Reset%20All"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.User.MFA.Reset.All-prototype"
     Tests = okta_user_mfa_reset_all_tests
 
     def rule(self, event):
         return event.get("eventtype") == "user.mfa.factor.reset_all"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py` & `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import okta_alert_context
 from pypanther.log_types import LogType
 
 okta_user_reported_suspicious_activity_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Other Event",
         ExpectedResult=False,
@@ -175,15 +175,15 @@
 
 class OktaUserReportedSuspiciousActivity(PantherRule):
     Description = "Suspicious Activity Reporting provides an end user with the option to report unrecognized activity from an account activity email notification.\nThis detection alerts when a user marks the raised activity as suspicious."
     Reference = (
         "https://help.okta.com/en-us/Content/Topics/Security/suspicious-activity-reporting.htm"
     )
     DisplayName = "Okta User Reported Suspicious Activity"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Okta_SystemLog]
     RuleID = "Okta.User.Reported.Suspicious.Activity-prototype"
     Tests = okta_user_reported_suspicious_activity_tests
 
     def rule(self, event):
         return event.get("eventtype") == "user.account.report_suspicious_activity_by_enduser"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import timedelta
 from typing import List
 
 from panther_detection_helpers.caching import add_to_string_set, get_string_set, put_string_set
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import is_ip_in_network
 from pypanther.log_types import LogType
 
 one_login_active_login_activity_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
@@ -35,15 +35,15 @@
 
 
 class OneLoginActiveLoginActivity(PantherRule):
     RuleID = "OneLogin.ActiveLoginActivity-prototype"
     DisplayName = "OneLogin Active Login Activity"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin", "Lateral Movement:Use Alternate Authentication Material"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0008:T1550"]}
     Description = "Multiple user accounts logged in from the same ip address."
     Reference = "https://support.onelogin.com/kb/4271392/user-policies"
     Runbook = "Investigate whether multiple user's logging in from the same ip address is expected. Determine if this ip address should be added to the SHARED_IP_SPACE array."
     SummaryAttributes = ["account_id", "user_name", "user_id"]
     Tests = one_login_active_login_activity_tests
     THRESH = 2
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_high_risk_failed_login_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
         Log={
@@ -31,15 +31,15 @@
 
 
 class OneLoginHighRiskFailedLogin(PantherRule):
     RuleID = "OneLogin.HighRiskFailedLogin-prototype"
     DisplayName = "OneLogin Failed High Risk Login"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = (
         "A OneLogin attempt with a high risk factor (>50) resulted in a failed authentication."
     )
     Reference = "https://resources.onelogin.com/OneLogin_RiskBasedAuthentication-WP-v5.pdf"
     Runbook = "Investigate why this user login is tagged as high risk as well as whether this was caused by expected user activity."
     SummaryAttributes = ["account_id", "user_name", "user_id"]
     Tests = one_login_high_risk_failed_login_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import timedelta
 from typing import List
 
 from panther_detection_helpers.caching import get_counter, increment_counter, reset_counter
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_high_risk_login_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
         Log={
@@ -22,15 +22,15 @@
 
 
 class OneLoginHighRiskLogin(PantherRule):
     RuleID = "OneLogin.HighRiskLogin-prototype"
     DisplayName = "OneLogin High Risk Login"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A OneLogin user successfully logged in after a failed high-risk login attempt."
     Reference = "https://resources.onelogin.com/OneLogin_RiskBasedAuthentication-WP-v5.pdf"
     Runbook = "Investigate whether this was caused by expected user activity."
     SummaryAttributes = ["account_id", "event_type_id", "user_name", "user_id"]
     Tests = one_login_high_risk_login_tests
     THRESH_TTL = timedelta(minutes=10).total_seconds()
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_password_accessed.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_password_accessed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_password_access_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User accessed their own password",
         ExpectedResult=False,
         Log={
@@ -31,15 +31,15 @@
 
 class OneLoginPasswordAccess(PantherRule):
     RuleID = "OneLogin.PasswordAccess-prototype"
     DisplayName = "OneLogin Password Access"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin", "Credential Access:Unsecured Credentials"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1552"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "User accessed another user's application password\n"
     Reference = "https://onelogin.service-now.com/kb_view_customer.do?sysparm_article=KB0010598"
     Runbook = "Investigate whether this was authorized access.\n"
     SummaryAttributes = ["account_id", "user_name", "user_id"]
     Tests = one_login_password_access_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_password_changed.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_password_changed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_password_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User changed their password",
         ExpectedResult=True,
         Log={
@@ -41,15 +41,15 @@
 
 
 class OneLoginPasswordChanged(PantherRule):
     RuleID = "OneLogin.PasswordChanged-prototype"
     DisplayName = "OneLogin User Password Changed"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin", "Identity & Access Management"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A user password was updated.\n"
     Reference = "https://onelogin.service-now.com/kb_view_customer.do?sysparm_article=KB0010510"
     Runbook = "Investigate whether this was an authorized action.\n"
     SummaryAttributes = ["account_id", "user_name", "user_id"]
     Tests = one_login_password_changed_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_auth_factor_removed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User removed an auth factor",
         ExpectedResult=True,
         Log={
@@ -37,15 +37,15 @@
     LogTypes = [LogType.OneLogin_Events]
     Tags = [
         "OneLogin",
         "Identity & Access Management",
         "Defense Evasion:Modify Authentication Process",
     ]
     Reports = {"MITRE ATT&CK": ["TA0005:T1556"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A user removed an authentication factor or otp device.\n"
     Reference = "https://onelogin.service-now.com/kb_view_customer.do?sysparm_article=KB0010426"
     Runbook = "Investigate whether this was an intentional action and if other multifactor devices exist.\n"
     SummaryAttributes = [
         "account_id",
         "event_type_id",
         "user_name",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_threshold_accounts_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal User Activated Event",
         ExpectedResult=False,
         Log={
@@ -30,15 +30,15 @@
 
 
 class OneLoginThresholdAccountsDeleted(PantherRule):
     RuleID = "OneLogin.ThresholdAccountsDeleted-prototype"
     DisplayName = "OneLogin Multiple Accounts Deleted"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin", "Impact:Account Access Removal"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0040:T1531"]}
     Description = (
         "Possible Denial of Service detected. Threshold for user account deletions exceeded.\n"
     )
     Threshold = 10
     DedupPeriodMinutes = 10
     Reference = "https://en.wikipedia.org/wiki/Denial-of-service_attack"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_threshold_accounts_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal User Activated Event",
         ExpectedResult=False,
         Log={
@@ -30,15 +30,15 @@
 
 
 class OneLoginThresholdAccountsModified(PantherRule):
     RuleID = "OneLogin.ThresholdAccountsModified-prototype"
     DisplayName = "OneLogin Multiple Accounts Modified"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin", "Impact:Account Access Removal"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0040:T1531"]}
     Description = "Possible Denial of Service detected. Threshold for user account password changes exceeded.\n"
     Threshold = 10
     DedupPeriodMinutes = 10
     Reference = "https://en.wikipedia.org/wiki/Denial-of-service_attack"
     Runbook = "Determine if this is normal user-cleanup activity."
     SummaryAttributes = ["account_id", "user_name", "user_id"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_unauthorized_access_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Event",
         ExpectedResult=False,
         Log={
@@ -29,15 +29,15 @@
 
 class OneLoginUnauthorizedAccess(PantherRule):
     RuleID = "OneLogin.UnauthorizedAccess-prototype"
     DisplayName = "OneLogin Unauthorized Access"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin", "Lateral Movement:Use Alternate Authentication Material"]
     Reports = {"MITRE ATT&CK": ["TA0008:T1550"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = (
         "A OneLogin user was denied access to an app more times than the configured threshold."
     )
     Threshold = 10
     DedupPeriodMinutes = 10
     Reference = "https://onelogin.service-now.com/kb_view_customer.do?sysparm_article=KB0010420"
     Runbook = "Analyze the user activity and actions."
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_user_account_locked_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User account locked via api - first method.",
         ExpectedResult=True,
         Log={
@@ -53,15 +53,15 @@
 
 class OneLoginUserAccountLocked(PantherRule):
     RuleID = "OneLogin.UserAccountLocked-prototype"
     DisplayName = "OneLogin User Locked"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin", "Credential Access:Brute Force"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "User locked or suspended from their account.\n"
     Reference = "https://onelogin.service-now.com/kb_view_customer.do?sysparm_article=KB0010420"
     Runbook = "Investigate whether this was caused by expected action.\n"
     SummaryAttributes = ["account_id", "event_type_id", "user_name", "user_id"]
     Tests = one_login_user_account_locked_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_user_assumed.py` & `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_user_assumed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 one_login_user_assumption_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User assumed their own account",
         ExpectedResult=False,
         Log={
@@ -31,15 +31,15 @@
 
 class OneLoginUserAssumption(PantherRule):
     RuleID = "OneLogin.UserAssumption-prototype"
     DisplayName = "OneLogin User Assumed Another User"
     LogTypes = [LogType.OneLogin_Events]
     Tags = ["OneLogin", "Lateral Movement:Use Alternate Authentication Material"]
     Reports = {"MITRE ATT&CK": ["TA0008:T1550"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "User assumed another user account"
     Reference = "https://onelogin.service-now.com/kb_view_customer.do?sysparm_article=KB0010594#:~:text=Prerequisites,Actions%20and%20select%20Assume%20User."
     Runbook = "Investigate whether this was authorized access.\n"
     SummaryAttributes = ["account_id", "user_name", "user_id"]
     Tests = one_login_user_assumption_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py` & `pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 one_password_lut_sensitive_item_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="1Password - Sensitive Item Accessed",
         ExpectedResult=True,
@@ -71,15 +71,15 @@
 class OnePasswordLutSensitiveItem(PantherRule):
     RuleID = "OnePassword.Lut.Sensitive.Item-prototype"
     DedupPeriodMinutes = 30
     DisplayName = "BETA - Sensitive 1Password Item Accessed"
     Enabled = False
     LogTypes = [LogType.OnePassword_ItemUsage]
     Reference = "https://support.1password.com/1password-com-items/"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Alerts when a user defined list of sensitive items in 1Password is accessed"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tags = [
         "Configuration Required",
         "1Password",
         "Lookup Table",
         "BETA",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py` & `pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 one_password_sensitive_item_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="1Password - Sensitive Item Accessed",
         ExpectedResult=True,
@@ -55,15 +55,15 @@
 class OnePasswordSensitiveItem(PantherRule):
     RuleID = "OnePassword.Sensitive.Item-prototype"
     DedupPeriodMinutes = 30
     DisplayName = "Configuration Required - Sensitive 1Password Item Accessed"
     Enabled = False
     LogTypes = [LogType.OnePassword_ItemUsage]
     Reference = "https://support.1password.com/1password-com-items/"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Alerts when a user defined list of sensitive items in 1Password is accessed"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tags = ["Configuration Required", "1Password", "Credential Access:Unsecured Credentials"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1552"]}
     Tests = one_password_sensitive_item_tests
     "\nThis rule detects access to high sensitivity items in your 1Password account. 1Password references\nthese items by their UUID so the SENSITIVE_ITEM_WATCHLIST below allows for the mapping of UUID to\nmeaningful name.\n\nThere is an alternative method for creating this rule that uses Panther's lookup table feature,\n(currently in beta). That rule can be found in the 1Password detection pack with the name\nBETA - Sensitive 1Password Item Accessed (onepassword_lut_sensitive_item_access.py)\n"
     SENSITIVE_ITEM_WATCHLIST = {"ecd1d435c26440dc930ddfbbef201a11": "demo_item"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_unusual_client.py` & `pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_unusual_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 one_password_unusual_client_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="1Password - Expected Client",
         ExpectedResult=False,
@@ -63,15 +63,15 @@
 
 
 class OnePasswordUnusualClient(PantherRule):
     RuleID = "OnePassword.Unusual.Client-prototype"
     DedupPeriodMinutes = 120
     DisplayName = "Unusual 1Password Client Detected"
     LogTypes = [LogType.OnePassword_SignInAttempt]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = (
         "Detects when unusual or undesirable 1Password clients access your 1Password account"
     )
     Reference = "https://support.1password.com/category/accounts/"
     Tags = ["1Password", "Credential Access:Credentials from Password Stores"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1555"]}
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import shlex
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_linux_aws_command_executed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="AWS command executed on MacOS",
         ExpectedResult=False,
@@ -82,15 +82,15 @@
 
 class OsqueryLinuxAWSCommandExecuted(PantherRule):
     RuleID = "Osquery.Linux.AWSCommandExecuted-prototype"
     DisplayName = "AWS command executed on the command line"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "Linux", "Execution:User Execution"]
     Reports = {"MITRE ATT&CK": ["TA0002:T1204"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "An AWS command was executed on a Linux instance"
     Runbook = "See which other commands were executed, and then remove IAM role causing the access"
     Reference = "https://attack.mitre.org/techniques/T1078/"
     SummaryAttributes = ["name", "action"]
     Tests = osquery_linux_aws_command_executed_tests
     PLATFORM_IGNORE_LIST = {"darwin"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ipaddress
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_linux_login_from_non_office_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Non-office network login (logged_in_users)",
         ExpectedResult=True,
@@ -46,15 +46,15 @@
 class OsqueryLinuxLoginFromNonOffice(PantherRule):
     RuleID = "Osquery.Linux.LoginFromNonOffice-prototype"
     DisplayName = "A Login from Outside the Corporate Office"
     Enabled = False
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Configuration Required", "Osquery", "Linux", "Initial Access:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1078"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A system has been logged into from a non approved IP space."
     Runbook = "Analyze the host IP, and if possible, update allowlist or fix ACL."
     Reference = "https://attack.mitre.org/techniques/T1078/"
     SummaryAttributes = ["name", "action", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = osquery_linux_login_from_non_office_tests
     # This is only an example network, but you can set it to whatever you'd like
     OFFICE_NETWORKS = [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 osquery_linux_mac_vulnerable_x_zliblzma_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Vulnerable liblzma",
         ExpectedResult=True,
         Log={
@@ -54,15 +54,15 @@
 
 class OsqueryLinuxMacVulnerableXZliblzma(PantherRule):
     RuleID = "Osquery.Linux.Mac.VulnerableXZliblzma-prototype"
     DisplayName = "A backdoored version of XZ or liblzma is vulnerable to CVE-2024-3094"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "MacOS", "Linux", "Emerging Threats", "Supply Chain Compromise"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1195.001"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects vulnerable versions of XZ and liblzma on Linux and MacOS using Osquery logs. Versions 5.6.0 and 5.6.1 of xz and liblzma are most likely vulnerable to backdoor exploit. Vuln management pack must be enabled: https://github.com/osquery/osquery/blob/master/packs/vuln-management.conf\n"
     Runbook = "Upgrade/downgrade xz and liblzma to non-vulnerable versions"
     Reference = "https://gist.github.com/jamesspi/ee8319f55d49b4f44345c626f80c430f"
     SummaryAttributes = ["name", "hostIdentifier", "action"]
     Tests = osquery_linux_mac_vulnerable_x_zliblzma_tests
     QUERY_NAMES = {
         "pack_vuln-management_homebrew_packages",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_mac_application_firewall_settings_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="ALF Disabled",
         ExpectedResult=True,
@@ -46,15 +46,15 @@
 
 class OsqueryMacApplicationFirewallSettings(PantherRule):
     RuleID = "Osquery.Mac.ApplicationFirewallSettings-prototype"
     DisplayName = "MacOS ALF is misconfigured"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "MacOS", "Security Control", "Defense Evasion:Impair Defenses"]
     Reports = {"CIS": ["2.6.3", "2.6.4"], "MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "The application level firewall blocks unwanted network connections made to your computer from other computers on your network.\n"
     Runbook = "Re-enable the firewall manually or with configuration management"
     Reference = "https://support.apple.com/en-us/HT201642"
     SummaryAttributes = ["name", "hostIdentifier", "action"]
     Tests = osquery_mac_application_firewall_settings_tests
     QUERIES = {"pack_incident-response_alf", "pack/mac-cis/ApplicationFirewall"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_mac_auto_update_enabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Auto Updates Disabled",
         ExpectedResult=True,
@@ -49,15 +49,15 @@
 
 class OsqueryMacAutoUpdateEnabled(PantherRule):
     RuleID = "Osquery.Mac.AutoUpdateEnabled-prototype"
     DisplayName = "OSQuery Reports Application Firewall Disabled"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "MacOS", "Security Control", "Defense Evasion:Impair Defenses"]
     Reports = {"CIS": ["1.2"], "MITRE ATT&CK": ["TA0005:T1562"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     DedupPeriodMinutes = 1440
     Description = "Verifies that MacOS has automatic software updates enabled.\n"
     Runbook = "Enable the auto updates on the host.\n"
     Reference = "https://support.apple.com/en-gb/guide/mac-help/mchlpx1065/mac"
     SummaryAttributes = ["name", "action", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = osquery_mac_auto_update_enabled_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 osquery_mac_osx_attacks_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Valid malware discovered",
         ExpectedResult=True,
         Log={
@@ -37,15 +37,15 @@
 
 class OsqueryMacOSXAttacks(PantherRule):
     RuleID = "Osquery.Mac.OSXAttacks-prototype"
     DisplayName = "macOS Malware Detected with osquery"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "MacOS", "Malware", "Resource Development:Develop Capabilities"]
     Reports = {"MITRE ATT&CK": ["TA0042:T1588"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Malware has potentially been detected on a macOS system"
     Runbook = "Check the executable against VirusTotal"
     Reference = "https://github.com/osquery/osquery/blob/master/packs/osx-attacks.conf"
     SummaryAttributes = ["name", "hostIdentifier", "action"]
     Tests = osquery_mac_osx_attacks_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fnmatch import fnmatch
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_mac_osx_attacks_keyboard_events_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="App running on Desktop that is watching keyboard events",
         ExpectedResult=True,
@@ -69,15 +69,15 @@
 
 class OsqueryMacOSXAttacksKeyboardEvents(PantherRule):
     RuleID = "Osquery.Mac.OSXAttacksKeyboardEvents-prototype"
     DisplayName = "MacOS Keyboard Events"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "MacOS", "Malware", "Collection:Input Capture"]
     Reports = {"MITRE ATT&CK": ["TA0009:T1056"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A Key Logger has potentially been detected on a macOS system"
     Runbook = "Verify the Application monitoring the keyboard taps"
     Reference = "https://support.apple.com/en-us/HT204899"
     SummaryAttributes = ["name", "hostIdentifier", "action"]
     Tests = osquery_mac_osx_attacks_keyboard_events_tests
     # sip protects against writing malware into the paths below.
     # additional apps can be added to this list based on your environments.
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 osquery_mac_unwanted_chrome_extensions_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Unwanted Extension Detected",
         ExpectedResult=True,
         Log={
@@ -77,15 +77,15 @@
 
 class OsqueryMacUnwantedChromeExtensions(PantherRule):
     RuleID = "Osquery.Mac.UnwantedChromeExtensions-prototype"
     DisplayName = "OSQuery Detected Unwanted Chrome Extensions"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "MacOS", "Malware", "Persistence:Browser Extensions"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1176"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Monitor for chrome extensions that could lead to a credential compromise.\n"
     Runbook = "Uninstall the unwanted extension"
     Reference = "https://securelist.com/threat-in-your-browser-extensions/107181/"
     SummaryAttributes = ["action", "hostIdentifier", "name"]
     Tests = osquery_mac_unwanted_chrome_extensions_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_ossec.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_ossec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 osquery_ossec_rootkit_detected_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Rootkit Detected",
         ExpectedResult=True,
         Log={
@@ -75,15 +75,15 @@
 
 class OsqueryOSSECRootkitDetected(PantherRule):
     RuleID = "Osquery.OSSECRootkitDetected-prototype"
     DisplayName = "OSSEC Rootkit Detected via Osquery"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "Malware", "Defense Evasion:Rootkit"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1014"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Checks if any results are returned for the Osquery OSSEC Rootkit pack.\n"
     Runbook = "Verify the presence of the rootkit and re-image the machine.\n"
     Reference = "https://panther.com/blog/osquery-log-analysis/"
     SummaryAttributes = ["name", "hostIdentifier", "action"]
     Tests = osquery_ossec_rootkit_detected_tests
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_outdated.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_outdated.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_outdated_agent_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="osquery out of date",
         ExpectedResult=True,
@@ -75,15 +75,15 @@
 
 
 class OsqueryOutdatedAgent(PantherRule):
     RuleID = "Osquery.OutdatedAgent-prototype"
     DisplayName = "Osquery Agent Outdated"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "Compliance"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "Keep track of osquery versions, current is 5.10.2."
     Runbook = "Update the osquery agent."
     Reference = "https://www.osquery.io/downloads/official/5.10.2"
     SummaryAttributes = ["name", "hostIdentifier", "action"]
     Tests = osquery_outdated_agent_tests
     LATEST_VERSION = "5.10.2"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_outdated_macos.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_outdated_macos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_unsupported_mac_os_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="MacOS out of date",
         ExpectedResult=True,
@@ -77,15 +77,15 @@
 
 
 class OsqueryUnsupportedMacOS(PantherRule):
     RuleID = "Osquery.UnsupportedMacOS-prototype"
     DisplayName = "Unsupported macOS version"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "Compliance"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Check that all laptops on the corporate environment are on a version of MacOS supported by IT.\n"
     Runbook = "Update the MacOs version"
     Reference = "https://support.apple.com/en-eg/HT201260"
     SummaryAttributes = ["name", "hostIdentifier", "action"]
     Tests = osquery_unsupported_mac_os_tests
     SUPPORTED_VERSIONS = ["10.15.1", "10.15.2", "10.15.3"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_ssh_listener.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_ssh_listener.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_ssh_listener_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="SSH Listener Detected",
         ExpectedResult=True,
@@ -78,15 +78,15 @@
 
 class OsquerySSHListener(PantherRule):
     RuleID = "Osquery.SSHListener-prototype"
     DisplayName = "OSQuery Detected SSH Listener"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "Lateral Movement:Remote Services"]
     Reports = {"MITRE ATT&CK": ["TA0008:T1021"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Check if SSH is listening in a non-production environment. This could be an indicator of persistent access within an environment.\n"
     Runbook = "Terminate the SSH daemon, investigate for signs of compromise.\n"
     Reference = (
         "https://medium.com/uptycs/osquery-what-it-is-how-it-works-and-how-to-use-it-ce4e81e60dfc"
     )
     SummaryAttributes = ["action", "hostIdentifier", "name"]
     Tests = osquery_ssh_listener_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_suspicious_cron.py` & `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_suspicious_cron.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import shlex
 from fnmatch import fnmatch
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 osquery_suspicious_cron_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Netcat Listener",
         ExpectedResult=True,
@@ -126,15 +126,15 @@
 
 class OsquerySuspiciousCron(PantherRule):
     RuleID = "Osquery.SuspiciousCron-prototype"
     DisplayName = "Suspicious cron detected"
     LogTypes = [LogType.Osquery_Differential]
     Tags = ["Osquery", "Execution:Scheduled Task/Job"]
     Reports = {"MITRE ATT&CK": ["TA0002:T1053"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A suspicious cron has been added"
     Runbook = "Analyze the command to ensure no nefarious activity is occurring"
     Reference = "https://en.wikipedia.org/wiki/Cron"
     SummaryAttributes = ["action", "hostIdentifier", "name"]
     Tests = osquery_suspicious_cron_tests
     # Running in unexpected locations
     # nosec
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_detection_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_detection_deleted.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 panther_detection_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Delete 1 Detection",
         ExpectedResult=True,
@@ -88,15 +88,15 @@
 ]
 
 
 class PantherDetectionDeleted(PantherRule):
     RuleID = "Panther.Detection.Deleted-prototype"
     DisplayName = "Detection content has been deleted from Panther"
     LogTypes = [LogType.Panther_Audit]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Tags = ["DataModel", "Defense Evasion:Impair Defenses"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
     Description = "Detection content has been removed from Panther."
     Runbook = "Ensure this change was approved and appropriate."
     Reference = "https://docs.panther.com/system-configuration/panther-audit-logs/querying-and-writing-detections-for-panther-audit-logs"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = panther_detection_deleted_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_saml_modified.py` & `pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_saml_modified.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 panther_saml_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="SAML config modified",
         ExpectedResult=True,
         Log={
@@ -49,15 +49,15 @@
 ]
 
 
 class PantherSAMLModified(PantherRule):
     RuleID = "Panther.SAML.Modified-prototype"
     DisplayName = "Panther SAML configuration has been modified"
     LogTypes = [LogType.Panther_Audit]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["DataModel", "Defense Evasion:Impair Defenses"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562"]}
     Description = "An Admin has modified Panther's SAML configuration."
     Runbook = "Ensure this change was approved and appropriate."
     Reference = "https://docs.panther.com/system-configuration/saml"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_usernames"]
     Tests = panther_saml_modified_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py` & `pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 panther_sensitive_role_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Admin Role Created",
         ExpectedResult=True,
@@ -160,15 +160,15 @@
 ]
 
 
 class PantherSensitiveRole(PantherRule):
     RuleID = "Panther.Sensitive.Role-prototype"
     DisplayName = "A User Role with Sensitive Permissions has been Created"
     LogTypes = [LogType.Panther_Audit]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["DataModel", "Persistence:Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Description = "A Panther user role has been created that contains admin level permissions."
     Runbook = "Contact the creator of this role to ensure its creation was appropriate."
     Reference = "https://docs.panther.com/system-configuration/rbac"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = panther_sensitive_role_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_user_modified.py` & `pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_user_modified.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 panther_user_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Admin Role Created",
         ExpectedResult=False,
@@ -187,15 +187,15 @@
 ]
 
 
 class PantherUserModified(PantherRule):
     RuleID = "Panther.User.Modified-prototype"
     DisplayName = "A User's Panther Account was Modified"
     LogTypes = [LogType.Panther_Audit]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["DataModel", "Persistence:Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1098"]}
     Description = "A Panther user's role has been modified. This could mean password, email, or role has changed for the user."
     Runbook = "Validate that this user modification was intentional."
     Reference = (
         "https://docs.panther.com/panther-developer-workflows/api/operations/user-management"
     )
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py` & `pypanther-0.1.1a8/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 salesforce_admin_login_as_user_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Normal Login Event",
         ExpectedResult=False,
         Log={
@@ -87,15 +87,15 @@
 class SalesforceAdminLoginAsUser(PantherRule):
     Description = "Salesforce detection that alerts when an admin logs in as another user. "
     DisplayName = "Salesforce Admin Login As User"
     Runbook = "Please do an indicator search on USER_ID to find which user was assumed. "
     Reference = (
         "https://help.salesforce.com/s/articleView?id=sf.logging_in_as_another_user.htm&type=5"
     )
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     LogTypes = [LogType.Salesforce_LoginAs]
     RuleID = "Salesforce.Admin.Login.As.User-prototype"
     Tests = salesforce_admin_login_as_user_tests
 
     def rule(self, event):
         return event.get("EVENT_TYPE", "<NO_EVENT_TYPE_FOUND>") == "LoginAs"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py` & `pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 sentinel_one_alert_passthrough_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="CRITICAL",
         ExpectedResult=True,
@@ -139,15 +139,15 @@
 
 class SentinelOneAlertPassthrough(PantherRule):
     Description = "SentinelOne Alert Passthrough"
     DisplayName = "SentinelOne Alert Passthrough"
     Reference = (
         "https://www.sentinelone.com/blog/feature-spotlight-introducing-the-new-threat-center/"
     )
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.SentinelOne_Activity]
     RuleID = "SentinelOne.Alert.Passthrough-prototype"
     Tests = sentinel_one_alert_passthrough_tests
     SENTINELONE_SEVERITY = {
         "E_LOW": "LOW",
         "E_MEDIUM": "MEDIUM",
         "E_HIGH": "HIGH",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/sentinelone_threats.py` & `pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/sentinelone_threats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.log_types import LogType
 
 sentinel_one_threats_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="malicious event",
         ExpectedResult=True,
@@ -111,15 +111,15 @@
 
 class SentinelOneThreats(PantherRule):
     Description = "Passthrough SentinelOne Threats "
     DisplayName = "SentinelOne Threats"
     Reference = (
         "https://www.sentinelone.com/blog/feature-spotlight-introducing-the-new-threat-center/"
     )
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.SentinelOne_Activity]
     RuleID = "SentinelOne.Threats-prototype"
     Tests = sentinel_one_threats_tests  # New Malicious Threat Not Mitigated
     # New Malicious Threat Not Mitigated
     # New Suspicious Threat Not Mitigated
     # New Suspicious Threat Not Mitigated
     NEW_THREAT_ACTIVITYTYPES = [19, 4108, 4003, 4109]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_access_expanded.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_access_expanded.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_app_access_expanded_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="App Scopes Expanded",
         ExpectedResult=True,
@@ -226,15 +226,15 @@
 
 class SlackAuditLogsAppAccessExpanded(PantherRule):
     RuleID = "Slack.AuditLogs.AppAccessExpanded-prototype"
     DisplayName = "Slack App Access Expanded"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Privilege Escalation", "Account Manipulation"]
     Reports = {"MITRE ATT&CK": ["TA0004:T1098"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when a Slack App has had its permission scopes expanded"
     Reference = "https://slack.com/intl/en-gb/help/articles/1500009181142-Manage-app-settings-and-permissions"
     SummaryAttributes = ["action", "p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_app_access_expanded_tests
     ACCESS_EXPANDED_ACTIONS = [
         "app_scopes_expanded",
         "app_resources_added",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_added.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_added.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_app_added_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="App added to workspace - Admin not in app scopes",
         ExpectedResult=True,
@@ -210,15 +210,15 @@
 
 class SlackAuditLogsAppAdded(PantherRule):
     RuleID = "Slack.AuditLogs.AppAdded-prototype"
     DisplayName = "Slack App Added"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Persistence", "Server Software Component"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1505"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when a Slack App has been added to a workspace"
     Reference = (
         "https://slack.com/intl/en-gb/help/articles/202035138-Add-apps-to-your-Slack-workspace"
     )
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_app_added_tests
     APP_ADDED_ACTIONS = ["app_approved", "app_installed", "org_app_workspace_added"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_removed.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_removed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_app_removed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="App Restricted",
         ExpectedResult=True,
@@ -168,15 +168,15 @@
         "Impact",
         "Service Stop",
         "Defense Evasion",
         "Indicator Removal",
         "Clear Persistence",
     ]
     Reports = {"MITRE ATT&CK": ["TA0040:T1489", "TA0005:T1070.009"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when a Slack App has been removed"
     Reference = "https://slack.com/intl/en-gb/help/articles/360003125231-Remove-apps-and-customised-integrations-from-your-workspace"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_app_removed_tests
     APP_REMOVED_ACTIONS = ["app_restricted", "app_uninstalled", "org_app_workspace_removed"]
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_application_dos.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_application_dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import timedelta
 from json import dumps
 from typing import List
 
 from panther_detection_helpers.caching import get_string_set, put_string_set
 
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get, slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_application_do_s_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User Session Reset - First time",
         ExpectedResult=False,
@@ -74,15 +74,15 @@
 
 class SlackAuditLogsApplicationDoS(PantherRule):
     RuleID = "Slack.AuditLogs.ApplicationDoS-prototype"
     DisplayName = "Slack Denial of Service"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Impact", "Endpoint Denial of Service", "Application Exhaustion Flood"]
     Reports = {"MITRE ATT&CK": ["TA0040:T1499.003"]}
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Description = "Detects when slack admin invalidates user session(s) more than once in a 24 hour period which can lead to DoS"
     Reference = "https://slack.com/intl/en-gb/help/articles/115005223763-Manage-session-duration-#pro-and-business+-subscriptions-2"
     Threshold = 60
     SummaryAttributes = ["action", "p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_application_do_s_tests
     DENIAL_OF_SERVICE_ACTIONS = [
         "bulk_session_reset_by_admin",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_dlp_modified.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_dlp_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_dlp_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Native DLP Rule Deactivated",
         ExpectedResult=True,
@@ -105,15 +105,15 @@
         "Slack",
         "Defense Evasion",
         "Impair Defenses",
         "Disable or Modify Tools",
         "Indicator Removal",
     ]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562.001", "TA0005:T1070"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when a Data Loss Prevention (DLP) rule has been deactivated or a violation has been deleted\n"
     Reference = "https://slack.com/intl/en-gb/help/articles/12914005852819-Slack-Connect--Data-loss-prevention"
     SummaryAttributes = ["action", "p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_dlp_modified_tests
     DLP_ACTIONS = ["native_dlp_rule_deactivated", "native_dlp_violation_deleted"]
     # DLP violations can be removed by security engineers in the case of FPs
     # We still want to alert on these, however those should not constitute a High severity
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_config_changed.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_config_changed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_ekm_config_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="EKM Config Changed",
         ExpectedResult=True,
@@ -73,15 +73,15 @@
 
 class SlackAuditLogsEKMConfigChanged(PantherRule):
     RuleID = "Slack.AuditLogs.EKMConfigChanged-prototype"
     DisplayName = "Slack EKM Config Changed"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Defense Evasion", "Impair Defenses", "Disable or Modify Cloud Logs"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562.008"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "Detects when the logging settings for a workspace's EKM configuration has changed"
     )
     Reference = (
         "https://slack.com/intl/en-gb/help/articles/360019110974-Slack-Enterprise-Key-Management"
     )
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_ekm_slackbot_unenrolled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="EKM Slackbot Unenrolled",
         ExpectedResult=True,
@@ -73,15 +73,15 @@
 
 class SlackAuditLogsEKMSlackbotUnenrolled(PantherRule):
     RuleID = "Slack.AuditLogs.EKMSlackbotUnenrolled-prototype"
     DisplayName = "Slack EKM Slackbot Unenrolled"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Impact", "Service Stop"]
     Reports = {"MITRE ATT&CK": ["TA0040:T1489"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when a workspace is longer enrolled in EKM"
     Reference = (
         "https://slack.com/intl/en-gb/help/articles/360019110974-Slack-Enterprise-Key-Management"
     )
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_ekm_slackbot_unenrolled_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_unenrolled.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_unenrolled.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_ekm_unenrolled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="EKM Unenrolled",
         ExpectedResult=True,
@@ -73,15 +73,15 @@
 
 class SlackAuditLogsEKMUnenrolled(PantherRule):
     RuleID = "Slack.AuditLogs.EKMUnenrolled-prototype"
     DisplayName = "Slack EKM Unenrolled"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Defense Evasion", "Weaken Encryption"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1600"]}
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Description = "Detects when a workspace is no longer enrolled or managed by EKM"
     Reference = (
         "https://slack.com/intl/en-gb/help/articles/360019110974-Slack-Enterprise-Key-Management"
     )
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_ekm_unenrolled_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_idp_configuration_change.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_idp_configuration_change.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_idp_configuration_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="IDP Configuration Added",
         ExpectedResult=True,
@@ -128,15 +128,15 @@
 
 class SlackAuditLogsIDPConfigurationChanged(PantherRule):
     RuleID = "Slack.AuditLogs.IDPConfigurationChanged-prototype"
     DisplayName = "Slack IDP Configuration Changed"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Persistence", "Credential Access", "Modify Authentication Process"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1556", "TA0006:T1556"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "Detects changes to the identity provider (IdP) configuration for Slack organizations."
     )
     Reference = "https://slack.com/intl/en-gb/help/articles/115001435788-Connect-identity-provider-groups-to-your-Enterprise-Grid-org"
     SummaryAttributes = ["action", "p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_idp_configuration_changed_tests
     IDP_CHANGE_ACTIONS = {
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_information_barrier_modified.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_information_barrier_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_information_barrier_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Information Barrier Deleted",
         ExpectedResult=True,
@@ -99,15 +99,15 @@
 
 class SlackAuditLogsInformationBarrierModified(PantherRule):
     RuleID = "Slack.AuditLogs.InformationBarrierModified-prototype"
     DisplayName = "Slack Information Barrier Modified"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Defense Evasion", "Impair Defenses", "Disable or Modify Tools"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562.001"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when a Slack information barrier is deleted/updated"
     Reference = "https://slack.com/intl/en-gb/help/articles/360056171734-Create-information-barriers-in-Slack"
     SummaryAttributes = ["action", "p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_information_barrier_modified_tests
     INFORMATION_BARRIER_ACTIONS = {
         "barrier_deleted": "Slack Information Barrier Deleted",
         "barrier_updated": "Slack Information Barrier Updated",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_intune_mdm_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Intune Disabled",
         ExpectedResult=True,
@@ -73,15 +73,15 @@
 
 class SlackAuditLogsIntuneMDMDisabled(PantherRule):
     RuleID = "Slack.AuditLogs.IntuneMDMDisabled-prototype"
     DisplayName = "Slack Intune MDM Disabled"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Defense Evasion", "Impair Defenses", "Disable or Modify Tools"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562.001"]}
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Description = "Detects the disabling of Microsoft Intune Enterprise MDM within Slack"
     Reference = "https://slack.com/intl/en-gb/help/articles/6495319642387-Set-up-Slack-for-Intune-mobile-apps"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_intune_mdm_disabled_tests
 
     def rule(self, event):
         return event.get("action") == "intune_disabled"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_legal_hold_policy_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Legal Hold - Entities Deleted",
         ExpectedResult=True,
@@ -151,15 +151,15 @@
 
 class SlackAuditLogsLegalHoldPolicyModified(PantherRule):
     RuleID = "Slack.AuditLogs.LegalHoldPolicyModified-prototype"
     DisplayName = "Slack Legal Hold Policy Modified"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Defense Evasion", "Impair Defenses", "Disable or Modify Tools"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1562.001"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects changes to configured legal hold policies"
     Reference = (
         "https://slack.com/intl/en-gb/help/articles/4401830811795-Create-and-manage-legal-holds"
     )
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_legal_hold_policy_modified_tests
     LEGAL_HOLD_POLICY_ACTIONS = {
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_mfa_settings_changed.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_mfa_settings_changed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_mfa_settings_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="MFA Auth Changed",
         ExpectedResult=True,
@@ -78,15 +78,15 @@
     Tags = [
         "Slack",
         "Defense Evasion",
         "Modify Authentication Process",
         "Multi-Factor Authentication",
     ]
     Reports = {"MITRE ATT&CK": ["TA0005:T1556.006"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects changes to Multi-Factor Authentication requirements"
     Reference = (
         "https://slack.com/intl/en-gb/help/articles/204509068-Set-up-two-factor-authentication"
     )
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_mfa_settings_changed_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_org_created.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_org_created.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_org_created_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Organization Created",
         ExpectedResult=True,
@@ -62,15 +62,15 @@
 
 class SlackAuditLogsOrgCreated(PantherRule):
     RuleID = "Slack.AuditLogs.OrgCreated-prototype"
     DisplayName = "Slack Organization Created"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Persistence", "Create Account"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1136"]}
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Detects when a Slack organization is created"
     Reference = "https://slack.com/intl/en-gb/help/articles/206845317-Create-a-Slack-workspace"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_org_created_tests
 
     def rule(self, event):
         return event.get("action") == "organization_created"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_org_deleted.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_org_deleted.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_org_deleted_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Organization Deleted",
         ExpectedResult=True,
@@ -62,15 +62,15 @@
 
 class SlackAuditLogsOrgDeleted(PantherRule):
     RuleID = "Slack.AuditLogs.OrgDeleted-prototype"
     DisplayName = "Slack Organization Deleted"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Impact", "Account Access Removal"]
     Reports = {"MITRE ATT&CK": ["TA0040:T1531"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when a Slack organization is deleted"
     Reference = "https://slack.com/intl/en-gb/help/articles/204067366-Delete-a-workspace"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_org_deleted_tests
 
     def rule(self, event):
         return event.get("action") == "organization_deleted"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_passthrough_anomaly.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_passthrough_anomaly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_passthrough_anomaly_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Name",
         ExpectedResult=True,
@@ -73,15 +73,15 @@
 
 class SlackAuditLogsPassthroughAnomaly(PantherRule):
     RuleID = "Slack.AuditLogs.PassthroughAnomaly-prototype"
     DisplayName = "Slack Anomaly Detected"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Command and Control", "Application Layer Protocol"]
     Reports = {"MITRE ATT&CK": ["TA0011:T1071"]}
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Description = "Passthrough for anomalies detected by Slack"
     Reference = "https://slack.com/intl/en-in/blog/news/three-new-security-features-to-protect-your-digital-hq"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_passthrough_anomaly_tests
 
     def rule(self, event):
         return event.get("action") == "anomaly"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_potentially_malicious_file_shared_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Malicious Content Detected",
         ExpectedResult=True,
@@ -73,15 +73,15 @@
 
 class SlackAuditLogsPotentiallyMaliciousFileShared(PantherRule):
     RuleID = "Slack.AuditLogs.PotentiallyMaliciousFileShared-prototype"
     DisplayName = "Slack Potentially Malicious File Shared"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Initial Access", "Phishing", "Spearphising Attachment"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1566.001"]}
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Description = "Detects when a potentially malicious file is shared within Slack"
     Reference = "https://threatpost.com/slack-remote-file-hijacking-malware/144871/"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_potentially_malicious_file_shared_tests
 
     def rule(self, event):
         return event.get("action") == "file_malicious_content_detected"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_private_channel_made_public.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_private_channel_made_public.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_private_channel_made_public_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Private Channel Made Public",
         ExpectedResult=True,
@@ -81,15 +81,15 @@
         "File and Directory Permissions Modification",
         "Persistence",
         "Account Manipulation",
         "Exfiltration",
         "Exfiltration Over Web Service",
     ]
     Reports = {"MITRE ATT&CK": ["TA0005:T1222", "TA0003:T1098", "TA0010:T1567"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when a channel that was previously private is made public"
     Reference = "https://slack.com/intl/en-gb/help/articles/213185467-Convert-a-channel-to-private-or-public"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_private_channel_made_public_tests
 
     def rule(self, event):
         return event.get("action") == "private_channel_converted_to_public"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_user_privilege_changed_to_user_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Role Changed to User",
         ExpectedResult=True,
@@ -84,15 +84,15 @@
 
 class SlackAuditLogsUserPrivilegeChangedToUser(PantherRule):
     RuleID = "Slack.AuditLogs.UserPrivilegeChangedToUser-prototype"
     DisplayName = "Slack User Privileges Changed to User"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Impact", "Account Access Removal"]
     Reports = {"MITRE ATT&CK": ["TA0040:T1531"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when a Slack account is changed to User from an elevated role."
     Reference = "https://slack.com/intl/en-gb/help/articles/360018112273-Types-of-roles-in-Slack"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_user_privilege_changed_to_user_tests
 
     def rule(self, event):
         return event.get("action") == "role_change_to_user"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_service_owner_transferred.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_service_owner_transferred.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_service_owner_transferred_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Service Owner Transferred",
         ExpectedResult=True,
@@ -81,15 +81,15 @@
         "File and Directory Permissions Modification",
         "Persistence",
         "Account Manipulation",
         "Impact",
         "Account Access Removal",
     ]
     Reports = {"MITRE ATT&CK": ["TA0005:T1222", "TA0003:T1098", "TA0040:T1531"]}
-    Severity = Severity.Critical
+    Severity = PantherSeverity.Critical
     Description = "Detects transferring of service owner on request from primary owner"
     Reference = "https://slack.com/intl/en-gb/help/articles/204401633-Transfer-ownership-of-a-workspace-or-org"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_service_owner_transferred_tests
 
     def rule(self, event):
         return event.get("action") == "service_owner_transferred"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_sso_settings_changed.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_sso_settings_changed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_sso_settings_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="SSO Setting Changed",
         ExpectedResult=True,
@@ -73,15 +73,15 @@
 
 class SlackAuditLogsSSOSettingsChanged(PantherRule):
     RuleID = "Slack.AuditLogs.SSOSettingsChanged-prototype"
     DisplayName = "Slack SSO Settings Changed"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Credential Access", "Persistence", "Modify Authentication Process"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1556", "TA0006:T1556"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects changes to Single Sign On (SSO) restrictions"
     Reference = (
         "https://slack.com/intl/en-gb/help/articles/220403548-Manage-single-sign-on-settings"
     )
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_sso_settings_changed_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_user_privilege_escalation.py` & `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_user_privilege_escalation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get, slack_alert_context
 from pypanther.log_types import LogType
 
 slack_audit_logs_user_privilege_escalation_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Owner Transferred",
         ExpectedResult=True,
@@ -151,15 +151,15 @@
 
 class SlackAuditLogsUserPrivilegeEscalation(PantherRule):
     RuleID = "Slack.AuditLogs.UserPrivilegeEscalation-prototype"
     DisplayName = "Slack User Privilege Escalation"
     LogTypes = [LogType.Slack_AuditLogs]
     Tags = ["Slack", "Privilege Escalation", "Account Manipulation", "Additional Cloud Roles"]
     Reports = {"MITRE ATT&CK": ["TA0004:T1098.003"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when a Slack user gains escalated privileges"
     Reference = "https://slack.com/intl/en-gb/help/articles/201314026-Permissions-by-role-in-Slack"
     SummaryAttributes = ["p_any_ip_addresses", "p_any_emails"]
     Tests = slack_audit_logs_user_privilege_escalation_tests
     USER_PRIV_ESC_ACTIONS = {
         "owner_transferred": "Slack Owner Transferred",
         "permissions_assigned": "Slack User Assigned Permissions",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_misc_settings.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_misc_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_misc_settings_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk Feature Flags changed",
@@ -34,15 +34,15 @@
 
 class SnykMiscSettings(PantherRule):
     RuleID = "Snyk.Misc.Settings-prototype"
     DisplayName = "Snyk Miscellaneous Settings"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
     Reference = "https://docs.snyk.io/snyk-admin/manage-settings"
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Detects when Snyk settings that lack a clear security impact are changed\n"
     SummaryAttributes = ["event"]
     Tests = snyk_misc_settings_tests
     ACTIONS = ["group.cloud_config.settings.edit", "group.feature_flags.edit"]
 
     def rule(self, event):
         action = deep_get(event, "event", default="<NO_EVENT>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_org_settings.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_org_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_org_settings_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="placeholder",
@@ -68,15 +68,15 @@
 
 class SnykOrgSettings(PantherRule):
     RuleID = "Snyk.Org.Settings-prototype"
     DisplayName = "Snyk Org Settings"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
     Reference = "https://docs.snyk.io/snyk-admin/manage-settings/organization-general-settings"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = (
         "Detects when Snyk Organization settings, like Integrations and Webhooks, are changed\n"
     )
     SummaryAttributes = ["event"]
     Tests = snyk_org_settings_tests
     ACTIONS = [
         "org.integration.create",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_ou_change.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_ou_change.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_ou_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk Org Deletion ( HIGH )",
@@ -65,15 +65,15 @@
 
 
 class SnykOUChange(PantherRule):
     RuleID = "Snyk.OU.Change-prototype"
     DisplayName = "Snyk Org or Group Settings Change"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when Snyk Group or Organization Settings are changed.\n"
     Runbook = "These actions in the Snyk Audit logs indicate that a Organization or  Group setting has changed, including Group and Org creation/deletion. Deletion events are marked with HIGH severity Creation events are marked with INFO severity Edit events are marked with MEDIUM Severity\n"
     Reference = "https://docs.snyk.io/snyk-admin/introduction-to-snyk-administration"
     SummaryAttributes = ["event"]
     Tests = snyk_ou_change_tests
     ACTIONS = [
         "group.create",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_project_settings.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_project_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_project_settings_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk Org Project Stop Monitor",
@@ -64,15 +64,15 @@
 
 class SnykProjectSettings(PantherRule):
     RuleID = "Snyk.Project.Settings-prototype"
     DisplayName = "Snyk Project Settings"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
     Reference = "https://docs.snyk.io/snyk-admin/introduction-to-snyk-projects/view-and-edit-project-settings"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when Snyk Project settings are changed\n"
     SummaryAttributes = ["event"]
     Tests = snyk_project_settings_tests
     # The bodies of these actions are quite diverse.
     # When projects are added, the logged detail is the sourceOrgId.
     # org.project.stop_monitor is logged for individual files
     #   that are ignored.
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_role_change.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_role_change.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_role_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk Group Role Edit -  ADMIN role ( CRIT )",
@@ -71,15 +71,15 @@
 
 
 class SnykRoleChange(PantherRule):
     RuleID = "Snyk.Role.Change-prototype"
     DisplayName = "Snyk Role Change"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when Snyk Roles are changed\n"
     Runbook = "These actions in the Snyk Audit logs indicate that a ServiceAccount has been created/deleted/modified.\nAll events where the Role is marked as ADMIN have CRITICAL severity Other events are marked with MEDIUM severity\n"
     Reference = "https://docs.snyk.io/snyk-admin/manage-users-and-permissions/member-roles"
     SummaryAttributes = ["event"]
     Tests = snyk_role_change_tests
     ACTIONS = [
         "group.role.create",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_svcacct_change.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_svcacct_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_service_account_change_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk Org Service Account ADMIN role ( CRIT )",
@@ -208,15 +208,15 @@
 
 
 class SnykServiceAccountChange(PantherRule):
     RuleID = "Snyk.ServiceAccount.Change-prototype"
     DisplayName = "Snyk Service Account Change"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when Snyk Service Accounts are changed\n"
     Runbook = "These actions in the Snyk Audit logs indicate that a ServiceAccount has been created/deleted/modified.\nService Accounts are system user accounts with an API token  associated to it in place of standard user credentials. All events where the Service Account's role is ADMIN have CRITICAL severity Deletion events are marked with HIGH severity Creation events are marked with HIGH severity Edit events are marked with MEDIUM Severity\n"
     Reference = "https://docs.snyk.io/snyk-admin/service-accounts"
     SummaryAttributes = ["event"]
     Tests = snyk_service_account_change_tests
     ACTIONS = [
         "group.service_account.create",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_externalaccess.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_externalaccess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_system_external_access_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk External Access Allowed By External Parties - Enabled",
@@ -49,15 +49,15 @@
 
 
 class SnykSystemExternalAccess(PantherRule):
     RuleID = "Snyk.System.ExternalAccess-prototype"
     DisplayName = "Snyk System External Access Settings Changed"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "Detects when Snyk Settings that control access for external parties have been changed.\n"
     )
     Runbook = "This action in the Snyk Audit logs indicate that the setting for allowing external parties to request access to your Snyk installation have changed.\n"
     Reference = (
         "https://docs.snyk.io/snyk-admin/manage-users-and-permissions/organization-access-requests"
     )
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_policysetting.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_policysetting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_system_policy_setting_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk System Policy Setting event happened ( Security Policy )",
@@ -96,15 +96,15 @@
 
 
 class SnykSystemPolicySetting(PantherRule):
     RuleID = "Snyk.System.PolicySetting-prototype"
     DisplayName = "Snyk System Policy Settings Changed"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects Snyk Policy Settings have been changed. Policies define Snyk's behavior when encountering security and licensing issues.\n"
     Runbook = "Snyk Policies can cause alerts to raise or not based on found security and license issues. Validate that that this change is expected.\n"
     Reference = "https://docs.snyk.io/manage-issues/policies/shared-policies-overview"
     SummaryAttributes = ["event"]
     Tests = snyk_system_policy_setting_tests
     ACTIONS = [
         "group.policy.create",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_sso.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_sso.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_system_sso_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk System SSO Setting event happened",
@@ -38,15 +38,15 @@
 
 
 class SnykSystemSSO(PantherRule):
     RuleID = "Snyk.System.SSO-prototype"
     DisplayName = "Snyk System SSO Settings Changed"
     LogTypes = [LogType.Snyk_GroupAudit]
     Tags = ["Snyk"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects Snyk SSO Settings have been changed. The reference URL from Snyk indicates that these events are likely to  originate exclusively from Snyk Support.\n"
     Reference = "https://docs.snyk.io/user-and-group-management/setting-up-sso-for-authentication/set-up-snyk-single-sign-on-sso"
     SummaryAttributes = ["event", "p_any_ip_addresses", "p_any_emails"]
     Tests = snyk_system_sso_tests
     ACTIONS = [
         "group.sso.auth0_connection.create",
         "group.sso.auth0_connection.edit",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_user_mgmt.py` & `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_user_mgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_snyk_helpers import snyk_alert_context
 from pypanther.log_types import LogType
 
 snyk_user_management_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Snyk User Removed",
@@ -82,15 +82,15 @@
 
 
 class SnykUserManagement(PantherRule):
     RuleID = "Snyk.User.Management-prototype"
     DisplayName = "Snyk User Management"
     LogTypes = [LogType.Snyk_GroupAudit, LogType.Snyk_OrgAudit]
     Tags = ["Snyk"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when Snyk Users are changed\n"
     Runbook = "These actions in the Snyk Audit logs indicate that a User has been created/deleted/modified.\n"
     Reference = "https://docs.snyk.io/snyk-admin/manage-users-and-permissions/member-roles"
     SummaryAttributes = ["event"]
     Tests = snyk_user_management_tests
     ACTIONS = [
         "group.user.add",
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/standard_rules/admin_assigned.py` & `pypanther-0.1.1a8/pypanther/rules/standard_rules/admin_assigned.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 standard_admin_role_assigned_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GCP - Admin Assigned",
         ExpectedResult=True,
         Log={
@@ -273,15 +273,15 @@
         LogType.GCP_AuditLog,
         LogType.GitHub_Audit,
         LogType.GSuite_Reports,
         LogType.OneLogin_Events,
         LogType.Zendesk_Audit,
     ]
     Tags = ["DataModel", "Privilege Escalation:Valid Accounts"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Reports = {"MITRE ATT&CK": ["TA0004:T1078"]}
     Description = "Assigning an admin role manually could be a sign of privilege escalation"
     Runbook = "Verify with the user who attached the role or add to a allowlist"
     Reference = "https://medium.com/@gokulelango1040/privilege-escalation-attacks-28a9ef226abb"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = standard_admin_role_assigned_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/standard_rules/brute_force_by_ip.py` & `pypanther-0.1.1a8/pypanther/rules/standard_rules/brute_force_by_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from json import loads
 from typing import List
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_default import lookup_aws_account_name
 from pypanther.helpers.panther_oss_helpers import add_parse_delay, geoinfo_from_ip
 from pypanther.log_types import LogType
 
 standard_brute_force_by_ip_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="AWS.CloudTrail - Successful Login",
@@ -396,15 +396,15 @@
         LogType.AWS_CloudTrail,
         LogType.Box_Event,
         LogType.GSuite_Reports,
         LogType.Okta_SystemLog,
         LogType.OneLogin_Events,
         LogType.OnePassword_SignInAttempt,
     ]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Tags = ["DataModel", "Credential Access:Brute Force"]
     Threshold = 20
     Reports = {"MITRE ATT&CK": ["TA0006:T1110"]}
     Description = "An actor user was denied login access more times than the configured threshold."
     Runbook = "Analyze the IP they came from, and other actions taken before/after. Check if a user from this ip eventually authenticated successfully."
     Reference = "https://owasp.org/www-community/controls/Blocking_Brute_Force_Attacks"
     SummaryAttributes = ["p_any_ip_addresses"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/standard_rules/impossible_travel_login.py` & `pypanther-0.1.1a8/pypanther/rules/standard_rules/impossible_travel_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime, timedelta
 from json import dumps, loads
 from typing import List
 
 from panther_detection_helpers.caching import get_string_set, put_string_set
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, RuleMock, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity, RuleMock
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_lookuptable_helpers import LookupTableMatches
 from pypanther.helpers.panther_oss_helpers import km_between_ipinfo_loc, resolve_timestamp_string
 from pypanther.log_types import LogType
 
 standard_impossible_travel_login_tests: List[PantherRuleTest] = [
     PantherRuleTest(
@@ -664,15 +664,15 @@
         LogType.Asana_Audit,
         LogType.AWS_CloudTrail,
         LogType.Notion_AuditLogs,
         LogType.Okta_SystemLog,
     ]
     Tags = ["Identity & Access Management", "Initial Access:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1078"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = (
         "A user has subsequent logins from two geographic locations that are very far apart"
     )
     Runbook = "Reach out to the user if needed to validate the activity, then lock the account. \nIf the user responds that the geolocation on the new location is incorrect, you can directly report the inaccuracy via  https://ipinfo.io/corrections\n"
     Reference = "https://expertinsights.com/insights/what-are-impossible-travel-logins/#:~:text=An%20impossible%20travel%20login%20is,of%20the%20logins%20is%20fraudulent"
     SummaryAttributes = ["p_any_usernames", "p_any_ip_addresses", "p_any_domain_names"]
     Tests = standard_impossible_travel_login_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py` & `pypanther-0.1.1a8/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import filter_crowdstrike_fdr_event_type
 from pypanther.log_types import LogType
 
 standard_malicious_ssodns_lookup_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Known Good SSO Domain",
         ExpectedResult=False,
@@ -173,15 +173,15 @@
     LogTypes = [
         LogType.CiscoUmbrella_DNS,
         LogType.Crowdstrike_DNSRequest,
         LogType.Crowdstrike_FDREvent,
         LogType.Suricata_DNS,
         LogType.Zeek_DNS,
     ]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Threshold = 1000
     Tags = ["Configuration Required"]
     Reports = {"MITRE ATT&CK": ["TA0001:T1566"]}
     Description = "The rule looks for DNS requests to sites potentially posing as SSO domains."
     Runbook = "Verify if the destination domain is owned by your organization."
     Reference = "https://www.cloudns.net/wiki/article/254/#:~:text=A%20DNS%20query%20(also%20known,associated%20with%20a%20domain%20name"
     SummaryAttributes = ["p_any_ip_addresses"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/standard_rules/mfa_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/standard_rules/mfa_disabled.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 standard_mfa_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="GitHub - Org MFA Disabled",
         ExpectedResult=True,
         Log={
@@ -205,15 +205,15 @@
         LogType.GitHub_Audit,
         LogType.Zendesk_Audit,
         LogType.Okta_SystemLog,
     ]
     Tags = ["DataModel", "Defense Evasion:Modify Authentication Process"]
     Reports = {"MITRE ATT&CK": ["TA0005:T1556"]}
     Reference = "https://en.wikipedia.org/wiki/Multi-factor_authentication"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when Multi-Factor Authentication (MFA) is disabled"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = standard_mfa_disabled_tests
 
     def rule(self, event):
         return event.udm("event_type") == event_type.MFA_DISABLED
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/standard_rules/standard_dns_base64.py` & `pypanther-0.1.1a8/pypanther/rules/standard_rules/standard_dns_base64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import defang_ioc, is_base64
 from pypanther.log_types import LogType
 
 standard_dns_base64_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="AWS VPC DNS (Positive)",
         ExpectedResult=True,
@@ -217,15 +217,15 @@
 
 class StandardDNSBase64(PantherRule):
     DisplayName = "DNS Base64 Encoded Query"
     Description = "Detects DNS queries with Base64 encoded subdomains, which could indicate an attempt to obfuscate data exfil."
     RuleID = "Standard.DNSBase64-prototype"
     Enabled = False
     Reference = "https://zofixer.com/what-is-base64-disclosure-vulnerability/"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Crowdstrike_FDREvent, LogType.AWS_VPCDns, LogType.CiscoUmbrella_DNS]
     Tests = standard_dns_base64_tests
     DECODED = ""
 
     def rule(self, event):
         args = event.udm("dns_query").split(".")
         # Check if Base64 encoded arguments are present in the command line
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_https_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_https_disabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tailscale_helpers import (
     is_tailscale_admin_console_event,
     tailscale_alert_context,
 )
 from pypanther.log_types import LogType
 
@@ -81,15 +81,15 @@
 
 
 class TailscaleHTTPSDisabled(PantherRule):
     Description = "A Tailscale User disabled HTTPS settings in your organization's tenant."
     DisplayName = "Tailscale HTTPS Disabled"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant to re-enable this setting as it's in the best security interest for your organization's security posture."
     Reference = "https://tailscale.com/kb/1153/enabling-https/#disable-https"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Tailscale_Audit]
     RuleID = "Tailscale.HTTPS.Disabled-prototype"
     Tests = tailscale_https_disabled_tests
 
     def rule(self, event):
         action = deep_get(event, "event", "action", default="<NO_ACTION_FOUND>")
         target_property = deep_get(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tailscale_helpers import (
     is_tailscale_admin_console_event,
     tailscale_alert_context,
 )
 from pypanther.log_types import LogType
 
@@ -82,15 +82,15 @@
 
 
 class TailscaleMachineApprovalRequirementsDisabled(PantherRule):
     Description = "A Tailscale User disabled machine approval requirement settings in your organization's tenant. This means devices can access your network without requiring approval."
     DisplayName = "Tailscale Machine Approval Requirements Disabled"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant to re-enable this setting as it's in the best security interest for your organization's security posture."
     Reference = "https://tailscale.com/kb/1099/device-approval/"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Tailscale_Audit]
     RuleID = "Tailscale.Machine.Approval.Requirements.Disabled-prototype"
     Tests = tailscale_machine_approval_requirements_disabled_tests
 
     def rule(self, event):
         action = deep_get(event, "event", "action", default="<NO_ACTION_FOUND>")
         target_property = deep_get(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tailscale_helpers import (
     is_tailscale_admin_console_event,
     tailscale_alert_context,
 )
 from pypanther.log_types import LogType
 
@@ -81,15 +81,15 @@
 
 
 class TailscaleMagicDNSDisabled(PantherRule):
     Description = "A Tailscale User disabled magic dns settings in your organization's tenant."
     DisplayName = "Tailscale Magic DNS Disabled"
     Runbook = "Assess if this was done by the user for a valid business reason. Be vigilant to re-enable this setting as it's in the best security interest for your organization's security posture."
     Reference = "https://tailscale.com/kb/1081/magicdns/"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     LogTypes = [LogType.Tailscale_Audit]
     RuleID = "Tailscale.Magic.DNS.Disabled-prototype"
     Tests = tailscale_magic_dns_disabled_tests
 
     def rule(self, event):
         action = deep_get(event, "event", "action", default="<NO_ACTION_FOUND>")
         target_property = deep_get(
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_actions_disabled_changes.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_actions_disabled_changes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_actions_disabled_changes_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Tines Actions Disabled Change",
@@ -41,15 +41,15 @@
 
 class TinesActionsDisabledChanges(PantherRule):
     RuleID = "Tines.Actions.DisabledChanges-prototype"
     DisplayName = "Tines Actions Disabled Change"
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines"]
     Reference = "https://www.tines.com/university/tines-basics/architecture-of-an-action"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detections when Tines Actions are set to Disabled Change\n"
     SummaryAttributes = ["user_id", "operation_name", "tenant_id", "request_ip"]
     Tests = tines_actions_disabled_changes_tests
     ACTIONS = ["ActionsDisabledChange"]
 
     def rule(self, event):
         action = deep_get(event, "operation_name", default="<NO_OPERATION_NAME>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_custom_ca.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_custom_ca.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_custom_certificate_authority_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Tines Login",
@@ -42,15 +42,15 @@
 
 class TinesCustomCertificateAuthority(PantherRule):
     RuleID = "Tines.Custom.CertificateAuthority-prototype"
     DisplayName = "Tines Custom CertificateAuthority setting changed"
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines", "IAM - Credential Security"]
     Reference = "https://www.tines.com/docs/admin/custom-certificate-authority"
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when Tines Custom CertificateAuthority settings are changed\n"
     SummaryAttributes = ["user_id", "operation_name", "tenant_id", "request_ip"]
     Tests = tines_custom_certificate_authority_tests
     ACTIONS = ["CustomCertificateAuthoritySet"]
 
     def rule(self, event):
         action = deep_get(event, "operation_name", default="<NO_OPERATION_NAME>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_enqueued_retrying_job_destruction_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Trigger - JobsQueuedDeletion",
@@ -58,15 +58,15 @@
 
 
 class TinesEnqueuedRetryingJobDestruction(PantherRule):
     RuleID = "Tines.Enqueued.Retrying.Job.Destruction-prototype"
     DisplayName = "Tines Enqueued/Retrying Job Deletion"
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Currently enqueued or retrying jobs were cleared"
     Runbook = "Possible data destruction. Please reach out to the user and confirm this was done for valid business reasons."
     Reference = "https://www.tines.com/docs/self-hosting/job-management"
     Tests = tines_enqueued_retrying_job_destruction_tests
 
     def rule(self, event):
         return deep_get(event, "operation_name", default="<NO_OPERATION_NAME>") in [
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_global_resource_destruction.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_global_resource_destruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_global_resource_destruction_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Detection Trigger",
@@ -43,15 +43,15 @@
 
 class TinesGlobalResourceDestruction(PantherRule):
     RuleID = "Tines.Global.Resource.Destruction-prototype"
     DisplayName = "Tines Global Resource Destruction"
     SummaryAttributes = ["user_id", "operation_name", "tenant_id", "request_ip"]
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A Tines user has destroyed a global resource."
     Runbook = "Possible data destruction. Please reach out to the user and confirm this was done for valid business reasons."
     Reference = "https://www.tines.com/docs/resources"
     Tests = tines_global_resource_destruction_tests
 
     def rule(self, event):
         return (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_sso_settings.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_sso_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_sso_settings_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Tines SsoConfigurationSamlSet",
@@ -46,15 +46,15 @@
 
 
 class TinesSSOSettings(PantherRule):
     RuleID = "Tines.SSO.Settings-prototype"
     DisplayName = "Tines SSO Settings"
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines", "IAM - Credential Security"]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "Detects when Tines SSO settings are changed\n"
     Reference = "https://www.tines.com/docs/admin/single-sign-on"
     SummaryAttributes = ["user_id", "operation_name", "tenant_id", "request_ip"]
     Tests = tines_sso_settings_tests
     ACTIONS = ["SsoConfigurationDefaultSet", "SsoConfigurationOidcSet", "SsoConfigurationSamlSet"]
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_story_items_destruction.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_story_items_destruction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_story_items_destruction_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Detection Trigger",
@@ -42,15 +42,15 @@
 
 
 class TinesStoryItemsDestruction(PantherRule):
     RuleID = "Tines.Story.Items.Destruction-prototype"
     DisplayName = "Tines Story Items Destruction"
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines"]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A user has destroyed a story item"
     Runbook = "Possible data destruction. Please reach out to the user and confirm this was done for valid business reasons."
     Reference = "https://www.tines.com/docs/stories"
     Tests = tines_story_items_destruction_tests
 
     def rule(self, event):
         return (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_story_jobs_clearance.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_story_jobs_clearance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_story_jobs_clearance_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Detection Trigger",
@@ -42,15 +42,15 @@
 
 
 class TinesStoryJobsClearance(PantherRule):
     RuleID = "Tines.Story.Jobs.Clearance-prototype"
     DisplayName = "Tines Story Jobs Clearance"
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A Tines User has cleared story jobs."
     Runbook = "Possible data destruction. Please reach out to the user and confirm this was done for valid business reasons."
     Reference = "https://www.tines.com/docs/stories"
     Tests = tines_story_jobs_clearance_tests
 
     def rule(self, event):
         return (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_team_destruction.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_team_destruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_team_destruction_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Detection Trigger",
@@ -42,15 +42,15 @@
 
 
 class TinesTeamDestruction(PantherRule):
     RuleID = "Tines.Team.Destruction-prototype"
     DisplayName = "Tines Team Destruction"
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "A user has destroyed a team"
     Runbook = "Possible data destruction. Please reach out to the user and confirm this was done for valid business reasons."
     Reference = "https://www.tines.com/docs/admin/teams"
     Tests = tines_team_destruction_tests
 
     def rule(self, event):
         return deep_get(event, "operation_name", default="<NO_OPERATION_NAME>") == "TeamDestruction"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_tenant_authtoken.py` & `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_tenant_authtoken.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import deep_get
 from pypanther.helpers.panther_tines_helpers import tines_alert_context
 from pypanther.log_types import LogType
 
 tines_tenant_auth_token_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Tines Login",
@@ -57,15 +57,15 @@
 
 
 class TinesTenantAuthToken(PantherRule):
     RuleID = "Tines.Tenant.AuthToken-prototype"
     DisplayName = "Tines Tenant API Keys Added"
     LogTypes = [LogType.Tines_Audit]
     Tags = ["Tines", "IAM - Credential Security"]
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "Detects when Tines Tenant API Keys are added\n"
     Reference = "https://www.tines.com/api/authentication"
     SummaryAttributes = ["user_id", "operation_name", "tenant_id", "request_ip"]
     Tests = tines_tenant_auth_token_tests
     # AuthenticationTokenDeletion does not include
     #  the scope of the deleted token.
     # Leaving deletion un-implemented for now
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py` & `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import ZENDESK_CHANGE_DESCRIPTION
 from pypanther.log_types import LogType
 
 zendesk_mobile_app_access_updated_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Zendesk - Mobile App Access Off",
         ExpectedResult=True,
@@ -67,15 +67,15 @@
 
 class ZendeskMobileAppAccessUpdated(PantherRule):
     RuleID = "Zendesk.MobileAppAccessUpdated-prototype"
     DisplayName = "Zendesk Mobile App Access Modified"
     LogTypes = [LogType.Zendesk_Audit]
     Tags = ["Zendesk", "Persistence:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0003:T1078"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "A user updated account setting that enabled or disabled mobile app access."
     Reference = "https://support.zendesk.com/hc/en-us/articles/4408846407066-About-the-Zendesk-Support-mobile-app#:~:text=More%20settings.-,Configuring%20the%20mobile%20app,-Activate%20the%20new"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = zendesk_mobile_app_access_updated_tests
     MOBILE_APP_ACTIONS = {"create", "update"}
 
     def rule(self, event):
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_new_api_token.py` & `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_new_api_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zendesk_new_api_token_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Zendesk - API Token Updated",
         ExpectedResult=False,
         Log={
@@ -45,15 +45,15 @@
 ]
 
 
 class ZendeskNewAPIToken(PantherRule):
     RuleID = "Zendesk.NewAPIToken-prototype"
     DisplayName = "Zendesk API Token Created"
     LogTypes = [LogType.Zendesk_Audit]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["Zendesk", "Credential Access:Steal Application Access Token"]
     Reports = {"MITRE ATT&CK": ["TA0006:T1528"]}
     Description = "A user created a new API token to be used with Zendesk."
     Runbook = "Validate the api token was created for valid use case, otherwise delete the token immediately."
     Reference = "https://support.zendesk.com/hc/en-us/articles/4408889192858-Managing-access-to-the-Zendesk-API#topic_bsw_lfg_mmb:~:text=enable%20token%20access.-,Generating%20API%20tokens,-To%20generate%20an"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = zendesk_new_api_token_tests
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_new_owner.py` & `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_new_owner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import ZENDESK_CHANGE_DESCRIPTION
 from pypanther.log_types import LogType
 
 zendesk_account_owner_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Zendesk - Owner Changed",
         ExpectedResult=True,
@@ -47,15 +47,15 @@
 ]
 
 
 class ZendeskAccountOwnerChanged(PantherRule):
     RuleID = "Zendesk.AccountOwnerChanged-prototype"
     DisplayName = "Zendesk Account Owner Changed"
     LogTypes = [LogType.Zendesk_Audit]
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Tags = ["Zendesk", "Privilege Escalation:Valid Accounts"]
     Reports = {"MITRE ATT&CK": ["TA0004:T1078"]}
     Description = (
         "Only one admin user can be the account owner. Ensure the change in ownership is expected."
     )
     Reference = (
         "https://support.zendesk.com/hc/en-us/articles/4408822084634-Changing-the-account-owner"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py` & `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import ZENDESK_CHANGE_DESCRIPTION
 from pypanther.log_types import LogType
 
 zendesk_sensitive_data_redaction_off_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Zendesk - Credit Card Redaction Off",
         ExpectedResult=True,
@@ -66,15 +66,15 @@
 
 class ZendeskSensitiveDataRedactionOff(PantherRule):
     RuleID = "Zendesk.SensitiveDataRedactionOff-prototype"
     DisplayName = "Zendesk Credit Card Redaction Off"
     LogTypes = [LogType.Zendesk_Audit]
     Tags = ["Zendesk", "Collection:Data from Information Repositories"]
     Reports = {"MITRE ATT&CK": ["TA0009:T1213"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A user updated account setting that disabled credit card redaction."
     Runbook = "Re-enable credit card redaction."
     Reference = "https://support.zendesk.com/hc/en-us/articles/4408822124314-Automatically-redacting-credit-card-numbers-from-tickets"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = zendesk_sensitive_data_redaction_off_tests
     REDACTION_ACTIONS = {"create", "destroy"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_assumption.py` & `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_assumption.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zendesk_user_assumption_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="User assumption settings changed",
         ExpectedResult=True,
         Log={
@@ -47,15 +47,15 @@
 
 class ZendeskUserAssumption(PantherRule):
     RuleID = "Zendesk.UserAssumption-prototype"
     DisplayName = "Enabled Zendesk Support to Assume Users"
     LogTypes = [LogType.Zendesk_Audit]
     Tags = ["Zendesk", "Lateral Movement:Use Alternate Authentication Material"]
     Reports = {"MITRE ATT&CK": ["TA0008:T1550"]}
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     Description = "User enabled or disabled zendesk support user assumption."
     Runbook = "Investigate whether allowing zendesk support to assume users is necessary. If not, disable the feature.\n"
     Reference = "https://support.zendesk.com/hc/en-us/articles/4408894200474-Assuming-end-users#:~:text=In%20Support%2C%20click%20the%20Customers,user%20in%20the%20information%20dialog"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = zendesk_user_assumption_tests
     USER_SUSPENSION_ACTIONS = {"create", "update"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_role.py` & `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import pypanther.helpers.panther_event_type_helpers as event_type
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import zendesk_get_roles
 from pypanther.log_types import LogType
 
 zendesk_user_role_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Zendesk - Role Changed",
         ExpectedResult=True,
@@ -47,15 +47,15 @@
 ]
 
 
 class ZendeskUserRoleChanged(PantherRule):
     RuleID = "Zendesk.UserRoleChanged-prototype"
     DisplayName = "Zendesk User Role Changed"
     LogTypes = [LogType.Zendesk_Audit]
-    Severity = Severity.Info
+    Severity = PantherSeverity.Info
     Description = "A user's Zendesk role was changed"
     Reference = "https://support.zendesk.com/hc/en-us/articles/4408824375450-Setting-roles-and-access-in-Zendesk-Admin-Center"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = zendesk_user_role_changed_tests
 
     def rule(self, event):
         if event.get("source_type") == "user" and event.get("action") == "update":
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_suspension.py` & `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_suspension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_base_helpers import ZENDESK_CHANGE_DESCRIPTION
 from pypanther.log_types import LogType
 
 zendesk_user_suspension_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Zendesk - Suspension Enabled",
         ExpectedResult=True,
@@ -67,15 +67,15 @@
 
 class ZendeskUserSuspension(PantherRule):
     RuleID = "Zendesk.UserSuspension-prototype"
     DisplayName = "Zendesk User Suspension Status Changed"
     LogTypes = [LogType.Zendesk_Audit]
     Tags = ["Zendesk", "Impact:Account Access Removal"]
     Reports = {"MITRE ATT&CK": ["TA0040:T1531"]}
-    Severity = Severity.High
+    Severity = PantherSeverity.High
     Description = "A user's Zendesk suspension status was changed."
     Runbook = "Ensure the user's suspension status is appropriate."
     Reference = "https://support.zendesk.com/hc/en-us/articles/4408889293978-Suspending-a-user#:~:text=select%20Unsuspend%20access.-,Identifying%20suspended%20users,name%20on%20the%20Customers%20page"
     SummaryAttributes = ["p_any_ip_addresses"]
     Tests = zendesk_user_suspension_tests
     USER_SUSPENSION_ACTIONS = {"create", "update"}
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zoom_all_meetings_secured_with_one_option_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Turn off",
         ExpectedResult=True,
         Log={
@@ -40,15 +40,15 @@
 
 
 class ZoomAllMeetingsSecuredWithOneOptionDisabled(PantherRule):
     Description = "A Zoom User turned off your organization's requirement that all meetings are secured with one security option."
     DisplayName = "Zoom All Meetings Secured With One Option Disabled"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0059862"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Zoom_Operation]
     RuleID = "Zoom.All.Meetings.Secured.With.One.Option.Disabled-prototype"
     Tests = zoom_all_meetings_secured_with_one_option_disabled_tests
 
     def rule(self, event):
         operation_detail = event.get("operation_detail", "<NO_OPS_DETAIL>")
         operation_flag = (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zoom_automatic_sign_out_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Automatic Signout Setting Disabled",
         ExpectedResult=True,
         Log={
@@ -30,15 +30,15 @@
 
 
 class ZoomAutomaticSignOutDisabled(PantherRule):
     Description = "A Zoom User turned off your organization's setting to automatically sign users out after a specified period of time."
     DisplayName = "Zoom Automatic Sign Out Disabled"
     Reference = "https://support.zoom.us/hc/en-us/articles/115005756143-Changing-account-security-settings#:~:text=Users%20need%20to%20sign%20in,of%205%20to%20120%20minutes"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Zoom_Operation]
     RuleID = "Zoom.Automatic.Sign.Out.Disabled-prototype"
     Tests = zoom_automatic_sign_out_disabled_tests
 
     def rule(self, event):
         operation_detail = event.get("operation_detail", "<NO_OPS_DETAIL>")
         operation_flag = "Automatically sign users out after a specified time: from On to Off"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zoom_new_meeting_passcode_required_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Setting Turn Off",
         ExpectedResult=True,
         Log={
@@ -43,15 +43,15 @@
 class ZoomNewMeetingPasscodeRequiredDisabled(PantherRule):
     Description = (
         "A Zoom User turned off your organization's setting to require passcodes for new meetings."
     )
     DisplayName = "Zoom New Meeting Passcode Required Disabled"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0063160#:~:text=Since%20September%202022%2C%20Zoom%20requires,enforced%20for%20all%20free%20accounts"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Zoom_Operation]
     RuleID = "Zoom.New.Meeting.Passcode.Required.Disabled-prototype"
     Tests = zoom_new_meeting_passcode_required_disabled_tests
 
     def rule(self, event):
         operation_detail = event.get("operation_detail", "<NO_OPS_DETAIL>")
         operation_flag = (
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.helpers.panther_zoom_helpers import get_zoom_usergroup_context as get_context
 from pypanther.log_types import LogType
 
 zoom_passcode_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Meeting Passcode Disabled",
         ExpectedResult=True,
@@ -45,15 +45,15 @@
 
 
 class ZoomPasscodeDisabled(PantherRule):
     RuleID = "Zoom.PasscodeDisabled-prototype"
     DisplayName = "Zoom Meeting Passcode Disabled"
     LogTypes = [LogType.Zoom_Operation]
     Tags = ["Zoom", "Collection:Video Capture"]
-    Severity = Severity.Low
+    Severity = PantherSeverity.Low
     Description = "Meeting passcode requirement has been disabled from usergroup\n"
     Reports = {"MITRE ATT&CK": ["TA0009:T1125"]}
     Reference = (
         "https://support.zoom.us/hc/en-us/articles/360033559832-Zoom-Meeting-and-Webinar-passcodes"
     )
     Runbook = "Follow up with user or Zoom admin to ensure this meeting room's use case does not allow a passcode.\n"
     SummaryAttributes = ["p_any_emails"]
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py` & `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zoom_sign_in_method_modified_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Google",
         ExpectedResult=True,
         Log={
@@ -41,15 +41,15 @@
 
 
 class ZoomSignInMethodModified(PantherRule):
     Description = "A Zoom User modified your organizations sign in method."
     DisplayName = "Zoom Sign In Method Modified"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0067602#:~:text=Go%20to%20the%20Zoom%20site,click%20Link%20and%20Sign%20In"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Zoom_Operation]
     RuleID = "Zoom.Sign.In.Method.Modified-prototype"
     Tests = zoom_sign_in_method_modified_tests
 
     def rule(self, event):
         operation_detail = event.get("operation_detail", "<NO_OPS_DETAIL>")
         operation_flag = "Sign-in Methods  - Allow users to sign in with "
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py` & `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zoom_sign_in_requirements_changed_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Setting Change One",
         ExpectedResult=True,
         Log={
@@ -52,15 +52,15 @@
 
 
 class ZoomSignInRequirementsChanged(PantherRule):
     Description = "A Zoom User changed your organization's sign in requirements. "
     DisplayName = "Zoom Sign In Requirements Changed"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0061263"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Zoom_Operation]
     RuleID = "Zoom.Sign.In.Requirements.Changed-prototype"
     SummaryAttributes = ["operation_detail"]
     Tests = zoom_sign_in_requirements_changed_tests
 
     def rule(self, event):
         operation_detail = event.get("operation_detail", "<NO_OPS_DETAIL>")
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py` & `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zoom_two_factor_authentication_disabled_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="2FA Disabled",
         ExpectedResult=True,
         Log={
@@ -41,15 +41,15 @@
 
 
 class ZoomTwoFactorAuthenticationDisabled(PantherRule):
     Description = "A Zoom User disabled your organization's setting to sign in with Two-Factor Authentication."
     DisplayName = "Zoom Two Factor Authentication Disabled"
     Runbook = "Confirm this user acted with valid business intent and determine whether this activity was authorized."
     Reference = "https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0066054"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Zoom_Operation]
     RuleID = "Zoom.Two.Factor.Authentication.Disabled-prototype"
     Tests = zoom_two_factor_authentication_disabled_tests
 
     def rule(self, event):
         operation_detail = event.get("operation_detail", "<NO_OPS_DETAIL>")
         operation_flag = "Security  - Sign in with Two-Factor Authentication: from On to Off"
```

### Comparing `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py` & `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from pypanther.base import PantherRule, PantherRuleTest, Severity
+from pypanther.base import PantherRule, PantherRuleTest, PantherSeverity
 from pypanther.log_types import LogType
 
 zoom_user_promotedto_privileged_role_tests: List[PantherRuleTest] = [
     PantherRuleTest(
         Name="Admin Promotion Event",
         ExpectedResult=True,
         Log={
@@ -85,15 +85,15 @@
 ]
 
 
 class ZoomUserPromotedtoPrivilegedRole(PantherRule):
     Description = "A Zoom user was promoted to a privileged role."
     DisplayName = "Zoom User Promoted to Privileged Role"
     Reference = "https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0064983"
-    Severity = Severity.Medium
+    Severity = PantherSeverity.Medium
     LogTypes = [LogType.Zoom_Operation]
     RuleID = "Zoom.User.Promoted.to.Privileged.Role-prototype"
     Tests = zoom_user_promotedto_privileged_role_tests
     PRIVILEGED_ROLES = ("Admin", "Co-Owner", "Owner", "Billing Admin")
 
     def extract_values(self, event):
         operator = event.get("operator", "<operator-not-found>")
```

### Comparing `pypanther-0.1.1a3/pypanther/upload.py` & `pypanther-0.1.1a8/pypanther/upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from pypanther.vendor.panther_analysis_tool.constants import ENABLE_CORRELATION_RULES_FLAG
 from pypanther.vendor.panther_analysis_tool.util import convert_unicode
 
 IGNORE_FOLDERS = [".mypy_cache", "pypanther", "panther_analysis", ".git", "__pycache__"]
 
 
 def run(backend: BackendClient, args: argparse.Namespace) -> Tuple[int, str]:
-    use_async = (not args.no_async) and backend.supports_async_uploads()
     with tempfile.NamedTemporaryFile() as tmp:
         with zipfile.ZipFile(tmp, "w") as zip_out:
             logging.info(f"Writing to temporary zip file at {tmp.name}")
 
             for root, dir, files in os.walk("."):
                 for bad in IGNORE_FOLDERS:
                     if bad in dir:
@@ -43,20 +42,18 @@
 
                     filepath = os.path.join(root, file)
 
                     zip_out.write(
                         filepath,
                         arcname=filepath,
                     )
-        return upload_zip(backend, args, archive=tmp.name, use_async=use_async)
+        return upload_zip(backend, args, archive=tmp.name)
 
 
-def upload_zip(
-    backend: BackendClient, args: argparse.Namespace, archive: str, use_async: bool
-) -> Tuple[int, str]:
+def upload_zip(backend: BackendClient, args: argparse.Namespace, archive: str) -> Tuple[int, str]:
     # extract max retries we should handle
     max_retries = 10
     if args.max_retries > 10:
         logging.warning("max_retries cannot be greater than 10, defaulting to 10")
     elif args.max_retries < 0:
         logging.warning("max_retries cannot be negative, defaulting to 0")
         max_retries = 0
@@ -65,18 +62,15 @@
         logging.info("Uploading items to Panther")
 
         upload_params = BulkUploadParams(zip_bytes=analysis_zip.read())
         retry_count = 0
 
         while True:
             try:
-                if use_async:
-                    response = backend.async_bulk_upload(upload_params)
-                else:
-                    response = backend.bulk_upload(upload_params)
+                response = backend.async_bulk_upload(upload_params)
 
                 resp_dict = asdict(response.data)
                 flags_params = FeatureFlagsParams(
                     flags=[FeatureFlagWithDefault(flag=ENABLE_CORRELATION_RULES_FLAG)]
                 )
                 try:
                     if not backend.feature_flags(flags_params).data.flags[0].treatment:
```

### Comparing `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/client.py` & `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/errors.py` & `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/errors.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql` & `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql` & `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py` & `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/cli_output.py` & `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/cli_output.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/constants.py` & `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Final
 
 VERSION_STRING: Final = "0.48.0"
+CONFIG_FILE = ".panther_settings.yml"
 
 # The UserID is required by Panther for some API calls, but we have no way of
 # acquiring it, and it isn't used for anything. This is a valid UUID used by the
 # Panther deployment tool to indicate this action was performed automatically.
 PANTHER_USER_ID = "00000000-0000-4000-8000-000000000000"
```

### Comparing `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/util.py` & `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,18 +18,14 @@
 """
 
 import argparse
 import re
 from typing import Any, Callable, Tuple
 
 from pypanther.vendor.panther_analysis_tool.backend.client import Client as BackendClient
-from pypanther.vendor.panther_analysis_tool.backend.lambda_client import (
-    LambdaClient,
-    LambdaClientOpts,
-)
 from pypanther.vendor.panther_analysis_tool.backend.public_api_client import (
     PublicAPIClient,
     PublicAPIClientOptions,
 )
 from pypanther.vendor.panther_analysis_tool.constants import PANTHER_USER_ID
 
 UNKNOWN_VERSION = "unknown"
@@ -42,37 +38,20 @@
 def func_with_backend(
     func: Callable[[BackendClient, argparse.Namespace], Any]
 ) -> Callable[[argparse.Namespace], Tuple[int, str]]:
     return lambda args: func(get_backend(args), args)
 
 
 def get_backend(args: argparse.Namespace) -> BackendClient:
-    if args.api_token:
-        return PublicAPIClient(
-            PublicAPIClientOptions(
-                token=args.api_token, user_id=PANTHER_USER_ID, host=args.api_host
-            )
-        )
-
-    datalake_lambda = get_datalake_lambda(args)
-
-    return LambdaClient(
-        LambdaClientOpts(
-            user_id=PANTHER_USER_ID,
-            aws_profile=args.aws_profile,
-            datalake_lambda=datalake_lambda,
-        )
-    )
-
+    if not args.api_token:
+        raise BackendNotFoundException("API token is required")
 
-def get_datalake_lambda(args: argparse.Namespace) -> str:
-    if "athena_datalake" not in args:
-        return ""
-
-    return "panther-athena-api" if args.athena_datalake else "panther-snowflake-api"
+    return PublicAPIClient(
+        PublicAPIClientOptions(token=args.api_token, user_id=PANTHER_USER_ID, host=args.api_host)
+    )
 
 
 def convert_unicode(obj: Any) -> str:
     """Swap unicode 4 byte strings with arbitrary numbers of leading slashes with the actual character
     e.g. \\\\u003c => <"""
     string_to_convert = str(obj)
     return re.sub(r"\\*\\u([0-9a-f]{4})", lambda m: chr(int(m.group(1), 16)), string_to_convert)
```

### Comparing `pypanther-0.1.1a3/pyproject.toml` & `pypanther-0.1.1a8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "pypanther"
-version = "0.1.1a3"
+version = "0.1.1a8"
 description = ""
 authors = ["Panther Labs Inc <pypi@runpanther.io>"]
 readme = "README.md"
 keywords = ["Security", "CLI"]
-classifiers = [
-    "Operating System :: OS Independent",
-]
+classifiers = ["Operating System :: OS Independent"]
 license = "AGPL-3.0-only"
+include = ["pypanther/py.typed"]
 
 [tool.poetry.dependencies]
 python = "3.11.*"
 pydantic = "^2.7.1"
 ruamel-yaml = "^0.18.6"
 ast-comments = "^1.2.2"
 black = "^24.4.2"
 panther-detection-helpers = "^0.4.0"
 panther-core = "^0.10.0"
 boto3 = "^1.34.99"
 policyuniverse = "^1.5.1.20231109"
 jsonpath-ng = "^1.6.1"
 gql = "^3.5.0"
 aiohttp = "^3.9.5"
+dynaconf = "^3.2.5"
 
 [tool.poetry.scripts]
 pypanther = 'pypanther.main:run'
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.10.0"
 pre-commit = "^3.7.0"
@@ -41,17 +41,17 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 exclude = [
-    '^pypanther/rules/', 
-    '^pypanther/helpers/', 
-    '^pypanther/data_models/', 
+    '^pypanther/rules/',
+    '^pypanther/helpers/',
+    '^pypanther/data_models/',
 ]
 
 [[tool.mypy.overrides]]
 module = "panther_detection_helpers.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
@@ -73,12 +73,8 @@
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
-exclude = [
-    'pypanther/rules/', 
-    'pypanther/helpers/', 
-    'pypanther/data_models/', 
-]
+exclude = ['pypanther/rules/', 'pypanther/helpers/', 'pypanther/data_models/']
```

### Comparing `pypanther-0.1.1a3/PKG-INFO` & `pypanther-0.1.1a8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pypanther
-Version: 0.1.1a3
+Version: 0.1.1a8
 Summary: 
 License: AGPL-3.0-only
 Keywords: Security,CLI
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 Requires-Python: ==3.11.*
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: ast-comments (>=1.2.2,<2.0.0)
 Requires-Dist: black (>=24.4.2,<25.0.0)
 Requires-Dist: boto3 (>=1.34.99,<2.0.0)
+Requires-Dist: dynaconf (>=3.2.5,<4.0.0)
 Requires-Dist: gql (>=3.5.0,<4.0.0)
 Requires-Dist: jsonpath-ng (>=1.6.1,<2.0.0)
 Requires-Dist: panther-core (>=0.10.0,<0.11.0)
 Requires-Dist: panther-detection-helpers (>=0.4.0,<0.5.0)
 Requires-Dist: policyuniverse (>=1.5.1.20231109,<2.0.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: ruamel-yaml (>=0.18.6,<0.19.0)
```

